# Comparing `tmp/droid-1.4.21.tar.gz` & `tmp/droid-1.4.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "droid-1.4.21.tar", last modified: Mon Mar  6 17:28:50 2023, max compression
+gzip compressed data, was "droid-1.4.22.tar", last modified: Wed Apr 17 04:51:09 2024, max compression
```

## Comparing `droid-1.4.21.tar` & `droid-1.4.22.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-03-06 17:28:50.095914 droid-1.4.21/
--rw-r--r--   0 azazel     (501) staff       (20)     1069 2023-03-06 16:22:51.000000 droid-1.4.21/LICENSE
--rw-r--r--   0 azazel     (501) staff       (20)     4536 2023-03-06 17:28:50.095770 droid-1.4.21/PKG-INFO
--rw-r--r--   0 azazel     (501) staff       (20)     4001 2023-03-06 17:28:23.000000 droid-1.4.21/README.md
-drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-03-06 17:28:50.094384 droid-1.4.21/droid/
--rw-r--r--   0 azazel     (501) staff       (20)      141 2023-03-06 16:34:44.000000 droid-1.4.21/droid/__init__.py
--rw-r--r--   0 azazel     (501) staff       (20)    11093 2023-03-06 17:25:46.000000 droid-1.4.21/droid/main.py
--rw-r--r--   0 azazel     (501) staff       (20)    51376 2023-03-06 17:24:03.000000 droid-1.4.21/droid/view.py
-drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-03-06 17:28:50.095582 droid-1.4.21/droid.egg-info/
--rw-r--r--   0 azazel     (501) staff       (20)     4536 2023-03-06 17:28:50.000000 droid-1.4.21/droid.egg-info/PKG-INFO
--rw-r--r--   0 azazel     (501) staff       (20)      248 2023-03-06 17:28:50.000000 droid-1.4.21/droid.egg-info/SOURCES.txt
--rw-r--r--   0 azazel     (501) staff       (20)        1 2023-03-06 17:28:50.000000 droid-1.4.21/droid.egg-info/dependency_links.txt
--rw-r--r--   0 azazel     (501) staff       (20)       48 2023-03-06 17:28:50.000000 droid-1.4.21/droid.egg-info/entry_points.txt
--rw-r--r--   0 azazel     (501) staff       (20)       30 2023-03-06 17:28:50.000000 droid-1.4.21/droid.egg-info/requires.txt
--rw-r--r--   0 azazel     (501) staff       (20)        6 2023-03-06 17:28:50.000000 droid-1.4.21/droid.egg-info/top_level.txt
--rw-r--r--   0 azazel     (501) staff       (20)       38 2023-03-06 17:28:50.095955 droid-1.4.21/setup.cfg
--rw-r--r--   0 azazel     (501) staff       (20)     1105 2023-03-06 17:23:22.000000 droid-1.4.21/setup.py
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2024-04-17 04:51:09.563917 droid-1.4.22/
+-rw-r--r--   0 azazel     (501) staff       (20)     1076 2024-04-17 04:50:04.000000 droid-1.4.22/LICENSE
+-rw-r--r--   0 azazel     (501) staff       (20)     5049 2024-04-17 04:51:09.563683 droid-1.4.22/PKG-INFO
+-rw-r--r--   0 azazel     (501) staff       (20)     4450 2024-04-17 04:49:52.000000 droid-1.4.22/README.md
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2024-04-17 04:51:09.562364 droid-1.4.22/droid/
+-rw-r--r--   0 azazel     (501) staff       (20)      147 2024-04-17 04:49:42.000000 droid-1.4.22/droid/__init__.py
+-rw-r--r--   0 azazel     (501) staff       (20)    11101 2024-04-17 04:50:28.000000 droid-1.4.22/droid/main.py
+-rw-r--r--   0 azazel     (501) staff       (20)    51382 2024-04-17 04:49:42.000000 droid-1.4.22/droid/view.py
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2024-04-17 04:51:09.563431 droid-1.4.22/droid.egg-info/
+-rw-r--r--   0 azazel     (501) staff       (20)     5049 2024-04-17 04:51:09.000000 droid-1.4.22/droid.egg-info/PKG-INFO
+-rw-r--r--   0 azazel     (501) staff       (20)      248 2024-04-17 04:51:09.000000 droid-1.4.22/droid.egg-info/SOURCES.txt
+-rw-r--r--   0 azazel     (501) staff       (20)        1 2024-04-17 04:51:09.000000 droid-1.4.22/droid.egg-info/dependency_links.txt
+-rw-r--r--   0 azazel     (501) staff       (20)       48 2024-04-17 04:51:09.000000 droid-1.4.22/droid.egg-info/entry_points.txt
+-rw-r--r--   0 azazel     (501) staff       (20)       30 2024-04-17 04:51:09.000000 droid-1.4.22/droid.egg-info/requires.txt
+-rw-r--r--   0 azazel     (501) staff       (20)        6 2024-04-17 04:51:09.000000 droid-1.4.22/droid.egg-info/top_level.txt
+-rw-r--r--   0 azazel     (501) staff       (20)       38 2024-04-17 04:51:09.563961 droid-1.4.22/setup.cfg
+-rw-r--r--   0 azazel     (501) staff       (20)     1115 2024-04-17 04:50:28.000000 droid-1.4.22/setup.py
```

### Comparing `droid-1.4.21/LICENSE` & `droid-1.4.22/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 azazelm3dj3d
+Copyright (c) 2022-2024 battleoverflow
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `droid-1.4.21/PKG-INFO` & `droid-1.4.22/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,49 @@
-Metadata-Version: 2.1
-Name: droid
-Version: 1.4.21
-Summary: Droid is a remote communication application created to communicate with Android devices on the local network over the Android debug bridge (adb). Available as a CLI or GUI.
-Home-page: https://github.com/azazelm3dj3d/droid
-Author: azazelm3dj3d
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Droid
 
-<img src="https://raw.githubusercontent.com/azazelm3dj3d/droid/main/.github/assets/droid_logo.png" />
+<img src="https://raw.githubusercontent.com/battleoverflow/droid/main/.github/assets/droid_logo.png" />
 
-Droid is a remote communication application created to communicate with Android devices on the local network over the Android debug bridge (adb). Droid allows you to completely control the Android device using multiple options, including a CLI and a GUI.
+Droid is a desktop application created to communicate with Android devices on the local network over the Android debug bridge (adb). You can access the Android device directly over USB or connect to the device through Droid via `adb`. Droid allows you to completely control the Android device using multiple options, including a CLI and a GUI.
 
-IMPORTANT NOTE: Script does require Android debug bridge (adb) to be installed on the system.
+IMPORTANT NOTE: Application does require Android debug bridge (adb) to be installed on the system.
 
 ## Install
-Droid can be installed via `pip`:
+
+Droid can be installed via `pip`
+
 ```bash
 pip install droid
 ```
 
-## Simple usage
+You can also download the executable from `itch.io`: https://battleoverflow.itch.io/droid
+
+## GUI
+
+If you would like to run the GUI, you can run this command to boot it up
+
+```bash
+droid
+
+# or
+
+droid -g
+```
+
+Current state of the user interface
+
+<img src="https://raw.githubusercontent.com/battleoverflow/droid/main/.github/assets/gui.png" />
+
+## Simple usage (CLI)
+
 ```bash
 droid -ip 127.0.0.1 -c
 ```
 
 ## Options
+
 ```
 -h,   --help	    |	Help menu
 -v,   --version	    |	Version information for Droid
 -ip,  --ip_address  |   IP address of the Android device
 -up,  --upload      |   Absolute path of the APK to upload (ex: ~/Downloads/ApkName.apk)
 -rm,  --remove      |   Removes the old APK with the same package name (requires the -p flag)
 -c,   --connect     |   Connects to the Android device (requires the -ip flag)
