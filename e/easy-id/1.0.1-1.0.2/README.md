# Comparing `tmp/easy_id-1.0.1.tar.gz` & `tmp/easy_id-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_id-1.0.1.tar", last modified: Wed Apr 17 08:08:21 2024, max compression
+gzip compressed data, was "easy_id-1.0.2.tar", last modified: Wed Apr 17 08:23:04 2024, max compression
```

## Comparing `easy_id-1.0.1.tar` & `easy_id-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 08:08:21.544977 easy_id-1.0.1/
--rw-rw-rw-   0        0        0      857 2024-04-17 08:08:21.544977 easy_id-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      490 2024-04-17 07:25:26.000000 easy_id-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 08:08:21.499616 easy_id-1.0.1/easy_id/
-drwxrwxrwx   0        0        0        0 2024-04-17 08:08:21.544977 easy_id-1.0.1/easy_id/easy_id.egg-info/
--rw-rw-rw-   0        0        0      857 2024-04-17 08:08:21.000000 easy_id-1.0.1/easy_id/easy_id.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2024-04-17 08:08:21.000000 easy_id-1.0.1/easy_id/easy_id.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 08:08:21.000000 easy_id-1.0.1/easy_id/easy_id.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-17 08:08:21.000000 easy_id-1.0.1/easy_id/easy_id.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-17 08:08:21.542595 easy_id-1.0.1/easy_id/generators/
--rw-rw-rw-   0        0        0      126 2024-04-17 06:35:22.000000 easy_id-1.0.1/easy_id/generators/__init__.py
--rw-rw-rw-   0        0        0      417 2024-04-17 06:15:22.000000 easy_id-1.0.1/easy_id/generators/base.py
--rw-rw-rw-   0        0        0      534 2024-04-17 06:15:22.000000 easy_id-1.0.1/easy_id/generators/nanoid.py
--rw-rw-rw-   0        0        0     2380 2024-04-17 06:09:18.000000 easy_id-1.0.1/easy_id/generators/snowflake.py
--rw-rw-rw-   0        0        0      852 2024-04-17 06:35:21.000000 easy_id-1.0.1/easy_id/generators/ulid.py
--rw-rw-rw-   0        0        0       82 2024-04-17 03:40:46.000000 easy_id-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      591 2024-04-17 08:08:21.549592 easy_id-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0       69 2024-04-17 03:42:16.000000 easy_id-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:23:04.885393 easy_id-1.0.2/
+-rw-rw-rw-   0        0        0      857 2024-04-17 08:23:04.885393 easy_id-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2024-04-17 08:13:09.000000 easy_id-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 08:23:04.829829 easy_id-1.0.2/easy_id/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:23:04.882231 easy_id-1.0.2/easy_id/easy_id.egg-info/
+-rw-rw-rw-   0        0        0      857 2024-04-17 08:23:04.000000 easy_id-1.0.2/easy_id/easy_id.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2024-04-17 08:23:04.000000 easy_id-1.0.2/easy_id/easy_id.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 08:23:04.000000 easy_id-1.0.2/easy_id/easy_id.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-17 08:23:04.000000 easy_id-1.0.2/easy_id/easy_id.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 08:23:04.880792 easy_id-1.0.2/easy_id/generators/
+-rw-rw-rw-   0        0        0      126 2024-04-17 06:35:22.000000 easy_id-1.0.2/easy_id/generators/__init__.py
+-rw-rw-rw-   0        0        0      417 2024-04-17 06:15:22.000000 easy_id-1.0.2/easy_id/generators/base.py
+-rw-rw-rw-   0        0        0      534 2024-04-17 06:15:22.000000 easy_id-1.0.2/easy_id/generators/nanoid.py
+-rw-rw-rw-   0        0        0     2380 2024-04-17 06:09:18.000000 easy_id-1.0.2/easy_id/generators/snowflake.py
+-rw-rw-rw-   0        0        0      852 2024-04-17 06:35:21.000000 easy_id-1.0.2/easy_id/generators/ulid.py
+-rw-rw-rw-   0        0        0       82 2024-04-17 03:40:46.000000 easy_id-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      591 2024-04-17 08:23:04.895623 easy_id-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       69 2024-04-17 03:42:16.000000 easy_id-1.0.2/setup.py
```

### Comparing `easy_id-1.0.1/PKG-INFO` & `easy_id-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: easy-id
-Version: 1.0.1
+Name: easy_id
+Version: 1.0.2
 Summary: An easy to use suite of configurable id generators
 Home-page: https://github.com/RadenTheFolf/easy_id
 Author: RadenTheFolf
 Author-email: raden@zynosstudios.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `easy_id-1.0.1/easy_id/easy_id.egg-info/PKG-INFO` & `easy_id-1.0.2/easy_id/easy_id.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: easy-id
-Version: 1.0.1
+Name: easy_id
+Version: 1.0.2
 Summary: An easy to use suite of configurable id generators
 Home-page: https://github.com/RadenTheFolf/easy_id
 Author: RadenTheFolf
 Author-email: raden@zynosstudios.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `easy_id-1.0.1/easy_id/generators/nanoid.py` & `easy_id-1.0.2/easy_id/generators/nanoid.py`

 * *Files identical despite different names*

### Comparing `easy_id-1.0.1/easy_id/generators/snowflake.py` & `easy_id-1.0.2/easy_id/generators/snowflake.py`

 * *Files identical despite different names*

### Comparing `easy_id-1.0.1/easy_id/generators/ulid.py` & `easy_id-1.0.2/easy_id/generators/ulid.py`

 * *Files identical despite different names*

### Comparing `easy_id-1.0.1/setup.cfg` & `easy_id-1.0.2/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2065 6173 792d 6964 0d0a 7665 7273   = easy-id..vers
-00000020: 696f 6e20 3d20 312e 302e 310d 0a61 7574  ion = 1.0.1..aut
+00000010: 203d 2065 6173 795f 6964 0d0a 7665 7273   = easy_id..vers
+00000020: 696f 6e20 3d20 312e 302e 320d 0a61 7574  ion = 1.0.2..aut
 00000030: 686f 7220 3d20 5261 6465 6e54 6865 466f  hor = RadenTheFo
 00000040: 6c66 0d0a 6175 7468 6f72 5f65 6d61 696c  lf..author_email
 00000050: 203d 2072 6164 656e 407a 796e 6f73 7374   = raden@zynosst
 00000060: 7564 696f 732e 636f 6d0d 0a64 6573 6372  udios.com..descr
 00000070: 6970 7469 6f6e 203d 2041 6e20 6561 7379  iption = An easy
 00000080: 2074 6f20 7573 6520 7375 6974 6520 6f66   to use suite of
 00000090: 2063 6f6e 6669 6775 7261 626c 6520 6964   configurable id
```

