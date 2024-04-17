# Comparing `tmp/zhmiscellany-2.0.6-py3-none-any.whl.zip` & `tmp/zhmiscellany-2.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 20158 bytes, number of entries: 18
+Zip file size: 20157 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat      236 b- defN 24-Apr-15 13:40 zhmiscellany/__init__.py
 -rw-rw-rw-  2.0 fat     6520 b- defN 23-Dec-08 14:13 zhmiscellany/_discord_supportfuncs.py
 -rw-rw-rw-  2.0 fat      673 b- defN 23-Nov-05 00:34 zhmiscellany/_misc_supportfuncs.py
 -rw-rw-rw-  2.0 fat       81 b- defN 23-Nov-01 22:45 zhmiscellany/dict.py
 -rw-rw-rw-  2.0 fat    15608 b- defN 24-Mar-07 15:37 zhmiscellany/discord.py
 -rw-rw-rw-  2.0 fat     4256 b- defN 23-Nov-01 20:01 zhmiscellany/fileio.py
 -rw-rw-rw-  2.0 fat      338 b- defN 23-Oct-31 21:16 zhmiscellany/image.py
 -rw-rw-rw-  2.0 fat      854 b- defN 23-Nov-14 14:55 zhmiscellany/list.py
 -rw-rw-rw-  2.0 fat      632 b- defN 23-Nov-18 07:12 zhmiscellany/math.py
 -rw-rw-rw-  2.0 fat     4531 b- defN 24-Apr-15 16:39 zhmiscellany/misc.py
 -rw-rw-rw-  2.0 fat     1685 b- defN 24-Apr-15 15:15 zhmiscellany/netio.py
 -rw-rw-rw-  2.0 fat     3807 b- defN 24-Apr-15 17:36 zhmiscellany/pipes.py
 -rw-rw-rw-  2.0 fat      761 b- defN 24-Feb-12 17:09 zhmiscellany/processing.py
 -rw-rw-rw-  2.0 fat     2412 b- defN 23-Nov-18 07:28 zhmiscellany/string.py
--rw-rw-rw-  2.0 fat    18893 b- defN 24-Apr-15 17:37 zhmiscellany-2.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-15 17:37 zhmiscellany-2.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-15 17:37 zhmiscellany-2.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1441 b- defN 24-Apr-15 17:37 zhmiscellany-2.0.6.dist-info/RECORD
-18 files, 62833 bytes uncompressed, 17810 bytes compressed:  71.7%
+-rw-rw-rw-  2.0 fat    18861 b- defN 24-Apr-17 10:19 zhmiscellany-2.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-17 10:19 zhmiscellany-2.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-17 10:19 zhmiscellany-2.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1441 b- defN 24-Apr-17 10:19 zhmiscellany-2.0.7.dist-info/RECORD
+18 files, 62801 bytes uncompressed, 17809 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: zhmiscellany/processing.py
 Comment: 
 
 Filename: zhmiscellany/string.py
 Comment: 
 
-Filename: zhmiscellany-2.0.6.dist-info/METADATA
+Filename: zhmiscellany-2.0.7.dist-info/METADATA
 Comment: 
 
-Filename: zhmiscellany-2.0.6.dist-info/WHEEL
+Filename: zhmiscellany-2.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: zhmiscellany-2.0.6.dist-info/top_level.txt
+Filename: zhmiscellany-2.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: zhmiscellany-2.0.6.dist-info/RECORD
+Filename: zhmiscellany-2.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `zhmiscellany-2.0.6.dist-info/METADATA` & `zhmiscellany-2.0.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: zhmiscellany
-Version: 2.0.6
+Version: 2.0.7
 Summary: A collection of useful/interesting python libraries made by zh.
 Home-page: https://discord.gg/ThBBAuueVJ
 Author: zh
 Author-email: imnotgivingmyemailjustaddmeondiscordmydiscordisz_h_@zh.com
 Project-URL: Bug Tracker, https://github.com/zen-ham/zhmiscellany/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pycryptodome >=0
 Requires-Dist: pywin32 >=0
 Requires-Dist: discum ==1.1.0
 Requires-Dist: Requests >=0
-Requires-Dist: pytesseract >=0
 Requires-Dist: random-header-generator >=0
 
 `zhmiscellany`,
 ===
 
 An organized collection of unique and useful functions/classes/modules.
 ---
```

## Comparing `zhmiscellany-2.0.6.dist-info/RECORD` & `zhmiscellany-2.0.7.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 zhmiscellany/list.py,sha256=2kqsscSFXEanmEdR1NuwWaf2l8nPTDUgRyrfL1snoRg,854
 zhmiscellany/math.py,sha256=v2WmHdKrwsrY08E6yUgb0nPHbTuyrljRdgUMw5uqu3U,632
 zhmiscellany/misc.py,sha256=JlibUEtNHc3nHDnlgyOE3050SIQkcMMedPK8WZookNU,4531
 zhmiscellany/netio.py,sha256=4dKBJp-fq_jnuDcwrag6kH7WZncnERPPtuCmGcdFAt0,1685
 zhmiscellany/pipes.py,sha256=lpP6wVVa6J6GW1SZtVEv9LWuRlZZ31rL7TIdMrInNK0,3807
 zhmiscellany/processing.py,sha256=pE2LVtaZwBvWgd6Xx0S_ZT0WhcKr6GtBhjAfbAflSYo,761
 zhmiscellany/string.py,sha256=2xL_rbJeiGH14k_JkXWUp-oBN30Ltl9-bZk0eHUPltA,2412
-zhmiscellany-2.0.6.dist-info/METADATA,sha256=_ngkfewoot4lbale7J7noYO--o73Oy_372NuNNLS8pQ,18893
-zhmiscellany-2.0.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-zhmiscellany-2.0.6.dist-info/top_level.txt,sha256=ioDtsrevCI52rTxZntMPljRIBsZs73tD0hI00HektiE,13
-zhmiscellany-2.0.6.dist-info/RECORD,,
+zhmiscellany-2.0.7.dist-info/METADATA,sha256=u5pf0I5VEsRow-5zwioNimc-K76JtMAczRfFj2ZINvA,18861
+zhmiscellany-2.0.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+zhmiscellany-2.0.7.dist-info/top_level.txt,sha256=ioDtsrevCI52rTxZntMPljRIBsZs73tD0hI00HektiE,13
+zhmiscellany-2.0.7.dist-info/RECORD,,
```

