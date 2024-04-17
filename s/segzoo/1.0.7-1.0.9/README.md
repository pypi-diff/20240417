# Comparing `tmp/segzoo-1.0.7.tar.gz` & `tmp/segzoo-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segzoo-1.0.7.tar", last modified: Thu Apr 28 14:06:55 2022, max compression
+gzip compressed data, was "segzoo-1.0.9.tar", last modified: Mon Sep 19 15:32:27 2022, max compression
```

## Comparing `segzoo-1.0.7.tar` & `segzoo-1.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 mickaelm (20914) mhoffma1  (9365)        0 2022-04-28 14:06:55.032443 segzoo-1.0.7/
--rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)    18093 2022-04-08 14:37:57.000000 segzoo-1.0.7/LICENSE.txt
--rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)      185 2022-04-08 14:37:57.000000 segzoo-1.0.7/MANIFEST.in
--rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)     7780 2022-04-28 14:06:55.031443 segzoo-1.0.7/PKG-INFO
--rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)     7176 2022-04-08 14:43:57.000000 segzoo-1.0.7/README.md
-drwxr-xr-x   0 mickaelm (20914) mhoffma1  (9365)        0 2022-04-28 14:06:55.031443 segzoo-1.0.7/segzoo/
--rwxr-xr-x   0 mickaelm (20914) mhoffma1  (9365)     9689 2022-04-14 01:28:45.000000 segzoo-1.0.7/segzoo/Snakefile
--rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)      969 2022-04-08 14:37:57.000000 segzoo-1.0.7/segzoo/__init__.py
--rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)      509 2022-04-08 14:37:57.000000 segzoo-1.0.7/segzoo/create_aggregation_results.py
--rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)     2394 2022-04-08 14:37:57.000000 segzoo-1.0.7/segzoo/create_gene_biotype_gtfs.py
--rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)     2696 2022-04-08 14:37:57.000000 segzoo-1.0.7/segzoo/create_gmtk_results.py
--rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)      695 2022-04-08 14:37:57.000000 segzoo-1.0.7/segzoo/create_nucleotide_results.py
--rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)      490 2022-04-08 14:37:57.000000 segzoo-1.0.7/segzoo/create_overlap_results.py
--rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)     1425 2022-04-08 14:37:57.000000 segzoo-1.0.7/segzoo/gene_biotypes.py
--rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)     3169 2022-04-13 16:18:04.000000 segzoo-1.0.7/segzoo/main.py
--rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)       22 2022-04-22 16:02:55.000000 segzoo-1.0.7/segzoo/version.py
--rwxr-xr-x   0 mickaelm (20914) mhoffma1  (9365)    21920 2022-04-08 14:37:57.000000 segzoo-1.0.7/segzoo/visualization.py
-drwxr-xr-x   0 mickaelm (20914) mhoffma1  (9365)        0 2022-04-28 14:06:55.031443 segzoo-1.0.7/segzoo.egg-info/
--rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)     7780 2022-04-28 14:06:54.000000 segzoo-1.0.7/segzoo.egg-info/PKG-INFO
--rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)      512 2022-04-28 14:06:55.000000 segzoo-1.0.7/segzoo.egg-info/SOURCES.txt
--rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)        1 2022-04-28 14:06:54.000000 segzoo-1.0.7/segzoo.egg-info/dependency_links.txt
--rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)       44 2022-04-28 14:06:54.000000 segzoo-1.0.7/segzoo.egg-info/entry_points.txt
--rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)       81 2022-04-28 14:06:54.000000 segzoo-1.0.7/segzoo.egg-info/requires.txt
--rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)        7 2022-04-28 14:06:54.000000 segzoo-1.0.7/segzoo.egg-info/top_level.txt
--rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)       38 2022-04-28 14:06:55.032443 segzoo-1.0.7/setup.cfg
--rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)     1424 2022-04-22 16:16:07.000000 segzoo-1.0.7/setup.py
+drwxr-xr-x   0 mickaelm (20914) mhoffma1  (9365)        0 2022-09-19 15:32:27.299080 segzoo-1.0.9/
+-rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)    18093 2022-09-16 19:09:51.000000 segzoo-1.0.9/LICENSE.txt
+-rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)      185 2022-09-16 19:09:51.000000 segzoo-1.0.9/MANIFEST.in
+-rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)     7592 2022-09-19 15:32:27.299080 segzoo-1.0.9/PKG-INFO
+-rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)     7022 2022-09-19 14:59:51.000000 segzoo-1.0.9/README.md
+drwxr-xr-x   0 mickaelm (20914) mhoffma1  (9365)        0 2022-09-19 15:32:27.298080 segzoo-1.0.9/segzoo/
+-rwxr-xr-x   0 mickaelm (20914) mhoffma1  (9365)     9689 2022-09-16 19:09:51.000000 segzoo-1.0.9/segzoo/Snakefile
+-rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)      969 2022-09-16 19:09:51.000000 segzoo-1.0.9/segzoo/__init__.py
+-rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)      509 2022-09-16 19:09:51.000000 segzoo-1.0.9/segzoo/create_aggregation_results.py
+-rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)     2394 2022-09-16 19:09:51.000000 segzoo-1.0.9/segzoo/create_gene_biotype_gtfs.py
+-rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)     2696 2022-09-16 19:09:51.000000 segzoo-1.0.9/segzoo/create_gmtk_results.py
+-rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)      695 2022-09-16 19:09:51.000000 segzoo-1.0.9/segzoo/create_nucleotide_results.py
+-rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)      490 2022-09-16 19:09:51.000000 segzoo-1.0.9/segzoo/create_overlap_results.py
+-rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)     1425 2022-09-16 19:09:51.000000 segzoo-1.0.9/segzoo/gene_biotypes.py
+-rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)     3169 2022-09-16 19:09:51.000000 segzoo-1.0.9/segzoo/main.py
+-rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)       22 2022-09-19 15:28:14.000000 segzoo-1.0.9/segzoo/version.py
+-rwxr-xr-x   0 mickaelm (20914) mhoffma1  (9365)    21920 2022-09-16 19:09:51.000000 segzoo-1.0.9/segzoo/visualization.py
+drwxr-xr-x   0 mickaelm (20914) mhoffma1  (9365)        0 2022-09-19 15:32:27.299080 segzoo-1.0.9/segzoo.egg-info/
+-rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)     7592 2022-09-19 15:32:27.000000 segzoo-1.0.9/segzoo.egg-info/PKG-INFO
+-rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)      512 2022-09-19 15:32:27.000000 segzoo-1.0.9/segzoo.egg-info/SOURCES.txt
+-rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)        1 2022-09-19 15:32:27.000000 segzoo-1.0.9/segzoo.egg-info/dependency_links.txt
+-rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)       44 2022-09-19 15:32:27.000000 segzoo-1.0.9/segzoo.egg-info/entry_points.txt
+-rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)       38 2022-09-19 15:32:27.000000 segzoo-1.0.9/segzoo.egg-info/requires.txt
+-rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)        7 2022-09-19 15:32:27.000000 segzoo-1.0.9/segzoo.egg-info/top_level.txt
+-rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)       38 2022-09-19 15:32:27.299080 segzoo-1.0.9/setup.cfg
+-rw-r--r--   0 mickaelm (20914) mhoffma1  (9365)     1346 2022-09-19 14:00:26.000000 segzoo-1.0.9/setup.py
```

### Comparing `segzoo-1.0.7/LICENSE.txt` & `segzoo-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `segzoo-1.0.7/PKG-INFO` & `segzoo-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: segzoo
-Version: 1.0.7
+Version: 1.0.9
 Summary: System for turnkey analysis of semi-automated genome annotations
 Home-page: https://github.com/hoffmangroup/segzoo
 Author: Mickael Mendez
 Author-email: mickael.mendez@mail.utoronto.ca
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
+Requires-Python: ==3.8.*
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Segzoo
 
 ## What is segzoo?
 
@@ -34,21 +32,19 @@
 5. After around 30 min, the resulting visualization will be stored in the current's directory `outdir/plots` folder
 
 
 ## How to install
 
 Segzoo is a python 3 tool, so if you have python 2 installed it is highly recommended for you to install segzoo in a separate python 3 environment.
 Although it can, this tool is not designed to run on a cluster node without internet access, so all the following steps should be done in a local computer.
-To create such an environment run `conda create -n segzooenv python=3.6` where you can change the name of the environment, `segzooenv`.
-Accept all the installation steps.
+To create such an environment run `conda create -n segzooenv python=3.8.* seaborn segtools ggd snakemake pybedtools -y` where you can change the name of the environment, `segzooenv`.
 
-Next, you need to activate this environment. Run `source activate segzooenv` specifying the name of the environment you chose before.
+Next, you need to activate this environment. Run `conda activate segzooenv` specifying the name of the environment you chose before.
 Now that you already are in it, you can install segzoo. You can do that by running `pip install segzoo`,
-which will require you to have bedtools already installed, as it's only in anaconda.
-To install bedtools beforehand you can use `conda install -c bioconda bedtools`.
+
 
 *Note*: currently it's being worked on uploading Segzoo to bioconda.
 When this is finished it will be possible to install it just by using `conda install -c bioconda segzoo` which will take care of all the dependencies.
 
 After accepting all installations, segzoo will be good to go!
 
 ## How to use
@@ -107,8 +103,7 @@
 
 ```csv
 old	new	type
 0	Quiescent	label
 1	TSS	label
 H3K4me3_robust_peaks	H3K4me3	track
 ```
-
```

