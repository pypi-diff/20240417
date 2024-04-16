# Comparing `tmp/cpg-utils-5.0.4.tar.gz` & `tmp/cpg-utils-5.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpg-utils-5.0.4.tar", last modified: Tue Apr 16 04:01:29 2024, max compression
+gzip compressed data, was "cpg-utils-5.0.5.tar", last modified: Tue Apr 16 22:31:25 2024, max compression
```

## Comparing `cpg-utils-5.0.4.tar` & `cpg-utils-5.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:01:29.016861 cpg-utils-5.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-16 04:01:27.000000 cpg-utils-5.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-16 04:01:29.016861 cpg-utils-5.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-16 04:01:27.000000 cpg-utils-5.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:01:29.012861 cpg-utils-5.0.4/cpg_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-16 04:01:27.000000 cpg-utils-5.0.4/cpg_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14297 2024-04-16 04:01:27.000000 cpg-utils-5.0.4/cpg_utils/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-16 04:01:27.000000 cpg-utils-5.0.4/cpg_utils/cloudpath_hail_az.py
--rw-r--r--   0 runner    (1001) docker     (127)    16312 2024-04-16 04:01:27.000000 cpg-utils-5.0.4/cpg_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-16 04:01:27.000000 cpg-utils-5.0.4/cpg_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    26173 2024-04-16 04:01:27.000000 cpg-utils-5.0.4/cpg_utils/cromwell.py
--rw-r--r--   0 runner    (1001) docker     (127)    13229 2024-04-16 04:01:27.000000 cpg-utils-5.0.4/cpg_utils/cromwell_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14008 2024-04-16 04:01:27.000000 cpg-utils-5.0.4/cpg_utils/dataproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-04-16 04:01:27.000000 cpg-utils-5.0.4/cpg_utils/git.py
--rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-04-16 04:01:27.000000 cpg-utils-5.0.4/cpg_utils/hail_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-16 04:01:27.000000 cpg-utils-5.0.4/cpg_utils/membership.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 04:01:27.000000 cpg-utils-5.0.4/cpg_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-16 04:01:27.000000 cpg-utils-5.0.4/cpg_utils/slack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:01:29.012861 cpg-utils-5.0.4/cpg_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-16 04:01:28.000000 cpg-utils-5.0.4/cpg_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-16 04:01:29.000000 cpg-utils-5.0.4/cpg_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 04:01:28.000000 cpg-utils-5.0.4/cpg_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-16 04:01:28.000000 cpg-utils-5.0.4/cpg_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 04:01:28.000000 cpg-utils-5.0.4/cpg_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-16 04:01:27.000000 cpg-utils-5.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 04:01:29.016861 cpg-utils-5.0.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1348 2024-04-16 04:01:27.000000 cpg-utils-5.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:01:29.012861 cpg-utils-5.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 04:01:27.000000 cpg-utils-5.0.4/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-04-16 04:01:27.000000 cpg-utils-5.0.4/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-16 04:01:27.000000 cpg-utils-5.0.4/test/test_cromwell.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-16 04:01:27.000000 cpg-utils-5.0.4/test/test_doctests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:31:25.990887 cpg-utils-5.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-16 22:31:25.990887 cpg-utils-5.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:31:25.986887 cpg-utils-5.0.5/cpg_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14297 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils/cloudpath_hail_az.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16401 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26173 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils/cromwell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13229 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils/cromwell_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14008 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils/dataproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils/hail_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils/membership.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:31:25.990887 cpg-utils-5.0.5/cpg_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 22:31:25.990887 cpg-utils-5.0.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1348 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:31:25.990887 cpg-utils-5.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/test/test_cromwell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/test/test_doctests.py
```

### Comparing `cpg-utils-5.0.4/LICENSE` & `cpg-utils-5.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.4/PKG-INFO` & `cpg-utils-5.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpg-utils
-Version: 5.0.4
+Version: 5.0.5
 Summary: Library of convenience functions specific to the CPG
 Home-page: https://github.com/populationgenomics/cpg-utils
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cpg-utils-5.0.4/README.md` & `cpg-utils-5.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.4/cpg_utils/__init__.py` & `cpg-utils-5.0.5/cpg_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.4/cpg_utils/cloud.py` & `cpg-utils-5.0.5/cpg_utils/cloud.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.4/cpg_utils/cloudpath_hail_az.py` & `cpg-utils-5.0.5/cpg_utils/cloudpath_hail_az.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.4/cpg_utils/config.py` & `cpg-utils-5.0.5/cpg_utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,17 +223,21 @@
     >> config_retrieve(['key1', 'key2', 'key3'], config={'key1': {'key2': {}}})
     ConfigError('Key "key3" not found in {} (path: key1 -> key2)')
 
     Allow None as default value
     >> config_retrieve(['key1', 'key2', 'key3'], config={}, default=None) is None
     True
     """
-    d = config if config is not None else get_config()
-    if d is None:
-        raise ValueError('No config provided and no default config found')
+    if default is UnsuppliedDefault:
+        d = config if config is not None else get_config()
+    else:
+        try:
+            d = config if config is not None else get_config()
+        except ConfigError:
+            return default
 
     if isinstance(key, str):
         key = [key]
 
     if not key:
         raise ValueError('Key cannot be empty')
```

### Comparing `cpg-utils-5.0.4/cpg_utils/constants.py` & `cpg-utils-5.0.5/cpg_utils/constants.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.4/cpg_utils/cromwell.py` & `cpg-utils-5.0.5/cpg_utils/cromwell.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.4/cpg_utils/cromwell_model.py` & `cpg-utils-5.0.5/cpg_utils/cromwell_model.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.4/cpg_utils/dataproc.py` & `cpg-utils-5.0.5/cpg_utils/dataproc.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.4/cpg_utils/git.py` & `cpg-utils-5.0.5/cpg_utils/git.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.4/cpg_utils/hail_batch.py` & `cpg-utils-5.0.5/cpg_utils/hail_batch.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.4/cpg_utils/membership.py` & `cpg-utils-5.0.5/cpg_utils/membership.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.4/cpg_utils/slack.py` & `cpg-utils-5.0.5/cpg_utils/slack.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.4/cpg_utils.egg-info/PKG-INFO` & `cpg-utils-5.0.5/cpg_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpg-utils
-Version: 5.0.4
+Version: 5.0.5
 Summary: Library of convenience functions specific to the CPG
 Home-page: https://github.com/populationgenomics/cpg-utils
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cpg-utils-5.0.4/cpg_utils.egg-info/SOURCES.txt` & `cpg-utils-5.0.5/cpg_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.4/pyproject.toml` & `cpg-utils-5.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.4/setup.py` & `cpg-utils-5.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='cpg-utils',
     # This tag is automatically updated by bumpversion
-    version='5.0.4',
+    version='5.0.5',
     description='Library of convenience functions specific to the CPG',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/populationgenomics/cpg-utils',
     license='MIT',
     packages=find_packages(),
     package_data={
```

### Comparing `cpg-utils-5.0.4/test/test_config.py` & `cpg-utils-5.0.5/test/test_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,19 +56,27 @@
             config_retrieve(['workflow', 'access_level'], config={})
 
         with self.assertRaises(ConfigError):
             config_retrieve(['key1', 'key2', 'key3'], config={'key1': {'key2': {}}})
 
         # check that providing default=None isn't triggering some falsey check
         self.assertIsNone(
-            self.assertIsNone(
-                config_retrieve(['key1', 'key2', 'key3'], config={}, default=None),
-            ),
+            config_retrieve(['key1', 'key2', 'key3'], config={}, default=None),
         )
 
+    def test_retrieve_no_config(self):
+        """
+        Test the config_retrieve behaviour when no config is available
+        """
+        # we've got not config here
+        with self.assertRaises(ConfigError):
+            config_retrieve(['some-key'])
+
+        self.assertIsNone(config_retrieve(['some-key'], default=None))
+
     @patch.dict(os.environ, {'CPG_CONFIG_PATH': test_config_path.as_posix()})
     def test_read_from_env(self):
         """
         test_conf : test TOML configuration
         """
         conf = get_config()
```

### Comparing `cpg-utils-5.0.4/test/test_cromwell.py` & `cpg-utils-5.0.5/test/test_cromwell.py`

 * *Files identical despite different names*

