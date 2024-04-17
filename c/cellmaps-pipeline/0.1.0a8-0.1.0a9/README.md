# Comparing `tmp/cellmaps_pipeline-0.1.0a8.tar.gz` & `tmp/cellmaps_pipeline-0.1.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_pipeline-0.1.0a8.tar", last modified: Mon Aug 14 22:00:07 2023, max compression
+gzip compressed data, was "dist/cellmaps_pipeline-0.1.0a9.tar", last modified: Thu Aug 17 23:54:51 2023, max compression
```

## Comparing `cellmaps_pipeline-0.1.0a8.tar` & `cellmaps_pipeline-0.1.0a9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-14 22:00:07.445028 cellmaps_pipeline-0.1.0a8/
--rw-r--r--   0 churas     (504) staff       (20)      266 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3649 2023-08-09 17:03:55.000000 cellmaps_pipeline-0.1.0a8/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     5991 2023-08-14 22:00:07.445339 cellmaps_pipeline-0.1.0a8/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     4006 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-14 22:00:07.433516 cellmaps_pipeline-0.1.0a8/cellmaps_pipeline/
--rw-r--r--   0 churas     (504) staff       (20)      282 2023-08-14 21:59:51.000000 cellmaps_pipeline-0.1.0a8/cellmaps_pipeline/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)    10509 2023-08-14 21:59:51.000000 cellmaps_pipeline-0.1.0a8/cellmaps_pipeline/cellmaps_pipelinecmd.py
--rw-r--r--   0 churas     (504) staff       (20)      132 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/cellmaps_pipeline/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)    15198 2023-08-14 21:59:51.000000 cellmaps_pipeline-0.1.0a8/cellmaps_pipeline/runner.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-14 22:00:07.435573 cellmaps_pipeline-0.1.0a8/cellmaps_pipeline.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     5991 2023-08-14 22:00:07.000000 cellmaps_pipeline-0.1.0a8/cellmaps_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     1134 2023-08-14 22:00:07.000000 cellmaps_pipeline-0.1.0a8/cellmaps_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-08-14 22:00:07.000000 cellmaps_pipeline-0.1.0a8/cellmaps_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-08-14 22:00:07.000000 cellmaps_pipeline-0.1.0a8/cellmaps_pipeline.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)      249 2023-08-14 22:00:07.000000 cellmaps_pipeline-0.1.0a8/cellmaps_pipeline.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       18 2023-08-14 22:00:07.000000 cellmaps_pipeline-0.1.0a8/cellmaps_pipeline.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-14 22:00:07.441489 cellmaps_pipeline-0.1.0a8/docs/
--rwxr-xr-x   0 churas     (504) staff       (20)     4096 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/docs/._cellmaps_pipeline.rst
--rw-r--r--   0 churas     (504) staff       (20)      618 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-14 22:00:07.428085 cellmaps_pipeline-0.1.0a8/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-14 22:00:07.428272 cellmaps_pipeline-0.1.0a8/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-14 22:00:07.441782 cellmaps_pipeline-0.1.0a8/docs/_build/html/_images/
--rw-r--r--   0 churas     (504) staff       (20)    31213 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/docs/_build/html/_images/pipeline_overview.png
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-14 22:00:07.442921 cellmaps_pipeline-0.1.0a8/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a8/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a8/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a8/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)      757 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/docs/cellmaps_pipeline.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6051 2023-08-09 17:02:19.000000 cellmaps_pipeline-0.1.0a8/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      285 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/docs/history.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-14 22:00:07.443296 cellmaps_pipeline-0.1.0a8/docs/images/
--rw-r--r--   0 churas     (504) staff       (20)    31213 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/docs/images/pipeline_overview.png
--rw-r--r--   0 churas     (504) staff       (20)     1852 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1201 2023-08-09 17:03:55.000000 cellmaps_pipeline-0.1.0a8/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      451 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      815 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       76 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4340 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      787 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)     1363 2023-08-09 17:03:55.000000 cellmaps_pipeline-0.1.0a8/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      400 2023-08-14 22:00:07.446076 cellmaps_pipeline-0.1.0a8/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     2485 2023-08-14 21:59:51.000000 cellmaps_pipeline-0.1.0a8/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-14 22:00:07.444754 cellmaps_pipeline-0.1.0a8/tests/
--rw-r--r--   0 churas     (504) staff       (20)       72 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/tests/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     1296 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/tests/test_cellmaps_pipelinecmd.py
--rw-r--r--   0 churas     (504) staff       (20)      896 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/tests/test_cellmapspipeline.py
--rw-r--r--   0 churas     (504) staff       (20)      772 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a8/tests/test_integration_cellmaps_pipeline.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-17 23:54:51.708671 cellmaps_pipeline-0.1.0a9/
+-rw-r--r--   0 churas     (504) staff       (20)      266 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3649 2023-08-09 17:03:55.000000 cellmaps_pipeline-0.1.0a9/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     5991 2023-08-17 23:54:51.708801 cellmaps_pipeline-0.1.0a9/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     4006 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-17 23:54:51.700870 cellmaps_pipeline-0.1.0a9/cellmaps_pipeline/
+-rw-r--r--   0 churas     (504) staff       (20)      282 2023-08-17 23:54:31.000000 cellmaps_pipeline-0.1.0a9/cellmaps_pipeline/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)    10509 2023-08-16 20:46:21.000000 cellmaps_pipeline-0.1.0a9/cellmaps_pipeline/cellmaps_pipelinecmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      132 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/cellmaps_pipeline/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)    16507 2023-08-17 23:54:31.000000 cellmaps_pipeline-0.1.0a9/cellmaps_pipeline/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-17 23:54:51.702370 cellmaps_pipeline-0.1.0a9/cellmaps_pipeline.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     5991 2023-08-17 23:54:51.000000 cellmaps_pipeline-0.1.0a9/cellmaps_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1134 2023-08-17 23:54:51.000000 cellmaps_pipeline-0.1.0a9/cellmaps_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-08-17 23:54:51.000000 cellmaps_pipeline-0.1.0a9/cellmaps_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-08-17 23:54:51.000000 cellmaps_pipeline-0.1.0a9/cellmaps_pipeline.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)      250 2023-08-17 23:54:51.000000 cellmaps_pipeline-0.1.0a9/cellmaps_pipeline.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       18 2023-08-17 23:54:51.000000 cellmaps_pipeline-0.1.0a9/cellmaps_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-17 23:54:51.706338 cellmaps_pipeline-0.1.0a9/docs/
+-rwxr-xr-x   0 churas     (504) staff       (20)     4096 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/docs/._cellmaps_pipeline.rst
+-rw-r--r--   0 churas     (504) staff       (20)      618 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-17 23:54:51.695381 cellmaps_pipeline-0.1.0a9/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-17 23:54:51.695684 cellmaps_pipeline-0.1.0a9/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-17 23:54:51.706596 cellmaps_pipeline-0.1.0a9/docs/_build/html/_images/
+-rw-r--r--   0 churas     (504) staff       (20)    31213 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/docs/_build/html/_images/pipeline_overview.png
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-17 23:54:51.707314 cellmaps_pipeline-0.1.0a9/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a9/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a9/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a9/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)      757 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/docs/cellmaps_pipeline.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6051 2023-08-09 17:02:19.000000 cellmaps_pipeline-0.1.0a9/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      285 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/docs/history.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-17 23:54:51.707527 cellmaps_pipeline-0.1.0a9/docs/images/
+-rw-r--r--   0 churas     (504) staff       (20)    31213 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/docs/images/pipeline_overview.png
+-rw-r--r--   0 churas     (504) staff       (20)     1852 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1201 2023-08-09 17:03:55.000000 cellmaps_pipeline-0.1.0a9/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      451 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      815 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       76 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4340 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      787 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1363 2023-08-09 17:03:55.000000 cellmaps_pipeline-0.1.0a9/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      400 2023-08-17 23:54:51.709396 cellmaps_pipeline-0.1.0a9/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     2486 2023-08-17 23:54:31.000000 cellmaps_pipeline-0.1.0a9/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-17 23:54:51.708486 cellmaps_pipeline-0.1.0a9/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       72 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/tests/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     1296 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/tests/test_cellmaps_pipelinecmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      896 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/tests/test_cellmapspipeline.py
+-rw-r--r--   0 churas     (504) staff       (20)      772 2023-08-09 17:00:59.000000 cellmaps_pipeline-0.1.0a9/tests/test_integration_cellmaps_pipeline.py
```

### Comparing `cellmaps_pipeline-0.1.0a8/CONTRIBUTING.rst` & `cellmaps_pipeline-0.1.0a9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a8/LICENSE` & `cellmaps_pipeline-0.1.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a8/PKG-INFO` & `cellmaps_pipeline-0.1.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps_pipeline
-Version: 0.1.0a8
+Version: 0.1.0a9
 Summary: Runs full Cell Maps pipeline
 Home-page: https://github.com/idekerlab/cellmaps_pipeline
 Author: Ideker Lab Cell Maps team
 Author-email: tools@cm4ai.org
 License: MIT license
 Description: ===================
         Cell Maps Pipeline
