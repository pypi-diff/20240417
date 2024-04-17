# Comparing `tmp/juice_phs-0.4.3-py3-none-any.whl.zip` & `tmp/juice_phs-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,31 +1,32 @@
-Zip file size: 39008 bytes, number of entries: 29
+Zip file size: 40118 bytes, number of entries: 30
 -rw-r--r--  2.0 unx       55 b- defN 23-Oct-03 23:54 phs/__init__.py
 -rw-r--r--  2.0 unx     3962 b- defN 24-Mar-04 13:25 phs/cli.py
 -rw-r--r--  2.0 unx     2548 b- defN 24-Mar-05 13:35 phs/setup.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-01 12:03 phs/geometry/__init__.py
 -rw-r--r--  2.0 unx     9144 b- defN 24-Mar-04 11:19 phs/geometry/derived.py
 -rw-r--r--  2.0 unx    28802 b- defN 24-Apr-10 23:46 phs/geometry/finder.py
 -rw-r--r--  2.0 unx    14098 b- defN 24-Mar-07 15:58 phs/geometry/ray_tracing.py
 -rw-r--r--  2.0 unx     1230 b- defN 24-Mar-05 22:38 phs/geometry/support.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Sep-26 14:51 phs/modelling/__init__.py
 -rw-r--r--  2.0 unx     8621 b- defN 23-Dec-21 13:21 phs/modelling/constraints.py
 -rw-r--r--  2.0 unx    10125 b- defN 24-Jan-15 08:41 phs/modelling/mga.py
 -rw-r--r--  2.0 unx     3111 b- defN 24-Mar-07 15:59 phs/modelling/rpwi.py
 -rw-r--r--  2.0 unx     6641 b- defN 23-Dec-15 14:51 phs/modelling/swi.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-01 12:06 phs/timeline/__init__.py
+-rw-r--r--  2.0 unx     2739 b- defN 24-Apr-17 12:28 phs/timeline/apl.py
 -rw-r--r--  2.0 unx     6371 b- defN 23-Sep-26 14:26 phs/timeline/coverage.py
 -rw-r--r--  2.0 unx     7008 b- defN 24-Feb-05 12:55 phs/timeline/itl.py
 -rw-r--r--  2.0 unx     5823 b- defN 24-Feb-16 13:31 phs/timeline/ptr.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-01 12:05 phs/utils/__init__.py
 -rw-r--r--  2.0 unx    15371 b- defN 23-Dec-21 08:11 phs/utils/coverage.py
 -rw-r--r--  2.0 unx     1599 b- defN 24-Mar-07 17:52 phs/utils/output.py
 -rw-r--r--  2.0 unx     5272 b- defN 24-Jan-09 09:55 phs/utils/plots.py
 -rw-r--r--  2.0 unx      661 b- defN 23-Dec-01 13:29 phs/utils/setup.py
 -rw-r--r--  2.0 unx     5534 b- defN 23-Dec-20 22:53 phs/utils/time.py
--rw-r--r--  2.0 unx       56 b- defN 24-Apr-10 23:53 juice_phs-0.4.3.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     5464 b- defN 24-Apr-10 23:53 juice_phs-0.4.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 23:53 juice_phs-0.4.3.dist-info/WHEEL
--rw-r--r--  2.0 unx      217 b- defN 24-Apr-10 23:53 juice_phs-0.4.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 24-Apr-10 23:53 juice_phs-0.4.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2264 b- defN 24-Apr-10 23:53 juice_phs-0.4.3.dist-info/RECORD
-29 files, 144073 bytes uncompressed, 35414 bytes compressed:  75.4%
+-rw-r--r--  2.0 unx       56 b- defN 24-Apr-17 12:35 juice_phs-0.5.0.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     5464 b- defN 24-Apr-17 12:35 juice_phs-0.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 12:35 juice_phs-0.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      217 b- defN 24-Apr-17 12:35 juice_phs-0.5.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 24-Apr-17 12:35 juice_phs-0.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2340 b- defN 24-Apr-17 12:35 juice_phs-0.5.0.dist-info/RECORD
+30 files, 146888 bytes uncompressed, 36410 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -36,14 +36,17 @@
 
 Filename: phs/modelling/swi.py
 Comment: 
 
 Filename: phs/timeline/__init__.py
 Comment: 
 
+Filename: phs/timeline/apl.py
+Comment: 
+
 Filename: phs/timeline/coverage.py
 Comment: 
 
 Filename: phs/timeline/itl.py
 Comment: 
 
 Filename: phs/timeline/ptr.py
@@ -63,26 +66,26 @@
 
 Filename: phs/utils/setup.py
 Comment: 
 
 Filename: phs/utils/time.py
 Comment: 
 
