# Comparing `tmp/chess2vec-0.1.0a0.tar.gz` & `tmp/chess2vec-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.1.0a0.tar", max compression
+gzip compressed data, was "chess2vec-0.1.1a0.tar", max compression
```

## Comparing `chess2vec-0.1.0a0.tar` & `chess2vec-0.1.1a0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.0a0/README.md
--rw-r--r--   0        0        0     4611 2024-04-16 21:35:46.344565 chess2vec-0.1.0a0/chess2vec/__init__.py
--rw-r--r--   0        0        0     1910 2024-04-16 20:11:28.318615 chess2vec-0.1.0a0/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc
--rw-r--r--   0        0        0      740 2024-04-16 16:21:07.852284 chess2vec-0.1.0a0/chess2vec/_utils/sparse.py
--rw-r--r--   0        0        0      538 2024-04-16 16:46:49.087490 chess2vec-0.1.0a0/chess2vec/_utils/vector.py
--rw-r--r--   0        0        0      367 2024-04-16 21:41:59.702128 chess2vec-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 chess2vec-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.1a0/README.md
+-rw-r--r--   0        0        0     5849 2024-04-17 19:45:16.721711 chess2vec-0.1.1a0/chess2vec/__init__.py
+-rw-r--r--   0        0        0     1910 2024-04-16 20:11:28.318615 chess2vec-0.1.1a0/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc
+-rw-r--r--   0        0        0      740 2024-04-16 16:21:07.852284 chess2vec-0.1.1a0/chess2vec/_utils/sparse.py
+-rw-r--r--   0        0        0      538 2024-04-16 16:46:49.087490 chess2vec-0.1.1a0/chess2vec/_utils/vector.py
+-rw-r--r--   0        0        0      367 2024-04-17 19:48:27.363534 chess2vec-0.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 chess2vec-0.1.1a0/PKG-INFO
```

### Comparing `chess2vec-0.1.0a0/chess2vec/__init__.py` & `chess2vec-0.1.1a0/chess2vec/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,87 +1,144 @@
-from typing import Iterable
+from typing import Iterable, TextIO, Callable
 
 import chess
 import chess.pgn
 import numpy as np
 import scipy.sparse
 from alive_progress import alive_bar
 
 import chess2vec._utils.sparse as spu
 
 VEC_BLOCK = 64 * 64
 VEC_SIZE = 5 * VEC_BLOCK
 
 
+from time import perf_counter
+
+def timeit(func: Callable, *args, **kwargs):
+    time_start = perf_counter()
+    result = func(*args, **kwargs)
+    time_end = perf_counter()
+    print(f"{func.__name__}: {(time_end - time_start):.8f}")
+    return result
+
+
+class csr_matrix_builder:
+    def __init__(self):
+        self.data = []
+        self.rows = []
+        self.columns = []
+
+    def add_entry(self, rows, columns, data=None):
+        self.columns += columns
+        
+        if isinstance(rows, int):
+            rows = [rows for _ in range(len(columns))]
+        
+        self.rows += rows
+
+        if data is None:
+            data = [1 for _ in range(len(rows))]
+
+        self.data += data
+
+    def build(self, shape):
+        return scipy.sparse.csr_matrix(
+            [self.data, (self.rows, self.columns)], shape=shape
+        )
+
+
+def _actions(board: chess.Board):
+    for move in board.legal_moves:
+        pt = board.piece_type_at(move.from_square)
+
+        if not board.turn:
+            move.from_square ^= 0x38
+            move.to_square ^= 0x38
+
+        idx = 64 * move.from_square + move.to_square
+
+        match pt:
+            case chess.QUEEN:
+                yield from (VEC_BLOCK * 2 + idx, VEC_BLOCK * 3 + idx)
+            case chess.KING:
+                yield VEC_BLOCK * 4 + idx
+            case _:
+                yield VEC_BLOCK * (pt - 1) + idx
+
+
 class PositionEncoder:
     def __init__(self) -> None:
         self.positions = []
         self._actions_matrix = scipy.sparse.csr_matrix((0, VEC_SIZE), dtype=np.uint8)
 
