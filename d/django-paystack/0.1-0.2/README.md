# Comparing `tmp/django-paystack-0.1.tar.gz` & `tmp/django_paystack-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-paystack-0.1.tar", last modified: Wed Apr 17 13:28:19 2024, max compression
+gzip compressed data, was "django_paystack-0.2.tar", last modified: Wed Apr 17 15:08:13 2024, max compression
```

## Comparing `django-paystack-0.1.tar` & `django_paystack-0.2.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxr-xr-x   0 nonso      (501) staff       (20)        0 2024-04-17 13:28:19.523212 django-paystack-0.1/
--rw-r--r--   0 nonso      (501) staff       (20)      142 2024-04-17 13:18:56.000000 django-paystack-0.1/MANIFEST.in
--rw-r--r--   0 nonso      (501) staff       (20)     1717 2024-04-17 13:28:19.523120 django-paystack-0.1/PKG-INFO
--rw-r--r--   0 nonso      (501) staff       (20)      678 2024-04-17 13:18:56.000000 django-paystack-0.1/README.rst
-drwxr-xr-x   0 nonso      (501) staff       (20)        0 2024-04-17 13:28:19.519312 django-paystack-0.1/django_paystack/
--rw-r--r--   0 nonso      (501) staff       (20)        0 2024-04-17 12:19:45.000000 django-paystack-0.1/django_paystack/__init__.py
--rw-r--r--   0 nonso      (501) staff       (20)       63 2024-04-17 12:19:45.000000 django-paystack-0.1/django_paystack/admin.py
--rw-r--r--   0 nonso      (501) staff       (20)      104 2024-04-17 12:19:45.000000 django-paystack-0.1/django_paystack/apps.py
--rw-r--r--   0 nonso      (501) staff       (20)     1769 2024-04-17 13:04:26.000000 django-paystack-0.1/django_paystack/base.py
-drwxr-xr-x   0 nonso      (501) staff       (20)        0 2024-04-17 13:28:19.520408 django-paystack-0.1/django_paystack/migrations/
--rw-r--r--   0 nonso      (501) staff       (20)        0 2024-04-17 12:19:45.000000 django-paystack-0.1/django_paystack/migrations/__init__.py
--rw-r--r--   0 nonso      (501) staff       (20)       57 2024-04-17 12:19:45.000000 django-paystack-0.1/django_paystack/models.py
--rw-r--r--   0 nonso      (501) staff       (20)      201 2024-04-17 12:52:21.000000 django-paystack-0.1/django_paystack/signals.py
-drwxr-xr-x   0 nonso      (501) staff       (20)        0 2024-04-17 13:28:19.521012 django-paystack-0.1/django_paystack/templatetags/
--rw-r--r--   0 nonso      (501) staff       (20)        0 2024-04-17 12:52:08.000000 django-paystack-0.1/django_paystack/templatetags/__init__.py
--rw-r--r--   0 nonso      (501) staff       (20)     1406 2024-04-17 12:52:08.000000 django-paystack-0.1/django_paystack/templatetags/base.py
--rw-r--r--   0 nonso      (501) staff       (20)     1292 2024-04-17 13:02:12.000000 django-paystack-0.1/django_paystack/templatetags/paystack.py
--rw-r--r--   0 nonso      (501) staff       (20)       60 2024-04-17 12:19:45.000000 django-paystack-0.1/django_paystack/tests.py
--rw-r--r--   0 nonso      (501) staff       (20)      773 2024-04-17 13:02:51.000000 django-paystack-0.1/django_paystack/urls.py
--rw-r--r--   0 nonso      (501) staff       (20)     1394 2024-04-17 12:53:26.000000 django-paystack-0.1/django_paystack/views.py
-drwxr-xr-x   0 nonso      (501) staff       (20)        0 2024-04-17 13:28:19.522722 django-paystack-0.1/django_paystack.egg-info/
--rw-r--r--   0 nonso      (501) staff       (20)     1717 2024-04-17 13:28:19.000000 django-paystack-0.1/django_paystack.egg-info/PKG-INFO
--rw-r--r--   0 nonso      (501) staff       (20)      729 2024-04-17 13:28:19.000000 django-paystack-0.1/django_paystack.egg-info/SOURCES.txt
--rw-r--r--   0 nonso      (501) staff       (20)        1 2024-04-17 13:28:19.000000 django-paystack-0.1/django_paystack.egg-info/dependency_links.txt
--rw-r--r--   0 nonso      (501) staff       (20)       31 2024-04-17 13:28:19.000000 django-paystack-0.1/django_paystack.egg-info/requires.txt
--rw-r--r--   0 nonso      (501) staff       (20)       25 2024-04-17 13:28:19.000000 django-paystack-0.1/django_paystack.egg-info/top_level.txt
-drwxr-xr-x   0 nonso      (501) staff       (20)        0 2024-04-17 13:28:19.522298 django-paystack-0.1/payments/
--rw-r--r--   0 nonso      (501) staff       (20)        0 2024-04-17 12:18:18.000000 django-paystack-0.1/payments/__init__.py
--rw-r--r--   0 nonso      (501) staff       (20)      393 2024-04-17 12:18:18.000000 django-paystack-0.1/payments/asgi.py
--rw-r--r--   0 nonso      (501) staff       (20)     3460 2024-04-17 12:59:19.000000 django-paystack-0.1/payments/settings.py
--rw-r--r--   0 nonso      (501) staff       (20)      800 2024-04-17 12:59:57.000000 django-paystack-0.1/payments/urls.py
--rw-r--r--   0 nonso      (501) staff       (20)      393 2024-04-17 12:18:18.000000 django-paystack-0.1/payments/wsgi.py
--rw-r--r--   0 nonso      (501) staff       (20)       88 2024-04-17 13:18:56.000000 django-paystack-0.1/pyproject.toml
--rw-r--r--   0 nonso      (501) staff       (20)     1020 2024-04-17 13:28:19.523665 django-paystack-0.1/setup.cfg
--rw-r--r--   0 nonso      (501) staff       (20)       37 2024-04-17 13:18:56.000000 django-paystack-0.1/setup.py
+drwxr-xr-x   0 nonso      (501) staff       (20)        0 2024-04-17 15:08:13.091140 django_paystack-0.2/
+-rw-r--r--   0 nonso      (501) staff       (20)     1047 2024-04-17 13:33:02.000000 django_paystack-0.2/LICENSE
+-rw-r--r--   0 nonso      (501) staff       (20)      148 2024-04-17 14:38:12.000000 django_paystack-0.2/MANIFEST.in
+-rw-r--r--   0 nonso      (501) staff       (20)     1719 2024-04-17 15:08:13.091058 django_paystack-0.2/PKG-INFO
+-rw-r--r--   0 nonso      (501) staff       (20)      678 2024-04-17 13:18:56.000000 django_paystack-0.2/README.rst
+drwxr-xr-x   0 nonso      (501) staff       (20)        0 2024-04-17 15:08:13.085919 django_paystack-0.2/django_paystack/
+-rw-r--r--   0 nonso      (501) staff       (20)        0 2024-04-17 12:19:45.000000 django_paystack-0.2/django_paystack/__init__.py
+-rw-r--r--   0 nonso      (501) staff       (20)       63 2024-04-17 12:19:45.000000 django_paystack-0.2/django_paystack/admin.py
+-rw-r--r--   0 nonso      (501) staff       (20)      134 2024-04-17 14:06:22.000000 django_paystack-0.2/django_paystack/apps.py
+-rw-r--r--   0 nonso      (501) staff       (20)     1769 2024-04-17 13:04:26.000000 django_paystack-0.2/django_paystack/base.py
+-rw-r--r--   0 nonso      (501) staff       (20)       57 2024-04-17 12:19:45.000000 django_paystack-0.2/django_paystack/models.py
+-rw-r--r--   0 nonso      (501) staff       (20)      201 2024-04-17 12:52:21.000000 django_paystack-0.2/django_paystack/signals.py
+drwxr-xr-x   0 nonso      (501) staff       (20)        0 2024-04-17 15:08:13.081953 django_paystack-0.2/django_paystack/templates/
+drwxr-xr-x   0 nonso      (501) staff       (20)        0 2024-04-17 15:08:13.087742 django_paystack-0.2/django_paystack/templates/django_paystack/
+-rw-r--r--   0 nonso      (501) staff       (20)      943 2024-04-17 12:54:27.000000 django_paystack-0.2/django_paystack/templates/django_paystack/paystack_button.html
+-rw-r--r--   0 nonso      (501) staff       (20)      460 2024-04-17 12:54:44.000000 django_paystack-0.2/django_paystack/templates/django_paystack/sample.htmx
+drwxr-xr-x   0 nonso      (501) staff       (20)        0 2024-04-17 15:08:13.088580 django_paystack-0.2/django_paystack/templatetags/
+-rw-r--r--   0 nonso      (501) staff       (20)        0 2024-04-17 12:52:08.000000 django_paystack-0.2/django_paystack/templatetags/__init__.py
+-rw-r--r--   0 nonso      (501) staff       (20)     1406 2024-04-17 12:52:08.000000 django_paystack-0.2/django_paystack/templatetags/base.py
+-rw-r--r--   0 nonso      (501) staff       (20)     1292 2024-04-17 13:02:12.000000 django_paystack-0.2/django_paystack/templatetags/paystack.py
+-rw-r--r--   0 nonso      (501) staff       (20)       60 2024-04-17 12:19:45.000000 django_paystack-0.2/django_paystack/tests.py
+-rw-r--r--   0 nonso      (501) staff       (20)      773 2024-04-17 13:02:51.000000 django_paystack-0.2/django_paystack/urls.py
+-rw-r--r--   0 nonso      (501) staff       (20)     1394 2024-04-17 12:53:26.000000 django_paystack-0.2/django_paystack/views.py
+drwxr-xr-x   0 nonso      (501) staff       (20)        0 2024-04-17 15:08:13.090650 django_paystack-0.2/django_paystack.egg-info/
+-rw-r--r--   0 nonso      (501) staff       (20)     1719 2024-04-17 15:08:13.000000 django_paystack-0.2/django_paystack.egg-info/PKG-INFO
+-rw-r--r--   0 nonso      (501) staff       (20)      835 2024-04-17 15:08:13.000000 django_paystack-0.2/django_paystack.egg-info/SOURCES.txt
+-rw-r--r--   0 nonso      (501) staff       (20)        1 2024-04-17 15:08:13.000000 django_paystack-0.2/django_paystack.egg-info/dependency_links.txt
+-rw-r--r--   0 nonso      (501) staff       (20)       31 2024-04-17 15:08:13.000000 django_paystack-0.2/django_paystack.egg-info/requires.txt
+-rw-r--r--   0 nonso      (501) staff       (20)       29 2024-04-17 15:08:13.000000 django_paystack-0.2/django_paystack.egg-info/top_level.txt
+-rw-r--r--   0 nonso      (501) staff       (20)       88 2024-04-17 13:18:56.000000 django_paystack-0.2/pyproject.toml
+-rw-r--r--   0 nonso      (501) staff       (20)     1000 2024-04-17 15:08:13.091651 django_paystack-0.2/setup.cfg
+-rw-r--r--   0 nonso      (501) staff       (20)       37 2024-04-17 13:18:56.000000 django_paystack-0.2/setup.py
+drwxr-xr-x   0 nonso      (501) staff       (20)        0 2024-04-17 15:08:13.090117 django_paystack-0.2/test_project/
+-rw-r--r--   0 nonso      (501) staff       (20)        0 2024-04-17 12:18:18.000000 django_paystack-0.2/test_project/__init__.py
+-rw-r--r--   0 nonso      (501) staff       (20)      393 2024-04-17 12:18:18.000000 django_paystack-0.2/test_project/asgi.py
+-rw-r--r--   0 nonso      (501) staff       (20)     3460 2024-04-17 12:59:19.000000 django_paystack-0.2/test_project/settings.py
+-rw-r--r--   0 nonso      (501) staff       (20)      800 2024-04-17 12:59:57.000000 django_paystack-0.2/test_project/urls.py
+-rw-r--r--   0 nonso      (501) staff       (20)      393 2024-04-17 12:18:18.000000 django_paystack-0.2/test_project/wsgi.py
```

### Comparing `django-paystack-0.1/PKG-INFO` & `django_paystack-0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: django-paystack
-Version: 0.1
+Version: 0.2
 Summary: A Simple Payment wrapper for the Paystack package for the Django Framework
 Home-page: https://github.com/KingNonso/django-paystack
 Author: Chinonso Ani
 Author-email: achinonso@gmail.com
