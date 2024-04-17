# Comparing `tmp/nanoCEM-0.0.5.6.tar.gz` & `tmp/nanoCEM-0.0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nanoCEM-0.0.5.6.tar", last modified: Tue Apr 16 08:18:55 2024, max compression
+gzip compressed data, was "dist/nanoCEM-0.0.5.7.tar", last modified: Tue Apr 16 08:40:58 2024, max compression
```

## Comparing `nanoCEM-0.0.5.6.tar` & `nanoCEM-0.0.5.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-04-16 08:18:55.164478 nanoCEM-0.0.5.6/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.5.6/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2730 2024-04-16 08:18:55.164478 nanoCEM-0.0.5.6/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2100 2024-03-07 07:08:59.000000 nanoCEM-0.0.5.6/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-04-16 08:18:55.164478 nanoCEM-0.0.5.6/nanoCEM/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    15641 2024-04-16 08:04:15.000000 nanoCEM-0.0.5.6/nanoCEM/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5416 2023-12-21 04:37:40.000000 nanoCEM-0.0.5.6/nanoCEM/NEW_TRAINER.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.5.6/nanoCEM/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4547 2023-12-10 10:36:58.000000 nanoCEM-0.0.5.6/nanoCEM/alignment_feature_camera.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10849 2024-04-16 04:27:47.000000 nanoCEM-0.0.5.6/nanoCEM/alignment_magnifier
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    14691 2024-04-16 08:18:09.000000 nanoCEM-0.0.5.6/nanoCEM/cem_utils.py
--rwxrwxr-x   0 zhguo     (1000) zhguo     (1000)    10801 2024-04-13 03:51:24.000000 nanoCEM-0.0.5.6/nanoCEM/current_events_magnifier
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5903 2024-03-27 13:32:46.000000 nanoCEM-0.0.5.6/nanoCEM/de_novo.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3137 2023-12-15 14:01:45.000000 nanoCEM-0.0.5.6/nanoCEM/density_2d.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4083 2024-02-22 02:44:17.000000 nanoCEM-0.0.5.6/nanoCEM/extract_sub_fast5_from_bam
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1868 2023-07-24 04:48:56.000000 nanoCEM-0.0.5.6/nanoCEM/extract_sub_fastq_from_bam
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2160 2024-03-27 13:32:46.000000 nanoCEM-0.0.5.6/nanoCEM/kmer_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1988 2024-02-23 07:56:30.000000 nanoCEM-0.0.5.6/nanoCEM/kmer_test_pr.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3600 2024-03-27 13:32:45.000000 nanoCEM-0.0.5.6/nanoCEM/machine_learning_trainer.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4427 2024-03-27 13:32:45.000000 nanoCEM-0.0.5.6/nanoCEM/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11200 2024-02-23 10:21:22.000000 nanoCEM-0.0.5.6/nanoCEM/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10253 2024-04-16 02:28:14.000000 nanoCEM-0.0.5.6/nanoCEM/read_f5c_eventalign.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6807 2024-04-16 07:47:03.000000 nanoCEM-0.0.5.6/nanoCEM/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6866 2024-04-16 02:51:06.000000 nanoCEM-0.0.5.6/nanoCEM/read_move_table.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13342 2024-02-26 08:39:30.000000 nanoCEM-0.0.5.6/nanoCEM/read_tombo_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8548 2024-04-09 09:41:06.000000 nanoCEM-0.0.5.6/nanoCEM/squigualiser_utils.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-04-16 08:18:55.164478 nanoCEM-0.0.5.6/nanoCEM.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2730 2024-04-16 08:18:55.000000 nanoCEM-0.0.5.6/nanoCEM.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      755 2024-04-16 08:18:55.000000 nanoCEM-0.0.5.6/nanoCEM.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2024-04-16 08:18:55.000000 nanoCEM-0.0.5.6/nanoCEM.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      178 2024-04-16 08:18:55.000000 nanoCEM-0.0.5.6/nanoCEM.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2024-04-16 08:18:55.000000 nanoCEM-0.0.5.6/nanoCEM.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2024-04-16 08:18:55.164478 nanoCEM-0.0.5.6/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1295 2024-04-16 08:18:54.000000 nanoCEM-0.0.5.6/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-04-16 08:40:58.660325 nanoCEM-0.0.5.7/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.5.7/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2730 2024-04-16 08:40:58.660325 nanoCEM-0.0.5.7/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2100 2024-03-07 07:08:59.000000 nanoCEM-0.0.5.7/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-04-16 08:40:58.660325 nanoCEM-0.0.5.7/nanoCEM/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    15641 2024-04-16 08:04:15.000000 nanoCEM-0.0.5.7/nanoCEM/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5416 2023-12-21 04:37:40.000000 nanoCEM-0.0.5.7/nanoCEM/NEW_TRAINER.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.5.7/nanoCEM/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4547 2023-12-10 10:36:58.000000 nanoCEM-0.0.5.7/nanoCEM/alignment_feature_camera.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10849 2024-04-16 04:27:47.000000 nanoCEM-0.0.5.7/nanoCEM/alignment_magnifier
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    14691 2024-04-16 08:18:09.000000 nanoCEM-0.0.5.7/nanoCEM/cem_utils.py
+-rwxrwxr-x   0 zhguo     (1000) zhguo     (1000)    10833 2024-04-16 08:40:57.000000 nanoCEM-0.0.5.7/nanoCEM/current_events_magnifier
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5903 2024-03-27 13:32:46.000000 nanoCEM-0.0.5.7/nanoCEM/de_novo.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3137 2023-12-15 14:01:45.000000 nanoCEM-0.0.5.7/nanoCEM/density_2d.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4083 2024-02-22 02:44:17.000000 nanoCEM-0.0.5.7/nanoCEM/extract_sub_fast5_from_bam
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1868 2023-07-24 04:48:56.000000 nanoCEM-0.0.5.7/nanoCEM/extract_sub_fastq_from_bam
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2160 2024-03-27 13:32:46.000000 nanoCEM-0.0.5.7/nanoCEM/kmer_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1988 2024-02-23 07:56:30.000000 nanoCEM-0.0.5.7/nanoCEM/kmer_test_pr.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3600 2024-03-27 13:32:45.000000 nanoCEM-0.0.5.7/nanoCEM/machine_learning_trainer.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4427 2024-03-27 13:32:45.000000 nanoCEM-0.0.5.7/nanoCEM/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11200 2024-02-23 10:21:22.000000 nanoCEM-0.0.5.7/nanoCEM/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10253 2024-04-16 02:28:14.000000 nanoCEM-0.0.5.7/nanoCEM/read_f5c_eventalign.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6807 2024-04-16 07:47:03.000000 nanoCEM-0.0.5.7/nanoCEM/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6866 2024-04-16 02:51:06.000000 nanoCEM-0.0.5.7/nanoCEM/read_move_table.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13342 2024-02-26 08:39:30.000000 nanoCEM-0.0.5.7/nanoCEM/read_tombo_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8548 2024-04-09 09:41:06.000000 nanoCEM-0.0.5.7/nanoCEM/squigualiser_utils.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-04-16 08:40:58.660325 nanoCEM-0.0.5.7/nanoCEM.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2730 2024-04-16 08:40:58.000000 nanoCEM-0.0.5.7/nanoCEM.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      755 2024-04-16 08:40:58.000000 nanoCEM-0.0.5.7/nanoCEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2024-04-16 08:40:58.000000 nanoCEM-0.0.5.7/nanoCEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      178 2024-04-16 08:40:58.000000 nanoCEM-0.0.5.7/nanoCEM.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2024-04-16 08:40:58.000000 nanoCEM-0.0.5.7/nanoCEM.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2024-04-16 08:40:58.660325 nanoCEM-0.0.5.7/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1295 2024-04-16 08:40:57.000000 nanoCEM-0.0.5.7/setup.py
```

### Comparing `nanoCEM-0.0.5.6/LICENSE` & `nanoCEM-0.0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.6/PKG-INFO` & `nanoCEM-0.0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.5.6
+Version: 0.0.5.7
 Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports 4 re-squiggle program(tombo resquiggle/f5c resquiggle/f5c eventalign/move_table).
 Home-page: https://github.com/lrslab/nanoCEM
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nanoCEM Version: 0.0.5.6 Summary: A simple tool
+Metadata-Version: 2.1 Name: nanoCEM Version: 0.0.5.7 Summary: A simple tool
 designed to visualize the features that distinguish between two groups of ONT
 data at the site level. It supports 4 re-squiggle program(tombo resquiggle/f5c
 resquiggle/f5c eventalign/move_table). Home-page: https://github.com/lrslab/
 nanoCEM Author: GUO Zhihao Author-email: qhuozhihao@icloud.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.7.0,<=3.11.7 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `nanoCEM-0.0.5.6/README.md` & `nanoCEM-0.0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.6/nanoCEM/CE_magnifier_test.py` & `nanoCEM-0.0.5.7/nanoCEM/CE_magnifier_test.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.6/nanoCEM/NEW_TRAINER.py` & `nanoCEM-0.0.5.7/nanoCEM/NEW_TRAINER.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.6/nanoCEM/alignment_feature_camera.py` & `nanoCEM-0.0.5.7/nanoCEM/alignment_feature_camera.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.6/nanoCEM/alignment_magnifier` & `nanoCEM-0.0.5.7/nanoCEM/alignment_magnifier`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.6/nanoCEM/cem_utils.py` & `nanoCEM-0.0.5.7/nanoCEM/cem_utils.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.6/nanoCEM/current_events_magnifier` & `nanoCEM-0.0.5.7/nanoCEM/current_events_magnifier`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     # f5c subparser
     parser_f5c = subparsers.add_parser('f5c_ev', help='tackle f5c eventalign')
     parser_f5c.add_argument("-i", "--input", required=True,
                             help="blow5_path")
     parser_f5c.add_argument('-c', "--control",
                             help="control_blow5_path")
-    parser_f5c.add_argument('--base_shift', action='store_true', help='Turn on the base shift')
+    parser_f5c.add_argument('--base_shift',choices=['auto',0,-1,-2,-3,-4,-5,-6,-7,-8],default='auto', help='base shift option')
     parser_f5c.add_argument('--pore', choices=['r9', 'r10','rna004'], help='Select pore type', default='r9')
     add_public_argument(parser_f5c)
 
     parser_f5c = subparsers.add_parser('f5c_re', help='tackle f5c re-squiggle')
     parser_f5c.add_argument("-i", "--input", required=True,
                             help="blow5_path")
     parser_f5c.add_argument('-c', "--control",
```

