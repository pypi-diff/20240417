# Comparing `tmp/xdriver-1.0.0.tar.gz` & `tmp/xdriver-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdriver-1.0.0.tar", last modified: Tue Apr  2 20:56:25 2024, max compression
+gzip compressed data, was "xdriver-1.1.0.tar", last modified: Wed Apr 17 15:07:17 2024, max compression
```

## Comparing `xdriver-1.0.0.tar` & `xdriver-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 20:56:25.481877 xdriver-1.0.0/
--rw-rw-rw-   0        0        0     1095 2024-04-02 14:11:13.000000 xdriver-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      703 2024-04-02 20:56:25.478311 xdriver-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       39 2024-04-02 19:34:38.000000 xdriver-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-02 20:56:25.482858 xdriver-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      917 2024-04-02 19:32:30.000000 xdriver-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:56:25.457795 xdriver-1.0.0/tests/
--rw-rw-rw-   0        0        0      760 2024-04-02 15:38:01.000000 xdriver-1.0.0/tests/test_xdriver.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:56:25.459751 xdriver-1.0.0/xdriver/
--rw-rw-rw-   0        0        0       33 2024-04-02 14:40:32.000000 xdriver-1.0.0/xdriver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:56:25.476271 xdriver-1.0.0/xdriver/src/
--rw-rw-rw-   0        0        0        0 2024-04-02 10:10:47.000000 xdriver-1.0.0/xdriver/src/__init__.py
--rw-rw-rw-   0        0        0     5457 2024-04-02 15:45:32.000000 xdriver-1.0.0/xdriver/src/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:56:25.471273 xdriver-1.0.0/xdriver.egg-info/
--rw-rw-rw-   0        0        0      703 2024-04-02 20:56:25.000000 xdriver-1.0.0/xdriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2024-04-02 20:56:25.000000 xdriver-1.0.0/xdriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 20:56:25.000000 xdriver-1.0.0/xdriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-04-02 20:56:25.000000 xdriver-1.0.0/xdriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-02 20:56:25.000000 xdriver-1.0.0/xdriver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 15:07:17.750995 xdriver-1.1.0/
+-rw-rw-rw-   0        0        0     1095 2024-04-05 14:16:27.000000 xdriver-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2775 2024-04-17 15:07:17.746736 xdriver-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2077 2024-04-05 16:00:08.000000 xdriver-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-17 15:07:17.750995 xdriver-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      917 2024-04-17 14:01:14.000000 xdriver-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 15:07:17.727199 xdriver-1.1.0/tests/
+-rw-rw-rw-   0        0        0      818 2024-04-17 14:58:45.000000 xdriver-1.1.0/tests/test_xdriver.py
+drwxrwxrwx   0        0        0        0 2024-04-17 15:07:17.730523 xdriver-1.1.0/xdriver/
+-rw-rw-rw-   0        0        0       35 2024-04-17 15:00:59.000000 xdriver-1.1.0/xdriver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 15:07:17.742683 xdriver-1.1.0/xdriver/src/
+-rw-rw-rw-   0        0        0        0 2024-04-05 14:16:27.000000 xdriver-1.1.0/xdriver/src/__init__.py
+-rw-rw-rw-   0        0        0     6255 2024-04-17 14:34:59.000000 xdriver-1.1.0/xdriver/src/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-04-17 15:07:17.740668 xdriver-1.1.0/xdriver.egg-info/
+-rw-rw-rw-   0        0        0     2775 2024-04-17 15:07:17.000000 xdriver-1.1.0/xdriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2024-04-17 15:07:17.000000 xdriver-1.1.0/xdriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 15:07:17.000000 xdriver-1.1.0/xdriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-17 15:07:17.000000 xdriver-1.1.0/xdriver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-17 15:07:17.000000 xdriver-1.1.0/xdriver.egg-info/top_level.txt
```

### Comparing `xdriver-1.0.0/LICENSE` & `xdriver-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xdriver-1.0.0/setup.py` & `xdriver-1.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="xdriver",
-    version="1.0.0",
+    version="1.1.0",
     packages=find_packages(include=["xdriver*"]),
     install_requires=[
         "pytest~=8.1.1",
         "selenium~=4.17.2",
         "webdriver-manager~=4.0.1"
     ],
     description="Expanded Selenium WebDriver",
