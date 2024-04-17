# Comparing `tmp/PKDevTools-0.13.20240416.86.tar.gz` & `tmp/PKDevTools-0.13.20240416.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKDevTools-0.13.20240416.86.tar", last modified: Tue Apr 16 18:32:49 2024, max compression
+gzip compressed data, was "PKDevTools-0.13.20240416.87.tar", last modified: Tue Apr 16 18:46:20 2024, max compression
```

## Comparing `PKDevTools-0.13.20240416.86.tar` & `PKDevTools-0.13.20240416.87.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 18:32:49.042412 PKDevTools-0.13.20240416.86/
--rw-rw-rw-   0        0        0     1086 2024-04-16 18:31:28.000000 PKDevTools-0.13.20240416.86/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-16 18:32:49.026794 PKDevTools-0.13.20240416.86/PKDevTools/
--rw-rw-rw-   0        0        0     1176 2024-04-16 18:31:28.000000 PKDevTools-0.13.20240416.86/PKDevTools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 18:32:49.042412 PKDevTools-0.13.20240416.86/PKDevTools/classes/
--rw-rw-rw-   0        0        0     3402 2024-04-16 18:31:28.000000 PKDevTools-0.13.20240416.86/PKDevTools/classes/Archiver.py
--rw-rw-rw-   0        0        0     3985 2024-04-16 18:31:28.000000 PKDevTools-0.13.20240416.86/PKDevTools/classes/ColorText.py
--rw-rw-rw-   0        0        0     3599 2024-04-16 18:31:28.000000 PKDevTools-0.13.20240416.86/PKDevTools/classes/Committer.py
--rw-rw-rw-   0        0        0     6212 2024-04-16 18:31:28.000000 PKDevTools-0.13.20240416.86/PKDevTools/classes/CookieHelper.py
--rw-rw-rw-   0        0        0     8879 2024-04-16 18:31:28.000000 PKDevTools-0.13.20240416.86/PKDevTools/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11963 2024-04-16 18:31:28.000000 PKDevTools-0.13.20240416.86/PKDevTools/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    12789 2024-04-16 18:31:28.000000 PKDevTools-0.13.20240416.86/PKDevTools/classes/PKDateUtilities.py
--rw-rw-rw-   0        0        0     2988 2024-04-16 18:31:28.000000 PKDevTools-0.13.20240416.86/PKDevTools/classes/PKGitFolderDownloader.py
--rw-rw-rw-   0        0        0     8048 2024-04-16 18:31:28.000000 PKDevTools-0.13.20240416.86/PKDevTools/classes/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    14224 2024-04-16 18:31:28.000000 PKDevTools-0.13.20240416.86/PKDevTools/classes/PKPickler.py
--rw-rw-rw-   0        0        0     3433 2024-04-16 18:31:28.000000 PKDevTools-0.13.20240416.86/PKDevTools/classes/PKTimer.py
--rw-rw-rw-   0        0        0     4548 2024-04-16 18:31:28.000000 PKDevTools-0.13.20240416.86/PKDevTools/classes/Singleton.py
--rw-rw-rw-   0        0        0     1916 2024-04-16 18:31:28.000000 PKDevTools-0.13.20240416.86/PKDevTools/classes/SuppressOutput.py
--rw-rw-rw-   0        0        0    11216 2024-04-16 18:31:28.000000 PKDevTools-0.13.20240416.86/PKDevTools/classes/Telegram.py
--rw-rw-rw-   0        0        0    24543 2024-04-16 18:31:28.000000 PKDevTools-0.13.20240416.86/PKDevTools/classes/Utils.py
--rw-rw-rw-   0        0        0     9984 2024-04-16 18:31:28.000000 PKDevTools-0.13.20240416.86/PKDevTools/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       27 2024-04-16 18:32:44.000000 PKDevTools-0.13.20240416.86/PKDevTools/classes/__init__.py
--rw-rw-rw-   0        0        0     3738 2024-04-16 18:31:28.000000 PKDevTools-0.13.20240416.86/PKDevTools/classes/githubutilities.py
--rw-rw-rw-   0        0        0    16118 2024-04-16 18:31:28.000000 PKDevTools-0.13.20240416.86/PKDevTools/classes/log.py
--rw-rw-rw-   0        0        0     5384 2024-04-16 18:31:28.000000 PKDevTools-0.13.20240416.86/PKDevTools/classes/multiprocessing_logging.py
--rw-rw-rw-   0        0        0     2864 2024-04-16 18:31:28.000000 PKDevTools-0.13.20240416.86/PKDevTools/classes/squash.py
--rw-rw-rw-   0        0        0     4846 2024-04-16 18:31:28.000000 PKDevTools-0.13.20240416.86/PKDevTools/classes/updater.py
-drwxrwxrwx   0        0        0        0 2024-04-16 18:32:49.026794 PKDevTools-0.13.20240416.86/PKDevTools.egg-info/
--rw-rw-rw-   0        0        0     5202 2024-04-16 18:32:48.000000 PKDevTools-0.13.20240416.86/PKDevTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1047 2024-04-16 18:32:48.000000 PKDevTools-0.13.20240416.86/PKDevTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 18:32:48.000000 PKDevTools-0.13.20240416.86/PKDevTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      363 2024-04-16 18:32:48.000000 PKDevTools-0.13.20240416.86/PKDevTools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 18:32:43.000000 PKDevTools-0.13.20240416.86/PKDevTools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      158 2024-04-16 18:32:48.000000 PKDevTools-0.13.20240416.86/PKDevTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-16 18:32:48.000000 PKDevTools-0.13.20240416.86/PKDevTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5202 2024-04-16 18:32:49.042412 PKDevTools-0.13.20240416.86/PKG-INFO
--rw-rw-rw-   0        0        0     4290 2024-04-16 18:31:28.000000 PKDevTools-0.13.20240416.86/README.md
--rw-rw-rw-   0        0        0       86 2024-04-16 18:32:49.042412 PKDevTools-0.13.20240416.86/setup.cfg
--rw-rw-rw-   0        0        0     4341 2024-04-16 18:31:28.000000 PKDevTools-0.13.20240416.86/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 18:46:20.514654 PKDevTools-0.13.20240416.87/
+-rw-rw-rw-   0        0        0     1086 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-16 18:46:20.499032 PKDevTools-0.13.20240416.87/PKDevTools/
+-rw-rw-rw-   0        0        0     1176 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 18:46:20.514654 PKDevTools-0.13.20240416.87/PKDevTools/classes/
+-rw-rw-rw-   0        0        0     3402 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/Archiver.py
+-rw-rw-rw-   0        0        0     3985 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/ColorText.py
+-rw-rw-rw-   0        0        0     3599 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/Committer.py
+-rw-rw-rw-   0        0        0     6212 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/CookieHelper.py
+-rw-rw-rw-   0        0        0     8879 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11963 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    13139 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/PKDateUtilities.py
+-rw-rw-rw-   0        0        0     2988 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/PKGitFolderDownloader.py
+-rw-rw-rw-   0        0        0     8048 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    14224 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/PKPickler.py
+-rw-rw-rw-   0        0        0     3433 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/PKTimer.py
+-rw-rw-rw-   0        0        0     4548 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/Singleton.py
+-rw-rw-rw-   0        0        0     1916 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/SuppressOutput.py
+-rw-rw-rw-   0        0        0    11216 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/Telegram.py
+-rw-rw-rw-   0        0        0    24543 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/Utils.py
+-rw-rw-rw-   0        0        0     9984 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       27 2024-04-16 18:46:16.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/__init__.py
+-rw-rw-rw-   0        0        0     3738 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/githubutilities.py
+-rw-rw-rw-   0        0        0    16118 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/log.py
+-rw-rw-rw-   0        0        0     5384 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/multiprocessing_logging.py
+-rw-rw-rw-   0        0        0     2864 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/squash.py
+-rw-rw-rw-   0        0        0     4846 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/updater.py
+drwxrwxrwx   0        0        0        0 2024-04-16 18:46:20.514654 PKDevTools-0.13.20240416.87/PKDevTools.egg-info/
+-rw-rw-rw-   0        0        0     5202 2024-04-16 18:46:20.000000 PKDevTools-0.13.20240416.87/PKDevTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1047 2024-04-16 18:46:20.000000 PKDevTools-0.13.20240416.87/PKDevTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 18:46:20.000000 PKDevTools-0.13.20240416.87/PKDevTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      363 2024-04-16 18:46:20.000000 PKDevTools-0.13.20240416.87/PKDevTools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 18:46:14.000000 PKDevTools-0.13.20240416.87/PKDevTools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      158 2024-04-16 18:46:20.000000 PKDevTools-0.13.20240416.87/PKDevTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-16 18:46:20.000000 PKDevTools-0.13.20240416.87/PKDevTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5202 2024-04-16 18:46:20.514654 PKDevTools-0.13.20240416.87/PKG-INFO
+-rw-rw-rw-   0        0        0     4290 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-16 18:46:20.514654 PKDevTools-0.13.20240416.87/setup.cfg
+-rw-rw-rw-   0        0        0     4341 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/setup.py
```

### Comparing `PKDevTools-0.13.20240416.86/LICENSE` & `PKDevTools-0.13.20240416.87/LICENSE`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.86/PKDevTools/__init__.py` & `PKDevTools-0.13.20240416.87/PKDevTools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.86/PKDevTools/classes/Archiver.py` & `PKDevTools-0.13.20240416.87/PKDevTools/classes/Archiver.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.86/PKDevTools/classes/ColorText.py` & `PKDevTools-0.13.20240416.87/PKDevTools/classes/ColorText.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.86/PKDevTools/classes/Committer.py` & `PKDevTools-0.13.20240416.87/PKDevTools/classes/Committer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.86/PKDevTools/classes/CookieHelper.py` & `PKDevTools-0.13.20240416.87/PKDevTools/classes/CookieHelper.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.86/PKDevTools/classes/Fetcher.py` & `PKDevTools-0.13.20240416.87/PKDevTools/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.86/PKDevTools/classes/MenuOptions.py` & `PKDevTools-0.13.20240416.87/PKDevTools/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.86/PKDevTools/classes/PKDateUtilities.py` & `PKDevTools-0.13.20240416.87/PKDevTools/classes/PKDateUtilities.py`

 * *Files 5% similar despite different names*