@@ -52,54 +61,57 @@
 -o,  --output       |   Name of the output file when taking a screenshot (omit the extension)
 -l,  --log          |   Outputs Logcat logs in real time to a set file
 -g,  --gui          |   A graphical user interface built to communicate with an Android device
 -co   --content     |   Update a file on the Android device without downloading it
 ```
 
 I would recommend running this command before doing anything else to confirm you can successfully connect to the Android device on your network
+
 ```bash
 droid -ip 127.0.0.1 -c
 ```
 
 ## Example(s)
+
 This example connects to the Android device (127.0.0.1), removes the specified APK package (`com.android.ui`), and then uploads a new APK called `test_apk_v1.apk`
+
 ```bash
 droid -ip 127.0.0.1 -c -rm -p com.android.ui -up ~/Downloads/test_apk_v1.apk
 ```
 
 This example downloads a test images from the Android device onto your local machine (automatically saves it in the ~/Downloads folder on most platforms)
+
 ```bash
 droid -ip 127.0.0.1 --download /sdcard/cool_pic.png
 ```
 
 Once you're finished working within the environment, you can run this command to disconnect from the Android device:
+
 ```bash
 droid -ip 127.0.0.1 -d
 ```
 
 We now have the option to control the bluetooth service on Android devices. You can `start` the service by running this command (stopping the service uses the `stop` argument):
+
 ```bash
 droid -ip 127.0.0.1 -bl=start
 ```
 
 You can `stop` the service by running this command (starting the service uses the `start` argument):
+
 ```bash
 droid -ip 127.0.0.1 -w=stop
 ```
+
 NOTE: When turning the wifi off, if you are communicating with the Android device remotely, this will result in the device being disconnected and unusable until the network is re-established.
 
 This command will take a screenshot of the current Android screen while monitoring Logcat in real-time:
+
 ```bash
 droid -ip 127.0.0.1 -sl -o screenshot
 ```
 
-## GUI
-You can now double-click the Droid icon to run it on most platforms
-
-If you would like to run the GUI, you can run this command to boot it up. Almost all CLI options are available in the GUI:
-```bash
-droid
+# More Info
 
