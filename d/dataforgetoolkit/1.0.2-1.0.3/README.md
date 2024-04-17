# Comparing `tmp/dataforgetoolkit-1.0.2-py3-none-any.whl.zip` & `tmp/dataforgetoolkit-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3155 bytes, number of entries: 7
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 07:17 dataforgetoolkit/__init__.py
+Zip file size: 4028 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      875 b- defN 24-Apr-17 09:58 dataforgetoolkit/__init__.py
 -rw-r--r--  2.0 unx      212 b- defN 24-Apr-17 09:19 dataforgetoolkit/common_utils.py
 -rw-r--r--  2.0 unx     3694 b- defN 24-Apr-17 09:21 dataforgetoolkit/datamapper.py
--rw-r--r--  2.0 unx      865 b- defN 24-Apr-17 09:22 dataforgetoolkit-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 09:22 dataforgetoolkit-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-17 09:22 dataforgetoolkit-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      590 b- defN 24-Apr-17 09:22 dataforgetoolkit-1.0.2.dist-info/RECORD
-7 files, 5470 bytes uncompressed, 2093 bytes compressed:  61.7%
+-rw-r--r--  2.0 unx     2003 b- defN 24-Apr-17 10:13 dataforgetoolkit-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 10:13 dataforgetoolkit-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 24-Apr-17 10:13 dataforgetoolkit-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      593 b- defN 24-Apr-17 10:13 dataforgetoolkit-1.0.3.dist-info/RECORD
+7 files, 7486 bytes uncompressed, 2966 bytes compressed:  60.4%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: dataforgetoolkit/common_utils.py
 Comment: 
 
 Filename: dataforgetoolkit/datamapper.py
 Comment: 
 
-Filename: dataforgetoolkit-1.0.2.dist-info/METADATA
+Filename: dataforgetoolkit-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: dataforgetoolkit-1.0.2.dist-info/WHEEL
+Filename: dataforgetoolkit-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: dataforgetoolkit-1.0.2.dist-info/top_level.txt
+Filename: dataforgetoolkit-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: dataforgetoolkit-1.0.2.dist-info/RECORD
+Filename: dataforgetoolkit-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dataforgetoolkit/__init__.py

