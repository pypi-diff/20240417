# Comparing `tmp/loe_simp_app_fw-1.0.1.tar.gz` & `tmp/loe_simp_app_fw-1.0.2.tar.gz`

## Comparing `loe_simp_app_fw-1.0.1.tar` & `loe_simp_app_fw-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.1/config-example.yaml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.1/src/loe_simp_app_fw/__init__.py
--rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.1/src/loe_simp_app_fw/config.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.1/src/loe_simp_app_fw/helper.py
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.1/src/loe_simp_app_fw/logger.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.1/tests/test_import.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.1/LICENSE
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.1/README.md
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.2/config-example.yaml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.2/src/loe_simp_app_fw/__init__.py
+-rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.2/src/loe_simp_app_fw/config.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.2/src/loe_simp_app_fw/helper.py
+-rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.2/src/loe_simp_app_fw/logger.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.2/tests/test_import.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.2/README.md
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.2/PKG-INFO
```

### Comparing `loe_simp_app_fw-1.0.1/src/loe_simp_app_fw/config.py` & `loe_simp_app_fw-1.0.2/src/loe_simp_app_fw/config.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.0.1/src/loe_simp_app_fw/helper.py` & `loe_simp_app_fw-1.0.2/src/loe_simp_app_fw/helper.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.0.1/src/loe_simp_app_fw/logger.py` & `loe_simp_app_fw-1.0.2/src/loe_simp_app_fw/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     @staticmethod
     def _log(level: str, msg: str) -> None:
         # Compose log
         composed_log_entry = f"{datetime.datetime.now()} {level.upper()}: {msg}\n"
         if Logger._isInit:
             # Write to file
             try:
-                with open(Logger._log_location, "a", encoding="utf-8") as f:
+                with open(Logger._log_location(), "a", encoding="utf-8") as f:
                     f.writelines(composed_log_entry)
             except FileNotFoundError:
                 Logger._create_log_file()
         else:
             # Write to buffer, not file
             Logger._log_buffer.append(composed_log_entry)
             print(composed_log_entry)
```

### Comparing `loe_simp_app_fw-1.0.1/tests/test_import.py` & `loe_simp_app_fw-1.0.2/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.0.1/.gitignore` & `loe_simp_app_fw-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.0.1/LICENSE` & `loe_simp_app_fw-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.0.1/README.md` & `loe_simp_app_fw-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.0.1/pyproject.toml` & `loe_simp_app_fw-1.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "loe_simp_app_fw"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="loeeeee", email="95266635+loeeeee@users.noreply.github.com" },
 ]
-description = "A super simple python app framework that includes a logger and a config management."
+description = "A super simple python app framework that includes a logger and a config management. Also usable in jupyter notebook."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
```

### Comparing `loe_simp_app_fw-1.0.1/PKG-INFO` & `loe_simp_app_fw-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.3
 Name: loe_simp_app_fw
-Version: 1.0.1
-Summary: A super simple python app framework that includes a logger and a config management.
+Version: 1.0.2
+Summary: A super simple python app framework that includes a logger and a config management. Also usable in jupyter notebook.
 Project-URL: Homepage, https://github.com/loeeeee/loe-simp-app-fw
 Project-URL: Issues, https://github.com/loeeeee/loe-simp-app-fw/issues
 Author-email: loeeeee <95266635+loeeeee@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

