# Comparing `tmp/ckzg-1.0.0-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/ckzg-1.0.1-cp38-cp38-musllinux_1_1_aarch64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,10 @@
-Zip file size: 65734 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat   163328 b- defN 24-Mar-12 14:05 ckzg.pypy39-pp73-win_amd64.pyd
--rw-rw-rw-  2.0 fat      695 b- defN 24-Mar-12 14:05 ckzg-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 24-Mar-12 14:05 ckzg-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 24-Mar-12 14:05 ckzg-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      374 b- defN 24-Mar-12 14:05 ckzg-1.0.0.dist-info/RECORD
-5 files, 164509 bytes uncompressed, 65040 bytes compressed:  60.5%
+Zip file size: 137764 bytes, number of entries: 8
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-17 01:20 ckzg.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-17 01:20 ckzg-1.0.1.dist-info/
+-rwxr-xr-x  2.0 unx   336128 b- defN 24-Apr-17 01:20 ckzg.cpython-38-aarch64-linux-gnu.so
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-17 01:20 ckzg-1.0.1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx      683 b- defN 24-Apr-17 01:20 ckzg-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      112 b- defN 24-Apr-17 01:20 ckzg-1.0.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      472 b- defN 24-Apr-17 01:20 ckzg-1.0.1.dist-info/RECORD
+-rw-r--r--  2.0 unx    11357 b- defN 24-Apr-17 01:20 ckzg-1.0.1.dist-info/LICENSE
+8 files, 348757 bytes uncompressed, 136712 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -1,16 +1,25 @@
-Filename: ckzg.pypy39-pp73-win_amd64.pyd
+Filename: ckzg.libs/
 Comment: 
 
-Filename: ckzg-1.0.0.dist-info/METADATA
+Filename: ckzg-1.0.1.dist-info/
 Comment: 
 
-Filename: ckzg-1.0.0.dist-info/WHEEL
+Filename: ckzg.cpython-38-aarch64-linux-gnu.so
 Comment: 
 
-Filename: ckzg-1.0.0.dist-info/top_level.txt
+Filename: ckzg-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ckzg-1.0.0.dist-info/RECORD
+Filename: ckzg-1.0.1.dist-info/METADATA
+Comment: 
+
+Filename: ckzg-1.0.1.dist-info/WHEEL
+Comment: 
+
+Filename: ckzg-1.0.1.dist-info/RECORD
+Comment: 
+
+Filename: ckzg-1.0.1.dist-info/LICENSE
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## Comparing `ckzg-1.0.0.dist-info/METADATA` & `ckzg-1.0.1.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-Metadata-Version: 2.1
-Name: ckzg
-Version: 1.0.0
-Summary: Python bindings for C-KZG-4844
-Home-page: https://github.com/ethereum/c-kzg-4844
-Author: Ethereum Foundation
-Author-email: security@ethereum.org
-License: Apache-2.0
-Description-Content-Type: text/markdown
-
-# Python bindings
-
-This directory contains Python bindings for the C-KZG-4844 library.
-
-## Prerequisites
-
-These bindings require `python3` and `PyYAML`.
-```
-sudo apt install python3 python3-pip
-python3 -m pip install PyYAML
-```
-
-## Build & test
-
-Everything is consolidated into one command:
-```
-make
-```
-
-You should expect to see these messages at the bottom:
-```
-python3 tests.py
-tests passed
-```
+Metadata-Version: 2.1
+Name: ckzg
+Version: 1.0.1
+Summary: Python bindings for C-KZG-4844
+Home-page: https://github.com/ethereum/c-kzg-4844
+Author: Ethereum Foundation
+Author-email: security@ethereum.org
+License: Apache-2.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Python bindings
+
+This directory contains Python bindings for the C-KZG-4844 library.
+
+## Prerequisites
+
+These bindings require `python3` and `PyYAML`.
+```
+sudo apt install python3 python3-pip
+python3 -m pip install PyYAML
+```
+
+## Build & test
+
+Everything is consolidated into one command:
+```
+make
+```
+
+You should expect to see these messages at the bottom:
+```
+python3 tests.py
+tests passed
+```
```