### Comparing `segzoo-1.0.7/README.md` & `segzoo-1.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -17,21 +17,19 @@
 5. After around 30 min, the resulting visualization will be stored in the current's directory `outdir/plots` folder
 
 
 ## How to install
 
 Segzoo is a python 3 tool, so if you have python 2 installed it is highly recommended for you to install segzoo in a separate python 3 environment.
 Although it can, this tool is not designed to run on a cluster node without internet access, so all the following steps should be done in a local computer.
-To create such an environment run `conda create -n segzooenv python=3.6` where you can change the name of the environment, `segzooenv`.
-Accept all the installation steps.
+To create such an environment run `conda create -n segzooenv python=3.8.* seaborn segtools ggd snakemake pybedtools -y` where you can change the name of the environment, `segzooenv`.
 
-Next, you need to activate this environment. Run `source activate segzooenv` specifying the name of the environment you chose before.
+Next, you need to activate this environment. Run `conda activate segzooenv` specifying the name of the environment you chose before.
 Now that you already are in it, you can install segzoo. You can do that by running `pip install segzoo`,
-which will require you to have bedtools already installed, as it's only in anaconda.
-To install bedtools beforehand you can use `conda install -c bioconda bedtools`.
+
 
 *Note*: currently it's being worked on uploading Segzoo to bioconda.
 When this is finished it will be possible to install it just by using `conda install -c bioconda segzoo` which will take care of all the dependencies.
 
 After accepting all installations, segzoo will be good to go!
 
 ## How to use
