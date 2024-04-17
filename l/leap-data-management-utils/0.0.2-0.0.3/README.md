# Comparing `tmp/leap_data_management_utils-0.0.2.tar.gz` & `tmp/leap_data_management_utils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leap_data_management_utils-0.0.2.tar", last modified: Tue Apr 16 20:57:54 2024, max compression
+gzip compressed data, was "leap_data_management_utils-0.0.3.tar", last modified: Wed Apr 17 18:29:53 2024, max compression
```

## Comparing `leap_data_management_utils-0.0.2.tar` & `leap_data_management_utils-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:57:54.742190 leap_data_management_utils-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:57:54.738190 leap_data_management_utils-0.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-16 20:57:40.000000 leap_data_management_utils-0.0.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:57:54.738190 leap_data_management_utils-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-16 20:57:40.000000 leap_data_management_utils-0.0.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-16 20:57:40.000000 leap_data_management_utils-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-16 20:57:40.000000 leap_data_management_utils-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-16 20:57:40.000000 leap_data_management_utils-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-16 20:57:54.742190 leap_data_management_utils-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-16 20:57:40.000000 leap_data_management_utils-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:57:54.738190 leap_data_management_utils-0.0.2/leap_data_management_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-16 20:57:40.000000 leap_data_management_utils-0.0.2/leap_data_management_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-16 20:57:54.000000 leap_data_management_utils-0.0.2/leap_data_management_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-16 20:57:40.000000 leap_data_management_utils-0.0.2/leap_data_management_utils/cmip_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-16 20:57:40.000000 leap_data_management_utils-0.0.2/leap_data_management_utils/cmip_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-04-16 20:57:40.000000 leap_data_management_utils-0.0.2/leap_data_management_utils/cmip_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-16 20:57:40.000000 leap_data_management_utils-0.0.2/leap_data_management_utils/data_management_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:57:54.738190 leap_data_management_utils-0.0.2/leap_data_management_utils/testing_notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    25238 2024-04-16 20:57:40.000000 leap_data_management_utils-0.0.2/leap_data_management_utils/testing_notebooks/testing_cmip_bigquery.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:57:54.742190 leap_data_management_utils-0.0.2/leap_data_management_utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-16 20:57:40.000000 leap_data_management_utils-0.0.2/leap_data_management_utils/tests/test_cmip_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-16 20:57:40.000000 leap_data_management_utils-0.0.2/leap_data_management_utils/tests/test_data_management_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:57:54.742190 leap_data_management_utils-0.0.2/leap_data_management_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-16 20:57:54.000000 leap_data_management_utils-0.0.2/leap_data_management_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-16 20:57:54.000000 leap_data_management_utils-0.0.2/leap_data_management_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:57:54.000000 leap_data_management_utils-0.0.2/leap_data_management_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-16 20:57:54.000000 leap_data_management_utils-0.0.2/leap_data_management_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-16 20:57:54.000000 leap_data_management_utils-0.0.2/leap_data_management_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-16 20:57:40.000000 leap_data_management_utils-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 20:57:54.742190 leap_data_management_utils-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:29:53.440287 leap_data_management_utils-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:29:53.436287 leap_data_management_utils-0.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-17 18:29:40.000000 leap_data_management_utils-0.0.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:29:53.436287 leap_data_management_utils-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-17 18:29:40.000000 leap_data_management_utils-0.0.3/.github/workflows/catalog-ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-17 18:29:40.000000 leap_data_management_utils-0.0.3/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-17 18:29:40.000000 leap_data_management_utils-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-17 18:29:40.000000 leap_data_management_utils-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-17 18:29:40.000000 leap_data_management_utils-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-17 18:29:53.440287 leap_data_management_utils-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-17 18:29:40.000000 leap_data_management_utils-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:29:53.436287 leap_data_management_utils-0.0.3/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-17 18:29:40.000000 leap_data_management_utils-0.0.3/ci/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:29:53.436287 leap_data_management_utils-0.0.3/leap_data_management_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-17 18:29:40.000000 leap_data_management_utils-0.0.3/leap_data_management_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 18:29:53.000000 leap_data_management_utils-0.0.3/leap_data_management_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-04-17 18:29:40.000000 leap_data_management_utils-0.0.3/leap_data_management_utils/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-17 18:29:40.000000 leap_data_management_utils-0.0.3/leap_data_management_utils/cmip_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-17 18:29:40.000000 leap_data_management_utils-0.0.3/leap_data_management_utils/cmip_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-04-17 18:29:40.000000 leap_data_management_utils-0.0.3/leap_data_management_utils/cmip_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-17 18:29:40.000000 leap_data_management_utils-0.0.3/leap_data_management_utils/data_management_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:29:53.436287 leap_data_management_utils-0.0.3/leap_data_management_utils/testing_notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    25238 2024-04-17 18:29:40.000000 leap_data_management_utils-0.0.3/leap_data_management_utils/testing_notebooks/testing_cmip_bigquery.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:29:53.436287 leap_data_management_utils-0.0.3/leap_data_management_utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-17 18:29:40.000000 leap_data_management_utils-0.0.3/leap_data_management_utils/tests/test_cmip_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-17 18:29:40.000000 leap_data_management_utils-0.0.3/leap_data_management_utils/tests/test_data_management_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:29:53.436287 leap_data_management_utils-0.0.3/leap_data_management_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-17 18:29:53.000000 leap_data_management_utils-0.0.3/leap_data_management_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-17 18:29:53.000000 leap_data_management_utils-0.0.3/leap_data_management_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 18:29:53.000000 leap_data_management_utils-0.0.3/leap_data_management_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-17 18:29:53.000000 leap_data_management_utils-0.0.3/leap_data_management_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-17 18:29:53.000000 leap_data_management_utils-0.0.3/leap_data_management_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-17 18:29:53.000000 leap_data_management_utils-0.0.3/leap_data_management_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-17 18:29:40.000000 leap_data_management_utils-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 18:29:53.440287 leap_data_management_utils-0.0.3/setup.cfg
```

### Comparing `leap_data_management_utils-0.0.2/.github/workflows/release.yaml` & `leap_data_management_utils-0.0.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.2/.gitignore` & `leap_data_management_utils-0.0.3/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -154,7 +154,9 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+
+_version.py
```

### Comparing `leap_data_management_utils-0.0.2/.pre-commit-config.yaml` & `leap_data_management_utils-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.2/LICENSE` & `leap_data_management_utils-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.2/PKG-INFO` & `leap_data_management_utils-0.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leap-data-management-utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: LEAP / pangeo-forge-recipes extension library for logging data in Google Big Query
 Author-email: LEAP <leap@columbia.edu>
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
@@ -13,21 +13,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: apache-beam
-Requires-Dist: google-cloud-bigquery
-Requires-Dist: google-api-core
-Requires-Dist: zarr
-Requires-Dist: xarray
-Requires-Dist: pangeo-forge-esgf
-Requires-Dist: db_dtypes
 Requires-Dist: cftime
