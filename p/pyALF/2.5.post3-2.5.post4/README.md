# Comparing `tmp/pyalf-2.5.post3.tar.gz` & `tmp/pyalf-2.5.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalf-2.5.post3.tar", last modified: Wed Apr 17 17:29:32 2024, max compression
+gzip compressed data, was "pyalf-2.5.post4.tar", last modified: Wed Apr 17 19:21:32 2024, max compression
```

## Comparing `pyalf-2.5.post3.tar` & `pyalf-2.5.post4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:29:32.372278 pyalf-2.5.post3/
--rw-rw-rw-   0 root         (0) root         (0)    18029 2024-04-17 17:29:20.000000 pyalf-2.5.post3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-17 17:29:20.000000 pyalf-2.5.post3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5056 2024-04-17 17:29:32.372278 pyalf-2.5.post3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4161 2024-04-17 17:29:20.000000 pyalf-2.5.post3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:29:32.372278 pyalf-2.5.post3/pyALF.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5056 2024-04-17 17:29:32.000000 pyalf-2.5.post3/pyALF.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      817 2024-04-17 17:29:32.000000 pyalf-2.5.post3/pyALF.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 17:29:32.000000 pyalf-2.5.post3/pyALF.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      343 2024-04-17 17:29:32.000000 pyalf-2.5.post3/pyALF.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       81 2024-04-17 17:29:32.000000 pyalf-2.5.post3/pyALF.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-17 17:29:32.000000 pyalf-2.5.post3/pyALF.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:29:32.372278 pyalf-2.5.post3/py_alf/
--rw-rw-rw-   0 root         (0) root         (0)     1478 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6245 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/alf_source.py
--rw-rw-rw-   0 root         (0) root         (0)    27314 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/ana.py
--rw-rw-rw-   0 root         (0) root         (0)     8849 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     5930 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/check_common.py
--rw-rw-rw-   0 root         (0) root         (0)     3445 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/check_rebin_ipy.py
--rw-rw-rw-   0 root         (0) root         (0)     3813 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/check_rebin_tk.py
--rw-rw-rw-   0 root         (0) root         (0)     3636 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/check_warmup_ipy.py
--rw-rw-rw-   0 root         (0) root         (0)     4313 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/check_warmup_tk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:29:32.372278 pyalf-2.5.post3/py_alf/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/cli/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1269 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/cli/alf_bin_count.py
--rwxrwxrwx   0 root         (0) root         (0)     1136 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/cli/alf_del_bins.py
--rwxrwxrwx   0 root         (0) root         (0)     4384 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/cli/alf_postprocess.py
--rwxrwxrwx   0 root         (0) root         (0)     3124 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/cli/alf_run.py
--rwxrwxrwx   0 root         (0) root         (0)     1248 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/cli/alf_show_obs.py
--rwxrwxrwx   0 root         (0) root         (0)     6007 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/cli/alf_test_branch.py
--rwxrwxrwx   0 root         (0) root         (0)     2035 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/cli/minimal_ALF_run.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2836 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/init_layout.py
--rw-rw-rw-   0 root         (0) root         (0)    18037 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/lattice.py
--rwxrwxrwx   0 root         (0) root         (0)   103762 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/lattices_armv8.4-a.so
--rwxrwxrwx   0 root         (0) root         (0)    97280 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/lattices_x86-64.so
--rw-rw-rw-   0 root         (0) root         (0)    24446 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/simulation.py
--rw-rw-rw-   0 root         (0) root         (0)     3433 2024-04-17 17:29:20.000000 pyalf-2.5.post3/py_alf/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1542 2024-04-17 17:29:20.000000 pyalf-2.5.post3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 17:29:32.372278 pyalf-2.5.post3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:29:32.372278 pyalf-2.5.post3/tests/
--rwxrwxrwx   0 root         (0) root         (0)     1288 2024-04-17 17:29:20.000000 pyalf-2.5.post3/tests/test_lattice_init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 19:21:32.688926 pyalf-2.5.post4/
+-rw-rw-rw-   0 root         (0) root         (0)    18029 2024-04-17 19:21:20.000000 pyalf-2.5.post4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-17 19:21:20.000000 pyalf-2.5.post4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5056 2024-04-17 19:21:32.688926 pyalf-2.5.post4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4161 2024-04-17 19:21:20.000000 pyalf-2.5.post4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 19:21:32.688926 pyalf-2.5.post4/pyALF.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5056 2024-04-17 19:21:32.000000 pyalf-2.5.post4/pyALF.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      817 2024-04-17 19:21:32.000000 pyalf-2.5.post4/pyALF.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 19:21:32.000000 pyalf-2.5.post4/pyALF.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      343 2024-04-17 19:21:32.000000 pyalf-2.5.post4/pyALF.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2024-04-17 19:21:32.000000 pyalf-2.5.post4/pyALF.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-17 19:21:32.000000 pyalf-2.5.post4/pyALF.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 19:21:32.688926 pyalf-2.5.post4/py_alf/
+-rw-rw-rw-   0 root         (0) root         (0)     1478 2024-04-17 19:21:20.000000 pyalf-2.5.post4/py_alf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6245 2024-04-17 19:21:20.000000 pyalf-2.5.post4/py_alf/alf_source.py
+-rw-rw-rw-   0 root         (0) root         (0)    27314 2024-04-17 19:21:20.000000 pyalf-2.5.post4/py_alf/ana.py
+-rw-rw-rw-   0 root         (0) root         (0)     8849 2024-04-17 19:21:20.000000 pyalf-2.5.post4/py_alf/analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5930 2024-04-17 19:21:20.000000 pyalf-2.5.post4/py_alf/check_common.py
+-rw-rw-rw-   0 root         (0) root         (0)     3445 2024-04-17 19:21:20.000000 pyalf-2.5.post4/py_alf/check_rebin_ipy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3813 2024-04-17 19:21:20.000000 pyalf-2.5.post4/py_alf/check_rebin_tk.py
+-rw-rw-rw-   0 root         (0) root         (0)     3636 2024-04-17 19:21:20.000000 pyalf-2.5.post4/py_alf/check_warmup_ipy.py
+-rw-rw-rw-   0 root         (0) root         (0)     4313 2024-04-17 19:21:20.000000 pyalf-2.5.post4/py_alf/check_warmup_tk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 19:21:32.688926 pyalf-2.5.post4/py_alf/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 19:21:20.000000 pyalf-2.5.post4/py_alf/cli/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1269 2024-04-17 19:21:20.000000 pyalf-2.5.post4/py_alf/cli/alf_bin_count.py
+-rwxrwxrwx   0 root         (0) root         (0)     1136 2024-04-17 19:21:20.000000 pyalf-2.5.post4/py_alf/cli/alf_del_bins.py
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2024-04-17 19:21:20.000000 pyalf-2.5.post4/py_alf/cli/alf_postprocess.py
+-rwxrwxrwx   0 root         (0) root         (0)     3124 2024-04-17 19:21:20.000000 pyalf-2.5.post4/py_alf/cli/alf_run.py
+-rwxrwxrwx   0 root         (0) root         (0)     1248 2024-04-17 19:21:20.000000 pyalf-2.5.post4/py_alf/cli/alf_show_obs.py
+-rwxrwxrwx   0 root         (0) root         (0)     6039 2024-04-17 19:21:20.000000 pyalf-2.5.post4/py_alf/cli/alf_test_branch.py
+-rwxrwxrwx   0 root         (0) root         (0)     2035 2024-04-17 19:21:20.000000 pyalf-2.5.post4/py_alf/cli/minimal_ALF_run.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-17 19:21:20.000000 pyalf-2.5.post4/py_alf/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2836 2024-04-17 19:21:20.000000 pyalf-2.5.post4/py_alf/init_layout.py
+-rw-rw-rw-   0 root         (0) root         (0)    18037 2024-04-17 19:21:20.000000 pyalf-2.5.post4/py_alf/lattice.py
+-rwxrwxrwx   0 root         (0) root         (0)   103762 2024-04-17 19:21:20.000000 pyalf-2.5.post4/py_alf/lattices_armv8.4-a.so
+-rwxrwxrwx   0 root         (0) root         (0)    97280 2024-04-17 19:21:20.000000 pyalf-2.5.post4/py_alf/lattices_x86-64.so
+-rw-rw-rw-   0 root         (0) root         (0)    24446 2024-04-17 19:21:20.000000 pyalf-2.5.post4/py_alf/simulation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3433 2024-04-17 19:21:20.000000 pyalf-2.5.post4/py_alf/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1542 2024-04-17 19:21:20.000000 pyalf-2.5.post4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 19:21:32.688926 pyalf-2.5.post4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 19:21:32.688926 pyalf-2.5.post4/tests/
+-rwxrwxrwx   0 root         (0) root         (0)     1288 2024-04-17 19:21:20.000000 pyalf-2.5.post4/tests/test_lattice_init.py
```

### Comparing `pyalf-2.5.post3/LICENSE` & `pyalf-2.5.post4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post3/PKG-INFO` & `pyalf-2.5.post4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyALF
-Version: 2.5.post3
+Version: 2.5.post4
 Summary: Python interface for ALF, plus scripts and Jupyter notebooks.
 Author-email: ALF Collaboration <alf@physik.uni-wuerzburg.de>, Jonas Schwab <jonas.schwab@uni-wuerzburg.de>
 Project-URL: Homepage, https://git.physik.uni-wuerzburg.de/ALF/pyALF
 Project-URL: Issues, https://git.physik.uni-wuerzburg.de/ALF/pyALF/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

