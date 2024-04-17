# Comparing `tmp/vcf2seq-0.4.0a0.tar.gz` & `tmp/vcf2seq-0.4.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcf2seq-0.4.0a0.tar", last modified: Wed Apr 10 14:29:48 2024, max compression
+gzip compressed data, was "vcf2seq-0.4.1a0.tar", last modified: Wed Apr 17 15:30:01 2024, max compression
```

## Comparing `vcf2seq-0.4.0a0.tar` & `vcf2seq-0.4.1a0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-04-10 14:29:48.875322 vcf2seq-0.4.0a0/
--rw-r--r--   0 benoit    (1001) bio2m     (1010)    34916 2023-03-07 08:59:59.000000 vcf2seq-0.4.0a0/LICENCE.md
--rw-r--r--   0 benoit    (1001) bio2m     (1010)       98 2024-04-09 10:58:25.000000 vcf2seq-0.4.0a0/MANIFEST.in
--rw-r--r--   0 benoit    (1001) bio2m     (1010)     2237 2024-04-10 14:29:48.875322 vcf2seq-0.4.0a0/PKG-INFO
--rw-r--r--   0 benoit    (1001) bio2m     (1010)     1645 2024-04-09 07:45:19.000000 vcf2seq-0.4.0a0/README.md
--rw-r--r--   0 benoit    (1001) bio2m     (1010)       38 2024-04-10 14:29:48.875322 vcf2seq-0.4.0a0/setup.cfg
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      990 2024-04-10 14:28:47.000000 vcf2seq-0.4.0a0/setup.py
-drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-04-10 14:29:48.875322 vcf2seq-0.4.0a0/vcf2seq/
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      163 2024-04-09 15:41:02.000000 vcf2seq-0.4.0a0/vcf2seq/__init__.py
--rwxr-xr-x   0 benoit    (1001) bio2m     (1010)     2393 2023-07-13 15:02:22.000000 vcf2seq-0.4.0a0/vcf2seq/ascii.py
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      215 2024-04-09 11:34:21.000000 vcf2seq-0.4.0a0/vcf2seq/info.py
--rwxr-xr-x   0 benoit    (1001) bio2m     (1010)    10887 2024-04-09 08:19:55.000000 vcf2seq-0.4.0a0/vcf2seq/vcf2seq.py
-drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-04-10 14:29:48.875322 vcf2seq-0.4.0a0/vcf2seq.egg-info/
--rw-r--r--   0 benoit    (1001) bio2m     (1010)     2237 2024-04-10 14:29:48.000000 vcf2seq-0.4.0a0/vcf2seq.egg-info/PKG-INFO
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      301 2024-04-10 14:29:48.000000 vcf2seq-0.4.0a0/vcf2seq.egg-info/SOURCES.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)        1 2024-04-10 14:29:48.000000 vcf2seq-0.4.0a0/vcf2seq.egg-info/dependency_links.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)       49 2024-04-10 14:29:48.000000 vcf2seq-0.4.0a0/vcf2seq.egg-info/entry_points.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-04-10 14:29:48.000000 vcf2seq-0.4.0a0/vcf2seq.egg-info/requires.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-04-10 14:29:48.000000 vcf2seq-0.4.0a0/vcf2seq.egg-info/top_level.txt
+drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-04-17 15:30:01.871774 vcf2seq-0.4.1a0/
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)    34916 2023-03-07 08:59:59.000000 vcf2seq-0.4.1a0/LICENCE.md
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)       98 2024-04-09 10:58:25.000000 vcf2seq-0.4.1a0/MANIFEST.in
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)     2198 2024-04-17 15:30:01.871774 vcf2seq-0.4.1a0/PKG-INFO
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)     1606 2024-04-17 15:23:42.000000 vcf2seq-0.4.1a0/README.md
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)       38 2024-04-17 15:30:01.871774 vcf2seq-0.4.1a0/setup.cfg
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      990 2024-04-10 14:28:47.000000 vcf2seq-0.4.1a0/setup.py
+drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-04-17 15:30:01.871774 vcf2seq-0.4.1a0/vcf2seq/
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      163 2024-04-09 15:41:02.000000 vcf2seq-0.4.1a0/vcf2seq/__init__.py
+-rwxr-xr-x   0 benoit    (1001) bio2m     (1010)     2393 2023-07-13 15:02:22.000000 vcf2seq-0.4.1a0/vcf2seq/ascii.py
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      215 2024-04-17 15:29:52.000000 vcf2seq-0.4.1a0/vcf2seq/info.py
+-rwxr-xr-x   0 benoit    (1001) bio2m     (1010)    11029 2024-04-17 15:23:37.000000 vcf2seq-0.4.1a0/vcf2seq/vcf2seq.py
+drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-04-17 15:30:01.871774 vcf2seq-0.4.1a0/vcf2seq.egg-info/
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)     2198 2024-04-17 15:30:01.000000 vcf2seq-0.4.1a0/vcf2seq.egg-info/PKG-INFO
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      301 2024-04-17 15:30:01.000000 vcf2seq-0.4.1a0/vcf2seq.egg-info/SOURCES.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)        1 2024-04-17 15:30:01.000000 vcf2seq-0.4.1a0/vcf2seq.egg-info/dependency_links.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)       49 2024-04-17 15:30:01.000000 vcf2seq-0.4.1a0/vcf2seq.egg-info/entry_points.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-04-17 15:30:01.000000 vcf2seq-0.4.1a0/vcf2seq.egg-info/requires.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-04-17 15:30:01.000000 vcf2seq-0.4.1a0/vcf2seq.egg-info/top_level.txt
```

### Comparing `vcf2seq-0.4.0a0/LICENCE.md` & `vcf2seq-0.4.1a0/LICENCE.md`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.4.0a0/PKG-INFO` & `vcf2seq-0.4.1a0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcf2seq
-Version: 0.4.0a0
+Version: 0.4.1a0
 Summary: like seqTailor, give a VCF file, it return genomic sequence.
 Home-page: https://github.com/bio2m/vcf2seq
 Author: Benoit Guibert
 Author-email: benoit.guibert@inserm.fr
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -16,37 +16,36 @@
 License-File: LICENCE.md
 
 # vcf2seq
 
 
 ## Aim
 
-like seqTailor, give a VCF file, it return genomic sequence.
+Similar to seqtailor [PMID:31045209] : reads a VCF file, outputs a genomic sequence (default length: 31)
+
+Unlike seqtailor, all sequences will have the same length. Moreover, it is possible to have an absence character (by default the dot ` .` ) for indels.
+
+- When a insertion is larger than ``--size`` parameter, only first ``--size`` nucleotides are outputed.
+- Sequence headers are formated as "<chr>_<position>_<ref>_<alt>".
+
+VCF format specifications: https://github.com/samtools/hts-specs/blob/master/VCFv4.4.pdf
+
 
 ## Installation
 
 ```
