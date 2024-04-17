# Comparing `tmp/django_tailwindcss_automated-0.7.tar.gz` & `tmp/django_tailwindcss_automated-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tailwindcss_automated-0.7.tar", last modified: Tue Apr 16 19:57:49 2024, max compression
+gzip compressed data, was "django_tailwindcss_automated-0.8.tar", last modified: Wed Apr 17 17:22:08 2024, max compression
```

## Comparing `django_tailwindcss_automated-0.7.tar` & `django_tailwindcss_automated-0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 19:57:49.432738 django_tailwindcss_automated-0.7/
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)     1227 2024-04-16 19:57:49.432738 django_tailwindcss_automated-0.7/PKG-INFO
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      980 2024-04-16 19:54:24.000000 django_tailwindcss_automated-0.7/README.md
-drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 19:57:49.420735 django_tailwindcss_automated-0.7/django_tailwindcss_automated/
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       37 2024-04-16 17:36:26.000000 django_tailwindcss_automated-0.7/django_tailwindcss_automated/__init__.py
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)     6909 2024-04-16 17:47:37.000000 django_tailwindcss_automated-0.7/django_tailwindcss_automated/main.py
-drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 19:57:49.432738 django_tailwindcss_automated-0.7/django_tailwindcss_automated.egg-info/
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)     1227 2024-04-16 19:57:47.000000 django_tailwindcss_automated-0.7/django_tailwindcss_automated.egg-info/PKG-INFO
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      359 2024-04-16 19:57:47.000000 django_tailwindcss_automated-0.7/django_tailwindcss_automated.egg-info/SOURCES.txt
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)        1 2024-04-16 19:57:47.000000 django_tailwindcss_automated-0.7/django_tailwindcss_automated.egg-info/dependency_links.txt
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       64 2024-04-16 19:57:47.000000 django_tailwindcss_automated-0.7/django_tailwindcss_automated.egg-info/entry_points.txt
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       29 2024-04-16 19:57:47.000000 django_tailwindcss_automated-0.7/django_tailwindcss_automated.egg-info/top_level.txt
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       38 2024-04-16 19:57:49.432738 django_tailwindcss_automated-0.7/setup.cfg
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      604 2024-04-16 19:54:18.000000 django_tailwindcss_automated-0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:22:08.709477 django_tailwindcss_automated-0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-17 17:22:08.709477 django_tailwindcss_automated-0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-17 17:22:03.000000 django_tailwindcss_automated-0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:22:08.709477 django_tailwindcss_automated-0.8/django_tailwindcss_automated/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 17:22:03.000000 django_tailwindcss_automated-0.8/django_tailwindcss_automated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6909 2024-04-17 17:22:03.000000 django_tailwindcss_automated-0.8/django_tailwindcss_automated/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:22:08.709477 django_tailwindcss_automated-0.8/django_tailwindcss_automated.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-17 17:22:08.000000 django_tailwindcss_automated-0.8/django_tailwindcss_automated.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-17 17:22:08.000000 django_tailwindcss_automated-0.8/django_tailwindcss_automated.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 17:22:08.000000 django_tailwindcss_automated-0.8/django_tailwindcss_automated.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-17 17:22:08.000000 django_tailwindcss_automated-0.8/django_tailwindcss_automated.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-17 17:22:08.000000 django_tailwindcss_automated-0.8/django_tailwindcss_automated.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 17:22:08.709477 django_tailwindcss_automated-0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-17 17:22:03.000000 django_tailwindcss_automated-0.8/setup.py
```

### Comparing `django_tailwindcss_automated-0.7/PKG-INFO` & `django_tailwindcss_automated-0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: django_tailwindcss_automated
-Version: 0.7
+Version: 0.8
 Summary: Handles all setup and configuration automatically.
 Home-page: UNKNOWN
 Author: Jan Leander
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 Automated Project Initialization 🐍💚💙 
 ---
 An automated setup for Django project with Tailwind. Handles all setup and configuration automatically.✨
 
+https://pypi.org/project/django-tailwindcss-automated/
+
 <p align="left">
   <a href="https://skillicons.dev">
     <img src="https://skillicons.dev/icons?i=django,tailwindcss,python" />
   </a>
 </p>
 
 ## Getting Started 💙
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: django_tailwindcss_automated Version: 0.7 Summary:
+Metadata-Version: 2.1 Name: django_tailwindcss_automated Version: 0.8 Summary:
 Handles all setup and configuration automatically. Home-page: UNKNOWN Author:
 Jan Leander License: UNKNOWN Platform: UNKNOWN Description-Content-Type: text/
 markdown Automated Project Initialization ððð --- An automated setup
 for Django project with Tailwind. Handles all setup and configuration
