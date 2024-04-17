# Comparing `tmp/chess2vec-0.1.3b1.tar.gz` & `tmp/chess2vec-0.1.3b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.1.3b1.tar", max compression
+gzip compressed data, was "chess2vec-0.1.3b2.tar", max compression
```

## Comparing `chess2vec-0.1.3b1.tar` & `chess2vec-0.1.3b2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.3b1/README.md
--rw-r--r--   0        0        0     5660 2024-04-17 21:13:49.266134 chess2vec-0.1.3b1/chess2vec/__init__.py
--rw-r--r--   0        0        0     1910 2024-04-16 20:11:28.318615 chess2vec-0.1.3b1/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc
--rw-r--r--   0        0        0      740 2024-04-16 16:21:07.852284 chess2vec-0.1.3b1/chess2vec/_utils/sparse.py
--rw-r--r--   0        0        0      538 2024-04-16 16:46:49.087490 chess2vec-0.1.3b1/chess2vec/_utils/vector.py
--rw-r--r--   0        0        0      358 2024-04-17 21:13:57.952971 chess2vec-0.1.3b1/pyproject.toml
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 chess2vec-0.1.3b1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.3b2/README.md
+-rw-r--r--   0        0        0     5567 2024-04-17 21:14:59.114117 chess2vec-0.1.3b2/chess2vec/__init__.py
+-rw-r--r--   0        0        0     1910 2024-04-16 20:11:28.318615 chess2vec-0.1.3b2/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc
+-rw-r--r--   0        0        0      740 2024-04-16 16:21:07.852284 chess2vec-0.1.3b2/chess2vec/_utils/sparse.py
+-rw-r--r--   0        0        0      538 2024-04-16 16:46:49.087490 chess2vec-0.1.3b2/chess2vec/_utils/vector.py
+-rw-r--r--   0        0        0      358 2024-04-17 21:15:13.984382 chess2vec-0.1.3b2/pyproject.toml
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 chess2vec-0.1.3b2/PKG-INFO
```

### Comparing `chess2vec-0.1.3b1/chess2vec/__init__.py` & `chess2vec-0.1.3b2/chess2vec/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,38 +98,37 @@
         builder = csr_matrix_builder()
         positions = []
         idx = num_game = 0
         
         if status:
             bar = tqdm()
 
-        with alive_bar() as bar:
-            game = chess.pgn.read_game(x)
+        game = chess.pgn.read_game(x)
 
-            while game and num_game < max_games:
-                board = game.board()
+        while game and num_game < max_games:
+            board = game.board()
 
-                builder.add_entry(idx, list(_actions(board)))
-                positions.append(board.fen())
+            builder.add_entry(idx, list(_actions(board)))
+            positions.append(board.fen())
 
-                idx += 1
+            idx += 1
 
-                for move in game.mainline_moves():
-                    board.push(move)
+            for move in game.mainline_moves():
+                board.push(move)
 
-                    builder.add_entry(idx, list(_actions(board)))
-                    positions.append(board.fen())
+                builder.add_entry(idx, list(_actions(board)))
+                positions.append(board.fen())
 
-                    idx += 1
+                idx += 1
 
-                if status:
-                    bar.update(1)
+            if status:
+                bar.update(1)
 
-                game = chess.pgn.read_game(x)
-                num_game += 1
+            game = chess.pgn.read_game(x)
+            num_game += 1
 
         self._actions_matrix = scipy.sparse.vstack(
             [self._actions_matrix, builder.build((idx, VEC_SIZE), np.uint8)]
         )
         self.positions += positions
         
         if status:
```

### Comparing `chess2vec-0.1.3b1/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc` & `chess2vec-0.1.3b2/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.3b1/chess2vec/_utils/sparse.py` & `chess2vec-0.1.3b2/chess2vec/_utils/sparse.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.3b1/chess2vec/_utils/vector.py` & `chess2vec-0.1.3b2/chess2vec/_utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.3b1/PKG-INFO` & `chess2vec-0.1.3b2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.1.3b1
+Version: 0.1.3b2
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

