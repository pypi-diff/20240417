# Comparing `tmp/cctext-0.1.2.tar.gz` & `tmp/cctext-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cctext-0.1.2.tar", last modified: Fri Apr 12 16:53:55 2024, max compression
+gzip compressed data, was "cctext-0.1.3.tar", last modified: Wed Apr 17 11:38:25 2024, max compression
```

## Comparing `cctext-0.1.2.tar` & `cctext-0.1.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 16:53:55.193759 cctext-0.1.2/
--rw-rw-rw-   0        0        0     1101 2024-04-12 07:07:09.000000 cctext-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     1278 2024-04-12 16:53:55.192759 cctext-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      396 2024-04-12 10:07:32.000000 cctext-0.1.2/README.md
--rw-rw-rw-   0        0        0        5 2024-04-12 16:47:27.000000 cctext-0.1.2/VERSION
-drwxrwxrwx   0        0        0        0 2024-04-12 16:53:55.172758 cctext-0.1.2/cctext/
--rw-rw-rw-   0        0        0      888 2024-04-11 20:12:00.000000 cctext-0.1.2/cctext/__init__.py
--rw-rw-rw-   0        0        0     2865 2024-04-11 20:11:26.000000 cctext-0.1.2/cctext/api.py
--rw-rw-rw-   0        0        0     2585 2024-04-11 19:52:19.000000 cctext-0.1.2/cctext/context.py
--rw-rw-rw-   0        0        0        0 2024-04-12 10:19:33.000000 cctext-0.1.2/cctext/py.typed
--rw-rw-rw-   0        0        0     1684 2024-04-11 20:24:09.000000 cctext-0.1.2/cctext/reference.py
--rw-rw-rw-   0        0        0     4869 2024-04-12 16:45:21.000000 cctext-0.1.2/cctext/resolver.py
--rw-rw-rw-   0        0        0     4868 2024-04-11 20:07:22.000000 cctext-0.1.2/cctext/rumodel.py
--rw-rw-rw-   0        0        0    20073 2024-04-11 20:10:47.000000 cctext-0.1.2/cctext/ruparser.py
--rw-rw-rw-   0        0        0     2620 2024-04-11 20:10:57.000000 cctext-0.1.2/cctext/syntax.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:53:55.191761 cctext-0.1.2/cctext.egg-info/
--rw-rw-rw-   0        0        0     1278 2024-04-12 16:53:55.000000 cctext-0.1.2/cctext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2024-04-12 16:53:55.000000 cctext-0.1.2/cctext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 16:53:55.000000 cctext-0.1.2/cctext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-12 10:18:13.000000 cctext-0.1.2/cctext.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       17 2024-04-12 16:53:55.000000 cctext-0.1.2/cctext.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-12 16:53:55.000000 cctext-0.1.2/cctext.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2024-04-12 10:22:23.000000 cctext-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      869 2024-04-12 16:53:55.194759 cctext-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      121 2024-04-12 10:17:50.000000 cctext-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:53:55.189760 cctext-0.1.2/tests/
--rw-rw-rw-   0        0        0      197 2024-04-11 20:06:04.000000 cctext-0.1.2/tests/__init__.py
--rw-rw-rw-   0        0        0     4079 2024-04-11 20:06:14.000000 cctext-0.1.2/tests/t_api.py
--rw-rw-rw-   0        0        0     1414 2024-04-11 20:03:25.000000 cctext-0.1.2/tests/t_context.py
--rw-rw-rw-   0        0        0     1955 2024-04-11 20:03:38.000000 cctext-0.1.2/tests/t_reference.py
--rw-rw-rw-   0        0        0     7429 2024-04-12 16:46:51.000000 cctext-0.1.2/tests/t_resolver.py
--rw-rw-rw-   0        0        0      621 2024-04-11 19:41:33.000000 cctext-0.1.2/tests/t_rumodel.py
--rw-rw-rw-   0        0        0    30488 2024-04-11 19:55:39.000000 cctext-0.1.2/tests/t_ruparser.py
--rw-rw-rw-   0        0        0     3421 2023-08-18 16:45:24.000000 cctext-0.1.2/tests/t_syntax.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:38:25.173075 cctext-0.1.3/
+-rw-rw-rw-   0        0        0     1101 2024-04-12 07:07:09.000000 cctext-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1326 2024-04-17 11:38:25.173075 cctext-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-04-12 10:07:32.000000 cctext-0.1.3/README.md
+-rw-rw-rw-   0        0        0        5 2024-04-17 11:37:40.000000 cctext-0.1.3/VERSION
+drwxrwxrwx   0        0        0        0 2024-04-17 11:38:25.154076 cctext-0.1.3/cctext/
+-rw-rw-rw-   0        0        0      888 2024-04-11 20:12:00.000000 cctext-0.1.3/cctext/__init__.py
+-rw-rw-rw-   0        0        0     2865 2024-04-11 20:11:26.000000 cctext-0.1.3/cctext/api.py
+-rw-rw-rw-   0        0        0     2585 2024-04-11 19:52:19.000000 cctext-0.1.3/cctext/context.py
+-rw-rw-rw-   0        0        0        0 2024-04-12 10:19:33.000000 cctext-0.1.3/cctext/py.typed
+-rw-rw-rw-   0        0        0     1684 2024-04-11 20:24:09.000000 cctext-0.1.3/cctext/reference.py
+-rw-rw-rw-   0        0        0     4869 2024-04-12 16:45:21.000000 cctext-0.1.3/cctext/resolver.py
+-rw-rw-rw-   0        0        0     4868 2024-04-11 20:07:22.000000 cctext-0.1.3/cctext/rumodel.py
+-rw-rw-rw-   0        0        0    20073 2024-04-11 20:10:47.000000 cctext-0.1.3/cctext/ruparser.py
+-rw-rw-rw-   0        0        0     2620 2024-04-11 20:10:57.000000 cctext-0.1.3/cctext/syntax.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:38:25.171076 cctext-0.1.3/cctext.egg-info/
+-rw-rw-rw-   0        0        0     1326 2024-04-17 11:38:24.000000 cctext-0.1.3/cctext.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2024-04-17 11:38:24.000000 cctext-0.1.3/cctext.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 11:38:24.000000 cctext-0.1.3/cctext.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-12 10:18:13.000000 cctext-0.1.3/cctext.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       17 2024-04-17 11:38:24.000000 cctext-0.1.3/cctext.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-17 11:38:24.000000 cctext-0.1.3/cctext.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2024-04-12 10:22:23.000000 cctext-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      912 2024-04-17 11:38:25.175131 cctext-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      121 2024-04-12 10:17:50.000000 cctext-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:38:25.170075 cctext-0.1.3/tests/
+-rw-rw-rw-   0        0        0      197 2024-04-11 20:06:04.000000 cctext-0.1.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     4079 2024-04-11 20:06:14.000000 cctext-0.1.3/tests/t_api.py
+-rw-rw-rw-   0        0        0     1414 2024-04-11 20:03:25.000000 cctext-0.1.3/tests/t_context.py
+-rw-rw-rw-   0        0        0     1955 2024-04-11 20:03:38.000000 cctext-0.1.3/tests/t_reference.py
+-rw-rw-rw-   0        0        0     7429 2024-04-12 16:46:51.000000 cctext-0.1.3/tests/t_resolver.py
+-rw-rw-rw-   0        0        0      621 2024-04-11 19:41:33.000000 cctext-0.1.3/tests/t_rumodel.py
+-rw-rw-rw-   0        0        0    30488 2024-04-11 19:55:39.000000 cctext-0.1.3/tests/t_ruparser.py
+-rw-rw-rw-   0        0        0     3421 2023-08-18 16:45:24.000000 cctext-0.1.3/tests/t_syntax.py
```

### Comparing `cctext-0.1.2/LICENSE` & `cctext-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cctext-0.1.2/PKG-INFO` & `cctext-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: cctext
-Version: 0.1.2
+Version: 0.1.3
 Summary: Text processing library for russian languange
