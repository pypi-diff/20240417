# Comparing `tmp/dkist-inventory-1.3.0rc1.tar.gz` & `tmp/dkist_inventory-1.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-inventory-1.3.0rc1.tar", last modified: Mon Feb 26 15:13:55 2024, max compression
+gzip compressed data, was "dkist_inventory-1.3.1rc1.tar", last modified: Wed Apr 17 15:20:19 2024, max compression
```

## Comparing `dkist-inventory-1.3.0rc1.tar` & `dkist_inventory-1.3.1rc1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 15:13:55.248844 dkist-inventory-1.3.0rc1/
--rw-rw-rw-   0 root         (0) root         (0)     3019 2024-02-26 15:13:26.000000 dkist-inventory-1.3.0rc1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      333 2024-02-26 15:13:26.000000 dkist-inventory-1.3.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2163 2024-02-26 15:13:55.248844 dkist-inventory-1.3.0rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1045 2024-02-26 15:13:26.000000 dkist-inventory-1.3.0rc1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1579 2024-02-26 15:13:26.000000 dkist-inventory-1.3.0rc1/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     1043 2024-02-26 15:13:26.000000 dkist-inventory-1.3.0rc1/conftest.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 15:13:55.240844 dkist-inventory-1.3.0rc1/dkist_inventory/
--rw-rw-rw-   0 root         (0) root         (0)      136 2024-02-26 15:13:26.000000 dkist-inventory-1.3.0rc1/dkist_inventory/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9134 2024-02-26 15:13:26.000000 dkist-inventory-1.3.0rc1/dkist_inventory/asdf_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    13490 2024-02-26 15:13:26.000000 dkist-inventory-1.3.0rc1/dkist_inventory/header_parsing.py
--rw-rw-rw-   0 root         (0) root         (0)    21673 2024-02-26 15:13:26.000000 dkist-inventory-1.3.0rc1/dkist_inventory/inventory.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 15:13:55.244844 dkist-inventory-1.3.0rc1/dkist_inventory/tests/
--rw-rw-rw-   0 root         (0) root         (0)       44 2024-02-26 15:13:26.000000 dkist-inventory-1.3.0rc1/dkist_inventory/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8941 2024-02-26 15:13:26.000000 dkist-inventory-1.3.0rc1/dkist_inventory/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     4069 2024-02-26 15:13:26.000000 dkist-inventory-1.3.0rc1/dkist_inventory/tests/test_asdf_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     3961 2024-02-26 15:13:26.000000 dkist-inventory-1.3.0rc1/dkist_inventory/tests/test_header_parsing.py
--rw-rw-rw-   0 root         (0) root         (0)    21441 2024-02-26 15:13:26.000000 dkist-inventory-1.3.0rc1/dkist_inventory/tests/test_inventory.py
--rw-rw-rw-   0 root         (0) root         (0)    23659 2024-02-26 15:13:26.000000 dkist-inventory-1.3.0rc1/dkist_inventory/tests/test_transforms.py
--rw-rw-rw-   0 root         (0) root         (0)    24250 2024-02-26 15:13:26.000000 dkist-inventory-1.3.0rc1/dkist_inventory/transforms.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2024-02-26 15:13:55.000000 dkist-inventory-1.3.0rc1/dkist_inventory/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 15:13:55.244844 dkist-inventory-1.3.0rc1/dkist_inventory.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2163 2024-02-26 15:13:55.000000 dkist-inventory-1.3.0rc1/dkist_inventory.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      891 2024-02-26 15:13:55.000000 dkist-inventory-1.3.0rc1/dkist_inventory.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-02-26 15:13:55.000000 dkist-inventory-1.3.0rc1/dkist_inventory.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-02-26 15:13:55.000000 dkist-inventory-1.3.0rc1/dkist_inventory.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      329 2024-02-26 15:13:55.000000 dkist-inventory-1.3.0rc1/dkist_inventory.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       16 2024-02-26 15:13:55.000000 dkist-inventory-1.3.0rc1/dkist_inventory.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 15:13:55.244844 dkist-inventory-1.3.0rc1/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2024-02-26 15:13:26.000000 dkist-inventory-1.3.0rc1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     2321 2024-02-26 15:13:26.000000 dkist-inventory-1.3.0rc1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      255 2024-02-26 15:13:26.000000 dkist-inventory-1.3.0rc1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      760 2024-02-26 15:13:26.000000 dkist-inventory-1.3.0rc1/docs/make.bat
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 15:13:55.244844 dkist-inventory-1.3.0rc1/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1482 2024-02-26 15:13:26.000000 dkist-inventory-1.3.0rc1/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-02-26 15:13:26.000000 dkist-inventory-1.3.0rc1/licenses/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1659 2024-02-26 15:13:26.000000 dkist-inventory-1.3.0rc1/licenses/TEMPLATE_LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      134 2024-02-26 15:13:26.000000 dkist-inventory-1.3.0rc1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2954 2024-02-26 15:13:55.248844 dkist-inventory-1.3.0rc1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      603 2024-02-26 15:13:26.000000 dkist-inventory-1.3.0rc1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1073 2024-02-26 15:13:26.000000 dkist-inventory-1.3.0rc1/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 15:20:19.778306 dkist_inventory-1.3.1rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     3019 2024-04-17 15:20:00.000000 dkist_inventory-1.3.1rc1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      333 2024-04-17 15:20:00.000000 dkist_inventory-1.3.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2154 2024-04-17 15:20:19.778306 dkist_inventory-1.3.1rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2024-04-17 15:20:00.000000 dkist_inventory-1.3.1rc1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1579 2024-04-17 15:20:00.000000 dkist_inventory-1.3.1rc1/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2024-04-17 15:20:00.000000 dkist_inventory-1.3.1rc1/conftest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 15:20:19.774306 dkist_inventory-1.3.1rc1/dkist_inventory/
+-rw-rw-rw-   0 root         (0) root         (0)      136 2024-04-17 15:20:00.000000 dkist_inventory-1.3.1rc1/dkist_inventory/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9134 2024-04-17 15:20:00.000000 dkist_inventory-1.3.1rc1/dkist_inventory/asdf_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    13490 2024-04-17 15:20:00.000000 dkist_inventory-1.3.1rc1/dkist_inventory/header_parsing.py
+-rw-rw-rw-   0 root         (0) root         (0)    22044 2024-04-17 15:20:00.000000 dkist_inventory-1.3.1rc1/dkist_inventory/inventory.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 15:20:19.774306 dkist_inventory-1.3.1rc1/dkist_inventory/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2024-04-17 15:20:00.000000 dkist_inventory-1.3.1rc1/dkist_inventory/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8941 2024-04-17 15:20:00.000000 dkist_inventory-1.3.1rc1/dkist_inventory/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4069 2024-04-17 15:20:00.000000 dkist_inventory-1.3.1rc1/dkist_inventory/tests/test_asdf_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3961 2024-04-17 15:20:00.000000 dkist_inventory-1.3.1rc1/dkist_inventory/tests/test_header_parsing.py
+-rw-rw-rw-   0 root         (0) root         (0)    21831 2024-04-17 15:20:00.000000 dkist_inventory-1.3.1rc1/dkist_inventory/tests/test_inventory.py
+-rw-rw-rw-   0 root         (0) root         (0)    23784 2024-04-17 15:20:00.000000 dkist_inventory-1.3.1rc1/dkist_inventory/tests/test_transforms.py
+-rw-rw-rw-   0 root         (0) root         (0)    24250 2024-04-17 15:20:00.000000 dkist_inventory-1.3.1rc1/dkist_inventory/transforms.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2024-04-17 15:20:19.000000 dkist_inventory-1.3.1rc1/dkist_inventory/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 15:20:19.774306 dkist_inventory-1.3.1rc1/dkist_inventory.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2154 2024-04-17 15:20:19.000000 dkist_inventory-1.3.1rc1/dkist_inventory.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      891 2024-04-17 15:20:19.000000 dkist_inventory-1.3.1rc1/dkist_inventory.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-17 15:20:19.000000 dkist_inventory-1.3.1rc1/dkist_inventory.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-17 15:20:19.000000 dkist_inventory-1.3.1rc1/dkist_inventory.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      320 2024-04-17 15:20:19.000000 dkist_inventory-1.3.1rc1/dkist_inventory.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-04-17 15:20:19.000000 dkist_inventory-1.3.1rc1/dkist_inventory.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 15:20:19.774306 dkist_inventory-1.3.1rc1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2024-04-17 15:20:00.000000 dkist_inventory-1.3.1rc1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     2321 2024-04-17 15:20:00.000000 dkist_inventory-1.3.1rc1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      255 2024-04-17 15:20:00.000000 dkist_inventory-1.3.1rc1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      760 2024-04-17 15:20:00.000000 dkist_inventory-1.3.1rc1/docs/make.bat
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 15:20:19.774306 dkist_inventory-1.3.1rc1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2024-04-17 15:20:00.000000 dkist_inventory-1.3.1rc1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-04-17 15:20:00.000000 dkist_inventory-1.3.1rc1/licenses/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2024-04-17 15:20:00.000000 dkist_inventory-1.3.1rc1/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      134 2024-04-17 15:20:00.000000 dkist_inventory-1.3.1rc1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2945 2024-04-17 15:20:19.778306 dkist_inventory-1.3.1rc1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      603 2024-04-17 15:20:00.000000 dkist_inventory-1.3.1rc1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2024-04-17 15:20:00.000000 dkist_inventory-1.3.1rc1/tox.ini
```

### Comparing `dkist-inventory-1.3.0rc1/.gitignore` & `dkist_inventory-1.3.1rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-inventory-1.3.0rc1/PKG-INFO` & `dkist_inventory-1.3.1rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: dkist-inventory
-Version: 1.3.0rc1
+Version: 1.3.1rc1
 Summary: A shared library for dataset inventory and asdf generation.
 Author: NSO / AURA
 Author-email: stuart@cadair.com
 License: BSD 3-Clause
 Requires-Python: >=3.9
 License-File: licenses/LICENSE.rst
 Requires-Dist: astropy>=5.0.4
 Requires-Dist: gwcs>=0.19.0
 Requires-Dist: sunpy[asdf,net]>=2.1
 Requires-Dist: numpy>=1.20
 Requires-Dist: ndcube>=2.0.1
 Requires-Dist: packaging
