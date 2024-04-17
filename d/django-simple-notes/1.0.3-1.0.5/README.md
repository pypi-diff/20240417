# Comparing `tmp/django-simple-notes-1.0.3.tar.gz` & `tmp/django_simple_notes-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-simple-notes-1.0.3.tar", last modified: Thu Apr 11 15:22:16 2024, max compression
+gzip compressed data, was "django_simple_notes-1.0.5.tar", last modified: Wed Apr 17 14:50:05 2024, max compression
```

## Comparing `django-simple-notes-1.0.3.tar` & `django_simple_notes-1.0.5.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-04-11 15:22:16.826783 django-simple-notes-1.0.3/
--rw-r--r--   0 kapt      (1000) kapt      (1000)    35150 2023-05-16 09:56:11.000000 django-simple-notes-1.0.3/LICENSE
--rw-r--r--   0 kapt      (1000) kapt      (1000)      436 2023-10-31 11:01:26.000000 django-simple-notes-1.0.3/MANIFEST.in
--rw-r--r--   0 kapt      (1000) kapt      (1000)    10284 2024-04-11 15:22:16.826783 django-simple-notes-1.0.3/PKG-INFO
--rw-r--r--   0 kapt      (1000) kapt      (1000)     8993 2023-10-30 17:13:10.000000 django-simple-notes-1.0.3/README.md
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-04-11 15:22:16.822782 django-simple-notes-1.0.3/django_simple_notes/
--rw-r--r--   0 kapt      (1000) kapt      (1000)       22 2023-05-16 09:56:11.000000 django-simple-notes-1.0.3/django_simple_notes/__init__.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     3637 2023-10-30 17:11:22.000000 django-simple-notes-1.0.3/django_simple_notes/admin.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)      120 2023-06-20 14:55:55.000000 django-simple-notes-1.0.3/django_simple_notes/apps.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     6665 2024-04-11 15:18:27.000000 django-simple-notes-1.0.3/django_simple_notes/cms_toolbars.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-04-11 15:22:16.822782 django-simple-notes-1.0.3/django_simple_notes/conf/
--rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2023-05-16 09:56:11.000000 django-simple-notes-1.0.3/django_simple_notes/conf/__init__.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)      841 2023-06-20 10:00:04.000000 django-simple-notes-1.0.3/django_simple_notes/conf/settings.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-04-11 15:22:16.818782 django-simple-notes-1.0.3/django_simple_notes/locale/
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-04-11 15:22:16.818782 django-simple-notes-1.0.3/django_simple_notes/locale/fr/
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-04-11 15:22:16.822782 django-simple-notes-1.0.3/django_simple_notes/locale/fr/LC_MESSAGES/
--rw-r--r--   0 kapt      (1000) kapt      (1000)      984 2023-06-20 12:15:22.000000 django-simple-notes-1.0.3/django_simple_notes/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 kapt      (1000) kapt      (1000)     1199 2023-06-20 12:15:14.000000 django-simple-notes-1.0.3/django_simple_notes/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-04-11 15:22:16.826783 django-simple-notes-1.0.3/django_simple_notes/migrations/
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2720 2023-05-23 16:16:32.000000 django-simple-notes-1.0.3/django_simple_notes/migrations/0001_initial.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2017 2023-06-16 10:10:10.000000 django-simple-notes-1.0.3/django_simple_notes/migrations/0002_auto_20230615_1805.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     1508 2023-06-20 15:30:42.000000 django-simple-notes-1.0.3/django_simple_notes/migrations/0003_auto_20230620_1207.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     1236 2023-06-20 15:30:42.000000 django-simple-notes-1.0.3/django_simple_notes/migrations/0004_auto_20230620_1452.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)      858 2023-10-31 10:48:29.000000 django-simple-notes-1.0.3/django_simple_notes/migrations/0005_auto_20231030_1751.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2023-05-16 11:42:48.000000 django-simple-notes-1.0.3/django_simple_notes/migrations/__init__.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2169 2023-10-31 10:48:29.000000 django-simple-notes-1.0.3/django_simple_notes/models.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-04-11 15:22:16.826783 django-simple-notes-1.0.3/django_simple_notes/templatetags/
--rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2023-06-20 14:35:50.000000 django-simple-notes-1.0.3/django_simple_notes/templatetags/__init__.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     1629 2023-07-31 08:15:07.000000 django-simple-notes-1.0.3/django_simple_notes/templatetags/django_simple_notes.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-04-11 15:22:16.826783 django-simple-notes-1.0.3/django_simple_notes.egg-info/
--rw-r--r--   0 kapt      (1000) kapt      (1000)    10284 2024-04-11 15:22:16.000000 django-simple-notes-1.0.3/django_simple_notes.egg-info/PKG-INFO
--rw-r--r--   0 kapt      (1000) kapt      (1000)     1033 2024-04-11 15:22:16.000000 django-simple-notes-1.0.3/django_simple_notes.egg-info/SOURCES.txt
--rw-r--r--   0 kapt      (1000) kapt      (1000)        1 2024-04-11 15:22:16.000000 django-simple-notes-1.0.3/django_simple_notes.egg-info/dependency_links.txt
--rw-r--r--   0 kapt      (1000) kapt      (1000)       74 2024-04-11 15:22:16.000000 django-simple-notes-1.0.3/django_simple_notes.egg-info/requires.txt
--rw-r--r--   0 kapt      (1000) kapt      (1000)       20 2024-04-11 15:22:16.000000 django-simple-notes-1.0.3/django_simple_notes.egg-info/top_level.txt
--rw-r--r--   0 kapt      (1000) kapt      (1000)      642 2023-05-23 16:21:10.000000 django-simple-notes-1.0.3/pyproject.toml
--rw-r--r--   0 kapt      (1000) kapt      (1000)     1252 2024-04-11 15:22:16.826783 django-simple-notes-1.0.3/setup.cfg
--rw-r--r--   0 kapt      (1000) kapt      (1000)       52 2023-05-23 16:22:28.000000 django-simple-notes-1.0.3/setup.py
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-17 14:50:05.479457 django_simple_notes-1.0.5/
+-rw-r--r--   0 kapt       (501) kapt        (20)    35150 2024-04-17 14:30:51.000000 django_simple_notes-1.0.5/LICENSE
+-rw-r--r--   0 kapt       (501) kapt        (20)      436 2024-04-17 14:30:51.000000 django_simple_notes-1.0.5/MANIFEST.in
+-rw-r--r--   0 kapt       (501) kapt        (20)    10284 2024-04-17 14:50:05.479457 django_simple_notes-1.0.5/PKG-INFO
+-rw-r--r--   0 kapt       (501) kapt        (20)     8993 2024-04-17 14:30:51.000000 django_simple_notes-1.0.5/README.md
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-17 14:50:05.472457 django_simple_notes-1.0.5/django_simple_notes/
+-rw-r--r--   0 kapt       (501) kapt        (20)       22 2024-04-17 14:30:51.000000 django_simple_notes-1.0.5/django_simple_notes/__init__.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     3637 2024-04-17 14:30:51.000000 django_simple_notes-1.0.5/django_simple_notes/admin.py
+-rw-r--r--   0 kapt       (501) kapt        (20)      120 2024-04-17 14:30:51.000000 django_simple_notes-1.0.5/django_simple_notes/apps.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     6665 2024-04-17 14:30:51.000000 django_simple_notes-1.0.5/django_simple_notes/cms_toolbars.py
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-17 14:50:05.474457 django_simple_notes-1.0.5/django_simple_notes/conf/
+-rw-r--r--   0 kapt       (501) kapt        (20)        0 2024-04-17 14:30:51.000000 django_simple_notes-1.0.5/django_simple_notes/conf/__init__.py
+-rw-r--r--   0 kapt       (501) kapt        (20)      841 2024-04-17 14:30:51.000000 django_simple_notes-1.0.5/django_simple_notes/conf/settings.py
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-17 14:50:05.465457 django_simple_notes-1.0.5/django_simple_notes/locale/
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-17 14:50:05.467457 django_simple_notes-1.0.5/django_simple_notes/locale/fr/
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-17 14:50:05.474457 django_simple_notes-1.0.5/django_simple_notes/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 kapt       (501) kapt        (20)      984 2024-04-17 14:30:51.000000 django_simple_notes-1.0.5/django_simple_notes/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 kapt       (501) kapt        (20)     1199 2024-04-17 14:30:51.000000 django_simple_notes-1.0.5/django_simple_notes/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-17 14:50:05.478457 django_simple_notes-1.0.5/django_simple_notes/migrations/
+-rw-r--r--   0 kapt       (501) kapt        (20)     2720 2024-04-17 14:30:51.000000 django_simple_notes-1.0.5/django_simple_notes/migrations/0001_initial.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     2017 2024-04-17 14:30:51.000000 django_simple_notes-1.0.5/django_simple_notes/migrations/0002_auto_20230615_1805.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     1508 2024-04-17 14:30:51.000000 django_simple_notes-1.0.5/django_simple_notes/migrations/0003_auto_20230620_1207.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     1236 2024-04-17 14:30:51.000000 django_simple_notes-1.0.5/django_simple_notes/migrations/0004_auto_20230620_1452.py
+-rw-r--r--   0 kapt       (501) kapt        (20)      858 2024-04-17 14:30:51.000000 django_simple_notes-1.0.5/django_simple_notes/migrations/0005_auto_20231030_1751.py
+-rw-r--r--   0 kapt       (501) kapt        (20)      902 2024-04-17 14:40:16.000000 django_simple_notes-1.0.5/django_simple_notes/migrations/0006_auto_20240417_1640.py
+-rw-r--r--   0 kapt       (501) kapt        (20)        0 2024-04-17 14:30:51.000000 django_simple_notes-1.0.5/django_simple_notes/migrations/__init__.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     2166 2024-04-17 14:48:02.000000 django_simple_notes-1.0.5/django_simple_notes/models.py
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-17 14:50:05.479457 django_simple_notes-1.0.5/django_simple_notes/templatetags/
+-rw-r--r--   0 kapt       (501) kapt        (20)        0 2024-04-17 14:30:51.000000 django_simple_notes-1.0.5/django_simple_notes/templatetags/__init__.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     1629 2024-04-17 14:30:51.000000 django_simple_notes-1.0.5/django_simple_notes/templatetags/django_simple_notes.py
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-17 14:50:05.479457 django_simple_notes-1.0.5/django_simple_notes.egg-info/
+-rw-r--r--   0 kapt       (501) kapt        (20)    10284 2024-04-17 14:50:05.000000 django_simple_notes-1.0.5/django_simple_notes.egg-info/PKG-INFO
+-rw-r--r--   0 kapt       (501) kapt        (20)     1091 2024-04-17 14:50:05.000000 django_simple_notes-1.0.5/django_simple_notes.egg-info/SOURCES.txt
+-rw-r--r--   0 kapt       (501) kapt        (20)        1 2024-04-17 14:50:05.000000 django_simple_notes-1.0.5/django_simple_notes.egg-info/dependency_links.txt
+-rw-r--r--   0 kapt       (501) kapt        (20)       74 2024-04-17 14:50:05.000000 django_simple_notes-1.0.5/django_simple_notes.egg-info/requires.txt
+-rw-r--r--   0 kapt       (501) kapt        (20)       20 2024-04-17 14:50:05.000000 django_simple_notes-1.0.5/django_simple_notes.egg-info/top_level.txt
+-rw-r--r--   0 kapt       (501) kapt        (20)      642 2024-04-17 14:30:51.000000 django_simple_notes-1.0.5/pyproject.toml
+-rw-r--r--   0 kapt       (501) kapt        (20)     1252 2024-04-17 14:50:05.480457 django_simple_notes-1.0.5/setup.cfg
+-rw-r--r--   0 kapt       (501) kapt        (20)       52 2024-04-17 14:30:51.000000 django_simple_notes-1.0.5/setup.py
```

### Comparing `django-simple-notes-1.0.3/LICENSE` & `django_simple_notes-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-simple-notes-1.0.3/PKG-INFO` & `django_simple_notes-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-notes
-Version: 1.0.3
+Version: 1.0.5
 Summary: Store simple notes linked to Django(-cms) pages. Supports apphooks (but not custom apps)!
 Home-page: https://gitlab.com/kapt/open-source/django-simple-notes
 Author: Dev Kapt
 Author-email: dev@kapt.mobi
 Project-URL: Documentation, https://gitlab.com/kapt/open-source/django-simple-notes/-/blob/main/README.md
 Project-URL: Release notes, https://gitlab.com/kapt/open-source/django-simple-notes/-/blob/main/CHANGELOG.rst
 Project-URL: Tracker, https://gitlab.com/kapt/open-source/django-simple-notes/-/issues
