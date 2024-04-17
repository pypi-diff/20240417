# Comparing `tmp/faim_wako_searchfirst-0.7.1.tar.gz` & `tmp/faim_wako_searchfirst-0.8.0.tar.gz`

## Comparing `faim_wako_searchfirst-0.7.1.tar` & `faim_wako_searchfirst-0.8.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/config.yml
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/config_cellpose.yml
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/.github/workflows/deploy.yml
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/LICENSES/MIT.txt
--rw-r--r--   0        0        0   167410 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/presentations/faim-wako-searchfirst_overview.pdf
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/presentations/faim-wako-searchfirst_overview.pdf.license
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/scripts/Visualize_Sampling.groovy
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/scripts/searchfirst.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/src/faim_wako_searchfirst/__init__.py
--rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/src/faim_wako_searchfirst/filter.py
--rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/src/faim_wako_searchfirst/main.py
--rw-r--r--   0        0        0     7736 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/src/faim_wako_searchfirst/sample.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/src/faim_wako_searchfirst/segment.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/__init__.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/test_cellpose.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/test_filter.py
--rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/test_main.py
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/test_sample.py
--rw-r--r--   0        0        0    43316 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/resources/simple_labels.tif
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/resources/simple_labels.tif.license
--rw-r--r--   0        0        0    65696 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/resources/TestSet/Other_name_D07_T0001F002L01A02Z01C01.tif
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/resources/TestSet/Other_name_D07_T0001F002L01A02Z01C01.tif.license
--rw-r--r--   0        0        0    65696 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/resources/TestSet/TestSet_C03_T0001F002L01A03Z01C03.tif
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/resources/TestSet/TestSet_C03_T0001F002L01A03Z01C03.tif.license
--rw-r--r--   0        0        0    65696 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/resources/TestSet/TestSet_D07_T0001F002L01A02Z01C01.tif
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/resources/TestSet/TestSet_D07_T0001F002L01A02Z01C01.tif.license
--rw-r--r--   0        0        0    65696 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/resources/TestSet/TestSet_D07_T0001F002L01A03Z01C03.tif
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/resources/TestSet/TestSet_D07_T0001F002L01A03Z01C03.tif.license
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/.gitignore
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/README.md
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/config.yml
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/config_cellpose.yml
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/LICENSES/MIT.txt
+-rw-r--r--   0        0        0   167410 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/presentations/faim-wako-searchfirst_overview.pdf
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/presentations/faim-wako-searchfirst_overview.pdf.license
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/scripts/Visualize_Sampling.groovy
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/scripts/searchfirst.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/src/faim_wako_searchfirst/__init__.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/src/faim_wako_searchfirst/filter.py
+-rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/src/faim_wako_searchfirst/main.py
+-rw-r--r--   0        0        0     7736 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/src/faim_wako_searchfirst/sample.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/src/faim_wako_searchfirst/segment.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/tests/test_cellpose.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/tests/test_filter.py
+-rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/tests/test_main.py
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/tests/test_sample.py
+-rw-r--r--   0        0        0    43316 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/tests/resources/simple_labels.tif
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/tests/resources/simple_labels.tif.license
+-rw-r--r--   0        0        0    65696 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/tests/resources/TestSet/Other_name_D07_T0001F002L01A02Z01C01.tif
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/tests/resources/TestSet/Other_name_D07_T0001F002L01A02Z01C01.tif.license
+-rw-r--r--   0        0        0    65696 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/tests/resources/TestSet/TestSet_C03_T0001F002L01A03Z01C03.tif
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/tests/resources/TestSet/TestSet_C03_T0001F002L01A03Z01C03.tif.license
+-rw-r--r--   0        0        0    65696 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/tests/resources/TestSet/TestSet_D07_T0001F002L01A02Z01C01.tif
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/tests/resources/TestSet/TestSet_D07_T0001F002L01A02Z01C01.tif.license
+-rw-r--r--   0        0        0    65696 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/tests/resources/TestSet/TestSet_D07_T0001F002L01A03Z01C03.tif
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/tests/resources/TestSet/TestSet_D07_T0001F002L01A03Z01C03.tif.license
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/.gitignore
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/README.md
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.8.0/PKG-INFO
```

### Comparing `faim_wako_searchfirst-0.7.1/config.yml` & `faim_wako_searchfirst-0.8.0/config.yml`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 file_selection:
     channel: C01
 
 # choose method how to segment, filter, and sample the objects
 process:
     # segment methods: threshold, cellpose
     segment: threshold
-    # filter methods: bounding_box, area, solidity, intensity
-    filter: [bounding_box, area, solidity, feature, intensity, dilate]
+    # filter methods: bounding_box, area, solidity, feature, border, intensity, dilate
+    filter: [bounding_box, area, solidity, feature, border, intensity, dilate]
     # sample methods: centers, grid_overlap, dense_grid,
     #                 object_centered_grid, region_centered_grid
     sample: centers
 
 # Each section below provides arguments to one of the methods set in 'process'.
 # Config sections for methods not selected above will be ignored.
 
@@ -40,19 +40,21 @@
 solidity:
     min_solidity: 0.9
     max_solidity: 1.0
 feature:
     feature: eccentricity
     min_value: 0.0
     max_value: 0.99
-dilate:
-    pixel_distance: 1.0
+border:
+    margin: 5  # default: 0
 intensity:
     target_channel: C03
     min_intensity: 128
+dilate:
+    pixel_distance: 1.0
 
 # sample
 dense_grid:
     binning_factor: 50  # default: 50
 grid_overlap:
     mag_first_pass: 4
     mag_second_pass: 60
```

