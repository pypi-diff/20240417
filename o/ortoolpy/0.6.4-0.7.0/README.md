# Comparing `tmp/ortoolpy-0.6.4-py3-none-any.whl.zip` & `tmp/ortoolpy-0.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 28185 bytes, number of entries: 8
+Zip file size: 28341 bytes, number of entries: 9
 -rw-r--r--  2.0 unx     1216 b- defN 80-Jan-01 00:00 ortoolpy/__init__.py
 -rw-r--r--  2.0 unx     3325 b- defN 80-Jan-01 00:00 ortoolpy/cover_by_rect.py
 -rw-r--r--  2.0 unx    51604 b- defN 80-Jan-01 00:00 ortoolpy/etc.py
 -rw-r--r--  2.0 unx    28688 b- defN 80-Jan-01 00:00 ortoolpy/optimization/__init__.py
--rw-r--r--  2.0 unx    10763 b- defN 80-Jan-01 00:00 ortoolpy-0.6.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     1553 b- defN 80-Jan-01 00:00 ortoolpy-0.6.4.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 ortoolpy-0.6.4.dist-info/WHEEL
-?rw-r--r--  2.0 unx      622 b- defN 16-Jan-01 00:00 ortoolpy-0.6.4.dist-info/RECORD
-8 files, 97859 bytes uncompressed, 27117 bytes compressed:  72.3%
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 ortoolpy/py.typed
+-rw-r--r--  2.0 unx    10763 b- defN 80-Jan-01 00:00 ortoolpy-0.7.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1556 b- defN 80-Jan-01 00:00 ortoolpy-0.7.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 ortoolpy-0.7.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx      693 b- defN 16-Jan-01 00:00 ortoolpy-0.7.0.dist-info/RECORD
+9 files, 97933 bytes uncompressed, 27163 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -6,20 +6,23 @@
 
 Filename: ortoolpy/etc.py
 Comment: 
 
 Filename: ortoolpy/optimization/__init__.py
 Comment: 
 
-Filename: ortoolpy-0.6.4.dist-info/LICENSE
+Filename: ortoolpy/py.typed
 Comment: 
 
-Filename: ortoolpy-0.6.4.dist-info/METADATA
+Filename: ortoolpy-0.7.0.dist-info/LICENSE
 Comment: 
 
-Filename: ortoolpy-0.6.4.dist-info/WHEEL
+Filename: ortoolpy-0.7.0.dist-info/METADATA
 Comment: 
 
-Filename: ortoolpy-0.6.4.dist-info/RECORD
+Filename: ortoolpy-0.7.0.dist-info/WHEEL
+Comment: 
+
+Filename: ortoolpy-0.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ortoolpy-0.6.4.dist-info/LICENSE` & `ortoolpy-0.7.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ortoolpy-0.6.4.dist-info/METADATA` & `ortoolpy-0.7.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: ortoolpy
-Version: 0.6.4
+Version: 0.7.0
 Summary: `ortoolpy` is a package for Operations Research.
 Home-page: https://github.com/SaitoTsutomu/ortoolpy
 License: Apache-2.0
 Author: SaitoTsutomu
 Author-email: tsutomu7@hotmail.co.jp
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.12,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
-Requires-Dist: more-itertools (>=10.1,<11.0)
-Requires-Dist: pandas (>=1.5.3)
-Requires-Dist: pulp (>=2.7,<3.0)
+Requires-Dist: more-itertools (>=10.2,<11.0)
+Requires-Dist: pandas (>=2.2,<3.0)
+Requires-Dist: pulp (>=2.8,<3.0)
 Description-Content-Type: text/x-rst
 
 `ortoolpy` is a package for Operations Research.
 It is user's responsibility for the use of `ortoolpy`.
 
 ::
```

## Comparing `ortoolpy-0.6.4.dist-info/RECORD` & `ortoolpy-0.7.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 ortoolpy/__init__.py,sha256=1Kz8xLBvOMajT-3p0MgqjnAiw81HGkrpO1NwR6a6gO0,1216
 ortoolpy/cover_by_rect.py,sha256=FuEIn4IiIo7UDQi3PGZXkxEVzxA3wQ8av97bWuz1vdQ,3325
 ortoolpy/etc.py,sha256=QCUDxR3dlK1ryFxuAARQBeYrJW8JD57fBcusnegxWOk,51604
 ortoolpy/optimization/__init__.py,sha256=HRK7lqfKpsDekUyfOzGXiHdbeC_JKdtNOjJ11iNqihA,28688
-ortoolpy-0.6.4.dist-info/LICENSE,sha256=bwiSACYkm_Y0590tyT1iojp4wcMh0hpNxLWjQboSyno,10763
-ortoolpy-0.6.4.dist-info/METADATA,sha256=E_K3KZGC1EfYAU6qK47oq77jfPMaDjsI_TOLLiec11A,1553
-ortoolpy-0.6.4.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-ortoolpy-0.6.4.dist-info/RECORD,,
+ortoolpy/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ortoolpy-0.7.0.dist-info/LICENSE,sha256=bwiSACYkm_Y0590tyT1iojp4wcMh0hpNxLWjQboSyno,10763
+ortoolpy-0.7.0.dist-info/METADATA,sha256=P2j00PtctEBf8U5HsXKfSqMcs5e2clWI5O63hu23O80,1556
+ortoolpy-0.7.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+ortoolpy-0.7.0.dist-info/RECORD,,
```