### Comparing `pyalf-2.5.post3/README.md` & `pyalf-2.5.post4/README.md`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post3/pyALF.egg-info/PKG-INFO` & `pyalf-2.5.post4/pyALF.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyALF
-Version: 2.5.post3
+Version: 2.5.post4
 Summary: Python interface for ALF, plus scripts and Jupyter notebooks.
 Author-email: ALF Collaboration <alf@physik.uni-wuerzburg.de>, Jonas Schwab <jonas.schwab@uni-wuerzburg.de>
 Project-URL: Homepage, https://git.physik.uni-wuerzburg.de/ALF/pyALF
 Project-URL: Issues, https://git.physik.uni-wuerzburg.de/ALF/pyALF/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

### Comparing `pyalf-2.5.post3/pyALF.egg-info/SOURCES.txt` & `pyalf-2.5.post4/pyALF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post3/py_alf/__init__.py` & `pyalf-2.5.post4/py_alf/__init__.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post3/py_alf/alf_source.py` & `pyalf-2.5.post4/py_alf/alf_source.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post3/py_alf/ana.py` & `pyalf-2.5.post4/py_alf/ana.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post3/py_alf/analysis.py` & `pyalf-2.5.post4/py_alf/analysis.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post3/py_alf/check_common.py` & `pyalf-2.5.post4/py_alf/check_common.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post3/py_alf/check_rebin_ipy.py` & `pyalf-2.5.post4/py_alf/check_rebin_ipy.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post3/py_alf/check_rebin_tk.py` & `pyalf-2.5.post4/py_alf/check_rebin_tk.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post3/py_alf/check_warmup_ipy.py` & `pyalf-2.5.post4/py_alf/check_warmup_ipy.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post3/py_alf/check_warmup_tk.py` & `pyalf-2.5.post4/py_alf/check_warmup_tk.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post3/py_alf/cli/alf_bin_count.py` & `pyalf-2.5.post4/py_alf/cli/alf_bin_count.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post3/py_alf/cli/alf_del_bins.py` & `pyalf-2.5.post4/py_alf/cli/alf_del_bins.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post3/py_alf/cli/alf_postprocess.py` & `pyalf-2.5.post4/py_alf/cli/alf_postprocess.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post3/py_alf/cli/alf_run.py` & `pyalf-2.5.post4/py_alf/cli/alf_run.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post3/py_alf/cli/alf_show_obs.py` & `pyalf-2.5.post4/py_alf/cli/alf_show_obs.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post3/py_alf/cli/alf_test_branch.py` & `pyalf-2.5.post4/py_alf/cli/alf_test_branch.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,26 +34,26 @@
         ham_name, sim_dict, sim_dir=sim_name+'_test', **kwargs
         )
     return sim_R, sim_T
 
 def _prepare_runs(tmpdir, sim_R, sim_T):
     executable_R = os.path.join(tmpdir, f'ALF_{sim_R.config.replace(" ", "_")}_reference.out')
     if os.path.isfile(executable_R):
