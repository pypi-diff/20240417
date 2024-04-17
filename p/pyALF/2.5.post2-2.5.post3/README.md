# Comparing `tmp/pyalf-2.5.post2.tar.gz` & `tmp/pyalf-2.5.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalf-2.5.post2.tar", last modified: Wed Apr 17 17:28:02 2024, max compression
+gzip compressed data, was "pyalf-2.5.post3.tar", last modified: Wed Apr 17 17:29:32 2024, max compression
```

## Comparing `pyalf-2.5.post2.tar` & `pyalf-2.5.post3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:28:02.251427 pyalf-2.5.post2/
--rw-rw-rw-   0 root         (0) root         (0)    18029 2024-04-17 17:27:50.000000 pyalf-2.5.post2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-17 17:27:50.000000 pyalf-2.5.post2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5057 2024-04-17 17:28:02.251427 pyalf-2.5.post2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4162 2024-04-17 17:27:50.000000 pyalf-2.5.post2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:28:02.251427 pyalf-2.5.post2/pyALF.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5057 2024-04-17 17:28:02.000000 pyalf-2.5.post2/pyALF.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      817 2024-04-17 17:28:02.000000 pyalf-2.5.post2/pyALF.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 17:28:02.000000 pyalf-2.5.post2/pyALF.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      343 2024-04-17 17:28:02.000000 pyalf-2.5.post2/pyALF.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       81 2024-04-17 17:28:02.000000 pyalf-2.5.post2/pyALF.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-17 17:28:02.000000 pyalf-2.5.post2/pyALF.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:28:02.247427 pyalf-2.5.post2/py_alf/
--rw-rw-rw-   0 root         (0) root         (0)     1478 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6245 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/alf_source.py
--rw-rw-rw-   0 root         (0) root         (0)    27314 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/ana.py
--rw-rw-rw-   0 root         (0) root         (0)     8849 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     5930 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/check_common.py
--rw-rw-rw-   0 root         (0) root         (0)     3445 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/check_rebin_ipy.py
--rw-rw-rw-   0 root         (0) root         (0)     3813 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/check_rebin_tk.py
--rw-rw-rw-   0 root         (0) root         (0)     3636 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/check_warmup_ipy.py
--rw-rw-rw-   0 root         (0) root         (0)     4313 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/check_warmup_tk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:28:02.251427 pyalf-2.5.post2/py_alf/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/cli/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1269 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/cli/alf_bin_count.py
--rwxrwxrwx   0 root         (0) root         (0)     1136 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/cli/alf_del_bins.py
--rwxrwxrwx   0 root         (0) root         (0)     4384 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/cli/alf_postprocess.py
--rwxrwxrwx   0 root         (0) root         (0)     3124 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/cli/alf_run.py
--rwxrwxrwx   0 root         (0) root         (0)     1248 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/cli/alf_show_obs.py
--rwxrwxrwx   0 root         (0) root         (0)     6007 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/cli/alf_test_branch.py
--rwxrwxrwx   0 root         (0) root         (0)     2035 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/cli/minimal_ALF_run.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2836 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/init_layout.py
--rw-rw-rw-   0 root         (0) root         (0)    18037 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/lattice.py
--rwxrwxrwx   0 root         (0) root         (0)   103762 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/lattices_armv8.4-a.so
--rwxrwxrwx   0 root         (0) root         (0)    97280 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/lattices_x86-64.so
--rw-rw-rw-   0 root         (0) root         (0)    24446 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/simulation.py
--rw-rw-rw-   0 root         (0) root         (0)     3433 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1542 2024-04-17 17:27:50.000000 pyalf-2.5.post2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 17:28:02.251427 pyalf-2.5.post2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:28:02.251427 pyalf-2.5.post2/tests/
--rwxrwxrwx   0 root         (0) root         (0)     1288 2024-04-17 17:27:50.000000 pyalf-2.5.post2/tests/test_lattice_init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:29:32.372278 pyalf-2.5.post3/
+-rw-rw-rw-   0 root         (0) root         (0)    18029 2024-04-17 17:29:20.000000 pyalf-2.5.post3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-17 17:29:20.000000 pyalf-2.5.post3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5056 2024-04-17 17:29:32.372278 pyalf-2.5.post3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4161 2024-04-17 17:29:20.000000 pyalf-2.5.post3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:29:32.372278 pyalf-2.5.post3/pyALF.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5056 2024-04-17 17:29:32.000000 pyalf-2.5.post3/pyALF.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      817 2024-04-17 17:29:32.000000 pyalf-2.5.post3/pyALF.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 17:29:32.000000 pyalf-2.5.post3/pyALF.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      343 2024-04-17 17:29:32.000000 pyalf-2.5.post3/pyALF.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2024-04-17 17:29:32.000000 pyalf-2.5.post3/pyALF.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-17 17:29:32.000000 pyalf-2.5.post3/pyALF.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:29:32.372278 pyalf-2.5.post3/py_alf/
+-rw-rw-rw-   0 root         (0) root         (0)     1478 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6245 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/alf_source.py
+-rw-rw-rw-   0 root         (0) root         (0)    27314 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/ana.py
+-rw-rw-rw-   0 root         (0) root         (0)     8849 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5930 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/check_common.py
+-rw-rw-rw-   0 root         (0) root         (0)     3445 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/check_rebin_ipy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3813 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/check_rebin_tk.py
+-rw-rw-rw-   0 root         (0) root         (0)     3636 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/check_warmup_ipy.py
+-rw-rw-rw-   0 root         (0) root         (0)     4313 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/check_warmup_tk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:29:32.372278 pyalf-2.5.post3/py_alf/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/cli/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1269 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/cli/alf_bin_count.py
+-rwxrwxrwx   0 root         (0) root         (0)     1136 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/cli/alf_del_bins.py
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/cli/alf_postprocess.py
+-rwxrwxrwx   0 root         (0) root         (0)     3124 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/cli/alf_run.py
+-rwxrwxrwx   0 root         (0) root         (0)     1248 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/cli/alf_show_obs.py
+-rwxrwxrwx   0 root         (0) root         (0)     6007 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/cli/alf_test_branch.py
+-rwxrwxrwx   0 root         (0) root         (0)     2035 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/cli/minimal_ALF_run.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2836 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/init_layout.py
+-rw-rw-rw-   0 root         (0) root         (0)    18037 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/lattice.py
+-rwxrwxrwx   0 root         (0) root         (0)   103762 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/lattices_armv8.4-a.so
+-rwxrwxrwx   0 root         (0) root         (0)    97280 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/lattices_x86-64.so
+-rw-rw-rw-   0 root         (0) root         (0)    24446 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/simulation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3433 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1542 2024-04-17 17:29:20.000000 pyalf-2.5.post3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 17:29:32.372278 pyalf-2.5.post3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:29:32.372278 pyalf-2.5.post3/tests/
+-rwxrwxrwx   0 root         (0) root         (0)     1288 2024-04-17 17:29:20.000000 pyalf-2.5.post3/tests/test_lattice_init.py
```

### Comparing `pyalf-2.5.post2/LICENSE` & `pyalf-2.5.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post2/PKG-INFO` & `pyalf-2.5.post3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyALF
-Version: 2.5.post2
+Version: 2.5.post3
 Summary: Python interface for ALF, plus scripts and Jupyter notebooks.
 Author-email: ALF Collaboration <alf@physik.uni-wuerzburg.de>, Jonas Schwab <jonas.schwab@uni-wuerzburg.de>
 Project-URL: Homepage, https://git.physik.uni-wuerzburg.de/ALF/pyALF
 Project-URL: Issues, https://git.physik.uni-wuerzburg.de/ALF/pyALF/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
