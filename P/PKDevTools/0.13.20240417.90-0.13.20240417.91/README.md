# Comparing `tmp/PKDevTools-0.13.20240417.90.tar.gz` & `tmp/PKDevTools-0.13.20240417.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKDevTools-0.13.20240417.90.tar", last modified: Wed Apr 17 12:33:00 2024, max compression
+gzip compressed data, was "PKDevTools-0.13.20240417.91.tar", last modified: Wed Apr 17 21:28:23 2024, max compression
```

## Comparing `PKDevTools-0.13.20240417.90.tar` & `PKDevTools-0.13.20240417.91.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 12:33:00.451700 PKDevTools-0.13.20240417.90/
--rw-rw-rw-   0        0        0     1086 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-17 12:33:00.436073 PKDevTools-0.13.20240417.90/PKDevTools/
--rw-rw-rw-   0        0        0     1176 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 12:33:00.451700 PKDevTools-0.13.20240417.90/PKDevTools/classes/
--rw-rw-rw-   0        0        0     3402 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/Archiver.py
--rw-rw-rw-   0        0        0     4831 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/ColorText.py
--rw-rw-rw-   0        0        0     3599 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/Committer.py
--rw-rw-rw-   0        0        0     6212 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/CookieHelper.py
--rw-rw-rw-   0        0        0     8879 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11963 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    13778 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/PKDateUtilities.py
--rw-rw-rw-   0        0        0     2988 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/PKGitFolderDownloader.py
--rw-rw-rw-   0        0        0     8048 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    14224 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/PKPickler.py
--rw-rw-rw-   0        0        0     3433 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/PKTimer.py
--rw-rw-rw-   0        0        0     4548 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/Singleton.py
--rw-rw-rw-   0        0        0     1916 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/SuppressOutput.py
--rw-rw-rw-   0        0        0    11216 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/Telegram.py
--rw-rw-rw-   0        0        0    24543 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/Utils.py
--rw-rw-rw-   0        0        0     9984 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       27 2024-04-17 12:32:55.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/__init__.py
--rw-rw-rw-   0        0        0     3738 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/githubutilities.py
--rw-rw-rw-   0        0        0    16118 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/log.py
--rw-rw-rw-   0        0        0     5384 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/multiprocessing_logging.py
--rw-rw-rw-   0        0        0     2864 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/squash.py
--rw-rw-rw-   0        0        0     4846 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/PKDevTools/classes/updater.py
-drwxrwxrwx   0        0        0        0 2024-04-17 12:33:00.436073 PKDevTools-0.13.20240417.90/PKDevTools.egg-info/
--rw-rw-rw-   0        0        0     5202 2024-04-17 12:33:00.000000 PKDevTools-0.13.20240417.90/PKDevTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1047 2024-04-17 12:33:00.000000 PKDevTools-0.13.20240417.90/PKDevTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 12:33:00.000000 PKDevTools-0.13.20240417.90/PKDevTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      363 2024-04-17 12:33:00.000000 PKDevTools-0.13.20240417.90/PKDevTools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-17 12:32:54.000000 PKDevTools-0.13.20240417.90/PKDevTools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      158 2024-04-17 12:33:00.000000 PKDevTools-0.13.20240417.90/PKDevTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-17 12:33:00.000000 PKDevTools-0.13.20240417.90/PKDevTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5202 2024-04-17 12:33:00.451700 PKDevTools-0.13.20240417.90/PKG-INFO
--rw-rw-rw-   0        0        0     4290 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/README.md
--rw-rw-rw-   0        0        0       86 2024-04-17 12:33:00.451700 PKDevTools-0.13.20240417.90/setup.cfg
--rw-rw-rw-   0        0        0     4341 2024-04-17 12:31:06.000000 PKDevTools-0.13.20240417.90/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 21:28:23.963895 PKDevTools-0.13.20240417.91/
+-rw-rw-rw-   0        0        0     1086 2024-04-17 21:27:11.000000 PKDevTools-0.13.20240417.91/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-17 21:28:23.948271 PKDevTools-0.13.20240417.91/PKDevTools/
+-rw-rw-rw-   0        0        0     1176 2024-04-17 21:27:11.000000 PKDevTools-0.13.20240417.91/PKDevTools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 21:28:23.963895 PKDevTools-0.13.20240417.91/PKDevTools/classes/
+-rw-rw-rw-   0        0        0     3402 2024-04-17 21:27:11.000000 PKDevTools-0.13.20240417.91/PKDevTools/classes/Archiver.py
+-rw-rw-rw-   0        0        0     4831 2024-04-17 21:27:11.000000 PKDevTools-0.13.20240417.91/PKDevTools/classes/ColorText.py
+-rw-rw-rw-   0        0        0     3599 2024-04-17 21:27:11.000000 PKDevTools-0.13.20240417.91/PKDevTools/classes/Committer.py
+-rw-rw-rw-   0        0        0     6212 2024-04-17 21:27:11.000000 PKDevTools-0.13.20240417.91/PKDevTools/classes/CookieHelper.py
+-rw-rw-rw-   0        0        0     8879 2024-04-17 21:27:11.000000 PKDevTools-0.13.20240417.91/PKDevTools/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11963 2024-04-17 21:27:11.000000 PKDevTools-0.13.20240417.91/PKDevTools/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0     2315 2024-04-17 21:27:11.000000 PKDevTools-0.13.20240417.91/PKDevTools/classes/OutputControls.py
+-rw-rw-rw-   0        0        0    13778 2024-04-17 21:27:11.000000 PKDevTools-0.13.20240417.91/PKDevTools/classes/PKDateUtilities.py
+-rw-rw-rw-   0        0        0     2988 2024-04-17 21:27:11.000000 PKDevTools-0.13.20240417.91/PKDevTools/classes/PKGitFolderDownloader.py
+-rw-rw-rw-   0        0        0     8048 2024-04-17 21:27:11.000000 PKDevTools-0.13.20240417.91/PKDevTools/classes/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    14332 2024-04-17 21:27:11.000000 PKDevTools-0.13.20240417.91/PKDevTools/classes/PKPickler.py
+-rw-rw-rw-   0        0        0     3433 2024-04-17 21:27:11.000000 PKDevTools-0.13.20240417.91/PKDevTools/classes/PKTimer.py
+-rw-rw-rw-   0        0        0     4548 2024-04-17 21:27:11.000000 PKDevTools-0.13.20240417.91/PKDevTools/classes/Singleton.py
+-rw-rw-rw-   0        0        0     1916 2024-04-17 21:27:11.000000 PKDevTools-0.13.20240417.91/PKDevTools/classes/SuppressOutput.py
+-rw-rw-rw-   0        0        0    11301 2024-04-17 21:27:11.000000 PKDevTools-0.13.20240417.91/PKDevTools/classes/Telegram.py
+-rw-rw-rw-   0        0        0    24543 2024-04-17 21:27:11.000000 PKDevTools-0.13.20240417.91/PKDevTools/classes/Utils.py
+-rw-rw-rw-   0        0        0     9984 2024-04-17 21:27:11.000000 PKDevTools-0.13.20240417.91/PKDevTools/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       27 2024-04-17 21:28:18.000000 PKDevTools-0.13.20240417.91/PKDevTools/classes/__init__.py
+-rw-rw-rw-   0        0        0     3738 2024-04-17 21:27:11.000000 PKDevTools-0.13.20240417.91/PKDevTools/classes/githubutilities.py
+-rw-rw-rw-   0        0        0    16118 2024-04-17 21:27:11.000000 PKDevTools-0.13.20240417.91/PKDevTools/classes/log.py
+-rw-rw-rw-   0        0        0     5384 2024-04-17 21:27:11.000000 PKDevTools-0.13.20240417.91/PKDevTools/classes/multiprocessing_logging.py
+-rw-rw-rw-   0        0        0     2864 2024-04-17 21:27:11.000000 PKDevTools-0.13.20240417.91/PKDevTools/classes/squash.py
+-rw-rw-rw-   0        0        0     4846 2024-04-17 21:27:11.000000 PKDevTools-0.13.20240417.91/PKDevTools/classes/updater.py
+drwxrwxrwx   0        0        0        0 2024-04-17 21:28:23.948271 PKDevTools-0.13.20240417.91/PKDevTools.egg-info/
+-rw-rw-rw-   0        0        0     5202 2024-04-17 21:28:23.000000 PKDevTools-0.13.20240417.91/PKDevTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1084 2024-04-17 21:28:23.000000 PKDevTools-0.13.20240417.91/PKDevTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 21:28:23.000000 PKDevTools-0.13.20240417.91/PKDevTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      363 2024-04-17 21:28:23.000000 PKDevTools-0.13.20240417.91/PKDevTools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-17 21:28:17.000000 PKDevTools-0.13.20240417.91/PKDevTools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      158 2024-04-17 21:28:23.000000 PKDevTools-0.13.20240417.91/PKDevTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-17 21:28:23.000000 PKDevTools-0.13.20240417.91/PKDevTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5202 2024-04-17 21:28:23.963895 PKDevTools-0.13.20240417.91/PKG-INFO
+-rw-rw-rw-   0        0        0     4290 2024-04-17 21:27:11.000000 PKDevTools-0.13.20240417.91/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-17 21:28:23.963895 PKDevTools-0.13.20240417.91/setup.cfg
+-rw-rw-rw-   0        0        0     4341 2024-04-17 21:27:11.000000 PKDevTools-0.13.20240417.91/setup.py
```

### Comparing `PKDevTools-0.13.20240417.90/LICENSE` & `PKDevTools-0.13.20240417.91/LICENSE`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.90/PKDevTools/__init__.py` & `PKDevTools-0.13.20240417.91/PKDevTools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.90/PKDevTools/classes/Archiver.py` & `PKDevTools-0.13.20240417.91/PKDevTools/classes/Archiver.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.90/PKDevTools/classes/ColorText.py` & `PKDevTools-0.13.20240417.91/PKDevTools/classes/ColorText.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.90/PKDevTools/classes/Committer.py` & `PKDevTools-0.13.20240417.91/PKDevTools/classes/Committer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.90/PKDevTools/classes/CookieHelper.py` & `PKDevTools-0.13.20240417.91/PKDevTools/classes/CookieHelper.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.90/PKDevTools/classes/Fetcher.py` & `PKDevTools-0.13.20240417.91/PKDevTools/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.90/PKDevTools/classes/MenuOptions.py` & `PKDevTools-0.13.20240417.91/PKDevTools/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.90/PKDevTools/classes/PKDateUtilities.py` & `PKDevTools-0.13.20240417.91/PKDevTools/classes/PKDateUtilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.90/PKDevTools/classes/PKGitFolderDownloader.py` & `PKDevTools-0.13.20240417.91/PKDevTools/classes/PKGitFolderDownloader.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.90/PKDevTools/classes/PKMultiProcessorClient.py` & `PKDevTools-0.13.20240417.91/PKDevTools/classes/PKMultiProcessorClient.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.90/PKDevTools/classes/PKPickler.py` & `PKDevTools-0.13.20240417.91/PKDevTools/classes/PKPickler.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from alive_progress import alive_bar
 from PKDevTools.classes.Singleton import SingletonType, SingletonMixin
 from PKDevTools.classes import Archiver
 from PKDevTools.classes.log import default_logger
 from PKDevTools.classes.Fetcher import fetcher
 from PKDevTools.classes.Utils import getProgressbarStyle, random_user_agent
 from PKDevTools.classes.ColorText import colorText
+from PKDevTools.classes.OutputControls import OutputControls
 
 class PKPickler(SingletonMixin, metaclass=SingletonType):
     def __init__(self):
         super(PKPickler, self).__init__()
         self.fetcher = fetcher()
 
     @property
@@ -225,15 +226,15 @@
                         if filesize > 0:
                             bar, spinner = getProgressbarStyle()
                             with self.attributes["lock"]:
                                 if not os.path.isfile(cache_file) and not dataLoaded:
                                     f = open(cache_file,"wb")  # .split(os.sep)[-1]
                                     dl = 0
                                     lastPath = (cache_file.split(os.sep)[-1]).replace("DB.pkl","")
-                                    print(f"{colorText.GREEN}[+] Downloading {lastPath} cache from pkscreener server...{colorText.END}")
+                                    OutputControls().printOutput(f"{colorText.GREEN}[+] Downloading {lastPath} cache from pkscreener server...{colorText.END}")
                                     with alive_bar(
                                         filesize, bar=bar, spinner=spinner, manual=True
                                     ) as progressbar:
                                         for data in resp.iter_content(chunk_size=chunksize):
                                             dl += 1
                                             f.write(data)
                                             progressbar(dl / filesize)
@@ -243,15 +244,15 @@
                                     sys.stdout.write(f"\x1b[2A")
                                 dataLoaded = True
                         else:
                             default_logger().debug(f"Data cache file:{fileName} on server has length ->{filesize}")
                     except Exception as e:  # pragma: no cover
                         default_logger().debug(e, exc_info=True)
                         f.close()
-                        print("[!] Download Error - " + str(e))
+                        OutputControls().printOutput("[!] Download Error - " + str(e))
                     if not retrial and dataLoaded:
                         # Don't try for more than once.
                         dataDict = self.unpickle(fileName=fileName, overWriteConfirmationFuncIfCorruptedOrError=overWriteConfirmationFuncIfCorruptedOrError,retrial=True)
         return dataDict
 
 class PKPicklerDB:
     def __init__(self, fileName="default.pkl"):
```

