# Comparing `tmp/pycups-2.0.2.tar.gz` & `tmp/pycups-2.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycups-2.0.2.tar", last modified: Wed Apr 17 13:07:47 2024, max compression
+gzip compressed data, was "pycups-2.0.2a0.tar", last modified: Wed Apr 17 14:25:32 2024, max compression
```

## Comparing `pycups-2.0.2.tar` & `pycups-2.0.2a0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 zdohnal   (1000) zdohnal   (1000)        0 2024-04-17 13:07:47.490276 pycups-2.0.2/
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)    18092 2022-08-31 12:07:01.000000 pycups-2.0.2/COPYING
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)      256 2022-08-31 12:07:01.000000 pycups-2.0.2/MANIFEST.in
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1222 2024-04-17 11:25:39.000000 pycups-2.0.2/Makefile
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)    11598 2024-04-17 11:30:11.000000 pycups-2.0.2/NEWS
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1197 2024-04-17 13:07:47.490276 pycups-2.0.2/PKG-INFO
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1189 2022-10-25 13:03:09.000000 pycups-2.0.2/README
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)      214 2022-08-31 12:07:01.000000 pycups-2.0.2/TODO
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)   172355 2024-04-17 11:30:11.000000 pycups-2.0.2/cupsconnection.c
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     2118 2022-08-31 12:07:01.000000 pycups-2.0.2/cupsconnection.h
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)    22247 2024-04-17 11:30:11.000000 pycups-2.0.2/cupsipp.c
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1386 2022-08-31 12:07:01.000000 pycups-2.0.2/cupsipp.h
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)    36411 2022-10-25 13:03:04.000000 pycups-2.0.2/cupsmodule.c
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1660 2022-08-31 12:07:01.000000 pycups-2.0.2/cupsmodule.h
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)    46838 2022-10-25 13:03:04.000000 pycups-2.0.2/cupsppd.c
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1358 2022-08-31 12:07:01.000000 pycups-2.0.2/cupsppd.h
-drwxr-xr-x   0 zdohnal   (1000) zdohnal   (1000)        0 2024-04-17 13:07:47.489276 pycups-2.0.2/examples/
--rwxr-xr-x   0 zdohnal   (1000) zdohnal   (1000)     2114 2023-04-06 06:01:00.000000 pycups-2.0.2/examples/cupstree.py
--rwxr-xr-x   0 zdohnal   (1000) zdohnal   (1000)     7754 2022-08-31 12:07:01.000000 pycups-2.0.2/postscriptdriver.prov
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)      165 2022-08-31 12:07:01.000000 pycups-2.0.2/psdriver.attr
-drwxr-xr-x   0 zdohnal   (1000) zdohnal   (1000)        0 2024-04-17 13:07:47.490276 pycups-2.0.2/pycups.egg-info/
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1197 2024-04-17 13:07:47.000000 pycups-2.0.2/pycups.egg-info/PKG-INFO
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)      339 2024-04-17 13:07:47.000000 pycups-2.0.2/pycups.egg-info/SOURCES.txt
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)        1 2024-04-17 13:07:47.000000 pycups-2.0.2/pycups.egg-info/dependency_links.txt
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)        5 2024-04-17 13:07:47.000000 pycups-2.0.2/pycups.egg-info/top_level.txt
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)       38 2024-04-17 13:07:47.490276 pycups-2.0.2/setup.cfg
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     2663 2024-04-17 11:31:11.000000 pycups-2.0.2/setup.py
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1401 2023-04-06 08:19:15.000000 pycups-2.0.2/test.py
+drwxr-xr-x   0 zdohnal   (1000) zdohnal   (1000)        0 2024-04-17 14:25:32.518317 pycups-2.0.2a0/
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)    18092 2022-08-31 12:07:01.000000 pycups-2.0.2a0/COPYING
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)      256 2022-08-31 12:07:01.000000 pycups-2.0.2a0/MANIFEST.in
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1222 2024-04-17 11:25:39.000000 pycups-2.0.2a0/Makefile
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)    11598 2024-04-17 11:30:11.000000 pycups-2.0.2a0/NEWS
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1247 2024-04-17 14:25:32.518317 pycups-2.0.2a0/PKG-INFO
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1189 2022-10-25 13:03:09.000000 pycups-2.0.2a0/README
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)      214 2022-08-31 12:07:01.000000 pycups-2.0.2a0/TODO
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)   172355 2024-04-17 11:30:11.000000 pycups-2.0.2a0/cupsconnection.c
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     2118 2022-08-31 12:07:01.000000 pycups-2.0.2a0/cupsconnection.h
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)    22247 2024-04-17 11:30:11.000000 pycups-2.0.2a0/cupsipp.c
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1386 2022-08-31 12:07:01.000000 pycups-2.0.2a0/cupsipp.h
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)    36411 2022-10-25 13:03:04.000000 pycups-2.0.2a0/cupsmodule.c
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1660 2022-08-31 12:07:01.000000 pycups-2.0.2a0/cupsmodule.h
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)    46838 2022-10-25 13:03:04.000000 pycups-2.0.2a0/cupsppd.c
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1358 2022-08-31 12:07:01.000000 pycups-2.0.2a0/cupsppd.h
+drwxr-xr-x   0 zdohnal   (1000) zdohnal   (1000)        0 2024-04-17 14:25:32.517317 pycups-2.0.2a0/examples/
+-rwxr-xr-x   0 zdohnal   (1000) zdohnal   (1000)     2114 2023-04-06 06:01:00.000000 pycups-2.0.2a0/examples/cupstree.py
+-rwxr-xr-x   0 zdohnal   (1000) zdohnal   (1000)     7754 2022-08-31 12:07:01.000000 pycups-2.0.2a0/postscriptdriver.prov
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)      165 2022-08-31 12:07:01.000000 pycups-2.0.2a0/psdriver.attr
+drwxr-xr-x   0 zdohnal   (1000) zdohnal   (1000)        0 2024-04-17 14:25:32.518317 pycups-2.0.2a0/pycups.egg-info/
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1247 2024-04-17 14:25:32.000000 pycups-2.0.2a0/pycups.egg-info/PKG-INFO
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)      368 2024-04-17 14:25:32.000000 pycups-2.0.2a0/pycups.egg-info/SOURCES.txt
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)        1 2024-04-17 14:25:32.000000 pycups-2.0.2a0/pycups.egg-info/dependency_links.txt
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)       18 2024-04-17 14:25:32.000000 pycups-2.0.2a0/pycups.egg-info/requires.txt
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)        5 2024-04-17 14:25:32.000000 pycups-2.0.2a0/pycups.egg-info/top_level.txt
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)       38 2024-04-17 14:25:32.518317 pycups-2.0.2a0/setup.cfg
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     2746 2024-04-17 14:22:29.000000 pycups-2.0.2a0/setup.py
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1401 2023-04-06 08:19:15.000000 pycups-2.0.2a0/test.py
```

### Comparing `pycups-2.0.2/COPYING` & `pycups-2.0.2a0/COPYING`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2/Makefile` & `pycups-2.0.2a0/Makefile`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2/NEWS` & `pycups-2.0.2a0/NEWS`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2/PKG-INFO` & `pycups-2.0.2a0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycups
-Version: 2.0.2
+Version: 2.0.2a0
 Summary: Python bindings for libcups
 Home-page: https://github.com/OpenPrinting/pycups
 Download-URL: https://github.com/OpenPrinting/pycups/releases
 Maintainer: Zdenek Dohnal
 Maintainer-email: zdohnal@redhat.com
 License: GPLv2+
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,16 @@
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 License-File: COPYING
+Requires-Dist: gcc
+Requires-Dist: python3-devel
 
 This is a set of Python bindings for the libcups library from the
 CUPS project.
 
 >>> # Example of getting a list of printers
 >>> import cups
 >>> conn = cups.Connection ()
```

