# Comparing `tmp/rahavard-0.0.14.tar.gz` & `tmp/rahavard-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rahavard-0.0.14.tar", last modified: Wed Apr 17 19:37:18 2024, max compression
+gzip compressed data, was "rahavard-0.0.9.tar", last modified: Thu Mar 21 13:06:07 2024, max compression
```

## Comparing `rahavard-0.0.14.tar` & `rahavard-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-04-17 19:37:18.385841 rahavard-0.0.14/
--rw-r--r--   0 nino      (1000) nino      (1000)     1072 2024-03-20 17:42:50.000000 rahavard-0.0.14/LICENSE
--rw-r--r--   0 nino      (1000) nino      (1000)      699 2024-04-17 19:37:18.385841 rahavard-0.0.14/PKG-INFO
--rw-r--r--   0 nino      (1000) nino      (1000)       93 2024-03-20 17:41:56.000000 rahavard-0.0.14/README.md
-drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-04-17 19:37:18.382507 rahavard-0.0.14/rahavard/
--rw-r--r--   0 nino      (1000) nino      (1000)      379 2024-04-17 19:36:01.000000 rahavard-0.0.14/rahavard/__init__.py
--rw-r--r--   0 nino      (1000) nino      (1000)     9279 2024-04-17 19:34:24.000000 rahavard-0.0.14/rahavard/utils.py
-drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-04-17 19:37:18.385841 rahavard-0.0.14/rahavard.egg-info/
--rw-r--r--   0 nino      (1000) nino      (1000)      699 2024-04-17 19:37:18.000000 rahavard-0.0.14/rahavard.egg-info/PKG-INFO
--rw-r--r--   0 nino      (1000) nino      (1000)      224 2024-04-17 19:37:18.000000 rahavard-0.0.14/rahavard.egg-info/SOURCES.txt
--rw-r--r--   0 nino      (1000) nino      (1000)        1 2024-04-17 19:37:18.000000 rahavard-0.0.14/rahavard.egg-info/dependency_links.txt
--rw-r--r--   0 nino      (1000) nino      (1000)       34 2024-04-17 19:37:18.000000 rahavard-0.0.14/rahavard.egg-info/requires.txt
--rw-r--r--   0 nino      (1000) nino      (1000)        9 2024-04-17 19:37:18.000000 rahavard-0.0.14/rahavard.egg-info/top_level.txt
--rw-r--r--   0 nino      (1000) nino      (1000)       38 2024-04-17 19:37:18.385841 rahavard-0.0.14/setup.cfg
--rw-r--r--   0 nino      (1000) nino      (1000)     1182 2024-04-17 19:36:31.000000 rahavard-0.0.14/setup.py
+drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-03-21 13:06:07.104723 rahavard-0.0.9/
+-rw-r--r--   0 nino      (1000) nino      (1000)     1072 2024-03-20 17:42:50.000000 rahavard-0.0.9/LICENSE
+-rw-r--r--   0 nino      (1000) nino      (1000)      698 2024-03-21 13:06:07.104723 rahavard-0.0.9/PKG-INFO
+-rw-r--r--   0 nino      (1000) nino      (1000)       93 2024-03-20 17:41:56.000000 rahavard-0.0.9/README.md
+drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-03-21 13:06:07.101390 rahavard-0.0.9/rahavard/
+-rw-r--r--   0 nino      (1000) nino      (1000)      333 2024-03-21 10:39:33.000000 rahavard-0.0.9/rahavard/__init__.py
+-rw-r--r--   0 nino      (1000) nino      (1000)     7560 2024-03-21 13:03:58.000000 rahavard-0.0.9/rahavard/utils.py
+drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-03-21 13:06:07.104723 rahavard-0.0.9/rahavard.egg-info/
+-rw-r--r--   0 nino      (1000) nino      (1000)      698 2024-03-21 13:06:07.000000 rahavard-0.0.9/rahavard.egg-info/PKG-INFO
+-rw-r--r--   0 nino      (1000) nino      (1000)      224 2024-03-21 13:06:07.000000 rahavard-0.0.9/rahavard.egg-info/SOURCES.txt
+-rw-r--r--   0 nino      (1000) nino      (1000)        1 2024-03-21 13:06:07.000000 rahavard-0.0.9/rahavard.egg-info/dependency_links.txt
+-rw-r--r--   0 nino      (1000) nino      (1000)       34 2024-03-21 13:06:07.000000 rahavard-0.0.9/rahavard.egg-info/requires.txt
+-rw-r--r--   0 nino      (1000) nino      (1000)        9 2024-03-21 13:06:07.000000 rahavard-0.0.9/rahavard.egg-info/top_level.txt
+-rw-r--r--   0 nino      (1000) nino      (1000)       38 2024-03-21 13:06:07.104723 rahavard-0.0.9/setup.cfg
+-rw-r--r--   0 nino      (1000) nino      (1000)     1181 2024-03-21 13:05:38.000000 rahavard-0.0.9/setup.py
```

### Comparing `rahavard-0.0.14/LICENSE` & `rahavard-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rahavard-0.0.14/PKG-INFO` & `rahavard-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rahavard
-Version: 0.0.14
+Version: 0.0.9
 Summary: Re-Usable Utils
 Author: Davoud Arsalani
 Author-email: d_arsalani@yahoo.com
 Keywords: python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rahavard-0.0.14/rahavard/utils.py` & `rahavard-0.0.9/rahavard/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from django.http import HttpResponse
