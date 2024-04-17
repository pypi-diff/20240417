# Comparing `tmp/jetson_examples-0.0.4.tar.gz` & `tmp/jetson_examples-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jetson_examples-0.0.4.tar", last modified: Tue Apr 16 08:45:23 2024, max compression
+gzip compressed data, was "jetson_examples-0.0.5.tar", last modified: Wed Apr 17 12:06:27 2024, max compression
```

## Comparing `jetson_examples-0.0.4.tar` & `jetson_examples-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,43 @@
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-04-16 08:45:23.316640 jetson_examples-0.0.4/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1066 2024-04-15 02:07:20.000000 jetson_examples-0.0.4/LICENSE
--rw-r--r--   0 youjiang  (1000) youjiang  (1000)     3903 2024-04-16 08:45:23.316640 jetson_examples-0.0.4/PKG-INFO
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     3253 2024-04-16 08:17:39.000000 jetson_examples-0.0.4/README.md
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-04-16 08:45:23.316640 jetson_examples-0.0.4/jetson_examples.egg-info/
--rw-r--r--   0 youjiang  (1000) youjiang  (1000)     3903 2024-04-16 08:45:23.000000 jetson_examples-0.0.4/jetson_examples.egg-info/PKG-INFO
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      388 2024-04-16 08:45:23.000000 jetson_examples-0.0.4/jetson_examples.egg-info/SOURCES.txt
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)        1 2024-04-16 08:45:23.000000 jetson_examples-0.0.4/jetson_examples.egg-info/dependency_links.txt
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       58 2024-04-16 08:45:23.000000 jetson_examples-0.0.4/jetson_examples.egg-info/entry_points.txt
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       21 2024-04-16 08:45:23.000000 jetson_examples-0.0.4/jetson_examples.egg-info/top_level.txt
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1081 2024-04-16 08:44:51.000000 jetson_examples-0.0.4/pyproject.toml
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-04-16 08:45:23.316640 jetson_examples-0.0.4/reComputer/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       22 2024-04-16 08:39:05.000000 jetson_examples-0.0.4/reComputer/__init__.py
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      809 2024-04-16 08:39:05.000000 jetson_examples-0.0.4/reComputer/main.py
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-04-16 08:45:23.316640 jetson_examples-0.0.4/reComputer/scripts/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      127 2024-04-16 08:39:05.000000 jetson_examples-0.0.4/reComputer/scripts/check.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)    10137 2024-04-16 08:42:42.000000 jetson_examples-0.0.4/reComputer/scripts/live-llava.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1875 2024-04-16 08:39:05.000000 jetson_examples-0.0.4/reComputer/scripts/nanodb.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     3585 2024-04-16 08:39:05.000000 jetson_examples-0.0.4/reComputer/scripts/run.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       38 2024-04-16 08:45:23.316640 jetson_examples-0.0.4/setup.cfg
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.308756 jetson_examples-0.0.5/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)     1066 2024-04-16 06:52:15.000000 jetson_examples-0.0.5/LICENSE
+-rw-r--r--   0 seeed     (1000) seeed     (1000)     3982 2024-04-17 12:06:27.308756 jetson_examples-0.0.5/PKG-INFO
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)     3332 2024-04-17 04:12:01.000000 jetson_examples-0.0.5/README.md
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.308756 jetson_examples-0.0.5/jetson_examples.egg-info/
+-rw-r--r--   0 seeed     (1000) seeed     (1000)     3982 2024-04-17 12:06:27.000000 jetson_examples-0.0.5/jetson_examples.egg-info/PKG-INFO
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)      878 2024-04-17 12:06:27.000000 jetson_examples-0.0.5/jetson_examples.egg-info/SOURCES.txt
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)        1 2024-04-17 12:06:27.000000 jetson_examples-0.0.5/jetson_examples.egg-info/dependency_links.txt
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)       58 2024-04-17 12:06:27.000000 jetson_examples-0.0.5/jetson_examples.egg-info/entry_points.txt
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)       27 2024-04-17 12:06:27.000000 jetson_examples-0.0.5/jetson_examples.egg-info/top_level.txt
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)     1081 2024-04-17 12:05:45.000000 jetson_examples-0.0.5/pyproject.toml
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.304756 jetson_examples-0.0.5/reComputer/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)       22 2024-04-17 12:05:53.000000 jetson_examples-0.0.5/reComputer/__init__.py
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)     1821 2024-04-17 12:03:58.000000 jetson_examples-0.0.5/reComputer/main.py
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.304756 jetson_examples-0.0.5/reComputer/scripts/
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.304756 jetson_examples-0.0.5/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)      134 2024-04-16 09:51:17.000000 jetson_examples-0.0.5/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/run.sh
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)      127 2024-04-16 09:45:34.000000 jetson_examples-0.0.5/reComputer/scripts/check.sh
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.304756 jetson_examples-0.0.5/reComputer/scripts/hello-world/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)       87 2024-04-17 03:08:32.000000 jetson_examples-0.0.5/reComputer/scripts/hello-world/readme.md
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)      280 2024-04-17 11:37:51.000000 jetson_examples-0.0.5/reComputer/scripts/hello-world/run.sh
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.304756 jetson_examples-0.0.5/reComputer/scripts/live-llava/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)    10137 2024-04-16 09:45:34.000000 jetson_examples-0.0.5/reComputer/scripts/live-llava/run.sh
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.304756 jetson_examples-0.0.5/reComputer/scripts/llava/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)      148 2024-04-16 09:49:26.000000 jetson_examples-0.0.5/reComputer/scripts/llava/run.sh
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.304756 jetson_examples-0.0.5/reComputer/scripts/llava-v1.5-7b/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)      147 2024-04-16 09:50:12.000000 jetson_examples-0.0.5/reComputer/scripts/llava-v1.5-7b/run.sh
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.304756 jetson_examples-0.0.5/reComputer/scripts/llava-v1.6-vicuna-7b/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)      165 2024-04-16 09:50:51.000000 jetson_examples-0.0.5/reComputer/scripts/llava-v1.6-vicuna-7b/run.sh
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.304756 jetson_examples-0.0.5/reComputer/scripts/nanodb/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)      247 2024-04-16 10:00:31.000000 jetson_examples-0.0.5/reComputer/scripts/nanodb/readme.md
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)     1875 2024-04-16 09:45:34.000000 jetson_examples-0.0.5/reComputer/scripts/nanodb/run.sh
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.308756 jetson_examples-0.0.5/reComputer/scripts/nanoowl/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)      161 2024-04-16 09:53:17.000000 jetson_examples-0.0.5/reComputer/scripts/nanoowl/run.sh
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)     2066 2024-04-17 11:48:07.000000 jetson_examples-0.0.5/reComputer/scripts/run.sh
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.308756 jetson_examples-0.0.5/reComputer/scripts/stable-diffusion-webui/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)       57 2024-04-16 09:52:42.000000 jetson_examples-0.0.5/reComputer/scripts/stable-diffusion-webui/run.sh
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.308756 jetson_examples-0.0.5/reComputer/scripts/text-generation-webui/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)      304 2024-04-16 09:52:01.000000 jetson_examples-0.0.5/reComputer/scripts/text-generation-webui/run.sh
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)      900 2024-04-17 12:02:17.000000 jetson_examples-0.0.5/reComputer/scripts/update.sh
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.308756 jetson_examples-0.0.5/reComputer/scripts/whisper/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)       43 2024-04-16 09:53:47.000000 jetson_examples-0.0.5/reComputer/scripts/whisper/run.sh
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)       38 2024-04-17 12:06:27.308756 jetson_examples-0.0.5/setup.cfg
```

### Comparing `jetson_examples-0.0.4/LICENSE` & `jetson_examples-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.0.4/PKG-INFO` & `jetson_examples-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetson-examples
-Version: 0.0.4
+Version: 0.0.5
 Summary: Running Gen AI models and applications on NVIDIA Jetson devices with one-line command
 Author-email: luozhixin <zhixin.luo@seeed.cc>
 Project-URL: Homepage, https://github.com/Seeed-Projects/jetson-examples
 Project-URL: Issues, https://github.com/Seeed-Projects/jetson-examples/issues
 Keywords: llama,llava,gpt,llm,nvidia,jetson,multimodal,jetson orin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -57,14 +57,16 @@
 | nanodb                 | Vector Database          | 76GB            | 7.0GB      | `reComputer run nanodb`                 |
 | whisper                | Audio                    | 1.5GB           | 6.0GB      | `reComputer run whisper`                |
 
 > Note: You should have enough space to run example, like `LLaVA`, at least `27.4GB` totally
 
 More Examples can be found [examples.md](./docs/examples.md)
 
