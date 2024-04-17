# Comparing `tmp/mlflow_oidc_auth-1.3.0.tar.gz` & `tmp/mlflow_oidc_auth-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow_oidc_auth-1.3.0.tar", last modified: Wed Apr 17 02:31:19 2024, max compression
+gzip compressed data, was "mlflow_oidc_auth-1.3.1.tar", last modified: Wed Apr 17 02:59:31 2024, max compression
```

## Comparing `mlflow_oidc_auth-1.3.0.tar` & `mlflow_oidc_auth-1.3.1.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:31:19.425439 mlflow_oidc_auth-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-04-17 02:30:09.000000 mlflow_oidc_auth-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17262 2024-04-17 02:31:19.425439 mlflow_oidc_auth-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-17 02:30:09.000000 mlflow_oidc_auth-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:31:19.417439 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-17 02:30:09.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-17 02:30:09.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    12050 2024-04-17 02:30:09.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-17 02:30:09.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:31:19.421439 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:30:09.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-17 02:30:09.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/db/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:31:19.421439 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:30:09.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/db/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-17 02:30:09.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/db/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-17 02:30:09.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/db/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:31:19.421439 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/db/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-17 02:30:09.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/db/migrations/versions/8606fa83a998_initial_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:30:09.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/db/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-17 02:30:09.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/db/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-17 02:30:09.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/db/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-17 02:30:09.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-17 02:30:09.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-17 02:30:09.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-17 02:30:09.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/sqlalchemy_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:31:19.421439 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/static/
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-17 02:30:09.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-04-17 02:30:09.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:31:19.421439 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-17 02:30:09.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/templates/_footer.html
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-17 02:30:09.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/templates/_head.html
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-17 02:30:09.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/templates/auth.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:31:19.425439 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/ui/
--rw-r--r--   0 runner    (1001) docker     (127)    16975 2024-04-17 02:31:16.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/ui/398.7b4ae9e14c5af3b5.js
--rw-r--r--   0 runner    (1001) docker     (127)    17458 2024-04-17 02:31:16.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/ui/3rdpartylicenses.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-17 02:31:16.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/ui/953.94c6a01c085d9731.js
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-17 02:31:16.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/ui/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    12078 2024-04-17 02:31:16.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (127)   703564 2024-04-17 02:31:16.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/ui/main.aa12189a64349ade.js
--rw-r--r--   0 runner    (1001) docker     (127)    35227 2024-04-17 02:31:16.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/ui/polyfills.90a0049d0bf863c4.js
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-17 02:31:16.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/ui/runtime.253378063cb1a335.js
--rw-r--r--   0 runner    (1001) docker     (127)   301021 2024-04-17 02:31:16.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/ui/styles.68f068b304676cf1.css
--rw-r--r--   0 runner    (1001) docker     (127)    35114 2024-04-17 02:30:09.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:31:19.425439 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17262 2024-04-17 02:31:19.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-17 02:31:19.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:31:19.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-17 02:31:19.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-17 02:31:19.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-17 02:31:19.000000 mlflow_oidc_auth-1.3.0/mlflow_oidc_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-17 02:30:09.000000 mlflow_oidc_auth-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 02:31:19.425439 mlflow_oidc_auth-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:59:31.842169 mlflow_oidc_auth-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17262 2024-04-17 02:59:31.842169 mlflow_oidc_auth-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:59:31.834169 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12050 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:59:31.838169 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:59:31.838169 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:59:31.838169 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/migrations/versions/8606fa83a998_initial_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/menu.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/sqlalchemy_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:59:31.838169 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:59:31.838169 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/templates/_footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/templates/_head.html
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/templates/auth.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:59:31.842169 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)    16975 2024-04-17 02:59:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/398.7b4ae9e14c5af3b5.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17458 2024-04-17 02:59:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/3rdpartylicenses.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-17 02:59:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/953.94c6a01c085d9731.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-17 02:59:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    12078 2024-04-17 02:59:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)   703564 2024-04-17 02:59:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/main.aa12189a64349ade.js
+-rw-r--r--   0 runner    (1001) docker     (127)    35227 2024-04-17 02:59:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/polyfills.90a0049d0bf863c4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-17 02:59:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/runtime.253378063cb1a335.js
+-rw-r--r--   0 runner    (1001) docker     (127)   301021 2024-04-17 02:59:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/styles.68f068b304676cf1.css
+-rw-r--r--   0 runner    (1001) docker     (127)    35114 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:59:31.842169 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17262 2024-04-17 02:59:31.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-17 02:59:31.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:59:31.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-17 02:59:31.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-17 02:59:31.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-17 02:59:31.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 02:59:31.842169 mlflow_oidc_auth-1.3.1/setup.cfg
```

### Comparing `mlflow_oidc_auth-1.3.0/LICENSE` & `mlflow_oidc_auth-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.0/PKG-INFO` & `mlflow_oidc_auth-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-oidc-auth
-Version: 1.3.0
+Version: 1.3.1
 Summary: OIDC auth plugin for MLflow
 Maintainer-email: Data Platform folks <noreply@example.com>
 License: 				Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mlflow_oidc_auth-1.3.0/README.md` & `mlflow_oidc_auth-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/app.py` & `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/app.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/client.py` & `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/client.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/config.py` & `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/config.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/db/migrations/alembic.ini` & `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/db/migrations/env.py` & `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/migrations/env.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/db/migrations/versions/8606fa83a998_initial_migration.py` & `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/migrations/versions/8606fa83a998_initial_migration.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/db/models.py` & `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/models.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/db/utils.py` & `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/entities.py` & `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/entities.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/permissions.py` & `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/permissions.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/routes.py` & `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/routes.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/sqlalchemy_store.py` & `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/sqlalchemy_store.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/static/favicon.ico` & `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/static/style.css` & `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/static/style.css`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/ui/398.7b4ae9e14c5af3b5.js` & `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/398.7b4ae9e14c5af3b5.js`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/ui/3rdpartylicenses.txt` & `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/3rdpartylicenses.txt`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/ui/953.94c6a01c085d9731.js` & `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/953.94c6a01c085d9731.js`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/ui/favicon.ico` & `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/ui/index.html` & `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/index.html`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/ui/main.aa12189a64349ade.js` & `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/main.aa12189a64349ade.js`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/ui/polyfills.90a0049d0bf863c4.js` & `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/polyfills.90a0049d0bf863c4.js`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/ui/runtime.253378063cb1a335.js` & `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/runtime.253378063cb1a335.js`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/ui/styles.68f068b304676cf1.css` & `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/styles.68f068b304676cf1.css`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.0/mlflow_oidc_auth/views.py` & `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/views.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.0/mlflow_oidc_auth.egg-info/PKG-INFO` & `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-oidc-auth
-Version: 1.3.0
+Version: 1.3.1
 Summary: OIDC auth plugin for MLflow
 Maintainer-email: Data Platform folks <noreply@example.com>
 License: 				Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mlflow_oidc_auth-1.3.0/mlflow_oidc_auth.egg-info/SOURCES.txt` & `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 pyproject.toml
 mlflow_oidc_auth/__init__.py
 mlflow_oidc_auth/app.py
 mlflow_oidc_auth/client.py
 mlflow_oidc_auth/config.py
 mlflow_oidc_auth/entities.py
+mlflow_oidc_auth/menu.html
 mlflow_oidc_auth/permissions.py
 mlflow_oidc_auth/routes.py
 mlflow_oidc_auth/sqlalchemy_store.py
 mlflow_oidc_auth/views.py
 mlflow_oidc_auth.egg-info/PKG-INFO
 mlflow_oidc_auth.egg-info/SOURCES.txt
 mlflow_oidc_auth.egg-info/dependency_links.txt
```

### Comparing `mlflow_oidc_auth-1.3.0/pyproject.toml` & `mlflow_oidc_auth-1.3.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -50,16 +50,17 @@
 
 [project.entry-points."mlflow_oidc_auth.client"]
 basic-auth = "mlflow_oidc_auth.client:AuthServiceClient"
 
 [tool.setuptools.package-data]
 mlflow_oidc_auth = [
   "db/migrations/alembic.ini",
-  "templates/*",
+  "menu.html",
   "static/*",
+  "templates/*",
   "ui/*",
 ]
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["mlflow_oidc_auth", "mlflow_oidc_auth.*"]
 exclude = ["tests", "tests.*"]
```

