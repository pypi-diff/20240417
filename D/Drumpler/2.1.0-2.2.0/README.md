# Comparing `tmp/drumpler-2.1.0.tar.gz` & `tmp/drumpler-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drumpler-2.1.0.tar", last modified: Tue Apr 16 20:02:33 2024, max compression
+gzip compressed data, was "drumpler-2.2.0.tar", last modified: Tue Apr 16 21:45:17 2024, max compression
```

## Comparing `drumpler-2.1.0.tar` & `drumpler-2.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 20:02:33.927339 drumpler-2.1.0/
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 20:02:33.925536 drumpler-2.1.0/Drumpler.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     4153 2024-04-16 20:02:33.000000 drumpler-2.1.0/Drumpler.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      514 2024-04-16 20:02:33.000000 drumpler-2.1.0/Drumpler.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-16 20:02:33.000000 drumpler-2.1.0/Drumpler.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)       64 2024-04-16 20:02:33.000000 drumpler-2.1.0/Drumpler.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-16 20:02:33.000000 drumpler-2.1.0/Drumpler.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler-2.1.0/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     4153 2024-04-16 20:02:33.926560 drumpler-2.1.0/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler-2.1.0/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 20:02:33.919631 drumpler-2.1.0/drumpler/
--rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-16 18:54:33.000000 drumpler-2.1.0/drumpler/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)      738 2024-04-16 19:59:55.000000 drumpler-2.1.0/drumpler/config.py
--rw-r--r--   0 Karel      (503) staff       (20)     8574 2024-04-16 20:01:16.000000 drumpler-2.1.0/drumpler/drumpler.py
--rw-r--r--   0 Karel      (503) staff       (20)       69 2024-04-16 18:54:36.000000 drumpler-2.1.0/drumpler/sql_base.py
--rw-r--r--   0 Karel      (503) staff       (20)      497 2024-04-16 18:54:38.000000 drumpler-2.1.0/drumpler/sql_event.py
--rw-r--r--   0 Karel      (503) staff       (20)      710 2024-04-16 18:54:37.000000 drumpler-2.1.0/drumpler/sql_job.py
--rw-r--r--   0 Karel      (503) staff       (20)      635 2024-04-16 18:54:37.000000 drumpler-2.1.0/drumpler/sql_request.py
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-16 20:02:33.927534 drumpler-2.1.0/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      783 2024-04-16 20:02:15.000000 drumpler-2.1.0/setup.py
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 20:02:33.924345 drumpler-2.1.0/test/
--rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 drumpler-2.1.0/test/test_drumpler.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 21:45:17.645516 drumpler-2.2.0/
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 21:45:17.643841 drumpler-2.2.0/Drumpler.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     4153 2024-04-16 21:45:17.000000 drumpler-2.2.0/Drumpler.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      355 2024-04-16 21:45:17.000000 drumpler-2.2.0/Drumpler.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-16 21:45:17.000000 drumpler-2.2.0/Drumpler.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       64 2024-04-16 21:45:17.000000 drumpler-2.2.0/Drumpler.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-16 21:45:17.000000 drumpler-2.2.0/Drumpler.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler-2.2.0/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     4153 2024-04-16 21:45:17.644816 drumpler-2.2.0/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler-2.2.0/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 21:45:17.642430 drumpler-2.2.0/drumpler/
+-rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-16 18:54:33.000000 drumpler-2.2.0/drumpler/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)      738 2024-04-16 19:59:55.000000 drumpler-2.2.0/drumpler/config.py
+-rw-r--r--   0 Karel      (503) staff       (20)    10073 2024-04-16 21:44:39.000000 drumpler-2.2.0/drumpler/drumpler.py
+-rw-r--r--   0 Karel      (503) staff       (20)       69 2024-04-16 18:54:36.000000 drumpler-2.2.0/drumpler/sql_base.py
+-rw-r--r--   0 Karel      (503) staff       (20)      497 2024-04-16 18:54:38.000000 drumpler-2.2.0/drumpler/sql_event.py
+-rw-r--r--   0 Karel      (503) staff       (20)      710 2024-04-16 18:54:37.000000 drumpler-2.2.0/drumpler/sql_job.py
+-rw-r--r--   0 Karel      (503) staff       (20)      579 2024-04-16 21:42:49.000000 drumpler-2.2.0/drumpler/sql_request.py
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-16 21:45:17.645667 drumpler-2.2.0/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)      783 2024-04-16 21:44:53.000000 drumpler-2.2.0/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 21:45:17.643033 drumpler-2.2.0/test/
+-rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 drumpler-2.2.0/test/test_drumpler.py
```

### Comparing `drumpler-2.1.0/Drumpler.egg-info/PKG-INFO` & `drumpler-2.2.0/Drumpler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 2.1.0
+Version: 2.2.0
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `drumpler-2.1.0/LICENSE` & `drumpler-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drumpler-2.1.0/PKG-INFO` & `drumpler-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 2.1.0
+Version: 2.2.0
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `drumpler-2.1.0/README.md` & `drumpler-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `drumpler-2.1.0/drumpler/config.py` & `drumpler-2.2.0/drumpler/config.py`

 * *Files identical despite different names*

### Comparing `drumpler-2.1.0/drumpler/sql_job.py` & `drumpler-2.2.0/drumpler/sql_job.py`

 * *Files identical despite different names*

### Comparing `drumpler-2.1.0/drumpler/sql_request.py` & `drumpler-2.2.0/drumpler/sql_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,8 +9,7 @@
     source_ip = Column(String(128))
     user_agent = Column(String(256))
     method = Column(String(8))
     request_url = Column(String(256))
     request_raw = Column(Text)
     custom_value = Column(String(256))
     is_handled = Column(Integer, default=0)
-    is_being_processed = Column(Boolean, default=False)
```

### Comparing `drumpler-2.1.0/setup.py` & `drumpler-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Drumpler',
-    version='2.1.0',
+    version='2.2.0',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='Framework for rapidly developing a restful API that requires post processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/Drumpler',
     packages=find_packages(),
```

### Comparing `drumpler-2.1.0/test/test_drumpler.py` & `drumpler-2.2.0/test/test_drumpler.py`

 * *Files identical despite different names*

