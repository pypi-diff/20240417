# Comparing `tmp/towbintools-0.1.4.tar.gz` & `tmp/towbintools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "towbintools-0.1.4.tar", last modified: Thu Apr 11 13:41:38 2024, max compression
+gzip compressed data, was "towbintools-0.1.5.tar", last modified: Wed Apr 17 14:30:26 2024, max compression
```

## Comparing `towbintools-0.1.4.tar` & `towbintools-0.1.5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:38.878879 towbintools-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-11 13:41:34.000000 towbintools-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-11 13:41:38.878879 towbintools-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-11 13:41:34.000000 towbintools-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-11 13:41:34.000000 towbintools-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:41:38.878879 towbintools-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:38.870879 towbintools-0.1.4/towbintools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:38.874879 towbintools-0.1.4/towbintools/classification/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/classification/classification_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:38.874879 towbintools-0.1.4/towbintools/data_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/data_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/data_analysis/growth_rate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:38.874879 towbintools-0.1.4/towbintools/deep_learning/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/deep_learning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:38.874879 towbintools-0.1.4/towbintools/deep_learning/architectures/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/deep_learning/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/deep_learning/architectures/archs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/deep_learning/architectures/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/deep_learning/deep_learning_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:38.874879 towbintools-0.1.4/towbintools/deep_learning/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/deep_learning/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/deep_learning/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12509 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/deep_learning/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/deep_learning/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/deep_learning/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:38.878879 towbintools-0.1.4/towbintools/foundation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/foundation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/foundation/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/foundation/binary_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    15736 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/foundation/detect_molts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/foundation/file_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)    10683 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/foundation/image_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/foundation/image_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/foundation/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/foundation/worm_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/foundation/zstack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:38.878879 towbintools-0.1.4/towbintools/legacy_straightening/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/legacy_straightening/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/legacy_straightening/straightening_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:38.878879 towbintools-0.1.4/towbintools/quantification/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/quantification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/quantification/quantification_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:38.878879 towbintools-0.1.4/towbintools/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12175 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/segmentation/segmentation_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:38.878879 towbintools-0.1.4/towbintools/straightening/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/straightening/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35283 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/straightening/straightening_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:38.878879 towbintools-0.1.4/towbintools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-11 13:41:38.000000 towbintools-0.1.4/towbintools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-11 13:41:38.000000 towbintools-0.1.4/towbintools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:41:38.000000 towbintools-0.1.4/towbintools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-11 13:41:38.000000 towbintools-0.1.4/towbintools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 13:41:38.000000 towbintools-0.1.4/towbintools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:26.114070 towbintools-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-17 14:30:21.000000 towbintools-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-17 14:30:26.114070 towbintools-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-17 14:30:21.000000 towbintools-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-17 14:30:21.000000 towbintools-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 14:30:26.114070 towbintools-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:26.106070 towbintools-0.1.5/towbintools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:26.106070 towbintools-0.1.5/towbintools/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/classification/classification_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:26.106070 towbintools-0.1.5/towbintools/data_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/data_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/data_analysis/growth_rate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:26.106070 towbintools-0.1.5/towbintools/deep_learning/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/deep_learning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:26.110070 towbintools-0.1.5/towbintools/deep_learning/architectures/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/deep_learning/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/deep_learning/architectures/archs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/deep_learning/architectures/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/deep_learning/deep_learning_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:26.110070 towbintools-0.1.5/towbintools/deep_learning/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/deep_learning/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/deep_learning/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12509 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/deep_learning/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/deep_learning/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/deep_learning/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:26.110070 towbintools-0.1.5/towbintools/foundation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/foundation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/foundation/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/foundation/binary_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15736 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/foundation/detect_molts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/foundation/file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10683 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/foundation/image_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/foundation/image_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/foundation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/foundation/worm_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/foundation/zstack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:26.110070 towbintools-0.1.5/towbintools/legacy_straightening/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/legacy_straightening/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/legacy_straightening/straightening_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:26.110070 towbintools-0.1.5/towbintools/quantification/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/quantification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/quantification/quantification_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:26.110070 towbintools-0.1.5/towbintools/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12298 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/segmentation/segmentation_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:26.110070 towbintools-0.1.5/towbintools/straightening/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/straightening/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35283 2024-04-17 14:30:21.000000 towbintools-0.1.5/towbintools/straightening/straightening_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:30:26.110070 towbintools-0.1.5/towbintools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-17 14:30:26.000000 towbintools-0.1.5/towbintools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-17 14:30:26.000000 towbintools-0.1.5/towbintools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 14:30:26.000000 towbintools-0.1.5/towbintools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-17 14:30:26.000000 towbintools-0.1.5/towbintools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 14:30:26.000000 towbintools-0.1.5/towbintools.egg-info/top_level.txt
```

### Comparing `towbintools-0.1.4/LICENSE` & `towbintools-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.4/PKG-INFO` & `towbintools-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: towbintools
-Version: 0.1.4
+Version: 0.1.5
 Summary: All the tools used by the Towbin Lab !
 Author-email: Sacha Psalmon <sacha.psalmon@unibe.ch>, Boris Gusev <boris.gusev@unibe.ch>
 Maintainer-email: Sacha Psalmon <sacha.psalmon@unibe.ch>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.22.4