```

### Comparing `segzoo-1.0.7/segzoo/Snakefile` & `segzoo-1.0.9/segzoo/Snakefile`

 * *Files identical despite different names*

### Comparing `segzoo-1.0.7/segzoo/__init__.py` & `segzoo-1.0.9/segzoo/__init__.py`

 * *Files identical despite different names*

### Comparing `segzoo-1.0.7/segzoo/create_gene_biotype_gtfs.py` & `segzoo-1.0.9/segzoo/create_gene_biotype_gtfs.py`

 * *Files identical despite different names*

### Comparing `segzoo-1.0.7/segzoo/create_gmtk_results.py` & `segzoo-1.0.9/segzoo/create_gmtk_results.py`

 * *Files identical despite different names*

### Comparing `segzoo-1.0.7/segzoo/create_nucleotide_results.py` & `segzoo-1.0.9/segzoo/create_nucleotide_results.py`

 * *Files identical despite different names*

### Comparing `segzoo-1.0.7/segzoo/gene_biotypes.py` & `segzoo-1.0.9/segzoo/gene_biotypes.py`

 * *Files identical despite different names*

### Comparing `segzoo-1.0.7/segzoo/main.py` & `segzoo-1.0.9/segzoo/main.py`

 * *Files identical despite different names*

### Comparing `segzoo-1.0.7/segzoo/visualization.py` & `segzoo-1.0.9/segzoo/visualization.py`

 * *Files identical despite different names*

### Comparing `segzoo-1.0.7/segzoo.egg-info/PKG-INFO` & `segzoo-1.0.9/segzoo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: segzoo
-Version: 1.0.7
+Version: 1.0.9
 Summary: System for turnkey analysis of semi-automated genome annotations
 Home-page: https://github.com/hoffmangroup/segzoo
 Author: Mickael Mendez
 Author-email: mickael.mendez@mail.utoronto.ca
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
+Requires-Python: ==3.8.*
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Segzoo
 
 ## What is segzoo?
 
