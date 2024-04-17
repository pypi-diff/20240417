# Comparing `tmp/TineAutomationToolkit-1.0.4.tar.gz` & `tmp/TineAutomationToolkit-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TineAutomationToolkit-1.0.4.tar", last modified: Thu Apr 11 01:14:28 2024, max compression
+gzip compressed data, was "dist\TineAutomationToolkit-1.0.5.tar", last modified: Wed Apr 17 15:56:42 2024, max compression
```

## Comparing `TineAutomationToolkit-1.0.4.tar` & `TineAutomationToolkit-1.0.5.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 01:14:28.000000 TineAutomationToolkit-1.0.4/
--rw-rw-rw-   0        0        0     2280 2024-04-11 01:14:28.000000 TineAutomationToolkit-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1623 2024-03-15 00:45:23.000000 TineAutomationToolkit-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 01:14:28.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit/
--rw-rw-rw-   0        0        0      356 2024-03-19 04:35:22.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 01:14:28.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit/detect/
--rw-rw-rw-   0        0        0       99 2024-04-10 08:38:20.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit/detect/__init__.py
--rw-rw-rw-   0        0        0     4950 2024-04-10 09:28:36.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit/detect/detectelement.py
-drwxrwxrwx   0        0        0        0 2024-04-11 01:14:28.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/
--rw-rw-rw-   0        0        0      587 2024-03-19 04:35:08.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/__init__.py
--rw-rw-rw-   0        0        0     3371 2024-03-19 02:54:39.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/capturescreenshot.py
--rw-rw-rw-   0        0        0     3913 2024-04-11 01:12:35.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/connectionmanagement.py
--rw-rw-rw-   0        0        0    11638 2024-04-10 08:38:10.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/controlelement.py
--rw-rw-rw-   0        0        0     3474 2024-03-19 03:06:11.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/scroll.py
--rw-rw-rw-   0        0        0      237 2024-03-14 00:55:44.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/toolkitstest.py
--rw-rw-rw-   0        0        0     5899 2024-03-19 02:59:09.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/waitingelement.py
-drwxrwxrwx   0        0        0        0 2024-04-11 01:14:28.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit.egg-info/
--rw-rw-rw-   0        0        0     2280 2024-04-11 01:14:28.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      699 2024-04-11 01:14:28.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 01:14:28.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-11 01:14:28.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-04-11 01:14:28.000000 TineAutomationToolkit-1.0.4/TineAutomationToolkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 01:14:28.000000 TineAutomationToolkit-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      739 2024-04-11 01:06:41.000000 TineAutomationToolkit-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 15:56:42.000000 TineAutomationToolkit-1.0.5/
+-rw-rw-rw-   0        0        0     2280 2024-04-17 15:56:42.000000 TineAutomationToolkit-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1623 2024-03-15 00:45:23.000000 TineAutomationToolkit-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 15:56:42.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/
+-rw-rw-rw-   0        0        0      383 2024-04-17 15:32:05.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 15:56:42.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/detect/
+-rw-rw-rw-   0        0        0       99 2024-04-10 08:38:20.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/detect/__init__.py
+-rw-rw-rw-   0        0        0     4950 2024-04-10 09:28:36.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/detect/detectelement.py
+drwxrwxrwx   0        0        0        0 2024-04-17 15:56:42.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/
+-rw-rw-rw-   0        0        0      724 2024-04-17 15:54:04.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/__init__.py
+-rw-rw-rw-   0        0        0     3371 2024-03-19 02:54:39.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/capturescreenshot.py
+-rw-rw-rw-   0        0        0     4726 2024-04-11 09:59:28.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/connectionmanagement.py
+-rw-rw-rw-   0        0        0    18184 2024-04-17 15:53:05.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/controlelement.py
+-rw-rw-rw-   0        0        0     2495 2024-04-17 15:53:57.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/keyevent.py
+-rw-rw-rw-   0        0        0     3474 2024-03-19 03:06:11.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/scroll.py
+-rw-rw-rw-   0        0        0      237 2024-03-14 00:55:44.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/toolkitstest.py
+-rw-rw-rw-   0        0        0     2444 2024-04-17 15:25:52.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/touch.py
+-rw-rw-rw-   0        0        0     6663 2024-04-11 09:12:10.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/waitingelement.py
+drwxrwxrwx   0        0        0        0 2024-04-17 15:56:42.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit.egg-info/
+-rw-rw-rw-   0        0        0     2280 2024-04-17 15:56:42.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      782 2024-04-17 15:56:42.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 15:56:42.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-17 15:56:42.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-17 15:56:42.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 15:56:42.000000 TineAutomationToolkit-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      739 2024-04-17 15:54:28.000000 TineAutomationToolkit-1.0.5/setup.py
```

### Comparing `TineAutomationToolkit-1.0.4/PKG-INFO` & `TineAutomationToolkit-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TineAutomationToolkit
-Version: 1.0.4
+Version: 1.0.5
 Summary: Test Library for TineAutomationToolkit
 Home-page: https://github.com/pornpawit08/TineAutomationToolkit.git
 Author: Pornpawit Suttha
 Author-email: pornpawit14suttha@gmail.com
 License: UNKNOWN
 Description: # TineAutomationToolkit
         TineAutomationToolkit is a comprehensive automation toolkit designed to streamline and enhance the testing and development process for mobile applications. With a focus on integrating seamlessly with Appium and Flutter, this toolkit provides a robust set of tools and utilities to simplify the automation of mobile app testing.