+Want to add a Example by yourself? Check this [develop.md](./docs/develop.md)
+
 ## TODO List
 
 - [ ] check disk space enough or not before run
 - [ ] allow to setting some configs, such as `BASE_PATH`
 - [ ] detect host environment and install what we need
 - [ ] support jetson-containers update
 - [ ] all type jetson support checking list
```

### Comparing `jetson_examples-0.0.4/README.md` & `jetson_examples-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 | nanodb                 | Vector Database          | 76GB            | 7.0GB      | `reComputer run nanodb`                 |
 | whisper                | Audio                    | 1.5GB           | 6.0GB      | `reComputer run whisper`                |
 
 > Note: You should have enough space to run example, like `LLaVA`, at least `27.4GB` totally
 
 More Examples can be found [examples.md](./docs/examples.md)
 
+Want to add a Example by yourself? Check this [develop.md](./docs/develop.md)
+
 ## TODO List
 
 - [ ] check disk space enough or not before run
 - [ ] allow to setting some configs, such as `BASE_PATH`
 - [ ] detect host environment and install what we need
 - [ ] support jetson-containers update
 - [ ] all type jetson support checking list
```

### Comparing `jetson_examples-0.0.4/jetson_examples.egg-info/PKG-INFO` & `jetson_examples-0.0.5/jetson_examples.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetson-examples
-Version: 0.0.4
+Version: 0.0.5
 Summary: Running Gen AI models and applications on NVIDIA Jetson devices with one-line command
 Author-email: luozhixin <zhixin.luo@seeed.cc>
 Project-URL: Homepage, https://github.com/Seeed-Projects/jetson-examples
 Project-URL: Issues, https://github.com/Seeed-Projects/jetson-examples/issues
 Keywords: llama,llava,gpt,llm,nvidia,jetson,multimodal,jetson orin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -57,14 +57,16 @@
 | nanodb                 | Vector Database          | 76GB            | 7.0GB      | `reComputer run nanodb`                 |
 | whisper                | Audio                    | 1.5GB           | 6.0GB      | `reComputer run whisper`                |
 
 > Note: You should have enough space to run example, like `LLaVA`, at least `27.4GB` totally
 
 More Examples can be found [examples.md](./docs/examples.md)
 