-Requires-Dist: dkist>=1.4.0rc1
-Requires-Dist: dkist-fits-specifications>=4.1.1rc1
+Requires-Dist: dkist>=1.4.0
+Requires-Dist: dkist-fits-specifications>=4.1.1
 Requires-Dist: scipy>=1.9.0
 Provides-Extra: asdf
 Requires-Dist: asdf; extra == "asdf"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-doctestplus; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
-Requires-Dist: dkist-data-simulator>=5.1.1rc1; extra == "test"
+Requires-Dist: dkist-data-simulator>=5.1.1; extra == "test"
 Requires-Dist: dkist-header-validator; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Requires-Dist: filelock; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-automodapi; extra == "docs"
```

### Comparing `dkist-inventory-1.3.0rc1/README.rst` & `dkist_inventory-1.3.1rc1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-inventory-1.3.0rc1/bitbucket-pipelines.yml` & `dkist_inventory-1.3.1rc1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-inventory-1.3.0rc1/conftest.py` & `dkist_inventory-1.3.1rc1/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-inventory-1.3.0rc1/dkist_inventory/asdf_generator.py` & `dkist_inventory-1.3.1rc1/dkist_inventory/asdf_generator.py`

 * *Files identical despite different names*

### Comparing `dkist-inventory-1.3.0rc1/dkist_inventory/header_parsing.py` & `dkist_inventory-1.3.1rc1/dkist_inventory/header_parsing.py`

 * *Files identical despite different names*

### Comparing `dkist-inventory-1.3.0rc1/dkist_inventory/inventory.py` & `dkist_inventory-1.3.1rc1/dkist_inventory/inventory.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,19 @@
 import scipy.stats
 from astropy.table import Table, Column
 from astropy.time import Time
 
 from dkist_inventory.transforms import TransformBuilder
 from dkist_inventory.header_parsing import HeaderParser
 
