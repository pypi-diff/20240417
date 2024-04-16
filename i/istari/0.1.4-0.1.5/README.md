# Comparing `tmp/istari-0.1.4.tar.gz` & `tmp/istari-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istari-0.1.4.tar", last modified: Wed Apr 10 20:33:33 2024, max compression
+gzip compressed data, was "istari-0.1.5.tar", last modified: Tue Apr 16 23:20:25 2024, max compression
```

## Comparing `istari-0.1.4.tar` & `istari-0.1.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-10 20:33:33.247547 istari-0.1.4/
--rw-r--r--   0 jay        (501) staff       (20)      114 2024-04-10 20:33:33.247294 istari-0.1.4/PKG-INFO
--rw-r--r--   0 jay        (501) staff       (20)        9 2024-04-05 20:19:27.000000 istari-0.1.4/README.md
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-10 20:33:33.244092 istari-0.1.4/istari/
--rw-r--r--   0 jay        (501) staff       (20)       22 2024-04-10 20:33:18.000000 istari-0.1.4/istari/__init__.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-10 20:33:33.244848 istari-0.1.4/istari/admin/
--rw-r--r--   0 jay        (501) staff       (20)     1661 2024-04-09 21:28:02.000000 istari-0.1.4/istari/admin/__init__.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-10 20:33:33.245085 istari-0.1.4/istari/auth/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 03:18:29.000000 istari-0.1.4/istari/auth/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     3043 2024-04-06 04:11:49.000000 istari-0.1.4/istari/auth/models.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-10 20:33:33.245299 istari-0.1.4/istari/cli/
--rw-r--r--   0 jay        (501) staff       (20)     2246 2024-04-07 03:00:00.000000 istari-0.1.4/istari/cli/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)      282 2024-04-05 20:45:04.000000 istari-0.1.4/istari/cli/base.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-10 20:33:33.245812 istari-0.1.4/istari/commands/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 00:32:25.000000 istari-0.1.4/istari/commands/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)      601 2024-04-10 20:32:30.000000 istari-0.1.4/istari/commands/freeze.py
--rw-r--r--   0 jay        (501) staff       (20)     2339 2024-04-09 21:32:52.000000 istari-0.1.4/istari/commands/startapp.py
--rw-r--r--   0 jay        (501) staff       (20)      775 2024-04-07 03:12:41.000000 istari-0.1.4/istari/commands/startproject.py
--rw-r--r--   0 jay        (501) staff       (20)      117 2024-04-07 03:09:41.000000 istari-0.1.4/istari/constants.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-10 20:33:33.246122 istari-0.1.4/istari/db/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 00:36:56.000000 istari-0.1.4/istari/db/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     1221 2024-04-06 00:37:44.000000 istari-0.1.4/istari/db/fields.py
--rw-r--r--   0 jay        (501) staff       (20)     1307 2024-04-09 21:23:29.000000 istari-0.1.4/istari/db/models.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-10 20:33:33.246307 istari-0.1.4/istari/templates/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 21:01:40.000000 istari-0.1.4/istari/templates/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     4412 2024-04-08 18:29:39.000000 istari-0.1.4/istari/templates/commands.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-10 20:33:33.246833 istari-0.1.4/istari/templates/plugins/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 21:22:01.000000 istari-0.1.4/istari/templates/plugins/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     1045 2024-04-09 02:44:58.000000 istari-0.1.4/istari/templates/plugins/base.py
--rw-r--r--   0 jay        (501) staff       (20)     1344 2024-04-09 02:35:05.000000 istari-0.1.4/istari/templates/plugins/defaultuser.py
--rw-r--r--   0 jay        (501) staff       (20)     1100 2024-04-09 03:00:11.000000 istari-0.1.4/istari/templates/plugins/drf.py
--rw-r--r--   0 jay        (501) staff       (20)     1194 2024-04-09 03:01:28.000000 istari-0.1.4/istari/templates/plugins/editable.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-10 20:33:33.247013 istari-0.1.4/istari/utils/
--rw-r--r--   0 jay        (501) staff       (20)      298 2024-04-07 03:12:18.000000 istari-0.1.4/istari/utils/__init__.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-10 20:33:33.247111 istari-0.1.4/istari/utils/io/
--rw-r--r--   0 jay        (501) staff       (20)     1438 2024-04-09 03:00:36.000000 istari-0.1.4/istari/utils/io/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)      359 2024-04-10 15:58:42.000000 istari-0.1.4/istari/utils/shell.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-10 20:33:33.244710 istari-0.1.4/istari.egg-info/
--rw-r--r--   0 jay        (501) staff       (20)      114 2024-04-10 20:33:33.000000 istari-0.1.4/istari.egg-info/PKG-INFO
--rw-r--r--   0 jay        (501) staff       (20)      811 2024-04-10 20:33:33.000000 istari-0.1.4/istari.egg-info/SOURCES.txt
--rw-r--r--   0 jay        (501) staff       (20)        1 2024-04-10 20:33:33.000000 istari-0.1.4/istari.egg-info/dependency_links.txt
--rw-r--r--   0 jay        (501) staff       (20)       43 2024-04-10 20:33:33.000000 istari-0.1.4/istari.egg-info/entry_points.txt
--rw-r--r--   0 jay        (501) staff       (20)        7 2024-04-10 20:33:33.000000 istari-0.1.4/istari.egg-info/top_level.txt
--rw-r--r--   0 jay        (501) staff       (20)       38 2024-04-10 20:33:33.247583 istari-0.1.4/setup.cfg
--rw-r--r--   0 jay        (501) staff       (20)      462 2024-04-05 20:34:04.000000 istari-0.1.4/setup.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-16 23:20:25.745206 istari-0.1.5/
+-rw-r--r--   0 jay        (501) staff       (20)      114 2024-04-16 23:20:25.744971 istari-0.1.5/PKG-INFO
+-rw-r--r--   0 jay        (501) staff       (20)        9 2024-04-05 20:19:27.000000 istari-0.1.5/README.md
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-16 23:20:25.741679 istari-0.1.5/istari/
+-rw-r--r--   0 jay        (501) staff       (20)       22 2024-04-16 23:17:11.000000 istari-0.1.5/istari/__init__.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-16 23:20:25.742653 istari-0.1.5/istari/admin/
+-rw-r--r--   0 jay        (501) staff       (20)     1661 2024-04-09 21:28:02.000000 istari-0.1.5/istari/admin/__init__.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-16 23:20:25.742842 istari-0.1.5/istari/auth/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 03:18:29.000000 istari-0.1.5/istari/auth/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     3043 2024-04-06 04:11:49.000000 istari-0.1.5/istari/auth/models.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-16 23:20:25.743026 istari-0.1.5/istari/cli/
+-rw-r--r--   0 jay        (501) staff       (20)     2246 2024-04-07 03:00:00.000000 istari-0.1.5/istari/cli/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)      282 2024-04-05 20:45:04.000000 istari-0.1.5/istari/cli/base.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-16 23:20:25.743448 istari-0.1.5/istari/commands/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 00:32:25.000000 istari-0.1.5/istari/commands/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)      601 2024-04-10 20:32:30.000000 istari-0.1.5/istari/commands/freeze.py
+-rw-r--r--   0 jay        (501) staff       (20)     2339 2024-04-09 21:32:52.000000 istari-0.1.5/istari/commands/startapp.py
+-rw-r--r--   0 jay        (501) staff       (20)      775 2024-04-07 03:12:41.000000 istari-0.1.5/istari/commands/startproject.py
+-rw-r--r--   0 jay        (501) staff       (20)      117 2024-04-07 03:09:41.000000 istari-0.1.5/istari/constants.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-16 23:20:25.743720 istari-0.1.5/istari/db/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 00:36:56.000000 istari-0.1.5/istari/db/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     1240 2024-04-16 23:17:04.000000 istari-0.1.5/istari/db/fields.py
+-rw-r--r--   0 jay        (501) staff       (20)     1307 2024-04-09 21:23:29.000000 istari-0.1.5/istari/db/models.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-16 23:20:25.743887 istari-0.1.5/istari/templates/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 21:01:40.000000 istari-0.1.5/istari/templates/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     4412 2024-04-08 18:29:39.000000 istari-0.1.5/istari/templates/commands.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-16 23:20:25.744383 istari-0.1.5/istari/templates/plugins/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 21:22:01.000000 istari-0.1.5/istari/templates/plugins/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     1045 2024-04-09 02:44:58.000000 istari-0.1.5/istari/templates/plugins/base.py
+-rw-r--r--   0 jay        (501) staff       (20)     1344 2024-04-09 02:35:05.000000 istari-0.1.5/istari/templates/plugins/defaultuser.py
+-rw-r--r--   0 jay        (501) staff       (20)     1100 2024-04-09 03:00:11.000000 istari-0.1.5/istari/templates/plugins/drf.py
+-rw-r--r--   0 jay        (501) staff       (20)     1194 2024-04-09 03:01:28.000000 istari-0.1.5/istari/templates/plugins/editable.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-16 23:20:25.744637 istari-0.1.5/istari/utils/
+-rw-r--r--   0 jay        (501) staff       (20)      298 2024-04-07 03:12:18.000000 istari-0.1.5/istari/utils/__init__.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-16 23:20:25.744752 istari-0.1.5/istari/utils/io/
+-rw-r--r--   0 jay        (501) staff       (20)     1438 2024-04-09 03:00:36.000000 istari-0.1.5/istari/utils/io/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)      359 2024-04-10 15:58:42.000000 istari-0.1.5/istari/utils/shell.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-16 23:20:25.742317 istari-0.1.5/istari.egg-info/
+-rw-r--r--   0 jay        (501) staff       (20)      114 2024-04-16 23:20:25.000000 istari-0.1.5/istari.egg-info/PKG-INFO
+-rw-r--r--   0 jay        (501) staff       (20)      811 2024-04-16 23:20:25.000000 istari-0.1.5/istari.egg-info/SOURCES.txt
+-rw-r--r--   0 jay        (501) staff       (20)        1 2024-04-16 23:20:25.000000 istari-0.1.5/istari.egg-info/dependency_links.txt
+-rw-r--r--   0 jay        (501) staff       (20)       43 2024-04-16 23:20:25.000000 istari-0.1.5/istari.egg-info/entry_points.txt
+-rw-r--r--   0 jay        (501) staff       (20)        7 2024-04-16 23:20:25.000000 istari-0.1.5/istari.egg-info/top_level.txt
+-rw-r--r--   0 jay        (501) staff       (20)       38 2024-04-16 23:20:25.745235 istari-0.1.5/setup.cfg
+-rw-r--r--   0 jay        (501) staff       (20)      462 2024-04-05 20:34:04.000000 istari-0.1.5/setup.py
```

### Comparing `istari-0.1.4/istari/admin/__init__.py` & `istari-0.1.5/istari/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.4/istari/auth/models.py` & `istari-0.1.5/istari/auth/models.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.4/istari/cli/__init__.py` & `istari-0.1.5/istari/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.4/istari/commands/freeze.py` & `istari-0.1.5/istari/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.4/istari/commands/startapp.py` & `istari-0.1.5/istari/commands/startapp.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.4/istari/commands/startproject.py` & `istari-0.1.5/istari/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.4/istari/db/fields.py` & `istari-0.1.5/istari/db/fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class AutoLastModifiedField(models.DateTimeField):
     def __init__(self, *args, **kwargs):
         kwargs.setdefault('auto_now', True)
         super().__init__(*args, **kwargs)
 
 
 class UUIDField(models.UUIDField):
