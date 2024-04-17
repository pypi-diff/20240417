# Comparing `tmp/loe_simp_app_fw-1.0.0.tar.gz` & `tmp/loe_simp_app_fw-1.0.1.tar.gz`

## Comparing `loe_simp_app_fw-1.0.0.tar` & `loe_simp_app_fw-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.0/config-example.yaml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.0/src/loe_simp_app_fw/__init__.py
--rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.0/src/loe_simp_app_fw/config.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.0/src/loe_simp_app_fw/helper.py
--rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.0/src/loe_simp_app_fw/logger.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.0/tests/test_import.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.0/LICENSE
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.0/README.md
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.1/config-example.yaml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.1/src/loe_simp_app_fw/__init__.py
+-rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.1/src/loe_simp_app_fw/config.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.1/src/loe_simp_app_fw/helper.py
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.1/src/loe_simp_app_fw/logger.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.1/tests/test_import.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.1/README.md
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.0.1/PKG-INFO
```

### Comparing `loe_simp_app_fw-1.0.0/src/loe_simp_app_fw/config.py` & `loe_simp_app_fw-1.0.1/src/loe_simp_app_fw/config.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.0.0/src/loe_simp_app_fw/helper.py` & `loe_simp_app_fw-1.0.1/src/loe_simp_app_fw/helper.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.0.0/src/loe_simp_app_fw/logger.py` & `loe_simp_app_fw-1.0.1/src/loe_simp_app_fw/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,16 +53,16 @@
             f.writelines(f"\n{datetime.datetime.now()} INIT Logger successful\n")
             f.writelines("".join(Logger._log_buffer))
         
         # Empty log buffer
         Logger._log_buffer = []
 
         # Update flags
-        _isInit = True
-        print("Logger init process finished.")
+        Logger._isInit = True
+        print(f"Logger init process finished, Logger isInit is set to {Logger._isInit}")
 
     @staticmethod
     def info(msg: str) -> None:
         Logger._log("INFO", msg)
 
     @staticmethod
     def debug(msg: str) -> None:
```

### Comparing `loe_simp_app_fw-1.0.0/.gitignore` & `loe_simp_app_fw-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.0.0/LICENSE` & `loe_simp_app_fw-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.0.0/pyproject.toml` & `loe_simp_app_fw-1.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "loe_simp_app_fw"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="loeeeee", email="95266635+loeeeee@users.noreply.github.com" },
 ]
 description = "A super simple python app framework that includes a logger and a config management."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