+Want to add a Example by yourself? Check this [develop.md](./docs/develop.md)
+
 ## TODO List
 
 - [ ] check disk space enough or not before run
 - [ ] allow to setting some configs, such as `BASE_PATH`
 - [ ] detect host environment and install what we need
 - [ ] support jetson-containers update
 - [ ] all type jetson support checking list
```

### Comparing `jetson_examples-0.0.4/pyproject.toml` & `jetson_examples-0.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=57.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jetson-examples"
-version = "0.0.4"
+version = "0.0.5"
 authors = [{ name = "luozhixin", email = "zhixin.luo@seeed.cc" }]
 description = "Running Gen AI models and applications on NVIDIA Jetson devices with one-line command"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
@@ -35,8 +35,8 @@
 # Tools settings -------------------------------------------------------------------------------------------------------
 
 [tool.setuptools.packages.find]
 namespaces = true
 where = ["."]
 
 [tool.setuptools.package-data]
-"reComputer.scripts" = ["*.sh"]
+"reComputer.scripts" = ["**/*"]
```

### Comparing `jetson_examples-0.0.4/reComputer/scripts/live-llava.sh` & `jetson_examples-0.0.5/reComputer/scripts/live-llava/run.sh`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.0.4/reComputer/scripts/nanodb.sh` & `jetson_examples-0.0.5/reComputer/scripts/nanodb/run.sh`

 * *Files identical despite different names*