-__all__ = ['generate_inventory_from_frame_inventory']
+__all__ = ['generate_inventory_from_frame_inventory', 'generate_asdf_filename']
 
 T = TypeVar('T')
 
+
 def process_json_headers(bucket, json_headers):
     """
     Extract the filenames and FITS headers from the inventory headers.
 
     Parameters
     ----------
     bucket: `str`
@@ -471,21 +472,34 @@
     inventory['averageDatasetSpectralSampling'] = transform_builder.spectral_sampling
     inventory['averageDatasetSpatialSampling'] = transform_builder.spatial_sampling
     inventory['averageDatasetTemporalSampling'] = transform_builder.temporal_sampling
 
     # Calculate the asdfObjectKey
     instrument = inventory['instrumentName'].upper()
     start_time = datetime.datetime.fromisoformat(inventory['startTime'])
-    asdf_filename = f"{instrument}_L1_{start_time:%Y%m%dT%H%M%S}_{inventory['datasetId']}.asdf"
+    asdf_filename = generate_asdf_filename(
+        instrument=instrument,
+        start_time=start_time,
+        dataset_id=inventory['datasetId']
+    )
     inventory[
         "asdfObjectKey"] = f"{inventory['primaryProposalId']}/{inventory['datasetId']}/{asdf_filename}"
 
     return inventory
 
 
+def generate_asdf_filename(instrument: str, start_time: datetime, dataset_id: str):
+    """
+    Generate the filename to use for ASDF files.
+
+    Example: VISP_L1_20240411T142700_ABCDE.asdf
+    """
+    return f"{instrument}_L1_{start_time:%Y%m%dT%H%M%S}_{dataset_id}_user_tools.asdf"
+
+
 # This is the function called by dataset-inventory-maker
 def generate_inventory_from_frame_inventory(bucket: str, json_headers: List[Dict[str, Any]]):
     """
     Generate the complete inventory record from frame inventory.
 
     Parameters
     ----------