@@ -41,17 +41,15 @@
 * Python Scripts in the folder `Scripts` that can be run to reproduce benchmark results for established models
 
 The **documentation** can be found [here](http://gitpages.physik.uni-wuerzburg.de/Jonas_schwab/pyalf-docu).
 
 ## Installation
 
 ---
-**⚠️ NOTE**
-
-In previous versions of pyALF, the installation instructions asked the users to set the environment variable `PYTHONPATH`.
+**⚠️ NOTE** In previous versions of pyALF, the installation instructions asked the users to set the environment variable `PYTHONPATH`.
 This conflicts with the newer pip package, therefore you should remove definitions of this environment variable related to pyALF.
 
 ---
 
 pyALF can be installed via the Python package installer [pip](https://pip.pypa.io/en/stable/).
 
 ```bash
```

### Comparing `pyalf-2.5.post2/README.md` & `pyalf-2.5.post3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -16,17 +16,15 @@
 * Python Scripts in the folder `Scripts` that can be run to reproduce benchmark results for established models
 
 The **documentation** can be found [here](http://gitpages.physik.uni-wuerzburg.de/Jonas_schwab/pyalf-docu).
 
 ## Installation
 
 ---
-**⚠️ NOTE**
-
-In previous versions of pyALF, the installation instructions asked the users to set the environment variable `PYTHONPATH`.
+**⚠️ NOTE** In previous versions of pyALF, the installation instructions asked the users to set the environment variable `PYTHONPATH`.
 This conflicts with the newer pip package, therefore you should remove definitions of this environment variable related to pyALF.
 
 ---
 
 pyALF can be installed via the Python package installer [pip](https://pip.pypa.io/en/stable/).
 
 ```bash
```

### Comparing `pyalf-2.5.post2/pyALF.egg-info/PKG-INFO` & `pyalf-2.5.post3/pyALF.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyALF
-Version: 2.5.post2
+Version: 2.5.post3
 Summary: Python interface for ALF, plus scripts and Jupyter notebooks.
 Author-email: ALF Collaboration <alf@physik.uni-wuerzburg.de>, Jonas Schwab <jonas.schwab@uni-wuerzburg.de>
 Project-URL: Homepage, https://git.physik.uni-wuerzburg.de/ALF/pyALF
 Project-URL: Issues, https://git.physik.uni-wuerzburg.de/ALF/pyALF/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
@@ -41,17 +41,15 @@
 * Python Scripts in the folder `Scripts` that can be run to reproduce benchmark results for established models
 
 The **documentation** can be found [here](http://gitpages.physik.uni-wuerzburg.de/Jonas_schwab/pyalf-docu).
 
 ## Installation
 
 ---
-**⚠️ NOTE**
-
-In previous versions of pyALF, the installation instructions asked the users to set the environment variable `PYTHONPATH`.
+**⚠️ NOTE** In previous versions of pyALF, the installation instructions asked the users to set the environment variable `PYTHONPATH`.
 This conflicts with the newer pip package, therefore you should remove definitions of this environment variable related to pyALF.
 
 ---
 
 pyALF can be installed via the Python package installer [pip](https://pip.pypa.io/en/stable/).
 
 ```bash
```

### Comparing `pyalf-2.5.post2/pyALF.egg-info/SOURCES.txt` & `pyalf-2.5.post3/pyALF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post2/py_alf/__init__.py` & `pyalf-2.5.post3/py_alf/__init__.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post2/py_alf/alf_source.py` & `pyalf-2.5.post3/py_alf/alf_source.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post2/py_alf/ana.py` & `pyalf-2.5.post3/py_alf/ana.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post2/py_alf/analysis.py` & `pyalf-2.5.post3/py_alf/analysis.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post2/py_alf/check_common.py` & `pyalf-2.5.post3/py_alf/check_common.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post2/py_alf/check_rebin_ipy.py` & `pyalf-2.5.post3/py_alf/check_rebin_ipy.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post2/py_alf/check_rebin_tk.py` & `pyalf-2.5.post3/py_alf/check_rebin_tk.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post2/py_alf/check_warmup_ipy.py` & `pyalf-2.5.post3/py_alf/check_warmup_ipy.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post2/py_alf/check_warmup_tk.py` & `pyalf-2.5.post3/py_alf/check_warmup_tk.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post2/py_alf/cli/alf_bin_count.py` & `pyalf-2.5.post3/py_alf/cli/alf_bin_count.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post2/py_alf/cli/alf_del_bins.py` & `pyalf-2.5.post3/py_alf/cli/alf_del_bins.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post2/py_alf/cli/alf_postprocess.py` & `pyalf-2.5.post3/py_alf/cli/alf_postprocess.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post2/py_alf/cli/alf_run.py` & `pyalf-2.5.post3/py_alf/cli/alf_run.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post2/py_alf/cli/alf_show_obs.py` & `pyalf-2.5.post3/py_alf/cli/alf_show_obs.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post2/py_alf/cli/alf_test_branch.py` & `pyalf-2.5.post3/py_alf/cli/alf_test_branch.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post2/py_alf/cli/minimal_ALF_run.py` & `pyalf-2.5.post3/py_alf/cli/minimal_ALF_run.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post2/py_alf/init_layout.py` & `pyalf-2.5.post3/py_alf/init_layout.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post2/py_alf/lattice.py` & `pyalf-2.5.post3/py_alf/lattice.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post2/py_alf/lattices_armv8.4-a.so` & `pyalf-2.5.post3/py_alf/lattices_armv8.4-a.so`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post2/py_alf/lattices_x86-64.so` & `pyalf-2.5.post3/py_alf/lattices_x86-64.so`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post2/py_alf/simulation.py` & `pyalf-2.5.post3/py_alf/simulation.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post2/py_alf/utils.py` & `pyalf-2.5.post3/py_alf/utils.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post2/pyproject.toml` & `pyalf-2.5.post3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post2/tests/test_lattice_init.py` & `pyalf-2.5.post3/tests/test_lattice_init.py`

 * *Files identical despite different names*