-License: BSD-3-Clause  # Example license
+License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.10
+License-File: LICENSE
 Requires-Dist: Django>=3.2
 Requires-Dist: pypaystack2==2.0.3
 
 ============
 django-polls
 ============
```

### Comparing `django-paystack-0.1/README.rst` & `django_paystack-0.2/README.rst`

 * *Files identical despite different names*

### Comparing `django-paystack-0.1/django_paystack/base.py` & `django_paystack-0.2/django_paystack/base.py`

 * *Files identical despite different names*

### Comparing `django-paystack-0.1/django_paystack/templatetags/base.py` & `django_paystack-0.2/django_paystack/templatetags/base.py`

 * *Files identical despite different names*

### Comparing `django-paystack-0.1/django_paystack/templatetags/paystack.py` & `django_paystack-0.2/django_paystack/templatetags/paystack.py`

 * *Files identical despite different names*

### Comparing `django-paystack-0.1/django_paystack/urls.py` & `django_paystack-0.2/django_paystack/urls.py`

 * *Files identical despite different names*

### Comparing `django-paystack-0.1/django_paystack/views.py` & `django_paystack-0.2/django_paystack/views.py`

 * *Files identical despite different names*

### Comparing `django-paystack-0.1/django_paystack.egg-info/PKG-INFO` & `django_paystack-0.2/django_paystack.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: django-paystack
-Version: 0.1
+Version: 0.2
 Summary: A Simple Payment wrapper for the Paystack package for the Django Framework
 Home-page: https://github.com/KingNonso/django-paystack
 Author: Chinonso Ani
 Author-email: achinonso@gmail.com
