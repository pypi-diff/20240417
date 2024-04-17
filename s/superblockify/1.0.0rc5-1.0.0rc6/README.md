# Comparing `tmp/superblockify-1.0.0rc5.tar.gz` & `tmp/superblockify-1.0.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superblockify-1.0.0rc5.tar", last modified: Tue Apr 16 10:15:03 2024, max compression
+gzip compressed data, was "superblockify-1.0.0rc6.tar", last modified: Wed Apr 17 08:12:19 2024, max compression
```

## Comparing `superblockify-1.0.0rc5.tar` & `superblockify-1.0.0rc6.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-16 10:15:03.441954 superblockify-1.0.0rc5/
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    34523 2024-03-25 08:40:49.000000 superblockify-1.0.0rc5/LICENSE
--rw-r--r--   0 carlsonb  (1000) carlsonb  (1000)     5984 2024-04-16 10:15:03.441954 superblockify-1.0.0rc5/PKG-INFO
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     3551 2024-04-16 10:06:49.000000 superblockify-1.0.0rc5/README.md
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     4733 2024-04-16 10:14:04.000000 superblockify-1.0.0rc5/pyproject.toml
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)       38 2024-04-16 10:15:03.441954 superblockify-1.0.0rc5/setup.cfg
-drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-16 10:15:03.197953 superblockify-1.0.0rc5/superblockify/
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      443 2024-04-08 20:10:55.000000 superblockify-1.0.0rc5/superblockify/__init__.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1153 2023-06-27 21:08:28.000000 superblockify-1.0.0rc5/superblockify/_api.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)       63 2024-04-16 10:10:49.000000 superblockify-1.0.0rc5/superblockify/_version.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     9072 2023-06-23 06:47:12.000000 superblockify-1.0.0rc5/superblockify/attribute.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     6240 2024-04-16 10:11:16.000000 superblockify-1.0.0rc5/superblockify/config.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     4592 2024-04-08 20:10:55.000000 superblockify-1.0.0rc5/superblockify/graph_stats.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      782 2024-04-16 09:34:18.000000 superblockify-1.0.0rc5/superblockify/logging.cfg
-drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-16 10:15:03.265953 superblockify-1.0.0rc5/superblockify/metrics/
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      272 2023-04-21 06:51:36.000000 superblockify-1.0.0rc5/superblockify/metrics/__init__.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    27220 2024-04-08 21:02:38.000000 superblockify-1.0.0rc5/superblockify/metrics/distances.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    29000 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/superblockify/metrics/measures.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    21147 2024-04-08 20:10:55.000000 superblockify-1.0.0rc5/superblockify/metrics/metric.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    16173 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/superblockify/metrics/plot.py
-drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-16 10:15:03.333953 superblockify-1.0.0rc5/superblockify/partitioning/
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      893 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/superblockify/partitioning/__init__.py
-drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-16 10:15:03.333953 superblockify-1.0.0rc5/superblockify/partitioning/approaches/
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      279 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/superblockify/partitioning/approaches/__init__.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     2672 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/superblockify/partitioning/approaches/attribute.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    30020 2024-04-08 20:10:55.000000 superblockify-1.0.0rc5/superblockify/partitioning/approaches/bearing.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     3988 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/superblockify/partitioning/approaches/betweenness.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1826 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/superblockify/partitioning/approaches/dummy.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     8957 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/superblockify/partitioning/approaches/steiner_tree.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1445 2023-05-22 07:49:38.000000 superblockify-1.0.0rc5/superblockify/partitioning/approaches/streettype.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    40014 2024-04-16 09:32:16.000000 superblockify-1.0.0rc5/superblockify/partitioning/base.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    10319 2024-04-08 20:10:55.000000 superblockify-1.0.0rc5/superblockify/partitioning/checks.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    11867 2024-04-08 20:10:55.000000 superblockify-1.0.0rc5/superblockify/partitioning/plot.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     2502 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/superblockify/partitioning/representative.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1914 2024-04-08 20:10:55.000000 superblockify-1.0.0rc5/superblockify/partitioning/speed.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    25005 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/superblockify/partitioning/utils.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    21795 2024-04-08 13:58:15.000000 superblockify-1.0.0rc5/superblockify/plot.py
-drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-16 10:15:03.389954 superblockify-1.0.0rc5/superblockify/population/
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      276 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/superblockify/population/__init__.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    12827 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/superblockify/population/approximation.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    10670 2024-04-08 20:10:55.000000 superblockify-1.0.0rc5/superblockify/population/ghsl.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    10445 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/superblockify/population/tessellation.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    14351 2024-04-08 20:10:55.000000 superblockify-1.0.0rc5/superblockify/utils.py
-drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-16 10:15:03.441954 superblockify-1.0.0rc5/superblockify.egg-info/
--rw-r--r--   0 carlsonb  (1000) carlsonb  (1000)     5984 2024-04-16 10:15:03.000000 superblockify-1.0.0rc5/superblockify.egg-info/PKG-INFO
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1467 2024-04-16 10:15:03.000000 superblockify-1.0.0rc5/superblockify.egg-info/SOURCES.txt
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)        1 2024-04-16 10:15:03.000000 superblockify-1.0.0rc5/superblockify.egg-info/dependency_links.txt
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      282 2024-04-16 10:15:03.000000 superblockify-1.0.0rc5/superblockify.egg-info/requires.txt
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)       14 2024-04-16 10:15:03.000000 superblockify-1.0.0rc5/superblockify.egg-info/top_level.txt
-drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-16 10:15:03.429954 superblockify-1.0.0rc5/tests/
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     7641 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/tests/test_attribute.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     3345 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/tests/test_graph_stats.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     6980 2024-04-08 20:10:55.000000 superblockify-1.0.0rc5/tests/test_plot.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    11491 2024-04-08 20:10:55.000000 superblockify-1.0.0rc5/tests/test_utils.py
+drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-17 08:12:19.542927 superblockify-1.0.0rc6/
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    34523 2024-04-16 14:27:06.000000 superblockify-1.0.0rc6/LICENSE
+-rw-r--r--   0 carlsonb  (1000) carlsonb  (1000)     6094 2024-04-17 08:12:19.542927 superblockify-1.0.0rc6/PKG-INFO
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     3683 2024-04-17 08:02:53.000000 superblockify-1.0.0rc6/README.md
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     4728 2024-04-16 16:11:38.000000 superblockify-1.0.0rc6/pyproject.toml
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)       38 2024-04-17 08:12:19.542927 superblockify-1.0.0rc6/setup.cfg
+drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-17 08:12:19.446926 superblockify-1.0.0rc6/superblockify/
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      443 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/superblockify/__init__.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1153 2023-06-27 21:08:28.000000 superblockify-1.0.0rc6/superblockify/_api.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)       63 2024-04-17 08:12:00.000000 superblockify-1.0.0rc6/superblockify/_version.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     9072 2023-06-23 06:47:12.000000 superblockify-1.0.0rc6/superblockify/attribute.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)   107000 2024-04-17 08:10:30.000000 superblockify-1.0.0rc6/superblockify/cities.yml
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     6722 2024-04-17 08:10:39.000000 superblockify-1.0.0rc6/superblockify/config.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     4592 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/superblockify/graph_stats.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      589 2024-04-16 16:07:46.000000 superblockify-1.0.0rc6/superblockify/logging.cfg
+drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-17 08:12:19.510927 superblockify-1.0.0rc6/superblockify/metrics/
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      272 2023-04-21 06:51:36.000000 superblockify-1.0.0rc6/superblockify/metrics/__init__.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    27220 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/superblockify/metrics/distances.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    28989 2024-04-16 14:28:20.000000 superblockify-1.0.0rc6/superblockify/metrics/measures.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    21147 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/superblockify/metrics/metric.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    16173 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/superblockify/metrics/plot.py
+drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-17 08:12:19.510927 superblockify-1.0.0rc6/superblockify/partitioning/
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      893 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/superblockify/partitioning/__init__.py
+drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-17 08:12:19.514927 superblockify-1.0.0rc6/superblockify/partitioning/approaches/
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      279 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/superblockify/partitioning/approaches/__init__.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     2672 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/superblockify/partitioning/approaches/attribute.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    30020 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/superblockify/partitioning/approaches/bearing.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     3988 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/superblockify/partitioning/approaches/betweenness.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1826 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/superblockify/partitioning/approaches/dummy.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     8957 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/superblockify/partitioning/approaches/steiner_tree.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1445 2023-05-22 07:49:38.000000 superblockify-1.0.0rc6/superblockify/partitioning/approaches/streettype.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    40014 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/superblockify/partitioning/base.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    10319 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/superblockify/partitioning/checks.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    11867 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/superblockify/partitioning/plot.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     2502 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/superblockify/partitioning/representative.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1914 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/superblockify/partitioning/speed.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    25028 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/superblockify/partitioning/utils.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    21795 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/superblockify/plot.py
+drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-17 08:12:19.530927 superblockify-1.0.0rc6/superblockify/population/
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      276 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/superblockify/population/__init__.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    12827 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/superblockify/population/approximation.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    10670 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/superblockify/population/ghsl.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    10445 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/superblockify/population/tessellation.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    14351 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/superblockify/utils.py
+drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-17 08:12:19.538927 superblockify-1.0.0rc6/superblockify.egg-info/
+-rw-r--r--   0 carlsonb  (1000) carlsonb  (1000)     6094 2024-04-17 08:12:19.000000 superblockify-1.0.0rc6/superblockify.egg-info/PKG-INFO
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1492 2024-04-17 08:12:19.000000 superblockify-1.0.0rc6/superblockify.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)        1 2024-04-17 08:12:19.000000 superblockify-1.0.0rc6/superblockify.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      275 2024-04-17 08:12:19.000000 superblockify-1.0.0rc6/superblockify.egg-info/requires.txt
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)       14 2024-04-17 08:12:19.000000 superblockify-1.0.0rc6/superblockify.egg-info/top_level.txt
+drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-17 08:12:19.530927 superblockify-1.0.0rc6/tests/
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     7641 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/tests/test_attribute.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     3345 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/tests/test_graph_stats.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     6980 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/tests/test_plot.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    12188 2024-04-16 14:27:07.000000 superblockify-1.0.0rc6/tests/test_utils.py
```

### Comparing `superblockify-1.0.0rc5/LICENSE` & `superblockify-1.0.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/PKG-INFO` & `superblockify-1.0.0rc6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superblockify
-Version: 1.0.0rc5
+Version: 1.0.0rc6
 Summary: Automated Generation, Visualization, and Analysis of potential Superblocks in Cities
 Author-email: Carlson Büth <carlson@cbueth.de>
 Maintainer: superblockify contributors
 License: APGL-3.0-or-later
 Project-URL: Documentation, https://NERDSITU.github.io/superblockify
 Project-URL: Repository, https://github.com/NERDSITU/superblockify
 Project-URL: Changelog, https://NERDSITU.github.io/superblockify/changelog/