-pip install vcf2ses
+pip install vcf2seq
 ```
 
 
 ## usage
 
 ```
 usage: vcf2seq.py [-h] -g genome [-s SIZE] [-t {alt,ref,both}] [-b BLANK] [-a ADD_COLUMNS [ADD_COLUMNS ...]] [-o OUTPUT] [-v] vcf
 
-================================================================================
-Like seqtailor, give a VCF file, it return genomic sequence (default length: 31)
-
-Nota:
-- When a insertion is larger than '--size' option, only first '--size' nucleotides are outputed.
-- header ID are formated like "<chr>_<position>_<ref>_<alt>".
-
-VCF format specifications: https://github.com/samtools/hts-specs/blob/master/VCFv4.4.pdf
-================================================================================
 
 positional arguments:
   vcf                   vcf file (mandatory)
 
 options:
   -h, --help            show this help message and exit
   -g genome, --genome genome
```

### Comparing `vcf2seq-0.4.0a0/README.md` & `vcf2seq-0.4.1a0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 # vcf2seq
 
 
 ## Aim
 
-like seqTailor, give a VCF file, it return genomic sequence.
+Similar to seqtailor [PMID:31045209] : reads a VCF file, outputs a genomic sequence (default length: 31)
+
+Unlike seqtailor, all sequences will have the same length. Moreover, it is possible to have an absence character (by default the dot ` .` ) for indels.
+
+- When a insertion is larger than ``--size`` parameter, only first ``--size`` nucleotides are outputed.
+- Sequence headers are formated as "<chr>_<position>_<ref>_<alt>".
+
+VCF format specifications: https://github.com/samtools/hts-specs/blob/master/VCFv4.4.pdf
+
 
 ## Installation
 
 ```
-pip install vcf2ses
+pip install vcf2seq
 ```
 
 
 ## usage
 
 ```
 usage: vcf2seq.py [-h] -g genome [-s SIZE] [-t {alt,ref,both}] [-b BLANK] [-a ADD_COLUMNS [ADD_COLUMNS ...]] [-o OUTPUT] [-v] vcf
 
-================================================================================
-Like seqtailor, give a VCF file, it return genomic sequence (default length: 31)
-
-Nota:
-- When a insertion is larger than '--size' option, only first '--size' nucleotides are outputed.
-- header ID are formated like "<chr>_<position>_<ref>_<alt>".
-
-VCF format specifications: https://github.com/samtools/hts-specs/blob/master/VCFv4.4.pdf
-================================================================================
 
 positional arguments:
   vcf                   vcf file (mandatory)
 
 options:
   -h, --help            show this help message and exit
   -g genome, --genome genome
```