```

### Comparing `dkist-inventory-1.3.0rc1/dkist_inventory/tests/conftest.py` & `dkist_inventory-1.3.1rc1/dkist_inventory/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-inventory-1.3.0rc1/dkist_inventory/tests/test_asdf_generator.py` & `dkist_inventory-1.3.1rc1/dkist_inventory/tests/test_asdf_generator.py`

 * *Files identical despite different names*

### Comparing `dkist-inventory-1.3.0rc1/dkist_inventory/tests/test_header_parsing.py` & `dkist_inventory-1.3.1rc1/dkist_inventory/tests/test_header_parsing.py`

 * *Files identical despite different names*

### Comparing `dkist-inventory-1.3.0rc1/dkist_inventory/tests/test_inventory.py` & `dkist_inventory-1.3.1rc1/dkist_inventory/tests/test_inventory.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
                                        _get_unique,
                                        _get_distribution,
                                        _inventory_from_headers,
                                        _inventory_from_wcs, extract_inventory,
                                        generate_inventory_from_frame_inventory,
                                        process_json_headers,
                                        _closest_angle_to_zero,
-                                       Distribution
-)
+                                       Distribution, generate_asdf_filename
+                                       )
 from dkist_inventory.transforms import TransformBuilder
 from dkist_data_simulator.spec214.visp import SimpleVISPDataset
 
 
 
 @pytest.fixture
 def headers_inventory_214_required():
@@ -534,7 +534,14 @@
 
     d3 = _get_distribution([0.0,10,100])
     assert d3 is not None
     assert d3["med"] == 10
     assert d3["p25"] == 5.0 
     assert d3["p75"] == 55.0
 
+
+def test_generate_asdf_filename():
+    instrument = "VBI"
+    start_time = datetime.datetime(2024, 1, 5, 4, 9, 6)
+    dataset_id = "AJFNR"
+    asdf_filename = generate_asdf_filename(instrument=instrument, start_time=start_time, dataset_id=dataset_id)
+    assert asdf_filename == "VBI_L1_20240105T040906_AJFNR_user_tools.asdf"
```

### Comparing `dkist-inventory-1.3.0rc1/dkist_inventory/tests/test_transforms.py` & `dkist_inventory-1.3.1rc1/dkist_inventory/tests/test_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,34 +37,35 @@
 
 
 def test_frames(transform_builder):
     frames = transform_builder.frames
     assert all([isinstance(frame, cf.CoordinateFrame) for frame in frames])
 
 