### Comparing `nanoCEM-0.0.5.6/nanoCEM/de_novo.py` & `nanoCEM-0.0.5.7/nanoCEM/de_novo.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.6/nanoCEM/density_2d.py` & `nanoCEM-0.0.5.7/nanoCEM/density_2d.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.6/nanoCEM/extract_sub_fast5_from_bam` & `nanoCEM-0.0.5.7/nanoCEM/extract_sub_fast5_from_bam`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.6/nanoCEM/extract_sub_fastq_from_bam` & `nanoCEM-0.0.5.7/nanoCEM/extract_sub_fastq_from_bam`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.6/nanoCEM/kmer_test.py` & `nanoCEM-0.0.5.7/nanoCEM/kmer_test.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.6/nanoCEM/kmer_test_pr.py` & `nanoCEM-0.0.5.7/nanoCEM/kmer_test_pr.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.6/nanoCEM/machine_learning_trainer.py` & `nanoCEM-0.0.5.7/nanoCEM/machine_learning_trainer.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.6/nanoCEM/normalization.py` & `nanoCEM-0.0.5.7/nanoCEM/normalization.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.6/nanoCEM/plot.py` & `nanoCEM-0.0.5.7/nanoCEM/plot.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.6/nanoCEM/read_f5c_eventalign.py` & `nanoCEM-0.0.5.7/nanoCEM/read_f5c_eventalign.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.6/nanoCEM/read_f5c_resquiggle.py` & `nanoCEM-0.0.5.7/nanoCEM/read_f5c_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.6/nanoCEM/read_move_table.py` & `nanoCEM-0.0.5.7/nanoCEM/read_move_table.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.6/nanoCEM/read_tombo_resquiggle.py` & `nanoCEM-0.0.5.7/nanoCEM/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.6/nanoCEM/squigualiser_utils.py` & `nanoCEM-0.0.5.7/nanoCEM/squigualiser_utils.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.6/nanoCEM.egg-info/PKG-INFO` & `nanoCEM-0.0.5.7/nanoCEM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.5.6
+Version: 0.0.5.7
 Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports 4 re-squiggle program(tombo resquiggle/f5c resquiggle/f5c eventalign/move_table).
 Home-page: https://github.com/lrslab/nanoCEM
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nanoCEM Version: 0.0.5.6 Summary: A simple tool
+Metadata-Version: 2.1 Name: nanoCEM Version: 0.0.5.7 Summary: A simple tool
 designed to visualize the features that distinguish between two groups of ONT
 data at the site level. It supports 4 re-squiggle program(tombo resquiggle/f5c
 resquiggle/f5c eventalign/move_table). Home-page: https://github.com/lrslab/
 nanoCEM Author: GUO Zhihao Author-email: qhuozhihao@icloud.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.7.0,<=3.11.7 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `nanoCEM-0.0.5.6/nanoCEM.egg-info/SOURCES.txt` & `nanoCEM-0.0.5.7/nanoCEM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.6/setup.py` & `nanoCEM-0.0.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nanoCEM",
-    version="0.0.5.6",
+    version="0.0.5.7",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports 4 re-squiggle program(tombo resquiggle/f5c resquiggle/f5c eventalign/move_table).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/nanoCEM",
```