```diff
@@ -153,14 +153,22 @@
         return (openTime <= curr <= closeTime) and PKDateUtilities.isTradingWeekday()
 
     def isTradingWeekday(checkDate=None):
         if checkDate is None:
             checkDate = PKDateUtilities.currentDateTime()
         return 0 <= checkDate.weekday() <= 4
 
+    def nextWeekday(forDate=None):
+        if forDate is None:
+            forDate = PKDateUtilities.currentDateTime()
+        nextWeekday = forDate + datetime.timedelta(days=1)
+        while not PKDateUtilities.isTradingWeekday(nextWeekday):
+            nextWeekday = nextWeekday + datetime.timedelta(days=1)
+        return nextWeekday
+    
     def ispreMarketTime():
         curr = PKDateUtilities.currentDateTime()
         openTime = curr.replace(hour=9, minute=15)
         return (openTime > curr) and PKDateUtilities.isTradingWeekday()
 
     def ispostMarketTime():
         curr = PKDateUtilities.currentDateTime()
```

### Comparing `PKDevTools-0.13.20240416.86/PKDevTools/classes/PKGitFolderDownloader.py` & `PKDevTools-0.13.20240416.87/PKDevTools/classes/PKGitFolderDownloader.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.86/PKDevTools/classes/PKMultiProcessorClient.py` & `PKDevTools-0.13.20240416.87/PKDevTools/classes/PKMultiProcessorClient.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.86/PKDevTools/classes/PKPickler.py` & `PKDevTools-0.13.20240416.87/PKDevTools/classes/PKPickler.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.86/PKDevTools/classes/PKTimer.py` & `PKDevTools-0.13.20240416.87/PKDevTools/classes/PKTimer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.86/PKDevTools/classes/Singleton.py` & `PKDevTools-0.13.20240416.87/PKDevTools/classes/Singleton.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.86/PKDevTools/classes/SuppressOutput.py` & `PKDevTools-0.13.20240416.87/PKDevTools/classes/SuppressOutput.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.86/PKDevTools/classes/Telegram.py` & `PKDevTools-0.13.20240416.87/PKDevTools/classes/Telegram.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.86/PKDevTools/classes/Utils.py` & `PKDevTools-0.13.20240416.87/PKDevTools/classes/Utils.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.86/PKDevTools/classes/WorkflowManager.py` & `PKDevTools-0.13.20240416.87/PKDevTools/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.86/PKDevTools/classes/githubutilities.py` & `PKDevTools-0.13.20240416.87/PKDevTools/classes/githubutilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.86/PKDevTools/classes/log.py` & `PKDevTools-0.13.20240416.87/PKDevTools/classes/log.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.86/PKDevTools/classes/multiprocessing_logging.py` & `PKDevTools-0.13.20240416.87/PKDevTools/classes/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.86/PKDevTools/classes/squash.py` & `PKDevTools-0.13.20240416.87/PKDevTools/classes/squash.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.86/PKDevTools/classes/updater.py` & `PKDevTools-0.13.20240416.87/PKDevTools/classes/updater.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.86/PKDevTools.egg-info/PKG-INFO` & `PKDevTools-0.13.20240416.87/PKDevTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240416.86
+Version: 0.13.20240416.87
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240416.86.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240416.87.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240416.86/PKDevTools.egg-info/SOURCES.txt` & `PKDevTools-0.13.20240416.87/PKDevTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.86/PKG-INFO` & `PKDevTools-0.13.20240416.87/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240416.86
+Version: 0.13.20240416.87
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240416.86.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240416.87.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240416.86/README.md` & `PKDevTools-0.13.20240416.87/README.md`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.86/setup.py` & `PKDevTools-0.13.20240416.87/setup.py`

 * *Files identical despite different names*