+Requires-Dist: db_dtypes
+Requires-Dist: google-api-core
+Requires-Dist: google-cloud-bigquery
 Requires-Dist: pandas
+Requires-Dist: pangeo-forge-esgf
+Requires-Dist: pydantic-core
+Requires-Dist: pydantic>=2
+Requires-Dist: pyyaml
+Requires-Dist: universal-pathlib
+Requires-Dist: xarray
+Requires-Dist: zarr
 Provides-Extra: test
 Requires-Dist: pre-commit; extra == "test"
 
 # LEAP Data Management Utils
 
 This Repo is intended to be installed via the `requirements.txt` during recipe execution in `pangeo-forge-recipes`. It currently contains beam transforms to log information into BigQuery tables. Additional shared utilities and checks that are commonly used between LEAP pangeo-forge-feedstocks can live here.
```

### Comparing `leap_data_management_utils-0.0.2/leap_data_management_utils/cmip_catalog.py` & `leap_data_management_utils-0.0.3/leap_data_management_utils/cmip_catalog.py`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.2/leap_data_management_utils/cmip_testing.py` & `leap_data_management_utils-0.0.3/leap_data_management_utils/cmip_testing.py`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.2/leap_data_management_utils/cmip_transforms.py` & `leap_data_management_utils-0.0.3/leap_data_management_utils/cmip_transforms.py`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.2/leap_data_management_utils/data_management_transforms.py` & `leap_data_management_utils-0.0.3/leap_data_management_utils/data_management_transforms.py`

 * *Files 20% similar despite different names*

```diff
@@ -112,7 +112,47 @@
     def _register_dataset_to_catalog(self, store: zarr.storage.FSStore) -> zarr.storage.FSStore:
         bq_interface = BQInterface(table_id=self.table_id)
         bq_interface.catalog_insert(dataset_id=self.dataset_id, dataset_url=store.path)
         return store
 
     def expand(self, pcoll: beam.PCollection) -> beam.PCollection:
         return pcoll | beam.Map(self._register_dataset_to_catalog)
+
+
+@dataclass
+class Copy(beam.PTransform):
+    target: str
+
+    def _copy(self, store: zarr.storage.FSStore) -> zarr.storage.FSStore:
+        import os
+
+        import gcsfs
+        import zarr
+
+        # We do need the gs:// prefix?
+        # TODO: Determine this dynamically from zarr.storage.FSStore
+        source = f'gs://{os.path.normpath(store.path)}/'  # FIXME more elegant. `.copytree` needs trailing slash
+        fs = gcsfs.GCSFileSystem()  # FIXME: How can we generalize this?
+        fs.cp(source, self.target, recursive=True)
+        # return a new store with the new path that behaves exactly like the input
+        # to this stage (so we can slot this stage right before testing/logging stages)
+        return zarr.storage.FSStore(self.target)
+
+    def expand(self, pcoll: beam.PCollection) -> beam.PCollection:
+        return pcoll | 'Copying Store' >> beam.Map(self._copy)
+
+
+@dataclass
+class InjectAttrs(beam.PTransform):
+    inject_attrs: dict
+
+    def _update_zarr_attrs(self, store: zarr.storage.FSStore) -> zarr.storage.FSStore:
+        # TODO: Can we get a warning here if the store does not exist?
+        attrs = zarr.open(store, mode='a').attrs
+        attrs.update(self.inject_attrs)
+        # ? Should we consolidate here? We are explicitly doing that later...
+        return store
+
+    def expand(
+        self, pcoll: beam.PCollection[zarr.storage.FSStore]
+    ) -> beam.PCollection[zarr.storage.FSStore]:
+        return pcoll | 'Injecting Attributes' >> beam.Map(self._update_zarr_attrs)
```