```

### Comparing `django-simple-notes-1.0.3/README.md` & `django_simple_notes-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `django-simple-notes-1.0.3/django_simple_notes/admin.py` & `django_simple_notes-1.0.5/django_simple_notes/admin.py`

 * *Files identical despite different names*

### Comparing `django-simple-notes-1.0.3/django_simple_notes/cms_toolbars.py` & `django_simple_notes-1.0.5/django_simple_notes/cms_toolbars.py`

 * *Files identical despite different names*

### Comparing `django-simple-notes-1.0.3/django_simple_notes/conf/settings.py` & `django_simple_notes-1.0.5/django_simple_notes/conf/settings.py`

 * *Files identical despite different names*

### Comparing `django-simple-notes-1.0.3/django_simple_notes/locale/fr/LC_MESSAGES/django.mo` & `django_simple_notes-1.0.5/django_simple_notes/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-simple-notes-1.0.3/django_simple_notes/locale/fr/LC_MESSAGES/django.po` & `django_simple_notes-1.0.5/django_simple_notes/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-simple-notes-1.0.3/django_simple_notes/migrations/0001_initial.py` & `django_simple_notes-1.0.5/django_simple_notes/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-simple-notes-1.0.3/django_simple_notes/migrations/0002_auto_20230615_1805.py` & `django_simple_notes-1.0.5/django_simple_notes/migrations/0002_auto_20230615_1805.py`

 * *Files identical despite different names*

