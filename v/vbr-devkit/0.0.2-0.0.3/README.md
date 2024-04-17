# Comparing `tmp/vbr_devkit-0.0.2.tar.gz` & `tmp/vbr_devkit-0.0.3.tar.gz`

## Comparing `vbr_devkit-0.0.2.tar` & `vbr_devkit-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 vbr_devkit-0.0.2/vbr_devkit/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 vbr_devkit-0.0.2/vbr_devkit/datasets/__init__.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 vbr_devkit-0.0.2/vbr_devkit/datasets/convert_bag.py
--rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 vbr_devkit-0.0.2/vbr_devkit/datasets/kitti.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 vbr_devkit-0.0.2/vbr_devkit/datasets/ros.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vbr_devkit-0.0.2/vbr_devkit/download/__init__.py
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 vbr_devkit-0.0.2/vbr_devkit/download/download_data.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 vbr_devkit-0.0.2/vbr_devkit/pybind/CMakeLists.txt
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 vbr_devkit-0.0.2/vbr_devkit/pybind/stl_vector_eigen.h
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 vbr_devkit-0.0.2/vbr_devkit/pybind/vbr_devkit_pybind.cpp
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 vbr_devkit-0.0.2/vbr_devkit/tools/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 vbr_devkit-0.0.2/vbr_devkit/tools/console.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 vbr_devkit-0.0.2/vbr_devkit/tools/image.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 vbr_devkit-0.0.2/vbr_devkit/tools/imu.py
--rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 vbr_devkit-0.0.2/vbr_devkit/tools/point_cloud2.py
--rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 vbr_devkit-0.0.2/vbr_devkit/tools/run.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 vbr_devkit-0.0.2/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 vbr_devkit-0.0.2/LICENSE
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 vbr_devkit-0.0.2/README.md
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 vbr_devkit-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 vbr_devkit-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/datasets/__init__.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/datasets/convert_bag.py
+-rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/datasets/kitti.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/datasets/ros.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/download/__init__.py
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/download/download_data.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/pybind/CMakeLists.txt
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/pybind/stl_vector_eigen.h
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/pybind/vbr_devkit_pybind.cpp
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/tools/__init__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/tools/console.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/tools/image.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/tools/imu.py
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/tools/point_cloud2.py
+-rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/vbr_devkit/tools/run.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/README.md
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 vbr_devkit-0.0.3/PKG-INFO
```

### Comparing `vbr_devkit-0.0.2/vbr_devkit/datasets/convert_bag.py` & `vbr_devkit-0.0.3/vbr_devkit/datasets/convert_bag.py`

 * *Files identical despite different names*

### Comparing `vbr_devkit-0.0.2/vbr_devkit/datasets/kitti.py` & `vbr_devkit-0.0.3/vbr_devkit/datasets/kitti.py`

 * *Files identical despite different names*

### Comparing `vbr_devkit-0.0.2/vbr_devkit/datasets/ros.py` & `vbr_devkit-0.0.3/vbr_devkit/datasets/ros.py`

 * *Files identical despite different names*

### Comparing `vbr_devkit-0.0.2/vbr_devkit/download/download_data.py` & `vbr_devkit-0.0.3/vbr_devkit/download/download_data.py`

 * *Files identical despite different names*

### Comparing `vbr_devkit-0.0.2/vbr_devkit/pybind/CMakeLists.txt` & `vbr_devkit-0.0.3/vbr_devkit/pybind/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vbr_devkit-0.0.2/vbr_devkit/pybind/stl_vector_eigen.h` & `vbr_devkit-0.0.3/vbr_devkit/pybind/stl_vector_eigen.h`

 * *Files identical despite different names*

### Comparing `vbr_devkit-0.0.2/vbr_devkit/pybind/vbr_devkit_pybind.cpp` & `vbr_devkit-0.0.3/vbr_devkit/pybind/vbr_devkit_pybind.cpp`

 * *Files identical despite different names*

### Comparing `vbr_devkit-0.0.2/vbr_devkit/tools/__init__.py` & `vbr_devkit-0.0.3/vbr_devkit/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `vbr_devkit-0.0.2/vbr_devkit/tools/image.py` & `vbr_devkit-0.0.3/vbr_devkit/tools/image.py`

 * *Files identical despite different names*