+    def _load_indices(self, rows, columns):
+        mat = scipy.sparse.csr_matrix(
+            (
+                np.ones_like(columns, dtype=np.uint8),
+                (rows, columns),
+            ),
+            shape=(int(np.max(rows)) + 1, VEC_SIZE),
+        )
+
+        self._actions_matrix = scipy.sparse.vstack([self._actions_matrix, mat])
+
     def load_fen(self, x: Iterable[str]):
         rows, columns = [], []
         row_idx = 0
 
         for fen in x:
             board = chess.Board(fen)
-            
-            for move in board.legal_moves:
-                pt = board.piece_type_at(move.from_square)
 
-                if not board.turn:
-                    move.from_square ^= 0x38
-                    move.to_square ^= 0x38
-
-                idx = 64 * move.from_square + move.to_square
-
-                match pt:
-                    case chess.QUEEN:
-                        columns += [VEC_BLOCK * 2 + idx, VEC_BLOCK * 3 + idx]
-                        rows += [row_idx, row_idx]
-                    case chess.KING:
-                        columns.append(VEC_BLOCK * 4 + idx)
-                        rows.append(row_idx)
-                    case _:
-                        columns.append(VEC_BLOCK * (pt - 1) + idx)
-                        rows.append(row_idx)
+            actions = list(_actions(board))
+            columns += actions
+            rows += [row_idx for _ in range(len(actions))]
 
             row_idx += 1
 
-        mat = scipy.sparse.csr_matrix(
-            (
-                np.ones_like(columns, dtype=np.uint8),
-                (rows, columns),
-            ),
-            shape=(row_idx, VEC_SIZE),
-        )
-
-        self._actions_matrix = scipy.sparse.vstack([self._actions_matrix, mat])
+        self._load_indices(rows, columns)
         self.positions += list(x)
 
-    def load_pgn(self, x: Iterable[str]):
+    def load_pgn(self, x: TextIO, max_games: int = None):
+        if max_games <= 0:
+            return
+
+        if max_games is None:
+            max_games = float("inf")
+            
+        builder = csr_matrix_builder()
         positions = []
+        idx = num_game = 0
         
         with alive_bar() as bar:
-            for file in x:
-                with open(file) as pgn:
-                    game = chess.pgn.read_game(pgn)
-
-                    while game:
-                        board = game.board()
-                        bar()
-                        
-                        positions += [board.fen()] + [
-                            board.push(move) or bar() or board.fen()
-                            for move in game.mainline_moves()
-                        ]
-                        
-                        game = chess.pgn.read_game(pgn)
-                        
-                    if len(positions) > 128_000:
-                        self.load_fen(positions)
+            game = chess.pgn.read_game(x)
+
+            while game and num_game < max_games:                    
+                board = game.board()
+
+                builder.add_entry(idx, list(_actions(board)))
+                positions.append(board.fen())
+                
+                idx += 1
+                bar()
+
+                for move in game.mainline_moves():
+                    board.push(move)
+
+                    builder.add_entry(idx, list(_actions(board)))
+                    positions.append(board.fen())
+                    
+                    idx += 1
+                    bar()
+
+                game = chess.pgn.read_game(x)
+                num_game += 1
+                    
+        self._actions_matrix = scipy.sparse.vstack([self._actions_matrix, builder.build((idx, VEC_SIZE))])
+        self.positions += positions
 
     def load_npz(self, x: Iterable[str]):
         for file in x:
             with np.load(file) as loaded:
                 indices = loaded["mat_indices"]
                 mat = scipy.sparse.csr_matrix(
                     (
```

### Comparing `chess2vec-0.1.0a0/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc` & `chess2vec-0.1.1a0/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.0a0/chess2vec/_utils/sparse.py` & `chess2vec-0.1.1a0/chess2vec/_utils/sparse.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.0a0/chess2vec/_utils/vector.py` & `chess2vec-0.1.1a0/chess2vec/_utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.0a0/PKG-INFO` & `chess2vec-0.1.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.1.0a0
+Version: 0.1.1a0
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