-Filename: juice_phs-0.4.3.dist-info/LICENSE.md
+Filename: juice_phs-0.5.0.dist-info/LICENSE.md
 Comment: 
 
-Filename: juice_phs-0.4.3.dist-info/METADATA
+Filename: juice_phs-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: juice_phs-0.4.3.dist-info/WHEEL
+Filename: juice_phs-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: juice_phs-0.4.3.dist-info/entry_points.txt
+Filename: juice_phs-0.5.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: juice_phs-0.4.3.dist-info/top_level.txt
+Filename: juice_phs-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: juice_phs-0.4.3.dist-info/RECORD
+Filename: juice_phs-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `juice_phs-0.4.3.dist-info/METADATA` & `juice_phs-0.5.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juice-phs
-Version: 0.4.3
+Version: 0.5.0
 Author: Marc Costa
 Author-email: marc.costa@ext.esa.int
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

## Comparing `juice_phs-0.4.3.dist-info/RECORD` & `juice_phs-0.5.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 phs/geometry/support.py,sha256=Qr_RTuXBxCQJEhTvGH2E7VW7oKFJRwzs5ecOYbYhuLc,1230
 phs/modelling/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 phs/modelling/constraints.py,sha256=MpthALMs5yg8SQ0Q6iSuw0s1FIVfSUNyW4XRzkVWVjw,8621
 phs/modelling/mga.py,sha256=zMWIexDl4VMkAQcL833nFPz_igyJ7DoLA6rwEntCOEA,10125
 phs/modelling/rpwi.py,sha256=39o6pgq0ycvSzknfB227x7fuls4ew0ZYU8aSjBLDBCI,3111
 phs/modelling/swi.py,sha256=6Evb1vEfwA6v9Q2Nyt_JHjj95l8Q-4w2d4_qDLKsRYg,6641
 phs/timeline/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+phs/timeline/apl.py,sha256=IC60jbCsBlC9LM2Qy0NAL9kvN6ZWlu830dv_5mleiqs,2739
 phs/timeline/coverage.py,sha256=svSNgiICjkMy2sWZihaMppmxtXJnvLCbse-yn2rwfMY,6371
 phs/timeline/itl.py,sha256=EkzLTK1e2I_SZ-R4YMVqKIBUALXVeZyHFAvaxwEc38g,7008
 phs/timeline/ptr.py,sha256=xKZvPjBFKfcPxjC6W_jXeLIQuBmt2tTcglaOBbBemGc,5823
 phs/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 phs/utils/coverage.py,sha256=jlKCMEVs3AE0QqrpWGnglWcpo2ywdw01QvFqdrNGjQA,15371
 phs/utils/output.py,sha256=EUVvfNy8kWcET77czR3TtDEaeR611EcQBqTML6Cy7Jg,1599
 phs/utils/plots.py,sha256=M_Iz5biEfh96Yw6Jhunv7DVHtjDYssfxe3mzK538Egk,5272
 phs/utils/setup.py,sha256=A5iZKWDclVIxH4iRiwlRf2M46J0kY-Iq0ulpPUAEm_8,661
 phs/utils/time.py,sha256=0NWfEfniefMahtlnPqEhi9jXZC4pId_YTWwvLIaHMnQ,5534
-juice_phs-0.4.3.dist-info/LICENSE.md,sha256=hRz6pas5P9ZszShrdhry116aE1REe03uSHO4iHa3k8c,56
-juice_phs-0.4.3.dist-info/METADATA,sha256=MkY70B3dmsfcKAQlY9kmWjPjC1zQVW3xuC0lER-nOyA,5464
-juice_phs-0.4.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-juice_phs-0.4.3.dist-info/entry_points.txt,sha256=QqjA-9av7GY3hVbKYQPChh_b2cdZM7VlduHOgTUtWiQ,217
-juice_phs-0.4.3.dist-info/top_level.txt,sha256=8e83LD8AFAocwFttFtG6X2AmXtIVdXb8dKW2RMA8gVY,4
-juice_phs-0.4.3.dist-info/RECORD,,
+juice_phs-0.5.0.dist-info/LICENSE.md,sha256=hRz6pas5P9ZszShrdhry116aE1REe03uSHO4iHa3k8c,56
+juice_phs-0.5.0.dist-info/METADATA,sha256=Z0Rtcxr_0eDDVqopGdem2-zype8fNrEpBTfpHSlKUa4,5464
+juice_phs-0.5.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+juice_phs-0.5.0.dist-info/entry_points.txt,sha256=QqjA-9av7GY3hVbKYQPChh_b2cdZM7VlduHOgTUtWiQ,217
+juice_phs-0.5.0.dist-info/top_level.txt,sha256=8e83LD8AFAocwFttFtG6X2AmXtIVdXb8dKW2RMA8gVY,4
+juice_phs-0.5.0.dist-info/RECORD,,
```

