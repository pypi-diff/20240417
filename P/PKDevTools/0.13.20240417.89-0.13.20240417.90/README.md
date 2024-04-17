# Comparing `tmp/PKDevTools-0.13.20240417.89.tar.gz` & `tmp/PKDevTools-0.13.20240417.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKDevTools-0.13.20240417.89.tar", last modified: Wed Apr 17 08:42:06 2024, max compression
+gzip compressed data, was "PKDevTools-0.13.20240417.90.tar", last modified: Wed Apr 17 12:33:00 2024, max compression
```

## Comparing `PKDevTools-0.13.20240417.89.tar` & `PKDevTools-0.13.20240417.90.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 08:42:06.584555 PKDevTools-0.13.20240417.89/
--rw-rw-rw-   0        0        0     1086 2024-04-17 08:40:11.000000 PKDevTools-0.13.20240417.89/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-17 08:42:06.568938 PKDevTools-0.13.20240417.89/PKDevTools/
--rw-rw-rw-   0        0        0     1176 2024-04-17 08:40:11.000000 PKDevTools-0.13.20240417.89/PKDevTools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 08:42:06.584555 PKDevTools-0.13.20240417.89/PKDevTools/classes/
--rw-rw-rw-   0        0        0     3402 2024-04-17 08:40:11.000000 PKDevTools-0.13.20240417.89/PKDevTools/classes/Archiver.py
--rw-rw-rw-   0        0        0     3985 2024-04-17 08:40:11.000000 PKDevTools-0.13.20240417.89/PKDevTools/classes/ColorText.py
--rw-rw-rw-   0        0        0     3599 2024-04-17 08:40:11.000000 PKDevTools-0.13.20240417.89/PKDevTools/classes/Committer.py
--rw-rw-rw-   0        0        0     6212 2024-04-17 08:40:11.000000 PKDevTools-0.13.20240417.89/PKDevTools/classes/CookieHelper.py
--rw-rw-rw-   0        0        0     8879 2024-04-17 08:40:11.000000 PKDevTools-0.13.20240417.89/PKDevTools/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11963 2024-04-17 08:40:11.000000 PKDevTools-0.13.20240417.89/PKDevTools/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    13778 2024-04-17 08:40:11.000000 PKDevTools-0.13.20240417.89/PKDevTools/classes/PKDateUtilities.py
--rw-rw-rw-   0        0        0     2988 2024-04-17 08:40:11.000000 PKDevTools-0.13.20240417.89/PKDevTools/classes/PKGitFolderDownloader.py
--rw-rw-rw-   0        0        0     8048 2024-04-17 08:40:11.000000 PKDevTools-0.13.20240417.89/PKDevTools/classes/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    14224 2024-04-17 08:40:11.000000 PKDevTools-0.13.20240417.89/PKDevTools/classes/PKPickler.py
--rw-rw-rw-   0        0        0     3433 2024-04-17 08:40:11.000000 PKDevTools-0.13.20240417.89/PKDevTools/classes/PKTimer.py
--rw-rw-rw-   0        0        0     4548 2024-04-17 08:40:11.000000 PKDevTools-0.13.20240417.89/PKDevTools/classes/Singleton.py
--rw-rw-rw-   0        0        0     1916 2024-04-17 08:40:11.000000 PKDevTools-0.13.20240417.89/PKDevTools/classes/SuppressOutput.py
--rw-rw-rw-   0        0        0    11216 2024-04-17 08:40:11.000000 PKDevTools-0.13.20240417.89/PKDevTools/classes/Telegram.py
--rw-rw-rw-   0        0        0    24543 2024-04-17 08:40:11.000000 PKDevTools-0.13.20240417.89/PKDevTools/classes/Utils.py
--rw-rw-rw-   0        0        0     9984 2024-04-17 08:40:11.000000 PKDevTools-0.13.20240417.89/PKDevTools/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       27 2024-04-17 08:42:00.000000 PKDevTools-0.13.20240417.89/PKDevTools/classes/__init__.py
--rw-rw-rw-   0        0        0     3738 2024-04-17 08:40:11.000000 PKDevTools-0.13.20240417.89/PKDevTools/classes/githubutilities.py
--rw-rw-rw-   0        0        0    16118 2024-04-17 08:40:11.000000 PKDevTools-0.13.20240417.89/PKDevTools/classes/log.py
--rw-rw-rw-   0        0        0     5384 2024-04-17 08:40:11.000000 PKDevTools-0.13.20240417.89/PKDevTools/classes/multiprocessing_logging.py
--rw-rw-rw-   0        0        0     2864 2024-04-17 08:40:11.000000 PKDevTools-0.13.20240417.89/PKDevTools/classes/squash.py
--rw-rw-rw-   0        0        0     4846 2024-04-17 08:40:11.000000 PKDevTools-0.13.20240417.89/PKDevTools/classes/updater.py
-drwxrwxrwx   0        0        0        0 2024-04-17 08:42:06.584555 PKDevTools-0.13.20240417.89/PKDevTools.egg-info/
--rw-rw-rw-   0        0        0     5202 2024-04-17 08:42:06.000000 PKDevTools-0.13.20240417.89/PKDevTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1047 2024-04-17 08:42:06.000000 PKDevTools-0.13.20240417.89/PKDevTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 08:42:06.000000 PKDevTools-0.13.20240417.89/PKDevTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      363 2024-04-17 08:42:06.000000 PKDevTools-0.13.20240417.89/PKDevTools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-17 08:41:59.000000 PKDevTools-0.13.20240417.89/PKDevTools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      158 2024-04-17 08:42:06.000000 PKDevTools-0.13.20240417.89/PKDevTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-17 08:42:06.000000 PKDevTools-0.13.20240417.89/PKDevTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5202 2024-04-17 08:42:06.584555 PKDevTools-0.13.20240417.89/PKG-INFO
--rw-rw-rw-   0        0        0     4290 2024-04-17 08:40:11.000000 PKDevTools-0.13.20240417.89/README.md
--rw-rw-rw-   0        0        0       86 2024-04-17 08:42:06.584555 PKDevTools-0.13.20240417.89/setup.cfg
--rw-rw-rw-   0        0        0     4341 2024-04-17 08:40:11.000000 PKDevTools-0.13.20240417.89/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:33:00.451700 PKDevTools-0.13.20240417.90/
+-rw-rw-rw-   0        0        0     1086 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-17 12:33:00.436073 PKDevTools-0.13.20240417.90/PKDevTools/
+-rw-rw-rw-   0        0        0     1176 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:33:00.451700 PKDevTools-0.13.20240417.90/PKDevTools/classes/
+-rw-rw-rw-   0        0        0     3402 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/Archiver.py
+-rw-rw-rw-   0        0        0     4831 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/ColorText.py
+-rw-rw-rw-   0        0        0     3599 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/Committer.py
+-rw-rw-rw-   0        0        0     6212 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/CookieHelper.py
+-rw-rw-rw-   0        0        0     8879 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11963 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    13778 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/PKDateUtilities.py
+-rw-rw-rw-   0        0        0     2988 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/PKGitFolderDownloader.py
+-rw-rw-rw-   0        0        0     8048 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    14224 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/PKPickler.py
+-rw-rw-rw-   0        0        0     3433 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/PKTimer.py
+-rw-rw-rw-   0        0        0     4548 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/Singleton.py
+-rw-rw-rw-   0        0        0     1916 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/SuppressOutput.py
+-rw-rw-rw-   0        0        0    11216 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/Telegram.py
+-rw-rw-rw-   0        0        0    24543 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/Utils.py
+-rw-rw-rw-   0        0        0     9984 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       27 2024-04-17 12:32:55.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/__init__.py
+-rw-rw-rw-   0        0        0     3738 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/githubutilities.py
+-rw-rw-rw-   0        0        0    16118 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/log.py
+-rw-rw-rw-   0        0        0     5384 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/multiprocessing_logging.py
+-rw-rw-rw-   0        0        0     2864 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/squash.py
+-rw-rw-rw-   0        0        0     4846 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/updater.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:33:00.436073 PKDevTools-0.13.20240417.90/PKDevTools.egg-info/
+-rw-rw-rw-   0        0        0     5202 2024-04-17 12:33:00.000000 PKDevTools-0.13.20240417.90/PKDevTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1047 2024-04-17 12:33:00.000000 PKDevTools-0.13.20240417.90/PKDevTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 12:33:00.000000 PKDevTools-0.13.20240417.90/PKDevTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      363 2024-04-17 12:33:00.000000 PKDevTools-0.13.20240417.90/PKDevTools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-17 12:32:54.000000 PKDevTools-0.13.20240417.90/PKDevTools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      158 2024-04-17 12:33:00.000000 PKDevTools-0.13.20240417.90/PKDevTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-17 12:33:00.000000 PKDevTools-0.13.20240417.90/PKDevTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5202 2024-04-17 12:33:00.451700 PKDevTools-0.13.20240417.90/PKG-INFO
+-rw-rw-rw-   0        0        0     4290 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-17 12:33:00.451700 PKDevTools-0.13.20240417.90/setup.cfg
+-rw-rw-rw-   0        0        0     4341 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/setup.py
```

### Comparing `PKDevTools-0.13.20240417.89/LICENSE` & `PKDevTools-0.13.20240417.90/LICENSE`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.89/PKDevTools/__init__.py` & `PKDevTools-0.13.20240417.90/PKDevTools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.89/PKDevTools/classes/Archiver.py` & `PKDevTools-0.13.20240417.90/PKDevTools/classes/Archiver.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.89/PKDevTools/classes/Committer.py` & `PKDevTools-0.13.20240417.90/PKDevTools/classes/Committer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.89/PKDevTools/classes/CookieHelper.py` & `PKDevTools-0.13.20240417.90/PKDevTools/classes/CookieHelper.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.89/PKDevTools/classes/Fetcher.py` & `PKDevTools-0.13.20240417.90/PKDevTools/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.89/PKDevTools/classes/MenuOptions.py` & `PKDevTools-0.13.20240417.90/PKDevTools/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.89/PKDevTools/classes/PKDateUtilities.py` & `PKDevTools-0.13.20240417.90/PKDevTools/classes/PKDateUtilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.89/PKDevTools/classes/PKGitFolderDownloader.py` & `PKDevTools-0.13.20240417.90/PKDevTools/classes/PKGitFolderDownloader.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.89/PKDevTools/classes/PKMultiProcessorClient.py` & `PKDevTools-0.13.20240417.90/PKDevTools/classes/PKMultiProcessorClient.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.89/PKDevTools/classes/PKPickler.py` & `PKDevTools-0.13.20240417.90/PKDevTools/classes/PKPickler.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.89/PKDevTools/classes/PKTimer.py` & `PKDevTools-0.13.20240417.90/PKDevTools/classes/PKTimer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.89/PKDevTools/classes/Singleton.py` & `PKDevTools-0.13.20240417.90/PKDevTools/classes/Singleton.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.89/PKDevTools/classes/SuppressOutput.py` & `PKDevTools-0.13.20240417.90/PKDevTools/classes/SuppressOutput.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.89/PKDevTools/classes/Telegram.py` & `PKDevTools-0.13.20240417.90/PKDevTools/classes/Telegram.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.89/PKDevTools/classes/Utils.py` & `PKDevTools-0.13.20240417.90/PKDevTools/classes/Utils.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.89/PKDevTools/classes/WorkflowManager.py` & `PKDevTools-0.13.20240417.90/PKDevTools/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.89/PKDevTools/classes/githubutilities.py` & `PKDevTools-0.13.20240417.90/PKDevTools/classes/githubutilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.89/PKDevTools/classes/log.py` & `PKDevTools-0.13.20240417.90/PKDevTools/classes/log.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.89/PKDevTools/classes/multiprocessing_logging.py` & `PKDevTools-0.13.20240417.90/PKDevTools/classes/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.89/PKDevTools/classes/squash.py` & `PKDevTools-0.13.20240417.90/PKDevTools/classes/squash.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.89/PKDevTools/classes/updater.py` & `PKDevTools-0.13.20240417.90/PKDevTools/classes/updater.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.89/PKDevTools.egg-info/PKG-INFO` & `PKDevTools-0.13.20240417.90/PKDevTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240417.89
+Version: 0.13.20240417.90
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240417.89.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240417.90.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240417.89/PKDevTools.egg-info/SOURCES.txt` & `PKDevTools-0.13.20240417.90/PKDevTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.89/PKG-INFO` & `PKDevTools-0.13.20240417.90/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240417.89
+Version: 0.13.20240417.90
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240417.89.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240417.90.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240417.89/README.md` & `PKDevTools-0.13.20240417.90/README.md`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.89/setup.py` & `PKDevTools-0.13.20240417.90/setup.py`

 * *Files identical despite different names*