-
 from math import floor, log as math_log, pow as math_pow
 from os import path, listdir, getenv
 from re import match, sub
 from uuid import uuid4
 
 from convert_numbers import english_to_persian
 from jdatetime import datetime as jdt
@@ -62,21 +60,21 @@
 def convert_second(seconds, verbose=True):
     seconds = int(seconds)
 
     if seconds == 0:
         if verbose:
             return '0'
         else:
-            return '0:00'
+            return '0:00:00'
 
     if seconds < 1:
         if verbose:
             return '~0'
         else:
-            return '~0:00'
+            return '~0:00:00'
 
     ss = f'{int(seconds % 60):02}'
     mi = f'{int(seconds / 60 % 60):02}'
     hh = f'{int(seconds / 3600 % 24):02}'
     dd = f'{int(seconds / 3600 / 24 % 30):02}'
     mo = f'{int(seconds / 3600 / 24 / 30 % 12):02}'
     yy = f'{int(seconds / 3600 / 24 / 30 / 12):02}'
@@ -160,32 +158,14 @@
     return f'{w} {english_to_persian(h)}:{english_to_persian(mi)}:{english_to_persian(s)} {english_to_persian(y)}/{english_to_persian(mo)}/{english_to_persian(d)}'
 
 
 def convert_to_second(date_obj):
     return int(date_obj.timestamp())  ## 1698381096
 
 
