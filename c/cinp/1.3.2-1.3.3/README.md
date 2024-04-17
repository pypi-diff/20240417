# Comparing `tmp/cinp-1.3.2.tar.gz` & `tmp/cinp-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cinp-1.3.2.tar", last modified: Fri Feb 16 20:39:54 2024, max compression
+gzip compressed data, was "cinp-1.3.3.tar", last modified: Wed Apr 17 04:45:19 2024, max compression
```

## Comparing `cinp-1.3.2.tar` & `cinp-1.3.3.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-02-16 20:39:54.593773 cinp-1.3.2/
--rw-rw-r--   0 peter     (1000) peter     (1000)      784 2024-02-16 20:39:54.597773 cinp-1.3.2/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)     1963 2024-02-01 05:02:53.435243 cinp-1.3.2/README.rst
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-02-16 20:39:54.593773 cinp-1.3.2/cinp/
--rw-rw-r--   0 peter     (1000) peter     (1000)        0 2017-01-05 15:06:39.795258 cinp-1.3.2/cinp/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    25071 2024-02-16 20:39:30.078288 cinp-1.3.2/cinp/client.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    37819 2024-02-01 05:02:53.435243 cinp-1.3.2/cinp/client_test.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4279 2024-02-01 05:02:53.435243 cinp-1.3.2/cinp/common.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     7291 2024-02-01 05:02:53.439242 cinp-1.3.2/cinp/common_test.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3357 2024-02-01 05:02:53.439242 cinp-1.3.2/cinp/django_file_handler.py
-lrwxrwxrwx   0 peter     (1000) peter     (1000)        0 2020-08-14 13:25:31.338020 cinp-1.3.2/cinp/django_settings.py -> ../django_test.settings
--rw-rw-r--   0 peter     (1000) peter     (1000)    26982 2024-02-01 05:02:53.443242 cinp-1.3.2/cinp/orm_django.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    34225 2024-02-01 05:02:53.447241 cinp-1.3.2/cinp/orm_django_test.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5086 2019-03-12 17:18:48.072860 cinp-1.3.2/cinp/orm_null.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    12710 2019-04-17 00:28:15.394905 cinp-1.3.2/cinp/orm_peewee.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      851 2020-08-11 23:28:51.800863 cinp-1.3.2/cinp/readers.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    53116 2024-02-09 05:19:15.953496 cinp-1.3.2/cinp/server_common.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    54417 2024-02-01 05:02:53.451241 cinp-1.3.2/cinp/server_common_test.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     7040 2024-02-16 20:39:30.078288 cinp-1.3.2/cinp/server_werkzeug.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5377 2024-02-01 05:02:53.455241 cinp-1.3.2/cinp/server_werkzeug_test.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)     1717 2024-02-01 05:02:53.459240 cinp-1.3.2/setup.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-04-17 04:45:19.350221 cinp-1.3.3/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      784 2024-04-17 04:45:19.350221 cinp-1.3.3/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1963 2021-01-09 19:32:33.073446 cinp-1.3.3/README.rst
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-04-17 04:45:19.350221 cinp-1.3.3/cinp/
+-rw-rw-r--   0 peter     (1000) peter     (1000)        0 2017-01-05 15:06:39.000000 cinp-1.3.3/cinp/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    25049 2024-04-07 03:26:14.408028 cinp-1.3.3/cinp/client.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    37819 2021-06-16 22:21:16.762807 cinp-1.3.3/cinp/client_test.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4279 2022-01-21 18:46:55.435187 cinp-1.3.3/cinp/common.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7291 2021-09-21 18:49:23.950327 cinp-1.3.3/cinp/common_test.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3357 2021-01-12 22:30:48.003805 cinp-1.3.3/cinp/django_file_handler.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    26982 2022-06-07 22:26:48.457763 cinp-1.3.3/cinp/orm_django.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    34225 2022-03-21 18:07:01.457825 cinp-1.3.3/cinp/orm_django_test.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5086 2019-03-12 17:18:48.000000 cinp-1.3.3/cinp/orm_null.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)        5 2022-06-08 00:02:10.239250 cinp-1.3.3/cinp/orm_peewee.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      851 2020-08-11 23:28:51.000000 cinp-1.3.3/cinp/readers.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    53116 2024-02-14 02:19:47.883791 cinp-1.3.3/cinp/server_common.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    54417 2022-02-11 15:37:54.302914 cinp-1.3.3/cinp/server_common_test.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7040 2024-02-14 02:17:38.927030 cinp-1.3.3/cinp/server_werkzeug.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5377 2022-02-10 15:57:52.529872 cinp-1.3.3/cinp/server_werkzeug_test.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     1717 2021-12-09 16:19:38.467916 cinp-1.3.3/setup.py
```

### Comparing `cinp-1.3.2/PKG-INFO` & `cinp-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cinp
-Version: 1.3.2
+Version: 1.3.3
 Summary: CInP, Concise Interaction Protocol
 Home-page: https://github.com/cinp/python
 Author: Peter Howe
 Author-email: pnhowe@gmail.com
 License: Apache2
 Description: A HTTP/JSON Protocol that brings some of the
         flexability of REST, but extends beyond CRUD to support Metod Calling and
