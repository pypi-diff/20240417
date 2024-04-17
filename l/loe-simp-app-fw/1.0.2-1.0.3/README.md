# Comparing `tmp/loe_simp_app_fw-1.0.2.tar.gz` & `tmp/loe_simp_app_fw-1.0.3.tar.gz`

## Comparing `loe_simp_app_fw-1.0.2.tar` & `loe_simp_app_fw-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.2/config-example.yaml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.2/src/loe_simp_app_fw/__init__.py
--rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.2/src/loe_simp_app_fw/config.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.2/src/loe_simp_app_fw/helper.py
--rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.2/src/loe_simp_app_fw/logger.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.2/tests/test_import.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.2/LICENSE
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.2/README.md
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.3/config-example.yaml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.3/src/loe_simp_app_fw/__init__.py
+-rw-r--r--   0        0        0     5966 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.3/src/loe_simp_app_fw/config.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.3/src/loe_simp_app_fw/helper.py
+-rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.3/src/loe_simp_app_fw/logger.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.3/tests/test_import.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.3/README.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.3/PKG-INFO
```

### Comparing `loe_simp_app_fw-1.0.2/src/loe_simp_app_fw/config.py` & `loe_simp_app_fw-1.0.3/src/loe_simp_app_fw/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,16 +101,18 @@
             config_path (str): path to config, should be a yaml file
             project_root_path (str, optional): path to project top level. Defaults to current working directory.
             example_config_path (str, optional): path to config example. Defaults to "".
         """
         print(f"Example config path: {example_config_path}")
         # Senity check
         ## No on-the-fly update of project root path
-        if Config._project_root_path and project_root_path and os.path.samefile(project_root_path, Config._project_root_path):
-            Logger.error("One should not change project root path twice")
+        if Config._project_root_path and project_root_path and not os.path.samefile(project_root_path, Config._project_root_path):
+            Logger.error("One should not change project root path twice.")
+            Logger.error(f"Orignial project root path: {Config._project_root_path}")
+            Logger.error(f"Updated project root path: {project_root_path}")
             raise ProjectRootChanged
 
         ## Check example config file
         if not example_config_path or not os.path.isfile(example_config_path):
             Logger.warning("Example config path not valid")
 
         ## Check config path
```

### Comparing `loe_simp_app_fw-1.0.2/src/loe_simp_app_fw/helper.py` & `loe_simp_app_fw-1.0.3/src/loe_simp_app_fw/helper.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.0.2/src/loe_simp_app_fw/logger.py` & `loe_simp_app_fw-1.0.3/src/loe_simp_app_fw/logger.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.0.2/tests/test_import.py` & `loe_simp_app_fw-1.0.3/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.0.2/.gitignore` & `loe_simp_app_fw-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.0.2/LICENSE` & `loe_simp_app_fw-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.0.2/README.md` & `loe_simp_app_fw-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.0.2/pyproject.toml` & `loe_simp_app_fw-1.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "loe_simp_app_fw"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="loeeeee", email="95266635+loeeeee@users.noreply.github.com" },
 ]
-description = "A super simple python app framework that includes a logger and a config management. Also usable in jupyter notebook."
+description = "A super simple python app framework that includes a logger and a config manager. Also usable in jupyter notebook."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
```

### Comparing `loe_simp_app_fw-1.0.2/PKG-INFO` & `loe_simp_app_fw-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.3
 Name: loe_simp_app_fw
-Version: 1.0.2
-Summary: A super simple python app framework that includes a logger and a config management. Also usable in jupyter notebook.
+Version: 1.0.3
+Summary: A super simple python app framework that includes a logger and a config manager. Also usable in jupyter notebook.
 Project-URL: Homepage, https://github.com/loeeeee/loe-simp-app-fw
 Project-URL: Issues, https://github.com/loeeeee/loe-simp-app-fw/issues
 Author-email: loeeeee <95266635+loeeeee@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