```

### Comparing `towbintools-0.1.4/README.md` & `towbintools-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.4/pyproject.toml` & `towbintools-0.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "towbintools"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   {name="Sacha Psalmon", email="sacha.psalmon@unibe.ch" },
   {name="Boris Gusev", email="boris.gusev@unibe.ch" }
 ]
 maintainers = [
     {name = "Sacha Psalmon", email="sacha.psalmon@unibe.ch"},
 ]
```

### Comparing `towbintools-0.1.4/towbintools/classification/classification_tools.py` & `towbintools-0.1.5/towbintools/classification/classification_tools.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.4/towbintools/data_analysis/growth_rate.py` & `towbintools-0.1.5/towbintools/data_analysis/growth_rate.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.4/towbintools/deep_learning/architectures/archs.py` & `towbintools-0.1.5/towbintools/deep_learning/architectures/archs.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.4/towbintools/deep_learning/architectures/models.py` & `towbintools-0.1.5/towbintools/deep_learning/architectures/models.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.4/towbintools/deep_learning/deep_learning_tools.py` & `towbintools-0.1.5/towbintools/deep_learning/deep_learning_tools.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.4/towbintools/deep_learning/utils/augmentation.py` & `towbintools-0.1.5/towbintools/deep_learning/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.4/towbintools/deep_learning/utils/dataset.py` & `towbintools-0.1.5/towbintools/deep_learning/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.4/towbintools/deep_learning/utils/loss.py` & `towbintools-0.1.5/towbintools/deep_learning/utils/loss.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.4/towbintools/foundation/backbone.py` & `towbintools-0.1.5/towbintools/foundation/backbone.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.4/towbintools/foundation/binary_image.py` & `towbintools-0.1.5/towbintools/foundation/binary_image.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.4/towbintools/foundation/detect_molts.py` & `towbintools-0.1.5/towbintools/foundation/detect_molts.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.4/towbintools/foundation/file_handling.py` & `towbintools-0.1.5/towbintools/foundation/file_handling.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.4/towbintools/foundation/image_handling.py` & `towbintools-0.1.5/towbintools/foundation/image_handling.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.4/towbintools/foundation/image_quality.py` & `towbintools-0.1.5/towbintools/foundation/image_quality.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.4/towbintools/foundation/utils.py` & `towbintools-0.1.5/towbintools/foundation/utils.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.4/towbintools/foundation/worm_features.py` & `towbintools-0.1.5/towbintools/foundation/worm_features.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.4/towbintools/foundation/zstack.py` & `towbintools-0.1.5/towbintools/foundation/zstack.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.4/towbintools/legacy_straightening/straightening_tools.py` & `towbintools-0.1.5/towbintools/legacy_straightening/straightening_tools.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.4/towbintools/quantification/quantification_tools.py` & `towbintools-0.1.5/towbintools/quantification/quantification_tools.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.4/towbintools/segmentation/segmentation_tools.py` & `towbintools-0.1.5/towbintools/segmentation/segmentation_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,29 +275,38 @@
     histogram = skimage.exposure.histogram(image, nbins=nbins)
     hist_vals, bin_centers = histogram
     # limited_mean lies somewhere in the histogram peak for background
     limited_mean = _mode_limited_mean(image, histogram=histogram)
     # threshold_triangle by-and-large finds the threshold for the bottom of background peak
     # so it's a good starting point for otsu threshold, which can struggle in the case when background is so large as a proportion of the image that the overall histogram appears to be unimodal
     thresh_lower_bound = image.min()
+    i = 0
     while thresh_lower_bound < limited_mean:
         # >= to allow possibility of thresh_lower_bound == limited_mean
         thresh_lower_bound = threshold_triangle(
             image[image >= thresh_lower_bound], nbins=nbins
         )
+        if i > 64:
+            break
+        i += 1
 
     # don't start right at lower bound because the histogram information below thresh_lower_bound may be useful in determining a good threshold in the last iteration
     # for example, when thresh_lower_bound is already a decent threshold, in which case the the very information used to calculate it would have been discarded
     thresh = image.min()
+    i = 0
     while thresh < thresh_lower_bound:
         # crop histogram to only include values above the current threshold
-        hist_vals = hist_vals[bin_centers >= thresh]
-        bin_centers = bin_centers[bin_centers >= thresh]
+        hist_vals = hist_vals[bin_centers > thresh]
+        bin_centers = bin_centers[bin_centers > thresh]
         thresh = threshold_otsu(hist=(hist_vals, bin_centers))
 
+        if i > 64:
+            break
+        i += 1
+
     # rescale threshold back to original image range and dtype since threshold is in (0, 1)
     # rather than do the math ourselves, let skimage do it as it also handles float quantization
     thresh = skimage.exposure.rescale_intensity(
         np.array(thresh).reshape(1, 1), in_range=(0, 1), out_range=image_range
     ).astype(image_dtype)[0, 0]
 
     return thresh
```

### Comparing `towbintools-0.1.4/towbintools/straightening/straightening_tools.py` & `towbintools-0.1.5/towbintools/straightening/straightening_tools.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.4/towbintools.egg-info/PKG-INFO` & `towbintools-0.1.5/towbintools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: towbintools
-Version: 0.1.4
+Version: 0.1.5
 Summary: All the tools used by the Towbin Lab !
 Author-email: Sacha Psalmon <sacha.psalmon@unibe.ch>, Boris Gusev <boris.gusev@unibe.ch>
 Maintainer-email: Sacha Psalmon <sacha.psalmon@unibe.ch>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.22.4
```

### Comparing `towbintools-0.1.4/towbintools.egg-info/SOURCES.txt` & `towbintools-0.1.5/towbintools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

