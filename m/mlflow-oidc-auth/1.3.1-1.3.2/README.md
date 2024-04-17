# Comparing `tmp/mlflow_oidc_auth-1.3.1.tar.gz` & `tmp/mlflow_oidc_auth-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow_oidc_auth-1.3.1.tar", last modified: Wed Apr 17 02:59:31 2024, max compression
+gzip compressed data, was "mlflow_oidc_auth-1.3.2.tar", last modified: Wed Apr 17 16:45:27 2024, max compression
```

## Comparing `mlflow_oidc_auth-1.3.1.tar` & `mlflow_oidc_auth-1.3.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:59:31.842169 mlflow_oidc_auth-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17262 2024-04-17 02:59:31.842169 mlflow_oidc_auth-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:59:31.834169 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    12050 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:59:31.838169 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:59:31.838169 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:59:31.838169 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/migrations/versions/8606fa83a998_initial_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/menu.html
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/sqlalchemy_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:59:31.838169 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/static/
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:59:31.838169 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/templates/_footer.html
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/templates/_head.html
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/templates/auth.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:59:31.842169 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/
--rw-r--r--   0 runner    (1001) docker     (127)    16975 2024-04-17 02:59:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/398.7b4ae9e14c5af3b5.js
--rw-r--r--   0 runner    (1001) docker     (127)    17458 2024-04-17 02:59:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/3rdpartylicenses.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-17 02:59:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/953.94c6a01c085d9731.js
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-17 02:59:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    12078 2024-04-17 02:59:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (127)   703564 2024-04-17 02:59:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/main.aa12189a64349ade.js
--rw-r--r--   0 runner    (1001) docker     (127)    35227 2024-04-17 02:59:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/polyfills.90a0049d0bf863c4.js
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-17 02:59:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/runtime.253378063cb1a335.js
--rw-r--r--   0 runner    (1001) docker     (127)   301021 2024-04-17 02:59:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/styles.68f068b304676cf1.css
--rw-r--r--   0 runner    (1001) docker     (127)    35114 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:59:31.842169 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17262 2024-04-17 02:59:31.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-17 02:59:31.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:59:31.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-17 02:59:31.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-17 02:59:31.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-17 02:59:31.000000 mlflow_oidc_auth-1.3.1/mlflow_oidc_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-17 02:58:29.000000 mlflow_oidc_auth-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 02:59:31.842169 mlflow_oidc_auth-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:45:27.593396 mlflow_oidc_auth-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17262 2024-04-17 16:45:27.593396 mlflow_oidc_auth-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:45:27.585396 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12050 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:45:27.589396 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/db/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:45:27.589396 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/db/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/db/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/db/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:45:27.589396 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/db/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/db/migrations/versions/8606fa83a998_initial_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/db/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/db/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/db/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/menu.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/sqlalchemy_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:45:27.589396 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:45:27.589396 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/templates/_footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/templates/_head.html
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/templates/auth.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:45:27.593396 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)    16975 2024-04-17 16:45:24.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/ui/398.7b4ae9e14c5af3b5.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17458 2024-04-17 16:45:24.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/ui/3rdpartylicenses.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-17 16:45:24.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/ui/953.94c6a01c085d9731.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-17 16:45:24.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/ui/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    12078 2024-04-17 16:45:25.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)   703564 2024-04-17 16:45:24.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/ui/main.aa12189a64349ade.js
+-rw-r--r--   0 runner    (1001) docker     (127)    35227 2024-04-17 16:45:24.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/ui/polyfills.90a0049d0bf863c4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-17 16:45:24.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/ui/runtime.253378063cb1a335.js
+-rw-r--r--   0 runner    (1001) docker     (127)   301021 2024-04-17 16:45:24.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/ui/styles.68f068b304676cf1.css
+-rw-r--r--   0 runner    (1001) docker     (127)    35211 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:45:27.593396 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17262 2024-04-17 16:45:27.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-17 16:45:27.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:45:27.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-17 16:45:27.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-17 16:45:27.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-17 16:45:27.000000 mlflow_oidc_auth-1.3.2/mlflow_oidc_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-17 16:44:23.000000 mlflow_oidc_auth-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 16:45:27.593396 mlflow_oidc_auth-1.3.2/setup.cfg
```

### Comparing `mlflow_oidc_auth-1.3.1/LICENSE` & `mlflow_oidc_auth-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.1/PKG-INFO` & `mlflow_oidc_auth-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-oidc-auth
-Version: 1.3.1
+Version: 1.3.2
 Summary: OIDC auth plugin for MLflow
 Maintainer-email: Data Platform folks <noreply@example.com>
 License: 				Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mlflow_oidc_auth-1.3.1/README.md` & `mlflow_oidc_auth-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/app.py` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/app.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/client.py` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/client.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/config.py` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     LEVEL = logging.DEBUG if os.environ.get("DEBUG") else logging.INFO
     LOG_LEVEL = os.environ.get("LOG_LEVEL", LEVEL)
     OIDC_USERS_DB_URI = os.environ.get("OIDC_USERS_DB_URI", "sqlite:///auth.db")
     OIDC_GROUP_NAME = os.environ.get("OIDC_GROUP_NAME", "mlflow")
     OIDC_ADMIN_GROUP_NAME = os.environ.get("OIDC_ADMIN_GROUP_NAME", "mlflow-admin")
     OIDC_PROVIDER_DISPLAY_NAME = os.environ.get("OIDC_PROVIDER_DISPLAY_NAME", "Login with OIDC")
     OIDC_DISCOVERY_URL = os.environ.get("OIDC_DISCOVERY_URL", None)
+    OIDC_GROUPS_ATTRIBUTE = os.environ.get("OIDC_GROUPS_ATTRIBUTE", "groups")
     OIDC_SCOPE = os.environ.get("OIDC_SCOPE", "openid,email,profile")
     OIDC_PROVIDER_TYPE = os.environ.get("OIDC_PROVIDER_TYPE", "oidc") # can be 'oidc' (with groups in user info) or 'microsoft' (with dedicated groups retrieval endpoint)
     if OIDC_DISCOVERY_URL:
         response = requests.get(OIDC_DISCOVERY_URL)
         config = response.json()
         OIDC_AUTHORIZATION_URL = config.get("authorization_endpoint")
         OIDC_TOKEN_URL = config.get("token_endpoint")
```

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/migrations/alembic.ini` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/db/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/migrations/env.py` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/db/migrations/env.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/migrations/versions/8606fa83a998_initial_migration.py` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/db/migrations/versions/8606fa83a998_initial_migration.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/models.py` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/db/models.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/db/utils.py` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/db/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/entities.py` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/entities.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/menu.html` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/menu.html`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/permissions.py` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/permissions.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/routes.py` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/routes.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/sqlalchemy_store.py` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/sqlalchemy_store.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/static/favicon.ico` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/static/style.css` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/static/style.css`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/398.7b4ae9e14c5af3b5.js` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/ui/398.7b4ae9e14c5af3b5.js`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/3rdpartylicenses.txt` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/ui/3rdpartylicenses.txt`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/953.94c6a01c085d9731.js` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/ui/953.94c6a01c085d9731.js`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/favicon.ico` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/index.html` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/ui/index.html`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/main.aa12189a64349ade.js` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/ui/main.aa12189a64349ade.js`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/polyfills.90a0049d0bf863c4.js` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/ui/polyfills.90a0049d0bf863c4.js`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/runtime.253378063cb1a335.js` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/ui/runtime.253378063cb1a335.js`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/ui/styles.68f068b304676cf1.css` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/ui/styles.68f068b304676cf1.css`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth/views.py` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -713,20 +713,22 @@
             for group in group_data["value"]
         ):
             return "User not in group", 401
         # set is_admin if user is in admin group
         if any(group["displayName"] == AppConfig.get_property("OIDC_ADMIN_GROUP_NAME") for group in group_data["value"]):
             is_admin = True
     elif AppConfig.get_property("OIDC_PROVIDER_TYPE") == "oidc":