### Comparing `django-simple-notes-1.0.3/django_simple_notes/migrations/0003_auto_20230620_1207.py` & `django_simple_notes-1.0.5/django_simple_notes/migrations/0003_auto_20230620_1207.py`

 * *Files identical despite different names*

### Comparing `django-simple-notes-1.0.3/django_simple_notes/migrations/0004_auto_20230620_1452.py` & `django_simple_notes-1.0.5/django_simple_notes/migrations/0004_auto_20230620_1452.py`

 * *Files identical despite different names*

### Comparing `django-simple-notes-1.0.3/django_simple_notes/migrations/0005_auto_20231030_1751.py` & `django_simple_notes-1.0.5/django_simple_notes/migrations/0005_auto_20231030_1751.py`

 * *Files identical despite different names*

### Comparing `django-simple-notes-1.0.3/django_simple_notes/models.py` & `django_simple_notes-1.0.5/django_simple_notes/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         verbose_name = SIMPLE_NOTES_NOTE_ADMIN_NAME
         verbose_name_plural = SIMPLE_NOTES_APP_NAME
 
 
 class SimpleFile(models.Model):
     note = models.ForeignKey(SimpleNote, on_delete=models.CASCADE)
     file = FilerFileField(
-        null=True, blank=True, on_delete=models.DO_NOTHING, verbose_name=("Files")
+        null=True, blank=True, on_delete=models.CASCADE, verbose_name=("Files")
     )
 
     def __str__(self):
         return ""
 
     class Meta:
         verbose_name = _("Extra file")