```

### Comparing `cellmaps_pipeline-0.1.0a8/README.rst` & `cellmaps_pipeline-0.1.0a9/README.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a8/cellmaps_pipeline/cellmaps_pipelinecmd.py` & `cellmaps_pipeline-0.1.0a9/cellmaps_pipeline/cellmaps_pipelinecmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a8/cellmaps_pipeline/runner.py` & `cellmaps_pipeline-0.1.0a9/cellmaps_pipeline/runner.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,16 +57,62 @@
         :param cmd:
         :raises NotImplementedError: Always raised cause
                                      subclasses need to implement
         """
         raise NotImplementedError('subclasses need to implement')
 
 
+class SLURMPipelineRunner(PipelineRunner):
+    """
+    Generates SLURM batch files and wrapper script to
+    run various steps in a SLURM environment
+    """
+    def __init__(self, outdir=None,
+                 samples=None,
+                 unique=None,
+                 edgelist=None,
+                 baitlist=None,
+                 model_path=None,
+                 proteinatlasxml=None,
+                 ppi_cutoffs=None,
+                 fake=None,
+                 provenance=None,
+                 provenance_utils=ProvenanceUtil(),
+                 fold=[1],
+                 input_data_dict=None):
+        """
+
+        :param outdir:
+        :param samples:
+        :param unique:
+        :param edgelist:
+        :param baitlist:
+        :param model_path:
+        :param proteinatlasxml:
+        :param ppi_cutoffs:
+        :param fake:
+        :param provenance:
+        :param provenance_utils:
+        :param fold:
+        :param input_data_dict:
+        """
+        pass
+
+    def run(self):
+        """
+        Runs pipeline
+        :param cmd:
+        :raises NotImplementedError: Always raised cause
+                                     subclasses need to implement
+        """
+        raise NotImplementedError('not implemented yet')
+
 class ProgrammaticPipelineRunner(PipelineRunner):
     """