+Home-page: https://github.com/IRBorisov/cctext
 Author: CIHT CONCEPT, IRBorisov
 Author-email: iborisov@acconcept.ru
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cctext-0.1.2/cctext/__init__.py` & `cctext-0.1.3/cctext/__init__.py`

 * *Files identical despite different names*

### Comparing `cctext-0.1.2/cctext/api.py` & `cctext-0.1.3/cctext/api.py`

 * *Files identical despite different names*

### Comparing `cctext-0.1.2/cctext/context.py` & `cctext-0.1.3/cctext/context.py`

 * *Files identical despite different names*

### Comparing `cctext-0.1.2/cctext/reference.py` & `cctext-0.1.3/cctext/reference.py`

 * *Files identical despite different names*

### Comparing `cctext-0.1.2/cctext/resolver.py` & `cctext-0.1.3/cctext/resolver.py`

 * *Files identical despite different names*

### Comparing `cctext-0.1.2/cctext/rumodel.py` & `cctext-0.1.3/cctext/rumodel.py`

 * *Files identical despite different names*

### Comparing `cctext-0.1.2/cctext/ruparser.py` & `cctext-0.1.3/cctext/ruparser.py`

 * *Files identical despite different names*

### Comparing `cctext-0.1.2/cctext/syntax.py` & `cctext-0.1.3/cctext/syntax.py`

 * *Files identical despite different names*

### Comparing `cctext-0.1.2/cctext.egg-info/PKG-INFO` & `cctext-0.1.3/cctext.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: cctext
-Version: 0.1.2
+Version: 0.1.3
 Summary: Text processing library for russian languange