@@ -34,21 +32,19 @@
 5. After around 30 min, the resulting visualization will be stored in the current's directory `outdir/plots` folder
 
 
 ## How to install
 
 Segzoo is a python 3 tool, so if you have python 2 installed it is highly recommended for you to install segzoo in a separate python 3 environment.
 Although it can, this tool is not designed to run on a cluster node without internet access, so all the following steps should be done in a local computer.
-To create such an environment run `conda create -n segzooenv python=3.6` where you can change the name of the environment, `segzooenv`.
-Accept all the installation steps.
+To create such an environment run `conda create -n segzooenv python=3.8.* seaborn segtools ggd snakemake pybedtools -y` where you can change the name of the environment, `segzooenv`.
 
-Next, you need to activate this environment. Run `source activate segzooenv` specifying the name of the environment you chose before.
+Next, you need to activate this environment. Run `conda activate segzooenv` specifying the name of the environment you chose before.
 Now that you already are in it, you can install segzoo. You can do that by running `pip install segzoo`,
-which will require you to have bedtools already installed, as it's only in anaconda.
-To install bedtools beforehand you can use `conda install -c bioconda bedtools`.
+
 
 *Note*: currently it's being worked on uploading Segzoo to bioconda.
 When this is finished it will be possible to install it just by using `conda install -c bioconda segzoo` which will take care of all the dependencies.
 
 After accepting all installations, segzoo will be good to go!
 
 ## How to use
@@ -107,8 +103,7 @@
 
 ```csv
 old	new	type
 0	Quiescent	label
 1	TSS	label
 H3K4me3_robust_peaks	H3K4me3	track
 ```
-
```

### Comparing `segzoo-1.0.7/segzoo.egg-info/SOURCES.txt` & `segzoo-1.0.9/segzoo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `segzoo-1.0.7/setup.py` & `segzoo-1.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,17 +23,16 @@
         'Development Status :: 3 - Alpha',
         # 'Intended Audience :: Developers',
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         'Programming Language :: Python :: 3.8'
     ],
     packages=find_packages('.'),
-    install_requires=['matplotlib==3.1.0', 'numpy', 'pandas', 'pysam',
-                      'seaborn', 'segtools', 'snakemake', 'pybedtools', 'scipy'],
-    python_requires='>=3.8',
+    install_requires=['seaborn', 'segtools', 'snakemake', 'pybedtools'],
+    python_requires='==3.8.*',
     package_data={  # Optional
         'segzoo': ['Snakefile'],
     },
     entry_points={  # Optional
         'console_scripts': [
             'segzoo=segzoo.main:main',
         ],
```

