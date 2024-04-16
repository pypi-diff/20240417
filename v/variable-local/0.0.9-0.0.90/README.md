# Comparing `tmp/variable_local-0.0.9.tar.gz` & `tmp/variable_local-0.0.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "variable_local-0.0.9.tar", last modified: Thu Aug 31 15:20:42 2023, max compression
+gzip compressed data, was "variable_local-0.0.90.tar", last modified: Tue Apr 16 22:46:35 2024, max compression
```

## Comparing `variable_local-0.0.9.tar` & `variable_local-0.0.90.tar`

### file list

```diff
@@ -1,11 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 15:20:42.781710 variable_local-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (999)      479 2023-08-31 15:20:42.781710 variable_local-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     2122 2023-08-31 15:20:24.000000 variable_local-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (999)      732 2023-08-31 15:20:24.000000 variable_local-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-31 15:20:42.781710 variable_local-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     1461 2023-08-31 15:20:24.000000 variable_local-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 15:20:42.781710 variable_local-0.0.9/variable_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)      479 2023-08-31 15:20:42.000000 variable_local-0.0.9/variable_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      185 2023-08-31 15:20:42.000000 variable_local-0.0.9/variable_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-31 15:20:42.000000 variable_local-0.0.9/variable_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-31 15:20:42.000000 variable_local-0.0.9/variable_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:46:35.848099 variable_local-0.0.90/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-16 22:46:35.848099 variable_local-0.0.90/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-16 22:46:04.000000 variable_local-0.0.90/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-16 22:46:04.000000 variable_local-0.0.90/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 22:46:35.848099 variable_local-0.0.90/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-16 22:46:04.000000 variable_local-0.0.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:46:35.844099 variable_local-0.0.90/variable_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:46:35.848099 variable_local-0.0.90/variable_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:46:04.000000 variable_local-0.0.90/variable_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-16 22:46:04.000000 variable_local-0.0.90/variable_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9672 2024-04-16 22:46:04.000000 variable_local-0.0.90/variable_local/src/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-16 22:46:04.000000 variable_local-0.0.90/variable_local/src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-04-16 22:46:04.000000 variable_local-0.0.90/variable_local/src/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:46:35.848099 variable_local-0.0.90/variable_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-16 22:46:35.000000 variable_local-0.0.90/variable_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-16 22:46:35.000000 variable_local-0.0.90/variable_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:46:35.000000 variable_local-0.0.90/variable_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-16 22:46:35.000000 variable_local-0.0.90/variable_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 22:46:35.000000 variable_local-0.0.90/variable_local.egg-info/top_level.txt
```

### Comparing `variable_local-0.0.9/README.md` & `variable_local-0.0.90/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,71 @@
 # python-package-template
+
 To create local package and remote package layers (not to create GraphQL and REST-API layers)
 
+# TODO
+
+Support new automated fields such as<br>
+
+## Geo fields
+
+${{ profile.main_city_name }}
+
+## Birthday
+
+${{ person.day_to_birthday }}
+
+# Used by
+
+Dialog Workflow<br>
+Messages<br>
+
 # directory structure
-Root directory should have only .github/, ,gitignore, README.md and the project directory (i.e. location_local_python_package same as repo) - This will allow is to easily switch to mono repo<br> 
+
+Root directory should have only .github/, ,gitignore, README.md and the project directory (i.e.
+location_local_python_package same as repo) - This will allow is to easily switch to mono repo<br>
 /location_local<br>
 /location_local/get_country_name<br>
 /location_local/get_country_name/src<br>
 /location_local/get_country_name/src/get_country_name.py<br>
 /location_local/get_country_name/tests<br>
 /location_local/get_country_name/tests/get_country_name_test.py<br>
 
 # database Python scripts in /db folder
+
 Please place <table-name>.py in /db<br>
 No need for seperate file for _ml table<br>
 Please delete the example file if not needed<br>
-  
+
 # Create the files to create the database schema, tables, view and populate metadata and Test-Data
+
 /db/<table-name>.py - CREATE SCHEMA ... CREATE TABLE ... CREATE VIEW ... including _ml_table<br>
 /db/<table-name>_insert.py to create metadata and Test-Data records
 
 # Update the setup.py (i.e.name, version)
- 
+
 # Please create test directory inside the directory of the project i.e. /<project-name>/tests
 
 # Update the serverless.yml in the root directory
+
 provider:
-  stage: play1
-  
+stage: play1
+
 Update the endpoints in serverless.yml
 
 # Working with VS Code
+
 Please make sure you push to the repo launch.json fie that enables to run and debug the code<br>
 
 # Unit-Test
+
 We prefer using pytest and not unittest package<br>
 
 Please create pytest.init in the project-directory and not in the root directory
+
 ```
 [pytest]
 markers =
     test: custom mark for tests
 ```
 
 # When you took care of all the TODOs in the repo, using our infrastructure classes (i.e. Logger, Database, Url, Importer ...) your Feature Branch GitHub Actions Workflow is Green without warnings, all tests are running in GHA, code is documented, README.md is clean and self explained, test coverage is above 90% and all your lines are covered with Unit-Tests, you can filter and analyse your records in Logz.io, pull dev to your Feature Branch and only then create Pull Request to dev
```