-def get_date_time_live():
-    jdatetime.set_locale('fa_IR')
-
-    jdt_now = jdt.now()
-
-    _year  = english_to_persian(jdt_now.strftime('%Y'))  ## ۱۴۰۱
-    _day   = english_to_persian(jdt_now.strftime('%d'))  ## ۱۷
-    _month = english_to_persian(jdt_now.strftime('%m'))  ## ۰۱
-
-    _hour = english_to_persian(jdt_now.strftime('%H'))
-    _min  = english_to_persian(jdt_now.strftime('%M'))
-    # _sec  = english_to_persian(jdt_now.strftime('%S'))
-
-    # _weekday = jdt_now.strftime('%A')  ## چهارشنبه
-
-    return HttpResponse(f'{_year}/{_month}/{_day} {_hour}:{_min}')
-
-
 def get_list_of_files(directory, extension):
     if not path.exists(directory):
         return []
     return natsorted([
         path.abspath(path.join(directory, _))
         for _ in listdir(directory)
         if all([
@@ -199,15 +179,15 @@
     return conn.execute(f'''
         SELECT MAX(id) FROM "{table_name}";
     ''').fetchone()[0] \
     or 0  ## added 'or 0' because max id may sometimes be None
 
 
 def get_percent(smaller_number, total_number, to_persian=False):
-    if smaller_number == 0 or total_number == 0:
+    if smaller_number == 0:
         if to_persian:
             return '۰'
         return '0'
 
     _perc = (smaller_number * 100) / total_number
 
     if int(_perc) == 0:
@@ -222,59 +202,17 @@
     _perc = sub('\.0+$', '', str(_perc))  ## 97.0 -> 97
 
     if to_persian:
         return persianize(_perc)
 
     return _perc
 
-## inspired by:
-## https://stackoverflow.com/questions/50319819/separate-thousands-while-typing-in-farsipersian
-def intcomma_persian(num):
-    '''
-        ۱۲۳۴۵۶۷۸    -> ۱۲،۳۴۵،۶۷۸
-        ۱۲۳۴۵۶۷۸.۶۷ -> ۱۲،۳۴۵،۶۷۸.۶۷
-        ۱۲۳۴۵۶۷۸/۶۷ -> ۱۲،۳۴۵،۶۷۸/۶۷
-    '''
-
-    commad = ''
-    left = ''
-    right = ''
-    is_float = False
-
-    ## JUMP_1 is float
-    if match('^[۱۲۳۴۵۶۷۸۹۰]+\.[۱۲۳۴۵۶۷۸۹۰]+$', num):
-        left, right = num.split('.')
-        separator = '.'
-        is_float = True
-
-    ## JUMP_1 is float
-    elif match('^[۱۲۳۴۵۶۷۸۹۰]+\/[۱۲۳۴۵۶۷۸۹۰]+$', num):
-        left, right = num.split('/')
-        separator = '/'
-        is_float = True
-
-    else:
-        left = num
-
-
-    for idx, char in enumerate(reversed(left), start=0):
-        if idx % 3 == 0 and idx > 0:
-            commad = char + '،' + commad
-        else:
-            commad = char + commad
-
-    if is_float:
-        commad = f'{commad}{separator}{right}'
-
-    return commad
 
 def persianize(number):
     number = str(number)
-
-    ## JUMP_1 is float
     if match('^[0-9]+\.[0-9]+$', number):
         _left, _right = number.split('.')
         if match('^0+$', _right):
             return english_to_persian(_left)
         return f'{english_to_persian(_left)}.{english_to_persian(_right[:2])}'
 
     return english_to_persian(int(number))
@@ -294,7 +232,9 @@
 
     return dictionary
 
 
 def to_tilda(text):
     '''/home/USERNAME/... -> ~/...'''
     return sub(getenv('HOME'), '~', text)
+
+
```

### Comparing `rahavard-0.0.14/rahavard.egg-info/PKG-INFO` & `rahavard-0.0.9/rahavard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rahavard
-Version: 0.0.14
+Version: 0.0.9
 Summary: Re-Usable Utils
 Author: Davoud Arsalani
 Author-email: d_arsalani@yahoo.com
 Keywords: python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rahavard-0.0.14/setup.py` & `rahavard-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 here = path.abspath(path.dirname(__file__))
 with codecs.open(path.join(here, 'README.md'), encoding='utf-8') as opened:
     long_description = '\n' + opened.read()
 
 
-VERSION = '0.0.14'
+VERSION = '0.0.9'
 DESCRIPTION = 'Re-Usable Utils'
 LONG_DESCRIPTION = 'Re-Usable Utils to Be Used on Our Django Projects'
 
 setup(
     name='rahavard',
     version=VERSION,
     author='Davoud Arsalani',
```