-License: BSD-3-Clause  # Example license
+License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.10
+License-File: LICENSE
 Requires-Dist: Django>=3.2
 Requires-Dist: pypaystack2==2.0.3
 
 ============
 django-polls
 ============
```

### Comparing `django-paystack-0.1/django_paystack.egg-info/SOURCES.txt` & `django_paystack-0.2/django_paystack.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 django_paystack/__init__.py
 django_paystack/admin.py
@@ -13,16 +14,17 @@
 django_paystack/urls.py
 django_paystack/views.py
 django_paystack.egg-info/PKG-INFO
 django_paystack.egg-info/SOURCES.txt
 django_paystack.egg-info/dependency_links.txt
 django_paystack.egg-info/requires.txt
 django_paystack.egg-info/top_level.txt
-django_paystack/migrations/__init__.py
+django_paystack/templates/django_paystack/paystack_button.html
+django_paystack/templates/django_paystack/sample.htmx
 django_paystack/templatetags/__init__.py
 django_paystack/templatetags/base.py
 django_paystack/templatetags/paystack.py
-payments/__init__.py
-payments/asgi.py
-payments/settings.py
-payments/urls.py
-payments/wsgi.py
+test_project/__init__.py
+test_project/asgi.py
+test_project/settings.py
+test_project/urls.py
+test_project/wsgi.py
```

### Comparing `django-paystack-0.1/payments/settings.py` & `django_paystack-0.2/test_project/settings.py`

 * *Files identical despite different names*

### Comparing `django-paystack-0.1/payments/urls.py` & `django_paystack-0.2/test_project/urls.py`

 * *Files identical despite different names*

### Comparing `django-paystack-0.1/setup.cfg` & `django_paystack-0.2/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [metadata]
 name = django-paystack
-version = 0.1
+version = 0.2
 description = A Simple Payment wrapper for the Paystack package for the Django Framework
 long_description = file: README.rst
 url = https://github.com/KingNonso/django-paystack
 author = Chinonso Ani
 author_email = achinonso@gmail.com
-license = BSD-3-Clause  # Example license
+license = MIT License
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 3.2
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
```