-        if (AppConfig.get_property("OIDC_GROUP_NAME") not in user_data.get("groups", [])) or (
-            AppConfig.get_property("OIDC_ADMIN_GROUP_NAME") not in user_data.get("groups", [])
+        if not any (
+            group == AppConfig.get_property("OIDC_GROUP_NAME")
+            or group == AppConfig.get_property("OIDC_ADMIN_GROUP_NAME")
+            for group in user_data.get(AppConfig.get_property("OIDC_GROUPS_ATTRIBUTE"), [])
         ):
             return "User not in group", 401
         # set is_admin if user is in admin group
-        if AppConfig.get_property("OIDC_ADMIN_GROUP_NAME") in user_data.get("groups", []):
+        if AppConfig.get_property("OIDC_ADMIN_GROUP_NAME") in user_data.get(AppConfig.get_property("OIDC_GROUPS_ATTRIBUTE"), []):
             is_admin = True
 
     # Create user due to auth
     create_user(username=email.lower(), display_name=display_name, is_admin=is_admin)
     _set_username(email.lower())
     return redirect(url_for("oidc_ui"))
```

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth.egg-info/PKG-INFO` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-oidc-auth
-Version: 1.3.1
+Version: 1.3.2
 Summary: OIDC auth plugin for MLflow
 Maintainer-email: Data Platform folks <noreply@example.com>
 License: 				Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mlflow_oidc_auth-1.3.1/mlflow_oidc_auth.egg-info/SOURCES.txt` & `mlflow_oidc_auth-1.3.2/mlflow_oidc_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_auth-1.3.1/pyproject.toml` & `mlflow_oidc_auth-1.3.2/pyproject.toml`

 * *Files identical despite different names*

