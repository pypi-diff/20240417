# Comparing `tmp/thepipe_api-0.2.4.tar.gz` & `tmp/thepipe_api-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thepipe_api-0.2.4.tar", last modified: Wed Apr 17 05:13:16 2024, max compression
+gzip compressed data, was "thepipe_api-0.2.5.tar", last modified: Wed Apr 17 06:24:03 2024, max compression
```

## Comparing `thepipe_api-0.2.4.tar` & `thepipe_api-0.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 05:13:16.960183 thepipe_api-0.2.4/
--rw-rw-rw-   0        0        0     1094 2024-03-27 18:15:40.000000 thepipe_api-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     9795 2024-04-17 05:13:16.959183 thepipe_api-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     9068 2024-04-16 05:29:43.000000 thepipe_api-0.2.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-17 05:13:16.960183 thepipe_api-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      859 2024-04-17 05:12:50.000000 thepipe_api-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 05:13:16.933184 thepipe_api-0.2.4/tests/
--rw-rw-rw-   0        0        0        0 2024-03-23 01:45:32.000000 thepipe_api-0.2.4/tests/__init__.py
--rw-rw-rw-   0        0        0     9265 2024-04-16 16:00:52.000000 thepipe_api-0.2.4/tests/test_thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-17 05:13:16.939188 thepipe_api-0.2.4/thepipe_api/
--rw-rw-rw-   0        0        0       86 2024-04-15 22:46:19.000000 thepipe_api-0.2.4/thepipe_api/__init__.py
--rw-rw-rw-   0        0        0     4821 2024-04-13 20:40:22.000000 thepipe_api-0.2.4/thepipe_api/compressor.py
--rw-rw-rw-   0        0        0     2778 2024-04-16 05:18:22.000000 thepipe_api-0.2.4/thepipe_api/core.py
--rw-rw-rw-   0        0        0    20809 2024-04-17 04:51:51.000000 thepipe_api-0.2.4/thepipe_api/extractor.py
--rw-rw-rw-   0        0        0     3649 2024-04-16 23:07:34.000000 thepipe_api-0.2.4/thepipe_api/thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-17 05:13:16.957186 thepipe_api-0.2.4/thepipe_api.egg-info/
--rw-rw-rw-   0        0        0     9795 2024-04-17 05:13:16.000000 thepipe_api-0.2.4/thepipe_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2024-04-17 05:13:16.000000 thepipe_api-0.2.4/thepipe_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 05:13:16.000000 thepipe_api-0.2.4/thepipe_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-17 05:13:16.000000 thepipe_api-0.2.4/thepipe_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      104 2024-04-17 05:13:16.000000 thepipe_api-0.2.4/thepipe_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-17 05:13:16.000000 thepipe_api-0.2.4/thepipe_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 06:24:03.978412 thepipe_api-0.2.5/
+-rw-rw-rw-   0        0        0     1094 2024-03-27 18:15:40.000000 thepipe_api-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0     9795 2024-04-17 06:24:03.977414 thepipe_api-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     9068 2024-04-16 05:29:43.000000 thepipe_api-0.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-17 06:24:03.978412 thepipe_api-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      859 2024-04-17 06:23:33.000000 thepipe_api-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:24:03.946419 thepipe_api-0.2.5/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-23 01:45:32.000000 thepipe_api-0.2.5/tests/__init__.py
+-rw-rw-rw-   0        0        0     9265 2024-04-16 16:00:52.000000 thepipe_api-0.2.5/tests/test_thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:24:03.950412 thepipe_api-0.2.5/thepipe_api/
+-rw-rw-rw-   0        0        0       86 2024-04-15 22:46:19.000000 thepipe_api-0.2.5/thepipe_api/__init__.py
+-rw-rw-rw-   0        0        0     4821 2024-04-13 20:40:22.000000 thepipe_api-0.2.5/thepipe_api/compressor.py
+-rw-rw-rw-   0        0        0     2778 2024-04-16 05:18:22.000000 thepipe_api-0.2.5/thepipe_api/core.py
+-rw-rw-rw-   0        0        0    20977 2024-04-17 06:23:20.000000 thepipe_api-0.2.5/thepipe_api/extractor.py
+-rw-rw-rw-   0        0        0     3649 2024-04-16 23:07:34.000000 thepipe_api-0.2.5/thepipe_api/thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:24:03.977414 thepipe_api-0.2.5/thepipe_api.egg-info/
+-rw-rw-rw-   0        0        0     9795 2024-04-17 06:24:03.000000 thepipe_api-0.2.5/thepipe_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-04-17 06:24:03.000000 thepipe_api-0.2.5/thepipe_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 06:24:03.000000 thepipe_api-0.2.5/thepipe_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-17 06:24:03.000000 thepipe_api-0.2.5/thepipe_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      104 2024-04-17 06:24:03.000000 thepipe_api-0.2.5/thepipe_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-17 06:24:03.000000 thepipe_api-0.2.5/thepipe_api.egg-info/top_level.txt
```

### Comparing `thepipe_api-0.2.4/LICENSE` & `thepipe_api-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.2.4/PKG-INFO` & `thepipe_api-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.2.4
+Version: 0.2.5
 Summary: Automate information extraction for multimodal LLMs.
 Home-page: https://github.com/emcf/thepipe
 Author: Emmett McFarlane
 Author-email: emmett@thepi.pe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.2.4 Summary: Automate
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.2.5 Summary: Automate
 information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
 thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
 python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