```

### Comparing `django-simple-notes-1.0.3/django_simple_notes/templatetags/django_simple_notes.py` & `django_simple_notes-1.0.5/django_simple_notes/templatetags/django_simple_notes.py`

 * *Files identical despite different names*

### Comparing `django-simple-notes-1.0.3/django_simple_notes.egg-info/PKG-INFO` & `django_simple_notes-1.0.5/django_simple_notes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-notes
-Version: 1.0.3
+Version: 1.0.5
 Summary: Store simple notes linked to Django(-cms) pages. Supports apphooks (but not custom apps)!
 Home-page: https://gitlab.com/kapt/open-source/django-simple-notes
 Author: Dev Kapt
 Author-email: dev@kapt.mobi
 Project-URL: Documentation, https://gitlab.com/kapt/open-source/django-simple-notes/-/blob/main/README.md
 Project-URL: Release notes, https://gitlab.com/kapt/open-source/django-simple-notes/-/blob/main/CHANGELOG.rst
 Project-URL: Tracker, https://gitlab.com/kapt/open-source/django-simple-notes/-/issues
```

### Comparing `django-simple-notes-1.0.3/django_simple_notes.egg-info/SOURCES.txt` & `django_simple_notes-1.0.5/django_simple_notes.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -19,10 +19,11 @@
 django_simple_notes/locale/fr/LC_MESSAGES/django.mo
 django_simple_notes/locale/fr/LC_MESSAGES/django.po
 django_simple_notes/migrations/0001_initial.py
 django_simple_notes/migrations/0002_auto_20230615_1805.py
 django_simple_notes/migrations/0003_auto_20230620_1207.py
 django_simple_notes/migrations/0004_auto_20230620_1452.py
 django_simple_notes/migrations/0005_auto_20231030_1751.py
+django_simple_notes/migrations/0006_auto_20240417_1640.py
 django_simple_notes/migrations/__init__.py
 django_simple_notes/templatetags/__init__.py
 django_simple_notes/templatetags/django_simple_notes.py
```

### Comparing `django-simple-notes-1.0.3/pyproject.toml` & `django_simple_notes-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-simple-notes-1.0.3/setup.cfg` & `django_simple_notes-1.0.5/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-simple-notes
-version = 1.0.3
+version = 1.0.5
 description = Store simple notes linked to Django(-cms) pages. Supports apphooks (but not custom apps)!
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = django, django-cms
 url = https://gitlab.com/kapt/open-source/django-simple-notes
 project_urls = 
 	Documentation = https://gitlab.com/kapt/open-source/django-simple-notes/-/blob/main/README.md
```

