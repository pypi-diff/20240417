# Comparing `tmp/django_tailwindcss_automated-0.8.tar.gz` & `tmp/django_tailwindcss_automated-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tailwindcss_automated-0.8.tar", last modified: Wed Apr 17 17:22:08 2024, max compression
+gzip compressed data, was "django_tailwindcss_automated-0.9.tar", last modified: Wed Apr 17 17:36:11 2024, max compression
```

## Comparing `django_tailwindcss_automated-0.8.tar` & `django_tailwindcss_automated-0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:22:08.709477 django_tailwindcss_automated-0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-17 17:22:08.709477 django_tailwindcss_automated-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-17 17:22:03.000000 django_tailwindcss_automated-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:22:08.709477 django_tailwindcss_automated-0.8/django_tailwindcss_automated/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 17:22:03.000000 django_tailwindcss_automated-0.8/django_tailwindcss_automated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6909 2024-04-17 17:22:03.000000 django_tailwindcss_automated-0.8/django_tailwindcss_automated/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:22:08.709477 django_tailwindcss_automated-0.8/django_tailwindcss_automated.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-17 17:22:08.000000 django_tailwindcss_automated-0.8/django_tailwindcss_automated.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-17 17:22:08.000000 django_tailwindcss_automated-0.8/django_tailwindcss_automated.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 17:22:08.000000 django_tailwindcss_automated-0.8/django_tailwindcss_automated.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-17 17:22:08.000000 django_tailwindcss_automated-0.8/django_tailwindcss_automated.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-17 17:22:08.000000 django_tailwindcss_automated-0.8/django_tailwindcss_automated.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 17:22:08.709477 django_tailwindcss_automated-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-17 17:22:03.000000 django_tailwindcss_automated-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:36:11.015528 django_tailwindcss_automated-0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-17 17:36:11.015528 django_tailwindcss_automated-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-17 17:36:06.000000 django_tailwindcss_automated-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:36:11.015528 django_tailwindcss_automated-0.9/django_tailwindcss_automated/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 17:36:06.000000 django_tailwindcss_automated-0.9/django_tailwindcss_automated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6909 2024-04-17 17:36:06.000000 django_tailwindcss_automated-0.9/django_tailwindcss_automated/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:36:11.015528 django_tailwindcss_automated-0.9/django_tailwindcss_automated.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-17 17:36:10.000000 django_tailwindcss_automated-0.9/django_tailwindcss_automated.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-17 17:36:11.000000 django_tailwindcss_automated-0.9/django_tailwindcss_automated.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 17:36:10.000000 django_tailwindcss_automated-0.9/django_tailwindcss_automated.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-17 17:36:10.000000 django_tailwindcss_automated-0.9/django_tailwindcss_automated.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-17 17:36:10.000000 django_tailwindcss_automated-0.9/django_tailwindcss_automated.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 17:36:11.019528 django_tailwindcss_automated-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-17 17:36:06.000000 django_tailwindcss_automated-0.9/setup.py
```

### Comparing `django_tailwindcss_automated-0.8/PKG-INFO` & `django_tailwindcss_automated-0.9/django_tailwindcss_automated.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: django_tailwindcss_automated
-Version: 0.8
+Name: django-tailwindcss-automated
+Version: 0.9
 Summary: Handles all setup and configuration automatically.
 Home-page: UNKNOWN
 Author: Jan Leander
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django_tailwindcss_automated Version: 0.8 Summary:
+Metadata-Version: 2.1 Name: django-tailwindcss-automated Version: 0.9 Summary:
 Handles all setup and configuration automatically. Home-page: UNKNOWN Author:
 Jan Leander License: UNKNOWN Platform: UNKNOWN Description-Content-Type: text/
 markdown Automated Project Initialization ððð --- An automated setup
 for Django project with Tailwind. Handles all setup and configuration
 automatically.â¨ https://pypi.org/project/django-tailwindcss-automated/
 _[_h_t_t_p_s_:_/_/_s_k_i_l_l_i_c_o_n_s_._d_e_v_/_i_c_o_n_s_?_i_=_d_j_a_n_g_o_,_t_a_i_l_w_i_n_d_c_s_s_,_p_y_t_h_o_n_]
 ## Getting Started ð - ð Before you dive in, make sure that you have
```

### Comparing `django_tailwindcss_automated-0.8/README.md` & `django_tailwindcss_automated-0.9/README.md`

 * *Files identical despite different names*

### Comparing `django_tailwindcss_automated-0.8/django_tailwindcss_automated/main.py` & `django_tailwindcss_automated-0.9/django_tailwindcss_automated/main.py`

 * *Files identical despite different names*

### Comparing `django_tailwindcss_automated-0.8/django_tailwindcss_automated.egg-info/PKG-INFO` & `django_tailwindcss_automated-0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: django-tailwindcss-automated
-Version: 0.8
+Name: django_tailwindcss_automated
+Version: 0.9
 Summary: Handles all setup and configuration automatically.
 Home-page: UNKNOWN
 Author: Jan Leander
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-tailwindcss-automated Version: 0.8 Summary:
+Metadata-Version: 2.1 Name: django_tailwindcss_automated Version: 0.9 Summary:
 Handles all setup and configuration automatically. Home-page: UNKNOWN Author:
 Jan Leander License: UNKNOWN Platform: UNKNOWN Description-Content-Type: text/
 markdown Automated Project Initialization ððð --- An automated setup
 for Django project with Tailwind. Handles all setup and configuration
 automatically.â¨ https://pypi.org/project/django-tailwindcss-automated/
 _[_h_t_t_p_s_:_/_/_s_k_i_l_l_i_c_o_n_s_._d_e_v_/_i_c_o_n_s_?_i_=_d_j_a_n_g_o_,_t_a_i_l_w_i_n_d_c_s_s_,_p_y_t_h_o_n_]
 ## Getting Started ð - ð Before you dive in, make sure that you have
```

### Comparing `django_tailwindcss_automated-0.8/setup.py` & `django_tailwindcss_automated-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name='django_tailwindcss_automated',
     description="Handles all setup and configuration automatically.",
-    version='0.8',
+    version='0.9',
     author='Jan Leander',
     packages=find_packages(),
     install_requires=[
         # add dependencies here.
         # e.g 'num>=1.11.1'
     ],
     entry_points={
```

