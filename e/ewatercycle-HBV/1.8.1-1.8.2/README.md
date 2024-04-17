# Comparing `tmp/ewatercycle_hbv-1.8.1.tar.gz` & `tmp/ewatercycle_hbv-1.8.2.tar.gz`

## Comparing `ewatercycle_hbv-1.8.1.tar` & `ewatercycle_hbv-1.8.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/.readthedocs.yaml
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/CHANGELOG.md
--rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/plugin_guide.md
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/.idea/.gitignore
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/.idea/ewatercycle-hbv-numpy.iml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/.idea/misc.xml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/.idea/vcs.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/docs/Makefile
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/docs/conf.py
--rw-r--r--   0        0        0    55896 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/docs/example_model_run_HBV.ipynb
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/docs/index.rst
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/docs/make.bat
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/docs/model.rst
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/docs/requirements.txt
--rw-r--r--   0        0        0    92385 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/docs/_images/model_layout.png
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/docs/_static/README.rst
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/src/ewatercycle_HBV/__init__.py
--rw-r--r--   0        0        0    15335 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/src/ewatercycle_HBV/forcing.py
--rw-r--r--   0        0        0    10036 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/src/ewatercycle_HBV/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/tests/__init__.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/tests/test_forcing.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/tests/test_model.py
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/LICENSE.txt
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/README.md
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/pyproject.toml
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/.readthedocs.yaml
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/CHANGELOG.md
+-rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/plugin_guide.md
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/.idea/.gitignore
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/.idea/ewatercycle-hbv-numpy.iml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/.idea/misc.xml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/.idea/vcs.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/docs/Makefile
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/docs/conf.py
+-rw-r--r--   0        0        0    55896 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/docs/example_model_run_HBV.ipynb
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/docs/index.rst
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/docs/make.bat
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/docs/model.rst
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/docs/requirements.txt
+-rw-r--r--   0        0        0    92385 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/docs/_images/model_layout.png
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/docs/_static/README.rst
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/src/ewatercycle_HBV/__init__.py
+-rw-r--r--   0        0        0    15335 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/src/ewatercycle_HBV/forcing.py
+-rw-r--r--   0        0        0     8652 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/src/ewatercycle_HBV/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/tests/__init__.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/tests/test_forcing.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/tests/test_model.py
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/LICENSE.txt
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/README.md
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.2/PKG-INFO
```

### Comparing `ewatercycle_hbv-1.8.1/.readthedocs.yaml` & `ewatercycle_hbv-1.8.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.1/CHANGELOG.md` & `ewatercycle_hbv-1.8.2/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -39,8 +39,10 @@
 ### 1.7.0
   - new version of HBV bmi which adds snow 
 #### 1.7.1
   - bug fix with definitions of state variable names
 ### 1.8.0
 - Refactor potential evaporation from `pev` to `evspsblpot` & `tasmean` to `tas` to match convention
 #### 1.8.1
-- Rename `LumpedCamelsForcing` to `CamelsForcing`
+- Rename `LumpedCamelsForcing` to `CamelsForcing`
+#### 1.8.2
+- No longer removes config on `finalize`, should be up to user
```

### Comparing `ewatercycle_hbv-1.8.1/plugin_guide.md` & `ewatercycle_hbv-1.8.2/plugin_guide.md`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.1/.github/workflows/python-publish.yml` & `ewatercycle_hbv-1.8.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.1/.github/workflows/test.yml` & `ewatercycle_hbv-1.8.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.1/docs/Makefile` & `ewatercycle_hbv-1.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.1/docs/conf.py` & `ewatercycle_hbv-1.8.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.1/docs/example_model_run_HBV.ipynb` & `ewatercycle_hbv-1.8.2/docs/example_model_run_HBV.ipynb`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.1/docs/index.rst` & `ewatercycle_hbv-1.8.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.1/docs/make.bat` & `ewatercycle_hbv-1.8.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.1/docs/model.rst` & `ewatercycle_hbv-1.8.2/docs/model.rst`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.1/docs/_images/model_layout.png` & `ewatercycle_hbv-1.8.2/docs/_images/model_layout.png`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.1/docs/_static/README.rst` & `ewatercycle_hbv-1.8.2/docs/_static/README.rst`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.1/src/ewatercycle_HBV/forcing.py` & `ewatercycle_hbv-1.8.2/src/ewatercycle_HBV/forcing.py`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.1/src/ewatercycle_HBV/model.py` & `ewatercycle_hbv-1.8.2/src/ewatercycle_HBV/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -195,49 +195,20 @@
 
 
     def finalize(self) -> None:
         """Perform tear-down tasks for the model.
 
         After finalization, the model should not be used anymore.
 
-        ADDED: Remove created config files, especially useful for DA models
         """
 
         # remove bmi
         self._bmi.finalize()
         del self._bmi
 
-        config_file = self._cfg_dir / "HBV_config.json"
-        try:
-            # remove config file
-            config_file.unlink()
-        except FileNotFoundError:
-            warnings.warn(message=f'Config not found at {config_file}, removed by user?',category=UserWarning)
-
-        try:
-            # once empty, remove it
-            self._cfg_dir.rmdir()
-        except FileNotFoundError:
-            warnings.warn(message=f'Config folder not found at {self._cfg_dir.rmdir()}',category=UserWarning)
-
-        if type(self.forcing).__name__ == 'HBVForcing':
-            # NetCDF files created are timestamped and running them a lot creates many files, remove these
-            if self.forcing.camels_txt_defined() or self.forcing.test_data_bool:
-                self.unlink()
-
-        elif type(self.forcing).__name__ == 'LumpedMakkinkForcing':
-            # we created a temporary file so let's unlink that
-            self.unlink()
-
-    def unlink(self):
-        for file in ["potential_evaporation_file", "precipitation_file","mean_temperature_file"]:
-            path = self.forcing.directory / self._config[file]
-            if path.is_file():  # often both with be the same, e.g. with camels data.
-                path.unlink()
-            else:
-                pass
+
 
 class HBV(ContainerizedModel, HBVMethods):
     """The HBV eWaterCycle model, with the Container Registry docker image."""
     bmi_image: ContainerImage = ContainerImage(
         "ghcr.io/daafip/hbv-bmi-grpc4bmi:v1.5.0"
     )
```

### Comparing `ewatercycle_hbv-1.8.1/.gitignore` & `ewatercycle_hbv-1.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.1/LICENSE.txt` & `ewatercycle_hbv-1.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.1/README.md` & `ewatercycle_hbv-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.1/pyproject.toml` & `ewatercycle_hbv-1.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 path = "src/ewatercycle_HBV/__init__.py"
 
 [project]
 name = "ewatercycle-HBV"
 description = "Implementation of HBV for eWaterCycle"
 readme = "README.md"
 license = "Apache-2.0"
-version = "1.8.1"
+version = "1.8.2"
 authors = [
   { name = "David Haasnoot", email = "davidhaasnoot@gmail.com" },
 ]
 keywords = ["ewatercycle", "hydrology"]
 classifiers = [
   "Intended Audience :: Developers",
   "License :: OSI Approved :: Apache Software License",
```

### Comparing `ewatercycle_hbv-1.8.1/PKG-INFO` & `ewatercycle_hbv-1.8.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ewatercycle-HBV
-Version: 1.8.1
+Version: 1.8.2
 Summary: Implementation of HBV for eWaterCycle
 Project-URL: homepage, https://github.com/Daafip/ewatercycle-hbv
 Author-email: David Haasnoot <davidhaasnoot@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Keywords: ewatercycle,hydrology
 Classifier: Intended Audience :: Developers
```

