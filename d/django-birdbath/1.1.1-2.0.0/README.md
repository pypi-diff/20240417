# Comparing `tmp/django-birdbath-1.1.1.tar.gz` & `tmp/django-birdbath-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-birdbath-1.1.1.tar", last modified: Mon Dec 18 11:58:50 2023, max compression
+gzip compressed data, was "django-birdbath-2.0.0.tar", last modified: Wed Apr 17 11:10:37 2024, max compression
```

## Comparing `django-birdbath-1.1.1.tar` & `django-birdbath-2.0.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-18 11:58:50.823680 django-birdbath-1.1.1/
--rw-r--r--   0 tom        (501) staff       (20)      872 2023-12-18 11:55:58.000000 django-birdbath-1.1.1/CHANGELOG.md
--rw-r--r--   0 tom        (501) staff       (20)      110 2023-12-18 11:55:07.000000 django-birdbath-1.1.1/MANIFEST.in
--rw-r--r--   0 tom        (501) staff       (20)     7476 2023-12-18 11:58:50.823585 django-birdbath-1.1.1/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     7064 2023-12-18 11:55:07.000000 django-birdbath-1.1.1/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-18 11:58:50.819423 django-birdbath-1.1.1/birdbath/
--rw-r--r--   0 tom        (501) staff       (20)       52 2023-12-18 11:55:07.000000 django-birdbath-1.1.1/birdbath/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      217 2023-12-18 11:55:07.000000 django-birdbath-1.1.1/birdbath/apps.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-18 11:58:50.819819 django-birdbath-1.1.1/birdbath/checks/
--rw-r--r--   0 tom        (501) staff       (20)       53 2023-12-18 11:55:07.000000 django-birdbath-1.1.1/birdbath/checks/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)       72 2023-12-18 11:55:07.000000 django-birdbath-1.1.1/birdbath/checks/base.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-18 11:58:50.820161 django-birdbath-1.1.1/birdbath/checks/contrib/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-12-18 11:55:07.000000 django-birdbath-1.1.1/birdbath/checks/contrib/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      504 2023-12-18 11:55:07.000000 django-birdbath-1.1.1/birdbath/checks/contrib/heroku.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-18 11:58:50.820342 django-birdbath-1.1.1/birdbath/management/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-12-18 11:55:07.000000 django-birdbath-1.1.1/birdbath/management/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-18 11:58:50.820560 django-birdbath-1.1.1/birdbath/management/commands/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-12-18 11:55:07.000000 django-birdbath-1.1.1/birdbath/management/commands/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1753 2023-12-18 11:55:07.000000 django-birdbath-1.1.1/birdbath/management/commands/run_birdbath.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-18 11:58:50.820899 django-birdbath-1.1.1/birdbath/migrations/
--rw-r--r--   0 tom        (501) staff       (20)      628 2023-12-18 11:55:07.000000 django-birdbath-1.1.1/birdbath/migrations/0001_initial.py
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-12-18 11:55:07.000000 django-birdbath-1.1.1/birdbath/migrations/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      122 2023-12-18 11:55:07.000000 django-birdbath-1.1.1/birdbath/models.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-18 11:58:50.821376 django-birdbath-1.1.1/birdbath/processors/
--rw-r--r--   0 tom        (501) staff       (20)      225 2023-12-18 11:55:07.000000 django-birdbath-1.1.1/birdbath/processors/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     7222 2023-12-18 11:55:07.000000 django-birdbath-1.1.1/birdbath/processors/base.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-18 11:58:50.821661 django-birdbath-1.1.1/birdbath/processors/contrib/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-12-18 11:55:07.000000 django-birdbath-1.1.1/birdbath/processors/contrib/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      364 2023-12-18 11:55:07.000000 django-birdbath-1.1.1/birdbath/processors/contrib/wagtail.py
--rw-r--r--   0 tom        (501) staff       (20)     1013 2023-12-18 11:55:07.000000 django-birdbath-1.1.1/birdbath/processors/users.py
--rw-r--r--   0 tom        (501) staff       (20)      721 2023-12-18 11:55:07.000000 django-birdbath-1.1.1/birdbath/settings.py
--rw-r--r--   0 tom        (501) staff       (20)     1276 2023-12-18 11:55:07.000000 django-birdbath-1.1.1/birdbath/system_checks.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-18 11:58:50.822602 django-birdbath-1.1.1/django_birdbath.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)     7476 2023-12-18 11:58:50.000000 django-birdbath-1.1.1/django_birdbath.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      827 2023-12-18 11:58:50.000000 django-birdbath-1.1.1/django_birdbath.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-12-18 11:58:50.000000 django-birdbath-1.1.1/django_birdbath.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)       58 2023-12-18 11:58:50.000000 django-birdbath-1.1.1/django_birdbath.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)        9 2023-12-18 11:58:50.000000 django-birdbath-1.1.1/django_birdbath.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)      885 2023-12-18 11:58:50.824120 django-birdbath-1.1.1/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-12-18 11:55:07.000000 django-birdbath-1.1.1/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-17 11:10:37.305973 django-birdbath-2.0.0/
+-rw-r--r--   0 tom        (501) staff       (20)     1001 2024-04-17 11:04:53.000000 django-birdbath-2.0.0/CHANGELOG.md
+-rw-r--r--   0 tom        (501) staff       (20)      110 2023-12-18 11:55:07.000000 django-birdbath-2.0.0/MANIFEST.in
+-rw-r--r--   0 tom        (501) staff       (20)     7476 2024-04-17 11:10:37.305894 django-birdbath-2.0.0/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     7064 2023-12-18 11:55:07.000000 django-birdbath-2.0.0/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-17 11:10:37.301654 django-birdbath-2.0.0/birdbath/
+-rw-r--r--   0 tom        (501) staff       (20)       52 2023-12-18 11:55:07.000000 django-birdbath-2.0.0/birdbath/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      217 2023-12-18 11:55:07.000000 django-birdbath-2.0.0/birdbath/apps.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-17 11:10:37.302084 django-birdbath-2.0.0/birdbath/checks/
+-rw-r--r--   0 tom        (501) staff       (20)       53 2023-12-18 11:55:07.000000 django-birdbath-2.0.0/birdbath/checks/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)       72 2023-12-18 11:55:07.000000 django-birdbath-2.0.0/birdbath/checks/base.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-17 11:10:37.302386 django-birdbath-2.0.0/birdbath/checks/contrib/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-12-18 11:55:07.000000 django-birdbath-2.0.0/birdbath/checks/contrib/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      504 2023-12-18 11:55:07.000000 django-birdbath-2.0.0/birdbath/checks/contrib/heroku.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-17 11:10:37.302568 django-birdbath-2.0.0/birdbath/management/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-12-18 11:55:07.000000 django-birdbath-2.0.0/birdbath/management/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-17 11:10:37.302809 django-birdbath-2.0.0/birdbath/management/commands/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-12-18 11:55:07.000000 django-birdbath-2.0.0/birdbath/management/commands/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1753 2023-12-18 11:55:07.000000 django-birdbath-2.0.0/birdbath/management/commands/run_birdbath.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-17 11:10:37.303147 django-birdbath-2.0.0/birdbath/migrations/
+-rw-r--r--   0 tom        (501) staff       (20)      628 2023-12-18 11:55:07.000000 django-birdbath-2.0.0/birdbath/migrations/0001_initial.py
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-12-18 11:55:07.000000 django-birdbath-2.0.0/birdbath/migrations/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      122 2023-12-18 11:55:07.000000 django-birdbath-2.0.0/birdbath/models.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-17 11:10:37.303686 django-birdbath-2.0.0/birdbath/processors/
+-rw-r--r--   0 tom        (501) staff       (20)      225 2023-12-18 11:55:07.000000 django-birdbath-2.0.0/birdbath/processors/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     7222 2023-12-18 11:55:07.000000 django-birdbath-2.0.0/birdbath/processors/base.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-17 11:10:37.304006 django-birdbath-2.0.0/birdbath/processors/contrib/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-12-18 11:55:07.000000 django-birdbath-2.0.0/birdbath/processors/contrib/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      383 2024-04-17 11:04:02.000000 django-birdbath-2.0.0/birdbath/processors/contrib/wagtail.py
+-rw-r--r--   0 tom        (501) staff       (20)     1013 2023-12-18 11:55:07.000000 django-birdbath-2.0.0/birdbath/processors/users.py
+-rw-r--r--   0 tom        (501) staff       (20)      721 2023-12-18 11:55:07.000000 django-birdbath-2.0.0/birdbath/settings.py
+-rw-r--r--   0 tom        (501) staff       (20)     1276 2023-12-18 11:55:07.000000 django-birdbath-2.0.0/birdbath/system_checks.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-17 11:10:37.305215 django-birdbath-2.0.0/django_birdbath.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)     7476 2024-04-17 11:10:37.000000 django-birdbath-2.0.0/django_birdbath.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      827 2024-04-17 11:10:37.000000 django-birdbath-2.0.0/django_birdbath.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2024-04-17 11:10:37.000000 django-birdbath-2.0.0/django_birdbath.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)       58 2024-04-17 11:10:37.000000 django-birdbath-2.0.0/django_birdbath.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)        9 2024-04-17 11:10:37.000000 django-birdbath-2.0.0/django_birdbath.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)      885 2024-04-17 11:10:37.306317 django-birdbath-2.0.0/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-12-18 11:55:07.000000 django-birdbath-2.0.0/setup.py
```

### Comparing `django-birdbath-1.1.1/CHANGELOG.md` & `django-birdbath-2.0.0/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # CHANGELOG
 
