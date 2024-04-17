# Comparing `tmp/pylzss-0.3.6.tar.gz` & `tmp/pylzss-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylzss-0.3.6.tar", last modified: Tue Jan 23 20:37:18 2024, max compression
+gzip compressed data, was "pylzss-0.3.7.tar", last modified: Wed Apr 17 04:11:15 2024, max compression
```

## Comparing `pylzss-0.3.6.tar` & `pylzss-0.3.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 20:37:18.985342 pylzss-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35146 2024-01-23 20:37:12.000000 pylzss-0.3.6/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-01-23 20:37:12.000000 pylzss-0.3.6/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-23 20:37:12.000000 pylzss-0.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-01-23 20:37:18.985342 pylzss-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-01-23 20:37:12.000000 pylzss-0.3.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 20:37:18.985342 pylzss-0.3.6/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 20:37:18.985342 pylzss-0.3.6/include/py3c/
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-01-23 20:37:12.000000 pylzss-0.3.6/include/py3c/capsulethunk.h
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-01-23 20:37:12.000000 pylzss-0.3.6/include/py3c/comparison.h
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-01-23 20:37:12.000000 pylzss-0.3.6/include/py3c/compat.h
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-01-23 20:37:12.000000 pylzss-0.3.6/include/py3c/fileshim.h
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-01-23 20:37:12.000000 pylzss-0.3.6/include/py3c/py3shims.h
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-01-23 20:37:12.000000 pylzss-0.3.6/include/py3c/tpflags.h
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-01-23 20:37:12.000000 pylzss-0.3.6/include/py3c.h
--rw-r--r--   0 runner    (1001) docker     (127)    12425 2024-01-23 20:37:12.000000 pylzss-0.3.6/pylzss.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 20:37:18.985342 pylzss-0.3.6/pylzss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-01-23 20:37:18.000000 pylzss-0.3.6/pylzss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-01-23 20:37:18.000000 pylzss-0.3.6/pylzss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 20:37:18.000000 pylzss-0.3.6/pylzss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-23 20:37:18.000000 pylzss-0.3.6/pylzss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-23 20:37:18.985342 pylzss-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-01-23 20:37:12.000000 pylzss-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:11:15.296414 pylzss-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35146 2024-04-17 04:11:11.000000 pylzss-0.3.7/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-04-17 04:11:11.000000 pylzss-0.3.7/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 04:11:11.000000 pylzss-0.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-17 04:11:15.296414 pylzss-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-17 04:11:11.000000 pylzss-0.3.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:11:15.292413 pylzss-0.3.7/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:11:15.292413 pylzss-0.3.7/include/py3c/
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-17 04:11:11.000000 pylzss-0.3.7/include/py3c/capsulethunk.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-17 04:11:11.000000 pylzss-0.3.7/include/py3c/comparison.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-04-17 04:11:11.000000 pylzss-0.3.7/include/py3c/compat.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-17 04:11:11.000000 pylzss-0.3.7/include/py3c/fileshim.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-17 04:11:11.000000 pylzss-0.3.7/include/py3c/py3shims.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-17 04:11:11.000000 pylzss-0.3.7/include/py3c/tpflags.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-17 04:11:11.000000 pylzss-0.3.7/include/py3c.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12425 2024-04-17 04:11:11.000000 pylzss-0.3.7/pylzss.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:11:15.296414 pylzss-0.3.7/pylzss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-17 04:11:15.000000 pylzss-0.3.7/pylzss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-17 04:11:15.000000 pylzss-0.3.7/pylzss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 04:11:15.000000 pylzss-0.3.7/pylzss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-17 04:11:15.000000 pylzss-0.3.7/pylzss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 04:11:15.296414 pylzss-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-17 04:11:11.000000 pylzss-0.3.7/setup.py
```

### Comparing `pylzss-0.3.6/COPYING` & `pylzss-0.3.7/COPYING`

 * *Files identical despite different names*

### Comparing `pylzss-0.3.6/COPYING.LESSER` & `pylzss-0.3.7/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `pylzss-0.3.6/PKG-INFO` & `pylzss-0.3.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylzss
-Version: 0.3.6
+Version: 0.3.7
 Summary: LZSS compression algorithm
 Home-page: https://github.com/m1stadev/pylzss
 Author: Guillaume Tucker
 Author-email: guillaume.tucker@plasticlogic.com
 Maintainer: m1sta
 Maintainer-email: adamhamdi31@gmail.com
 License: GNU LGPL v3
```

### Comparing `pylzss-0.3.6/include/py3c/capsulethunk.h` & `pylzss-0.3.7/include/py3c/capsulethunk.h`

 * *Files identical despite different names*

### Comparing `pylzss-0.3.6/include/py3c/comparison.h` & `pylzss-0.3.7/include/py3c/comparison.h`

 * *Files identical despite different names*

### Comparing `pylzss-0.3.6/include/py3c/compat.h` & `pylzss-0.3.7/include/py3c/compat.h`

 * *Files identical despite different names*

### Comparing `pylzss-0.3.6/include/py3c/fileshim.h` & `pylzss-0.3.7/include/py3c/fileshim.h`

 * *Files identical despite different names*

### Comparing `pylzss-0.3.6/include/py3c/py3shims.h` & `pylzss-0.3.7/include/py3c/py3shims.h`

 * *Files identical despite different names*

### Comparing `pylzss-0.3.6/include/py3c/tpflags.h` & `pylzss-0.3.7/include/py3c/tpflags.h`

 * *Files identical despite different names*

### Comparing `pylzss-0.3.6/include/py3c.h` & `pylzss-0.3.7/include/py3c.h`

 * *Files identical despite different names*

### Comparing `pylzss-0.3.6/pylzss.c` & `pylzss-0.3.7/pylzss.c`

 * *Files identical despite different names*

### Comparing `pylzss-0.3.6/pylzss.egg-info/PKG-INFO` & `pylzss-0.3.7/pylzss.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylzss
-Version: 0.3.6
+Version: 0.3.7
 Summary: LZSS compression algorithm
 Home-page: https://github.com/m1stadev/pylzss
 Author: Guillaume Tucker
 Author-email: guillaume.tucker@plasticlogic.com
 Maintainer: m1sta
 Maintainer-email: adamhamdi31@gmail.com
 License: GNU LGPL v3
```

### Comparing `pylzss-0.3.6/setup.py` & `pylzss-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from setuptools import setup, Extension
 
 setup(
     name="pylzss",
-    version="0.3.6",
+    version="0.3.7",
     description="LZSS compression algorithm",
     author="Guillaume Tucker",
     author_email="guillaume.tucker@plasticlogic.com",
     maintainer="m1sta",
     maintainer_email="adamhamdi31@gmail.com",
     url="https://github.com/m1stadev/pylzss",
     license="GNU LGPL v3",
```