### Comparing `PKDevTools-0.13.20240417.90/PKDevTools/classes/PKTimer.py` & `PKDevTools-0.13.20240417.91/PKDevTools/classes/PKTimer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.90/PKDevTools/classes/Singleton.py` & `PKDevTools-0.13.20240417.91/PKDevTools/classes/Singleton.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.90/PKDevTools/classes/SuppressOutput.py` & `PKDevTools-0.13.20240417.91/PKDevTools/classes/SuppressOutput.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.90/PKDevTools/classes/Telegram.py` & `PKDevTools-0.13.20240417.91/PKDevTools/classes/Telegram.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 # Get from telegram
 # See tutorial https://www.siteguarding.com/en/how-to-get-telegram-bot-api-token
 
 import requests
 from dotenv import dotenv_values
 from PKDevTools.classes.log import default_logger
+from PKDevTools.classes.OutputControls import OutputControls
 from telegram.constants import ParseMode
 
 # from io import BytesIO
 # from PIL import Image
 
 
 # URL_TELE = f"https://api.telegram.org/bot{TOKEN}/getUpdates"
@@ -150,15 +151,15 @@
     #     # print(telegram_msg.content)
 
 
 def send_photo(photoFilePath, message="", message_id=None, userID=None, retrial=False):
     initTelegram()
     if not is_token_telegram_configured():
         return