### Comparing `pycups-2.0.2/README` & `pycups-2.0.2a0/README`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2/cupsconnection.c` & `pycups-2.0.2a0/cupsconnection.c`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2/cupsconnection.h` & `pycups-2.0.2a0/cupsconnection.h`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2/cupsipp.c` & `pycups-2.0.2a0/cupsipp.c`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2/cupsipp.h` & `pycups-2.0.2a0/cupsipp.h`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2/cupsmodule.c` & `pycups-2.0.2a0/cupsmodule.c`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2/cupsmodule.h` & `pycups-2.0.2a0/cupsmodule.h`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2/cupsppd.c` & `pycups-2.0.2a0/cupsppd.c`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2/cupsppd.h` & `pycups-2.0.2a0/cupsppd.h`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2/examples/cupstree.py` & `pycups-2.0.2a0/examples/cupstree.py`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2/postscriptdriver.prov` & `pycups-2.0.2a0/postscriptdriver.prov`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2/pycups.egg-info/PKG-INFO` & `pycups-2.0.2a0/pycups.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycups
-Version: 2.0.2
+Version: 2.0.2a0
 Summary: Python bindings for libcups
 Home-page: https://github.com/OpenPrinting/pycups
 Download-URL: https://github.com/OpenPrinting/pycups/releases
 Maintainer: Zdenek Dohnal
 Maintainer-email: zdohnal@redhat.com
 License: GPLv2+
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,16 @@
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 License-File: COPYING
+Requires-Dist: gcc
+Requires-Dist: python3-devel
 
 This is a set of Python bindings for the libcups library from the
 CUPS project.
 
 >>> # Example of getting a list of printers
 >>> import cups
 >>> conn = cups.Connection ()
```

### Comparing `pycups-2.0.2/setup.py` & `pycups-2.0.2a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 duplex ipp://192.168.1.1:631/printers/duplex
 HP-LaserJet-6MP ipp://192.168.1.1:631/printers/HP-LaserJet-6MP
 EPSON-Stylus-D78 usb://EPSON/Stylus%20D78
 """
 
 from distutils.core import setup, Extension
 import sys
-VERSION="2.0.2"
+VERSION="2.0.2a"
 libraries=["cups"]
 
 if sys.platform == "darwin" or sys.platform.startswith("freebsd"):
     libraries.append ("iconv")
 
 setup (name="pycups",
        version=VERSION,
@@ -57,12 +57,16 @@
            "Development Status :: 5 - Production/Stable",
            "Operating System :: Unix",
            "Programming Language :: C",
            "Programming Language :: Python",
            "Programming Language :: Python :: 3",
            ],
        license="GPLv2+",
+       install_requires=[
+           'gcc',
+           'python3-devel',
+       ],
        ext_modules=[Extension("cups",
                               ["cupsmodule.c", "cupsconnection.c",
                                "cupsppd.c", "cupsipp.c"],
                               libraries=libraries,
                               define_macros=[("VERSION", '"%s"' % VERSION)])])
```

### Comparing `pycups-2.0.2/test.py` & `pycups-2.0.2a0/test.py`

 * *Files identical despite different names*

