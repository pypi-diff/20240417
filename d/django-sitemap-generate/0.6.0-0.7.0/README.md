# Comparing `tmp/django-sitemap-generate-0.6.0.tar.gz` & `tmp/django_sitemap_generate-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sitemap-generate-0.6.0.tar", last modified: Sun Aug 21 10:16:05 2022, max compression
+gzip compressed data, was "django_sitemap_generate-0.7.0.tar", last modified: Wed Apr 17 06:49:22 2024, max compression
```

## Comparing `django-sitemap-generate-0.6.0.tar` & `django_sitemap_generate-0.7.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:16:05.300840 django-sitemap-generate-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-08-21 10:15:46.000000 django-sitemap-generate-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6584 2022-08-21 10:16:05.300840 django-sitemap-generate-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5580 2022-08-21 10:15:46.000000 django-sitemap-generate-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:16:05.292840 django-sitemap-generate-0.6.0/django_sitemap_generate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6584 2022-08-21 10:16:05.000000 django-sitemap-generate-0.6.0/django_sitemap_generate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      900 2022-08-21 10:16:05.000000 django-sitemap-generate-0.6.0/django_sitemap_generate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-21 10:16:05.000000 django-sitemap-generate-0.6.0/django_sitemap_generate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-21 10:16:05.000000 django-sitemap-generate-0.6.0/django_sitemap_generate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-08-21 10:16:05.000000 django-sitemap-generate-0.6.0/django_sitemap_generate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-21 10:16:05.300840 django-sitemap-generate-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3002 2022-08-21 10:15:46.000000 django-sitemap-generate-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:16:05.292840 django-sitemap-generate-0.6.0/sitemap_generate/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-21 10:15:46.000000 django-sitemap-generate-0.6.0/sitemap_generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-08-21 10:15:46.000000 django-sitemap-generate-0.6.0/sitemap_generate/defaults.py
--rw-r--r--   0 runner    (1001) docker     (121)     5593 2022-08-21 10:15:46.000000 django-sitemap-generate-0.6.0/sitemap_generate/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:16:05.292840 django-sitemap-generate-0.6.0/sitemap_generate/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-21 10:15:46.000000 django-sitemap-generate-0.6.0/sitemap_generate/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:16:05.292840 django-sitemap-generate-0.6.0/sitemap_generate/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-21 10:15:46.000000 django-sitemap-generate-0.6.0/sitemap_generate/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-08-21 10:15:46.000000 django-sitemap-generate-0.6.0/sitemap_generate/management/commands/generate_sitemap.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:16:05.296840 django-sitemap-generate-0.6.0/testproject/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-21 10:15:46.000000 django-sitemap-generate-0.6.0/testproject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-08-21 10:15:46.000000 django-sitemap-generate-0.6.0/testproject/asgi.py
--rw-r--r--   0 runner    (1001) docker     (121)     3394 2022-08-21 10:15:46.000000 django-sitemap-generate-0.6.0/testproject/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:16:05.296840 django-sitemap-generate-0.6.0/testproject/testapp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-21 10:15:46.000000 django-sitemap-generate-0.6.0/testproject/testapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-08-21 10:15:46.000000 django-sitemap-generate-0.6.0/testproject/testapp/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:16:05.300840 django-sitemap-generate-0.6.0/testproject/testapp/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)      647 2022-08-21 10:15:46.000000 django-sitemap-generate-0.6.0/testproject/testapp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-21 10:15:46.000000 django-sitemap-generate-0.6.0/testproject/testapp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-08-21 10:15:46.000000 django-sitemap-generate-0.6.0/testproject/testapp/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-08-21 10:15:46.000000 django-sitemap-generate-0.6.0/testproject/testapp/sitemaps.py
--rw-r--r--   0 runner    (1001) docker     (121)     4319 2022-08-21 10:15:46.000000 django-sitemap-generate-0.6.0/testproject/testapp/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-08-21 10:15:46.000000 django-sitemap-generate-0.6.0/testproject/testapp/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-08-21 10:15:46.000000 django-sitemap-generate-0.6.0/testproject/testapp/views.py
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-08-21 10:15:46.000000 django-sitemap-generate-0.6.0/testproject/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-08-21 10:15:46.000000 django-sitemap-generate-0.6.0/testproject/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:49:22.533593 django_sitemap_generate-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-17 06:49:14.000000 django_sitemap_generate-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-04-17 06:49:22.533593 django_sitemap_generate-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-04-17 06:49:14.000000 django_sitemap_generate-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:49:22.533593 django_sitemap_generate-0.7.0/django_sitemap_generate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-04-17 06:49:22.000000 django_sitemap_generate-0.7.0/django_sitemap_generate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-17 06:49:22.000000 django_sitemap_generate-0.7.0/django_sitemap_generate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:49:22.000000 django_sitemap_generate-0.7.0/django_sitemap_generate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-17 06:49:22.000000 django_sitemap_generate-0.7.0/django_sitemap_generate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-17 06:49:22.000000 django_sitemap_generate-0.7.0/django_sitemap_generate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 06:49:22.533593 django_sitemap_generate-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-17 06:49:14.000000 django_sitemap_generate-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:49:22.533593 django_sitemap_generate-0.7.0/sitemap_generate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:49:14.000000 django_sitemap_generate-0.7.0/sitemap_generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-17 06:49:14.000000 django_sitemap_generate-0.7.0/sitemap_generate/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-17 06:49:14.000000 django_sitemap_generate-0.7.0/sitemap_generate/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:49:22.533593 django_sitemap_generate-0.7.0/sitemap_generate/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:49:14.000000 django_sitemap_generate-0.7.0/sitemap_generate/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:49:22.533593 django_sitemap_generate-0.7.0/sitemap_generate/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:49:14.000000 django_sitemap_generate-0.7.0/sitemap_generate/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-17 06:49:14.000000 django_sitemap_generate-0.7.0/sitemap_generate/management/commands/generate_sitemap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:49:22.533593 django_sitemap_generate-0.7.0/testproject/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:49:14.000000 django_sitemap_generate-0.7.0/testproject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-17 06:49:14.000000 django_sitemap_generate-0.7.0/testproject/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-17 06:49:14.000000 django_sitemap_generate-0.7.0/testproject/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:49:22.533593 django_sitemap_generate-0.7.0/testproject/testapp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:49:14.000000 django_sitemap_generate-0.7.0/testproject/testapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-17 06:49:14.000000 django_sitemap_generate-0.7.0/testproject/testapp/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:49:22.533593 django_sitemap_generate-0.7.0/testproject/testapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-17 06:49:14.000000 django_sitemap_generate-0.7.0/testproject/testapp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:49:14.000000 django_sitemap_generate-0.7.0/testproject/testapp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-17 06:49:14.000000 django_sitemap_generate-0.7.0/testproject/testapp/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-17 06:49:14.000000 django_sitemap_generate-0.7.0/testproject/testapp/sitemaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-04-17 06:49:14.000000 django_sitemap_generate-0.7.0/testproject/testapp/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-17 06:49:14.000000 django_sitemap_generate-0.7.0/testproject/testapp/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-17 06:49:14.000000 django_sitemap_generate-0.7.0/testproject/testapp/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-17 06:49:14.000000 django_sitemap_generate-0.7.0/testproject/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-17 06:49:14.000000 django_sitemap_generate-0.7.0/testproject/wsgi.py
```

### Comparing `django-sitemap-generate-0.6.0/LICENSE` & `django_sitemap_generate-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-sitemap-generate-0.6.0/PKG-INFO` & `django_sitemap_generate-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: django-sitemap-generate
-Version: 0.6.0
+Version: 0.7.0
 Summary: Background sitemap generation for Django
 Home-page: https://github.com/just-work/django-sitemap-generate
 Author: Sergey Tikhonov
 Author-email: zimbler@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Django<5.1,>=3.2
 
 Django Sitemap Generate
 =======================
 
 Background sitemap generation for Django.
 
 [![Build Status](https://github.com/just-work/django-sitemap-generate/workflows/build/badge.svg?branch=master&event=push)](https://github.com/just-work/django-sitemap-generate/actions?query=event%3Apush+branch%3Amaster+workflow%3Abuild)
```

### Comparing `django-sitemap-generate-0.6.0/README.md` & `django_sitemap_generate-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `django-sitemap-generate-0.6.0/django_sitemap_generate.egg-info/PKG-INFO` & `django_sitemap_generate-0.7.0/django_sitemap_generate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: django-sitemap-generate
-Version: 0.6.0
+Version: 0.7.0
 Summary: Background sitemap generation for Django
 Home-page: https://github.com/just-work/django-sitemap-generate
 Author: Sergey Tikhonov
 Author-email: zimbler@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Django<5.1,>=3.2
 
 Django Sitemap Generate
 =======================
 
 Background sitemap generation for Django.
 
 [![Build Status](https://github.com/just-work/django-sitemap-generate/workflows/build/badge.svg?branch=master&event=push)](https://github.com/just-work/django-sitemap-generate/actions?query=event%3Apush+branch%3Amaster+workflow%3Abuild)
```

### Comparing `django-sitemap-generate-0.6.0/django_sitemap_generate.egg-info/SOURCES.txt` & `django_sitemap_generate-0.7.0/django_sitemap_generate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-sitemap-generate-0.6.0/setup.py` & `django_sitemap_generate-0.7.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,39 +55,36 @@
             version = None
 
     return version
 
 
 setup(
     name='django-sitemap-generate',
-    version=get_version() or 'dev',
+    version=get_version() or '9999999',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     include_package_data=True,
     url='https://github.com/just-work/django-sitemap-generate',
     license='MIT',
     author='Sergey Tikhonov',
     author_email='zimbler@gmail.com',
     description='Background sitemap generation for Django',
     install_requires=[
-        'Django>=2.2,<4.2',
+        'Django>=3.2,<5.1',
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Console',
-        'Framework :: Django :: 2.2',
-        'Framework :: Django :: 3.0',
-        'Framework :: Django :: 3.1',
         'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
-        'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
+        'Framework :: Django :: 5.0',
         'Operating System :: POSIX',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         ('Topic :: Internet :: WWW/HTTP :: Dynamic Content :: '
          'Content Management System'),
     ]
 )
```

### Comparing `django-sitemap-generate-0.6.0/sitemap_generate/defaults.py` & `django_sitemap_generate-0.7.0/sitemap_generate/defaults.py`

 * *Files identical despite different names*

### Comparing `django-sitemap-generate-0.6.0/sitemap_generate/generator.py` & `django_sitemap_generate-0.7.0/sitemap_generate/generator.py`

 * *Files identical despite different names*

### Comparing `django-sitemap-generate-0.6.0/testproject/settings.py` & `django_sitemap_generate-0.7.0/testproject/settings.py`

 * *Files identical despite different names*

### Comparing `django-sitemap-generate-0.6.0/testproject/testapp/migrations/0001_initial.py` & `django_sitemap_generate-0.7.0/testproject/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-sitemap-generate-0.6.0/testproject/testapp/tests.py` & `django_sitemap_generate-0.7.0/testproject/testapp/tests.py`

 * *Files identical despite different names*

### Comparing `django-sitemap-generate-0.6.0/testproject/urls.py` & `django_sitemap_generate-0.7.0/testproject/urls.py`

 * *Files identical despite different names*