-    print(f"Sending message:{message}")
+    OutputControls().printOutput(f"Sending message:{message}")
     method = "/sendPhoto"
     global chat_idADMIN, botsUrl, Channel_Id, LIST_PEOPLE_IDS_CHAT, TOKEN
     photo = open(photoFilePath, "rb")
     if message_id is not None:
         params = {
             "chat_id": (userID if userID is not None else Channel_Id),
             "caption": message,
```

### Comparing `PKDevTools-0.13.20240417.90/PKDevTools/classes/Utils.py` & `PKDevTools-0.13.20240417.91/PKDevTools/classes/Utils.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.90/PKDevTools/classes/WorkflowManager.py` & `PKDevTools-0.13.20240417.91/PKDevTools/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.90/PKDevTools/classes/githubutilities.py` & `PKDevTools-0.13.20240417.91/PKDevTools/classes/githubutilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.90/PKDevTools/classes/log.py` & `PKDevTools-0.13.20240417.91/PKDevTools/classes/log.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.90/PKDevTools/classes/multiprocessing_logging.py` & `PKDevTools-0.13.20240417.91/PKDevTools/classes/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.90/PKDevTools/classes/squash.py` & `PKDevTools-0.13.20240417.91/PKDevTools/classes/squash.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.90/PKDevTools/classes/updater.py` & `PKDevTools-0.13.20240417.91/PKDevTools/classes/updater.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.90/PKDevTools.egg-info/PKG-INFO` & `PKDevTools-0.13.20240417.91/PKDevTools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240417.90
+Version: 0.13.20240417.91
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240417.90.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240417.91.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240417.90/PKDevTools.egg-info/SOURCES.txt` & `PKDevTools-0.13.20240417.91/PKDevTools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 PKDevTools.egg-info/top_level.txt
 PKDevTools/classes/Archiver.py
 PKDevTools/classes/ColorText.py
 PKDevTools/classes/Committer.py
 PKDevTools/classes/CookieHelper.py
 PKDevTools/classes/Fetcher.py
 PKDevTools/classes/MenuOptions.py
+PKDevTools/classes/OutputControls.py
 PKDevTools/classes/PKDateUtilities.py
 PKDevTools/classes/PKGitFolderDownloader.py
 PKDevTools/classes/PKMultiProcessorClient.py
 PKDevTools/classes/PKPickler.py
 PKDevTools/classes/PKTimer.py
 PKDevTools/classes/Singleton.py
 PKDevTools/classes/SuppressOutput.py
```

### Comparing `PKDevTools-0.13.20240417.90/PKG-INFO` & `PKDevTools-0.13.20240417.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240417.90
+Version: 0.13.20240417.91
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240417.90.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240417.91.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240417.90/README.md` & `PKDevTools-0.13.20240417.91/README.md`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240417.90/setup.py` & `PKDevTools-0.13.20240417.91/setup.py`

 * *Files identical despite different names*

