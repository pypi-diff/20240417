# Comparing `tmp/gemsembler-0.6.3.tar.gz` & `tmp/gemsembler-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemsembler-0.6.3.tar", last modified: Wed Apr 10 08:59:58 2024, max compression
+gzip compressed data, was "gemsembler-0.6.4.tar", last modified: Wed Apr 17 14:50:27 2024, max compression
```

## Comparing `gemsembler-0.6.3.tar` & `gemsembler-0.6.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 08:59:58.832836 gemsembler-0.6.3/
--rw-rw-rw-   0 root         (0) root         (0)     1083 2024-04-10 08:59:46.000000 gemsembler-0.6.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-10 08:59:46.000000 gemsembler-0.6.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4287 2024-04-10 08:59:58.832836 gemsembler-0.6.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1867 2024-04-10 08:59:46.000000 gemsembler-0.6.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-10 08:59:46.000000 gemsembler-0.6.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 08:59:58.832836 gemsembler-0.6.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 08:59:58.821836 gemsembler-0.6.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 08:59:58.825836 gemsembler-0.6.3/src/gemsembler/
--rw-rw-rw-   0 root         (0) root         (0)     1785 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      896 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     7898 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/anticreation.py
--rw-rw-rw-   0 root         (0) root         (0)    19906 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/comparison.py
--rw-rw-rw-   0 root         (0) root         (0)    14845 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)    52270 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/creation.py
--rw-rw-rw-   0 root         (0) root         (0)     4300 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/curation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 08:59:58.826836 gemsembler-0.6.3/src/gemsembler/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 08:59:58.828836 gemsembler-0.6.3/src/gemsembler/data/BU/
--rw-rw-rw-   0 root         (0) root         (0)   180894 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/BU/BU_agora.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   303843 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/BU/BU_carveme_hom.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   381510 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/BU/BU_gapseq.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)    83221 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/BU/BU_modelSEED.sbml.gz
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/BU/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 08:59:58.831836 gemsembler-0.6.3/src/gemsembler/data/LP/
--rw-rw-rw-   0 root         (0) root         (0)   153653 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/LP/LP_CA1.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   157673 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/LP/LP_CA2.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)    82710 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/LP/LP_MS2.sbml.gz
--rw-rw-rw-   0 root         (0) root         (0)   885760 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/LP/LP_WCFS1.fasta.gz
--rw-rw-rw-   0 root         (0) root         (0)   151435 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/LP/LP_WCFS1_agora.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   124883 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/LP/LP_iLP728_revision_data_met_C_c.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   547669 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/LP/LP_protein_fasta.faa.gz
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/LP/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10388 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/dbs.py
--rw-rw-rw-   0 root         (0) root         (0)    19185 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/downstream.py
--rw-rw-rw-   0 root         (0) root         (0)    50045 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/drawing.py
--rw-rw-rw-   0 root         (0) root         (0)    24476 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/gathering.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/general.py
--rw-rw-rw-   0 root         (0) root         (0)    13452 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/genes.py
--rw-rw-rw-   0 root         (0) root         (0)    22859 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/pathsfinding.py
--rw-rw-rw-   0 root         (0) root         (0)     4557 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/periplasmic.py
--rw-rw-rw-   0 root         (0) root         (0)    10165 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/selection.py
--rw-rw-rw-   0 root         (0) root         (0)    31443 2024-04-10 08:59:46.000000 gemsembler-0.6.3/src/gemsembler/structural.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 08:59:58.832836 gemsembler-0.6.3/src/gemsembler.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4287 2024-04-10 08:59:58.000000 gemsembler-0.6.3/src/gemsembler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1435 2024-04-10 08:59:58.000000 gemsembler-0.6.3/src/gemsembler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 08:59:58.000000 gemsembler-0.6.3/src/gemsembler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2024-04-10 08:59:58.000000 gemsembler-0.6.3/src/gemsembler.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      121 2024-04-10 08:59:58.000000 gemsembler-0.6.3/src/gemsembler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-10 08:59:58.000000 gemsembler-0.6.3/src/gemsembler.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 08:59:58.832836 gemsembler-0.6.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)    12691 2024-04-10 08:59:46.000000 gemsembler-0.6.3/tests/test_conversion.py
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-04-10 08:59:46.000000 gemsembler-0.6.3/tests/test_curation.py
--rw-rw-rw-   0 root         (0) root         (0)     4293 2024-04-10 08:59:46.000000 gemsembler-0.6.3/tests/test_dbs.py
--rw-rw-rw-   0 root         (0) root         (0)     4021 2024-04-10 08:59:46.000000 gemsembler-0.6.3/tests/test_gathering.py
--rw-rw-rw-   0 root         (0) root         (0)     2357 2024-04-10 08:59:46.000000 gemsembler-0.6.3/tests/test_selection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:50:27.782412 gemsembler-0.6.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2024-04-17 14:50:14.000000 gemsembler-0.6.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-17 14:50:14.000000 gemsembler-0.6.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4287 2024-04-17 14:50:27.782412 gemsembler-0.6.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2024-04-17 14:50:14.000000 gemsembler-0.6.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-17 14:50:14.000000 gemsembler-0.6.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 14:50:27.782412 gemsembler-0.6.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:50:27.772412 gemsembler-0.6.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:50:27.775412 gemsembler-0.6.4/src/gemsembler/
+-rw-rw-rw-   0 root         (0) root         (0)     1785 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      896 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7898 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/anticreation.py
+-rw-rw-rw-   0 root         (0) root         (0)    19906 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/comparison.py
+-rw-rw-rw-   0 root         (0) root         (0)    14845 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)    52270 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/creation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4300 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/curation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:50:27.776412 gemsembler-0.6.4/src/gemsembler/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:50:27.778412 gemsembler-0.6.4/src/gemsembler/data/BU/
+-rw-rw-rw-   0 root         (0) root         (0)   180894 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/BU/BU_agora.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   303843 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/BU/BU_carveme_hom.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   381510 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/BU/BU_gapseq.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)    83221 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/BU/BU_modelSEED.sbml.gz
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/BU/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:50:27.781412 gemsembler-0.6.4/src/gemsembler/data/LP/
+-rw-rw-rw-   0 root         (0) root         (0)   153653 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/LP/LP_CA1.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   157673 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/LP/LP_CA2.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)    82710 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/LP/LP_MS2.sbml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   885760 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/LP/LP_WCFS1.fasta.gz
+-rw-rw-rw-   0 root         (0) root         (0)   151435 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/LP/LP_WCFS1_agora.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   124883 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/LP/LP_iLP728_revision_data_met_C_c.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   547669 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/LP/LP_protein_fasta.faa.gz
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/LP/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10388 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/dbs.py
+-rw-rw-rw-   0 root         (0) root         (0)    19185 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/downstream.py
+-rw-rw-rw-   0 root         (0) root         (0)    35714 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/drawing.py
+-rw-rw-rw-   0 root         (0) root         (0)    24476 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/gathering.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/general.py
+-rw-rw-rw-   0 root         (0) root         (0)    13452 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/genes.py
+-rw-rw-rw-   0 root         (0) root         (0)    22859 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/pathsfinding.py
+-rw-rw-rw-   0 root         (0) root         (0)     4557 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/periplasmic.py
+-rw-rw-rw-   0 root         (0) root         (0)    10165 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/selection.py
+-rw-rw-rw-   0 root         (0) root         (0)    31443 2024-04-17 14:50:14.000000 gemsembler-0.6.4/src/gemsembler/structural.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:50:27.782412 gemsembler-0.6.4/src/gemsembler.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4287 2024-04-17 14:50:27.000000 gemsembler-0.6.4/src/gemsembler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1435 2024-04-17 14:50:27.000000 gemsembler-0.6.4/src/gemsembler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 14:50:27.000000 gemsembler-0.6.4/src/gemsembler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2024-04-17 14:50:27.000000 gemsembler-0.6.4/src/gemsembler.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      121 2024-04-17 14:50:27.000000 gemsembler-0.6.4/src/gemsembler.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-17 14:50:27.000000 gemsembler-0.6.4/src/gemsembler.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:50:27.782412 gemsembler-0.6.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    12691 2024-04-17 14:50:14.000000 gemsembler-0.6.4/tests/test_conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-04-17 14:50:14.000000 gemsembler-0.6.4/tests/test_curation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4293 2024-04-17 14:50:14.000000 gemsembler-0.6.4/tests/test_dbs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4021 2024-04-17 14:50:14.000000 gemsembler-0.6.4/tests/test_gathering.py
+-rw-rw-rw-   0 root         (0) root         (0)     2357 2024-04-17 14:50:14.000000 gemsembler-0.6.4/tests/test_selection.py
```

### Comparing `gemsembler-0.6.3/LICENSE` & `gemsembler-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/PKG-INFO` & `gemsembler-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemsembler
-Version: 0.6.3
+Version: 0.6.4
 Summary: A tool for assembling and comparing several types of Genome-Scale Metabolic Models.
 Author-email: Elena Matveishina <elena.matveishina@embl.de>, Bartosz Bartmanski <bartosz.bartmanski@embl.de>
 License: MIT License
         
         Copyright (c) 2024 Zimmermann-Kogadeeva Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gemsembler-0.6.3/README.md` & `gemsembler-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/pyproject.toml` & `gemsembler-0.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gemsembler"