-automatically.â¨
+automatically.â¨ https://pypi.org/project/django-tailwindcss-automated/
 _[_h_t_t_p_s_:_/_/_s_k_i_l_l_i_c_o_n_s_._d_e_v_/_i_c_o_n_s_?_i_=_d_j_a_n_g_o_,_t_a_i_l_w_i_n_d_c_s_s_,_p_y_t_h_o_n_]
 ## Getting Started ð - ð Before you dive in, make sure that you have
 Node.js, Git, and Python installed on your computer. - Create a folder for your
 Django project. ## Install the Package Open your terminal and install the
 package using pip: ```bash pip install django_tailwindcss_automated ``` ## Run
 the Script In your terminal, run the following script to automate the setup:
 ```bash automate ``` ## Start the Development Server Open another terminal and
```

### Comparing `django_tailwindcss_automated-0.7/README.md` & `django_tailwindcss_automated-0.8/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Automated Project Initialization 🐍💚💙 
 ---
 An automated setup for Django project with Tailwind. Handles all setup and configuration automatically.✨
 
+https://pypi.org/project/django-tailwindcss-automated/
+
 <p align="left">
   <a href="https://skillicons.dev">
     <img src="https://skillicons.dev/icons?i=django,tailwindcss,python" />
   </a>
 </p>
 
 ## Getting Started 💙
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 Automated Project Initialization ððð --- An automated setup for Django
 project with Tailwind. Handles all setup and configuration automatically.â¨
+https://pypi.org/project/django-tailwindcss-automated/
 _[_h_t_t_p_s_:_/_/_s_k_i_l_l_i_c_o_n_s_._d_e_v_/_i_c_o_n_s_?_i_=_d_j_a_n_g_o_,_t_a_i_l_w_i_n_d_c_s_s_,_p_y_t_h_o_n_]
 ## Getting Started ð - ð Before you dive in, make sure that you have
 Node.js, Git, and Python installed on your computer. - Create a folder for your
 Django project. ## Install the Package Open your terminal and install the
 package using pip: ```bash pip install django_tailwindcss_automated ``` ## Run
 the Script In your terminal, run the following script to automate the setup:
 ```bash automate ``` ## Start the Development Server Open another terminal and
```

### Comparing `django_tailwindcss_automated-0.7/django_tailwindcss_automated/main.py` & `django_tailwindcss_automated-0.8/django_tailwindcss_automated/main.py`

 * *Files identical despite different names*

### Comparing `django_tailwindcss_automated-0.7/django_tailwindcss_automated.egg-info/PKG-INFO` & `django_tailwindcss_automated-0.8/django_tailwindcss_automated.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: django-tailwindcss-automated
-Version: 0.7
+Version: 0.8
 Summary: Handles all setup and configuration automatically.
 Home-page: UNKNOWN
 Author: Jan Leander
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 Automated Project Initialization 🐍💚💙 
 ---
 An automated setup for Django project with Tailwind. Handles all setup and configuration automatically.✨
 
+https://pypi.org/project/django-tailwindcss-automated/
+
 <p align="left">
   <a href="https://skillicons.dev">
     <img src="https://skillicons.dev/icons?i=django,tailwindcss,python" />
   </a>
 </p>
 
 ## Getting Started 💙
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: django-tailwindcss-automated Version: 0.7 Summary:
+Metadata-Version: 2.1 Name: django-tailwindcss-automated Version: 0.8 Summary:
 Handles all setup and configuration automatically. Home-page: UNKNOWN Author:
 Jan Leander License: UNKNOWN Platform: UNKNOWN Description-Content-Type: text/
 markdown Automated Project Initialization ððð --- An automated setup
 for Django project with Tailwind. Handles all setup and configuration
-automatically.â¨
+automatically.â¨ https://pypi.org/project/django-tailwindcss-automated/
 _[_h_t_t_p_s_:_/_/_s_k_i_l_l_i_c_o_n_s_._d_e_v_/_i_c_o_n_s_?_i_=_d_j_a_n_g_o_,_t_a_i_l_w_i_n_d_c_s_s_,_p_y_t_h_o_n_]
 ## Getting Started ð - ð Before you dive in, make sure that you have
 Node.js, Git, and Python installed on your computer. - Create a folder for your
 Django project. ## Install the Package Open your terminal and install the
 package using pip: ```bash pip install django_tailwindcss_automated ``` ## Run
 the Script In your terminal, run the following script to automate the setup:
 ```bash automate ``` ## Start the Development Server Open another terminal and
```

### Comparing `django_tailwindcss_automated-0.7/setup.py` & `django_tailwindcss_automated-0.8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name='django_tailwindcss_automated',
     description="Handles all setup and configuration automatically.",
-    version='0.7',
+    version='0.8',
     author='Jan Leander',
     packages=find_packages(),
     install_requires=[
         # add dependencies here.
         # e.g 'num>=1.11.1'
     ],
     entry_points={
```