```

### Comparing `cinp-1.3.2/README.rst` & `cinp-1.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `cinp-1.3.2/cinp/client.py` & `cinp-1.3.3/cinp/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import random
 from datetime import datetime
 from tempfile import NamedTemporaryFile
 from urllib import request
 
 from cinp.common import URI
 
-__CLIENT_VERSION__ = '1.3.2'
+__CLIENT_VERSION__ = '1.3.3'
 __CINP_VERSION__ = '1.0'
 
 __all__ = [ 'Timeout', 'ResponseError', 'DetailedInvalidRequest',
             'InvalidRequest', 'InvalidSession', 'NotAuthorized',
             'NotFound', 'ServerError', 'CInP' ]
 
 DELAY_MULTIPLIER = 15
@@ -309,21 +309,20 @@
 
     return ( http_code, data, header_map )
 
   def setAuth( self, auth_id=None, auth_token=None ):
     """
     Sets the Authencation id and token headers, call with out paramaters to remove the headers.
     """
-    if not auth_id:
-      logging.debug( 'cinp: removing auth info' )
-      for index in range( len( self.opener.addheaders ) - 1, -1, -1 ):
-        if self.opener.addheaders[ index ][0] in ( 'Auth-Id', 'Auth-Token' ):
-          del self.opener.addheaders[ index ]
+    logging.debug( 'cinp: removing auth info' )
+    for index in range( len( self.opener.addheaders ) - 1, -1, -1 ):
+      if self.opener.addheaders[ index ][0] in ( 'Auth-Id', 'Auth-Token' ):
+        del self.opener.addheaders[ index ]
 
-    else:
+    if auth_id:
       logging.debug( 'cinp: setting auth info, id "{0}"'.format( auth_id ) )
       self.opener.addheaders += [ ( 'Auth-Id', auth_id ), ( 'Auth-Token', auth_token ) ]
 
   def describe( self, uri, timeout=30, retry_count=0, retry_on=None ):
     """
     DESCRIE
     """
```

### Comparing `cinp-1.3.2/cinp/client_test.py` & `cinp-1.3.3/cinp/client_test.py`

 * *Files identical despite different names*

### Comparing `cinp-1.3.2/cinp/common.py` & `cinp-1.3.3/cinp/common.py`

 * *Files identical despite different names*

### Comparing `cinp-1.3.2/cinp/common_test.py` & `cinp-1.3.3/cinp/common_test.py`

 * *Files identical despite different names*

### Comparing `cinp-1.3.2/cinp/django_file_handler.py` & `cinp-1.3.3/cinp/django_file_handler.py`

 * *Files identical despite different names*

### Comparing `cinp-1.3.2/cinp/orm_django.py` & `cinp-1.3.3/cinp/orm_django.py`

 * *Files identical despite different names*

### Comparing `cinp-1.3.2/cinp/orm_django_test.py` & `cinp-1.3.3/cinp/orm_django_test.py`

 * *Files identical despite different names*

### Comparing `cinp-1.3.2/cinp/orm_null.py` & `cinp-1.3.3/cinp/orm_null.py`

 * *Files identical despite different names*

### Comparing `cinp-1.3.2/cinp/readers.py` & `cinp-1.3.3/cinp/readers.py`

 * *Files identical despite different names*

### Comparing `cinp-1.3.2/cinp/server_common.py` & `cinp-1.3.3/cinp/server_common.py`

 * *Files identical despite different names*

### Comparing `cinp-1.3.2/cinp/server_common_test.py` & `cinp-1.3.3/cinp/server_common_test.py`

 * *Files identical despite different names*

### Comparing `cinp-1.3.2/cinp/server_werkzeug.py` & `cinp-1.3.3/cinp/server_werkzeug.py`

 * *Files identical despite different names*

### Comparing `cinp-1.3.2/cinp/server_werkzeug_test.py` & `cinp-1.3.3/cinp/server_werkzeug_test.py`

 * *Files identical despite different names*

### Comparing `cinp-1.3.2/setup.py` & `cinp-1.3.3/setup.py`

 * *Files identical despite different names*