### Comparing `faim_wako_searchfirst-0.7.1/config_cellpose.yml` & `faim_wako_searchfirst-0.8.0/config_cellpose.yml`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.7.1/.github/workflows/deploy.yml` & `faim_wako_searchfirst-0.8.0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.7.1/.github/workflows/test.yml` & `faim_wako_searchfirst-0.8.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.7.1/LICENSES/MIT.txt` & `faim_wako_searchfirst-0.8.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.7.1/presentations/faim-wako-searchfirst_overview.pdf` & `faim_wako_searchfirst-0.8.0/presentations/faim-wako-searchfirst_overview.pdf`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.7.1/scripts/Visualize_Sampling.groovy` & `faim_wako_searchfirst-0.8.0/scripts/Visualize_Sampling.groovy`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.7.1/scripts/searchfirst.py` & `faim_wako_searchfirst-0.8.0/scripts/searchfirst.py`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.7.1/src/faim_wako_searchfirst/filter.py` & `faim_wako_searchfirst-0.8.0/src/faim_wako_searchfirst/filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import re
 from pathlib import Path
 
 from numpy import ndarray
 from skimage.measure import regionprops
-from skimage.segmentation import expand_labels
+from skimage.segmentation import clear_border, expand_labels
 from tifffile import imread
 
 
 def bounding_box(tif_file: Path, labels, min_x: int, min_y: int, max_x: int, max_y: int):
     """Modify 'labels' to set everything outside the bounding box to zero."""
     labels[0 : max(min_y, 0), :] = 0
     labels[:, 0 : max(min_x, 0)] = 0
@@ -67,14 +67,23 @@
     """Modify 'labels' to only keep objects within range."""
     regions = regionprops(labels)
     for region in regions:
         if not min_solidity <= region.solidity <= max_solidity:
             labels[labels == region.label] = 0
 
 
+def border(
+    tif_file: Path,
+    labels: ndarray,
+    margin: int = 0,
+):
+    """Modify 'labels' to discard objects touching the image border."""
+    labels[:] = clear_border(labels=labels, buffer_size=margin)
+
+
 def dilate(
     tif_file: Path,
     labels: ndarray,
     pixel_distance: float = 10.0,
 ):
     """Dilate objects by specified amount."""
     labels[:] = expand_labels(label_image=labels, distance=pixel_distance)
@@ -82,15 +91,15 @@
 
 def intensity(
     tif_file: Path,
     labels: ndarray,
     target_channel: str,
     min_intensity: int,
 ):
-    """Filter objects in 'labels' using the provided function."""
+    """Filter objects in 'labels' by intensity in other channel."""
     intensity_image = imread(_get_other_channel_file(tif_file, target_channel))
     _filter_objects_by_intensity(labels, intensity_image, min_intensity)
 
 
 def _get_other_channel_file(tif_file: Path, target_channel: str) -> Path:
     """Detect the file of target channel with the same well and field as the given 'tif_file'."""
     pattern = re.compile(r"(.*_[A-Z]\d{2}_T\d{4}F\d{3}L\d{2})(A\d{2})(Z\d{2})(C\d{2})\.tif")
```

### Comparing `faim_wako_searchfirst-0.7.1/src/faim_wako_searchfirst/main.py` & `faim_wako_searchfirst-0.8.0/src/faim_wako_searchfirst/main.py`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.7.1/src/faim_wako_searchfirst/sample.py` & `faim_wako_searchfirst-0.8.0/src/faim_wako_searchfirst/sample.py`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.7.1/src/faim_wako_searchfirst/segment.py` & `faim_wako_searchfirst-0.8.0/src/faim_wako_searchfirst/segment.py`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.7.1/tests/test_cellpose.py` & `faim_wako_searchfirst-0.8.0/tests/test_cellpose.py`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.7.1/tests/test_filter.py` & `faim_wako_searchfirst-0.8.0/tests/test_filter.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 """Test faim_wako_searchfirst.filter module."""
 
 from pathlib import Path
 
 import numpy as np
 import pytest
-from faim_wako_searchfirst.filter import dilate, feature
+from faim_wako_searchfirst.filter import border, dilate, feature
 from skimage.io import imread
 
 
 @pytest.fixture
 def _label_image():
     return imread(Path("tests") / "resources" / "simple_labels.tif")
 
@@ -26,14 +26,26 @@
         feature="solidity",
         min_value=0.9,
         max_value=1.0,
     )
     assert np.unique(labels).tolist() == [0, 2, 3, 4]
 
 