```

### Comparing `thepipe_api-0.2.4/README.md` & `thepipe_api-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.2.4/setup.py` & `thepipe_api-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='thepipe_api',
-    version='0.2.4',
+    version='0.2.5',
     author='Emmett McFarlane',
     author_email='emmett@thepi.pe',
     description='Automate information extraction for multimodal LLMs.',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/emcf/thepipe',
     packages=find_packages(),
```

### Comparing `thepipe_api-0.2.4/tests/test_thepipe.py` & `thepipe_api-0.2.5/tests/test_thepipe.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.2.4/thepipe_api/compressor.py` & `thepipe_api-0.2.5/thepipe_api/compressor.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.2.4/thepipe_api/core.py` & `thepipe_api-0.2.5/thepipe_api/core.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.2.4/thepipe_api/extractor.py` & `thepipe_api-0.2.5/thepipe_api/extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,19 +50,19 @@
             with open(file_path, 'rb') as f:
                 response = requests.post(
                     url=API_URL,
                     files={'file': (file_path, f)},
                     data={'api_key': THEPIPE_API_KEY, 'ai_extraction': ai_extraction, 'text_only': text_only}
                 )
         except Exception as e:
-            raise ValueError(f"Failed to extract from {file_path}. Exception: {e}.")
+            raise ValueError(f"Failed to extract from {file_path}. This may mean our backend couldn't handle this request. Exception: {e}.")
         try:
             response = response.json()
         except json.JSONDecodeError:
-            raise ValueError(f"Failed to extract from {file_path}. Response: {response}.")
+            raise ValueError(f"Failed to extract from {file_path}. This may mean our backend couldn't handle this request. Response: {response}.")
         if 'error' in response:
             raise ValueError(f"{response['error']}")
         chunks = create_chunks_from_messages(response['messages'])
         return chunks
     try:    
         if source_type == SourceTypes.PDF:
             extraction = extract_pdf(file_path=file_path, ai_extraction=ai_extraction, text_only=text_only, verbose=verbose)
@@ -250,15 +250,15 @@
                 data={'url': url, 'api_key': THEPIPE_API_KEY, 'text_only': text_only}
             )
         except Exception as e:
             raise ValueError(f"Failed to extract from URL. This may mean our backend couldn't handle this request. Exception: {e}.")
         try:
             response = response.json()
         except json.JSONDecodeError:
-            raise ValueError(f"Failed to extract from URL. Response: {response}.")
+            raise ValueError(f"Failed to extract from URL. This may mean our backend couldn't handle this request. Response: {response}.")
         if 'error' in response:
             raise ValueError(f"{response['error']}")
         chunks = create_chunks_from_messages(response['messages'])
         return chunks
     chunks = []
     _, extension = os.path.splitext(urlparse(url).path)
     if extension is not None and extension in KNOWN_EXTENSIONS:
```

### Comparing `thepipe_api-0.2.4/thepipe_api/thepipe.py` & `thepipe_api-0.2.5/thepipe_api/thepipe.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.2.4/thepipe_api.egg-info/PKG-INFO` & `thepipe_api-0.2.5/thepipe_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.2.4
+Version: 0.2.5
 Summary: Automate information extraction for multimodal LLMs.
 Home-page: https://github.com/emcf/thepipe
 Author: Emmett McFarlane
 Author-email: emmett@thepi.pe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.2.4 Summary: Automate
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.2.5 Summary: Automate
 information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
 thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
 python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
```