+Home-page: https://github.com/IRBorisov/cctext
 Author: CIHT CONCEPT, IRBorisov
 Author-email: iborisov@acconcept.ru
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cctext-0.1.2/cctext.egg-info/SOURCES.txt` & `cctext-0.1.3/cctext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cctext-0.1.2/setup.cfg` & `cctext-0.1.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -10,46 +10,48 @@
 00000090: 726f 6365 7373 696e 6720 6c69 6272 6172  rocessing librar
 000000a0: 7920 666f 7220 7275 7373 6961 6e20 6c61  y for russian la
 000000b0: 6e67 7561 6e67 650d 0a6c 6f6e 675f 6465  nguange..long_de
 000000c0: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
 000000d0: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
 000000e0: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
 000000f0: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
-00000100: 742f 6d61 726b 646f 776e 0d0a 6c69 6365  t/markdown..lice
-00000110: 6e73 6520 3d20 4d49 540d 0a63 6c61 7373  nse = MIT..class
-00000120: 6966 6965 7273 203d 200d 0a09 4465 7665  ifiers = ...Deve
-00000130: 6c6f 706d 656e 7420 5374 6174 7573 203a  lopment Status :
-00000140: 3a20 3320 2d20 416c 7068 610d 0a09 496e  : 3 - Alpha...In
-00000150: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
-00000160: 3a3a 2044 6576 656c 6f70 6572 730d 0a09  :: Developers...
-00000170: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
-00000180: 6520 3a3a 2053 6369 656e 6365 2f52 6573  e :: Science/Res
-00000190: 6561 7263 680d 0a09 4c69 6365 6e73 6520  earch...License 
-000001a0: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-000001b0: 3a3a 204d 4954 204c 6963 656e 7365 0d0a  :: MIT License..
-000001c0: 094e 6174 7572 616c 204c 616e 6775 6167  .Natural Languag
-000001d0: 6520 3a3a 2052 7573 7369 616e 0d0a 0950  e :: Russian...P
-000001e0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000001f0: 6167 6520 3a3a 2050 7974 686f 6e0d 0a09  age :: Python...
-00000200: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000210: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000220: 3a20 330d 0a09 5072 6f67 7261 6d6d 696e  : 3...Programmin
-00000230: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000240: 7468 6f6e 203a 3a20 332e 3132 0d0a 0954  thon :: 3.12...T
-00000250: 6f70 6963 203a 3a20 536f 6674 7761 7265  opic :: Software
-00000260: 2044 6576 656c 6f70 6d65 6e74 203a 3a20   Development :: 
-00000270: 4c69 6272 6172 6965 7320 3a3a 2050 7974  Libraries :: Pyt
-00000280: 686f 6e20 4d6f 6475 6c65 730d 0a09 546f  hon Modules...To
-00000290: 7069 6320 3a3a 2053 6369 656e 7469 6669  pic :: Scientifi
-000002a0: 632f 456e 6769 6e65 6572 696e 6720 3a3a  c/Engineering ::
-000002b0: 2049 6e66 6f72 6d61 7469 6f6e 2041 6e61   Information Ana
-000002c0: 6c79 7369 730d 0a09 546f 7069 6320 3a3a  lysis...Topic ::
-000002d0: 2054 6578 7420 5072 6f63 6573 7369 6e67   Text Processing
-000002e0: 203a 3a20 4c69 6e67 7569 7374 6963 0d0a   :: Linguistic..
-000002f0: 0d0a 5b6f 7074 696f 6e73 5d0d 0a70 6163  ..[options]..pac
-00000300: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a69  kages = find:..i
-00000310: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
-00000320: 3d20 0d0a 0972 617a 6465 6c0d 0a09 7079  = ...razdel...py
-00000330: 6d6f 7270 6879 330d 0a0d 0a5b 6567 675f  morphy3....[egg_
-00000340: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-00000350: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-00000360: 300d 0a0d 0a                             0....
+00000100: 742f 6d61 726b 646f 776e 0d0a 7572 6c20  t/markdown..url 
+00000110: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+00000120: 2e63 6f6d 2f49 5242 6f72 6973 6f76 2f63  .com/IRBorisov/c
+00000130: 6374 6578 740d 0a6c 6963 656e 7365 203d  ctext..license =
+00000140: 204d 4954 0d0a 636c 6173 7369 6669 6572   MIT..classifier
+00000150: 7320 3d20 0d0a 0944 6576 656c 6f70 6d65  s = ...Developme
+00000160: 6e74 2053 7461 7475 7320 3a3a 2033 202d  nt Status :: 3 -
+00000170: 2041 6c70 6861 0d0a 0949 6e74 656e 6465   Alpha...Intende
+00000180: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
+00000190: 7665 6c6f 7065 7273 0d0a 0949 6e74 656e  velopers...Inten
+000001a0: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
+000001b0: 5363 6965 6e63 652f 5265 7365 6172 6368  Science/Research
+000001c0: 0d0a 094c 6963 656e 7365 203a 3a20 4f53  ...License :: OS
+000001d0: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
+000001e0: 5420 4c69 6365 6e73 650d 0a09 4e61 7475  T License...Natu
+000001f0: 7261 6c20 4c61 6e67 7561 6765 203a 3a20  ral Language :: 
+00000200: 5275 7373 6961 6e0d 0a09 5072 6f67 7261  Russian...Progra
+00000210: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000220: 3a20 5079 7468 6f6e 0d0a 0950 726f 6772  : Python...Progr
+00000230: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000240: 3a3a 2050 7974 686f 6e20 3a3a 2033 0d0a  :: Python :: 3..
+00000250: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+00000260: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000270: 3a3a 2033 2e31 320d 0a09 546f 7069 6320  :: 3.12...Topic 
+00000280: 3a3a 2053 6f66 7477 6172 6520 4465 7665  :: Software Deve
+00000290: 6c6f 706d 656e 7420 3a3a 204c 6962 7261  lopment :: Libra
+000002a0: 7269 6573 203a 3a20 5079 7468 6f6e 204d  ries :: Python M
+000002b0: 6f64 756c 6573 0d0a 0954 6f70 6963 203a  odules...Topic :
+000002c0: 3a20 5363 6965 6e74 6966 6963 2f45 6e67  : Scientific/Eng
+000002d0: 696e 6565 7269 6e67 203a 3a20 496e 666f  ineering :: Info
+000002e0: 726d 6174 696f 6e20 416e 616c 7973 6973  rmation Analysis
+000002f0: 0d0a 0954 6f70 6963 203a 3a20 5465 7874  ...Topic :: Text
+00000300: 2050 726f 6365 7373 696e 6720 3a3a 204c   Processing :: L
+00000310: 696e 6775 6973 7469 630d 0a0d 0a5b 6f70  inguistic....[op
+00000320: 7469 6f6e 735d 0d0a 7061 636b 6167 6573  tions]..packages
+00000330: 203d 2066 696e 643a 0d0a 696e 7374 616c   = find:..instal
+00000340: 6c5f 7265 7175 6972 6573 203d 200d 0a09  l_requires = ...
+00000350: 7261 7a64 656c 0d0a 0970 796d 6f72 7068  razdel...pymorph
+00000360: 7933 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  y3....[egg_info]
+00000370: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+00000380: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

### Comparing `cctext-0.1.2/tests/t_api.py` & `cctext-0.1.3/tests/t_api.py`

 * *Files identical despite different names*

### Comparing `cctext-0.1.2/tests/t_context.py` & `cctext-0.1.3/tests/t_context.py`

 * *Files identical despite different names*

### Comparing `cctext-0.1.2/tests/t_reference.py` & `cctext-0.1.3/tests/t_reference.py`

 * *Files identical despite different names*

### Comparing `cctext-0.1.2/tests/t_resolver.py` & `cctext-0.1.3/tests/t_resolver.py`

 * *Files identical despite different names*

### Comparing `cctext-0.1.2/tests/t_rumodel.py` & `cctext-0.1.3/tests/t_rumodel.py`

 * *Files identical despite different names*

### Comparing `cctext-0.1.2/tests/t_ruparser.py` & `cctext-0.1.3/tests/t_ruparser.py`

 * *Files identical despite different names*

### Comparing `cctext-0.1.2/tests/t_syntax.py` & `cctext-0.1.3/tests/t_syntax.py`

 * *Files identical despite different names*