+def test_border(_label_image: np.ndarray):
+    """Test discard border objects."""
+    labels = _label_image.copy()
+    assert np.unique(labels).tolist() == [0, 1, 2, 3, 4]
+    border(
+        tif_file=None,
+        labels=labels,
+        margin=15,
+    )
+    assert np.unique(labels).tolist() == [0, 3, 4]
+
+
 def test_dilate(_label_image: np.ndarray):
     """Test oject dilation."""
     labels = _label_image.copy()
     assert np.sum(labels[labels == 1]) == 1353
     dilate(
         tif_file=None,
         labels=labels,
```

### Comparing `faim_wako_searchfirst-0.7.1/tests/test_main.py` & `faim_wako_searchfirst-0.8.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.7.1/tests/test_sample.py` & `faim_wako_searchfirst-0.8.0/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.7.1/tests/resources/simple_labels.tif` & `faim_wako_searchfirst-0.8.0/tests/resources/simple_labels.tif`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.7.1/tests/resources/TestSet/Other_name_D07_T0001F002L01A02Z01C01.tif` & `faim_wako_searchfirst-0.8.0/tests/resources/TestSet/Other_name_D07_T0001F002L01A02Z01C01.tif`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.7.1/tests/resources/TestSet/TestSet_C03_T0001F002L01A03Z01C03.tif` & `faim_wako_searchfirst-0.8.0/tests/resources/TestSet/TestSet_C03_T0001F002L01A03Z01C03.tif`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.7.1/tests/resources/TestSet/TestSet_D07_T0001F002L01A02Z01C01.tif` & `faim_wako_searchfirst-0.8.0/tests/resources/TestSet/TestSet_D07_T0001F002L01A02Z01C01.tif`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.7.1/tests/resources/TestSet/TestSet_D07_T0001F002L01A03Z01C03.tif` & `faim_wako_searchfirst-0.8.0/tests/resources/TestSet/TestSet_D07_T0001F002L01A03Z01C03.tif`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.7.1/README.md` & `faim_wako_searchfirst-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -38,16 +38,16 @@
 file_selection:
     channel: C01
 
 # choose method how to segment, filter, and sample the objects
 process:
     # segment methods: threshold, cellpose
     segment: threshold
-    # filter methods: bounding_box, area, solidity, intensity
-    filter: [bounding_box, area, solidity, feature, dilate, intensity]
+    # filter methods: bounding_box, area, solidity, feature, border, intensity, dilate
+    filter: [bounding_box, area, solidity, feature, border, intensity, dilate]
     # sample methods: centers, grid_overlap, dense_grid,
     #                 object_centered_grid, region_centered_grid
     sample: centers
 
 # Each section below provides arguments to one of the methods set in 'process'.
 # Config sections for methods not selected above will be ignored.
 
@@ -69,19 +69,21 @@
 solidity:
     min_solidity: 0.9
     max_solidity: 1.0
 feature:
     feature: eccentricity
     min_value: 0.0
     max_value: 0.99
-dilate:
-    pixel_distance: 1.0
+border:
+    margin: 5  # default: 0
 intensity:
     target_channel: C03
     min_intensity: 128
+dilate:
+    pixel_distance: 1.0
 
 # sample
 dense_grid:
     binning_factor: 50  # default: 50
 grid_overlap:
     mag_first_pass: 4
     mag_second_pass: 60
```

### Comparing `faim_wako_searchfirst-0.7.1/pyproject.toml` & `faim_wako_searchfirst-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.7.1/PKG-INFO` & `faim_wako_searchfirst-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: faim-wako-searchfirst
-Version: 0.7.1
+Version: 0.8.0
 Project-URL: Documentation, https://github.com/fmi-faim/faim-wako-searchfirst#readme
 Project-URL: Issues, https://github.com/fmi-faim/faim-wako-searchfirst/issues
 Project-URL: Source, https://github.com/fmi-faim/faim-wako-searchfirst
 Author-email: Jan Eglinger <jan.eglinger@fmi.ch>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -63,16 +63,16 @@
 file_selection:
     channel: C01
 
 # choose method how to segment, filter, and sample the objects
 process:
     # segment methods: threshold, cellpose
     segment: threshold
-    # filter methods: bounding_box, area, solidity, intensity
-    filter: [bounding_box, area, solidity, feature, dilate, intensity]
+    # filter methods: bounding_box, area, solidity, feature, border, intensity, dilate
+    filter: [bounding_box, area, solidity, feature, border, intensity, dilate]
     # sample methods: centers, grid_overlap, dense_grid,
     #                 object_centered_grid, region_centered_grid
     sample: centers
 
 # Each section below provides arguments to one of the methods set in 'process'.
 # Config sections for methods not selected above will be ignored.
 
@@ -94,19 +94,21 @@
 solidity:
     min_solidity: 0.9
     max_solidity: 1.0
 feature:
     feature: eccentricity
     min_value: 0.0
     max_value: 0.99
-dilate:
-    pixel_distance: 1.0
+border:
+    margin: 5  # default: 0
 intensity:
     target_channel: C03
     min_intensity: 128
+dilate:
+    pixel_distance: 1.0
 
 # sample
 dense_grid:
     binning_factor: 50  # default: 50
 grid_overlap:
     mag_first_pass: 4
     mag_second_pass: 60
```