```

### Comparing `TineAutomationToolkit-1.0.4/README.md` & `TineAutomationToolkit-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.4/TineAutomationToolkit/detect/detectelement.py` & `TineAutomationToolkit-1.0.5/TineAutomationToolkit/detect/detectelement.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/__init__.py` & `TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,9 +2,11 @@
 
 from TineAutomationToolkit.keywords.connectionmanagement import ConnectionManagement
 from TineAutomationToolkit.keywords.controlelement import ControlElement
 from TineAutomationToolkit.keywords.waitingelement import WaitingElement
 from TineAutomationToolkit.keywords.scroll import Scroll
 from TineAutomationToolkit.keywords.toolkitstest import ToolkitsTest
 from TineAutomationToolkit.keywords.capturescreenshot import CaptureScreenShot
+from TineAutomationToolkit.keywords.keyevent import KeyEvent
+from TineAutomationToolkit.keywords.touch import Touch
 
-__all__ = ['ToolkitsTest' , 'ConnectionManagement', 'WaitingElement', 'ControlElement','Scroll','CaptureScreenShot']
+__all__ = ['ToolkitsTest' , 'ConnectionManagement', 'WaitingElement', 'ControlElement','Scroll','CaptureScreenShot','KeyEvent','Touch']
```

### Comparing `TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/capturescreenshot.py` & `TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/capturescreenshot.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/connectionmanagement.py` & `TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/connectionmanagement.py`

 * *Files 10% similar despite different names*

```diff
@@ -67,15 +67,16 @@
 
         app_id - BundleId สำหรับ iOS, ชื่อแพ็คเกจสำหรับ Android.
         ใหม่ใน AppiumLibrary เวอร์ชัน 2
         """
         return self._current_application().terminate_app(app_id)
     
     def commond_install_app(self, app_path, app_package):
-        """ Install App via Appium
+        """ *******Not available wait for update flutter*******
+        Install App via Appium
         
         Android .
 
         - app_path - path to app (.apk)
         - app_package - package of install app to verify
 
         Ios .
@@ -96,8 +97,18 @@
         =========================================================
 
         คืนค่าอินสแตนซ์ของแอปพลิเคชันปัจจุบัน
         จาก AppiumFlutterLibrary
         """
         return cache_app.get_library_instance('AppiumFlutterLibrary')._current_application()
         # return self._bi.get_library_instance('AppiumFlutterLibrary')._current_application()