@@ -27,15 +27,14 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: osmnx
 Requires-Dist: geopandas
 Requires-Dist: rasterio
 Requires-Dist: shapely
-Requires-Dist: pyrosm
 Requires-Dist: numba
 Requires-Dist: tqdm
 Requires-Dist: contextily
 Requires-Dist: ruamel.yaml
 Requires-Dist: pyarrow
 Requires-Dist: seaborn
 Requires-Dist: psutil
@@ -54,51 +53,56 @@
 Requires-Dist: myst-nb; extra == "doc"
 Requires-Dist: sphinx-book-theme; extra == "doc"
 Requires-Dist: rasterstats; extra == "doc"
 Requires-Dist: momepy; extra == "doc"
 Provides-Extra: all
 Requires-Dist: superblockify[doc,lint,test]; extra == "all"
 
-# superblockify
+![superblockify](superblockify_logo.png "superblockify")
 
 [![Dev](https://img.shields.io/badge/docs-dev-blue.svg)](https://NERDSITU.github.io/superblockify/)
 [![PyPI Version](https://badge.fury.io/py/superblockify.svg)](https://pypi.org/project/superblockify/)
 [![Python Version](https://img.shields.io/pypi/pyversions/superblockify)](https://pypi.org/project/superblockify/)
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI License](https://img.shields.io/pypi/l/superblockify)](https://pypi.org/project/superblockify/)
 
 [![Docs](https://github.com/NERDSITU/superblockify/actions/workflows/docs.yml/badge.svg)](https://github.com/NERDSITU/superblockify/actions/workflows/docs.yml)
 [![Lint](https://github.com/NERDSITU/superblockify/actions/workflows/lint.yml/badge.svg)](https://github.com/NERDSITU/superblockify/actions/workflows/lint.yml)
 [![Test](https://github.com/NERDSITU/superblockify/actions/workflows/test.yml/badge.svg)](https://github.com/NERDSITU/superblockify/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/NERDSITU/superblockify/branch/main/graph/badge.svg?token=AS72IFT2Q4)](https://codecov.io/gh/NERDSITU/superblockify)
 
-Source code for blockifying existing street networks.
+Source code to `superblockify` an urban street network
 
 ---
 
+`superblockify` is a Python package for partitioning an urban street network into
+Superblock-like neighborhoods and for visualizing and analyzing the partition results. A Superblock is a set of adjacent urban blocks where vehicular through traffic is prevented or pacified, giving priority to people walking and cycling. 
+
 ## Installation
 
-We recommend using `micromamba` to create a virtual
-environment and installing the package in editable mode.
-Alternatively, one can use `conda` or `mamba` to create the environment
-(they can be used interchangeably).
-After cloning the repository, navigate to the root folder and
-create the environment with the wished python version and the development dependencies.
+We recommend
+using [`micromamba`](https://mamba.readthedocs.io/en/latest/installation/micromamba-installation.html)
+to create a virtual environment and installing the package in editable mode.
+Alternatively, one can
+use [`conda`](https://docs.conda.io/projects/conda/en/latest/index.html)
+or [`mamba`](https://mamba.readthedocs.io/en/latest/installation/mamba-installation.html)
+to create the environment (they can be used interchangeably).
 
 ```bash
 micromamba create -n sb_env -c conda-forge python=3.12 osmnx
 micromamba activate sb_env
 pip install superblockify
 ```
 
 This installs the package and its dependencies,
 ready for use when activating the environment.
 Learn more about `superblockify` by reading
 the [documentation](https://NERDSITU.github.io/superblockify/)
+with the [usage section](https://nerdsitu.github.io/superblockify/usage/)
 or
 the [minimal working example](https://github.com/NERDSITU/superblockify/blob/main/scripts/examples/mwe.py).
 
 ## Development Setup
 
 For development, clone the repository, navigate to the root folder and
 create the environment with the wished python version and the development dependencies.
@@ -118,20 +122,12 @@
 ## Usage
 
 For a quick start there are example scripts in
 the [`examples/`](https://github.com/NERDSITU/superblockify/blob/main/scripts/examples/)
 folder and
 a [minimal working example](https://github.com/NERDSITU/superblockify/blob/main/scripts/examples/mwe.py).
 
-## Logging
-
-The logging is done using the `logging` module. The logging level can be set in the
-`setup.cfg` file. The logging level can be set to `DEBUG`, `INFO`, `WARNING`, `ERROR`
-or `CRITICAL`. It defaults to `INFO` and a rotating file handler is set up to log
-to `results/logs/superblockify.log`. The log file is rotated every megabyte, and the
-last three log files are kept.
-
 ## Testing
 
 The tests are specified using the `pytest` signature, see [`tests/`](tests/) folder, and
 can be run using a test runner of choice.
 A pipeline is set up, see [`.github/workflows/test.yml`](.github/workflows/test.yml).
```

### Comparing `superblockify-1.0.0rc5/README.md` & `superblockify-1.0.0rc6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,49 @@
-# superblockify
+![superblockify](superblockify_logo.png "superblockify")
 
 [![Dev](https://img.shields.io/badge/docs-dev-blue.svg)](https://NERDSITU.github.io/superblockify/)
 [![PyPI Version](https://badge.fury.io/py/superblockify.svg)](https://pypi.org/project/superblockify/)
 [![Python Version](https://img.shields.io/pypi/pyversions/superblockify)](https://pypi.org/project/superblockify/)
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI License](https://img.shields.io/pypi/l/superblockify)](https://pypi.org/project/superblockify/)
 
 [![Docs](https://github.com/NERDSITU/superblockify/actions/workflows/docs.yml/badge.svg)](https://github.com/NERDSITU/superblockify/actions/workflows/docs.yml)
 [![Lint](https://github.com/NERDSITU/superblockify/actions/workflows/lint.yml/badge.svg)](https://github.com/NERDSITU/superblockify/actions/workflows/lint.yml)
 [![Test](https://github.com/NERDSITU/superblockify/actions/workflows/test.yml/badge.svg)](https://github.com/NERDSITU/superblockify/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/NERDSITU/superblockify/branch/main/graph/badge.svg?token=AS72IFT2Q4)](https://codecov.io/gh/NERDSITU/superblockify)
 
-Source code for blockifying existing street networks.
+Source code to `superblockify` an urban street network
 
 ---
 
+`superblockify` is a Python package for partitioning an urban street network into
+Superblock-like neighborhoods and for visualizing and analyzing the partition results. A Superblock is a set of adjacent urban blocks where vehicular through traffic is prevented or pacified, giving priority to people walking and cycling. 
+
 ## Installation
 
-We recommend using `micromamba` to create a virtual
-environment and installing the package in editable mode.
-Alternatively, one can use `conda` or `mamba` to create the environment
-(they can be used interchangeably).
-After cloning the repository, navigate to the root folder and
-create the environment with the wished python version and the development dependencies.
+We recommend
+using [`micromamba`](https://mamba.readthedocs.io/en/latest/installation/micromamba-installation.html)
+to create a virtual environment and installing the package in editable mode.
+Alternatively, one can
+use [`conda`](https://docs.conda.io/projects/conda/en/latest/index.html)
+or [`mamba`](https://mamba.readthedocs.io/en/latest/installation/mamba-installation.html)
+to create the environment (they can be used interchangeably).
 
 ```bash
 micromamba create -n sb_env -c conda-forge python=3.12 osmnx
 micromamba activate sb_env
 pip install superblockify
 ```
 
 This installs the package and its dependencies,
 ready for use when activating the environment.
 Learn more about `superblockify` by reading
 the [documentation](https://NERDSITU.github.io/superblockify/)
+with the [usage section](https://nerdsitu.github.io/superblockify/usage/)
 or
 the [minimal working example](https://github.com/NERDSITU/superblockify/blob/main/scripts/examples/mwe.py).
 
 ## Development Setup
 
 For development, clone the repository, navigate to the root folder and
 create the environment with the wished python version and the development dependencies.
@@ -58,20 +63,12 @@
 ## Usage
 
 For a quick start there are example scripts in
 the [`examples/`](https://github.com/NERDSITU/superblockify/blob/main/scripts/examples/)
 folder and
 a [minimal working example](https://github.com/NERDSITU/superblockify/blob/main/scripts/examples/mwe.py).
 
-## Logging
-
-The logging is done using the `logging` module. The logging level can be set in the
-`setup.cfg` file. The logging level can be set to `DEBUG`, `INFO`, `WARNING`, `ERROR`
-or `CRITICAL`. It defaults to `INFO` and a rotating file handler is set up to log
-to `results/logs/superblockify.log`. The log file is rotated every megabyte, and the
-last three log files are kept.
-
 ## Testing
 
 The tests are specified using the `pytest` signature, see [`tests/`](tests/) folder, and
 can be run using a test runner of choice.
 A pipeline is set up, see [`.github/workflows/test.yml`](.github/workflows/test.yml).
```

### Comparing `superblockify-1.0.0rc5/pyproject.toml` & `superblockify-1.0.0rc6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 dynamic = ["version"]
 requires-python = ">=3.10"
 dependencies = [
     "osmnx",
     "geopandas",
     "rasterio",
     "shapely",
-    "pyrosm",
     "numba",
     "tqdm",
     "contextily",
     "ruamel.yaml",
     "pyarrow",
     "seaborn",
     "psutil",
@@ -67,15 +66,15 @@
 namespaces = false
 
 [tool.setuptools.dynamic]
 readme = { file = ["README.md", "LICENSE"] }
 version = { attr = "superblockify._version.__version__" }
 
 [tool.setuptools.package-data]
-superblockify = ["*.cfg"]
+superblockify = ["*.cfg", "*.yml"]
 
 # --------------------------------------------------------------------------------------
 # Linting
 # --------------------------------------------------------------------------------------
 [tool.pylint.main]
 # Number of processes to use to do the linting.
 jobs = 5
```

### Comparing `superblockify-1.0.0rc5/superblockify/_api.py` & `superblockify-1.0.0rc6/superblockify/_api.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/superblockify/attribute.py` & `superblockify-1.0.0rc6/superblockify/attribute.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/superblockify/config.py` & `superblockify-1.0.0rc6/superblockify/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,33 @@
 logging.config.fileConfig(join(dirname(__file__), "logging.cfg"))
 # Get the logger for this module
 numba_logger = logging.getLogger("numba")
 numba_logger.setLevel(logging.WARNING)
 logger = logging.getLogger("superblockify")
 
 
+def set_log_level(level: int | str) -> None:
+    """Set the logging level for the superblockify logger.
+
+    Also sets the logging level for the first handler of the root logger.
+
+    Parameters
+    ----------
+    level : int | str
+        The logging level. See the :mod:`logging` module for more information.
+
+    Raises
+    ------
+    ValueError
+        If the level is not a valid logging level.
+    """
+    logger.setLevel(level)
+    logging.getLogger().handlers[0].setLevel(level)
+
+
 class Config:  # pylint: disable=too-few-public-methods
     """Configuration class for superblockify.
 
     Attributes
     ----------
 
     WORK_DIR
@@ -81,15 +100,15 @@
         Same as ``PLACES_GENERAL`` but for places of which the graph is small enough to
         be used in the tests.
     PLACES_100_CITIES
         100 cities from Boeing et al. (2019) <https://doi.org/10.1007/s41109-019-0189-1>
         A dictionary of the form ``{name: place}`` where ``name`` is the name of the
         place, and ``place`` is a dictionary of various attributes. One of them is the
         ``query`` attribute which is the place string or a list of place strings.
-        Find the extensive list in the ``../cities.yml`` file.
+        Find the extensive list in the ``./cities.yml`` file.
     PLACES_GERMANY
         List of cities in Germany by population. All cities with more than 100,000
         inhabitants are included. Data from the German Federal Statistical Office.
 
     PLOT_SUFFIX
         The format of the plots. Can be ``"png"``, ``"jpg"``, ``"pdf"``, ``"svg"``, etc.
         Matplotlib uses the Pillow library to save the plots,
@@ -133,15 +152,15 @@
     DOWNLOAD_TIMEOUT = 60
 
     # Tests
     TEST_DATA_PATH = join(dirname(__file__), "..", "tests", "test_data")
     HIDE_PLOTS = True
 
     # Places
-    PLACES_FILE = join(dirname(__file__), "..", "cities.yml")
+    PLACES_FILE = join(dirname(__file__), "cities.yml")
     # see if the file is available
     if exists(PLACES_FILE):
         with open(PLACES_FILE, "r", encoding="utf-8") as file:
             yaml = YAML(typ="safe")
             places = yaml.load(file)
             PLACES_GENERAL = [
                 (name, data["query"])
```

### Comparing `superblockify-1.0.0rc5/superblockify/graph_stats.py` & `superblockify-1.0.0rc6/superblockify/graph_stats.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/superblockify/logging.cfg` & `superblockify-1.0.0rc6/superblockify/logging.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [loggers]
 keys = root
 
 [handlers]
-keys = consoleHandler,RotatingFileHandler
+keys = consoleHandler
 
 [formatters]
 keys = simpleFormatter
 
 [logger_root]
 level = INFO
 handlers = consoleHandler
 
 [logger_superblockify]
 level = INFO
-handlers = consoleHandler,RotatingFileHandler
+handlers = consoleHandler
 qualname = superblockify
 propagate = 1
 
 [handler_consoleHandler]
 class = StreamHandler
 level = INFO
 formatter = simpleFormatter
@@ -26,15 +26,9 @@
 [handler_tqdmHandler]
 class = StreamHandler
 level = INFO
 formatter = simpleFormatter
 args = (sys.stdout,)
 qualname = tqdm
 
-[handler_RotatingFileHandler]
-class = handlers.RotatingFileHandler
-level = DEBUG
-formatter = simpleFormatter
-args = ('superblockify.log', 'w+', 1e6, 3)
-
 [formatter_simpleFormatter]
 format = %(asctime)s | %(levelname)8s | %(filename)s:%(lineno)d | %(message)s
```

### Comparing `superblockify-1.0.0rc5/superblockify/metrics/distances.py` & `superblockify-1.0.0rc6/superblockify/metrics/distances.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/superblockify/metrics/measures.py` & `superblockify-1.0.0rc6/superblockify/metrics/measures.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from ..config import logger
 from ..utils import __edges_to_1d, __edge_to_1d, percentual_increase
 
 
 def calculate_directness(distance_matrix, measure1, measure2):
     r"""Calculate the directness for the given network measures.
 
-    The directness in the mean of the ratios between the distances of the two
+    The directness is the mean of the ratios between the distances of the two
     network measures.
 
     If any of the distances is 0 or infinite, it is ignored in the calculation.
 
     Parameters
     ----------
     distance_matrix : dict
@@ -189,15 +189,15 @@
 
 
 def write_relative_increase_to_edges(
     graph, distance_matrix, node_list, measure1, measure2
 ):
     """Write the relative increase of the distance matrix to the edges of the graph.
 
-    For each edge the relative increases to and from every node to the two nodes
+    For each edge, the relative increases to and from every node to the two nodes
     of the edge are averaged and written to the edge attribute "rel_increase".
 
     Parameters
     ----------
     graph : nx.Graph
         The graph to write the relative increase to
     distance_matrix : dict
@@ -241,15 +241,15 @@
     seed=None,
     max_range=None,
 ):
     """Calculate several types of betweenness centrality for the nodes and edges.
 
     Uses the predecessors to calculate the betweenness centrality of the nodes and
     edges. The normalized betweenness centrality is calculated, length-scaled, and
-    linearly scaled betweenness centrality are calculated for the nodes and edges. When
+    linearly scaled betweenness centrality is calculated for the nodes and edges. When
     passing a k, the summation is only done over k random nodes. [1]_ [2]_ [3]_
 
     Parameters
     ----------
     graph : nx.MultiDiGraph
         The graph to calculate the betweenness centrality for, distances and
         predecessors must be calculated for this graph
@@ -276,27 +276,27 @@
     max_range : float, optional
         The maximum path length to consider, by default None, which means no maximum
         path length. It is measured in unit of the weight attribute.
 
     Raises
     ------
     ValueError
-        If weight is not None and the graph does not have the weight attribute on all
+        If weight is not None, and the graph does not have the weight attribute on all
         edges.
 
     Notes
     -----
     Works in-place on the graph.
 
-    Does not include endpoints.
+    It Does not include endpoints.
 
     Modified from :mod:`networkx.algorithms.centrality.betweenness`.
 
     The :attr:`weight` attribute is not used to determine the shortest paths, these are
-    taken from the predecessors matrix. It is only used for parallel edges, to decide
+    taken from the predecessor matrix. It is only used for parallel edges to decide
     which edge to attribute the betweenness centrality to.
 
     If there are :math:`<=` 2 nodes, node betweenness is 0 for all nodes. If there are
     :math:`<=` 1 edges, edge betweenness is 0 for all edges.
 
     References
     ----------
@@ -596,15 +596,15 @@
     Notes
     -----
     The edges_u and edges_v arrays are sorted together, this way indices can be
     found using a binary search. This is faster than using np.where.
     """
 
     betweennesses = np.zeros((len(pred) + len(edges_uv), 3), dtype=np.float64)
-    # The first len(pred) rows correspond to node betweenness, the rest to edge
+    # The first len(pred) rows correspond to node betweenness; the rest to edge
     # The 3 layers correspond to normal, length-scaled, and linearly scaled
 
     # Loop over nodes to collect betweenness using pair-wise dependencies
     for idx in prange(loop_indices.shape[0]):  # pylint: disable=not-an-iterable
         betweennesses += __accumulate_bc(
             loop_indices[idx],
             pred[loop_indices[idx]],
@@ -677,15 +677,15 @@
         \sum_{i = 1}^{N} \| x_i - x_{\mathrm{cm}, \theta} \|
 
     .. math::
         x_{\mathrm{cm}, \theta} = \frac{1}{N_{\theta}}
         \sum_{i = 1}^{N_{\theta}} x_i
 
     The distance calculation :math:`\| x_i - x_{\mathrm{cm}, \theta} \|` includes the
-    x and y coordinates of the node, and is the Euclidean distance. In this case it
+    x and y coordinates of the node, and is the Euclidean distance. In this case, it
     is the Frobenius norm of the difference between the node coordinates and the
     center of mass of the high betweenness nodes.
 
     Parameters
     ----------
     coord_bc : np.ndarray
         Array of node coordinates and betweenness values, sorted by betweenness.
@@ -696,23 +696,23 @@
     -------
     high_bc_clustering : float
         Clustering coefficient for the nodes with the highest betweenness.
 
     Raises
     ------
     ValueError
-        If the coordinate array is has less than two nodes.
+        If the coordinate array has less than two nodes.
     ValueError
         If the threshold index is greater than the number of nodes.
     """
     if len(coord_bc) < 2:
         raise ValueError("Coordinate array must have at least two nodes.")
     if threshold_idx >= len(coord_bc):
         raise ValueError("Threshold index must be less than the number of nodes.")
-    # Center of mass of high betweenness nodes
+    # High betweenness nodes center of mass
     high_bc_cm = np.mean(coord_bc[threshold_idx:, :2], axis=0)
     # Average distance to center of mass
     avg_dist = np.mean(
         np.linalg.norm(coord_bc[threshold_idx:, :2] - high_bc_cm, axis=1)
     )
     # Norm by average distance of all nodes
     return avg_dist / np.mean(np.linalg.norm(coord_bc[:, :2] - high_bc_cm, axis=1))
@@ -725,15 +725,15 @@
     :math:`A_{\theta}=\lambda_1/\lambda_2`, where :math:`\lambda_i` are the positive
     eigenvalues of the covariance matrix of the high betweenness nodes, and
     :math:`\lambda_1 \geq \lambda_2`. [1]_
 
     Parameters
     ----------
     coord_high_bc : np.ndarray
-        Array of node coordinates of the high betweenness nodes.
+        Array of the high betweenness nodes coordinates.
 
     Returns
     -------
     high_bc_anisotropy : float
         Anisotropy for the nodes with the highest betweenness.
 
     Raises
```

### Comparing `superblockify-1.0.0rc5/superblockify/metrics/metric.py` & `superblockify-1.0.0rc6/superblockify/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/superblockify/metrics/plot.py` & `superblockify-1.0.0rc6/superblockify/metrics/plot.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/superblockify/partitioning/__init__.py` & `superblockify-1.0.0rc6/superblockify/partitioning/__init__.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/superblockify/partitioning/approaches/attribute.py` & `superblockify-1.0.0rc6/superblockify/partitioning/approaches/attribute.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/superblockify/partitioning/approaches/bearing.py` & `superblockify-1.0.0rc6/superblockify/partitioning/approaches/bearing.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/superblockify/partitioning/approaches/betweenness.py` & `superblockify-1.0.0rc6/superblockify/partitioning/approaches/betweenness.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/superblockify/partitioning/approaches/dummy.py` & `superblockify-1.0.0rc6/superblockify/partitioning/approaches/dummy.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/superblockify/partitioning/approaches/steiner_tree.py` & `superblockify-1.0.0rc6/superblockify/partitioning/approaches/steiner_tree.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/superblockify/partitioning/approaches/streettype.py` & `superblockify-1.0.0rc6/superblockify/partitioning/approaches/streettype.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/superblockify/partitioning/base.py` & `superblockify-1.0.0rc6/superblockify/partitioning/base.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/superblockify/partitioning/checks.py` & `superblockify-1.0.0rc6/superblockify/partitioning/checks.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/superblockify/partitioning/plot.py` & `superblockify-1.0.0rc6/superblockify/partitioning/plot.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/superblockify/partitioning/representative.py` & `superblockify-1.0.0rc6/superblockify/partitioning/representative.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/superblockify/partitioning/speed.py` & `superblockify-1.0.0rc6/superblockify/partitioning/speed.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/superblockify/partitioning/utils.py` & `superblockify-1.0.0rc6/superblockify/partitioning/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from os import remove
 from os.path import exists, join
 from uuid import uuid4
 
 from geopandas import GeoDataFrame
 from networkx import set_edge_attributes, strongly_connected_components
 from numpy import generic
-from osmnx import graph_to_gdfs, get_undirected
+from osmnx import graph_to_gdfs
+from osmnx.convert import to_undirected
 from pandas import DataFrame
 from shapely import Point, Geometry
 from shapely.ops import substring
 
 from .representative import find_representative_node_id
 from ..config import logger
 from ..graph_stats import get_population_area, basic_graph_stats
@@ -381,15 +382,15 @@
     rest = graph.edge_subgraph(
         [
             (u, v, k)
             for u, v, k in graph.edges(keys=True, data=False)
             if (u, v, k) not in sparsified.edges(keys=True)
         ]
     )
-    rest_un = get_undirected(rest)
+    rest_un = to_undirected(rest)
 
     # for u, v, k, d in rest.edges(keys=True, data=True):
     for u_isol, v_isol in [
         (u, v)
         for u, v in rest_un.edges()
         if rest_un.degree(u) == 1 and rest_un.degree(v) == 1
     ]:
```

### Comparing `superblockify-1.0.0rc5/superblockify/plot.py` & `superblockify-1.0.0rc6/superblockify/plot.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/superblockify/population/approximation.py` & `superblockify-1.0.0rc6/superblockify/population/approximation.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/superblockify/population/ghsl.py` & `superblockify-1.0.0rc6/superblockify/population/ghsl.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/superblockify/population/tessellation.py` & `superblockify-1.0.0rc6/superblockify/population/tessellation.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/superblockify/utils.py` & `superblockify-1.0.0rc6/superblockify/utils.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/superblockify.egg-info/PKG-INFO` & `superblockify-1.0.0rc6/superblockify.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superblockify
-Version: 1.0.0rc5
+Version: 1.0.0rc6
 Summary: Automated Generation, Visualization, and Analysis of potential Superblocks in Cities
 Author-email: Carlson Büth <carlson@cbueth.de>
 Maintainer: superblockify contributors
 License: APGL-3.0-or-later
 Project-URL: Documentation, https://NERDSITU.github.io/superblockify
 Project-URL: Repository, https://github.com/NERDSITU/superblockify
 Project-URL: Changelog, https://NERDSITU.github.io/superblockify/changelog/
@@ -27,15 +27,14 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: osmnx
 Requires-Dist: geopandas
 Requires-Dist: rasterio
 Requires-Dist: shapely
-Requires-Dist: pyrosm
 Requires-Dist: numba
 Requires-Dist: tqdm
 Requires-Dist: contextily
 Requires-Dist: ruamel.yaml
 Requires-Dist: pyarrow
 Requires-Dist: seaborn
 Requires-Dist: psutil
@@ -54,51 +53,56 @@
 Requires-Dist: myst-nb; extra == "doc"
 Requires-Dist: sphinx-book-theme; extra == "doc"
 Requires-Dist: rasterstats; extra == "doc"
 Requires-Dist: momepy; extra == "doc"
 Provides-Extra: all
 Requires-Dist: superblockify[doc,lint,test]; extra == "all"
 
-# superblockify
+![superblockify](superblockify_logo.png "superblockify")
 
 [![Dev](https://img.shields.io/badge/docs-dev-blue.svg)](https://NERDSITU.github.io/superblockify/)
 [![PyPI Version](https://badge.fury.io/py/superblockify.svg)](https://pypi.org/project/superblockify/)
 [![Python Version](https://img.shields.io/pypi/pyversions/superblockify)](https://pypi.org/project/superblockify/)
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI License](https://img.shields.io/pypi/l/superblockify)](https://pypi.org/project/superblockify/)
 
 [![Docs](https://github.com/NERDSITU/superblockify/actions/workflows/docs.yml/badge.svg)](https://github.com/NERDSITU/superblockify/actions/workflows/docs.yml)
 [![Lint](https://github.com/NERDSITU/superblockify/actions/workflows/lint.yml/badge.svg)](https://github.com/NERDSITU/superblockify/actions/workflows/lint.yml)
 [![Test](https://github.com/NERDSITU/superblockify/actions/workflows/test.yml/badge.svg)](https://github.com/NERDSITU/superblockify/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/NERDSITU/superblockify/branch/main/graph/badge.svg?token=AS72IFT2Q4)](https://codecov.io/gh/NERDSITU/superblockify)
 
-Source code for blockifying existing street networks.
+Source code to `superblockify` an urban street network
 
 ---
 
+`superblockify` is a Python package for partitioning an urban street network into
+Superblock-like neighborhoods and for visualizing and analyzing the partition results. A Superblock is a set of adjacent urban blocks where vehicular through traffic is prevented or pacified, giving priority to people walking and cycling. 
+
 ## Installation
 
-We recommend using `micromamba` to create a virtual
-environment and installing the package in editable mode.
-Alternatively, one can use `conda` or `mamba` to create the environment
-(they can be used interchangeably).
-After cloning the repository, navigate to the root folder and
-create the environment with the wished python version and the development dependencies.
+We recommend
+using [`micromamba`](https://mamba.readthedocs.io/en/latest/installation/micromamba-installation.html)
+to create a virtual environment and installing the package in editable mode.
+Alternatively, one can
+use [`conda`](https://docs.conda.io/projects/conda/en/latest/index.html)
+or [`mamba`](https://mamba.readthedocs.io/en/latest/installation/mamba-installation.html)
+to create the environment (they can be used interchangeably).
 
 ```bash
 micromamba create -n sb_env -c conda-forge python=3.12 osmnx
 micromamba activate sb_env
 pip install superblockify
 ```
 
 This installs the package and its dependencies,
 ready for use when activating the environment.
 Learn more about `superblockify` by reading
 the [documentation](https://NERDSITU.github.io/superblockify/)
+with the [usage section](https://nerdsitu.github.io/superblockify/usage/)
 or
 the [minimal working example](https://github.com/NERDSITU/superblockify/blob/main/scripts/examples/mwe.py).
 
 ## Development Setup
 
 For development, clone the repository, navigate to the root folder and
 create the environment with the wished python version and the development dependencies.
@@ -118,20 +122,12 @@
 ## Usage
 
 For a quick start there are example scripts in
 the [`examples/`](https://github.com/NERDSITU/superblockify/blob/main/scripts/examples/)
 folder and
 a [minimal working example](https://github.com/NERDSITU/superblockify/blob/main/scripts/examples/mwe.py).
 
-## Logging
-
-The logging is done using the `logging` module. The logging level can be set in the
-`setup.cfg` file. The logging level can be set to `DEBUG`, `INFO`, `WARNING`, `ERROR`
-or `CRITICAL`. It defaults to `INFO` and a rotating file handler is set up to log
-to `results/logs/superblockify.log`. The log file is rotated every megabyte, and the
-last three log files are kept.
-
 ## Testing
 
 The tests are specified using the `pytest` signature, see [`tests/`](tests/) folder, and
 can be run using a test runner of choice.
 A pipeline is set up, see [`.github/workflows/test.yml`](.github/workflows/test.yml).
```

### Comparing `superblockify-1.0.0rc5/superblockify.egg-info/SOURCES.txt` & `superblockify-1.0.0rc6/superblockify.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 superblockify/__init__.py
 superblockify/_api.py
 superblockify/_version.py
 superblockify/attribute.py
+superblockify/cities.yml
 superblockify/config.py
 superblockify/graph_stats.py
 superblockify/logging.cfg
 superblockify/plot.py
 superblockify/utils.py
 superblockify.egg-info/PKG-INFO
 superblockify.egg-info/SOURCES.txt
```

### Comparing `superblockify-1.0.0rc5/tests/test_attribute.py` & `superblockify-1.0.0rc6/tests/test_attribute.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/tests/test_graph_stats.py` & `superblockify-1.0.0rc6/tests/test_graph_stats.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/tests/test_plot.py` & `superblockify-1.0.0rc6/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc5/tests/test_utils.py` & `superblockify-1.0.0rc6/tests/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Tests for the utils module."""
 
+from logging import DEBUG
 from os import remove
 from os.path import exists, join
 
 import pytest
 from networkx import Graph, MultiDiGraph
 from numpy import array, array_equal, int32, int64, inf, nan, isnan
 from shapely import MultiPolygon, Polygon
 
-from superblockify.config import Config
+from superblockify.config import Config, set_log_level
 from superblockify.utils import (
     load_graph_from_place,
     has_pairwise_overlap,
     compare_dicts,
     __edge_to_1d,
     __edges_to_1d,
     percentual_increase,
@@ -360,7 +361,40 @@
     especially checks if the values in the dict are equal or isomorphic if type is
     Graph.
     """
     if list2 is None:
         assert compare_components_and_partitions(list1, list1) is True
     else:
         assert compare_components_and_partitions(list1, list2) == expected
+
+
+@pytest.mark.parametrize(
+    "level",
+    [
+        10,
+        20,
+        30,
+        40,
+        50,
+        "DEBUG",
+        "INFO",
+        "WARNING",
+        "ERROR",
+        DEBUG,
+    ],
+)
+def test_set_level(level):
+    """Test `set_log_level`."""
+    set_log_level(level)
+
+
+@pytest.mark.parametrize("level", ["DEBUG1", ""])
+def test_set_level_value_error(level):
+    """Test `set_log_level` exception handling."""
+    with pytest.raises(ValueError):
+        set_log_level(level)
+
+
+def test_set_level_type_error():
+    """Test `set_log_level` exception handling."""
+    with pytest.raises(TypeError):
+        set_log_level(None)  # type: ignore
```

