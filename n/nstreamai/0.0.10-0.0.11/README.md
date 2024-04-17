# Comparing `tmp/nstreamai-0.0.10.tar.gz` & `tmp/nstreamai-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nstreamai-0.0.10.tar", last modified: Tue Apr 16 17:54:23 2024, max compression
+gzip compressed data, was "nstreamai-0.0.11.tar", last modified: Wed Apr 17 08:26:39 2024, max compression
```

## Comparing `nstreamai-0.0.10.tar` & `nstreamai-0.0.11.tar`

### file list

```diff
@@ -1,16 +1,30 @@
-drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-16 17:54:23.045680 nstreamai-0.0.10/
--rw-r--r--   0 shiv       (501) staff       (20)    35149 2024-04-16 12:23:16.000000 nstreamai-0.0.10/LICENSE
--rw-r--r--   0 shiv       (501) staff       (20)    16606 2024-04-16 17:54:23.045478 nstreamai-0.0.10/PKG-INFO
--rw-r--r--   0 shiv       (501) staff       (20)    15429 2024-04-16 15:45:18.000000 nstreamai-0.0.10/README.md
--rw-r--r--   0 shiv       (501) staff       (20)      229 2024-04-16 17:49:31.000000 nstreamai-0.0.10/pyproject.toml
--rw-r--r--   0 shiv       (501) staff       (20)       74 2024-04-16 17:54:23.045918 nstreamai-0.0.10/setup.cfg
--rw-r--r--   0 shiv       (501) staff       (20)     2063 2024-04-16 17:54:18.000000 nstreamai-0.0.10/setup.py
-drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-16 17:54:23.042963 nstreamai-0.0.10/src/
-drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-16 17:54:23.045159 nstreamai-0.0.10/src/nstreamai.egg-info/
--rw-r--r--   0 shiv       (501) staff       (20)    16606 2024-04-16 17:54:23.000000 nstreamai-0.0.10/src/nstreamai.egg-info/PKG-INFO
--rw-r--r--   0 shiv       (501) staff       (20)      272 2024-04-16 17:54:23.000000 nstreamai-0.0.10/src/nstreamai.egg-info/SOURCES.txt
--rw-r--r--   0 shiv       (501) staff       (20)        1 2024-04-16 17:54:23.000000 nstreamai-0.0.10/src/nstreamai.egg-info/dependency_links.txt
--rw-r--r--   0 shiv       (501) staff       (20)      340 2024-04-16 17:54:23.000000 nstreamai-0.0.10/src/nstreamai.egg-info/requires.txt
--rw-r--r--   0 shiv       (501) staff       (20)       21 2024-04-16 17:54:23.000000 nstreamai-0.0.10/src/nstreamai.egg-info/top_level.txt
-drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-16 17:54:23.044979 nstreamai-0.0.10/src/nstreamai_nstream_ai/
--rw-r--r--   0 shiv       (501) staff       (20)        0 2024-04-16 17:04:20.000000 nstreamai-0.0.10/src/nstreamai_nstream_ai/__init__.py
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-17 08:26:39.396360 nstreamai-0.0.11/
+-rw-r--r--   0 shiv       (501) staff       (20)    35149 2024-04-16 12:23:16.000000 nstreamai-0.0.11/LICENSE
+-rw-r--r--   0 shiv       (501) staff       (20)    16606 2024-04-17 08:26:39.396274 nstreamai-0.0.11/PKG-INFO
+-rw-r--r--   0 shiv       (501) staff       (20)    15429 2024-04-16 15:45:18.000000 nstreamai-0.0.11/README.md
+-rw-r--r--   0 shiv       (501) staff       (20)      229 2024-04-17 08:26:03.000000 nstreamai-0.0.11/pyproject.toml
+-rw-r--r--   0 shiv       (501) staff       (20)       74 2024-04-17 08:26:39.396605 nstreamai-0.0.11/setup.cfg
+-rw-r--r--   0 shiv       (501) staff       (20)     2063 2024-04-17 08:26:10.000000 nstreamai-0.0.11/setup.py
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-17 08:26:39.389042 nstreamai-0.0.11/src/
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-17 08:26:39.395967 nstreamai-0.0.11/src/nstreamai.egg-info/
+-rw-r--r--   0 shiv       (501) staff       (20)    16606 2024-04-17 08:26:39.000000 nstreamai-0.0.11/src/nstreamai.egg-info/PKG-INFO
+-rw-r--r--   0 shiv       (501) staff       (20)      774 2024-04-17 08:26:39.000000 nstreamai-0.0.11/src/nstreamai.egg-info/SOURCES.txt
+-rw-r--r--   0 shiv       (501) staff       (20)        1 2024-04-17 08:26:39.000000 nstreamai-0.0.11/src/nstreamai.egg-info/dependency_links.txt
+-rw-r--r--   0 shiv       (501) staff       (20)      340 2024-04-17 08:26:39.000000 nstreamai-0.0.11/src/nstreamai.egg-info/requires.txt
+-rw-r--r--   0 shiv       (501) staff       (20)       21 2024-04-17 08:26:39.000000 nstreamai-0.0.11/src/nstreamai.egg-info/top_level.txt
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-17 08:26:39.391237 nstreamai-0.0.11/src/nstreamai_nstream_ai/
+-rw-r--r--   0 shiv       (501) staff       (20)       58 2024-04-17 08:25:05.000000 nstreamai-0.0.11/src/nstreamai_nstream_ai/__init__.py
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-17 08:26:39.392952 nstreamai-0.0.11/src/nstreamai_nstream_ai/core/
+-rw-r--r--   0 shiv       (501) staff       (20)      340 2024-04-17 08:25:23.000000 nstreamai-0.0.11/src/nstreamai_nstream_ai/core/__init__.py
+-rw-r--r--   0 shiv       (501) staff       (20)     4490 2024-04-17 07:56:39.000000 nstreamai-0.0.11/src/nstreamai_nstream_ai/core/nsgraph.py
+-rw-r--r--   0 shiv       (501) staff       (20)     3924 2024-04-16 16:23:31.000000 nstreamai-0.0.11/src/nstreamai_nstream_ai/core/nsinit.py
+-rw-r--r--   0 shiv       (501) staff       (20)      682 2024-04-16 16:23:44.000000 nstreamai-0.0.11/src/nstreamai_nstream_ai/core/nsneuron.py
+-rw-r--r--   0 shiv       (501) staff       (20)     6971 2024-04-16 16:23:55.000000 nstreamai-0.0.11/src/nstreamai_nstream_ai/core/nsnode.py
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-17 08:26:39.395738 nstreamai-0.0.11/src/nstreamai_nstream_ai/utils/
+-rw-r--r--   0 shiv       (501) staff       (20)     1244 2024-04-17 08:25:18.000000 nstreamai-0.0.11/src/nstreamai_nstream_ai/utils/__init__.py
+-rw-r--r--   0 shiv       (501) staff       (20)     1890 2024-04-16 12:19:23.000000 nstreamai-0.0.11/src/nstreamai_nstream_ai/utils/logger.py
+-rw-r--r--   0 shiv       (501) staff       (20)      531 2024-04-17 08:17:40.000000 nstreamai-0.0.11/src/nstreamai_nstream_ai/utils/output_data.py
+-rw-r--r--   0 shiv       (501) staff       (20)     5542 2024-04-17 08:17:24.000000 nstreamai-0.0.11/src/nstreamai_nstream_ai/utils/run.py
+-rw-r--r--   0 shiv       (501) staff       (20)     6263 2024-04-17 08:16:45.000000 nstreamai-0.0.11/src/nstreamai_nstream_ai/utils/template.py
+-rw-r--r--   0 shiv       (501) staff       (20)     1182 2024-04-17 08:18:32.000000 nstreamai-0.0.11/src/nstreamai_nstream_ai/utils/variables.py
+-rw-r--r--   0 shiv       (501) staff       (20)     1191 2024-04-17 08:20:20.000000 nstreamai-0.0.11/src/nstreamai_nstream_ai/utils/welcome.py
```

### Comparing `nstreamai-0.0.10/LICENSE` & `nstreamai-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `nstreamai-0.0.10/PKG-INFO` & `nstreamai-0.0.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nstreamai
-Version: 0.0.10
+Version: 0.0.11
 Summary: Official SDK for nstream ai stream processing powered by Gen AI
 Home-page: https://github.com/nstream-ai/ms-public-sdk
 Author: Nstream AI
 Author-email: hello@nstream.ai
 License: MIT
 Keywords: nstreamai,streaming,rag,analytics,realtime
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nstreamai-0.0.10/README.md` & `nstreamai-0.0.11/README.md`

 * *Files identical despite different names*

### Comparing `nstreamai-0.0.10/setup.py` & `nstreamai-0.0.11/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 else:
     platform_specific_requires = []
 # if sys.platform == 'darwin':  # macOS
 #     extension_mod.extra_compile_args = ['-stdlib=libc++']
 
 setup(
     name='nstreamai',
-    version='0.0.10',
+    version='0.0.11',
     description='Official SDK for nstream ai stream processing powered by Gen AI',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     keywords="nstreamai, streaming, rag, analytics, realtime",
     package_dir={"": "src"},
     python_requires=">=3.8, <4",
     packages=find_packages(where="src"),
```

### Comparing `nstreamai-0.0.10/src/nstreamai.egg-info/PKG-INFO` & `nstreamai-0.0.11/src/nstreamai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nstreamai
-Version: 0.0.10
+Version: 0.0.11
 Summary: Official SDK for nstream ai stream processing powered by Gen AI
 Home-page: https://github.com/nstream-ai/ms-public-sdk
 Author: Nstream AI
 Author-email: hello@nstream.ai
 License: MIT
 Keywords: nstreamai,streaming,rag,analytics,realtime
 Classifier: License :: OSI Approved :: MIT License
```