```diff
@@ -0,0 +1,55 @@
+00000000: 2320 496d 706f 7274 206e 6563 6573 7361  # Import necessa
+00000010: 7279 206d 6f64 756c 6573 2f63 6c61 7373  ry modules/class
+00000020: 6573 2f66 756e 6374 696f 6e73 2066 6f72  es/functions for
+00000030: 2065 6173 7920 6163 6365 7373 2077 6865   easy access whe
+00000040: 6e20 7468 6520 6c69 6272 6172 7920 6973  n the library is
+00000050: 2069 6d70 6f72 7465 640a 6672 6f6d 202e   imported.from .
+00000060: 6461 7461 6d61 7070 6572 2069 6d70 6f72  datamapper impor
+00000070: 7420 6d61 700a 6672 6f6d 202e 636f 6d6d  t map.from .comm
+00000080: 6f6e 5f75 7469 6c73 2069 6d70 6f72 7420  on_utils import 
+00000090: 4445 4641 554c 545f 5641 4c55 452c 2046  DEFAULT_VALUE, F
+000000a0: 494c 5445 525f 5641 4c55 450a 0a23 204c  ILTER_VALUE..# L
+000000b0: 6973 7420 6f66 206e 616d 6573 2074 6f20  ist of names to 
+000000c0: 6265 2065 7870 6f72 7465 6420 7768 656e  be exported when
+000000d0: 2075 7369 6e67 2060 6672 6f6d 2064 6174   using `from dat
+000000e0: 6166 6f72 6765 746f 6f6c 6b69 7420 696d  aforgetoolkit im
+000000f0: 706f 7274 202a 600a 5f5f 616c 6c5f 5f20  port *`.__all__ 
+00000100: 3d20 5b27 6d61 7027 2c20 2744 4546 4155  = ['map', 'DEFAU
+00000110: 4c54 5f56 414c 5545 272c 2027 4649 4c54  LT_VALUE', 'FILT
+00000120: 4552 5f56 414c 5545 272c 2252 4550 4c41  ER_VALUE',"REPLA
+00000130: 4345 5f56 414c 5545 222c 2243 4f4e 4341  CE_VALUE","CONCA
+00000140: 545f 5641 4c55 4522 2c22 5550 5045 5243  T_VALUE","UPPERC
+00000150: 4153 455f 5641 4c55 4522 2c22 4c4f 5745  ASE_VALUE","LOWE
+00000160: 5243 4153 455f 5641 4c55 4522 5d0a 0a23  RCASE_VALUE"]..#
+00000170: 2041 7574 686f 7220 696e 666f 726d 6174   Author informat
+00000180: 696f 6e0a 5f5f 6175 7468 6f72 5f5f 203d  ion.__author__ =
+00000190: 2022 416d 6974 2053 696e 6768 220a 0a23   "Amit Singh"..#
+000001a0: 5075 7270 6f73 6520 6f66 2074 6865 206c  Purpose of the l
+000001b0: 6962 7261 7279 0a5f 5f64 6f63 5f5f 203d  ibrary.__doc__ =
+000001c0: 2022 2222 0a44 6174 6146 6f72 6765 546f   """.DataForgeTo
+000001d0: 6f6c 6b69 743a 2041 206c 6962 7261 7279  olkit: A library
+000001e0: 2066 6f72 206d 6170 7069 6e67 2043 5356   for mapping CSV
+000001f0: 206f 7220 4578 6365 6c20 6669 6c65 7320   or Excel files 
+00000200: 6261 7365 6420 6f6e 204a 534f 4e20 7472  based on JSON tr
+00000210: 616e 7366 6f72 6d61 7469 6f6e 206d 6170  ansformation map
+00000220: 7069 6e67 732e 0a0a 5573 6167 653a 0a20  pings...Usage:. 
+00000230: 2020 2069 6d70 6f72 7420 6461 7461 666f     import datafo
+00000240: 7267 6574 6f6f 6c6b 6974 0a0a 2020 2020  rgetoolkit..    
+00000250: 2320 4d61 7020 6120 4353 5620 6f72 2045  # Map a CSV or E
+00000260: 7863 656c 2066 696c 6520 6261 7365 6420  xcel file based 
+00000270: 6f6e 2061 204a 534f 4e20 7472 616e 7366  on a JSON transf
+00000280: 6f72 6d61 7469 6f6e 206d 6170 7069 6e67  ormation mapping
+00000290: 0a20 2020 206d 6170 7065 645f 6461 7461  .    mapped_data
+000002a0: 203d 2064 6174 6166 6f72 6765 746f 6f6c   = dataforgetool
+000002b0: 6b69 742e 6d61 7028 7265 706f 7274 5f66  kit.map(report_f
+000002c0: 696c 655f 7061 7468 2c20 7472 616e 7366  ile_path, transf
+000002d0: 6f72 6d61 7469 6f6e 5f66 696c 655f 7061  ormation_file_pa
+000002e0: 7468 290a 0a20 2020 2023 2041 6363 6573  th)..    # Acces
+000002f0: 7320 636f 6d6d 6f6e 2075 7469 6c69 7469  s common utiliti
+00000300: 6573 0a20 2020 2064 6566 6175 6c74 5f76  es.    default_v
+00000310: 616c 7565 203d 2064 6174 6166 6f72 6765  alue = dataforge
+00000320: 746f 6f6c 6b69 742e 4445 4641 554c 545f  toolkit.DEFAULT_
+00000330: 5641 4c55 450a 2020 2020 6669 6c74 6572  VALUE.    filter
+00000340: 5f76 616c 7565 203d 2064 6174 6166 6f72  _value = datafor
+00000350: 6765 746f 6f6c 6b69 742e 4649 4c54 4552  getoolkit.FILTER
+00000360: 5f56 414c 5545 0a22 2222 0a              _VALUE.""".
```

## Comparing `dataforgetoolkit-1.0.2.dist-info/RECORD` & `dataforgetoolkit-1.0.3.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-dataforgetoolkit/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+dataforgetoolkit/__init__.py,sha256=zkyUri73xFqI869Ok73yH2SidWrsS7D7a7y0foTFatE,875
 dataforgetoolkit/common_utils.py,sha256=pjPA-SU6f8V_l6ICe9YLmLUVxvlWJQeIOLyvBJXTjDs,212
 dataforgetoolkit/datamapper.py,sha256=xnjB3__KSsEiH3d-KVCf62rHh-AD2U2ZjOCcpO1t3Cg,3694
-dataforgetoolkit-1.0.2.dist-info/METADATA,sha256=oVszjc5555-oufAKfy4sJ2rCc9DZQdfV33_QnGKvSA8,865
-dataforgetoolkit-1.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-dataforgetoolkit-1.0.2.dist-info/top_level.txt,sha256=WL_asJIhhKds6gBhWlc8rIVvUF_KWPJ03uzY92r6tcg,17
-dataforgetoolkit-1.0.2.dist-info/RECORD,,
+dataforgetoolkit-1.0.3.dist-info/METADATA,sha256=5Q5lUAjVTiynf4bZ_iW5psaJk9zxwZP9xRb0Qhmk89w,2003
+dataforgetoolkit-1.0.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+dataforgetoolkit-1.0.3.dist-info/top_level.txt,sha256=WL_asJIhhKds6gBhWlc8rIVvUF_KWPJ03uzY92r6tcg,17
+dataforgetoolkit-1.0.3.dist-info/RECORD,,
```