### Comparing `leap_data_management_utils-0.0.2/leap_data_management_utils/testing_notebooks/testing_cmip_bigquery.ipynb` & `leap_data_management_utils-0.0.3/leap_data_management_utils/testing_notebooks/testing_cmip_bigquery.ipynb`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.2/leap_data_management_utils/tests/test_cmip_transforms.py` & `leap_data_management_utils-0.0.3/leap_data_management_utils/tests/test_cmip_transforms.py`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.2/leap_data_management_utils.egg-info/PKG-INFO` & `leap_data_management_utils-0.0.3/leap_data_management_utils.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leap-data-management-utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: LEAP / pangeo-forge-recipes extension library for logging data in Google Big Query
 Author-email: LEAP <leap@columbia.edu>
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
@@ -13,21 +13,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: apache-beam
-Requires-Dist: google-cloud-bigquery
-Requires-Dist: google-api-core
-Requires-Dist: zarr
-Requires-Dist: xarray
-Requires-Dist: pangeo-forge-esgf
-Requires-Dist: db_dtypes
 Requires-Dist: cftime
+Requires-Dist: db_dtypes
+Requires-Dist: google-api-core
+Requires-Dist: google-cloud-bigquery
 Requires-Dist: pandas
+Requires-Dist: pangeo-forge-esgf
+Requires-Dist: pydantic-core
+Requires-Dist: pydantic>=2
+Requires-Dist: pyyaml
+Requires-Dist: universal-pathlib
+Requires-Dist: xarray
+Requires-Dist: zarr
 Provides-Extra: test
 Requires-Dist: pre-commit; extra == "test"
 
 # LEAP Data Management Utils
 
 This Repo is intended to be installed via the `requirements.txt` during recipe execution in `pangeo-forge-recipes`. It currently contains beam transforms to log information into BigQuery tables. Additional shared utilities and checks that are commonly used between LEAP pangeo-forge-feedstocks can live here.
```

### Comparing `leap_data_management_utils-0.0.2/leap_data_management_utils.egg-info/SOURCES.txt` & `leap_data_management_utils-0.0.3/leap_data_management_utils.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.md
 pyproject.toml
 .github/dependabot.yml
+.github/workflows/catalog-ci.yaml
 .github/workflows/release.yaml
+ci/environment.yaml
 leap_data_management_utils/__init__.py
 leap_data_management_utils/_version.py
+leap_data_management_utils/catalog.py
 leap_data_management_utils/cmip_catalog.py
 leap_data_management_utils/cmip_testing.py
 leap_data_management_utils/cmip_transforms.py
 leap_data_management_utils/data_management_transforms.py
 leap_data_management_utils.egg-info/PKG-INFO
 leap_data_management_utils.egg-info/SOURCES.txt
 leap_data_management_utils.egg-info/dependency_links.txt
+leap_data_management_utils.egg-info/entry_points.txt
 leap_data_management_utils.egg-info/requires.txt
 leap_data_management_utils.egg-info/top_level.txt
 leap_data_management_utils/testing_notebooks/testing_cmip_bigquery.ipynb
 leap_data_management_utils/tests/test_cmip_transforms.py
 leap_data_management_utils/tests/test_data_management_transforms.py
```

### Comparing `leap_data_management_utils-0.0.2/pyproject.toml` & `leap_data_management_utils-0.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -19,29 +19,41 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
 ]
 dependencies = [
     "apache-beam",
-    "google-cloud-bigquery",
-    "google-api-core",
-    "zarr",
-    "xarray",
-    "pangeo-forge-esgf",
-    "db_dtypes",
     "cftime",
+    "db_dtypes",
+    "google-api-core",
+    "google-cloud-bigquery",
     "pandas",
+    "pangeo-forge-esgf",
+    "pydantic-core",
+    "pydantic>=2",
+    "pyyaml",
+    "universal-pathlib",
+    "xarray",
+    "zarr",
 ]
 
 [project.optional-dependencies]
 test = [
     "pre-commit",
 ]
 
+
+[project.scripts]
+leap-catalog = "leap_data_management_utils.catalog:main"
+
+
+[tool.setuptools.packages.find]
+include = ["leap_data_management_utils*"]
+
 [tool.setuptools_scm]
 write_to = "leap_data_management_utils/_version.py"
 write_to_template = "__version__ = '{version}'"
 
 [tool.ruff]
 line-length = 100
 target-version = "py39"
```

