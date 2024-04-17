# Comparing `tmp/thepipe_api-0.2.2.tar.gz` & `tmp/thepipe_api-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thepipe_api-0.2.2.tar", last modified: Tue Apr 16 18:08:40 2024, max compression
+gzip compressed data, was "thepipe_api-0.2.3.tar", last modified: Tue Apr 16 23:08:45 2024, max compression
```

## Comparing `thepipe_api-0.2.2.tar` & `thepipe_api-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 18:08:40.765298 thepipe_api-0.2.2/
--rw-rw-rw-   0        0        0     1094 2024-03-27 18:15:40.000000 thepipe_api-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     9795 2024-04-16 18:08:40.764298 thepipe_api-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     9068 2024-04-16 05:29:43.000000 thepipe_api-0.2.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-16 18:08:40.766298 thepipe_api-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      859 2024-04-16 18:08:14.000000 thepipe_api-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 18:08:40.733785 thepipe_api-0.2.2/tests/
--rw-rw-rw-   0        0        0        0 2024-03-23 01:45:32.000000 thepipe_api-0.2.2/tests/__init__.py
--rw-rw-rw-   0        0        0     9265 2024-04-16 16:00:52.000000 thepipe_api-0.2.2/tests/test_thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-16 18:08:40.737785 thepipe_api-0.2.2/thepipe_api/
--rw-rw-rw-   0        0        0       86 2024-04-15 22:46:19.000000 thepipe_api-0.2.2/thepipe_api/__init__.py
--rw-rw-rw-   0        0        0     4821 2024-04-13 20:40:22.000000 thepipe_api-0.2.2/thepipe_api/compressor.py
--rw-rw-rw-   0        0        0     2778 2024-04-16 05:18:22.000000 thepipe_api-0.2.2/thepipe_api/core.py
--rw-rw-rw-   0        0        0    19869 2024-04-16 18:07:02.000000 thepipe_api-0.2.2/thepipe_api/extractor.py
--rw-rw-rw-   0        0        0     3649 2024-04-16 05:20:42.000000 thepipe_api-0.2.2/thepipe_api/thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-16 18:08:40.764298 thepipe_api-0.2.2/thepipe_api.egg-info/
--rw-rw-rw-   0        0        0     9795 2024-04-16 18:08:40.000000 thepipe_api-0.2.2/thepipe_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2024-04-16 18:08:40.000000 thepipe_api-0.2.2/thepipe_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 18:08:40.000000 thepipe_api-0.2.2/thepipe_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-16 18:08:40.000000 thepipe_api-0.2.2/thepipe_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      104 2024-04-16 18:08:40.000000 thepipe_api-0.2.2/thepipe_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-16 18:08:40.000000 thepipe_api-0.2.2/thepipe_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 23:08:45.698692 thepipe_api-0.2.3/
+-rw-rw-rw-   0        0        0     1094 2024-03-27 18:15:40.000000 thepipe_api-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     9795 2024-04-16 23:08:45.696691 thepipe_api-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9068 2024-04-16 05:29:43.000000 thepipe_api-0.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-16 23:08:45.698692 thepipe_api-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      859 2024-04-16 23:03:54.000000 thepipe_api-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 23:08:45.668691 thepipe_api-0.2.3/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-23 01:45:32.000000 thepipe_api-0.2.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     9265 2024-04-16 16:00:52.000000 thepipe_api-0.2.3/tests/test_thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-16 23:08:45.672691 thepipe_api-0.2.3/thepipe_api/
+-rw-rw-rw-   0        0        0       86 2024-04-15 22:46:19.000000 thepipe_api-0.2.3/thepipe_api/__init__.py
+-rw-rw-rw-   0        0        0     4821 2024-04-13 20:40:22.000000 thepipe_api-0.2.3/thepipe_api/compressor.py
+-rw-rw-rw-   0        0        0     2778 2024-04-16 05:18:22.000000 thepipe_api-0.2.3/thepipe_api/core.py
+-rw-rw-rw-   0        0        0    19915 2024-04-16 23:07:59.000000 thepipe_api-0.2.3/thepipe_api/extractor.py
+-rw-rw-rw-   0        0        0     3649 2024-04-16 23:07:34.000000 thepipe_api-0.2.3/thepipe_api/thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-16 23:08:45.695780 thepipe_api-0.2.3/thepipe_api.egg-info/
+-rw-rw-rw-   0        0        0     9795 2024-04-16 23:08:45.000000 thepipe_api-0.2.3/thepipe_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-04-16 23:08:45.000000 thepipe_api-0.2.3/thepipe_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 23:08:45.000000 thepipe_api-0.2.3/thepipe_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-16 23:08:45.000000 thepipe_api-0.2.3/thepipe_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      104 2024-04-16 23:08:45.000000 thepipe_api-0.2.3/thepipe_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-16 23:08:45.000000 thepipe_api-0.2.3/thepipe_api.egg-info/top_level.txt
```

### Comparing `thepipe_api-0.2.2/LICENSE` & `thepipe_api-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.2.2/PKG-INFO` & `thepipe_api-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.2.2
+Version: 0.2.3
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
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.2.2 Summary: Automate
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.2.3 Summary: Automate
 information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
 thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
 python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