+    Runs pipeline programmatically in a serial fashion
 
     """
     def __init__(self, outdir=None,
                  samples=None,
                  unique=None,
                  edgelist=None,
                  baitlist=None,
```

### Comparing `cellmaps_pipeline-0.1.0a8/cellmaps_pipeline.egg-info/PKG-INFO` & `cellmaps_pipeline-0.1.0a9/cellmaps_pipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps-pipeline
-Version: 0.1.0a8
+Version: 0.1.0a9
 Summary: Runs full Cell Maps pipeline
 Home-page: https://github.com/idekerlab/cellmaps_pipeline
 Author: Ideker Lab Cell Maps team
 Author-email: tools@cm4ai.org
 License: MIT license
 Description: ===================
         Cell Maps Pipeline
```

### Comparing `cellmaps_pipeline-0.1.0a8/cellmaps_pipeline.egg-info/SOURCES.txt` & `cellmaps_pipeline-0.1.0a9/cellmaps_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a8/docs/._cellmaps_pipeline.rst` & `cellmaps_pipeline-0.1.0a9/docs/._cellmaps_pipeline.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a8/docs/Makefile` & `cellmaps_pipeline-0.1.0a9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a8/docs/_build/html/_images/pipeline_overview.png` & `cellmaps_pipeline-0.1.0a9/docs/_build/html/_images/pipeline_overview.png`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a8/docs/cellmaps_pipeline.rst` & `cellmaps_pipeline-0.1.0a9/docs/cellmaps_pipeline.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a8/docs/conf.py` & `cellmaps_pipeline-0.1.0a9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a8/docs/images/pipeline_overview.png` & `cellmaps_pipeline-0.1.0a9/docs/images/pipeline_overview.png`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a8/docs/index.rst` & `cellmaps_pipeline-0.1.0a9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a8/docs/installation.rst` & `cellmaps_pipeline-0.1.0a9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a8/docs/make.bat` & `cellmaps_pipeline-0.1.0a9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a8/docs/newrelease.rst` & `cellmaps_pipeline-0.1.0a9/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a8/docs/pypircfile.rst` & `cellmaps_pipeline-0.1.0a9/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a8/docs/usage.rst` & `cellmaps_pipeline-0.1.0a9/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a8/docs/versioningscheme.rst` & `cellmaps_pipeline-0.1.0a9/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a8/setup.py` & `cellmaps_pipeline-0.1.0a9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-requirements = ['cellmaps_utils==0.1.0a16',
-                'cellmaps_imagedownloader==0.1.0a10',
-                'cellmaps_ppidownloader==0.1.0a3',
-                'cellmaps_image_embedding==0.1.0a9',
-                'cellmaps_ppi_embedding==0.1.0a5',
-                'cellmaps_coembedding==0.1.0a5',
-                'cellmaps_generate_hierarchy==0.1.0a8',
+requirements = ['cellmaps_utils==0.1.0a18',
+                'cellmaps_imagedownloader==0.1.0a11',
+                'cellmaps_ppidownloader==0.1.0a4',
+                'cellmaps_image_embedding==0.1.0a10',
+                'cellmaps_ppi_embedding==0.1.0a6',
+                'cellmaps_coembedding==0.1.0a6',
+                'cellmaps_generate_hierarchy==0.1.0a9',
                 'networkx>=2.8,<2.9',
                 'tqdm']
 
 setup_requirements = [ ]
 
 test_requirements = [ ]
```

### Comparing `cellmaps_pipeline-0.1.0a8/tests/test_cellmaps_pipelinecmd.py` & `cellmaps_pipeline-0.1.0a9/tests/test_cellmaps_pipelinecmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a8/tests/test_cellmapspipeline.py` & `cellmaps_pipeline-0.1.0a9/tests/test_cellmapspipeline.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a8/tests/test_integration_cellmaps_pipeline.py` & `cellmaps_pipeline-0.1.0a9/tests/test_integration_cellmaps_pipeline.py`

 * *Files identical despite different names*