```

### Comparing `xdriver-1.0.0/xdriver/src/webdriver.py` & `xdriver-1.1.0/xdriver/src/webdriver.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from selenium.common import StaleElementReferenceException, NoSuchElementException, TimeoutException
+from selenium.webdriver import ActionChains
 from selenium.webdriver.chrome.webdriver import WebDriver
 from webdriver_manager.chrome import ChromeDriverManager
 from typing import List, Optional
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options as ChromeOptions
 from selenium.webdriver.chrome.service import Service as ChromeService
 from selenium.webdriver.remote.webelement import WebElement
@@ -61,15 +62,15 @@
         """
         Opens the webpage provided in the 'url' parameter
 
         :param url: url
         """
         self.driver.get(url)
 
-    def get_clickable_elem_by_locator(self, locator: tuple[str, str], timeout: int = None) -> WebElement:
+    def get_clickable_element(self, locator: tuple[str, str], timeout: int = None) -> WebElement:
         """
         Waits for element to become clickable and returns that element
 
         :param locator: tuple of (selector, value)
         :param timeout: max time to wait for the WebElement before failing in seconds (Optional), default = 30
 
         :return: WebElement
@@ -77,15 +78,15 @@
         if timeout is None:
             timeout = self._default_timeout
         try:
             return WebDriverWait(self.driver, timeout).until(EC.element_to_be_clickable(locator))
         except (StaleElementReferenceException, NoSuchElementException, TimeoutException) as e:
             raise TimeoutException(f"Web element was not found! locator={locator}, Exception={e}")
 
-    def get_elem_by_locator(self, locator: tuple[str, str], timeout: int = None) -> WebElement:
+    def get_element(self, locator: tuple[str, str], timeout: int = None) -> WebElement:
         """
         Waits for element and returns that element
 
         :param locator: tuple of (selector, value)
         :param timeout: max time to wait for the WebElement before failing in seconds (Optional), default = 30
 
         :return: WebElement
@@ -93,40 +94,56 @@
         if timeout is None:
             timeout = self._default_timeout
         try:
             return WebDriverWait(self.driver, timeout).until(EC.presence_of_element_located(locator))
         except (StaleElementReferenceException, NoSuchElementException, TimeoutException) as e:
             raise TimeoutException(f"Web element was not found! locator={locator}, Exception={e}")
 
-    def check_if_elem_exists_by_locator(self, locator: tuple[str, str], timeout: int = None) -> bool:
+    def check_if_element_exists(self, locator: tuple[str, str], timeout: int = None) -> bool:
         """
         Checks if element exists by locator and returns a bool
 
         :param locator: tuple of (selector, value)
         :param timeout:  max time to wait for the WebElement before failing in seconds (Optional), default = 30
 
         :return: bool if element exists by locator
         """
         if timeout is None:
             timeout = self._default_timeout
         try:
-            self.get_elem_by_locator(locator=locator, timeout=timeout)
+            self.get_element(locator=locator, timeout=timeout)
         except TimeoutException:
             return False
         return True
 
-    def check_if_clickable_elem_exists_by_locator(self, locator: tuple[str, str], timeout: int = None) -> bool:
+    def check_if_clickable_element_exists(self, locator: tuple[str, str], timeout: int = None) -> bool:
         """
         Checks if clickable element exists by locator and returns a bool
 
         :param locator: tuple of (selector, value)
         :param timeout: max time to wait for the WebElement before failing in seconds (Optional), default = 30
 
         :return: bool if element exists and is clickable by locator
         """
         if timeout is None:
             timeout = self._default_timeout
         try:
-            self.get_elem_by_locator(locator=locator, timeout=timeout)
+            self.get_element(locator=locator, timeout=timeout)
         except TimeoutException:
             return False
         return True
+
+    def hover_over_element(self, locator: tuple[str, str], timeout: Optional[int] = 30) -> None:
+        """
+        Hovers over WebElement by locator
+
+        :param locator: tuple of (selector, value)
+        :param timeout: max time to wait for the WebElement before failing in seconds (Optional), default = 30
+        """
+        if timeout is None:
+            timeout = self._default_timeout
+        try:
+            (ActionChains(self.driver)
+             .move_to_element(WebDriverWait(self.driver, timeout).until(EC.presence_of_element_located(locator)))
+             .perform())
+        except (StaleElementReferenceException, NoSuchElementException, TimeoutException) as e:
+            raise TimeoutException(f"Web element was not found! locator={locator}, Exception={e}")
```