+## v2.0.0 (2024-04-17)
+
+- Updates imports for compatibility with Wagtail >= 5.0, drops compatibility for older Wagtail releases
+
 ## v1.1.1 (2023-12-18)
 
 - Remove upper bound on Faker dependency
 
 ## v1.1.0 (2023-02-20)
 
 - Add black, flake8 and isort and fix all associated errors
```

### Comparing `django-birdbath-1.1.1/PKG-INFO` & `django-birdbath-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-birdbath
-Version: 1.1.1
+Version: 2.0.0
 Home-page: https://git.torchbox.com/internal/django-birdbath
 Author: Torchbox
 Author-email: info@torchbox.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: Faker>=8
 Provides-Extra: dev
```

### Comparing `django-birdbath-1.1.1/README.md` & `django-birdbath-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `django-birdbath-1.1.1/birdbath/management/commands/run_birdbath.py` & `django-birdbath-2.0.0/birdbath/management/commands/run_birdbath.py`

 * *Files identical despite different names*

### Comparing `django-birdbath-1.1.1/birdbath/migrations/0001_initial.py` & `django-birdbath-2.0.0/birdbath/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-birdbath-1.1.1/birdbath/processors/base.py` & `django-birdbath-2.0.0/birdbath/processors/base.py`

 * *Files identical despite different names*

