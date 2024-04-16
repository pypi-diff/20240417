# Comparing `tmp/resolutecns-0.1.6.tar.gz` & `tmp/resolutecns-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resolutecns-0.1.6.tar", last modified: Tue Apr 16 21:48:01 2024, max compression
+gzip compressed data, was "resolutecns-0.1.7.tar", last modified: Tue Apr 16 21:56:00 2024, max compression
```

## Comparing `resolutecns-0.1.6.tar` & `resolutecns-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 21:48:01.532846 resolutecns-0.1.6/
--rw-rw-rw-   0        0        0       31 2024-04-15 18:34:47.000000 resolutecns-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0      553 2024-04-16 21:48:01.526842 resolutecns-0.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 21:48:01.471842 resolutecns-0.1.6/ResoluteCNS/
--rw-rw-rw-   0        0        0     6139 2024-04-16 21:47:38.000000 resolutecns-0.1.6/ResoluteCNS/ResoluteCNS.py
--rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.1.6/ResoluteCNS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 21:48:01.513844 resolutecns-0.1.6/ResoluteCNS/bankruptcies/
--rw-rw-rw-   0        0        0       37 2024-04-15 20:45:24.000000 resolutecns-0.1.6/ResoluteCNS/bankruptcies/__init__.py
--rw-rw-rw-   0        0        0     1889 2024-04-16 19:15:21.000000 resolutecns-0.1.6/ResoluteCNS/bankruptcies/bankruptcies.py
--rw-rw-rw-   0        0        0  3834815 2024-02-29 20:00:53.000000 resolutecns-0.1.6/ResoluteCNS/uBlock0.xpi
-drwxrwxrwx   0        0        0        0 2024-04-16 21:48:01.520963 resolutecns-0.1.6/ResoluteCNS.egg-info/
--rw-rw-rw-   0        0        0      553 2024-04-16 21:48:01.000000 resolutecns-0.1.6/ResoluteCNS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2024-04-16 21:48:01.000000 resolutecns-0.1.6/ResoluteCNS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 21:48:01.000000 resolutecns-0.1.6/ResoluteCNS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-16 21:48:01.000000 resolutecns-0.1.6/ResoluteCNS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-16 21:48:01.000000 resolutecns-0.1.6/ResoluteCNS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 21:48:01.533846 resolutecns-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1146 2024-04-16 21:47:55.000000 resolutecns-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 21:56:00.698973 resolutecns-0.1.7/
+-rw-rw-rw-   0        0        0       31 2024-04-15 18:34:47.000000 resolutecns-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      553 2024-04-16 21:56:00.693971 resolutecns-0.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-16 21:56:00.648752 resolutecns-0.1.7/ResoluteCNS/
+-rw-rw-rw-   0        0        0     6146 2024-04-16 21:51:35.000000 resolutecns-0.1.7/ResoluteCNS/ResoluteCNS.py
+-rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.1.7/ResoluteCNS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 21:56:00.683752 resolutecns-0.1.7/ResoluteCNS/bankruptcies/
+-rw-rw-rw-   0        0        0       37 2024-04-15 20:45:24.000000 resolutecns-0.1.7/ResoluteCNS/bankruptcies/__init__.py
+-rw-rw-rw-   0        0        0     1889 2024-04-16 19:15:21.000000 resolutecns-0.1.7/ResoluteCNS/bankruptcies/bankruptcies.py
+-rw-rw-rw-   0        0        0  3834815 2024-02-29 20:00:53.000000 resolutecns-0.1.7/ResoluteCNS/uBlock0.xpi
+drwxrwxrwx   0        0        0        0 2024-04-16 21:56:00.689973 resolutecns-0.1.7/ResoluteCNS.egg-info/
+-rw-rw-rw-   0        0        0      553 2024-04-16 21:56:00.000000 resolutecns-0.1.7/ResoluteCNS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-04-16 21:56:00.000000 resolutecns-0.1.7/ResoluteCNS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 21:56:00.000000 resolutecns-0.1.7/ResoluteCNS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-16 21:56:00.000000 resolutecns-0.1.7/ResoluteCNS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-16 21:56:00.000000 resolutecns-0.1.7/ResoluteCNS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 21:56:00.699978 resolutecns-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1146 2024-04-16 21:55:45.000000 resolutecns-0.1.7/setup.py
```

### Comparing `resolutecns-0.1.6/PKG-INFO` & `resolutecns-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.1.6
+Version: 0.1.7
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.1.6/ResoluteCNS/ResoluteCNS.py` & `resolutecns-0.1.7/ResoluteCNS/ResoluteCNS.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         if states:
             self.set_state_filters(states)
         if counties:
             self.set_county_filters(counties)
         
         self.click_search_complaints()
 
-        self.download_excel_complaints()
+        return self.download_excel_complaints()
 
 
     def download_excel_complaints(self):
         self._driver.set_page_load_timeout(10)
         try:
             download_excel = self._driver.find_elements(By.XPATH, "//a[@href='/SearchBeta/GetComplaintsExcel']/child::img")
             download_excel.click()
```

### Comparing `resolutecns-0.1.6/ResoluteCNS/bankruptcies/bankruptcies.py` & `resolutecns-0.1.7/ResoluteCNS/bankruptcies/bankruptcies.py`

 * *Files identical despite different names*

### Comparing `resolutecns-0.1.6/ResoluteCNS/uBlock0.xpi` & `resolutecns-0.1.7/ResoluteCNS/uBlock0.xpi`

 * *Files identical despite different names*

### Comparing `resolutecns-0.1.6/ResoluteCNS.egg-info/PKG-INFO` & `resolutecns-0.1.7/ResoluteCNS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.1.6
+Version: 0.1.7
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.1.6/setup.py` & `resolutecns-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.6' 
+VERSION = '0.1.7' 
 DESCRIPTION = 'CNS Scraping Package'
 LONG_DESCRIPTION = 'CNS Scraping Package'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="ResoluteCNS",
```

