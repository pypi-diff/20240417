# Comparing `tmp/pyalf-2.5.post1.tar.gz` & `tmp/pyalf-2.5.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalf-2.5.post1.tar", last modified: Wed Apr 17 16:17:35 2024, max compression
+gzip compressed data, was "pyalf-2.5.post2.tar", last modified: Wed Apr 17 17:28:02 2024, max compression
```

## Comparing `pyalf-2.5.post1.tar` & `pyalf-2.5.post2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 16:17:35.319163 pyalf-2.5.post1/
--rw-rw-rw-   0 root         (0) root         (0)    18029 2024-04-17 16:17:23.000000 pyalf-2.5.post1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-17 16:17:23.000000 pyalf-2.5.post1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4632 2024-04-17 16:17:35.319163 pyalf-2.5.post1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3737 2024-04-17 16:17:23.000000 pyalf-2.5.post1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 16:17:35.319163 pyalf-2.5.post1/pyALF.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4632 2024-04-17 16:17:35.000000 pyalf-2.5.post1/pyALF.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      817 2024-04-17 16:17:35.000000 pyalf-2.5.post1/pyALF.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 16:17:35.000000 pyalf-2.5.post1/pyALF.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      343 2024-04-17 16:17:35.000000 pyalf-2.5.post1/pyALF.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       81 2024-04-17 16:17:35.000000 pyalf-2.5.post1/pyALF.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-17 16:17:35.000000 pyalf-2.5.post1/pyALF.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 16:17:35.315163 pyalf-2.5.post1/py_alf/
--rw-rw-rw-   0 root         (0) root         (0)     1478 2024-04-17 16:17:23.000000 pyalf-2.5.post1/py_alf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6245 2024-04-17 16:17:23.000000 pyalf-2.5.post1/py_alf/alf_source.py
--rw-rw-rw-   0 root         (0) root         (0)    27314 2024-04-17 16:17:23.000000 pyalf-2.5.post1/py_alf/ana.py
--rw-rw-rw-   0 root         (0) root         (0)     8849 2024-04-17 16:17:23.000000 pyalf-2.5.post1/py_alf/analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     5930 2024-04-17 16:17:23.000000 pyalf-2.5.post1/py_alf/check_common.py
--rw-rw-rw-   0 root         (0) root         (0)     3445 2024-04-17 16:17:23.000000 pyalf-2.5.post1/py_alf/check_rebin_ipy.py
--rw-rw-rw-   0 root         (0) root         (0)     3813 2024-04-17 16:17:23.000000 pyalf-2.5.post1/py_alf/check_rebin_tk.py
--rw-rw-rw-   0 root         (0) root         (0)     3636 2024-04-17 16:17:23.000000 pyalf-2.5.post1/py_alf/check_warmup_ipy.py
--rw-rw-rw-   0 root         (0) root         (0)     4313 2024-04-17 16:17:23.000000 pyalf-2.5.post1/py_alf/check_warmup_tk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 16:17:35.315163 pyalf-2.5.post1/py_alf/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 16:17:23.000000 pyalf-2.5.post1/py_alf/cli/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1269 2024-04-17 16:17:23.000000 pyalf-2.5.post1/py_alf/cli/alf_bin_count.py
--rwxrwxrwx   0 root         (0) root         (0)     1136 2024-04-17 16:17:23.000000 pyalf-2.5.post1/py_alf/cli/alf_del_bins.py
--rwxrwxrwx   0 root         (0) root         (0)     4384 2024-04-17 16:17:23.000000 pyalf-2.5.post1/py_alf/cli/alf_postprocess.py
--rwxrwxrwx   0 root         (0) root         (0)     3124 2024-04-17 16:17:23.000000 pyalf-2.5.post1/py_alf/cli/alf_run.py
--rwxrwxrwx   0 root         (0) root         (0)     1248 2024-04-17 16:17:23.000000 pyalf-2.5.post1/py_alf/cli/alf_show_obs.py
--rwxrwxrwx   0 root         (0) root         (0)     6007 2024-04-17 16:17:23.000000 pyalf-2.5.post1/py_alf/cli/alf_test_branch.py
--rwxrwxrwx   0 root         (0) root         (0)     2035 2024-04-17 16:17:23.000000 pyalf-2.5.post1/py_alf/cli/minimal_ALF_run.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-17 16:17:23.000000 pyalf-2.5.post1/py_alf/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2836 2024-04-17 16:17:23.000000 pyalf-2.5.post1/py_alf/init_layout.py
--rw-rw-rw-   0 root         (0) root         (0)    18037 2024-04-17 16:17:23.000000 pyalf-2.5.post1/py_alf/lattice.py
--rwxrwxrwx   0 root         (0) root         (0)   103762 2024-04-17 16:17:23.000000 pyalf-2.5.post1/py_alf/lattices_armv8.4-a.so
--rwxrwxrwx   0 root         (0) root         (0)    97280 2024-04-17 16:17:23.000000 pyalf-2.5.post1/py_alf/lattices_x86-64.so
--rw-rw-rw-   0 root         (0) root         (0)    24446 2024-04-17 16:17:23.000000 pyalf-2.5.post1/py_alf/simulation.py
--rw-rw-rw-   0 root         (0) root         (0)     3433 2024-04-17 16:17:23.000000 pyalf-2.5.post1/py_alf/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1542 2024-04-17 16:17:23.000000 pyalf-2.5.post1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 16:17:35.319163 pyalf-2.5.post1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 16:17:35.319163 pyalf-2.5.post1/tests/
--rwxrwxrwx   0 root         (0) root         (0)     1288 2024-04-17 16:17:23.000000 pyalf-2.5.post1/tests/test_lattice_init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:28:02.251427 pyalf-2.5.post2/
+-rw-rw-rw-   0 root         (0) root         (0)    18029 2024-04-17 17:27:50.000000 pyalf-2.5.post2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-17 17:27:50.000000 pyalf-2.5.post2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5057 2024-04-17 17:28:02.251427 pyalf-2.5.post2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4162 2024-04-17 17:27:50.000000 pyalf-2.5.post2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:28:02.251427 pyalf-2.5.post2/pyALF.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5057 2024-04-17 17:28:02.000000 pyalf-2.5.post2/pyALF.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      817 2024-04-17 17:28:02.000000 pyalf-2.5.post2/pyALF.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 17:28:02.000000 pyalf-2.5.post2/pyALF.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      343 2024-04-17 17:28:02.000000 pyalf-2.5.post2/pyALF.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2024-04-17 17:28:02.000000 pyalf-2.5.post2/pyALF.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-17 17:28:02.000000 pyalf-2.5.post2/pyALF.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:28:02.247427 pyalf-2.5.post2/py_alf/
+-rw-rw-rw-   0 root         (0) root         (0)     1478 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6245 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/alf_source.py
+-rw-rw-rw-   0 root         (0) root         (0)    27314 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/ana.py
+-rw-rw-rw-   0 root         (0) root         (0)     8849 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5930 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/check_common.py
+-rw-rw-rw-   0 root         (0) root         (0)     3445 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/check_rebin_ipy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3813 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/check_rebin_tk.py
+-rw-rw-rw-   0 root         (0) root         (0)     3636 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/check_warmup_ipy.py
+-rw-rw-rw-   0 root         (0) root         (0)     4313 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/check_warmup_tk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:28:02.251427 pyalf-2.5.post2/py_alf/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/cli/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1269 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/cli/alf_bin_count.py
+-rwxrwxrwx   0 root         (0) root         (0)     1136 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/cli/alf_del_bins.py
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/cli/alf_postprocess.py
+-rwxrwxrwx   0 root         (0) root         (0)     3124 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/cli/alf_run.py
+-rwxrwxrwx   0 root         (0) root         (0)     1248 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/cli/alf_show_obs.py
+-rwxrwxrwx   0 root         (0) root         (0)     6007 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/cli/alf_test_branch.py
+-rwxrwxrwx   0 root         (0) root         (0)     2035 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/cli/minimal_ALF_run.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2836 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/init_layout.py
+-rw-rw-rw-   0 root         (0) root         (0)    18037 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/lattice.py
+-rwxrwxrwx   0 root         (0) root         (0)   103762 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/lattices_armv8.4-a.so
+-rwxrwxrwx   0 root         (0) root         (0)    97280 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/lattices_x86-64.so
+-rw-rw-rw-   0 root         (0) root         (0)    24446 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/simulation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3433 2024-04-17 17:27:50.000000 pyalf-2.5.post2/py_alf/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1542 2024-04-17 17:27:50.000000 pyalf-2.5.post2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 17:28:02.251427 pyalf-2.5.post2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:28:02.251427 pyalf-2.5.post2/tests/
+-rwxrwxrwx   0 root         (0) root         (0)     1288 2024-04-17 17:27:50.000000 pyalf-2.5.post2/tests/test_lattice_init.py
```

### Comparing `pyalf-2.5.post1/LICENSE` & `pyalf-2.5.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post1/PKG-INFO` & `pyalf-2.5.post2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyALF
-Version: 2.5.post1
+Version: 2.5.post2
 Summary: Python interface for ALF, plus scripts and Jupyter notebooks.
 Author-email: ALF Collaboration <alf@physik.uni-wuerzburg.de>, Jonas Schwab <jonas.schwab@uni-wuerzburg.de>
 Project-URL: Homepage, https://git.physik.uni-wuerzburg.de/ALF/pyALF
 Project-URL: Issues, https://git.physik.uni-wuerzburg.de/ALF/pyALF/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
