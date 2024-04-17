# Comparing `tmp/qxelarator-0.6.5-cp39-cp39-win_amd64.whl.zip` & `tmp/qxelarator-0.7.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 469859 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat      915 b- defN 23-Dec-04 12:36 qxelarator/__init__.py
--rw-rw-rw-  2.0 fat  1539072 b- defN 23-Dec-04 12:39 qxelarator/_qxelarator.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     3037 b- defN 23-Dec-04 12:39 qxelarator/qxelarator.py
--rw-rw-rw-  2.0 fat      187 b- defN 23-Dec-04 12:39 qxelarator-0.6.5.dist-info/AUTHORS
--rw-rw-rw-  2.0 fat      587 b- defN 23-Dec-04 12:39 qxelarator-0.6.5.dist-info/LICENSE.md
--rw-rw-rw-  2.0 fat     1646 b- defN 23-Dec-04 12:39 qxelarator-0.6.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Dec-04 12:39 qxelarator-0.6.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Dec-04 12:39 qxelarator-0.6.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      754 b- defN 23-Dec-04 12:39 qxelarator-0.6.5.dist-info/RECORD
-9 files, 1546309 bytes uncompressed, 468557 bytes compressed:  69.7%
+Zip file size: 562368 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat      915 b- defN 24-Apr-17 11:34 qxelarator/__init__.py
+-rw-rw-rw-  2.0 fat  1651200 b- defN 24-Apr-17 11:36 qxelarator/_qxelarator.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2308 b- defN 24-Apr-17 11:36 qxelarator/qxelarator.py
+-rw-rw-rw-  2.0 fat      187 b- defN 24-Apr-17 11:36 qxelarator-0.7.0.dist-info/AUTHORS
+-rw-rw-rw-  2.0 fat      587 b- defN 24-Apr-17 11:36 qxelarator-0.7.0.dist-info/LICENSE.md
+-rw-rw-rw-  2.0 fat     1388 b- defN 24-Apr-17 11:36 qxelarator-0.7.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-17 11:36 qxelarator-0.7.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 24-Apr-17 11:36 qxelarator-0.7.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      754 b- defN 24-Apr-17 11:36 qxelarator-0.7.0.dist-info/RECORD
+9 files, 1657450 bytes uncompressed, 561066 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: qxelarator/_qxelarator.cp39-win_amd64.pyd
 Comment: 
 
 Filename: qxelarator/qxelarator.py
 Comment: 
 
-Filename: qxelarator-0.6.5.dist-info/AUTHORS
+Filename: qxelarator-0.7.0.dist-info/AUTHORS
 Comment: 
 
-Filename: qxelarator-0.6.5.dist-info/LICENSE.md
+Filename: qxelarator-0.7.0.dist-info/LICENSE.md
 Comment: 
 
-Filename: qxelarator-0.6.5.dist-info/METADATA
+Filename: qxelarator-0.7.0.dist-info/METADATA
 Comment: 
 
-Filename: qxelarator-0.6.5.dist-info/WHEEL
+Filename: qxelarator-0.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: qxelarator-0.6.5.dist-info/top_level.txt
+Filename: qxelarator-0.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: qxelarator-0.6.5.dist-info/RECORD
+Filename: qxelarator-0.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qxelarator/qxelarator.py

```diff
@@ -56,36 +56,14 @@
 
 
 class _SwigNonDynamicMeta(type):
     """Meta class to enforce nondynamic attributes (no new attributes) for a class"""
     __setattr__ = _swig_setattr_nondynamic_class_variable(type.__setattr__)
 
 
-class QX(object):
-    thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
-    __repr__ = _swig_repr
-
-    def set_json_output_path(self, filePath):
-        return _qxelarator.QX_set_json_output_path(self, filePath)
-
-    def set(self, filePath):
-        return _qxelarator.QX_set(self, filePath)
-
-    def set_string(self, s):
-        return _qxelarator.QX_set_string(self, s)
-
-    def execute(self, iterations=1):
-        return _qxelarator.QX_execute(self, iterations)
-
-    def __init__(self):
-        _qxelarator.QX_swiginit(self, _qxelarator.new_QX())
-    __swig_destroy__ = _qxelarator.delete_QX
-
-# Register QX in _qxelarator:
-_qxelarator.QX_swigregister(QX)
 
 def execute_string(*args, **kwargs):
     return _qxelarator.execute_string(*args, **kwargs)
 
 def execute_file(*args, **kwargs):
     return _qxelarator.execute_file(*args, **kwargs)
```

## Comparing `qxelarator-0.6.5.dist-info/LICENSE.md` & `qxelarator-0.7.0.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `qxelarator-0.6.5.dist-info/METADATA` & `qxelarator-0.7.0.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 Metadata-Version: 2.1
 Name: qxelarator
-Version: 0.6.5
+Version: 0.7.0
 Summary: qxelarator Python Package
 Home-page: https://github.com/QuTech-Delft/qx-simulator
 Author: QuTech, TU Delft
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: AUTHORS
 Requires-Dist: msvc-runtime ; platform_system == "Windows"
 
 # QX Simulator
```