-# or
+A wiki for common Android snippets is also available. This wiki shows examples of how Droid can used with the Android operating system
 
-droid -g
-```
+Wiki: https://github.com/battleoverflow/droid/wiki/Helpful-Android-Snippets
```

### Comparing `droid-1.4.21/README.md` & `droid-1.4.22/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,64 @@
+Metadata-Version: 2.1
+Name: droid
+Version: 1.4.22
+Summary: Droid is a remote communication application created to communicate with Android devices on the local network over the Android debug bridge (adb). Available as a CLI or GUI.
+Home-page: https://github.com/battleoverflow/droid
+Author: battleoverflow
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: argparse
+Requires-Dist: customtkinter==4.6.3
+
 # Droid
 
-<img src="https://raw.githubusercontent.com/azazelm3dj3d/droid/main/.github/assets/droid_logo.png" />
+<img src="https://raw.githubusercontent.com/battleoverflow/droid/main/.github/assets/droid_logo.png" />
 
-Droid is a remote communication application created to communicate with Android devices on the local network over the Android debug bridge (adb). Droid allows you to completely control the Android device using multiple options, including a CLI and a GUI.
+Droid is a desktop application created to communicate with Android devices on the local network over the Android debug bridge (adb). You can access the Android device directly over USB or connect to the device through Droid via `adb`. Droid allows you to completely control the Android device using multiple options, including a CLI and a GUI.
 
-IMPORTANT NOTE: Script does require Android debug bridge (adb) to be installed on the system.
+IMPORTANT NOTE: Application does require Android debug bridge (adb) to be installed on the system.
 
 ## Install
-Droid can be installed via `pip`:
+
+Droid can be installed via `pip`
+
 ```bash
 pip install droid
 ```
 
-## Simple usage
+You can also download the executable from `itch.io`: https://battleoverflow.itch.io/droid
+
+## GUI
+
+If you would like to run the GUI, you can run this command to boot it up
+
+```bash
+droid
+
+# or
+
+droid -g
+```
+
+Current state of the user interface
+
+<img src="https://raw.githubusercontent.com/battleoverflow/droid/main/.github/assets/gui.png" />
+
+## Simple usage (CLI)
+
 ```bash
 droid -ip 127.0.0.1 -c
 ```
 
 ## Options
+
 ```
 -h,   --help	    |	Help menu
 -v,   --version	    |	Version information for Droid
 -ip,  --ip_address  |   IP address of the Android device
 -up,  --upload      |   Absolute path of the APK to upload (ex: ~/Downloads/ApkName.apk)
 -rm,  --remove      |   Removes the old APK with the same package name (requires the -p flag)
 -c,   --connect     |   Connects to the Android device (requires the -ip flag)
@@ -39,54 +76,57 @@
 -o,  --output       |   Name of the output file when taking a screenshot (omit the extension)
 -l,  --log          |   Outputs Logcat logs in real time to a set file
 -g,  --gui          |   A graphical user interface built to communicate with an Android device
 -co   --content     |   Update a file on the Android device without downloading it
 ```
 
 I would recommend running this command before doing anything else to confirm you can successfully connect to the Android device on your network
+
 ```bash
 droid -ip 127.0.0.1 -c
 ```
 
 ## Example(s)
+
 This example connects to the Android device (127.0.0.1), removes the specified APK package (`com.android.ui`), and then uploads a new APK called `test_apk_v1.apk`
+
 ```bash
 droid -ip 127.0.0.1 -c -rm -p com.android.ui -up ~/Downloads/test_apk_v1.apk
 ```
 
 This example downloads a test images from the Android device onto your local machine (automatically saves it in the ~/Downloads folder on most platforms)
+
 ```bash
 droid -ip 127.0.0.1 --download /sdcard/cool_pic.png
 ```
 
 Once you're finished working within the environment, you can run this command to disconnect from the Android device:
+
 ```bash
 droid -ip 127.0.0.1 -d
 ```
 
 We now have the option to control the bluetooth service on Android devices. You can `start` the service by running this command (stopping the service uses the `stop` argument):
+
 ```bash
 droid -ip 127.0.0.1 -bl=start
 ```
 
 You can `stop` the service by running this command (starting the service uses the `start` argument):
+
 ```bash
 droid -ip 127.0.0.1 -w=stop
 ```
+
 NOTE: When turning the wifi off, if you are communicating with the Android device remotely, this will result in the device being disconnected and unusable until the network is re-established.
 
 This command will take a screenshot of the current Android screen while monitoring Logcat in real-time:
+
 ```bash
 droid -ip 127.0.0.1 -sl -o screenshot
 ```
 
-## GUI
-You can now double-click the Droid icon to run it on most platforms
-
-If you would like to run the GUI, you can run this command to boot it up. Almost all CLI options are available in the GUI:
-```bash
-droid
+# More Info
 
-# or
+A wiki for common Android snippets is also available. This wiki shows examples of how Droid can used with the Android operating system
 
-droid -g
-```
+Wiki: https://github.com/battleoverflow/droid/wiki/Helpful-Android-Snippets
```

### Comparing `droid-1.4.21/droid/main.py` & `droid-1.4.22/droid/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-    Owner: azazelm3dj3d (https://github.com/azazelm3dj3d)
-    Project: Droid (https://github.com/azazelm3dj3d/droid)
+    Owner: battleoverflow (https://github.com/battleoverflow)
+    Project: Droid (https://github.com/battleoverflow/droid)
     License: MIT
 """
 
 import os, argparse, sys, time, platform
 from subprocess import getoutput
 from droid.view import View
 # from _tkinter import TclError
@@ -30,16 +30,16 @@
 parser.add_argument('-o', '--output', help="Name of the output file when taking a screenshot (omit the extension)", default="screenshot", required=False)
 parser.add_argument('-l', '--log', help="Outputs Logcat logs in real time to a set file", action='store_true', default=False, required=False)
 parser.add_argument('-g', '--gui', help="Opens Droid in a graphical user interface", action='store_true', default=False, required=False)
 parser.add_argument('-co', '--content', help="Update a file on the Android device without downloading it", default=None, required=False)
 
 args = parser.parse_args()
 
-author = "azazelm3dj3d"
-version = "1.4.21"
+author = "battleoverflow"
+version = "1.4.22"
 
 # Default Android Debug Bridge (adb) location on specific platforms
 if platform.system() == 'Darwin':
     adb = "$HOME/Library/Android/sdk/platform-tools/adb"
 elif platform.system() == 'Windows':
     adb = "%LOCALAPPDATA%\Android\sdk\platform-tools\\adb"
 elif platform.system() == 'Linux':
```

### Comparing `droid-1.4.21/droid/view.py` & `droid-1.4.22/droid/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-    Owner: azazelm3dj3d (https://github.com/azazelm3dj3d)
-    Project: Droid (https://github.com/azazelm3dj3d/droid)
+    Owner: battleoverflow (https://github.com/battleoverflow)
+    Project: Droid (https://github.com/battleoverflow/droid)
     License: MIT
 """
 
 import tkinter, customtkinter, platform, time, json
 from tkinter import PhotoImage, messagebox
 from subprocess import getoutput
 from os.path import getsize, exists
```

### Comparing `droid-1.4.21/droid.egg-info/PKG-INFO` & `droid-1.4.22/droid.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,64 @@
 Metadata-Version: 2.1
 Name: droid
-Version: 1.4.21
+Version: 1.4.22
 Summary: Droid is a remote communication application created to communicate with Android devices on the local network over the Android debug bridge (adb). Available as a CLI or GUI.
-Home-page: https://github.com/azazelm3dj3d/droid
-Author: azazelm3dj3d
+Home-page: https://github.com/battleoverflow/droid
+Author: battleoverflow
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: argparse
+Requires-Dist: customtkinter==4.6.3
 
 # Droid
 
-<img src="https://raw.githubusercontent.com/azazelm3dj3d/droid/main/.github/assets/droid_logo.png" />
+<img src="https://raw.githubusercontent.com/battleoverflow/droid/main/.github/assets/droid_logo.png" />
 
-Droid is a remote communication application created to communicate with Android devices on the local network over the Android debug bridge (adb). Droid allows you to completely control the Android device using multiple options, including a CLI and a GUI.
+Droid is a desktop application created to communicate with Android devices on the local network over the Android debug bridge (adb). You can access the Android device directly over USB or connect to the device through Droid via `adb`. Droid allows you to completely control the Android device using multiple options, including a CLI and a GUI.
 
-IMPORTANT NOTE: Script does require Android debug bridge (adb) to be installed on the system.
+IMPORTANT NOTE: Application does require Android debug bridge (adb) to be installed on the system.
 
 ## Install
-Droid can be installed via `pip`:
+
+Droid can be installed via `pip`
+
 ```bash
 pip install droid
 ```
 
-## Simple usage
+You can also download the executable from `itch.io`: https://battleoverflow.itch.io/droid
+
+## GUI
+
+If you would like to run the GUI, you can run this command to boot it up
+
+```bash
+droid
+
+# or
+
+droid -g
+```
+
+Current state of the user interface
+
+<img src="https://raw.githubusercontent.com/battleoverflow/droid/main/.github/assets/gui.png" />
+
+## Simple usage (CLI)
+
 ```bash
 droid -ip 127.0.0.1 -c
 ```
 
 ## Options
+
 ```
 -h,   --help	    |	Help menu
 -v,   --version	    |	Version information for Droid
 -ip,  --ip_address  |   IP address of the Android device
 -up,  --upload      |   Absolute path of the APK to upload (ex: ~/Downloads/ApkName.apk)
 -rm,  --remove      |   Removes the old APK with the same package name (requires the -p flag)
 -c,   --connect     |   Connects to the Android device (requires the -ip flag)
@@ -52,54 +76,57 @@
 -o,  --output       |   Name of the output file when taking a screenshot (omit the extension)
 -l,  --log          |   Outputs Logcat logs in real time to a set file
 -g,  --gui          |   A graphical user interface built to communicate with an Android device
 -co   --content     |   Update a file on the Android device without downloading it
 ```
 
 I would recommend running this command before doing anything else to confirm you can successfully connect to the Android device on your network
+
 ```bash
 droid -ip 127.0.0.1 -c
 ```
 
 ## Example(s)
+
 This example connects to the Android device (127.0.0.1), removes the specified APK package (`com.android.ui`), and then uploads a new APK called `test_apk_v1.apk`
+
 ```bash
 droid -ip 127.0.0.1 -c -rm -p com.android.ui -up ~/Downloads/test_apk_v1.apk
 ```
 
 This example downloads a test images from the Android device onto your local machine (automatically saves it in the ~/Downloads folder on most platforms)
+
 ```bash
 droid -ip 127.0.0.1 --download /sdcard/cool_pic.png
 ```
 
 Once you're finished working within the environment, you can run this command to disconnect from the Android device:
+
 ```bash
 droid -ip 127.0.0.1 -d
 ```
 
 We now have the option to control the bluetooth service on Android devices. You can `start` the service by running this command (stopping the service uses the `stop` argument):
+
 ```bash
 droid -ip 127.0.0.1 -bl=start
 ```
 
 You can `stop` the service by running this command (starting the service uses the `start` argument):
+
 ```bash
 droid -ip 127.0.0.1 -w=stop
 ```
+
 NOTE: When turning the wifi off, if you are communicating with the Android device remotely, this will result in the device being disconnected and unusable until the network is re-established.
 
 This command will take a screenshot of the current Android screen while monitoring Logcat in real-time:
+
 ```bash
 droid -ip 127.0.0.1 -sl -o screenshot
 ```
 
-## GUI
-You can now double-click the Droid icon to run it on most platforms
-
-If you would like to run the GUI, you can run this command to boot it up. Almost all CLI options are available in the GUI:
-```bash
-droid
+# More Info
 
-# or
+A wiki for common Android snippets is also available. This wiki shows examples of how Droid can used with the Android operating system
 
-droid -g
-```
+Wiki: https://github.com/battleoverflow/droid/wiki/Helpful-Android-Snippets
```

### Comparing `droid-1.4.21/setup.py` & `droid-1.4.22/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
-    Owner: azazelm3dj3d (https://github.com/azazelm3dj3d)
-    Project: Droid (https://github.com/azazelm3dj3d/droid)
+    Owner: battleoverflow (https://github.com/battleoverflow)
+    Project: Droid (https://github.com/battleoverflow/droid)
     License: MIT
 """
 
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "droid",
-    version = "1.4.21",
-    author = "azazelm3dj3d",
+    version = "1.4.22",
+    author = "battleoverflow",
     description = "Droid is a remote communication application created to communicate with Android devices on the local network over the Android debug bridge (adb). Available as a CLI or GUI.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
-    url = "https://github.com/azazelm3dj3d/droid",
+    url = "https://github.com/battleoverflow/droid",
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages = ["droid"],
     install_requires=[
```

