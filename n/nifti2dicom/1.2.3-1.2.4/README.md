# Comparing `tmp/nifti2dicom-1.2.3.tar.gz` & `tmp/nifti2dicom-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nifti2dicom-1.2.3.tar", last modified: Wed Apr 10 13:06:13 2024, max compression
+gzip compressed data, was "nifti2dicom-1.2.4.tar", last modified: Wed Apr 17 15:21:02 2024, max compression
```

## Comparing `nifti2dicom-1.2.3.tar` & `nifti2dicom-1.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:06:13.130909 nifti2dicom-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 13:06:09.000000 nifti2dicom-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-04-10 13:06:13.130909 nifti2dicom-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-04-10 13:06:09.000000 nifti2dicom-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:06:13.130909 nifti2dicom-1.2.3/nifti2dicom/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-10 13:06:09.000000 nifti2dicom-1.2.3/nifti2dicom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-10 13:06:09.000000 nifti2dicom-1.2.3/nifti2dicom/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    30015 2024-04-10 13:06:09.000000 nifti2dicom-1.2.3/nifti2dicom/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-10 13:06:09.000000 nifti2dicom-1.2.3/nifti2dicom/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-04-10 13:06:09.000000 nifti2dicom-1.2.3/nifti2dicom/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:06:13.130909 nifti2dicom-1.2.3/nifti2dicom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-04-10 13:06:13.000000 nifti2dicom-1.2.3/nifti2dicom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-10 13:06:13.000000 nifti2dicom-1.2.3/nifti2dicom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:06:13.000000 nifti2dicom-1.2.3/nifti2dicom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-10 13:06:13.000000 nifti2dicom-1.2.3/nifti2dicom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-10 13:06:13.000000 nifti2dicom-1.2.3/nifti2dicom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 13:06:13.000000 nifti2dicom-1.2.3/nifti2dicom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 13:06:13.130909 nifti2dicom-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-10 13:06:09.000000 nifti2dicom-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:21:02.651372 nifti2dicom-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-17 15:20:58.000000 nifti2dicom-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-04-17 15:21:02.651372 nifti2dicom-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-04-17 15:20:58.000000 nifti2dicom-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:21:02.647372 nifti2dicom-1.2.4/nifti2dicom/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-17 15:20:58.000000 nifti2dicom-1.2.4/nifti2dicom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-17 15:20:58.000000 nifti2dicom-1.2.4/nifti2dicom/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30619 2024-04-17 15:20:58.000000 nifti2dicom-1.2.4/nifti2dicom/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-17 15:20:58.000000 nifti2dicom-1.2.4/nifti2dicom/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-04-17 15:20:58.000000 nifti2dicom-1.2.4/nifti2dicom/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:21:02.651372 nifti2dicom-1.2.4/nifti2dicom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-04-17 15:21:02.000000 nifti2dicom-1.2.4/nifti2dicom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-17 15:21:02.000000 nifti2dicom-1.2.4/nifti2dicom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 15:21:02.000000 nifti2dicom-1.2.4/nifti2dicom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-17 15:21:02.000000 nifti2dicom-1.2.4/nifti2dicom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-17 15:21:02.000000 nifti2dicom-1.2.4/nifti2dicom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 15:21:02.000000 nifti2dicom-1.2.4/nifti2dicom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 15:21:02.651372 nifti2dicom-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-17 15:20:58.000000 nifti2dicom-1.2.4/setup.py
```

### Comparing `nifti2dicom-1.2.3/LICENSE` & `nifti2dicom-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nifti2dicom-1.2.3/PKG-INFO` & `nifti2dicom-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifti2dicom
-Version: 1.2.3
+Version: 1.2.4
 Summary: A package to convert NIfTI images to DICOM format using a reference DICOM series.
 Author: Lalith Kumar Shiyam Sundar
 License: MIT
 Keywords: nifti dicom converter
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydicom
```

### Comparing `nifti2dicom-1.2.3/README.md` & `nifti2dicom-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `nifti2dicom-1.2.3/nifti2dicom/constants.py` & `nifti2dicom-1.2.4/nifti2dicom/constants.py`

 * *Files identical despite different names*

### Comparing `nifti2dicom-1.2.3/nifti2dicom/converter.py` & `nifti2dicom-1.2.4/nifti2dicom/converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -189,15 +189,22 @@
     """
 
     if not os.path.exists(output_directory):
         os.makedirs(output_directory)
 
     metadata = get_metadata_from_dicom_series(reference_dicom_series)
 
+    # Load the dicom series
+
+    dicom_reference_img = load_image(reference_dicom_series, 'dicom')
+
     rgb_img = sitk.ReadImage(nifti_file_path)
+    # set rgb_img origin and direction to match the dicom series
+    rgb_img.SetOrigin(dicom_reference_img.GetOrigin())
+    rgb_img.SetDirection(dicom_reference_img.GetDirection())
     arr = sitk.GetArrayFromImage(rgb_img)
     arr = arr[:, :, :, :3]  # Ensure only RGB, no alpha
 
     modification_time = time.strftime("%H%M%S")
     modification_date = time.strftime("%Y%m%d")
 
     # Define DICOM series and study attributes
@@ -209,14 +216,19 @@
     }
     total_slices = len(arr)
     with Progress() as progress:
         task = progress.add_task("[cyan]Writing DICOM slices...", total=total_slices)
         for i, slice_array in enumerate(arr, start=1):
             ds = create_rgb_dicom_from_slice(slice_array, series_tag_values, metadata, i)
             dicom_filename = os.path.join(output_directory, f"slice_{i}.dcm")
+            ds.ImageOrientationPatient = metadata.ImageOrientationPatient
+            ds.ImagePositionPatient = list(rgb_img.TransformIndexToPhysicalPoint((0, 0, i)))
+            ds.PatientName = metadata.PatientName
+            ds.PatientID = metadata.PatientID
+            ds.PatientBirthDate = metadata.PatientBirthDate
             write_file(dicom_filename, ds, write_like_original=False)
             progress.update(task, advance=1, description=f"[white] Writing RGB DICOM slices... [{i}/{total_slices}]")
 
 
 def check_directory_exists(directory: str) -> None:
     """
     Checks if the specified directory exists.
```

### Comparing `nifti2dicom-1.2.3/nifti2dicom/display.py` & `nifti2dicom-1.2.4/nifti2dicom/display.py`

 * *Files identical despite different names*

### Comparing `nifti2dicom-1.2.3/nifti2dicom/viewer.py` & `nifti2dicom-1.2.4/nifti2dicom/viewer.py`

 * *Files identical despite different names*

### Comparing `nifti2dicom-1.2.3/nifti2dicom.egg-info/PKG-INFO` & `nifti2dicom-1.2.4/nifti2dicom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifti2dicom
-Version: 1.2.3
+Version: 1.2.4
 Summary: A package to convert NIfTI images to DICOM format using a reference DICOM series.
 Author: Lalith Kumar Shiyam Sundar
 License: MIT
 Keywords: nifti dicom converter
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydicom
```

### Comparing `nifti2dicom-1.2.3/setup.py` & `nifti2dicom-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='nifti2dicom',
-    version='1.2.3',
+    version='1.2.4',
     packages=find_packages(),
     install_requires=[
         'pydicom',
         'nibabel',
         'numpy',
         'emoji',
         'rich',
```

