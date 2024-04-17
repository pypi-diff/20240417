# Comparing `tmp/yaast-0.0.4.tar.gz` & `tmp/yaast-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/kjetil/code/yaast/dist/tmp9c2k8i4c/yaast-0.0.4.tar", last modified: Mon May  3 11:45:19 2021, max compression
+gzip compressed data, was "yaast-0.1.5.tar", last modified: Wed Apr 17 11:15:13 2024, max compression
```

## Comparing `yaast-0.0.4.tar` & `yaast-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 kjetil    (1000) kjetil    (1000)        0 2021-05-03 11:45:19.594462 yaast-0.0.4/
--rw-rw-r--   0 kjetil    (1000) kjetil    (1000)     1065 2020-03-03 20:55:54.000000 yaast-0.0.4/LICENSE
--rw-rw-r--   0 kjetil    (1000) kjetil    (1000)     1611 2021-05-03 11:45:19.594462 yaast-0.0.4/PKG-INFO
--rw-rw-r--   0 kjetil    (1000) kjetil    (1000)      836 2021-05-03 11:39:22.000000 yaast-0.0.4/README.md
--rw-rw-r--   0 kjetil    (1000) kjetil    (1000)      104 2021-05-03 08:02:07.000000 yaast-0.0.4/pyproject.toml
--rw-rw-r--   0 kjetil    (1000) kjetil    (1000)      711 2021-05-03 11:45:19.594462 yaast-0.0.4/setup.cfg
-drwxrwxr-x   0 kjetil    (1000) kjetil    (1000)        0 2021-05-03 11:45:19.590462 yaast-0.0.4/src/
-drwxrwxr-x   0 kjetil    (1000) kjetil    (1000)        0 2021-05-03 11:45:19.594462 yaast-0.0.4/src/yaast/
--rw-rw-r--   0 kjetil    (1000) kjetil    (1000)      186 2021-05-03 11:29:51.000000 yaast-0.0.4/src/yaast/__init__.py
--rw-rw-r--   0 kjetil    (1000) kjetil    (1000)       57 2021-05-03 10:33:33.000000 yaast-0.0.4/src/yaast/__main__.py
--rw-rw-r--   0 kjetil    (1000) kjetil    (1000)     3524 2021-05-03 10:45:41.000000 yaast-0.0.4/src/yaast/awsconfigparser.py
--rw-rw-r--   0 kjetil    (1000) kjetil    (1000)     4421 2021-05-03 10:51:34.000000 yaast-0.0.4/src/yaast/write_session.py
-drwxrwxr-x   0 kjetil    (1000) kjetil    (1000)        0 2021-05-03 11:45:19.594462 yaast-0.0.4/src/yaast.egg-info/
--rw-rw-r--   0 kjetil    (1000) kjetil    (1000)     1611 2021-05-03 11:45:19.000000 yaast-0.0.4/src/yaast.egg-info/PKG-INFO
--rw-rw-r--   0 kjetil    (1000) kjetil    (1000)      342 2021-05-03 11:45:19.000000 yaast-0.0.4/src/yaast.egg-info/SOURCES.txt
--rw-rw-r--   0 kjetil    (1000) kjetil    (1000)        1 2021-05-03 11:45:19.000000 yaast-0.0.4/src/yaast.egg-info/dependency_links.txt
--rw-rw-r--   0 kjetil    (1000) kjetil    (1000)       38 2021-05-03 11:45:19.000000 yaast-0.0.4/src/yaast.egg-info/entry_points.txt
--rw-rw-r--   0 kjetil    (1000) kjetil    (1000)        9 2021-05-03 11:45:19.000000 yaast-0.0.4/src/yaast.egg-info/requires.txt
--rw-rw-r--   0 kjetil    (1000) kjetil    (1000)        6 2021-05-03 11:45:19.000000 yaast-0.0.4/src/yaast.egg-info/top_level.txt
+drwxr-xr-x   0 kdm       (1000) docker     (130)        0 2024-04-17 11:15:13.728350 yaast-0.1.5/
+-rw-r--r--   0 kdm       (1000) docker     (130)     1065 2021-11-24 08:06:17.000000 yaast-0.1.5/LICENSE
+-rw-r--r--   0 kdm       (1000) docker     (130)     1351 2024-04-17 11:15:13.728350 yaast-0.1.5/PKG-INFO
+-rw-r--r--   0 kdm       (1000) docker     (130)      834 2024-04-16 07:46:00.000000 yaast-0.1.5/README.md
+-rwxr-xr-x   0 kdm       (1000) docker     (130)     1673 2024-04-16 07:21:09.000000 yaast-0.1.5/console_url.sh
+-rw-r--r--   0 kdm       (1000) docker     (130)      104 2021-11-24 08:06:17.000000 yaast-0.1.5/pyproject.toml
+-rw-r--r--   0 kdm       (1000) docker     (130)      738 2024-04-17 11:15:13.728350 yaast-0.1.5/setup.cfg
+drwxr-xr-x   0 kdm       (1000) docker     (130)        0 2024-04-17 11:15:13.724350 yaast-0.1.5/src/
+drwxr-xr-x   0 kdm       (1000) docker     (130)        0 2024-04-17 11:15:13.728350 yaast-0.1.5/src/yaast/
+-rw-r--r--   0 kdm       (1000) docker     (130)      186 2021-11-24 08:06:17.000000 yaast-0.1.5/src/yaast/__init__.py
+-rw-r--r--   0 kdm       (1000) docker     (130)       57 2021-11-24 08:06:17.000000 yaast-0.1.5/src/yaast/__main__.py
+-rw-r--r--   0 kdm       (1000) docker     (130)     3524 2021-11-24 08:06:17.000000 yaast-0.1.5/src/yaast/awsconfigparser.py
+-rw-r--r--   0 kdm       (1000) docker     (130)     4421 2021-11-24 08:06:17.000000 yaast-0.1.5/src/yaast/write_session.py
+drwxr-xr-x   0 kdm       (1000) docker     (130)        0 2024-04-17 11:15:13.728350 yaast-0.1.5/src/yaast.egg-info/
+-rw-r--r--   0 kdm       (1000) docker     (130)     1351 2024-04-17 11:15:13.000000 yaast-0.1.5/src/yaast.egg-info/PKG-INFO
+-rw-r--r--   0 kdm       (1000) docker     (130)      357 2024-04-17 11:15:13.000000 yaast-0.1.5/src/yaast.egg-info/SOURCES.txt
+-rw-r--r--   0 kdm       (1000) docker     (130)        1 2024-04-17 11:15:13.000000 yaast-0.1.5/src/yaast.egg-info/dependency_links.txt
+-rw-r--r--   0 kdm       (1000) docker     (130)       37 2024-04-17 11:15:13.000000 yaast-0.1.5/src/yaast.egg-info/entry_points.txt
+-rw-r--r--   0 kdm       (1000) docker     (130)        9 2024-04-17 11:15:13.000000 yaast-0.1.5/src/yaast.egg-info/requires.txt
+-rw-r--r--   0 kdm       (1000) docker     (130)        6 2024-04-17 11:15:13.000000 yaast-0.1.5/src/yaast.egg-info/top_level.txt
```

### Comparing `yaast-0.0.4/LICENSE` & `yaast-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yaast-0.0.4/README.md` & `yaast-0.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # Yaast (Jåst)
 
-
-
 ## YetAnotherAWSSessionTool
 
 *Why?* ..After obtaining a normal accessKey set, 
 the MFA enabled user faces the challege of 
 mantaining a daily set of temp accessKeys+token (session) for
 use with awscli, sdks and the stuff like terraform.
```

### Comparing `yaast-0.0.4/setup.cfg` & `yaast-0.1.5/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = yaast
-version = 0.0.4
+version = 0.1.5
 author = Kjetil Midtile
 author_email = kjetil.midtlie@gmail.com
 description = AWS credentials MFA-Resolver tool
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/dynnamitt/yaast
 project_urls = 
@@ -17,14 +17,16 @@
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	botocore
+scripts = 
+	console_url.sh
 
 [options.entry_points]
 console_scripts = 
 	yaast = yaast:main
 
 [options.packages.find]
 where = src
```

### Comparing `yaast-0.0.4/src/yaast/awsconfigparser.py` & `yaast-0.1.5/src/yaast/awsconfigparser.py`

 * *Files identical despite different names*

### Comparing `yaast-0.0.4/src/yaast/write_session.py` & `yaast-0.1.5/src/yaast/write_session.py`

 * *Files identical despite different names*

