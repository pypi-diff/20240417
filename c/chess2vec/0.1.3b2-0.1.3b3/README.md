# Comparing `tmp/chess2vec-0.1.3b2.tar.gz` & `tmp/chess2vec-0.1.3b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.1.3b2.tar", max compression
+gzip compressed data, was "chess2vec-0.1.3b3.tar", max compression
```

## Comparing `chess2vec-0.1.3b2.tar` & `chess2vec-0.1.3b3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.3b2/README.md
--rw-r--r--   0        0        0     5567 2024-04-17 21:14:59.114117 chess2vec-0.1.3b2/chess2vec/__init__.py
--rw-r--r--   0        0        0     1910 2024-04-16 20:11:28.318615 chess2vec-0.1.3b2/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc
--rw-r--r--   0        0        0      740 2024-04-16 16:21:07.852284 chess2vec-0.1.3b2/chess2vec/_utils/sparse.py
--rw-r--r--   0        0        0      538 2024-04-16 16:46:49.087490 chess2vec-0.1.3b2/chess2vec/_utils/vector.py
--rw-r--r--   0        0        0      358 2024-04-17 21:15:13.984382 chess2vec-0.1.3b2/pyproject.toml
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 chess2vec-0.1.3b2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.3b3/README.md
+-rw-r--r--   0        0        0     5582 2024-04-17 21:16:47.895949 chess2vec-0.1.3b3/chess2vec/__init__.py
+-rw-r--r--   0        0        0     1910 2024-04-16 20:11:28.318615 chess2vec-0.1.3b3/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc
+-rw-r--r--   0        0        0      740 2024-04-16 16:21:07.852284 chess2vec-0.1.3b3/chess2vec/_utils/sparse.py
+-rw-r--r--   0        0        0      538 2024-04-16 16:46:49.087490 chess2vec-0.1.3b3/chess2vec/_utils/vector.py
+-rw-r--r--   0        0        0      358 2024-04-17 21:16:58.389446 chess2vec-0.1.3b3/pyproject.toml
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 chess2vec-0.1.3b3/PKG-INFO
```

### Comparing `chess2vec-0.1.3b2/chess2vec/__init__.py` & `chess2vec-0.1.3b3/chess2vec/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             max_games = float("inf")
 
         builder = csr_matrix_builder()
         positions = []
         idx = num_game = 0
         
         if status:
-            bar = tqdm()
+            bar = tqdm(total=max_games)
 
         game = chess.pgn.read_game(x)
 
         while game and num_game < max_games:
             board = game.board()
 
             builder.add_entry(idx, list(_actions(board)))
```

### Comparing `chess2vec-0.1.3b2/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc` & `chess2vec-0.1.3b3/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.3b2/chess2vec/_utils/sparse.py` & `chess2vec-0.1.3b3/chess2vec/_utils/sparse.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.3b2/chess2vec/_utils/vector.py` & `chess2vec-0.1.3b3/chess2vec/_utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.3b2/PKG-INFO` & `chess2vec-0.1.3b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.1.3b2
+Version: 0.1.3b3
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

