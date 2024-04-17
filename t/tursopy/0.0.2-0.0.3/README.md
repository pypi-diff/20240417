# Comparing `tmp/tursopy-0.0.2.tar.gz` & `tmp/tursopy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tursopy-0.0.2.tar", last modified: Fri Apr 12 01:16:32 2024, max compression
+gzip compressed data, was "tursopy-0.0.3.tar", last modified: Wed Apr 17 06:00:27 2024, max compression
```

## Comparing `tursopy-0.0.2.tar` & `tursopy-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:16:32.649390 tursopy-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-12 01:16:08.000000 tursopy-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-12 01:16:32.649390 tursopy-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-12 01:16:08.000000 tursopy-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-12 01:16:30.000000 tursopy-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 01:16:32.649390 tursopy-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:16:32.645390 tursopy-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-12 01:16:08.000000 tursopy-0.0.2/tests/test_tursopy_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10258 2024-04-12 01:16:08.000000 tursopy-0.0.2/tests/test_tursopy_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:16:32.645390 tursopy-0.0.2/tursopy/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-12 01:16:08.000000 tursopy-0.0.2/tursopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-12 01:16:08.000000 tursopy-0.0.2/tursopy/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)    14537 2024-04-12 01:16:08.000000 tursopy-0.0.2/tursopy/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-12 01:16:08.000000 tursopy-0.0.2/tursopy/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-12 01:16:08.000000 tursopy-0.0.2/tursopy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-04-12 01:16:08.000000 tursopy-0.0.2/tursopy/tursopy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:16:32.649390 tursopy-0.0.2/tursopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-12 01:16:32.000000 tursopy-0.0.2/tursopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-12 01:16:32.000000 tursopy-0.0.2/tursopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 01:16:32.000000 tursopy-0.0.2/tursopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 01:16:32.000000 tursopy-0.0.2/tursopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 01:16:32.000000 tursopy-0.0.2/tursopy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:00:27.348638 tursopy-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-17 06:00:03.000000 tursopy-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-17 06:00:27.344638 tursopy-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-17 06:00:03.000000 tursopy-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-17 06:00:25.000000 tursopy-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 06:00:27.348638 tursopy-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:00:27.344638 tursopy-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-17 06:00:03.000000 tursopy-0.0.3/tests/test_tursopy_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10258 2024-04-17 06:00:03.000000 tursopy-0.0.3/tests/test_tursopy_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:00:27.344638 tursopy-0.0.3/tursopy/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 06:00:03.000000 tursopy-0.0.3/tursopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-17 06:00:03.000000 tursopy-0.0.3/tursopy/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14537 2024-04-17 06:00:03.000000 tursopy-0.0.3/tursopy/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-17 06:00:03.000000 tursopy-0.0.3/tursopy/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-17 06:00:03.000000 tursopy-0.0.3/tursopy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-04-17 06:00:03.000000 tursopy-0.0.3/tursopy/tursopy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:00:27.344638 tursopy-0.0.3/tursopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-17 06:00:27.000000 tursopy-0.0.3/tursopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-17 06:00:27.000000 tursopy-0.0.3/tursopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:00:27.000000 tursopy-0.0.3/tursopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 06:00:27.000000 tursopy-0.0.3/tursopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 06:00:27.000000 tursopy-0.0.3/tursopy.egg-info/top_level.txt
```

### Comparing `tursopy-0.0.2/LICENSE` & `tursopy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tursopy-0.0.2/PKG-INFO` & `tursopy-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: tursopy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Fully type-hinted Turso Platform API wrapper for Python. 
 Author-email: Maurice Künicke <m.kuenicke1995@gmail.com>
 Project-URL: Homepage, https://github.com/MauriceKuenicke/tursopy
 Project-URL: Issues, https://github.com/MauriceKuenicke/tursopy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 <h1 align="center">
   TursoPy
 </h1>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: tursopy Version: 0.0.2 Summary: Fully type-hinted
+Metadata-Version: 2.1 Name: tursopy Version: 0.0.3 Summary: Fully type-hinted
 Turso Platform API wrapper for Python. Author-email: Maurice KÃ¼nicke
 gmail.com> Project-URL: Homepage, https://github.com/MauriceKuenicke/tursopy
 Project-URL: Issues, https://github.com/MauriceKuenicke/tursopy/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
+Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: requests
                              ************ TTuurrssooPPyy ************
            FFuullllyy ttyyppee--hhiinntteedd TTuurrssoo PPllaattffoorrmm AAPPII wwrraappppeerr ffoorr PPyytthhoonn..
     _[_T_e_s_t_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_M_a_u_r_i_c_e_K_u_e_n_i_c_k_e_/_t_u_r_s_o_p_y_/_b_r_a_n_c_h_/_m_a_i_n_/_g_r_a_p_h_/
                           _b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_N_Y_H_1_6_2_M_D_J_D_]
 --- **Documentation**: _h_t_t_p_s_:_/_/_m_a_u_r_i_c_e_k_u_e_n_i_c_k_e_._g_i_t_h_u_b_._i_o_/_t_u_r_s_o_p_y_/ **Source
 Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_M_a_u_r_i_c_e_K_u_e_n_i_c_k_e_/_t_u_r_s_o_p_y --- # â ï¸ Important This
```

### Comparing `tursopy-0.0.2/README.md` & `tursopy-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tursopy-0.0.2/pyproject.toml` & `tursopy-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tursopy"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name="Maurice Künicke", email="m.kuenicke1995@gmail.com" },
 ]
 description = "Fully type-hinted Turso Platform API wrapper for Python. "
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "requests"
```

### Comparing `tursopy-0.0.2/tests/test_tursopy_client.py` & `tursopy-0.0.3/tests/test_tursopy_client.py`

 * *Files identical despite different names*

### Comparing `tursopy-0.0.2/tests/test_tursopy_db.py` & `tursopy-0.0.3/tests/test_tursopy_db.py`

 * *Files identical despite different names*

### Comparing `tursopy-0.0.2/tursopy/dataclasses.py` & `tursopy-0.0.3/tursopy/dataclasses.py`

 * *Files identical despite different names*

### Comparing `tursopy-0.0.2/tursopy/db.py` & `tursopy-0.0.3/tursopy/db.py`

 * *Files identical despite different names*

### Comparing `tursopy-0.0.2/tursopy/endpoints.py` & `tursopy-0.0.3/tursopy/endpoints.py`

 * *Files identical despite different names*

### Comparing `tursopy-0.0.2/tursopy/exceptions.py` & `tursopy-0.0.3/tursopy/exceptions.py`

 * *Files identical despite different names*

### Comparing `tursopy-0.0.2/tursopy/tursopy.py` & `tursopy-0.0.3/tursopy/tursopy.py`

 * *Files identical despite different names*

### Comparing `tursopy-0.0.2/tursopy.egg-info/PKG-INFO` & `tursopy-0.0.3/tursopy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: tursopy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Fully type-hinted Turso Platform API wrapper for Python. 
 Author-email: Maurice Künicke <m.kuenicke1995@gmail.com>
 Project-URL: Homepage, https://github.com/MauriceKuenicke/tursopy
 Project-URL: Issues, https://github.com/MauriceKuenicke/tursopy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 <h1 align="center">
   TursoPy
 </h1>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: tursopy Version: 0.0.2 Summary: Fully type-hinted
+Metadata-Version: 2.1 Name: tursopy Version: 0.0.3 Summary: Fully type-hinted
 Turso Platform API wrapper for Python. Author-email: Maurice KÃ¼nicke
 gmail.com> Project-URL: Homepage, https://github.com/MauriceKuenicke/tursopy
 Project-URL: Issues, https://github.com/MauriceKuenicke/tursopy/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
+Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: requests
                              ************ TTuurrssooPPyy ************
            FFuullllyy ttyyppee--hhiinntteedd TTuurrssoo PPllaattffoorrmm AAPPII wwrraappppeerr ffoorr PPyytthhoonn..
     _[_T_e_s_t_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_M_a_u_r_i_c_e_K_u_e_n_i_c_k_e_/_t_u_r_s_o_p_y_/_b_r_a_n_c_h_/_m_a_i_n_/_g_r_a_p_h_/
                           _b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_N_Y_H_1_6_2_M_D_J_D_]
 --- **Documentation**: _h_t_t_p_s_:_/_/_m_a_u_r_i_c_e_k_u_e_n_i_c_k_e_._g_i_t_h_u_b_._i_o_/_t_u_r_s_o_p_y_/ **Source
 Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_M_a_u_r_i_c_e_K_u_e_n_i_c_k_e_/_t_u_r_s_o_p_y --- # â ï¸ Important This
```

