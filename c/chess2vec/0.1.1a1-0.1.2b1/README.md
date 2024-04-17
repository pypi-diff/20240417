# Comparing `tmp/chess2vec-0.1.1a1.tar.gz` & `tmp/chess2vec-0.1.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.1.1a1.tar", max compression
+gzip compressed data, was "chess2vec-0.1.2b1.tar", max compression
```

## Comparing `chess2vec-0.1.1a1.tar` & `chess2vec-0.1.2b1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.1a1/README.md
--rw-r--r--   0        0        0     5610 2024-04-17 20:33:25.778470 chess2vec-0.1.1a1/chess2vec/__init__.py
--rw-r--r--   0        0        0     1910 2024-04-16 20:11:28.318615 chess2vec-0.1.1a1/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc
--rw-r--r--   0        0        0      740 2024-04-16 16:21:07.852284 chess2vec-0.1.1a1/chess2vec/_utils/sparse.py
--rw-r--r--   0        0        0      538 2024-04-16 16:46:49.087490 chess2vec-0.1.1a1/chess2vec/_utils/vector.py
--rw-r--r--   0        0        0      367 2024-04-17 20:33:33.613573 chess2vec-0.1.1a1/pyproject.toml
--rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 chess2vec-0.1.1a1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.2b1/README.md
+-rw-r--r--   0        0        0     5511 2024-04-17 20:58:35.876387 chess2vec-0.1.2b1/chess2vec/__init__.py
+-rw-r--r--   0        0        0     1910 2024-04-16 20:11:28.318615 chess2vec-0.1.2b1/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc
+-rw-r--r--   0        0        0      740 2024-04-16 16:21:07.852284 chess2vec-0.1.2b1/chess2vec/_utils/sparse.py
+-rw-r--r--   0        0        0      538 2024-04-16 16:46:49.087490 chess2vec-0.1.2b1/chess2vec/_utils/vector.py
+-rw-r--r--   0        0        0      367 2024-04-17 20:58:52.362764 chess2vec-0.1.2b1/pyproject.toml
+-rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 chess2vec-0.1.2b1/PKG-INFO
```

### Comparing `chess2vec-0.1.1a1/chess2vec/__init__.py` & `chess2vec-0.1.2b1/chess2vec/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Iterable, TextIO, Callable
+from typing import Iterable, TextIO
 
 import chess
 import chess.pgn
 import numpy as np
 import scipy.sparse
 from alive_progress import alive_bar
 
@@ -16,28 +16,28 @@
     def __init__(self):
         self.data = []
         self.rows = []
         self.columns = []
 
     def add_entry(self, rows, columns, data=None):
         self.columns += columns
-        
+
         if isinstance(rows, int):
             rows = [rows for _ in range(len(columns))]
-        
+
         self.rows += rows
 
         if data is None:
             data = [1 for _ in range(len(rows))]
 
         self.data += data
 
-    def build(self, shape):
+    def build(self, shape, dtype=np.float32):
         return scipy.sparse.csr_matrix(
-            (self.data, (self.rows, self.columns)), shape=shape, dtype=np.uin8
+            (self.data, (self.rows, self.columns)), shape=shape, dtype=dtype
         )
 
 
 def _actions(board: chess.Board):
     for move in board.legal_moves:
         pt = board.piece_type_at(move.from_square)
 
@@ -90,44 +90,46 @@
 
     def load_pgn(self, x: TextIO, max_games: int = None):
         if max_games <= 0:
             return
 
         if max_games is None:
             max_games = float("inf")
-            
+
         builder = csr_matrix_builder()
         positions = []
         idx = num_game = 0
-        
+
         with alive_bar() as bar:
             game = chess.pgn.read_game(x)
 
-            while game and num_game < max_games:                    
+            while game and num_game < max_games:
                 board = game.board()
 
                 builder.add_entry(idx, list(_actions(board)))
                 positions.append(board.fen())
-                
+
                 idx += 1
-                bar()
 
                 for move in game.mainline_moves():
                     board.push(move)
 
                     builder.add_entry(idx, list(_actions(board)))
                     positions.append(board.fen())
-                    
+
                     idx += 1
-                    bar()
+
+                bar()
 
                 game = chess.pgn.read_game(x)
                 num_game += 1
-                    
-        self._actions_matrix = scipy.sparse.vstack([self._actions_matrix, builder.build((idx, VEC_SIZE))])
+
+        self._actions_matrix = scipy.sparse.vstack(
+            [self._actions_matrix, builder.build((idx, VEC_SIZE), np.uint8)]
+        )
         self.positions += positions
 
     def load_npz(self, x: Iterable[str]):
         for file in x:
             with np.load(file) as loaded:
                 indices = loaded["mat_indices"]
                 mat = scipy.sparse.csr_matrix(
```

### Comparing `chess2vec-0.1.1a1/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc` & `chess2vec-0.1.2b1/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.1a1/chess2vec/_utils/sparse.py` & `chess2vec-0.1.2b1/chess2vec/_utils/sparse.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.1a1/chess2vec/_utils/vector.py` & `chess2vec-0.1.2b1/chess2vec/_utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.1a1/PKG-INFO` & `chess2vec-0.1.2b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.1.1a1
+Version: 0.1.2b1
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