-        shutil.copy(executable_R, f'{sim_R.alf_src}/Prog/ALF.out')
+        shutil.copy(executable_R, f'{sim_R.alf_src.alf_dir}/Prog/ALF.out')
     else:
         sim_R.compile()
-        shutil.copy(f'{sim_R.alf_src}/Prog/ALF.out', executable_R)
+        shutil.copy(f'{sim_R.alf_src.alf_dir}/Prog/ALF.out', executable_R)
     sim_R.run(copy_bin=True, only_prep=True)
 
     executable_T = os.path.join(tmpdir, f'ALF_{sim_T.config.replace(" ", "_")}_test.out')
     if os.path.isfile(executable_T):
-        shutil.copy(executable_T, f'{sim_T.alf_src}/Prog/ALF.out')
+        shutil.copy(executable_T, f'{sim_T.alf_src.alf_dir}/Prog/ALF.out')
     else:
         sim_T.compile()
-        shutil.copy(f'{sim_T.alf_src}/Prog/ALF.out', executable_T)
+        shutil.copy(f'{sim_T.alf_src.alf_dir}/Prog/ALF.out', executable_T)
     sim_T.run(copy_bin=True, only_prep=True)
 
 
 def _analyze(sim_R, sim_T):
     sim_R.analysis()
     obs_R = sim_R.get_obs()
     sim_T.analysis()
```

### Comparing `pyalf-2.5.post3/py_alf/cli/minimal_ALF_run.py` & `pyalf-2.5.post4/py_alf/cli/minimal_ALF_run.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post3/py_alf/init_layout.py` & `pyalf-2.5.post4/py_alf/init_layout.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post3/py_alf/lattice.py` & `pyalf-2.5.post4/py_alf/lattice.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post3/py_alf/lattices_armv8.4-a.so` & `pyalf-2.5.post4/py_alf/lattices_armv8.4-a.so`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post3/py_alf/lattices_x86-64.so` & `pyalf-2.5.post4/py_alf/lattices_x86-64.so`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post3/py_alf/simulation.py` & `pyalf-2.5.post4/py_alf/simulation.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post3/py_alf/utils.py` & `pyalf-2.5.post4/py_alf/utils.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post3/pyproject.toml` & `pyalf-2.5.post4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post3/tests/test_lattice_init.py` & `pyalf-2.5.post4/tests/test_lattice_init.py`

 * *Files identical despite different names*