@@ -38,38 +38,48 @@
 * The Python module `py_alf`, exposing all the package's utility to Python.
 * A set of command line tools in the folder `py_alf/cli`, that make it easy to leverage pyALF from a Unix shell.
 * Jupyter notebooks in the folder `Notebooks`, serving as an easy introduction to QMC and ALF
 * Python Scripts in the folder `Scripts` that can be run to reproduce benchmark results for established models
 
 The **documentation** can be found [here](http://gitpages.physik.uni-wuerzburg.de/Jonas_schwab/pyalf-docu).
 
-## Prerequisites
+## Installation
 
-* Python3
-* Jupyter
-* The following Python packages:
-  * h5py
-  * numpy
-  * pandas
-  * matplotlib
-  * numba
-  * scipy
-  * tkinter
-  * ipywidgets
-  * ipympl
-  * f90nml
-* The libraries Lapack and Blas
-* A Fortran compiler, such as gfortran or ifort,
+---
+**⚠️ NOTE**
 
-where the last two are required by the main package [ALF](https://git.physik.uni-wuerzburg.de/ALF).
+In previous versions of pyALF, the installation instructions asked the users to set the environment variable `PYTHONPATH`.
+This conflicts with the newer pip package, therefore you should remove definitions of this environment variable related to pyALF.
 
-Also, add pyALF's path to your environment variable `PYTHONPATH`. In Linux, this can be achieved, e.g., by adding the following line to `~/.bashrc` if the used shell if bash or `~/.zshrc`, if the shell is zsh:
+---
+
+pyALF can be installed via the Python package installer [pip](https://pip.pypa.io/en/stable/).
 
 ```bash
-export PYTHONPATH="/local/path/to/pyALF:$PYTHONPATH"
+pip install pyALF
+```
+
+### Development installation
+
+If you want to develop pyALF, you can clone the repository and install it in
+[development mode](https://setuptools.pypa.io/en/latest/userguide/development_mode.html),
+which allows you to edit the files while using them like an installed package.
+For this, it is highly recommended to use a dedicated Python environment using e.g.
+[Python venv](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/)
+or a
+[conda environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).
+The following example shows how to install pyALF in development mode using venv.
+
+```bash
+git clone https://git.physik.uni-wuerzburg.de/ALF/pyALF.git
+cd pyALF
+python -m venv .venv
+source .venv/bin/activate
+
+pip install --editable .
 ```
 
 ## Usage
 
 There are multiple ways to use pyALF, which roughly breaks down into three approaches:
 * Using Jupyter notebooks
 * Using the command line interface
@@ -89,31 +99,28 @@
 jupyter-lab
 ```
 
 which opens the "notebook dashboard" in your default browser, from where one can open the sample notebooks in `Notebooks/` and create new notebooks.
 
 ### Command line interface
 
-pyALF also delivers a set of command line scripts, located in the folder `/py_alf/cli/`, to be use from a UNIX shell. For convenient access, it makes sense to add the folder to the environment variable `PATH`:
+pyALF also delivers a set of command line scripts, to be use from a UNIX shell. For a full list of command line scripts see [here](gitpages.physik.uni-wuerzburg.de/Jonas_schwab/pyalf-docu/source/reference/cli.html).
 
-```bash
-export PATH="/path/to/pyALF/py_alf/cli:$PATH"
-```
-
-Then the scripts can simply be called by their names, try e.g. 
+Try, e.g.
 
 ```bash
-alf_run.py -h
+alf_run -h
 ```
 
-For a full list of command line scripts see [here](gitpages.physik.uni-wuerzburg.de/Jonas_schwab/pyalf-docu/source/reference/cli.html).
+The source code for the scripts can be found in the folder `/py_alf/cli/`.
+
 
 ### Use module `py_alf` in custom scripts
 
-Finally, one can also use the module module `py_alf` in custon Python scripts, which is analogous to the usage in Jupyter notebooks minus some interactivity.
+Finally, one can also use the module module `py_alf` in custom Python scripts, which is analogous to the usage in Jupyter notebooks minus some interactivity.
 
 ## License
 
 The various works that make up the ALF project are placed under licenses that put
 a strong emphasis on the attribution of the original authors and the sharing of the contained knowledge.
 To that end we have placed the ALF source code under the GPL version 3 license (see license.GPL and license.additional)
 and took the liberty as per GPLv3 section 7 to include additional terms that deal with the attribution
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyalf-2.5.post1/README.md` & `pyalf-2.5.post2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -13,38 +13,48 @@
 * The Python module `py_alf`, exposing all the package's utility to Python.
 * A set of command line tools in the folder `py_alf/cli`, that make it easy to leverage pyALF from a Unix shell.
 * Jupyter notebooks in the folder `Notebooks`, serving as an easy introduction to QMC and ALF
 * Python Scripts in the folder `Scripts` that can be run to reproduce benchmark results for established models
 
 The **documentation** can be found [here](http://gitpages.physik.uni-wuerzburg.de/Jonas_schwab/pyalf-docu).
 
-## Prerequisites
+## Installation
 
-* Python3
-* Jupyter
-* The following Python packages:
-  * h5py
-  * numpy
-  * pandas
-  * matplotlib
-  * numba
-  * scipy
-  * tkinter
-  * ipywidgets
-  * ipympl
-  * f90nml
-* The libraries Lapack and Blas
-* A Fortran compiler, such as gfortran or ifort,
+---
+**⚠️ NOTE**
 
-where the last two are required by the main package [ALF](https://git.physik.uni-wuerzburg.de/ALF).
+In previous versions of pyALF, the installation instructions asked the users to set the environment variable `PYTHONPATH`.
+This conflicts with the newer pip package, therefore you should remove definitions of this environment variable related to pyALF.
 
-Also, add pyALF's path to your environment variable `PYTHONPATH`. In Linux, this can be achieved, e.g., by adding the following line to `~/.bashrc` if the used shell if bash or `~/.zshrc`, if the shell is zsh:
+---
+
+pyALF can be installed via the Python package installer [pip](https://pip.pypa.io/en/stable/).
 
 ```bash
-export PYTHONPATH="/local/path/to/pyALF:$PYTHONPATH"
+pip install pyALF
+```
+
+### Development installation
+
+If you want to develop pyALF, you can clone the repository and install it in
+[development mode](https://setuptools.pypa.io/en/latest/userguide/development_mode.html),
+which allows you to edit the files while using them like an installed package.
+For this, it is highly recommended to use a dedicated Python environment using e.g.
+[Python venv](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/)
+or a
+[conda environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).
+The following example shows how to install pyALF in development mode using venv.
+
+```bash
+git clone https://git.physik.uni-wuerzburg.de/ALF/pyALF.git
+cd pyALF
+python -m venv .venv
+source .venv/bin/activate
+
+pip install --editable .
 ```
 
 ## Usage
 
 There are multiple ways to use pyALF, which roughly breaks down into three approaches:
 * Using Jupyter notebooks
 * Using the command line interface
@@ -64,31 +74,28 @@
 jupyter-lab
 ```
 
 which opens the "notebook dashboard" in your default browser, from where one can open the sample notebooks in `Notebooks/` and create new notebooks.
 
 ### Command line interface
 
-pyALF also delivers a set of command line scripts, located in the folder `/py_alf/cli/`, to be use from a UNIX shell. For convenient access, it makes sense to add the folder to the environment variable `PATH`:
+pyALF also delivers a set of command line scripts, to be use from a UNIX shell. For a full list of command line scripts see [here](gitpages.physik.uni-wuerzburg.de/Jonas_schwab/pyalf-docu/source/reference/cli.html).
 
-```bash
-export PATH="/path/to/pyALF/py_alf/cli:$PATH"
-```
-
-Then the scripts can simply be called by their names, try e.g. 
+Try, e.g.
 
 ```bash
-alf_run.py -h
+alf_run -h
 ```
 
-For a full list of command line scripts see [here](gitpages.physik.uni-wuerzburg.de/Jonas_schwab/pyalf-docu/source/reference/cli.html).
+The source code for the scripts can be found in the folder `/py_alf/cli/`.
+
 
 ### Use module `py_alf` in custom scripts
 
-Finally, one can also use the module module `py_alf` in custon Python scripts, which is analogous to the usage in Jupyter notebooks minus some interactivity.
+Finally, one can also use the module module `py_alf` in custom Python scripts, which is analogous to the usage in Jupyter notebooks minus some interactivity.
 
 ## License
 
 The various works that make up the ALF project are placed under licenses that put
 a strong emphasis on the attribution of the original authors and the sharing of the contained knowledge.
 To that end we have placed the ALF source code under the GPL version 3 license (see license.GPL and license.additional)
 and took the liberty as per GPLv3 section 7 to include additional terms that deal with the attribution
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyalf-2.5.post1/pyALF.egg-info/PKG-INFO` & `pyalf-2.5.post2/pyALF.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyALF
-Version: 2.5.post1
+Version: 2.5.post2
 Summary: Python interface for ALF, plus scripts and Jupyter notebooks.
 Author-email: ALF Collaboration <alf@physik.uni-wuerzburg.de>, Jonas Schwab <jonas.schwab@uni-wuerzburg.de>
 Project-URL: Homepage, https://git.physik.uni-wuerzburg.de/ALF/pyALF
 Project-URL: Issues, https://git.physik.uni-wuerzburg.de/ALF/pyALF/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
@@ -38,38 +38,48 @@
 * The Python module `py_alf`, exposing all the package's utility to Python.
 * A set of command line tools in the folder `py_alf/cli`, that make it easy to leverage pyALF from a Unix shell.
 * Jupyter notebooks in the folder `Notebooks`, serving as an easy introduction to QMC and ALF
 * Python Scripts in the folder `Scripts` that can be run to reproduce benchmark results for established models
 
 The **documentation** can be found [here](http://gitpages.physik.uni-wuerzburg.de/Jonas_schwab/pyalf-docu).
 
-## Prerequisites
+## Installation
 
-* Python3
-* Jupyter
-* The following Python packages:
-  * h5py
-  * numpy
-  * pandas
-  * matplotlib
-  * numba
-  * scipy
-  * tkinter
-  * ipywidgets
-  * ipympl
-  * f90nml
-* The libraries Lapack and Blas
-* A Fortran compiler, such as gfortran or ifort,
+---
+**⚠️ NOTE**
 
-where the last two are required by the main package [ALF](https://git.physik.uni-wuerzburg.de/ALF).
+In previous versions of pyALF, the installation instructions asked the users to set the environment variable `PYTHONPATH`.
+This conflicts with the newer pip package, therefore you should remove definitions of this environment variable related to pyALF.
 
-Also, add pyALF's path to your environment variable `PYTHONPATH`. In Linux, this can be achieved, e.g., by adding the following line to `~/.bashrc` if the used shell if bash or `~/.zshrc`, if the shell is zsh:
+---
+
+pyALF can be installed via the Python package installer [pip](https://pip.pypa.io/en/stable/).
 
 ```bash
-export PYTHONPATH="/local/path/to/pyALF:$PYTHONPATH"
+pip install pyALF
+```
+
+### Development installation
+
+If you want to develop pyALF, you can clone the repository and install it in
+[development mode](https://setuptools.pypa.io/en/latest/userguide/development_mode.html),
+which allows you to edit the files while using them like an installed package.
+For this, it is highly recommended to use a dedicated Python environment using e.g.
+[Python venv](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/)
+or a
+[conda environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).
+The following example shows how to install pyALF in development mode using venv.
+
+```bash
+git clone https://git.physik.uni-wuerzburg.de/ALF/pyALF.git
+cd pyALF
+python -m venv .venv
+source .venv/bin/activate
+
+pip install --editable .
 ```
 
 ## Usage
 
 There are multiple ways to use pyALF, which roughly breaks down into three approaches:
 * Using Jupyter notebooks
 * Using the command line interface
@@ -89,31 +99,28 @@
 jupyter-lab
 ```
 
 which opens the "notebook dashboard" in your default browser, from where one can open the sample notebooks in `Notebooks/` and create new notebooks.
 
 ### Command line interface
 
-pyALF also delivers a set of command line scripts, located in the folder `/py_alf/cli/`, to be use from a UNIX shell. For convenient access, it makes sense to add the folder to the environment variable `PATH`:
+pyALF also delivers a set of command line scripts, to be use from a UNIX shell. For a full list of command line scripts see [here](gitpages.physik.uni-wuerzburg.de/Jonas_schwab/pyalf-docu/source/reference/cli.html).
 
-```bash
-export PATH="/path/to/pyALF/py_alf/cli:$PATH"
-```
-
-Then the scripts can simply be called by their names, try e.g. 
+Try, e.g.
 
 ```bash
-alf_run.py -h
+alf_run -h
 ```
 
-For a full list of command line scripts see [here](gitpages.physik.uni-wuerzburg.de/Jonas_schwab/pyalf-docu/source/reference/cli.html).
+The source code for the scripts can be found in the folder `/py_alf/cli/`.
+
 
 ### Use module `py_alf` in custom scripts
 
-Finally, one can also use the module module `py_alf` in custon Python scripts, which is analogous to the usage in Jupyter notebooks minus some interactivity.
+Finally, one can also use the module module `py_alf` in custom Python scripts, which is analogous to the usage in Jupyter notebooks minus some interactivity.
 
 ## License
 
 The various works that make up the ALF project are placed under licenses that put
 a strong emphasis on the attribution of the original authors and the sharing of the contained knowledge.
 To that end we have placed the ALF source code under the GPL version 3 license (see license.GPL and license.additional)
 and took the liberty as per GPLv3 section 7 to include additional terms that deal with the attribution
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyalf-2.5.post1/pyALF.egg-info/SOURCES.txt` & `pyalf-2.5.post2/pyALF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post1/py_alf/__init__.py` & `pyalf-2.5.post2/py_alf/__init__.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post1/py_alf/alf_source.py` & `pyalf-2.5.post2/py_alf/alf_source.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post1/py_alf/ana.py` & `pyalf-2.5.post2/py_alf/ana.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post1/py_alf/analysis.py` & `pyalf-2.5.post2/py_alf/analysis.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post1/py_alf/check_common.py` & `pyalf-2.5.post2/py_alf/check_common.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post1/py_alf/check_rebin_ipy.py` & `pyalf-2.5.post2/py_alf/check_rebin_ipy.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post1/py_alf/check_rebin_tk.py` & `pyalf-2.5.post2/py_alf/check_rebin_tk.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post1/py_alf/check_warmup_ipy.py` & `pyalf-2.5.post2/py_alf/check_warmup_ipy.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post1/py_alf/check_warmup_tk.py` & `pyalf-2.5.post2/py_alf/check_warmup_tk.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post1/py_alf/cli/alf_bin_count.py` & `pyalf-2.5.post2/py_alf/cli/alf_bin_count.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post1/py_alf/cli/alf_del_bins.py` & `pyalf-2.5.post2/py_alf/cli/alf_del_bins.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post1/py_alf/cli/alf_postprocess.py` & `pyalf-2.5.post2/py_alf/cli/alf_postprocess.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post1/py_alf/cli/alf_run.py` & `pyalf-2.5.post2/py_alf/cli/alf_run.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post1/py_alf/cli/alf_show_obs.py` & `pyalf-2.5.post2/py_alf/cli/alf_show_obs.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post1/py_alf/cli/alf_test_branch.py` & `pyalf-2.5.post2/py_alf/cli/alf_test_branch.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post1/py_alf/cli/minimal_ALF_run.py` & `pyalf-2.5.post2/py_alf/cli/minimal_ALF_run.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post1/py_alf/init_layout.py` & `pyalf-2.5.post2/py_alf/init_layout.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post1/py_alf/lattice.py` & `pyalf-2.5.post2/py_alf/lattice.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post1/py_alf/lattices_armv8.4-a.so` & `pyalf-2.5.post2/py_alf/lattices_armv8.4-a.so`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post1/py_alf/lattices_x86-64.so` & `pyalf-2.5.post2/py_alf/lattices_x86-64.so`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post1/py_alf/simulation.py` & `pyalf-2.5.post2/py_alf/simulation.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post1/py_alf/utils.py` & `pyalf-2.5.post2/py_alf/utils.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post1/pyproject.toml` & `pyalf-2.5.post2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post1/tests/test_lattice_init.py` & `pyalf-2.5.post2/tests/test_lattice_init.py`

 * *Files identical despite different names*

