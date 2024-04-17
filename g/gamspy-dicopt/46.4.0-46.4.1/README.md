# Comparing `tmp/gamspy_dicopt-46.4.0-py3-none-win_amd64.whl.zip` & `tmp/gamspy_dicopt-46.4.1-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 199565 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat      322 b- defN 24-Apr-04 14:13 gamspy_dicopt/__init__.py
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-04 14:13 gamspy_dicopt/gmsdi_nt.cmd
--rw-rw-rw-  2.0 fat   544768 b- defN 24-Apr-04 14:13 gamspy_dicopt/gmsdi_nx.exe
--rw-rw-rw-  2.0 fat     4787 b- defN 24-Apr-04 14:13 gamspy_dicopt/optdicopt.def
--rw-rw-rw-  2.0 fat       22 b- defN 24-Apr-04 14:13 gamspy_dicopt/version.py
--rw-rw-rw-  2.0 fat       63 b- defN 24-Apr-04 14:13 gamspy_dicopt-46.4.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      104 b- defN 24-Apr-04 14:13 gamspy_dicopt-46.4.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 24-Apr-04 14:13 gamspy_dicopt-46.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      735 b- defN 24-Apr-04 14:13 gamspy_dicopt-46.4.0.dist-info/RECORD
-9 files, 550907 bytes uncompressed, 198291 bytes compressed:  64.0%
+Zip file size: 199564 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat      322 b- defN 24-Apr-17 09:01 gamspy_dicopt/__init__.py
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-17 09:01 gamspy_dicopt/gmsdi_nt.cmd
+-rw-rw-rw-  2.0 fat   544768 b- defN 24-Apr-17 09:01 gamspy_dicopt/gmsdi_nx.exe
+-rw-rw-rw-  2.0 fat     4787 b- defN 24-Apr-17 09:01 gamspy_dicopt/optdicopt.def
+-rw-rw-rw-  2.0 fat       22 b- defN 24-Apr-17 09:01 gamspy_dicopt/version.py
+-rw-rw-rw-  2.0 fat       63 b- defN 24-Apr-17 09:01 gamspy_dicopt-46.4.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      104 b- defN 24-Apr-17 09:01 gamspy_dicopt-46.4.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 24-Apr-17 09:01 gamspy_dicopt-46.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      735 b- defN 24-Apr-17 09:01 gamspy_dicopt-46.4.1.dist-info/RECORD
+9 files, 550907 bytes uncompressed, 198290 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: gamspy_dicopt/optdicopt.def
 Comment: 
 
 Filename: gamspy_dicopt/version.py
 Comment: 
 
-Filename: gamspy_dicopt-46.4.0.dist-info/METADATA
+Filename: gamspy_dicopt-46.4.1.dist-info/METADATA
 Comment: 
 
-Filename: gamspy_dicopt-46.4.0.dist-info/WHEEL
+Filename: gamspy_dicopt-46.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: gamspy_dicopt-46.4.0.dist-info/top_level.txt
+Filename: gamspy_dicopt-46.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: gamspy_dicopt-46.4.0.dist-info/RECORD
+Filename: gamspy_dicopt-46.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gamspy_dicopt/gmsdi_nx.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140070640
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr  2 07:57:27 2024
+Time/Date		Tue Apr 16 08:16:10 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000071e00
 SizeOfInitializedData	0000000000017600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000070640
@@ -122747,15 +122747,16 @@
    14007e613:	rex add %eax,(%rax)
    14007e616:	add    %al,(%rax)
    14007e618:	shlb   $0x40,0x8(%rax)
    14007e61c:	add    %eax,(%rax)
    14007e61e:	add    %al,(%rax)
    14007e620:	add    %al,(%rax)
    14007e622:	add    %al,(%rax)
-   14007e624:	addr32 mov $0x660b,%edx
+   14007e624:	lret   $0x1e33
+   14007e627:	data16 add %al,(%rax)
    14007e62a:	add    %al,(%rax)
    14007e62c:	or     $0x90000000,%eax
    14007e631:	add    (%rax),%al
    14007e633:	add    %bl,-0x67fff819(%rax)
    14007e639:	flds   (%rdi)
    14007e63b:	add    %al,(%rax)
    14007e63d:	add    %al,(%rax)
```

## gamspy_dicopt/version.py

```diff
@@ -1 +1 @@
-__version__ = '46.4.0'
+__version__ = '46.4.1'
```

## Comparing `gamspy_dicopt-46.4.0.dist-info/RECORD` & `gamspy_dicopt-46.4.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 gamspy_dicopt/__init__.py,sha256=h-VSFs3t80tfczPH_L-YDAmm8FHHqh3zI4svwb8HqZU,322
 gamspy_dicopt/gmsdi_nt.cmd,sha256=kkdjYr0OiEFswKqyYItwfrTtQSF31ZrthCM2gJQ3v3E,92
-gamspy_dicopt/gmsdi_nx.exe,sha256=TI6jMAZkbgNpRNlOnfIJjR5Aq2Rl6lPSuV4AQ1Lo5Ng,544768
+gamspy_dicopt/gmsdi_nx.exe,sha256=IkC8SPOu90B0wBwP0JRZZUB3pVHHTPOWzTIH-fWKB_0,544768
 gamspy_dicopt/optdicopt.def,sha256=7HMCf4XUqNz4mKo7uHwsc6p4QS3H-r-Fk545l2GIosI,4787
-gamspy_dicopt/version.py,sha256=aPpKdDaOIvtNrT9mpHftLgRfZ1X1uLWURDzyhZyW1zI,22
-gamspy_dicopt-46.4.0.dist-info/METADATA,sha256=55SzAb94OvOmtX9Tvfn9B6RtxL3SdHOpl7vlf-kiKyM,63
-gamspy_dicopt-46.4.0.dist-info/WHEEL,sha256=-H981hu6jK6YKd-c0qWpYxXA3UZMihQ3r30_4YPQguI,104
-gamspy_dicopt-46.4.0.dist-info/top_level.txt,sha256=ILTBzffzbwuSjw3592ZR4ep11uEYxZd-gVMNpEiJXYs,14
-gamspy_dicopt-46.4.0.dist-info/RECORD,,
+gamspy_dicopt/version.py,sha256=PfEsnAfLuXVTA7hSNu9m9ueNe8npaTtOAv06fL-xeY4,22
+gamspy_dicopt-46.4.1.dist-info/METADATA,sha256=pLt8z1_bVmOxDI61gQAXWqPOzwZKxyXM3ShTkQk5-Q4,63
+gamspy_dicopt-46.4.1.dist-info/WHEEL,sha256=-H981hu6jK6YKd-c0qWpYxXA3UZMihQ3r30_4YPQguI,104
+gamspy_dicopt-46.4.1.dist-info/top_level.txt,sha256=ILTBzffzbwuSjw3592ZR4ep11uEYxZd-gVMNpEiJXYs,14
+gamspy_dicopt-46.4.1.dist-info/RECORD,,
```