-version = "0.6.3"
+version = "0.6.4"
 description = "A tool for assembling and comparing several types of Genome-Scale Metabolic Models."
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
     { name = "Elena Matveishina", email = "elena.matveishina@embl.de" },
     { name = "Bartosz Bartmanski", email = "bartosz.bartmanski@embl.de" }
 ]
@@ -49,15 +49,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 namespaces = true
 where = ["src"]
 
 [tool.bumpver]
-current_version = "0.6.3"
+current_version = "0.6.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `gemsembler-0.6.3/src/gemsembler/__init__.py` & `gemsembler-0.6.4/src/gemsembler/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from importlib.resources import files
 
 from .anticreation import get_model_of_interest
 from .creation import read_supermodel_from_pkl
 from .data import BU, LP
 from .gathering import GatheredModels, load_sbml_model
 
-__version__ = "0.6.3"
+__version__ = "0.6.4"
 
 lp_example = [
     dict(
         model_id="curated_LP",
         path_to_model=files(LP) / "LP_iLP728_revision_data_met_C_c.xml.gz",
         model_type="carveme",
         path_to_genome=files(LP) / "LP_protein_fasta.faa.gz",
```

### Comparing `gemsembler-0.6.3/src/gemsembler/__main__.py` & `gemsembler-0.6.4/src/gemsembler/__main__.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/src/gemsembler/anticreation.py` & `gemsembler-0.6.4/src/gemsembler/anticreation.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/src/gemsembler/comparison.py` & `gemsembler-0.6.4/src/gemsembler/comparison.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/src/gemsembler/conversion.py` & `gemsembler-0.6.4/src/gemsembler/conversion.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/src/gemsembler/creation.py` & `gemsembler-0.6.4/src/gemsembler/creation.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/src/gemsembler/curation.py` & `gemsembler-0.6.4/src/gemsembler/curation.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/src/gemsembler/data/BU/BU_agora.xml.gz` & `gemsembler-0.6.4/src/gemsembler/data/BU/BU_agora.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/src/gemsembler/data/BU/BU_carveme_hom.xml.gz` & `gemsembler-0.6.4/src/gemsembler/data/BU/BU_carveme_hom.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/src/gemsembler/data/BU/BU_gapseq.xml.gz` & `gemsembler-0.6.4/src/gemsembler/data/BU/BU_gapseq.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/src/gemsembler/data/BU/BU_modelSEED.sbml.gz` & `gemsembler-0.6.4/src/gemsembler/data/BU/BU_modelSEED.sbml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/src/gemsembler/data/LP/LP_CA1.xml.gz` & `gemsembler-0.6.4/src/gemsembler/data/LP/LP_CA1.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/src/gemsembler/data/LP/LP_CA2.xml.gz` & `gemsembler-0.6.4/src/gemsembler/data/LP/LP_CA2.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/src/gemsembler/data/LP/LP_MS2.sbml.gz` & `gemsembler-0.6.4/src/gemsembler/data/LP/LP_MS2.sbml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/src/gemsembler/data/LP/LP_WCFS1.fasta.gz` & `gemsembler-0.6.4/src/gemsembler/data/LP/LP_WCFS1.fasta.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/src/gemsembler/data/LP/LP_WCFS1_agora.xml.gz` & `gemsembler-0.6.4/src/gemsembler/data/LP/LP_WCFS1_agora.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/src/gemsembler/data/LP/LP_iLP728_revision_data_met_C_c.xml.gz` & `gemsembler-0.6.4/src/gemsembler/data/LP/LP_iLP728_revision_data_met_C_c.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/src/gemsembler/data/LP/LP_protein_fasta.faa.gz` & `gemsembler-0.6.4/src/gemsembler/data/LP/LP_protein_fasta.faa.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/src/gemsembler/dbs.py` & `gemsembler-0.6.4/src/gemsembler/dbs.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/src/gemsembler/downstream.py` & `gemsembler-0.6.4/src/gemsembler/downstream.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/src/gemsembler/drawing.py` & `gemsembler-0.6.4/src/gemsembler/drawing.py`

 * *Files 21% similar despite different names*

```diff
@@ -934,383 +934,106 @@
                     medium,
                     [k.removesuffix("_path_pfba")],
                     f"{write_output_to_folder}/{k}_{model_id}.html",
                     draw_met_not_int=draw_met_not_int,
                 )
 
 
-def drawCore(
-    supermodel,
-    met_not_int,
-    colorBrewer,
-    name,
-    union=False,
-    directed=False,
-    wid=2000,
-    hei=1000,
-    Nletter=1,
-    union_size=1,
-    core_size=None,
+def draw_met_neighborhood(
+    supermodel: SuperModel,
+    metabolite_id: str,
+    output_name: str,
+    neighborhood_dist=2,
+    highly_connected_t=10,
+    draw_met_not_int=False,
+    genes=True,
+    and_as_solid=False,
+    directed=True,
+    met_not_int=None,
+    n_letter=None,
+    wid=1920,
+    hei=1080,
+    size=25,
 ):
-    g = nx.DiGraph()
-    if union:
-        attribute = "converted"
-        attribute_connect = "union" + str(union_size)
-    else:
-        if core_size:
-            attribute = "core" + str(core_size)
-        else:
-            attribute = "core" + str(len(supermodel.sources))
-        attribute_connect = attribute
-    for r in getattr(supermodel.reactions, attribute).values():
-        if r.id != "Biomass":
-            for rea in r.reactants.get(attribute_connect):
-                tmp_rea = (
-                    rea.id.removesuffix("_c").removesuffix("_e").removesuffix("_p")
+    if metabolite_id not in supermodel.metabolites.assembly.keys():
+        raise ValueError(f"{metabolite_id} is not in the supermodel")
+    if met_not_int is None:
+        met_not_int = {
+            "h": 0,
+            "h2o": 0,
+            "h2": 0,
+            "oh1": 0,
+            "o2": 0,
+            "co2": 0,
+            "coa": 0,
+            "ppi": 0,
+            "pi": 0,
+            "amp": 0,
+            "adp": 0,
+            "atp": 0,
+            "cmp": 0,
+            "cdp": 0,
+            "ctp": 0,
+            "gmp": 0,
+            "gdp": 0,
+            "gtp": 0,
+            "ump": 0,
+            "udp": 0,
+            "utp": 0,
+            "nad": 0,
+            "nadh": 0,
+            "nadp": 0,
+            "nadph": 0,
+            "dadp": 0,
+            "damp": 0,
+            "nh3": 0,
+            "nh4": 0,
+            "fadh2": 0,
+            "fad": 0,
+            "ac": 0,
+            "accoa": 0,
+            "h2s": 0,
+            "HC00250": 0,
+        }
+    all_r = set()
+    med_high_connect = []
+    all_m = [metabolite_id]
+    for i in range(neighborhood_dist):
+        new_all_m = set()
+        for m_id in all_m:
+            tmp_m = re.sub("_([cep])$", "", m_id)
+            if tmp_m in met_not_int.keys():
+                continue
+            met = supermodel.metabolites.assembly.get(m_id)
+            reactions = [r.id for r in met.reactions["assembly"]]
+            if len(reactions) > highly_connected_t:
+                reactions = []
+                med_high_connect.append(re.sub("_([cep])$", "", met.id))
+            all_r = all_r | set(reactions)
+            for r_id in reactions:
+                if r_id == "Biomass":
+                    continue
+                new_all_m = new_all_m | set(
+                    [
+                        m.id
+                        for m in supermodel.reactions.assembly[r_id]
+                        .metabolites["assembly"]
+                        .keys()
+                    ]
                 )
-                for pro in r.products.get(attribute_connect):
-                    tmp_pro = (
-                        pro.id.removesuffix("_c").removesuffix("_e").removesuffix("_p")
-                    )
-                    if (tmp_rea not in met_not_int) & (tmp_pro not in met_not_int):
-                        colname_r = define_node_features(
-                            colorBrewer, "purples", r.id, supermodel.reactions, Nletter
-                        )
-                        colname_rea = define_node_features(
-                            colorBrewer, "reds", rea.id, supermodel.metabolites, Nletter
-                        )
-                        colname_pro = define_node_features(
-                            colorBrewer, "reds", pro.id, supermodel.metabolites, Nletter
-                        )
-                        cn_rea = define_edge_features(
-                            colorBrewer, "purples", rea, r.reactants, Nletter
-                        )
-                        cn_pro = define_edge_features(
-                            colorBrewer, "purples", pro, r.products, Nletter
-                        )
-                        g.add_node(colname_r[1], shape="box", color=colname_r[0])
-                        g.add_node(colname_rea[1], shape="o", color=colname_rea[0])
-                        g.add_node(colname_pro[1], shape="o", color=colname_pro[0])
-                        g.add_edge(
-                            colname_rea[1],
-                            colname_r[1],
-                            color=cn_rea[0],
-                            font_color="black",
-                        )
-                        g.add_edge(
-                            colname_r[1],
-                            colname_pro[1],
-                            color=cn_pro[0],
-                            font_color="black",
-                        )
-
-    pyvis_graph = Network(
-        width="{}px".format(wid),
-        height="{}px".format(hei),
-        directed=directed,
-        notebook=False,
+        all_m = new_all_m
+    draw_one_synt_path(
+        supermodel,
+        list(all_r),
+        med_high_connect,
+        [re.sub("_([cep])$", "", metabolite_id)],
+        output_name,
+        draw_met_not_int,
+        genes,
+        and_as_solid,
+        directed,
+        met_not_int,
+        n_letter,
+        wid,
+        hei,
+        size,
     )
-    pyvis_graph.from_nx(g)
-    pyvis_graph.show("../Output/" + name + ".html")
-    return g
-
-
-def drawMetSynthesis(
-    supermodel,
-    met_not_int: list,
-    colorBrewer: dict,
-    met_of_int: str,
-    paths,
-    sources: list,
-    level: str,
-    name_dir: str,
-    directed=True,
-    wid=2000,
-    hei=1000,
-    Nletter=1,
-):
-    g = nx.DiGraph()
-    r_done = []
-    if type(paths) == list:
-        for path in paths:
-            for r_id in path:
-                if r_id not in r_done:
-                    r = supermodel.reactions.converted.get(r_id)
-                    for rea in r.reactants.get("core1"):
-                        tmp_rea = (
-                            rea.id.removesuffix("_c")
-                            .removesuffix("_e")
-                            .removesuffix("_p")
-                        )
-                        for pro in r.products.get("core1"):
-                            tmp_pro = (
-                                pro.id.removesuffix("_c")
-                                .removesuffix("_e")
-                                .removesuffix("_p")
-                            )
-                            if (tmp_rea not in met_not_int) & (
-                                tmp_pro not in met_not_int
-                            ):
-                                colname_r = define_node_features(
-                                    colorBrewer, "single_path_r", r, Nletter
-                                )
-                                cn_rea = define_edge_features(
-                                    colorBrewer,
-                                    "metabolites",
-                                    rea,
-                                    r,
-                                    r.reactants,
-                                    Nletter,
-                                )
-                                cn_pro = define_edge_features(
-                                    colorBrewer,
-                                    "metabolites",
-                                    pro,
-                                    r,
-                                    r.products,
-                                    Nletter,
-                                )
-                                cn_rea_2 = define_edge_features(
-                                    colorBrewer,
-                                    "single_path_r",
-                                    rea,
-                                    r,
-                                    r.reactants,
-                                    Nletter,
-                                )
-                                cn_pro_2 = define_edge_features(
-                                    colorBrewer,
-                                    "single_path_r",
-                                    pro,
-                                    r,
-                                    r.products,
-                                    Nletter,
-                                )
-                                if (rea.id == met_of_int) or (rea.id in sources):
-                                    colname_rea = define_node_features(
-                                        colorBrewer, "interest", rea, Nletter
-                                    )
-                                else:
-                                    colname_rea = define_node_features(
-                                        colorBrewer, "metabolites", rea, Nletter
-                                    )
-                                if (pro.id == met_of_int) or (pro.id in sources):
-                                    colname_pro = define_node_features(
-                                        colorBrewer, "interest", pro, Nletter
-                                    )
-                                else:
-                                    colname_pro = define_node_features(
-                                        colorBrewer, "metabolites", pro, Nletter
-                                    )
-                                g.add_node(
-                                    colname_r[1], shape="box", color=colname_r[0]
-                                )
-                                g.add_node(
-                                    colname_rea[1], shape="o", color=colname_rea[0]
-                                )
-                                g.add_node(
-                                    colname_pro[1], shape="o", color=colname_pro[0]
-                                )
-                                if r.lower_bound.get(level)[0] >= 0:
-                                    g.add_edge(
-                                        colname_rea[1],
-                                        colname_r[1],
-                                        color=cn_rea[0],
-                                        font_color="black",
-                                    )
-                                    g.add_edge(
-                                        colname_r[1],
-                                        colname_pro[1],
-                                        color=cn_pro_2[0],
-                                        font_color="black",
-                                    )
-                                if r.upper_bound.get(level)[0] <= 0:
-                                    g.add_edge(
-                                        colname_pro[1],
-                                        colname_r[1],
-                                        color=cn_pro[0],
-                                        font_color="black",
-                                    )
-                                    g.add_edge(
-                                        colname_r[1],
-                                        colname_rea[1],
-                                        color=cn_rea_2[0],
-                                        font_color="black",
-                                    )
-                                else:
-                                    g.add_edge(
-                                        colname_rea[1],
-                                        colname_r[1],
-                                        color=cn_rea[0],
-                                        font_color="black",
-                                    )
-                                    g.add_edge(
-                                        colname_r[1],
-                                        colname_pro[1],
-                                        color=cn_pro_2[0],
-                                        font_color="black",
-                                    )
-                                    g.add_edge(
-                                        colname_pro[1],
-                                        colname_r[1],
-                                        color=cn_pro_2[0],
-                                        font_color="black",
-                                    )
-                                    g.add_edge(
-                                        colname_r[1],
-                                        colname_rea[1],
-                                        color=cn_rea[0],
-                                        font_color="black",
-                                    )
-                    r_done.append(r_id)
-        pyvis_graph = Network(
-            width="{}px".format(wid),
-            height="{}px".format(hei),
-            directed=directed,
-            notebook=False,
-        )
-        pyvis_graph.from_nx(g)
-        pyvis_graph.show("../Output/" + name_dir + "/" + met_of_int + ".html")
-    else:
-        print(f"No paths for {met_of_int}, because {paths}")
-    return g
-
-
-def drawMetSynthesis1model(
-    g,
-    col_r,
-    supermodel,
-    met_not_int: list,
-    colorBrewer: dict,
-    met_of_int: str,
-    paths,
-    sources: list,
-    level: str,
-    directed=True,
-    wid=2000,
-    hei=1000,
-    Nletter=1,
-):
-    r_done = []
-    if type(paths) == list:
-        for path in paths:
-            for r_id in path:
-                if r_id not in r_done:
-                    r = supermodel.reactions.converted.get(r_id)
-                    for rea in r.reactants.get("core1"):
-                        tmp_rea = (
-                            rea.id.removesuffix("_c")
-                            .removesuffix("_e")
-                            .removesuffix("_p")
-                        )
-                        for pro in r.products.get("core1"):
-                            tmp_pro = (
-                                pro.id.removesuffix("_c")
-                                .removesuffix("_e")
-                                .removesuffix("_p")
-                            )
-                            if (tmp_rea not in met_not_int) & (
-                                tmp_pro not in met_not_int
-                            ):
-                                colname_r = define_node_features(
-                                    colorBrewer, col_r, r, Nletter
-                                )
-                                cn_rea = define_edge_features(
-                                    colorBrewer,
-                                    "metabolites",
-                                    rea,
-                                    r,
-                                    r.reactants,
-                                    Nletter,
-                                )
-                                cn_pro = define_edge_features(
-                                    colorBrewer,
-                                    "metabolites",
-                                    pro,
-                                    r,
-                                    r.products,
-                                    Nletter,
-                                )
-                                cn_rea_2 = define_edge_features(
-                                    colorBrewer, col_r, rea, r, r.reactants, Nletter
-                                )
-                                cn_pro_2 = define_edge_features(
-                                    colorBrewer, col_r, pro, r, r.products, Nletter
-                                )
-                                if (rea.id == met_of_int) or (rea.id in sources):
-                                    colname_rea = define_node_features(
-                                        colorBrewer, "interest", rea, Nletter
-                                    )
-                                else:
-                                    colname_rea = define_node_features(
-                                        colorBrewer, "metabolites", rea, Nletter
-                                    )
-                                if (pro.id == met_of_int) or (pro.id in sources):
-                                    colname_pro = define_node_features(
-                                        colorBrewer, "interest", pro, Nletter
-                                    )
-                                else:
-                                    colname_pro = define_node_features(
-                                        colorBrewer, "metabolites", pro, Nletter
-                                    )
-                                g.add_node(
-                                    colname_r[1], shape="box", color=colname_r[0]
-                                )
-                                g.add_node(
-                                    colname_rea[1], shape="o", color=colname_rea[0]
-                                )
-                                g.add_node(
-                                    colname_pro[1], shape="o", color=colname_pro[0]
-                                )
-                                if r.lower_bound.get(level)[0] >= 0:
-                                    g.add_edge(
-                                        colname_rea[1],
-                                        colname_r[1],
-                                        color=cn_rea[0],
-                                        font_color="black",
-                                    )
-                                    g.add_edge(
-                                        colname_r[1],
-                                        colname_pro[1],
-                                        color=cn_pro_2[0],
-                                        font_color="black",
-                                    )
-                                if r.upper_bound.get(level)[0] <= 0:
-                                    g.add_edge(
-                                        colname_pro[1],
-                                        colname_r[1],
-                                        color=cn_pro[0],
-                                        font_color="black",
-                                    )
-                                    g.add_edge(
-                                        colname_r[1],
-                                        colname_rea[1],
-                                        color=cn_rea_2[0],
-                                        font_color="black",
-                                    )
-                                else:
-                                    g.add_edge(
-                                        colname_rea[1],
-                                        colname_r[1],
-                                        color=cn_rea[0],
-                                        font_color="black",
-                                    )
-                                    g.add_edge(
-                                        colname_r[1],
-                                        colname_pro[1],
-                                        color=cn_pro_2[0],
-                                        font_color="black",
-                                    )
-                                    g.add_edge(
-                                        colname_pro[1],
-                                        colname_r[1],
-                                        color=cn_pro_2[0],
-                                        font_color="black",
-                                    )
-                                    g.add_edge(
-                                        colname_r[1],
-                                        colname_rea[1],
-                                        color=cn_rea[0],
-                                        font_color="black",
-                                    )
-                    r_done.append(r_id)
-    return g
```

### Comparing `gemsembler-0.6.3/src/gemsembler/gathering.py` & `gemsembler-0.6.4/src/gemsembler/gathering.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/src/gemsembler/genes.py` & `gemsembler-0.6.4/src/gemsembler/genes.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/src/gemsembler/pathsfinding.py` & `gemsembler-0.6.4/src/gemsembler/pathsfinding.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/src/gemsembler/periplasmic.py` & `gemsembler-0.6.4/src/gemsembler/periplasmic.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/src/gemsembler/selection.py` & `gemsembler-0.6.4/src/gemsembler/selection.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/src/gemsembler/structural.py` & `gemsembler-0.6.4/src/gemsembler/structural.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/src/gemsembler.egg-info/PKG-INFO` & `gemsembler-0.6.4/src/gemsembler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemsembler
-Version: 0.6.3
+Version: 0.6.4
 Summary: A tool for assembling and comparing several types of Genome-Scale Metabolic Models.
 Author-email: Elena Matveishina <elena.matveishina@embl.de>, Bartosz Bartmanski <bartosz.bartmanski@embl.de>
 License: MIT License
         
         Copyright (c) 2024 Zimmermann-Kogadeeva Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gemsembler-0.6.3/src/gemsembler.egg-info/SOURCES.txt` & `gemsembler-0.6.4/src/gemsembler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/tests/test_conversion.py` & `gemsembler-0.6.4/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/tests/test_curation.py` & `gemsembler-0.6.4/tests/test_curation.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/tests/test_dbs.py` & `gemsembler-0.6.4/tests/test_dbs.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/tests/test_gathering.py` & `gemsembler-0.6.4/tests/test_gathering.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.3/tests/test_selection.py` & `gemsembler-0.6.4/tests/test_selection.py`

 * *Files identical despite different names*