### Comparing `vcf2seq-0.4.0a0/setup.py` & `vcf2seq-0.4.1a0/setup.py`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.4.0a0/vcf2seq/ascii.py` & `vcf2seq-0.4.1a0/vcf2seq/ascii.py`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.4.0a0/vcf2seq/vcf2seq.py` & `vcf2seq-0.4.1a0/vcf2seq/vcf2seq.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 #!/usr/bin/env python3
 
 """
-Like seqtailor, give a VCF file, it return genomic sequence (default length: 31)
+Similar to seqtailor [PMID:31045209] : reads a VCF file, outputs a genomic sequence
+(default length: 31)
 
-Nota:
-- When a insertion is larger than '--size' option, only first '--size' nucleotides are outputed.
-- header ID are formated like "<chr>_<position>_<ref>_<alt>".
+Unlike seqtailor, all sequences will have the same length. Moreover, it is possible to have an
+absence character (by default the dot ` .` ) for indels.
+
+- When a insertion is larger than `--size` parameter, only first `--size` nucleotides are outputed.
+- Sequence headers are formated as "<chr>_<position>_<ref>_<alt>".
 
 VCF format specifications: https://github.com/samtools/hts-specs/blob/master/VCFv4.4.pdf
 """
 
 import sys
 import os
 import argparse
@@ -204,30 +207,29 @@
     parser.add_argument("-g", "--genome",
                         help="genome as fasta file (mandatory)",
                         metavar="genome",
                         required=True,
                        )
     parser.add_argument('-s', '--size',
                         type=int,
-                        help="size of the output sequence (defalt: 31)",
+                        help="size of the output sequence (default: 31)",
                         default=31,
                        )
     parser.add_argument("-t", "--type",
                         type=str,
                         choices=['alt', 'ref', 'both'],
                         default='alt',
                         help="alt, ref, or both output? (default: alt)"
                         )
     parser.add_argument("-b", "--blank",
                         type=str,
                         help="Missing nucleotide character, default is dot (.)",
                         default='.',
                         )
     parser.add_argument("-a", "--add-columns",
-                        # ~ type=int,
                         help="Add one or more columns to header (ex: '-a 3 AA' will add columns "
                              "3 and 27). The first column is '1' (or 'A')",
                         nargs= '+',
                         )
     parser.add_argument("-o", "--output",
                         type=str,
                         help=f"Output file (default: <input_file>-{info.APPNAME}.fa)",
```

### Comparing `vcf2seq-0.4.0a0/vcf2seq.egg-info/PKG-INFO` & `vcf2seq-0.4.1a0/vcf2seq.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcf2seq
-Version: 0.4.0a0
+Version: 0.4.1a0
 Summary: like seqTailor, give a VCF file, it return genomic sequence.
 Home-page: https://github.com/bio2m/vcf2seq
 Author: Benoit Guibert
 Author-email: benoit.guibert@inserm.fr
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -16,37 +16,36 @@
 License-File: LICENCE.md
 
 # vcf2seq
 
 
 ## Aim
 
-like seqTailor, give a VCF file, it return genomic sequence.
+Similar to seqtailor [PMID:31045209] : reads a VCF file, outputs a genomic sequence (default length: 31)
+
+Unlike seqtailor, all sequences will have the same length. Moreover, it is possible to have an absence character (by default the dot ` .` ) for indels.
+
+- When a insertion is larger than ``--size`` parameter, only first ``--size`` nucleotides are outputed.
+- Sequence headers are formated as "<chr>_<position>_<ref>_<alt>".
+
+VCF format specifications: https://github.com/samtools/hts-specs/blob/master/VCFv4.4.pdf
+
 
 ## Installation
 
 ```
-pip install vcf2ses
+pip install vcf2seq
 ```
 
 
 ## usage
 
 ```
 usage: vcf2seq.py [-h] -g genome [-s SIZE] [-t {alt,ref,both}] [-b BLANK] [-a ADD_COLUMNS [ADD_COLUMNS ...]] [-o OUTPUT] [-v] vcf
 
-================================================================================
-Like seqtailor, give a VCF file, it return genomic sequence (default length: 31)
-
-Nota:
-- When a insertion is larger than '--size' option, only first '--size' nucleotides are outputed.
-- header ID are formated like "<chr>_<position>_<ref>_<alt>".
-
-VCF format specifications: https://github.com/samtools/hts-specs/blob/master/VCFv4.4.pdf
-================================================================================
 
 positional arguments:
   vcf                   vcf file (mandatory)
 
 options:
   -h, --help            show this help message and exit
   -g genome, --genome genome
```