-    def __init__(self, primary_key=False, version=4, editable=False, *args, **kwargs):
+    def __init__(self, verbose_name=None, primary_key=False, version=4, editable=False, **kwargs):
         if version == 2:
             raise ValidationError('UUID version 2 is not supported.')
         
         if version < 1 or version > 5:
             raise ValidationError('UUID version is not valid.')
         
         if version == 1:
@@ -31,8 +31,8 @@
             default = uuid.uuid4
         elif version == 5:
             default == uuid.uuid5
 
         kwargs.setdefault('primary_key', primary_key)
         kwargs.setdefault('default', default)
         kwargs.setdefault('editable', editable)
-        super().__init__(*args, **kwargs)
+        super().__init__(verbose_name, **kwargs)
```

### Comparing `istari-0.1.4/istari/db/models.py` & `istari-0.1.5/istari/db/models.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.4/istari/templates/commands.py` & `istari-0.1.5/istari/templates/commands.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.4/istari/templates/plugins/base.py` & `istari-0.1.5/istari/templates/plugins/base.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.4/istari/templates/plugins/defaultuser.py` & `istari-0.1.5/istari/templates/plugins/defaultuser.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.4/istari/templates/plugins/drf.py` & `istari-0.1.5/istari/templates/plugins/drf.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.4/istari/templates/plugins/editable.py` & `istari-0.1.5/istari/templates/plugins/editable.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.4/istari/utils/io/__init__.py` & `istari-0.1.5/istari/utils/io/__init__.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.4/istari.egg-info/SOURCES.txt` & `istari-0.1.5/istari.egg-info/SOURCES.txt`

 * *Files identical despite different names*