-def test_roundtrip(wcs, dataset_name):
-    """
-    Test that a pixel>world>pixel transformation gives the same outputs as inputs.
-
-    This asserts that the forward and backwards transforms run without error.
-    """
-    # Known gwcs issue due to axis ordering
-    if dataset_name in (
-        "visp",
-        "visp-time-varying-single",
-        "visp-time-varying-multi",
-        "cryonirsp-sp-multi-meas-no-stokes",
-        "cryonirsp-sp-multi-meas-stokes",
-    ):
-        pytest.importorskip("gwcs", minversion="0.21.0.dev0")
-
-    pixel_inputs = [0] * wcs.pixel_n_dim
-    world_outputs = wcs.pixel_to_world_values(*pixel_inputs)
-    pixel_outputs = wcs.world_to_pixel_values(*world_outputs)
-    assert np.allclose(pixel_inputs, pixel_outputs, atol=1e-6)
+# TODO this test is dependent on a gwcs fix that has not been merged as of gwcs=0.21.0
+# def test_roundtrip(wcs, dataset_name):
+#     """
+#     Test that a pixel>world>pixel transformation gives the same outputs as inputs.
+#
+#     This asserts that the forward and backwards transforms run without error.
+#     """
+#     # Known gwcs issue due to axis ordering
+#     if dataset_name in (
+#         "visp",
+#         "visp-time-varying-single",
+#         "visp-time-varying-multi",
+#         "cryonirsp-sp-multi-meas-no-stokes",
+#         "cryonirsp-sp-multi-meas-stokes",
+#     ):
+#         pytest.importorskip("gwcs", minversion="0.21.0.dev0")
+#
+#     pixel_inputs = [0] * wcs.pixel_n_dim
+#     world_outputs = wcs.pixel_to_world_values(*pixel_inputs)
+#     pixel_outputs = wcs.world_to_pixel_values(*world_outputs)
+#     assert np.allclose(pixel_inputs, pixel_outputs, atol=1e-6)
 
 
 def test_input_name_ordering(transform_builder):
     # Check the ordering of the input and output frames
     wcs = transform_builder.gwcs
     allowed_pixel_names = {
         "VISP": (
```

### Comparing `dkist-inventory-1.3.0rc1/dkist_inventory/transforms.py` & `dkist_inventory-1.3.1rc1/dkist_inventory/transforms.py`

 * *Files identical despite different names*

### Comparing `dkist-inventory-1.3.0rc1/dkist_inventory.egg-info/PKG-INFO` & `dkist_inventory-1.3.1rc1/dkist_inventory.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: dkist-inventory
-Version: 1.3.0rc1
+Version: 1.3.1rc1
 Summary: A shared library for dataset inventory and asdf generation.
 Author: NSO / AURA
 Author-email: stuart@cadair.com
 License: BSD 3-Clause
 Requires-Python: >=3.9
 License-File: licenses/LICENSE.rst
 Requires-Dist: astropy>=5.0.4
 Requires-Dist: gwcs>=0.19.0
 Requires-Dist: sunpy[asdf,net]>=2.1
 Requires-Dist: numpy>=1.20
 Requires-Dist: ndcube>=2.0.1
 Requires-Dist: packaging
-Requires-Dist: dkist>=1.4.0rc1
-Requires-Dist: dkist-fits-specifications>=4.1.1rc1
+Requires-Dist: dkist>=1.4.0
+Requires-Dist: dkist-fits-specifications>=4.1.1
 Requires-Dist: scipy>=1.9.0
 Provides-Extra: asdf
 Requires-Dist: asdf; extra == "asdf"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-doctestplus; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
-Requires-Dist: dkist-data-simulator>=5.1.1rc1; extra == "test"
+Requires-Dist: dkist-data-simulator>=5.1.1; extra == "test"
 Requires-Dist: dkist-header-validator; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Requires-Dist: filelock; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-automodapi; extra == "docs"
```

### Comparing `dkist-inventory-1.3.0rc1/dkist_inventory.egg-info/SOURCES.txt` & `dkist_inventory-1.3.1rc1/dkist_inventory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist-inventory-1.3.0rc1/docs/Makefile` & `dkist_inventory-1.3.1rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-inventory-1.3.0rc1/docs/conf.py` & `dkist_inventory-1.3.1rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-inventory-1.3.0rc1/docs/make.bat` & `dkist_inventory-1.3.1rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-inventory-1.3.0rc1/licenses/LICENSE.rst` & `dkist_inventory-1.3.1rc1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-inventory-1.3.0rc1/licenses/TEMPLATE_LICENSE.rst` & `dkist_inventory-1.3.1rc1/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-inventory-1.3.0rc1/setup.cfg` & `dkist_inventory-1.3.1rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 install_requires = 
 	astropy>=5.0.4
 	gwcs>=0.19.0
 	sunpy[net,asdf]>=2.1
 	numpy>=1.20  # For numpy typing support
 	ndcube>=2.0.1
 	packaging
-	dkist>=1.4.0rc1
-	dkist-fits-specifications>=4.1.1rc1
+	dkist>=1.4.0
+	dkist-fits-specifications>=4.1.1
 	scipy>=1.9.0
 
 [options.extras_require]
 asdf = 
 	asdf
 test = 
 	pytest
 	pytest-doctestplus
 	pytest-cov
 	pytest-xdist
-	dkist-data-simulator>=5.1.1rc1
+	dkist-data-simulator>=5.1.1
 	dkist-header-validator
 	pytest-mock
 	filelock
 docs = 
 	sphinx
 	sphinx-automodapi
```

### Comparing `dkist-inventory-1.3.0rc1/setup.py` & `dkist_inventory-1.3.1rc1/setup.py`

 * *Files identical despite different names*

### Comparing `dkist-inventory-1.3.0rc1/tox.ini` & `dkist_inventory-1.3.1rc1/tox.ini`

 * *Files identical despite different names*