```

### Comparing `thepipe_api-0.2.2/README.md` & `thepipe_api-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.2.2/setup.py` & `thepipe_api-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='thepipe_api',
-    version='0.2.2',
+    version='0.2.3',
     author='Emmett McFarlane',
     author_email='emmett@thepi.pe',
     description='Automate information extraction for multimodal LLMs.',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/emcf/thepipe',
     packages=find_packages(),
```

### Comparing `thepipe_api-0.2.2/tests/test_thepipe.py` & `thepipe_api-0.2.3/tests/test_thepipe.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.2.2/thepipe_api/compressor.py` & `thepipe_api-0.2.3/thepipe_api/compressor.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.2.2/thepipe_api/core.py` & `thepipe_api-0.2.3/thepipe_api/core.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.2.2/thepipe_api/extractor.py` & `thepipe_api-0.2.3/thepipe_api/extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     source_type = detect_type(source)
     if source_type is None:
         raise ValueError(f"Could not detect source type for {source}.")
     if verbose: print_status(f"Extracting from {source_type.value}", status='info')
     if source_type == SourceTypes.DIR or source == '.' or source == './':
         if source == '.' or source == './':
             source = os.getcwd()
-        return extract_from_directory(dir_path=source, match=match, ignore=ignore, verbose=verbose, ai_extraction=ai_extraction, text_only=text_only, limit=limit)
+        return extract_from_directory(dir_path=source, match=match, ignore=ignore, verbose=verbose, ai_extraction=ai_extraction, text_only=text_only, limit=limit, local=local)
     elif source_type == SourceTypes.GITHUB:
         return extract_github(github_url=source, file_path='', match=match, ignore=ignore, text_only=text_only, verbose=verbose, ai_extraction=ai_extraction, branch='master')
     elif source_type == SourceTypes.URL:
         return extract_url(url=source, text_only=text_only, local=local)
     elif source_type == SourceTypes.ZIP:
         return extract_zip(file_path=source, match=match, ignore=ignore, verbose=verbose, ai_extraction=ai_extraction, text_only=text_only)
     return extract_from_file(file_path=source, source_type=source_type, verbose=verbose, ai_extraction=ai_extraction, text_only=text_only, local=local)
@@ -144,21 +144,21 @@
         return True
     if any(x in file_path for x in ['node_modules', 'venv', '.git', '.vscode', '__pycache__']):
         return True
     if not os.path.isfile(file_path):
         return True
     return False
 
-def extract_from_directory(dir_path: str, match: Optional[str] = None, ignore: Optional[str] = None, verbose: bool = False, ai_extraction: bool = False, text_only: bool = False, limit: int = None) -> List[Chunk]:
+def extract_from_directory(dir_path: str, match: Optional[str] = None, ignore: Optional[str] = None, verbose: bool = False, ai_extraction: bool = False, text_only: bool = False, limit: int = None, local: bool = True) -> List[Chunk]:
     all_files = glob.glob(dir_path + "/**/*", recursive=True)
     matched_files = [file for file in all_files if re.search(match, file, re.IGNORECASE)] if match else all_files
     file_paths = [file for file in matched_files if not should_ignore(file, ignore)]
     contents = []
     with ThreadPoolExecutor() as executor:
-        results = executor.map(lambda file_path: extract_from_source(source=file_path, match=match, ignore=ignore, verbose=verbose, ai_extraction=ai_extraction, text_only=text_only, limit=limit), file_paths)
+        results = executor.map(lambda file_path: extract_from_source(source=file_path, match=match, ignore=ignore, verbose=verbose, ai_extraction=ai_extraction, text_only=text_only, limit=limit, local=local), file_paths)
         for result in results:
             contents += result
     return contents
 
 def extract_zip(file_path: str, match: Optional[str] = None, ignore: Optional[str] = None, verbose: bool = False, ai_extraction: bool = False, text_only: bool = False) -> List[Chunk]:
     extracted_files = []
     with tempfile.TemporaryDirectory() as temp_dir:
```

### Comparing `thepipe_api-0.2.2/thepipe_api/thepipe.py` & `thepipe_api-0.2.3/thepipe_api/thepipe.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.2.2/thepipe_api.egg-info/PKG-INFO` & `thepipe_api-0.2.3/thepipe_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.2.2
+Version: 0.2.3
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
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.2.2 Summary: Automate
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.2.3 Summary: Automate
 information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
 thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
 python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
```

