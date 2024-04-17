# Comparing `tmp/pycups-2.0.0.tar.gz` & `tmp/pycups-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "./pycups-2.0.0.tar", last modified: Thu Apr 23 10:35:01 2020, max compression
+gzip compressed data, was "./pycups-2.0.1.tar", last modified: Thu Apr 23 12:34:49 2020, max compression
```

## Comparing `pycups-2.0.0.tar` & `pycups-2.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 zdohnal  (28720) zdohnal  (28720)        0 2020-04-23 10:35:01.000000 pycups-2.0.0/
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)    18092 2019-08-20 07:58:13.000000 pycups-2.0.0/COPYING
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)     1171 2020-04-23 10:34:54.000000 pycups-2.0.0/Makefile
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)    11040 2020-04-23 09:51:47.000000 pycups-2.0.0/NEWS
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)     1296 2020-04-23 10:35:01.000000 pycups-2.0.0/PKG-INFO
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)     1091 2020-04-20 04:37:30.000000 pycups-2.0.0/README
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)       45 2019-08-20 07:58:13.000000 pycups-2.0.0/TODO
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)   172122 2020-04-23 09:29:17.000000 pycups-2.0.0/cupsconnection.c
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)     2118 2020-04-23 07:17:21.000000 pycups-2.0.0/cupsconnection.h
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)    22243 2020-04-23 08:59:55.000000 pycups-2.0.0/cupsipp.c
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)     1360 2020-04-23 07:22:50.000000 pycups-2.0.0/cupsipp.h
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)    36367 2020-04-23 09:35:55.000000 pycups-2.0.0/cupsmodule.c
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)     1660 2020-04-23 07:19:09.000000 pycups-2.0.0/cupsmodule.h
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)    46838 2020-04-23 07:19:59.000000 pycups-2.0.0/cupsppd.c
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)     1358 2020-04-23 07:23:29.000000 pycups-2.0.0/cupsppd.h
-drwxrwxr-x   0 zdohnal  (28720) zdohnal  (28720)        0 2020-04-23 10:35:01.000000 pycups-2.0.0/examples/
--rwxrwxr-x   0 zdohnal  (28720) zdohnal  (28720)     1804 2019-08-20 07:58:13.000000 pycups-2.0.0/examples/cupstree.py
--rwxrwxr-x   0 zdohnal  (28720) zdohnal  (28720)     7703 2020-04-23 07:25:04.000000 pycups-2.0.0/postscriptdriver.prov
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)      165 2019-08-20 07:58:13.000000 pycups-2.0.0/psdriver.attr
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)     2565 2020-04-23 10:13:35.000000 pycups-2.0.0/setup.py
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)      886 2019-08-20 07:58:13.000000 pycups-2.0.0/test.py
+drwxrwxr-x   0 zdohnal  (28720) zdohnal  (28720)        0 2020-04-23 12:34:49.000000 pycups-2.0.1/
+-rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)    18092 2019-08-20 07:58:13.000000 pycups-2.0.1/COPYING
+-rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)     1171 2020-04-23 10:34:54.000000 pycups-2.0.1/Makefile
+-rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)    11132 2020-04-23 12:32:38.000000 pycups-2.0.1/NEWS
+-rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)     1296 2020-04-23 12:34:49.000000 pycups-2.0.1/PKG-INFO
+-rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)     1091 2020-04-20 04:37:30.000000 pycups-2.0.1/README
+-rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)      214 2020-04-23 10:42:09.000000 pycups-2.0.1/TODO
+-rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)   172122 2020-04-23 09:29:17.000000 pycups-2.0.1/cupsconnection.c
+-rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)     2118 2020-04-23 07:17:21.000000 pycups-2.0.1/cupsconnection.h
+-rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)    22243 2020-04-23 08:59:55.000000 pycups-2.0.1/cupsipp.c
+-rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)     1360 2020-04-23 07:22:50.000000 pycups-2.0.1/cupsipp.h
+-rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)    36411 2020-04-23 11:44:12.000000 pycups-2.0.1/cupsmodule.c
+-rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)     1660 2020-04-23 07:19:09.000000 pycups-2.0.1/cupsmodule.h
+-rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)    46838 2020-04-23 07:19:59.000000 pycups-2.0.1/cupsppd.c
+-rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)     1358 2020-04-23 07:23:29.000000 pycups-2.0.1/cupsppd.h
+drwxrwxr-x   0 zdohnal  (28720) zdohnal  (28720)        0 2020-04-23 12:34:49.000000 pycups-2.0.1/examples/
+-rwxrwxr-x   0 zdohnal  (28720) zdohnal  (28720)     1804 2019-08-20 07:58:13.000000 pycups-2.0.1/examples/cupstree.py
+-rwxrwxr-x   0 zdohnal  (28720) zdohnal  (28720)     7703 2020-04-23 07:25:04.000000 pycups-2.0.1/postscriptdriver.prov
+-rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)      165 2019-08-20 07:58:13.000000 pycups-2.0.1/psdriver.attr
+-rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)     2565 2020-04-23 12:33:30.000000 pycups-2.0.1/setup.py
+-rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)      886 2019-08-20 07:58:13.000000 pycups-2.0.1/test.py
```

### Comparing `pycups-2.0.0/COPYING` & `pycups-2.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `pycups-2.0.0/Makefile` & `pycups-2.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `pycups-2.0.0/NEWS` & `pycups-2.0.1/NEWS`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 NEWS
 ----
 
+New in 2.0.1:
+* pypi required .tar.gz
+* cups.require couldn't handle version bigger than 1
+
 New in 2.0.0:
 * dropped macros for older CUPS < 2.0.0
 * dropped Python 2 support and its related macros
 * update license headers
 * thread did not hold GIL when called Py_XDECREF() from destroy_TLS(), causing SIGSEGV(Fedora bug #1816107)
 * fixed several compiler warnings
 * fix silent error on Connection.printFiles() (patch by Wilbert Berendsen)
```