+
+    def get_source(self):
+        """Returns the entire source of the current page.
+        
+        =========================================================
+
+        ฟังก์ชันนี้จะส่งคืนสตริงที่มีซอร์สโค้ด HTML ของหน้าเว็บที่กำลังแสดงอยู่ในเบราว์เซอร์ในขณะนั้น 
+        ซึ่งสามารถนำไปใช้ในการตรวจสอบหรือวิเคราะห์โครงสร้างหรือเนื้อหาของหน้าเว็บได้
+        """
+        return self._current_application().page_source
```

### Comparing `TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/scroll.py` & `TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/scroll.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.4/TineAutomationToolkit/keywords/waitingelement.py` & `TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/waitingelement.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,14 +93,33 @@
         ตัวอย่างการใช้งาน:
 
         | t_wait_until_page_contains_element | ตำแหน่ง | เวลาที่จะให้รอ (ค่าเริ่มต้น=20s) |
         """
         if not error:
             error = "Element '%s' did not appear in <TIMEOUT>" % locator
         self._wait_until(timeout, error, conelement._is_element_present, locator)
+
+    def native_wait_until_page_contains(self, text, timeout=None, error=None):
+        """Waits until `text` appears on current page.
+
+        Fails if `timeout` expires before the text appears. See
+        `introduction` for more information about `timeout` and its
+        default value.
+
+        `error` can be used to override the default error message.
+
+        See also `Wait Until Page Does Not Contain`,
+        `Wait Until Page Contains Element`,
+        `Wait Until Page Does Not Contain Element` and
+        BuiltIn keyword `Wait Until Keyword Succeeds`.
+        """
+        if not error:
+            error = "Text '%s' did not appear in <TIMEOUT>" % text
+        self._wait_until(timeout, error, conelement._is_text_present, text)
+
     
     #PRIVATE_FUNCTION
         
     def _format_timeout(self, timeout):
         timeout = robot.utils.timestr_to_secs(timeout) if timeout is not None else timeout_in_secs
         return robot.utils.secs_to_timestr(timeout)
```

### Comparing `TineAutomationToolkit-1.0.4/TineAutomationToolkit.egg-info/PKG-INFO` & `TineAutomationToolkit-1.0.5/TineAutomationToolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TineAutomationToolkit
-Version: 1.0.4
+Version: 1.0.5
 Summary: Test Library for TineAutomationToolkit
 Home-page: https://github.com/pornpawit08/TineAutomationToolkit.git
 Author: Pornpawit Suttha
 Author-email: pornpawit14suttha@gmail.com
 License: UNKNOWN
 Description: # TineAutomationToolkit
         TineAutomationToolkit is a comprehensive automation toolkit designed to streamline and enhance the testing and development process for mobile applications. With a focus on integrating seamlessly with Appium and Flutter, this toolkit provides a robust set of tools and utilities to simplify the automation of mobile app testing.
```

### Comparing `TineAutomationToolkit-1.0.4/TineAutomationToolkit.egg-info/SOURCES.txt` & `TineAutomationToolkit-1.0.5/TineAutomationToolkit.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,10 +8,12 @@
 TineAutomationToolkit.egg-info/top_level.txt
 TineAutomationToolkit/detect/__init__.py
 TineAutomationToolkit/detect/detectelement.py
 TineAutomationToolkit/keywords/__init__.py
 TineAutomationToolkit/keywords/capturescreenshot.py
 TineAutomationToolkit/keywords/connectionmanagement.py
 TineAutomationToolkit/keywords/controlelement.py
+TineAutomationToolkit/keywords/keyevent.py
 TineAutomationToolkit/keywords/scroll.py
 TineAutomationToolkit/keywords/toolkitstest.py
+TineAutomationToolkit/keywords/touch.py
 TineAutomationToolkit/keywords/waitingelement.py
```

### Comparing `TineAutomationToolkit-1.0.4/setup.py` & `TineAutomationToolkit-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="TineAutomationToolkit",
-    version="1.0.4",
+    version="1.0.5",
     author="Pornpawit Suttha",
     author_email="pornpawit14suttha@gmail.com",
     description="Test Library for TineAutomationToolkit",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/pornpawit08/TineAutomationToolkit.git",
     packages=find_packages(),
```