### Comparing `django-birdbath-1.1.1/birdbath/processors/users.py` & `django-birdbath-2.0.0/birdbath/processors/users.py`

 * *Files identical despite different names*

### Comparing `django-birdbath-1.1.1/birdbath/settings.py` & `django-birdbath-2.0.0/birdbath/settings.py`

 * *Files identical despite different names*

### Comparing `django-birdbath-1.1.1/birdbath/system_checks.py` & `django-birdbath-2.0.0/birdbath/system_checks.py`

 * *Files identical despite different names*

### Comparing `django-birdbath-1.1.1/django_birdbath.egg-info/PKG-INFO` & `django-birdbath-2.0.0/django_birdbath.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-birdbath
-Version: 1.1.1
+Version: 2.0.0
 Home-page: https://git.torchbox.com/internal/django-birdbath
 Author: Torchbox
 Author-email: info@torchbox.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: Faker>=8
 Provides-Extra: dev
```

### Comparing `django-birdbath-1.1.1/django_birdbath.egg-info/SOURCES.txt` & `django-birdbath-2.0.0/django_birdbath.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-birdbath-1.1.1/setup.cfg` & `django-birdbath-2.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-birdbath
-version = 1.1.1
+version = 2.0.0
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Torchbox
 author_email = info@torchbox.com
 url = https://git.torchbox.com/internal/django-birdbath
 
 [options]
```