### Comparing `pycups-2.0.0/PKG-INFO` & `pycups-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pycups
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python bindings for libcups
 Home-page: https://github.com/zdohnal/pycups
 Author: Zdenek Dohnal
 Author-email: zdohnal@redhat.com
 License: GPLv2+
 Download-URL: https://github.com/zdohnal/pycups/releases
 Description: This is a set of Python bindings for the libcups library from the
```

### Comparing `pycups-2.0.0/README` & `pycups-2.0.1/README`

 * *Files identical despite different names*

### Comparing `pycups-2.0.0/cupsconnection.c` & `pycups-2.0.1/cupsconnection.c`

 * *Files identical despite different names*

### Comparing `pycups-2.0.0/cupsconnection.h` & `pycups-2.0.1/cupsconnection.h`

 * *Files identical despite different names*

### Comparing `pycups-2.0.0/cupsipp.c` & `pycups-2.0.1/cupsipp.c`

 * *Files identical despite different names*

### Comparing `pycups-2.0.0/cupsipp.h` & `pycups-2.0.1/cupsipp.h`

 * *Files identical despite different names*

### Comparing `pycups-2.0.0/cupsmodule.c` & `pycups-2.0.1/cupsmodule.c`

 * *Files 1% similar despite different names*

```diff
@@ -578,18 +578,21 @@
       pver = end;
       if (*pver == '.')
 	pver++;
     }
 
     if (nver < nreq)
       goto fail;
+    if (nver > nreq)
+      goto good;
 
     nreq = strtoul (preq, &end, 0);
   }
 
+good:
   Py_RETURN_NONE;
 fail:
   PyErr_SetString (PyExc_RuntimeError, "I am version " VERSION);
   return NULL;
 }
 
 struct module_state {
```

### Comparing `pycups-2.0.0/cupsmodule.h` & `pycups-2.0.1/cupsmodule.h`

 * *Files identical despite different names*

### Comparing `pycups-2.0.0/cupsppd.c` & `pycups-2.0.1/cupsppd.c`

 * *Files identical despite different names*

### Comparing `pycups-2.0.0/cupsppd.h` & `pycups-2.0.1/cupsppd.h`

 * *Files identical despite different names*

### Comparing `pycups-2.0.0/examples/cupstree.py` & `pycups-2.0.1/examples/cupstree.py`

 * *Files identical despite different names*

### Comparing `pycups-2.0.0/postscriptdriver.prov` & `pycups-2.0.1/postscriptdriver.prov`

 * *Files identical despite different names*

### Comparing `pycups-2.0.0/setup.py` & `pycups-2.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 duplex ipp://192.168.1.1:631/printers/duplex
 HP-LaserJet-6MP ipp://192.168.1.1:631/printers/HP-LaserJet-6MP
 EPSON-Stylus-D78 usb://EPSON/Stylus%20D78
 """
 
 from distutils.core import setup, Extension
 import sys
-VERSION="2.0.0"
+VERSION="2.0.1"
 libraries=["cups"]
 
 if sys.platform == "darwin" or sys.platform.startswith("freebsd"):
 	libraries.append ("iconv")
 
 setup (name="pycups",
        version=VERSION,
```

### Comparing `pycups-2.0.0/test.py` & `pycups-2.0.1/test.py`

 * *Files identical despite different names*