### Comparing `vbr_devkit-0.0.2/vbr_devkit/tools/imu.py` & `vbr_devkit-0.0.3/vbr_devkit/tools/imu.py`

 * *Files identical despite different names*

### Comparing `vbr_devkit-0.0.2/vbr_devkit/tools/point_cloud2.py` & `vbr_devkit-0.0.3/vbr_devkit/tools/point_cloud2.py`

 * *Files identical despite different names*

### Comparing `vbr_devkit-0.0.2/vbr_devkit/tools/run.py` & `vbr_devkit-0.0.3/vbr_devkit/tools/run.py`

 * *Files identical despite different names*

### Comparing `vbr_devkit-0.0.2/LICENSE` & `vbr_devkit-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vbr_devkit-0.0.2/README.md` & `vbr_devkit-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `vbr_devkit-0.0.2/pyproject.toml` & `vbr_devkit-0.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "vbr-devkit"
-version = "0.0.2"
+version = "0.0.3"
 description = "Development kit for VBR SLAM dataset"
 readme = "README.md"
 authors = [
     { name = "Emanuele Giacomini", email = "giacomini@diag.uniroma1.it" },
 ]
 requires-python = ">=3.8"
 
@@ -21,15 +21,16 @@
 ]
 
 dependencies = [
     "natsort",
     "numpy",
     "rich",
     "typer[all]>=0.10.0",
-    "rosbags"
+    "rosbags",
+    "rosbags.image"
 ]
 
 [project.scripts]
 vbr = "vbr_devkit.tools.run:app"
 
 [project.urls]
 Homepage = "https://github.com/rvp-group/vbr-devkit"
```

### Comparing `vbr_devkit-0.0.2/PKG-INFO` & `vbr_devkit-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.3
 Name: vbr-devkit
-Version: 0.0.2
+Version: 0.0.3
 Summary: Development kit for VBR SLAM dataset
 Project-URL: Homepage, https://github.com/rvp-group/vbr-devkit
 Project-URL: Issues, https://github.com/rvp-group/vbr-devkit/issues
 Author-email: Emanuele Giacomini <giacomini@diag.uniroma1.it>
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: natsort
 Requires-Dist: numpy
 Requires-Dist: rich
 Requires-Dist: rosbags
+Requires-Dist: rosbags-image
 Requires-Dist: typer[all]>=0.10.0
 Description-Content-Type: text/markdown
 
 <div align="center">
     <h1>VBR Development Kit</h1>
     <a href=""><img src=https://github.com/rvp-group/vbr-devkit/actions/workflows/python.yml/badge.svg /></a>
     <a href=""><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/vbr-devkit" /></a>
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
-Metadata-Version: 2.3 Name: vbr-devkit Version: 0.0.2 Summary: Development kit
+Metadata-Version: 2.3 Name: vbr-devkit Version: 0.0.3 Summary: Development kit
 for VBR SLAM dataset Project-URL: Homepage, https://github.com/rvp-group/vbr-
 devkit Project-URL: Issues, https://github.com/rvp-group/vbr-devkit/issues
 Author-email: Emanuele Giacomini
 diag.uniroma1.it> License-File: LICENSE Requires-Python: >=3.8 Requires-Dist:
 natsort Requires-Dist: numpy Requires-Dist: rich Requires-Dist: rosbags
-Requires-Dist: typer[all]>=0.10.0 Description-Content-Type: text/markdown
+Requires-Dist: rosbags-image Requires-Dist: typer[all]>=0.10.0 Description-
+Content-Type: text/markdown
                        ************ VVBBRR DDeevveellooppmmeenntt KKiitt ************
     [https://github.com/rvp-group/vbr-devkit/actions/workflows/python.yml/
                  badge.svg][PyPI - Version][PyPI - Downloads]
 
   _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_r_v_p_-_g_r_o_u_p_/_v_b_r_-_d_e_v_k_i_t_/_a_s_s_e_t_s_/_5_3_0_5_5_3_0_/_f_1_a_8_d_2_2_a_-_a_f_1_e_-_4_2_d_4_-
                               _b_2_9_6_-_d_9_4_0_2_1_a_9_8_0_c_f_]
 This kit contains utilities to work on the VBR SLAM dataset # Install ```shell
```

