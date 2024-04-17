# Comparing `tmp/tensorpowerflow-0.0.5.tar.gz` & `tmp/tensorpowerflow-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorpowerflow-0.0.5.tar", last modified: Fri Nov 11 11:37:37 2022, max compression
+gzip compressed data, was "tensorpowerflow-0.0.7.tar", last modified: Wed Apr 17 14:54:33 2024, max compression
```

## Comparing `tensorpowerflow-0.0.5.tar` & `tensorpowerflow-0.0.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2022-11-11 11:37:37.938795 tensorpowerflow-0.0.5/
--rw-rw-rw-   0        0        0     1086 2022-07-06 19:08:06.000000 tensorpowerflow-0.0.5/LICENSE
--rw-rw-rw-   0        0        0        0 2022-07-08 13:37:27.000000 tensorpowerflow-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     5334 2022-11-11 11:37:37.938795 tensorpowerflow-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4600 2022-11-11 11:35:05.000000 tensorpowerflow-0.0.5/README.rst
--rw-rw-rw-   0        0        0     1526 2022-11-11 11:36:21.000000 tensorpowerflow-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-11-11 11:37:37.939795 tensorpowerflow-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      144 2022-07-06 19:17:21.000000 tensorpowerflow-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-11 11:37:37.795679 tensorpowerflow-0.0.5/tensorpowerflow/
--rw-rw-rw-   0        0        0      354 2022-11-11 11:36:21.000000 tensorpowerflow-0.0.5/tensorpowerflow/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-11 11:37:37.835231 tensorpowerflow-0.0.5/tensorpowerflow/data/
--rw-rw-rw-   0        0        0       46 2022-06-17 14:22:53.000000 tensorpowerflow-0.0.5/tensorpowerflow/data/Lines_2.csv
--rw-rw-rw-   0        0        0      865 2021-06-17 09:19:40.000000 tensorpowerflow-0.0.5/tensorpowerflow/data/Lines_34.csv
--rw-rw-rw-   0        0        0       62 2022-06-17 15:10:48.000000 tensorpowerflow-0.0.5/tensorpowerflow/data/Nodes_2.csv
--rw-rw-rw-   0        0        0      897 2021-06-17 09:19:42.000000 tensorpowerflow-0.0.5/tensorpowerflow/data/Nodes_34.csv
-drwxrwxrwx   0        0        0        0 2022-11-11 11:37:37.850439 tensorpowerflow-0.0.5/tensorpowerflow/gpu_tensor/
--rw-rw-rw-   0        0        0       39 2022-11-03 13:58:50.000000 tensorpowerflow-0.0.5/tensorpowerflow/gpu_tensor/__init__.py
--rw-rw-rw-   0        0        0     5433 2022-11-10 14:19:09.000000 tensorpowerflow-0.0.5/tensorpowerflow/gpu_tensor/gpu_interface.py
--rw-rw-rw-   0        0        0    44477 2022-11-11 11:22:35.000000 tensorpowerflow-0.0.5/tensorpowerflow/grid.py
--rw-rw-rw-   0        0        0     8702 2022-11-07 16:24:21.000000 tensorpowerflow-0.0.5/tensorpowerflow/numbarize.py
-drwxrwxrwx   0        0        0        0 2022-11-11 11:37:37.889980 tensorpowerflow-0.0.5/tensorpowerflow/pyMKL/
--rw-rw-rw-   0        0        0     1839 2022-09-14 21:59:07.000000 tensorpowerflow-0.0.5/tensorpowerflow/pyMKL/MKLutils.py
--rw-rw-rw-   0        0        0      128 2022-10-04 09:10:50.000000 tensorpowerflow-0.0.5/tensorpowerflow/pyMKL/README.txt
-drwxrwxrwx   0        0        0        0 2022-11-11 11:37:37.909325 tensorpowerflow-0.0.5/tensorpowerflow/pyMKL/Tests/
--rw-rw-rw-   0        0        0      764 2022-09-14 19:25:42.000000 tensorpowerflow-0.0.5/tensorpowerflow/pyMKL/Tests/test_MKLUtils.py
--rw-rw-rw-   0        0        0     6383 2022-09-14 19:25:42.000000 tensorpowerflow-0.0.5/tensorpowerflow/pyMKL/Tests/test_Pardiso.py
--rw-rw-rw-   0        0        0      669 2022-11-08 14:06:10.000000 tensorpowerflow-0.0.5/tensorpowerflow/pyMKL/__init__.py
--rw-rw-rw-   0        0        0     1141 2022-10-10 14:55:27.000000 tensorpowerflow-0.0.5/tensorpowerflow/pyMKL/loadMKL.py
--rw-rw-rw-   0        0        0     1322 2022-09-14 21:59:22.000000 tensorpowerflow-0.0.5/tensorpowerflow/pyMKL/pardisoInterface.py
--rw-rw-rw-   0        0        0     8756 2022-09-29 08:41:59.000000 tensorpowerflow-0.0.5/tensorpowerflow/pyMKL/pardisoSolver.py
-drwxrwxrwx   0        0        0        0 2022-11-11 11:37:37.935793 tensorpowerflow-0.0.5/tensorpowerflow/tests/
--rw-rw-rw-   0        0        0        0 2022-07-05 18:05:43.000000 tensorpowerflow-0.0.5/tensorpowerflow/tests/__init__.py
--rw-rw-rw-   0        0        0     2346 2022-11-10 14:03:19.000000 tensorpowerflow-0.0.5/tensorpowerflow/tests/test_powerflows.py
--rw-rw-rw-   0        0        0     1558 2022-11-10 16:40:21.000000 tensorpowerflow-0.0.5/tensorpowerflow/tests/test_powerflows_pardiso_gpu.py
--rw-rw-rw-   0        0        0      558 2022-11-11 08:46:38.000000 tensorpowerflow-0.0.5/tensorpowerflow/tests/test_tensor_power_flow.py
--rw-rw-rw-   0        0        0     6589 2022-10-04 16:41:39.000000 tensorpowerflow-0.0.5/tensorpowerflow/utils.py
-drwxrwxrwx   0        0        0        0 2022-11-11 11:37:37.821423 tensorpowerflow-0.0.5/tensorpowerflow.egg-info/
--rw-rw-rw-   0        0        0     5334 2022-11-11 11:37:37.000000 tensorpowerflow-0.0.5/tensorpowerflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1051 2022-11-11 11:37:37.000000 tensorpowerflow-0.0.5/tensorpowerflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-11 11:37:37.000000 tensorpowerflow-0.0.5/tensorpowerflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      162 2022-11-11 11:37:37.000000 tensorpowerflow-0.0.5/tensorpowerflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-11-11 11:37:37.000000 tensorpowerflow-0.0.5/tensorpowerflow.egg-info/top_level.txt
+drwxr-xr-x   0 mauricio   (501) staff       (20)        0 2024-04-17 14:54:33.665769 tensorpowerflow-0.0.7/
+-rw-r--r--   0 mauricio   (501) staff       (20)     1086 2024-04-16 10:02:10.000000 tensorpowerflow-0.0.7/LICENSE
+-rw-r--r--   0 mauricio   (501) staff       (20)        0 2024-04-16 10:02:10.000000 tensorpowerflow-0.0.7/MANIFEST.in
+-rw-r--r--   0 mauricio   (501) staff       (20)     6041 2024-04-17 14:54:33.665586 tensorpowerflow-0.0.7/PKG-INFO
+-rw-r--r--   0 mauricio   (501) staff       (20)     4868 2024-04-17 13:43:18.000000 tensorpowerflow-0.0.7/README.md
+-rw-r--r--   0 mauricio   (501) staff       (20)     1510 2024-04-17 14:54:21.000000 tensorpowerflow-0.0.7/pyproject.toml
+-rw-r--r--   0 mauricio   (501) staff       (20)       38 2024-04-17 14:54:33.665804 tensorpowerflow-0.0.7/setup.cfg
+-rw-r--r--   0 mauricio   (501) staff       (20)      144 2024-04-16 10:02:10.000000 tensorpowerflow-0.0.7/setup.py
+drwxr-xr-x   0 mauricio   (501) staff       (20)        0 2024-04-17 14:54:33.660645 tensorpowerflow-0.0.7/tensorpowerflow/
+-rw-r--r--   0 mauricio   (501) staff       (20)      354 2024-04-16 10:02:10.000000 tensorpowerflow-0.0.7/tensorpowerflow/__init__.py
+drwxr-xr-x   0 mauricio   (501) staff       (20)        0 2024-04-17 14:54:33.662128 tensorpowerflow-0.0.7/tensorpowerflow/data/
+-rw-r--r--   0 mauricio   (501) staff       (20)       44 2024-04-16 10:02:10.000000 tensorpowerflow-0.0.7/tensorpowerflow/data/Lines_2.csv
+-rw-r--r--   0 mauricio   (501) staff       (20)      831 2024-04-16 10:02:10.000000 tensorpowerflow-0.0.7/tensorpowerflow/data/Lines_34.csv
+-rw-r--r--   0 mauricio   (501) staff       (20)       59 2024-04-16 10:02:10.000000 tensorpowerflow-0.0.7/tensorpowerflow/data/Nodes_2.csv
+-rw-r--r--   0 mauricio   (501) staff       (20)      862 2024-04-16 10:02:10.000000 tensorpowerflow-0.0.7/tensorpowerflow/data/Nodes_34.csv
+drwxr-xr-x   0 mauricio   (501) staff       (20)        0 2024-04-17 14:54:33.662385 tensorpowerflow-0.0.7/tensorpowerflow/gpu_tensor/
+-rw-r--r--   0 mauricio   (501) staff       (20)       39 2024-04-16 10:02:10.000000 tensorpowerflow-0.0.7/tensorpowerflow/gpu_tensor/__init__.py
+-rw-r--r--   0 mauricio   (501) staff       (20)     5558 2024-04-16 15:52:27.000000 tensorpowerflow-0.0.7/tensorpowerflow/gpu_tensor/gpu_interface.py
+-rw-r--r--   0 mauricio   (501) staff       (20)    43853 2024-04-17 13:43:18.000000 tensorpowerflow-0.0.7/tensorpowerflow/grid.py
+-rw-r--r--   0 mauricio   (501) staff       (20)     6828 2024-04-17 13:43:18.000000 tensorpowerflow-0.0.7/tensorpowerflow/numbarize.py
+drwxr-xr-x   0 mauricio   (501) staff       (20)        0 2024-04-17 14:54:33.663349 tensorpowerflow-0.0.7/tensorpowerflow/pyMKL/
+-rw-r--r--   0 mauricio   (501) staff       (20)     1787 2024-04-16 10:02:10.000000 tensorpowerflow-0.0.7/tensorpowerflow/pyMKL/MKLutils.py
+-rw-r--r--   0 mauricio   (501) staff       (20)      128 2024-04-16 10:02:10.000000 tensorpowerflow-0.0.7/tensorpowerflow/pyMKL/README.txt
+drwxr-xr-x   0 mauricio   (501) staff       (20)        0 2024-04-17 14:54:33.663910 tensorpowerflow-0.0.7/tensorpowerflow/pyMKL/Tests/
+-rw-r--r--   0 mauricio   (501) staff       (20)      783 2024-04-16 16:34:13.000000 tensorpowerflow-0.0.7/tensorpowerflow/pyMKL/Tests/trial_MKLUtils.py
+-rw-r--r--   0 mauricio   (501) staff       (20)     6185 2024-04-17 13:43:18.000000 tensorpowerflow-0.0.7/tensorpowerflow/pyMKL/Tests/trial_Pardiso.py
+-rw-r--r--   0 mauricio   (501) staff       (20)      647 2024-04-16 10:02:10.000000 tensorpowerflow-0.0.7/tensorpowerflow/pyMKL/__init__.py
+-rw-r--r--   0 mauricio   (501) staff       (20)     1107 2024-04-16 10:02:10.000000 tensorpowerflow-0.0.7/tensorpowerflow/pyMKL/loadMKL.py
+-rw-r--r--   0 mauricio   (501) staff       (20)     1287 2024-04-16 10:02:10.000000 tensorpowerflow-0.0.7/tensorpowerflow/pyMKL/pardisoInterface.py
+-rw-r--r--   0 mauricio   (501) staff       (20)     8566 2024-04-16 10:02:10.000000 tensorpowerflow-0.0.7/tensorpowerflow/pyMKL/pardisoSolver.py
+drwxr-xr-x   0 mauricio   (501) staff       (20)        0 2024-04-17 14:54:33.664649 tensorpowerflow-0.0.7/tensorpowerflow/tests/
+-rw-r--r--   0 mauricio   (501) staff       (20)        0 2024-04-16 10:02:10.000000 tensorpowerflow-0.0.7/tensorpowerflow/tests/__init__.py
+-rw-r--r--   0 mauricio   (501) staff       (20)     2415 2024-04-17 13:43:18.000000 tensorpowerflow-0.0.7/tensorpowerflow/tests/test_powerflows.py
+-rw-r--r--   0 mauricio   (501) staff       (20)     1857 2024-04-17 13:43:18.000000 tensorpowerflow-0.0.7/tensorpowerflow/tests/test_powerflows_pardiso_gpu.py
+-rw-r--r--   0 mauricio   (501) staff       (20)      586 2024-04-16 16:29:00.000000 tensorpowerflow-0.0.7/tensorpowerflow/tests/test_tensor_power_flow.py
+-rw-r--r--   0 mauricio   (501) staff       (20)     7118 2024-04-17 13:43:18.000000 tensorpowerflow-0.0.7/tensorpowerflow/utils.py
+drwxr-xr-x   0 mauricio   (501) staff       (20)        0 2024-04-17 14:54:33.665080 tensorpowerflow-0.0.7/tensorpowerflow.egg-info/
+-rw-r--r--   0 mauricio   (501) staff       (20)     6041 2024-04-17 14:54:33.000000 tensorpowerflow-0.0.7/tensorpowerflow.egg-info/PKG-INFO
+-rw-r--r--   0 mauricio   (501) staff       (20)     1052 2024-04-17 14:54:33.000000 tensorpowerflow-0.0.7/tensorpowerflow.egg-info/SOURCES.txt
+-rw-r--r--   0 mauricio   (501) staff       (20)        1 2024-04-17 14:54:33.000000 tensorpowerflow-0.0.7/tensorpowerflow.egg-info/dependency_links.txt
+-rw-r--r--   0 mauricio   (501) staff       (20)      194 2024-04-17 14:54:33.000000 tensorpowerflow-0.0.7/tensorpowerflow.egg-info/requires.txt
+-rw-r--r--   0 mauricio   (501) staff       (20)       16 2024-04-17 14:54:33.000000 tensorpowerflow-0.0.7/tensorpowerflow.egg-info/top_level.txt
```

### Comparing `tensorpowerflow-0.0.5/LICENSE` & `tensorpowerflow-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorpowerflow-0.0.5/PKG-INFO` & `tensorpowerflow-0.0.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,134 +1,129 @@
-Metadata-Version: 2.1
-Name: tensorpowerflow
-Version: 0.0.5
-Summary: Ultra fast power flow based in Laurent series expansion.
-Author-email: e.m.salazar.duque@tue.nl
-License: MIT
-Project-URL: repository, https://github.com/MauricioSalazare/tensorpowerflow
-Keywords: power flow,power systems,time series loading
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.0
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-Provides-Extra: test
-Provides-Extra: doc
-License-File: LICENSE
-
-.. Binder
-.. image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/MauricioSalazare/tensorpowerflow/master?urlpath=lab/tree/examples
-   :alt: binder
-
-.. License
-.. image:: https://img.shields.io/github/license/MauricioSalazare/tensorpowerflow
-   :target: https://github.com/MauricioSalazare/tensorpowerflow/blob/master/LICENSE
-
-.. Python versions supported
-.. image:: https://img.shields.io/pypi/pyversions/tensorpowerflow.svg
-   :target: https://pypi.python.org/pypi/tensorpowerflow/
-
-.. Downloads per month
-.. image:: https://img.shields.io/pypi/dm/tensorpowerflow.svg
-   :target: https://pypi.python.org/pypi/tensorpowerflow/
-
-.. Code size
-.. image:: https://img.shields.io/github/languages/code-size/MauricioSalazare/tensorpowerflow
-   :target: https://github.com/MauricioSalazare/tensorpowerflow
-
-.. PyPi version
-.. image:: https://img.shields.io/pypi/v/tensorpowerflow
-   :target: https://pypi.python.org/pypi/tensorpowerflow/
-
-.. Build (GithubActions)
-.. image:: https://img.shields.io/github/workflow/status/MauricioSalazare/tensorpowerflow/Python%20package/master
-   :target: https://github.com/MauricioSalazare/tensorpowerflow/actions
-
-.. Test (GithubActions)
-.. image:: https://img.shields.io/github/workflow/status/MauricioSalazare/tensorpowerflow/Python%20package/master?label=tests
-   :target: https://github.com/MauricioSalazare/tensorpowerflow/actions
-
-
-
-
-TensorPowerFlow
-===============
-
-
-What is TensorPowerFlow?
-------------------------
-
-An ultra-fast power flow based on Laurent series expansion. The power flow is intended for applications where massive
-amounts of power flow computations are required. e.g., electrical load time series, metaheuristics, electrical grid
-environments for reinforcement learning.
-
-How to install
---------------
-The package can be installed via pip using:
-
-.. code:: shell
-
-    pip install tensorpowerflow
-
-Example:
---------
-Run the load base case as:
-
-.. code-block:: python
-
-    from tensorpowerflow import GridTensor
-    import numpy as np
-    from time import perf_counter
-
-    #%% Solve base case (34 node bus)
-    network = GridTensor()
-    solution = network.run_pf()
-    print(solution["v"])
-
-    #%% Solve 10_000 power flows on the 34 node bus case.
-    network_size = network.nb - 1  # Size of network without slack bus.
-    active_ns = np.random.normal(50, scale=1, size=(10_000, network_size)) # Power in kW
-    reactive_ns = active_ns * 0.1  # kVAr
-    solution_tensor = network.run_pf(active_power=active_ns, reactive_power=reactive_ns)
-    print(solution_tensor["v"])
-
-    #%% Generate random radial network of 100 nodes and a maximum of 1 to 3 branches per node.
-    network_rnd = GridTensor.generate_from_graph(nodes=100, child=3, plot_graph=True)
-    solution_rnd = network_rnd.run_pf()
-    print(solution_rnd["v"])
-
-    #%% Solve a tensor power flow. For 10 scenarios, 8_760 time steps (one year - 1 hr res), for the 33 PQ nodes.
-    # Meaning that the dimensions of the tensor is (10, 8_760, 33)
-
-    network = GridTensor(numba=True)  # Loads the basic 34 bus node network.
-    active_ns = np.random.normal(50,  # Power in kW
-                                 scale=10,
-                                 size=(10, 8_760, 33)).round(3)  # Assume 1 slack variable
-    reactive_ns = (active_ns * .1).round(3)  # Constant PF of 0.1
-
-    start_tensor_dense = perf_counter()
-    solution = network.run_pf(active_power=active_ns, reactive_power=reactive_ns, algorithm="tensor")
-    t_tensor_dense = perf_counter() - start_tensor_dense
-    assert solution["convergence"], "Algorithm did not converge."
-    assert solution["v"].shape == active_ns.shape
-    print(f"Time tensor dense: {t_tensor_dense:.3f} sec.")
-
-More examples can be found in the `examples folder <https://github.com/MauricioSalazare/tensorpowerflow/tree/master/examples>`_ (under development).
-Also, you can try the package via jupyter lab clicking in the binder icon:
-
-.. image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/MauricioSalazare/tensorpowerflow/master?urlpath=lab/tree/examples
-   :alt: binder
-
-Reading and citations:
-----------------------
-The mathematical formulation of the power flow can be found at:
-
-*"A Fixed-Point Current Injection Power Flow for Electric Distribution Systems using Laurent Series."* J.S. Giraldo,
-O.D. Montoya, P.P. Vergara, F. Milano. Power Systems Computational Conference (PSCC) 2022. `link <http://faraday1.ucd.ie/archive/papers/laurent.pdf>`_
-
-
-How to contact us
------------------
-Any questions, suggestions or collaborations contact Juan S. Giraldo at <jnse@ieee.org>
+Metadata-Version: 2.1
+Name: tensorpowerflow
+Version: 0.0.7
+Summary: Ultra fast power flow based in Laurent series expansion.
+Author-email: Mauricio Salazar <e.m.salazar.duque@tue.nl>
+License: MIT
+Project-URL: repository, https://github.com/MauricioSalazare/tensorpowerflow
+Keywords: power flow,power systems,time series loading
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: scipy
+Requires-Dist: tqdm
+Requires-Dist: numba>=0.53.0
+Requires-Dist: networkx
+Requires-Dist: seaborn
+Requires-Dist: pandapower
+Requires-Dist: mkl; platform_system != "Darwin"
+Requires-Dist: psutil
+Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: matplotlib; extra == "dev"
+Requires-Dist: jupyterlab; extra == "dev"
+Requires-Dist: tox; extra == "dev"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Provides-Extra: doc
+Requires-Dist: sphinx; extra == "doc"
+
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/MauricioSalazare/tensorpowerflow/master?urlpath=lab/tree/examples)
+[![MIT License](https://img.shields.io/badge/License-MIT-yellow)](https://github.com/MauricioSalazare/tensorpowerflow/blob/master/LICENSE)
+[![Python versions supported](https://img.shields.io/pypi/pyversions/tensorpowerflow.svg)](https://pypi.python.org/pypi/tensorpowerflow/)
+[![Downloads per month](https://img.shields.io/pypi/dm/tensorpowerflow.svg)](https://pypi.python.org/pypi/tensorpowerflow/)
+[![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/MauricioSalazare/tensorpowerflow)](https://github.com/MauricioSalazare/tensorpowerflow)
+[![PyPI - Version](https://img.shields.io/pypi/v/tensorpowerflow)](https://pypi.python.org/pypi/tensorpowerflow/)
+[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/MauricioSalazare/tensorpowerflow/python-package.yml)](https://github.com/MauricioSalazare/tensorpowerflow/actions)
+
+
+# TensorPowerFlow
+
+## What is TensorPowerFlow?
+An ultra-fast power flow based on a fixed-point iteration algorithm. The power flow is intended for applications requiring massive
+amounts of power flow computations. e.g., electrical load time series, metaheuristics, and electrical grid
+environments for reinforcement learning.
+
+## How to install
+
+The package can be installed via pip using:
+
+```shell
+pip install tensorpowerflow
+```
+
+## Example:
+
+Here we show four examples of what can be done with the packages:
+1. *Example 1:* The package comes with a preloaded network case of 34 nodes that can be solved by default. 
+2. *Example 2:* Solve 10.000 PF for the default network case. The active power for the nodes is generated by sampling a Normal 
+    distribution.
+3. *Example 3:* The GridTensor class can generate a random grid using the `GridTensor.generate_from_graph()` method.
+    The parameters `nodes` and `child`, respectively, can control the number of nodes and branching per node.
+4. *Example 4:* We test the grid with a tensor of 3 dimensions. The first dimension is the number of scenarios 
+    (10 in the example). The second dimension is the number of time steps (8.760 to simulate a 30-minute resolution 
+    consumption for one year). The third dimension is the number of PQ nodes in the grid (33 PQ nodes for the base 
+    grid case).
+
+```python
+from tensorpowerflow import GridTensor
+import numpy as np
+from time import perf_counter
+
+#%% Example 1: Solve base case (34 node bus)
+network = GridTensor(gpu_mode=False)
+solution = network.run_pf()
+print(solution["v"])
+
+#%% Example 2: Solve 10_000 power flows on the 34 node bus network case.
+network_size = network.nb - 1 # Size of the network without the slack bus.
+active_ns = np.random.normal(50, scale=1, size=(10_000, network_size)) # Power in kW
+reactive_ns = active_ns * 0.1  # kVAr
+solution_tensor = network.run_pf(active_power=active_ns, reactive_power=reactive_ns)
+print(solution_tensor["v"])
+
+#%% Example 3: Generate a random radial network of 100 nodes and a maximum of 1 to 3 branches per node.
+network_rnd = GridTensor.generate_from_graph(nodes=100, child=3, plot_graph=True)
+solution_rnd = network_rnd.run_pf()
+print(solution_rnd["v"])
+
+#%% Example 4: Solve a tensor power flow. For 10 scenarios, 8_760 time steps (one year - 1 hr res) for the 33 PQ nodes.
+# Meaning that the dimensions of the tensor are (10, 8_760, 33)
+
+network = GridTensor(numba=True)  # Loads the basic 34 bus node network.
+active_ns = np.random.normal(50,  # Power in kW
+                             scale=10,
+                             size=(10, 8_760, 33)).round(3)  # Assume 1 slack variable
+reactive_ns = (active_ns * .1).round(3)  # Constant PF of 0.1
+
+start_tensor_dense = perf_counter()
+solution = network.run_pf(active_power=active_ns, reactive_power=reactive_ns, algorithm="tensor")
+t_tensor_dense = perf_counter() - start_tensor_dense
+assert solution["convergence"], "Algorithm did not converge."
+assert solution["v"].shape == active_ns.shape
+print(f"Time tensor dense: {t_tensor_dense:.3f} sec.")
+
+
+```
+
+More examples can be found in the [examples folder](examples) (under development).
+Also, you can try the package via Jupyter lab by clicking on the binder icon:
+
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/MauricioSalazare/tensorpowerflow/master?urlpath=lab/tree/examples)
+
+## Reading and citations:
+
+The mathematical formulation of the power flow can be found at:
+
+> *"Tensor Power Flow Formulations for Multidimensional Analyses in Distribution Systems."* E.M. Salazar Duque,
+Juan S. Giraldo, Pedro P. Vergara, Phuong H. Nguyen, and Han (J.G.) Slootweg. [arXiv:2403.04578 (2024)](https://arxiv.org/pdf/2403.04578).
+
+## How to contact us
+
+For any questions, suggestions or collaborations, contact Juan S. Giraldo at <jnse@ieee.org>
```

### Comparing `tensorpowerflow-0.0.5/README.rst` & `tensorpowerflow-0.0.7/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,116 +1,93 @@
-.. Binder
-.. image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/MauricioSalazare/tensorpowerflow/master?urlpath=lab/tree/examples
-   :alt: binder
-
-.. License
-.. image:: https://img.shields.io/github/license/MauricioSalazare/tensorpowerflow
-   :target: https://github.com/MauricioSalazare/tensorpowerflow/blob/master/LICENSE
-
-.. Python versions supported
-.. image:: https://img.shields.io/pypi/pyversions/tensorpowerflow.svg
-   :target: https://pypi.python.org/pypi/tensorpowerflow/
-
-.. Downloads per month
-.. image:: https://img.shields.io/pypi/dm/tensorpowerflow.svg
-   :target: https://pypi.python.org/pypi/tensorpowerflow/
-
-.. Code size
-.. image:: https://img.shields.io/github/languages/code-size/MauricioSalazare/tensorpowerflow
-   :target: https://github.com/MauricioSalazare/tensorpowerflow
-
-.. PyPi version
-.. image:: https://img.shields.io/pypi/v/tensorpowerflow
-   :target: https://pypi.python.org/pypi/tensorpowerflow/
-
-.. Build (GithubActions)
-.. image:: https://img.shields.io/github/workflow/status/MauricioSalazare/tensorpowerflow/Python%20package/master
-   :target: https://github.com/MauricioSalazare/tensorpowerflow/actions
-
-.. Test (GithubActions)
-.. image:: https://img.shields.io/github/workflow/status/MauricioSalazare/tensorpowerflow/Python%20package/master?label=tests
-   :target: https://github.com/MauricioSalazare/tensorpowerflow/actions
-
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/MauricioSalazare/tensorpowerflow/master?urlpath=lab/tree/examples)
+[![MIT License](https://img.shields.io/badge/License-MIT-yellow)](https://github.com/MauricioSalazare/tensorpowerflow/blob/master/LICENSE)
+[![Python versions supported](https://img.shields.io/pypi/pyversions/tensorpowerflow.svg)](https://pypi.python.org/pypi/tensorpowerflow/)
+[![Downloads per month](https://img.shields.io/pypi/dm/tensorpowerflow.svg)](https://pypi.python.org/pypi/tensorpowerflow/)
+[![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/MauricioSalazare/tensorpowerflow)](https://github.com/MauricioSalazare/tensorpowerflow)
+[![PyPI - Version](https://img.shields.io/pypi/v/tensorpowerflow)](https://pypi.python.org/pypi/tensorpowerflow/)
+[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/MauricioSalazare/tensorpowerflow/python-package.yml)](https://github.com/MauricioSalazare/tensorpowerflow/actions)
 
 
+# TensorPowerFlow
+
+## What is TensorPowerFlow?
+An ultra-fast power flow based on a fixed-point iteration algorithm. The power flow is intended for applications requiring massive
+amounts of power flow computations. e.g., electrical load time series, metaheuristics, and electrical grid
+environments for reinforcement learning.
 
-TensorPowerFlow
-===============
+## How to install
 
+The package can be installed via pip using:
 
-What is TensorPowerFlow?
-------------------------
+```shell
+pip install tensorpowerflow
+```
+
+## Example:
+
+Here we show four examples of what can be done with the packages:
+1. *Example 1:* The package comes with a preloaded network case of 34 nodes that can be solved by default. 
+2. *Example 2:* Solve 10.000 PF for the default network case. The active power for the nodes is generated by sampling a Normal 
+    distribution.
+3. *Example 3:* The GridTensor class can generate a random grid using the `GridTensor.generate_from_graph()` method.
+    The parameters `nodes` and `child`, respectively, can control the number of nodes and branching per node.
+4. *Example 4:* We test the grid with a tensor of 3 dimensions. The first dimension is the number of scenarios 
+    (10 in the example). The second dimension is the number of time steps (8.760 to simulate a 30-minute resolution 
+    consumption for one year). The third dimension is the number of PQ nodes in the grid (33 PQ nodes for the base 
+    grid case).
+
+```python
+from tensorpowerflow import GridTensor
+import numpy as np
+from time import perf_counter
+
+#%% Example 1: Solve base case (34 node bus)
+network = GridTensor(gpu_mode=False)
+solution = network.run_pf()
+print(solution["v"])
+
+#%% Example 2: Solve 10_000 power flows on the 34 node bus network case.
+network_size = network.nb - 1 # Size of the network without the slack bus.
+active_ns = np.random.normal(50, scale=1, size=(10_000, network_size)) # Power in kW
+reactive_ns = active_ns * 0.1  # kVAr
+solution_tensor = network.run_pf(active_power=active_ns, reactive_power=reactive_ns)
+print(solution_tensor["v"])
+
+#%% Example 3: Generate a random radial network of 100 nodes and a maximum of 1 to 3 branches per node.
+network_rnd = GridTensor.generate_from_graph(nodes=100, child=3, plot_graph=True)
+solution_rnd = network_rnd.run_pf()
+print(solution_rnd["v"])
+
+#%% Example 4: Solve a tensor power flow. For 10 scenarios, 8_760 time steps (one year - 1 hr res) for the 33 PQ nodes.
+# Meaning that the dimensions of the tensor are (10, 8_760, 33)
+
+network = GridTensor(numba=True)  # Loads the basic 34 bus node network.
+active_ns = np.random.normal(50,  # Power in kW
+                             scale=10,
+                             size=(10, 8_760, 33)).round(3)  # Assume 1 slack variable
+reactive_ns = (active_ns * .1).round(3)  # Constant PF of 0.1
+
+start_tensor_dense = perf_counter()
+solution = network.run_pf(active_power=active_ns, reactive_power=reactive_ns, algorithm="tensor")
+t_tensor_dense = perf_counter() - start_tensor_dense
+assert solution["convergence"], "Algorithm did not converge."
+assert solution["v"].shape == active_ns.shape
+print(f"Time tensor dense: {t_tensor_dense:.3f} sec.")
 
-An ultra-fast power flow based on Laurent series expansion. The power flow is intended for applications where massive
-amounts of power flow computations are required. e.g., electrical load time series, metaheuristics, electrical grid
-environments for reinforcement learning.
 
-How to install
---------------
-The package can be installed via pip using:
+```
 
-.. code:: shell
+More examples can be found in the [examples folder](examples) (under development).
+Also, you can try the package via Jupyter lab by clicking on the binder icon:
 
-    pip install tensorpowerflow
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/MauricioSalazare/tensorpowerflow/master?urlpath=lab/tree/examples)
 
-Example:
---------
-Run the load base case as:
-
-.. code-block:: python
-
-    from tensorpowerflow import GridTensor
-    import numpy as np
-    from time import perf_counter
-
-    #%% Solve base case (34 node bus)
-    network = GridTensor()
-    solution = network.run_pf()
-    print(solution["v"])
-
-    #%% Solve 10_000 power flows on the 34 node bus case.
-    network_size = network.nb - 1  # Size of network without slack bus.
-    active_ns = np.random.normal(50, scale=1, size=(10_000, network_size)) # Power in kW
-    reactive_ns = active_ns * 0.1  # kVAr
-    solution_tensor = network.run_pf(active_power=active_ns, reactive_power=reactive_ns)
-    print(solution_tensor["v"])
-
-    #%% Generate random radial network of 100 nodes and a maximum of 1 to 3 branches per node.
-    network_rnd = GridTensor.generate_from_graph(nodes=100, child=3, plot_graph=True)
-    solution_rnd = network_rnd.run_pf()
-    print(solution_rnd["v"])
-
-    #%% Solve a tensor power flow. For 10 scenarios, 8_760 time steps (one year - 1 hr res), for the 33 PQ nodes.
-    # Meaning that the dimensions of the tensor is (10, 8_760, 33)
-
-    network = GridTensor(numba=True)  # Loads the basic 34 bus node network.
-    active_ns = np.random.normal(50,  # Power in kW
-                                 scale=10,
-                                 size=(10, 8_760, 33)).round(3)  # Assume 1 slack variable
-    reactive_ns = (active_ns * .1).round(3)  # Constant PF of 0.1
-
-    start_tensor_dense = perf_counter()
-    solution = network.run_pf(active_power=active_ns, reactive_power=reactive_ns, algorithm="tensor")
-    t_tensor_dense = perf_counter() - start_tensor_dense
-    assert solution["convergence"], "Algorithm did not converge."
-    assert solution["v"].shape == active_ns.shape
-    print(f"Time tensor dense: {t_tensor_dense:.3f} sec.")
-
-More examples can be found in the `examples folder <https://github.com/MauricioSalazare/tensorpowerflow/tree/master/examples>`_ (under development).
-Also, you can try the package via jupyter lab clicking in the binder icon:
-
-.. image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/MauricioSalazare/tensorpowerflow/master?urlpath=lab/tree/examples
-   :alt: binder
+## Reading and citations:
 
-Reading and citations:
-----------------------
 The mathematical formulation of the power flow can be found at:
 
-*"A Fixed-Point Current Injection Power Flow for Electric Distribution Systems using Laurent Series."* J.S. Giraldo,
-O.D. Montoya, P.P. Vergara, F. Milano. Power Systems Computational Conference (PSCC) 2022. `link <http://faraday1.ucd.ie/archive/papers/laurent.pdf>`_
+> *"Tensor Power Flow Formulations for Multidimensional Analyses in Distribution Systems."* E.M. Salazar Duque,
+Juan S. Giraldo, Pedro P. Vergara, Phuong H. Nguyen, and Han (J.G.) Slootweg. [arXiv:2403.04578 (2024)](https://arxiv.org/pdf/2403.04578).
 
+## How to contact us
 
-How to contact us
------------------
-Any questions, suggestions or collaborations contact Juan S. Giraldo at <jnse@ieee.org>
+For any questions, suggestions or collaborations, contact Juan S. Giraldo at <jnse@ieee.org>
```

### Comparing `tensorpowerflow-0.0.5/tensorpowerflow/data/Nodes_34.csv` & `tensorpowerflow-0.0.7/tensorpowerflow/data/Nodes_34.csv`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-NODES,Tb,PD,QD,Pct,Ict,Zct
-1,1,0,0,1,0,0
-2,0,387.09,254.3625,1,0,0
-3,0,0,0,1,0,0
-4,0,387.09,254.3625,1,0,0
-5,0,387.09,254.3625,1,0,0
-6,0,0,0,1,0,0
-7,0,0,0,1,0,0
-8,0,387.09,254.3625,1,0,0
-9,0,387.09,254.3625,1,0,0
-10,0,0,0,1,0,0
-11,0,387.09,254.3625,1,0,0
-12,0,230.571,149.94,1,0,0
-13,0,121.176,80.325,1,0,0
-14,0,121.176,80.325,1,0,0
-15,0,121.176,80.325,1,0,0
-16,0,22.7205,13.3875,1,0,0
-17,0,387.09,254.3625,1,0,0
-18,0,387.09,254.3625,1,0,0
-19,0,387.09,254.3625,1,0,0
-20,0,387.09,254.3625,1,0,0
-21,0,387.09,254.3625,1,0,0
-22,0,387.09,254.3625,1,0,0
-23,0,387.09,254.3625,1,0,0
-24,0,387.09,254.3625,1,0,0
-25,0,387.09,254.3625,1,0,0
-26,0,387.09,254.3625,1,0,0
-27,0,230.571,151.725,1,0,0
-28,0,126.225,85.68,1,0,0
-29,0,126.225,85.68,1,0,0
-30,0,126.225,85.68,1,0,0
-31,0,95.931,66.9375,1,0,0
-32,0,95.931,66.9375,1,0,0
-33,0,95.931,66.9375,1,0,0
-34,0,95.931,66.9375,1,0,0
+NODES,Tb,PD,QD,Pct,Ict,Zct
+1,1,0,0,1,0,0
+2,0,387.09,254.3625,1,0,0
+3,0,0,0,1,0,0
+4,0,387.09,254.3625,1,0,0
+5,0,387.09,254.3625,1,0,0
+6,0,0,0,1,0,0
+7,0,0,0,1,0,0
+8,0,387.09,254.3625,1,0,0
+9,0,387.09,254.3625,1,0,0
+10,0,0,0,1,0,0
+11,0,387.09,254.3625,1,0,0
+12,0,230.571,149.94,1,0,0
+13,0,121.176,80.325,1,0,0
+14,0,121.176,80.325,1,0,0
+15,0,121.176,80.325,1,0,0
+16,0,22.7205,13.3875,1,0,0
+17,0,387.09,254.3625,1,0,0
+18,0,387.09,254.3625,1,0,0
+19,0,387.09,254.3625,1,0,0
+20,0,387.09,254.3625,1,0,0
+21,0,387.09,254.3625,1,0,0
+22,0,387.09,254.3625,1,0,0
+23,0,387.09,254.3625,1,0,0
+24,0,387.09,254.3625,1,0,0
+25,0,387.09,254.3625,1,0,0
+26,0,387.09,254.3625,1,0,0
+27,0,230.571,151.725,1,0,0
+28,0,126.225,85.68,1,0,0
+29,0,126.225,85.68,1,0,0
+30,0,126.225,85.68,1,0,0
+31,0,95.931,66.9375,1,0,0
+32,0,95.931,66.9375,1,0,0
+33,0,95.931,66.9375,1,0,0
+34,0,95.931,66.9375,1,0,0
```

### Comparing `tensorpowerflow-0.0.5/tensorpowerflow/gpu_tensor/gpu_interface.py` & `tensorpowerflow-0.0.7/tensorpowerflow/gpu_tensor/gpu_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 
     if platform == "linux" or platform == "linux2":
         # linux (Hard coded in the meantime)
         so_file = r"/home/mauricio/PycharmProjects/gpu_tensorpf/shared_library_complex.so"
         my_functions = CDLL(so_file)
 
     elif platform == "darwin":
-        raise NotImplementedError("MacOS is not currently supported.")
+        raise NotImplementedError("GPU in MacOS is not currently supported.")
 
     elif platform == "win32":
+        raise NotImplementedError("GPU implementation in Windows is disabled. Contact the maintainer for more info.")
         # TODO: Fallback if the gpu library is not found.
         # Windows.
         # os.add_dll_directory(r"C:\Users\20175334\Documents\PycharmProjects\tensorpowerflow\experiments\dll")
         # dynamic_library = r"C:\Users\20175334\Documents\PycharmProjects\tensorpowerflow\experiments\dll\shared_library_complex.dll"
 
         # Hardcode the directory for debugging purposes.
         os.add_dll_directory(r"C:\Users\20175334\source\repos\gpu_windows\x64\Debug")
```

### Comparing `tensorpowerflow-0.0.5/tensorpowerflow/grid.py` & `tensorpowerflow-0.0.7/tensorpowerflow/grid.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,61 +1,66 @@
 import pandas as pd
 import numpy as np
 from scipy.sparse import csr_matrix, csc_matrix, diags
 from scipy.sparse.linalg import spsolve, inv
-from tensorpowerflow.pyMKL import pardisoSolver
 from time import perf_counter
 from numba import njit, set_num_threads
 import warnings
 from .gpu_tensor import GPUPowerFlow
 from .utils import generate_network, _load_default_34_node_case
-from .numbarize import (pre_power_flow_tensor,
-                        power_flow_tensor,
-                        power_flow_tensor_constant_power,
-                        pre_power_flow_sam_sequential,
-                        power_flow_sam_sequential,
-                        power_flow_sam_sequential_constant_power_only)
+from .numbarize import (
+    pre_power_flow_tensor,
+    power_flow_tensor,
+    power_flow_tensor_constant_power,
+    pre_power_flow_sam_sequential,
+    power_flow_sam_sequential,
+    power_flow_sam_sequential_constant_power_only,
+)
 import psutil
 from tqdm import trange
 
 # TODO List:
 # 1. Allow to specify start value of the voltage (i.e., v_0)
 # 2. Allow to change the voltage in the fixed node.
 # 3. Create a wrapper to run the power flow at least once for tensor methods (circumvent numba compiling times)
 # 4. Improve memory management of Ybus (keep it sparse all times)
 # 5. Create a flag if the pardiso has converged or not (the output is all zeros, but it is better if there is a flag)
 # 6. Improve the construction of the huge M matrix in the tensor-hp
 # 7. In the case that the algorithm didn't reach convergence, reset voltages to zero.
 # 8. Change the chunk method to np.array_split()
 # 9. Fall back to normal CPU mode if the GPU library is not found.
 
+
 class GridTensor:
-    def __init__(self,
-                 node_file_path: str = None,
-                 lines_file_path: str = None,
-                 *,
-                 s_base: int = 1000,  # kVA - 1 phase
-                 v_base: float = 11,  # kV - 1 phase
-                 iterations: int = 100,
-                 tolerance: float = 1e-5,
-                 from_file=True,
-                 nodes_frame: pd.DataFrame = None,
-                 lines_frame: pd.DataFrame = None,
-                 numba=True,
-                 gpu_mode=True):
+    def __init__(
+        self,
+        node_file_path: str = None,
+        lines_file_path: str = None,
+        *,
+        s_base: int = 1000,  # kVA - 1 phase
+        v_base: float = 11,  # kV - 1 phase
+        iterations: int = 100,
+        tolerance: float = 1e-5,
+        from_file=True,
+        nodes_frame: pd.DataFrame = None,
+        lines_frame: pd.DataFrame = None,
+        numba=True,
+        gpu_mode=False
+    ):
 
         self.s_base = s_base
         self.v_base = v_base  # This is better loaded from the file (Extra column)
-        self.z_base = (self.v_base ** 2 * 1000) / self.s_base
+        self.z_base = (self.v_base**2 * 1000) / self.s_base
         self.i_base = self.s_base / (np.sqrt(3) * self.v_base)
 
         self.iterations = iterations
         self.tolerance = tolerance
 
         if node_file_path is None and lines_file_path is None:
+            # here node frame and line frame are given to the inverse value
             _nodes_frame, _lines_frame = _load_default_34_node_case()
             self.branch_info = _nodes_frame
             self.bus_info = _lines_frame
             print("Default case loaded.")
 
         elif node_file_path is not None and lines_file_path is not None and from_file:
             self.branch_info = pd.read_csv(lines_file_path)
@@ -63,17 +68,20 @@
 
         elif nodes_frame is not None and lines_frame is not None:
             self.branch_info = lines_frame
             self.bus_info = nodes_frame
         else:
             raise ValueError("Wrong input configuration")
 
-
-        self.P_file = self.bus_info[self.bus_info.Tb != 1].PD.values  # Vector with all active power except slack
-        self.Q_file = self.bus_info[self.bus_info.Tb != 1].QD.values  # Vector with all reactive power except slack
+        self.P_file = self.bus_info[
+            self.bus_info.Tb != 1
+        ].PD.values  # Vector with all active power except slack
+        self.Q_file = self.bus_info[
+            self.bus_info.Tb != 1
+        ].QD.values  # Vector with all reactive power except slack
 
         self._make_y_bus()
         self._compute_alphas()
         self.v_0 = None
         self._F_ = None
         self._W_ = None
 
@@ -85,103 +93,131 @@
         self._pre_power_flow_sam_sequential = None
         self._power_flow_sam_sequential = None
         self._power_flow_sam_sequential_constant_power_only = None
 
         self.is_numba_enabled = False
         self.is_gpu_enabled = False
 
-        if np.all(self.alpha_P) and not np.any(self.alpha_Z) and not np.any(self.alpha_I):
+        if (
+            np.all(self.alpha_P)
+            and not np.any(self.alpha_Z)
+            and not np.any(self.alpha_I)
+        ):
             # From ZIP model, only P is equal to one, the rest are zero.
             self.constant_power_only = True
             self.start_time_pre_pf_tensor_constant_power_only = perf_counter()
 
             # TODO: Change to sparse inverse.
+            # By reduced version I mean the cases that \alpha_s=1, meaning constant power
             # self._K_ = -np.linalg.inv(self.Ydd)  # Reduced version of -B^-1 (Reduced version of _F_)
-            self._K_ = np.array(-inv(self.Ydd_sparse).todense())  # Reduced version of -B^-1 (Reduced version of _F_)  TODO: check it exist .toarray()
+            self._K_ = np.array(
+                -inv(self.Ydd_sparse).todense()
+            )  # Reduced version of -B^-1 (Reduced version of _F_)  TODO: check it exist .toarray()
             self._L_ = self._K_ @ self.Yds  # Reduced version of _W_
             self.end_time_pre_pf_tensor_constant_power_only = perf_counter()
         else:
             self.constant_power_only = False
 
         if numba:
             self.enable_numba()
             self.is_numba_enabled = True
         else:
-            warnings.warn("Numba NOT enabled. Performance is greatly reduced.", RuntimeWarning)
+            warnings.warn(
+                "Numba NOT enabled. Performance is greatly reduced.", RuntimeWarning
+            )
             self.disable_numba()
             self.is_numba_enabled = False
 
         if gpu_mode:
             self.gpu_solver = GPUPowerFlow()
             self.is_gpu_enabled = True
 
-
-
-
     def enable_numba(self):
         parallel = True
         # TODO: If the base case is not solvable, the jit will take a lot to compile (For random generated graphs)
 
         # self._power_flow_sequential_constant_power = njit(power_flow_sequential_constant_power)
         # self._pre_power_flow_sequential = njit(pre_power_flow_sequential)
         # self._power_flow_sequential = njit(power_flow_sequential)
 
         # self._power_flow_tensor_constant_power = njit(power_flow_tensor_constant_power, parallel=parallel)  # When enablin the parallel parameter, the dimensions of the matrices change.
         self._power_flow_tensor_constant_power = power_flow_tensor_constant_power
         self._pre_power_flow_tensor = njit(pre_power_flow_tensor, parallel=parallel)
         self._power_flow_tensor = njit(power_flow_tensor, parallel=parallel)
 
-        self._pre_power_flow_sam_sequential = njit(pre_power_flow_sam_sequential, parallel=parallel)
-        self._power_flow_sam_sequential = njit(power_flow_sam_sequential, parallel=parallel)
-        self._power_flow_sam_sequential_constant_power_only = njit(power_flow_sam_sequential_constant_power_only,
-                                                                   parallel=parallel)
+        self._pre_power_flow_sam_sequential = njit(
+            pre_power_flow_sam_sequential, parallel=parallel
+        )
+        self._power_flow_sam_sequential = njit(
+            power_flow_sam_sequential, parallel=parallel
+        )
+        self._power_flow_sam_sequential_constant_power_only = njit(
+            power_flow_sam_sequential_constant_power_only, parallel=parallel
+        )
 
         self._compile_numba()
 
     def disable_numba(self):
         # self._power_flow_sequential_constant_power = power_flow_sequential_constant_power
         # self._pre_power_flow_sequential = pre_power_flow_sequential
         # self._power_flow_sequential = power_flow_sequential
 
         self._power_flow_tensor_constant_power = power_flow_tensor_constant_power
         self._pre_power_flow_tensor = pre_power_flow_tensor
         self._power_flow_tensor = power_flow_tensor
 
         self._pre_power_flow_sam_sequential = pre_power_flow_sam_sequential
         self._power_flow_sam_sequential = power_flow_sam_sequential
-        self._power_flow_sam_sequential_constant_power_only = power_flow_sam_sequential_constant_power_only
-
-
+        self._power_flow_sam_sequential_constant_power_only = (
+            power_flow_sam_sequential_constant_power_only
+        )
 
     @classmethod
-    def generate_from_graph(cls, *, nodes=100, child=2, plot_graph=True, load_factor=2, line_factor=3, **kwargs):
+    def generate_from_graph(
+        cls,
+        *,
+        nodes=100,
+        child=2,
+        plot_graph=True,
+        load_factor=2,
+        line_factor=3,
+        **kwargs
+    ):
         """
         Constructor of a synthetic grid using networkX package
         """
 
-        nodes_frame, lines_frame = generate_network(nodes=nodes,
-                                                    child=child,
-                                                    plot_graph=plot_graph,
-                                                    load_factor=load_factor,
-                                                    line_factor=line_factor)
-
-        return cls(node_file_path="",
-                   lines_file_path="",
-                   from_file=False,
-                   nodes_frame=nodes_frame,
-                   lines_frame=lines_frame,
-                   **kwargs)
+        nodes_frame, lines_frame = generate_network(
+            nodes=nodes,
+            child=child,
+            plot_graph=plot_graph,
+            load_factor=load_factor,
+            line_factor=line_factor,
+        )
+
+        return cls(
+            node_file_path="",
+            lines_file_path="",
+            from_file=False,
+            nodes_frame=nodes_frame,
+            lines_frame=lines_frame,
+            **kwargs
+        )
 
     def reset_start(self):
-        self.v_0 = np.ones((self.nb - 1, 1), dtype="complex128")  # Flat start  #2D array
+        self.v_0 = np.ones(
+            (self.nb - 1, 1), dtype="complex128"
+        )  # Flat start  #2D array
 
     def _set_number_of_threads(self, threads):
-        """ Set the number of threads that can be used by numba"""
+        """Set the number of threads that can be used by numba"""
         assert isinstance(threads, int)
-        assert threads <= psutil.cpu_count(), "Number of threads must be lower of cpu count."
+        assert (
+            threads <= psutil.cpu_count()
+        ), "Number of threads must be lower of cpu count."
         set_num_threads(threads)
         print(f"Number of threads set to: {threads}")
 
     def _make_y_bus(self) -> None:
         """
         Compute Y_bus submatrices
 
@@ -190,25 +226,29 @@
               |    | = |          | * |    |
               |-Id |   | Yds  Ydd |   | Vd |
         """
 
         self.nb = self.bus_info.shape[0]  # number of buses
         self.nl = self.branch_info.shape[0]  # number of lines
 
-        sl = self.bus_info[self.bus_info['Tb'] == 1]['NODES'].tolist()  # Slack node(s)
+        sl = self.bus_info[self.bus_info["Tb"] == 1]["NODES"].tolist()  # Slack node(s)
 
         stat = self.branch_info.iloc[:, 5]  # ones at in-service branches
-        Ys = stat / ((self.branch_info.iloc[:, 2] + 1j * self.branch_info.iloc[:, 3]) / (
-                    self.v_base ** 2 * 1000 / self.s_base))  # series admittance
-        Bc = stat * self.branch_info.iloc[:, 4] * (self.v_base ** 2 * 1000 / self.s_base)  # line charging susceptance
+        Ys = stat / (
+            (self.branch_info.iloc[:, 2] + 1j * self.branch_info.iloc[:, 3])
+            / (self.v_base**2 * 1000 / self.s_base)
+        )  # series admittance
+        Bc = (
+            stat * self.branch_info.iloc[:, 4] * (self.v_base**2 * 1000 / self.s_base)
+        )  # line charging susceptance
         tap = stat * self.branch_info.iloc[:, 6]  # default tap ratio = 1
 
         Ytt = Ys + 1j * Bc / 2
         Yff = Ytt / tap
-        Yft = - Ys / tap
+        Yft = -Ys / tap
         Ytf = Yft
 
         # build connection matrices
         f = self.branch_info.iloc[:, 0] - 1  # list of "from" buses
         t = self.branch_info.iloc[:, 1] - 1  # list of "to" buses
 
         # connection matrix for line & from buses
@@ -226,29 +266,43 @@
 
         # build Ybus
         Ybus = Cf.T * Yf + Ct.T * Yt  # Full Ybus
 
         # Dense matrices
         # TODO: This takes a lot of memory. Check if I can save it always as sparse for all methods.
         self._Ybus = Ybus.toarray()
-        self.Yss = csr_matrix(Ybus[sl[0] - 1, sl[0] - 1], shape=(len(sl), len(sl))).toarray()
-        self.Ysd = np.array(Ybus[0, 1:].toarray())  # TODO: Here assume the slack is the first one?
+        self.Yss = csr_matrix(
+            Ybus[sl[0] - 1, sl[0] - 1], shape=(len(sl), len(sl))
+        ).toarray()
+        self.Ysd = np.array(
+            Ybus[0, 1:].toarray()
+        )  # TODO: Here assume the slack is the first one?
         self.Yds = self.Ysd.T
-        self.Ydd = np.array(Ybus[1:, 1:].toarray())  # TODO: This consumes a huge amount of memory
+        self.Ydd = np.array(
+            Ybus[1:, 1:].toarray()
+        )  # TODO: This consumes a huge amount of memory
 
         self._Ybus_sparse = Ybus
-        self.Yss_sparse = csr_matrix(Ybus[sl[0] - 1, sl[0] - 1], shape=(len(sl), len(sl)))
+        self.Yss_sparse = csr_matrix(
+            Ybus[sl[0] - 1, sl[0] - 1], shape=(len(sl), len(sl))
+        )
         self.Ysd_sparse = Ybus[0, 1:]  # TODO: Here assume the slack is the first one?
         self.Yds_sparse = csc_matrix(self.Ysd.T)
         self.Ydd_sparse = Ybus[1:, 1:]
 
     def _compute_alphas(self):
-        self.alpha_P = self.bus_info[self.bus_info.Tb != 1].Pct.values.reshape(-1, )
-        self.alpha_I = self.bus_info[self.bus_info.Tb != 1].Ict.values.reshape(-1, )
-        self.alpha_Z = self.bus_info[self.bus_info.Tb != 1].Zct.values.reshape(-1, )
+        self.alpha_P = self.bus_info[self.bus_info.Tb != 1].Pct.values.reshape(
+            -1,
+        )
+        self.alpha_I = self.bus_info[self.bus_info.Tb != 1].Ict.values.reshape(
+            -1,
+        )
+        self.alpha_Z = self.bus_info[self.bus_info.Tb != 1].Zct.values.reshape(
+            -1,
+        )
 
         self.flag_all_constant_impedance_is_zero = not np.any(self.alpha_Z)
         self.flag_all_constant_current_is_zero = not np.any(self.alpha_I)
         self.flag_all_constant_powers_are_ones = np.all(self.alpha_P)
 
     def _compile_numba(self):
         # Compile JIT code running the base case PF at least once
@@ -259,37 +313,46 @@
     def _check_2d_to_1d(self, active_power, reactive_power):
         """
         Checks if the 2D matrix has only one row. In that case, constructs a 1D vector.
         Checks that active and reactive power matrices has the same dimensions and shapes.
         This is a helper method for the sequential algorithms that uses the tensor method (check run_pf method).
         """
 
-        assert active_power.ndim == reactive_power.ndim, "Active and reactive power must have same dimension."
-
-        if (active_power.ndim == 2 and active_power.shape[0] == 1) and \
-                (reactive_power.ndim == 2 and reactive_power.shape[0] == 1):
+        assert (
+            active_power.ndim == reactive_power.ndim
+        ), "Active and reactive power must have same dimension."
+
+        if (active_power.ndim == 2 and active_power.shape[0] == 1) and (
+            reactive_power.ndim == 2 and reactive_power.shape[0] == 1
+        ):
             active_power = active_power.flatten()
             reactive_power = reactive_power.flatten()
-        elif (active_power.ndim == 2 and active_power.shape[0] != 1) and \
-                (reactive_power.ndim == 2 and reactive_power.shape[0] != 1):
-            raise ValueError("Active and reactive power tensors must have only one time step.")
+        elif (active_power.ndim == 2 and active_power.shape[0] != 1) and (
+            reactive_power.ndim == 2 and reactive_power.shape[0] != 1
+        ):
+            raise ValueError(
+                "Active and reactive power tensors must have only one time step."
+            )
 
         assert active_power.ndim == 1, "Array should be one dimensional."
         assert reactive_power.ndim == 1, "Array should be one dimensional."
-        assert len(active_power) == len(reactive_power) == self.nb - 1, "All load nodes must have power values."
+        assert (
+            len(active_power) == len(reactive_power) == self.nb - 1
+        ), "All load nodes must have power values."
 
         return active_power, reactive_power
 
     def _compute_chunks(self, DIMENSION_BOUND, n_nodes, n_steps):
         """
-        Breaks the n_steps in chunks so it can fit in memory.
-        The ideas is that n_nodes * n_steps cannot be bigger than DIMENSION_BOUND
-        DIMENSION_BOUND is a empirically found value (should vary due to the computer's RAM).
+        Breaks the n_steps in chunks, so it can fit in memory.
+        The ideas are that n_nodes * n_steps cannot be bigger than DIMENSION_BOUND
+        DIMENSION_BOUND is an empirically found value (should vary due to the computer's RAM).
 
         Return:
+        ------
             idx: list: All the ts indices to slice the power consumption array.
                 e.g., idx = [0, 1000, 2000, 2500]. 2500 time step requested, chunked in 1000 time steps (last item is
                 the reminder: 2500-2000=500).
         """
 
         # DIMENSION_BOUND =  500 * 5_000
         # n_nodes = 4999
@@ -342,16 +405,20 @@
         # Placeholder for H-vector
         idx_row_H_temp = []
         H_data_temp = []
         if n_steps > 1:
             times_multiplying = []
             for ii in range(1, n_steps):
                 start_multiply = perf_counter()
-                M_temp = -diags(1 / np.conj(S_nom[ii, :])).dot(Ydd_sparse).asformat("coo")
-                H_temp = diags(1 / np.conj(S_nom[ii, :])).dot(Yds_sparse).asformat("coo")
+                M_temp = (
+                    -diags(1 / np.conj(S_nom[ii, :])).dot(Ydd_sparse).asformat("coo")
+                )
+                H_temp = (
+                    diags(1 / np.conj(S_nom[ii, :])).dot(Yds_sparse).asformat("coo")
+                )
 
                 idx_col_M_temp.append(M_temp.col + ii * n_nodes)
                 idx_row_M_temp.append(M_temp.row + ii * n_nodes)
                 M_data_temp.append(M_temp.data)
 
                 idx_row_H_temp.append(H_temp.row + ii * n_nodes)
                 H_data_temp.append(H_temp.data)
@@ -363,49 +430,56 @@
             M_big_idx_data = np.hstack([M_1_data, np.hstack(M_data_temp)])
 
             H_big_idx_row = np.hstack([idx_1_H_row, np.hstack(idx_row_H_temp)])
             H_big_idx_col = np.zeros(H_big_idx_row.shape[0], dtype=np.int32)
             H_big_data = np.hstack([H_1_data, np.hstack(H_data_temp)])
 
             M_big = csr_matrix((M_big_idx_data, (M_big_idx_row, M_big_idx_col)))
-            H_big = csr_matrix((H_big_data, (H_big_idx_row, H_big_idx_col)), shape=(n_steps * n_nodes, 1))
+            H_big = csr_matrix(
+                (H_big_data, (H_big_idx_row, H_big_idx_col)),
+                shape=(n_steps * n_nodes, 1),
+            )
 
         else:
             M_big = M
             H_big = H
 
         return M_big, H_big
 
     def reshape_tensor(sefl, tensor_array):
         original_shape = tensor_array.shape
         tau = np.prod(original_shape[:-1])
-        tensor_array.shape = (tau, original_shape[-1])   # This reshapes in place (No new memory use)
+        tensor_array.shape = (
+            tau,
+            original_shape[-1],
+        )  # This reshapes in place (No new memory use)
 
         return tensor_array, original_shape
 
-    def run_pf(self,
-               active_power: np.ndarray = None,
-               reactive_power: np.ndarray = None,
-               flat_start: bool = True,
-               start_value: np.ndarray = None,
-               tolerance: float = 1e-6,
-               algorithm: str = "tensor",
-               sparse_solver: str = "scipy"):
-
+    def run_pf(
+        self,
+        active_power: np.ndarray = None,
+        reactive_power: np.ndarray = None,
+        flat_start: bool = True,
+        start_value: np.ndarray = None,
+        tolerance: float = 1e-6,
+        algorithm: str = "tensor",
+        sparse_solver: str = "scipy",
+    ):
         """
         Computes the power flow on the grid for the active and reactive power matrices/tensor.
 
         Parameters:
         -----------
             active_power: np.ndarray: Real array/tensor type np.float64. The dimension of the tensor should be
                             of the form (a x b x ... x m), where m is the number of buses minus the slack bus.
                             e.g., m = nbus - 1. The values of the array are in kilo-Watt [kW].
-            reactive_power: np.ndarray: The array/tensor has the same characteristics than the active_power parameter.
-            flat_start: bool: Flag to indicate if ta flat start should be use. This is currently the default. All
-                            values of voltage starts at (1.0 + j0.0) p.u.
+            reactive_power: np.ndarray: The array/tensor has the same characteristics as the active_power parameter.
+            flat_start: bool: Flag to indicate if the flat start should be used. This is currently the default. All
+                            values of voltage start at (1.0 + j0.0) p.u.
             start_value: np.ndarray: Array/Tensor with the same dimension os active_power parameter. It indicates the
                             warm start voltage values for the iterative algorithm. This array is in complex number
                             of type np.complex128.
             algorithm: str: Algorithm to be used for the power flow. The options are:
                             "hp-tensor":  Tensor-sparse power flow. The sparse solver is defined by the "sparse_solver"
                                         parameter.
                             "tensor":  Tensor-dense power flow.
@@ -436,90 +510,103 @@
                         "time_pf_log": NOT USED.
                         "convergence_log": NOT USED.
                         }
         """
 
         is_tensor = False
         if active_power is not None and reactive_power is not None:
-            assert active_power.shape == reactive_power.shape, "Active and reactive power arrays must have the " \
-                                                               "same shape."
+            assert active_power.shape == reactive_power.shape, (
+                "Active and reactive power arrays must have the " "same shape."
+            )
             original_shape = active_power.shape
 
             if active_power.ndim > 2:  # Reshape form N-D to 2-D:
                 active_power, original_shape = self.reshape_tensor(active_power)
                 reactive_power, _ = self.reshape_tensor(reactive_power)
                 is_tensor = True
 
-
         kwargs = dict()
         if algorithm == "hp":  # Same as hp-tensor but receive 1-D vectors
             pf_algorithm = self.run_pf_tensor_hp_laurent
             kwargs.update(solver=sparse_solver)
         elif algorithm == "sam":
             pf_algorithm = self.run_pf_sam_sequential
         elif algorithm == "sequential":  # Same as tensor but receive 1-D vectors
             pf_algorithm = self.run_pf_tensor
         elif algorithm == "tensor":
             pf_algorithm = self.run_pf_tensor
         elif algorithm == "hp-tensor":
             pf_algorithm = self.run_pf_tensor_hp_laurent
+            kwargs.update(solver=sparse_solver)
         elif algorithm == "gpu-tensor":
             pf_algorithm = self.run_pf_tensor
             kwargs.update(compute="gpu")
         else:
             raise ValueError("Incorrect power flow algorithm selected")
 
-        solutions = pf_algorithm(active_power=active_power,  # 2-D Array
-                                 reactive_power=reactive_power,  # 2-D Array
-                                 flat_start=flat_start,
-                                 start_value=start_value,
-                                 tolerance=tolerance,
-                                 **kwargs)
+        solutions = pf_algorithm(
+            active_power=active_power,  # 2-D Array
+            reactive_power=reactive_power,  # 2-D Array
+            flat_start=flat_start,
+            start_value=start_value,
+            tolerance=tolerance,
+            **kwargs
+        )
 
         if is_tensor:  # Solutions from a 2-D array to an N-D array.
             solutions["v"].shape = original_shape
             active_power.shape = original_shape
             reactive_power.shape = original_shape
 
         return solutions
 
-    def run_pf_tensor(self,
-                      active_power: np.ndarray = None,
-                      reactive_power: np.ndarray = None,
-                      *,
-                      start_value=None,
-                      iterations: int = 100,
-                      tolerance: float = 1e-6,
-                      flat_start: bool = True,
-                      compute: str = "cpu") -> dict:
+    def run_pf_tensor(
+        self,
+        active_power: np.ndarray = None,
+        reactive_power: np.ndarray = None,
+        *,
+        start_value=None,
+        iterations: int = 100,
+        tolerance: float = 1e-6,
+        flat_start: bool = True,
+        compute: str = "cpu"
+    ) -> dict:
         """Run power flow for an array of active and reactive power consumption"""
 
         if (active_power is not None) and (reactive_power is not None):
             assert len(active_power.shape) == 2, "Array must be two dimensional."
             assert len(reactive_power.shape) == 2, "Array must be two dimensional."
-            assert active_power.shape[1] == reactive_power.shape[1] == self.nb - 1, "All nodes must have power values."
+            assert (
+                active_power.shape[1] == reactive_power.shape[1] == self.nb - 1
+            ), "All nodes must have power values."
             # rows are time steps, columns are nodes
         else:
             active_power = self.P_file[np.newaxis, :]
             reactive_power = self.Q_file[np.newaxis, :]
 
         self.ts_n = active_power.shape[0]  # Time steps to be simulated
         if flat_start:
-            self.v_0 = np.ones((self.ts_n, self.nb - 1)) + 1j * np.zeros((self.ts_n, self.nb - 1))  # Flat start
+            self.v_0 = np.ones((self.ts_n, self.nb - 1)) + 1j * np.zeros(
+                (self.ts_n, self.nb - 1)
+            )  # Flat start
 
         v0_solutions = []
         total_time_pre_pf_all = []
         total_time_pf_all = []
         total_time_algorithm_all = []
         iterations_all = []
         flag_convergence_all = []
         flag_convergence_bool_all = True
 
-        active_power_pu = active_power / self.s_base  # Vector with all active power except slack
-        reactive_power_pu = reactive_power / self.s_base  # Vector with all reactive power except slack
+        active_power_pu = (
+            active_power / self.s_base
+        )  # Vector with all active power except slack
+        reactive_power_pu = (
+            reactive_power / self.s_base
+        )  # Vector with all reactive power except slack
         S_nom = active_power_pu + 1j * reactive_power_pu  # (ts x nodes)
 
         n_steps = S_nom.shape[0]
         n_nodes = S_nom.shape[1]
 
         # if n_nodes >= 1000:
         #     warnings.warn(f"The size of the system is >= 1_000 nodes. Consider using a sparse algorithm.")
@@ -531,74 +618,85 @@
             warnings.warn("GPU library not found, falling back to CPU.")
             self._power_flow_tensor_solver = self._power_flow_tensor_constant_power
         elif compute == "gpu" and self.is_gpu_enabled is True:
             # print("GPU Solver selected")
             self._power_flow_tensor_solver = self.gpu_solver.power_flow_gpu
 
         if compute == "cpu":
-            DIMENSION_BOUND = 500 * 100_000  # 5_000 x 10_000 did work. Empirical value for my machine
+            DIMENSION_BOUND = (
+                500 * 100_000
+            )  # 5_000 x 10_000 did work. Empirical value for my machine
         else:
-            DIMENSION_BOUND = 500 * 125_000  # 5_000 x 15_000 did work. Empirical value for my machine
+            DIMENSION_BOUND = (
+                500 * 125_000
+            )  # 5_000 x 15_000 did work. Empirical value for my machine
 
         # DIMENSION_BOUND = 100_000 * 100_000  # 5_000 x 10_000 did work. Empirical value for my machine
         # MEMORY_BOUND = 200 * 500_000  # TODO: Even if I chunk everything, saving v0 requires extra memory.
 
         idx = self._compute_chunks(DIMENSION_BOUND, n_nodes=n_nodes, n_steps=n_steps)
         n_chunks = len(idx) - 1
         # print(f"Number of chunks: {n_chunks}")
 
-        t = trange(n_chunks, desc='Chunk', leave=False)
+        t = trange(n_chunks, desc="Chunk", leave=False)
         for ii in t:
             t.set_description(f"Chunk: {ii + 1} of {n_chunks}", refresh=True)
 
             ts_chunk = idx[ii + 1] - idx[ii]  # Size of the chunk
-            self.v_0 = np.ones((ts_chunk, self.nb - 1)) + 1j * np.zeros((ts_chunk, self.nb - 1))  # Flat start
-            S_chunk = S_nom[idx[ii]:idx[ii + 1]]
-
+            self.v_0 = np.ones((ts_chunk, self.nb - 1)) + 1j * np.zeros(
+                (ts_chunk, self.nb - 1)
+            )  # Flat start
+            S_chunk = S_nom[idx[ii] : idx[ii + 1]]
 
             if self.constant_power_only:
                 start_time_pre_pf = self.start_time_pre_pf_tensor_constant_power_only
                 # No pre-computing (Already done when creating the object)
                 end_time_pre_pf = self.end_time_pre_pf_tensor_constant_power_only
 
                 start_time_pf = perf_counter()
-                self.v_0, t_iterations = self._power_flow_tensor_solver(K=self._K_,
-                                                                        L=self._L_,
-                                                                        S=S_chunk,
-                                                                        v0=self.v_0,
-                                                                        ts=ts_chunk,
-                                                                        nb=self.nb,
-                                                                        iterations=iterations,
-                                                                        tolerance=tolerance)
+                self.v_0, t_iterations = self._power_flow_tensor_solver(
+                    K=self._K_,
+                    L=self._L_,
+                    S=S_chunk,
+                    v0=self.v_0,
+                    ts=ts_chunk,
+                    nb=self.nb,
+                    iterations=iterations,
+                    tolerance=tolerance,
+                )
                 end_time_pf = perf_counter()
 
             else:
                 # raise ValueError("This should not be running")
                 start_time_pre_pf = perf_counter()
-                self._F_, self._W_ = self._pre_power_flow_tensor(flag_all_constant_impedance_is_zero=self.flag_all_constant_impedance_is_zero,
-                                                                 flag_all_constant_current_is_zero=self.flag_all_constant_current_is_zero,
-                                                                 flag_all_constant_powers_are_ones=self.flag_all_constant_powers_are_ones,
-                                                                 ts_n=ts_chunk,
-                                                                 nb=self.nb,
-                                                                 S_nom=S_chunk,
-                                                                 alpha_Z=self.alpha_Z,
-                                                                 alpha_I=self.alpha_I,
-                                                                 alpha_P=self.alpha_P,
-                                                                 Yds=self.Yds,
-                                                                 Ydd=self.Ydd)
+                self._F_, self._W_ = self._pre_power_flow_tensor(
+                    flag_all_constant_impedance_is_zero=self.flag_all_constant_impedance_is_zero,
+                    flag_all_constant_current_is_zero=self.flag_all_constant_current_is_zero,
+                    flag_all_constant_powers_are_ones=self.flag_all_constant_powers_are_ones,
+                    ts_n=ts_chunk,
+                    nb=self.nb,
+                    S_nom=S_chunk,
+                    alpha_Z=self.alpha_Z,
+                    alpha_I=self.alpha_I,
+                    alpha_P=self.alpha_P,
+                    Yds=self.Yds,
+                    Ydd=self.Ydd,
+                )
                 end_time_pre_pf = perf_counter()
 
                 start_time_pf = perf_counter()
-                self.v_0, t_iterations = self._power_flow_tensor(_F_=self._F_,
-                                                                 _W_=self._W_,
-                                                                 v_0=self.v_0,
-                                                                 ts_n=ts_chunk,
-                                                                 nb=self.nb,
-                                                                 iterations=iterations,
-                                                                 tolerance=tolerance)
+                self.v_0, t_iterations = self._power_flow_tensor(
+                    _F_=self._F_,
+                    _W_=self._W_,
+                    v_0=self.v_0,
+                    ts_n=ts_chunk,
+                    nb=self.nb,
+                    iterations=iterations,
+                    tolerance=tolerance,
+                )
                 end_time_pf = perf_counter()
 
             if t_iterations == iterations:
                 flag_convergence = False
                 warnings.warn("Power flow did not converge.")
             else:
                 flag_convergence = True
@@ -614,170 +712,201 @@
             flag_convergence_all.append(flag_convergence)
             flag_convergence_bool_all = flag_convergence_bool_all & flag_convergence
 
             v0_solutions.append(self.v_0.copy())
 
         self.v_0 = np.vstack(v0_solutions)
 
-        solution = {"v": self.v_0,  # 2D-Vector. Solution of voltage in complex numbers
-                    "time_pre_pf": sum(total_time_pre_pf_all),
-                    "time_pf":  sum(total_time_pf_all),
-                    "time_algorithm":  sum(total_time_algorithm_all),
-                    "iterations": np.floor(np.mean(iterations_all)),
-
-                    "convergence": flag_convergence_bool_all,
-                    "iterations_log": iterations_all,
-                    "time_pre_pf_log": total_time_pre_pf_all,
-                    "time_pf_log": total_time_pf_all,
-                    "convergence_log": flag_convergence_all
-                    }
+        solution = {
+            "v": self.v_0,  # 2D-Vector. Solution of voltage in complex numbers
+            "time_pre_pf": sum(total_time_pre_pf_all),
+            "time_pf": sum(total_time_pf_all),
+            "time_algorithm": sum(total_time_algorithm_all),
+            "iterations": np.floor(np.mean(iterations_all)),
+            "convergence": flag_convergence_bool_all,
+            "iterations_log": iterations_all,
+            "time_pre_pf_log": total_time_pre_pf_all,
+            "time_pf_log": total_time_pf_all,
+            "convergence_log": flag_convergence_all,
+        }
 
         return solution
 
-
-    def run_pf_sam_sequential(self,
-                              active_power: np.ndarray = None,
-                              reactive_power: np.ndarray = None,
-                              flat_start: bool = True,
-                              start_value: np.array = None):
-
-        """
+    def run_pf_sam_sequential(
+        self,
+        active_power: np.ndarray = None,
+        reactive_power: np.ndarray = None,
+        flat_start: bool = True,
+        start_value: np.array = None,
+        tolerance: float = 1e-6,
+    ):
+        r"""
         Single time step power flow with numba performance increase.
         This is the implementation of [1], algorithm called SAM (Successive Approximation Method)
 
         V[k+1] = B^{-1} ( A[k] @ V[k]^{*}  - C - D[k])
 
         Where:
         A[k] = np.diag(\alpha_p \odot V[k]^{* -2} * S_n^{*}), \odot == Hadamard product, * == complex conjugate
         B = np.diag(\alpha_z \odot S_n^{*}) + Y_dd
         C = Y_ds @ V_s + \alpha_i \odot S_n^{*}
         D[k] = 2 \alpha_p \odot V[k]^{* -1} \odot S_n^{*}
 
         Please note that for constant power only. i.e., \alpha_p = 1, \alpha_i = 0, \alpha_z = 0.
-        The matrices reduces to:
+        The matrices reduce to:
 
         A[k] = np.diag(V[k]^{* -2} * S_n^{*}), \odot == Hadamard product, * == complex conjugate
         B = Y_dd
         C = Y_ds @ V_s
         D[k] = 2 V[k]^{* -1} \odot S_n^{*}
 
         [1] Juan S. Giraldo, Oscar Danilo Montoya, Pedro P. Vergara, Federico Milano, "A fixed-point current injection
             power flow for electric distribution systems using Laurent series", Electric Power Systems Research,
             Volume 211, 2022. https://doi.org/10.1016/j.epsr.2022.108326.
 
         """
 
         if (active_power is not None) and (reactive_power is not None):
-            active_power, reactive_power = self._check_2d_to_1d(active_power, reactive_power)
+            active_power, reactive_power = self._check_2d_to_1d(
+                active_power, reactive_power
+            )
         else:  # Default case
             active_power = self.P_file
             reactive_power = self.Q_file
 
         if flat_start:
             # self.v_0 = np.ones((self.nb - 1, 1), dtype="complex128")  # 2D-Vector
             self.v_0 = np.ones(self.nb - 1, dtype="complex128")  # 2D-Vector
         elif start_value is not None:
             # TODO: Check the dimensions of the flat start
             self.v_0 = start_value  # User's start value
 
-        active_power_pu = active_power / self.s_base  # Vector with all active power except slack
-        reactive_power_pu = reactive_power / self.s_base  # Vector with all reactive power except slack
-        S_nom = (active_power_pu + 1j * reactive_power_pu).reshape(-1, )
-
+        active_power_pu = (
+            active_power / self.s_base
+        )  # Vector with all active power except slack
+        reactive_power_pu = (
+            reactive_power / self.s_base
+        )  # Vector with all reactive power except slack
+        S_nom = (active_power_pu + 1j * reactive_power_pu).reshape(
+            -1,
+        )
 
         if self.constant_power_only:
             start_time_pre_pf = perf_counter()
             # No precomputing, the minimum matrix multiplication is done in the initialization of the object.
             end_time_pre_pf = perf_counter()
 
             start_time_pf = perf_counter()
-            V, iteration = self._power_flow_sam_sequential_constant_power_only(B_inv=-self._K_,
-                                                                               C=self.Yds.flatten(),
-                                                                               v_0=self.v_0,
-                                                                               s_n=S_nom,
-                                                                               iterations=self.iterations,
-                                                                               tolerance=self.tolerance)
+            V, iteration = self._power_flow_sam_sequential_constant_power_only(
+                B_inv=-self._K_,
+                C=self.Yds.flatten(),
+                v_0=self.v_0,
+                s_n=S_nom,
+                iterations=self.iterations,
+                tolerance=self.tolerance,
+            )
             end_time_pf = perf_counter()
 
         else:
             start_time_pre_pf = perf_counter()
-            B_inv, C, S_nom = self._pre_power_flow_sam_sequential(active_power,  # TODO: Change the input to S_nom
-                                                                  reactive_power,
-                                                                  s_base=self.s_base,
-                                                                  alpha_Z=self.alpha_Z,
-                                                                  alpha_I=self.alpha_I,
-                                                                  Yds=self.Yds,
-                                                                  Ydd=self.Ydd,
-                                                                  nb=self.nb)
+            B_inv, C, S_nom = self._pre_power_flow_sam_sequential(
+                active_power,  # TODO: Change the input to S_nom
+                reactive_power,
+                s_base=self.s_base,
+                alpha_Z=self.alpha_Z,
+                alpha_I=self.alpha_I,
+                Yds=self.Yds,
+                Ydd=self.Ydd,
+                nb=self.nb,
+            )
             end_time_pre_pf = perf_counter()
 
             start_time_pf = perf_counter()
-            V, iteration = self._power_flow_sam_sequential(B_inv,
-                                                           C,
-                                                           v_0=self.v_0,
-                                                           s_n=S_nom,
-                                                           alpha_P=self.alpha_P,
-                                                           iterations=self.iterations,
-                                                           tolerance=self.tolerance)
+            V, iteration = self._power_flow_sam_sequential(
+                B_inv,
+                C,
+                v_0=self.v_0,
+                s_n=S_nom,
+                alpha_P=self.alpha_P,
+                iterations=self.iterations,
+                tolerance=self.tolerance,
+            )
             end_time_pf = perf_counter()
 
         if iteration == self.iterations:
             flag_convergence = False
         else:
             flag_convergence = True
 
         total_time_pre_pf = end_time_pre_pf - start_time_pre_pf
         total_time_pf = end_time_pf - start_time_pf
         total_time_algorithm = total_time_pre_pf + total_time_pf
 
-        solution = {"v": V.flatten(),  # 1D-Vector. Solution of voltage in complex numbers
-                    "time_pre_pf": total_time_pre_pf,
-                    "time_pf": total_time_pf,
-                    "time_algorithm": total_time_algorithm,
-                    "iterations": iteration,
-                    "convergence": flag_convergence,}
+        solution = {
+            "v": V.flatten(),  # 1D-Vector. Solution of voltage in complex numbers
+            "time_pre_pf": total_time_pre_pf,
+            "time_pf": total_time_pf,
+            "time_algorithm": total_time_algorithm,
+            "iterations": iteration,
+            "convergence": flag_convergence,
+        }
 
         return solution
 
-    def run_pf_sam_sequential_juan(self,
-                                   active_power: np.ndarray = None,
-                                   reactive_power: np.ndarray = None,
-                                   flat_start: bool = True,
-                                   start_value: np.array = None):
+    def run_pf_sam_sequential_juan(
+        self,
+        active_power: np.ndarray = None,
+        reactive_power: np.ndarray = None,
+        flat_start: bool = True,
+        start_value: np.array = None,
+    ):
         """This function is just for reference. Not used anywhere"""
 
         if (active_power is not None) and (reactive_power is not None):
-            active_power, reactive_power = self._check_2d_to_1d(active_power, reactive_power)
+            active_power, reactive_power = self._check_2d_to_1d(
+                active_power, reactive_power
+            )
         else:
             active_power = self.P_file
             reactive_power = self.Q_file
 
         if flat_start:
             self.v_0 = np.ones((self.nb - 1, 1), dtype="complex128")  # 2D-Vector
         elif start_value is not None:
             # TODO: Check the dimensions of the flat start
             self.v_0 = start_value  # User's start value
 
-        active_power_pu = active_power / self.s_base  # Vector with all active power except slack
-        reactive_power_pu = reactive_power / self.s_base  # Vector with all reactive power except slack
+        active_power_pu = (
+            active_power / self.s_base
+        )  # Vector with all active power except slack
+        reactive_power_pu = (
+            reactive_power / self.s_base
+        )  # Vector with all reactive power except slack
         S_nom = active_power_pu + 1j * reactive_power_pu  # (ts x nodes)
 
         start_time_pre_pf = perf_counter()
         B = np.diag(np.multiply(self.alpha_Z, np.conj(S_nom))) + self.Ydd  # Constant
         B_inv = np.linalg.inv(B)
-        C = self.Yds + (np.multiply(self.alpha_I, np.conj(S_nom))).reshape(self.nb - 1, 1)  # Constant
+        C = self.Yds + (np.multiply(self.alpha_I, np.conj(S_nom))).reshape(
+            self.nb - 1, 1
+        )  # Constant
         end_time_pre_pf = perf_counter()
 
         start_time_pf = perf_counter()
         iteration = 0
         tol = np.inf
         while (iteration < self.iterations) & (tol >= self.tolerance):
 
-            A = np.diag(np.multiply(self.alpha_P, 1. / np.conj(self.v_0.ravel()) ** (2)) * np.conj(S_nom))  # Needs update
-            D = np.multiply(np.multiply(2, self.alpha_P), 1. / np.conj(self.v_0.ravel())) * np.conj(S_nom)
+            A = np.diag(
+                np.multiply(self.alpha_P, 1.0 / np.conj(self.v_0.ravel()) ** (2))
+                * np.conj(S_nom)
+            )  # Needs update
+            D = np.multiply(
+                np.multiply(2, self.alpha_P), 1.0 / np.conj(self.v_0.ravel())
+            ) * np.conj(S_nom)
             D = D.reshape(-1, 1)  # Needs update
 
             V = B_inv @ (A @ np.conj(self.v_0) - C - D)
 
             tol = np.max(np.abs(np.abs(V) - np.abs(self.v_0)))
             self.v_0 = V  # Voltage at load buses
             iteration += 1
@@ -788,80 +917,112 @@
         total_time_algorithm = total_time_pre_pf + total_time_pf
 
         if iteration == self.iterations:
             flag_convergence = False
         else:
             flag_convergence = True
 
-        solution = {"v": self.v_0.flatten(),  # 1D-Vector. Solution of voltage in complex numbers
-                    "time_pre_pf": total_time_pre_pf,
-                    "time_pf": total_time_pf,
-                    "time_algorithm": total_time_algorithm,
-                    "iterations": iteration,
-                    "convergence": flag_convergence}
+        solution = {
+            "v": self.v_0.flatten(),  # 1D-Vector. Solution of voltage in complex numbers
+            "time_pre_pf": total_time_pre_pf,
+            "time_pf": total_time_pf,
+            "time_algorithm": total_time_algorithm,
+            "iterations": iteration,
+            "convergence": flag_convergence,
+        }
 
         return solution
 
-
-    def run_pf_tensor_hp_laurent(self,
-                                 active_power: np.ndarray = None,
-                                 reactive_power: np.ndarray = None,
-                                 *,
-                                 start_value=None,
-                                 iterations: int = 100,
-                                 tolerance: float = 1e-6,
-                                 flat_start: bool = True,
-                                 solver="pardiso"):
-
+    def run_pf_tensor_hp_laurent(
+        self,
+        active_power: np.ndarray = None,
+        reactive_power: np.ndarray = None,
+        *,
+        start_value=None,
+        iterations: int = 100,
+        tolerance: float = 1e-6,
+        flat_start: bool = True,
+        solver="scipy"
+    ):
+        # This is the sparse version of the algorithm
 
         if (active_power is not None) and (reactive_power is not None):
             assert active_power.ndim == 2, "Array should be two dimensional."
             assert reactive_power.ndim == 2, "Array should be two dimensional."
-            assert active_power.shape[1] == reactive_power.shape[1] == self.nb - 1, "All load nodes must have power" \
-            # rows are time steps, columns are nodes
+            assert (
+                active_power.shape[1] == reactive_power.shape[1] == self.nb - 1
+            ), "All load nodes must have power"  # rows are time steps, columns are nodes
         else:
             active_power = self.P_file[np.newaxis, :]
             reactive_power = self.Q_file[np.newaxis, :]
 
+        if solver == "pardiso":
+            # Check if MKL solver is available
+            try:
+                from tensorpowerflow.pyMKL import pardisoSolver
+
+                PARDISO_SOLVER_AVAILABLE = True
+            except:
+                PARDISO_SOLVER_AVAILABLE = False
+                warnings.warn(
+                    "Pardiso solver not found for sparse power flow. Install it with `pip install mkl`. "
+                    "Rolling back to scipy solver."
+                )
+
         v0_solutions = []
         total_time_pre_pf_all = []
         total_time_pf_all = []
         total_time_algorithm_all = []
         iterations_all = []
         flag_convergence_all = []
         flag_convergence_bool_all = True
 
-        active_power_pu = active_power / self.s_base  # Vector with all active power except slack
-        reactive_power_pu = reactive_power / self.s_base  # Vector with all reactive power except slack
-        S_nom = (active_power_pu + 1j * reactive_power_pu) + (1e-10 + 1j * 1e-10)  # (ts x nodes)
+        active_power_pu = (
+            active_power / self.s_base
+        )  # Vector with all active power except slack
+        reactive_power_pu = (
+            reactive_power / self.s_base
+        )  # Vector with all reactive power except slack
+        S_nom = (active_power_pu + 1j * reactive_power_pu) + (
+            1e-10 + 1j * 1e-10
+        )  # (ts x nodes)
 
         n_steps = S_nom.shape[0]
         n_nodes = S_nom.shape[1]
 
-        DIMENSION_BOUND = 500 * 5_000  # The Ax=b sparse problem can not have a matrix A with more than 5M x 5M.
+        DIMENSION_BOUND = (
+            500 * 5_000
+        )  # The Ax=b sparse problem can not have a matrix A with more than 5M x 5M.
         # TODO: This method can be replace by np.array_split() ???
         # Check: https://people.duke.edu/~ccc14/sta-663-2016/19B_Threads_Processses_Concurrency.html
 
         idx = self._compute_chunks(DIMENSION_BOUND, n_nodes=n_nodes, n_steps=n_steps)
         n_chunks = len(idx) - 1
 
-        t = trange(n_chunks, desc='Chunk', leave=False)
+        t = trange(n_chunks, desc="Chunk", leave=False)
         for ii in t:
             t.set_description(f"Chunk: {ii + 1} of {n_chunks}", refresh=True)
             ts_chunk = idx[ii + 1] - idx[ii]  # Size of the chunk
 
-            self.v_0 = np.ones((ts_chunk * (self.nb - 1), 1)) + 1j * np.zeros((ts_chunk * (self.nb - 1), 1))  # Flat start
+            self.v_0 = np.ones((ts_chunk * (self.nb - 1), 1)) + 1j * np.zeros(
+                (ts_chunk * (self.nb - 1), 1)
+            )  # Flat start
 
             start_time_pre_pf = perf_counter()
-            M, H = self._make_big_sparse_matrices(S_nom[ idx[ii]:idx[ii + 1] ], self.Ydd_sparse, self.Yds_sparse)
+            M, H = self._make_big_sparse_matrices(
+                S_nom[idx[ii] : idx[ii + 1]], self.Ydd_sparse, self.Yds_sparse
+            )
 
-            if solver == "pardiso":  # TODO: Add the flag to see if pardiso is in the system
-                pSolve = pardisoSolver(M, mtype=13)  # Prepare to solve Mx = b
-                pSolve.run_pardiso(12)  # Factorize matrix M.
-                sparse_solver = pSolve.solve_pardiso
+            if solver == "pardiso":
+                if PARDISO_SOLVER_AVAILABLE:
+                    pSolve = pardisoSolver(M, mtype=13)  # Prepare to solve Mx = b
+                    pSolve.run_pardiso(12)  # Factorize matrix M.
+                    sparse_solver = pSolve.solve_pardiso
+                else:
+                    sparse_solver = spsolve
             elif solver == "scipy":
                 sparse_solver = spsolve
             else:
                 raise ValueError("Incorrect sparse solver selected")
             end_time_pre_pf = perf_counter()
 
             start_time_pf = perf_counter()
@@ -879,19 +1040,21 @@
                 end_time_tol = perf_counter()
 
                 self.v_0 = V[:, np.newaxis]  # Voltage at load buses
                 iteration += 1
 
             self.v_0 = self.v_0.reshape(ts_chunk, n_nodes)
 
-            if solver == "pardiso":
+            if solver == "pardiso" and PARDISO_SOLVER_AVAILABLE:
                 pSolve.clear()
             end_time_pf = perf_counter() - (end_time_tol - start_time_tol)
 
-            if iteration == iterations:  # TODO: If the answer is 0, the iterations are < iterations but the solutions is not good.
+            if (
+                iteration == iterations
+            ):  # TODO: If the answer is 0, the iterations are < iterations but the solutions is not good.
                 flag_convergence = False
                 warnings.warn("Power flow did not converge.")
             else:
                 flag_convergence = True
 
             total_time_pre_pf = end_time_pre_pf - start_time_pre_pf
             total_time_pf = end_time_pf - start_time_pf
@@ -904,27 +1067,29 @@
             flag_convergence_all.append(flag_convergence)
             flag_convergence_bool_all = flag_convergence_bool_all & flag_convergence
 
             v0_solutions.append(self.v_0.copy())
 
         self.v_0 = np.vstack(v0_solutions)
 
-
-        solution = {"v": self.v_0,  # 2D-Vector. Solution of voltage in complex numbers
-                    "time_pre_pf": sum(total_time_pre_pf_all),
-                    "time_pf": sum(total_time_pf_all),
-                    "time_algorithm": sum(total_time_algorithm_all),
-                    "iterations": np.floor(np.mean(iterations_all)),
-
-                    # In this case, the report are the batches
-                    "convergence": flag_convergence_bool_all,
-                    "iterations_log": iterations_all,
-                    "time_pre_pf_log": total_time_pre_pf_all,
-                    "time_pf_log": total_time_pf_all,
-                    "convergence_log": flag_convergence_all
-                    }
+        solution = {
+            "v": self.v_0,  # 2D-Vector. Solution of voltage in complex numbers
+            "time_pre_pf": sum(total_time_pre_pf_all),
+            "time_pf": sum(total_time_pf_all),
+            "time_algorithm": sum(total_time_algorithm_all),
+            "iterations": np.floor(np.mean(iterations_all)),
+            # In this case, the report are the batches
+            "convergence": flag_convergence_bool_all,
+            "iterations_log": iterations_all,
+            "time_pre_pf_log": total_time_pre_pf_all,
+            "time_pf_log": total_time_pf_all,
+            "convergence_log": flag_convergence_all,
+        }
 
         return solution
 
-
     def line_currents(self, volt_solutions=None):
         raise NotImplementedError
+
+
+if __name__ == "__main__":
+    testing = GridTensor()
```

### Comparing `tensorpowerflow-0.0.5/tensorpowerflow/numbarize.py` & `tensorpowerflow-0.0.7/tensorpowerflow/numbarize.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 from numba import prange
 import numpy as np
 
 
-def pre_power_flow_sam_sequential(active_power,
-                                  reactive_power,
-                                  s_base,
-                                  alpha_Z,
-                                  alpha_I,
-                                  Yds,
-                                  Ydd,
-                                  nb
-                                  ):
+def pre_power_flow_sam_sequential(
+    active_power, reactive_power, s_base, alpha_Z, alpha_I, Yds, Ydd, nb
+):
     active_power_pu = active_power / s_base  # Vector with all active power except slack
-    reactive_power_pu = reactive_power / s_base  # Vector with all reactive power except slack
-
-    S_nom = (active_power_pu + 1j * reactive_power_pu).reshape(-1, )
+    reactive_power_pu = (
+        reactive_power / s_base
+    )  # Vector with all reactive power except slack
+
+    S_nom = (active_power_pu + 1j * reactive_power_pu).reshape(
+        -1,
+    )
     if not np.any(alpha_Z):  # \alpha_z is 0
         B_inv = np.linalg.inv(Ydd)
     else:
         # TODO: Assert that the shapoes of alpha_Z and S_nom are the same
         B = np.diag(np.multiply(alpha_Z, np.conj(S_nom))) + Ydd
         B_inv = np.linalg.inv(B)
 
     if not np.any(alpha_I):  # all \alpha_i are 0
         C = Yds  # Constant
     else:
         C = Yds + np.multiply(alpha_I, np.conj(S_nom)).reshape(nb - 1, 1)  # Constant
 
     return B_inv, C, S_nom
 
-def power_flow_sam_sequential(B_inv,
-                              C,
-                              v_0,
-                              s_n,
-                              alpha_P,
-                              iterations,
-                              tolerance,
-                              ):
+
+def power_flow_sam_sequential(
+    B_inv,
+    C,
+    v_0,
+    s_n,
+    alpha_P,
+    iterations,
+    tolerance,
+):
     iteration = 0
     tol = np.inf
     while (iteration < iterations) & (tol >= tolerance):
         # Update matrices A and D:
         A = np.diag(alpha_P * (1 / np.conj(v_0) ** 2) * np.conj(s_n))
         D = 2 * alpha_P * (1 / np.conj(v_0)) * np.conj(s_n)
 
@@ -48,21 +48,22 @@
         tol = np.max(np.abs(np.abs(v) - np.abs(v_0)))
         v_0 = v  # Voltage at load buses
         iteration += 1
 
     return v_0, iteration  # Solution of voltage in complex numbers
 
 
-def power_flow_sam_sequential_constant_power_only(B_inv,
-                                                  C,
-                                                  v_0,
-                                                  s_n,
-                                                  iterations,
-                                                  tolerance,
-                                                  ):
+def power_flow_sam_sequential_constant_power_only(
+    B_inv,
+    C,
+    v_0,
+    s_n,
+    iterations,
+    tolerance,
+):
     iteration = 0
     tol = np.inf
     while (iteration < iterations) & (tol >= tolerance):
         # Update matrices A and D:
         A = np.diag((1 / np.conj(v_0) ** 2) * np.conj(s_n))
         D = 2 * (1 / np.conj(v_0)) * np.conj(s_n)
         # D = D.reshape(-1, 1)
@@ -71,25 +72,27 @@
         tol = np.max(np.abs(np.abs(v) - np.abs(v_0)))
         v_0 = v  # Voltage at load buses
         iteration += 1
 
     return v_0, iteration  # Solution of voltage in complex numbers
 
 
-def pre_power_flow_tensor(flag_all_constant_impedance_is_zero,
-                          flag_all_constant_current_is_zero,
-                          flag_all_constant_powers_are_ones,
-                          ts_n,
-                          nb,
-                          S_nom,
-                          alpha_Z,
-                          alpha_I,
-                          alpha_P,
-                          Yds,
-                          Ydd):
+def pre_power_flow_tensor(
+    flag_all_constant_impedance_is_zero,
+    flag_all_constant_current_is_zero,
+    flag_all_constant_powers_are_ones,
+    ts_n,
+    nb,
+    S_nom,
+    alpha_Z,
+    alpha_I,
+    alpha_P,
+    Yds,
+    Ydd,
+):
     if not flag_all_constant_impedance_is_zero:
         _alpha_z_power = np.multiply(np.conj(S_nom), alpha_Z)  # (ts x nodes)
     else:
         _alpha_z_power = np.zeros((ts_n, nb - 1))  # (ts x nodes)
 
     if not flag_all_constant_current_is_zero:
         _alpha_i_power = np.multiply(np.conj(S_nom), alpha_I)  # (ts x nodes)
@@ -101,31 +104,37 @@
     else:
         _alpha_p_power = np.multiply(np.conj(S_nom), alpha_P)  # (ts x nodes)
 
     _B_inv2 = np.zeros((ts_n, nb - 1, nb - 1), dtype="complex128")
     _F_2 = np.zeros((ts_n, nb - 1, nb - 1), dtype="complex128")
     _W_2 = np.zeros((ts_n, nb - 1), dtype="complex128")
 
-    _C2 = _alpha_i_power + Yds.reshape(-1)  # (ts x nodes)  Sum is broadcasted to all rows of _alpha_i_power
+    _C2 = _alpha_i_power + Yds.reshape(
+        -1
+    )  # (ts x nodes)  Sum is broadcasted to all rows of _alpha_i_power
 
     for i in prange(ts_n):
         _B_inv2[i] = np.linalg.inv(np.diag(_alpha_z_power[i]) + Ydd)
-        _F_2[i] = -_B_inv2[i] * _alpha_p_power[i].reshape(1, -1)  # Broadcast multiplication
+        _F_2[i] = -_B_inv2[i] * _alpha_p_power[i].reshape(
+            1, -1
+        )  # Broadcast multiplication
         _W_2[i] = (-_B_inv2[i] @ _C2[i].reshape(-1, 1)).reshape(-1)
 
     return _F_2, _W_2
 
-def power_flow_tensor(_F_,
-                      _W_,
-                      v_0,
-                      ts_n,
-                      nb,
-                      iterations,
-                      tolerance,
-                      ):
+
+def power_flow_tensor(
+    _F_,
+    _W_,
+    v_0,
+    ts_n,
+    nb,
+    iterations,
+    tolerance,
+):
     iteration = 0
     tol = np.inf
     while (iteration < iterations) & (tol >= tolerance):
         v_recp_conj = np.reciprocal(np.conj(v_0))
         RT2 = np.zeros((ts_n, nb - 1), dtype="complex128")
         for i in prange(ts_n):  # This is critical as it makes a lot of difference
             RT2[i] = _F_[i] @ v_recp_conj[i]
@@ -133,84 +142,65 @@
         tol = np.max(np.abs(np.abs(v) - np.abs(v_0)))
         v_0 = v
         iteration += 1
 
     return v_0, iteration
 
 
-
-def power_flow_tensor_constant_power_numba_parallel_True(K,
-                                         L,
-                                         S,
-                                         v0,
-                                         ts,
-                                         nb,
-                                         iterations,
-                                         tolerance
-                                         ):
+def power_flow_tensor_constant_power_numba_parallel_True(
+    K, L, S, v0, ts, nb, iterations, tolerance
+):
     """
     Original formulation of the CPU-Dense Tensor power flow. The operation of the for loop with the prange is
     quite inefficient.
     """
 
     iteration = 0
     tol = np.inf
     while (iteration < iterations) & (tol >= tolerance):
-        v = np.zeros((ts, nb - 1), dtype="complex128")  # TODO: Test putting this outside of while loop
+        v = np.zeros(
+            (ts, nb - 1), dtype="complex128"
+        )  # TODO: Test putting this outside of while loop
         for i in prange(ts):
             v[i] = (K @ (np.conj(S[i]) * (1 / np.conj(v0[i]))).reshape(-1, 1) + L).T
         tol = np.max(np.abs(np.abs(v) - np.abs(v0)))
         v0 = v  # Voltage at load buses
         iteration += 1
 
     return v0, iteration
 
 
-def power_flow_tensor_constant_power(K,
-                                     L,
-                                     S,
-                                     v0,
-                                     ts,
-                                     nb,
-                                     iterations,
-                                     tolerance
-                                     ):
+def power_flow_tensor_constant_power(K, L, S, v0, ts, nb, iterations, tolerance):
     """This implementation is very efficient, but the broadcasting of Z + L is not supported by numba -> parallel=True"""
     iteration = 0
     tol = np.inf
     S = S.T
     v0 = v0.T
 
     LAMBDA = np.zeros((nb - 1, ts)).astype(np.complex128)
     Z = np.zeros((nb - 1, ts)).astype(np.complex128)
     voltage_k = np.zeros((nb - 1, ts)).astype(np.complex128)
 
     while iteration < iterations and tol >= tolerance:
         LAMBDA = np.conj(S * (1 / v0))  # Hadamard product ( (nb-1) x ts)
         Z = K @ LAMBDA  # Matrix ( (nb-1) x ts )
-        voltage_k = Z + L  # This is a broadcasted sum dim => ( (nb-1) x ts  +  (nb-1) x 1 => (nb-1) x ts )
+        voltage_k = (
+            Z + L
+        )  # This is a broadcasted sum dim => ( (nb-1) x ts  +  (nb-1) x 1 => (nb-1) x ts )
         tol = np.max(np.abs(np.abs(voltage_k) - np.abs(v0)))
         v0 = voltage_k
         iteration += 1
 
     S = S.T  # Recover the original shape of the power
     v0 = v0.T  # Recover the original shape of the power
 
     return v0, iteration
 
 
-def power_flow_tensor_constant_power_new(K,
-                                         L,
-                                         S,
-                                         v0,
-                                         ts,
-                                         nb,
-                                         iterations,
-                                         tolerance
-                                         ):
+def power_flow_tensor_constant_power_new(K, L, S, v0, ts, nb, iterations, tolerance):
     """This version support parallel=True but the results are incorrect"""
     iteration = 0
     tol = np.inf
     # S = S.T
     # v0 = v0.T
 
     LAMBDA = np.zeros((nb - 1, ts)).astype(np.complex128)
@@ -220,15 +210,17 @@
     voltage_k = voltage_k.T
     W = L.ravel()
 
     while iteration < iterations and tol >= tolerance:
         LAMBDA = np.conj(S.T * (1 / v0.T))  # Hadamard product ( (nb-1) x ts)
         Z = K @ LAMBDA  # Matrix ( (nb-1) x ts )
         Z = Z.T
-        for j in prange(ts): # This is a brodcasted sum ( (nb-1) x ts  +  (nb-1) x 1 => (nb-1) x ts )
+        for j in prange(
+            ts
+        ):  # This is a brodcasted sum ( (nb-1) x ts  +  (nb-1) x 1 => (nb-1) x ts )
             voltage_k[j] = Z[j] + W
 
         tol = np.max(np.abs(np.abs(voltage_k) - np.abs(v0)))
         v0 = voltage_k
         iteration += 1
 
-    return v0, iteration
+    return v0, iteration
```

### Comparing `tensorpowerflow-0.0.5/tensorpowerflow/pyMKL/MKLutils.py` & `tensorpowerflow-0.0.7/tensorpowerflow/pyMKL/MKLutils.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import division
-from __future__ import absolute_import
-# from future import standard_library
-# standard_library.install_aliases()
-
-from ctypes import Structure, POINTER, c_int, c_char_p
-from . import MKLlib
-
-class pyMKLVersion(Structure):
-    _fields_ = [('MajorVersion',c_int),
-                ('MinorVersion',c_int),
-                ('UpdateVersion',c_int),
-                ('ProductStatus',c_char_p),
-                ('Build',c_char_p),
-                ('Processor',c_char_p),
-                ('Platform',c_char_p)]
-_mkl_get_version = MKLlib.mkl_get_version
-_mkl_get_version.argtypes = [POINTER(pyMKLVersion)]
-_mkl_get_version.restype = None
-
-def mkl_get_version():
-    MKLVersion = pyMKLVersion()
-    _mkl_get_version(MKLVersion)
-    version = {'MajorVersion':MKLVersion.MajorVersion,
-               'MinorVersion':MKLVersion.MinorVersion,
-               'UpdateVersion':MKLVersion.UpdateVersion,
-               'ProductStatus':MKLVersion.ProductStatus,
-               'Build':MKLVersion.Build,
-               'Platform':MKLVersion.Platform}
-
-    versionString = 'Intel(R) Math Kernel Library Version {MajorVersion}.{MinorVersion}.{UpdateVersion} {ProductStatus} Build {Build} for {Platform} applications'.format(**version)
-
-    return versionString
-
-
-_mkl_get_max_threads = MKLlib.mkl_get_max_threads
-_mkl_get_max_threads.argtypes = None
-_mkl_get_max_threads.restype = c_int
-
-def mkl_get_max_threads():
-    max_threads = _mkl_get_max_threads()
-    return max_threads
-
-
-_mkl_set_num_threads = MKLlib.mkl_set_num_threads
-_mkl_set_num_threads.argtypes = [POINTER(c_int)]
-_mkl_set_num_threads.restype = None
-
-def mkl_set_num_threads(num_threads):
-    _mkl_set_num_threads(c_int(num_threads))
+from __future__ import unicode_literals
+from __future__ import print_function
+from __future__ import division
+from __future__ import absolute_import
+# from future import standard_library
+# standard_library.install_aliases()
+
+from ctypes import Structure, POINTER, c_int, c_char_p
+from . import MKLlib
+
+class pyMKLVersion(Structure):
+    _fields_ = [('MajorVersion',c_int),
+                ('MinorVersion',c_int),
+                ('UpdateVersion',c_int),
+                ('ProductStatus',c_char_p),
+                ('Build',c_char_p),
+                ('Processor',c_char_p),
+                ('Platform',c_char_p)]
+_mkl_get_version = MKLlib.mkl_get_version
+_mkl_get_version.argtypes = [POINTER(pyMKLVersion)]
+_mkl_get_version.restype = None
+
+def mkl_get_version():
+    MKLVersion = pyMKLVersion()
+    _mkl_get_version(MKLVersion)
+    version = {'MajorVersion':MKLVersion.MajorVersion,
+               'MinorVersion':MKLVersion.MinorVersion,
+               'UpdateVersion':MKLVersion.UpdateVersion,
+               'ProductStatus':MKLVersion.ProductStatus,
+               'Build':MKLVersion.Build,
+               'Platform':MKLVersion.Platform}
+
+    versionString = 'Intel(R) Math Kernel Library Version {MajorVersion}.{MinorVersion}.{UpdateVersion} {ProductStatus} Build {Build} for {Platform} applications'.format(**version)
+
+    return versionString
+
+
+_mkl_get_max_threads = MKLlib.mkl_get_max_threads
+_mkl_get_max_threads.argtypes = None
+_mkl_get_max_threads.restype = c_int
+
+def mkl_get_max_threads():
+    max_threads = _mkl_get_max_threads()
+    return max_threads
+
+
+_mkl_set_num_threads = MKLlib.mkl_set_num_threads
+_mkl_set_num_threads.argtypes = [POINTER(c_int)]
+_mkl_set_num_threads.restype = None
+
+def mkl_set_num_threads(num_threads):
+    _mkl_set_num_threads(c_int(num_threads))
```

### Comparing `tensorpowerflow-0.0.5/tensorpowerflow/pyMKL/Tests/test_Pardiso.py` & `tensorpowerflow-0.0.7/tensorpowerflow/pyMKL/Tests/trial_Pardiso.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,206 +1,205 @@
-from __future__ import division
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import absolute_import
-from future import standard_library
-standard_library.install_aliases()
-
-import unittest
-import numpy as np
-import scipy.sparse as sp
-from pyMKL import pardisoSolver
-
-nSize = 100
-
-class TestPardiso_oneRHS(unittest.TestCase):
-
-    def test_RealNonSym(self):
-        nSize = 100
-        A = sp.rand(nSize, nSize, 0.05, format='csr', random_state=100)
-        A = A + sp.spdiags(np.ones(nSize), 0, nSize, nSize)
-        A = A.tocsr()
-
-        np.random.seed(1)
-        xTrue = np.random.rand(nSize)
-        rhs = A.dot(xTrue)
-
-        pSolve = pardisoSolver(A, mtype=11)
-
-        pSolve.run_pardiso(12)
-        x = pSolve.run_pardiso(33, rhs)
-        pSolve.clear()
-
-        self.assertLess(np.linalg.norm(x-xTrue)/np.linalg.norm(xTrue), 1e-12)
-
-    def test_RealSPD(self):
-
-        A = sp.rand(nSize, nSize, 0.05, format='csr', random_state=100)
-        A = A.T.dot(A) + sp.spdiags(np.ones(nSize), 0, nSize, nSize)
-        A = A.tocsr()
-
-        np.random.seed(1)
-        xTrue = np.random.rand(nSize)
-        rhs = A.dot(xTrue)
-
-        pSolve = pardisoSolver(A, mtype=2)
-
-        pSolve.run_pardiso(12)
-        x = pSolve.run_pardiso(33, rhs)
-        pSolve.clear()
-
-        self.assertLess(np.linalg.norm(x-xTrue)/np.linalg.norm(xTrue), 1e-12)
-
-    def test_RealPosInd(self):
-
-        A = sp.rand(nSize, nSize, 0.05, format='csr', random_state=100)
-        d = np.ones(nSize)
-        d[nSize//2:] = -1.
-        A = A.T.dot(A) + sp.spdiags(d, 0, nSize, nSize)
-        A = A.tocsr()
-
-        np.random.seed(1)
-        xTrue = np.random.rand(nSize)
-        rhs = A.dot(xTrue)
-
-        pSolve = pardisoSolver(A, mtype=-2)
-
-        pSolve.run_pardiso(12)
-        x = pSolve.run_pardiso(33, rhs)
-        pSolve.clear()
-
-        self.assertLess(np.linalg.norm(x-xTrue)/np.linalg.norm(xTrue), 1e-12)
-
-    def test_ComplexNonSym(self):
-        nSize = 100
-        A = sp.rand(nSize, nSize, 0.05, format='csr', random_state=100)
-        A = A + sp.spdiags(np.ones(nSize), 0, nSize, nSize)
-        A.data = A.data + 1j*np.random.rand(A.nnz)
-        A = A.tocsr()
-
-        np.random.seed(1)
-        xTrue = np.random.rand(nSize) + 1j*np.random.rand(nSize)
-        rhs = A.dot(xTrue)
-
-        pSolve = pardisoSolver(A, mtype=13)
-        pSolve.run_pardiso(12)
-        x = pSolve.run_pardiso(33, rhs)
-        pSolve.clear()
-
-        self.assertLess(np.linalg.norm(x-xTrue)/np.linalg.norm(xTrue), 1e-12)
-
-    def test_ComplexNonSym_RealRHS(self):
-        nSize = 100
-        A = sp.rand(nSize, nSize, 0.05, format='csr', random_state=100)
-        A = A + sp.spdiags(np.ones(nSize), 0, nSize, nSize)
-        A.data = A.data + 1j*np.random.rand(A.nnz)
-        A = A.tocsr()
-
-        np.random.seed(1)
-        rhs = np.random.rand(nSize)
-
-        pSolve = pardisoSolver(A, mtype=13)
-        pSolve.run_pardiso(12)
-        x = pSolve.run_pardiso(33, rhs)
-        pSolve.clear()
-
-        self.assertLess(np.linalg.norm(A.dot(x)-rhs), 1e-12)
-
-    def test_ComplexSym(self):
-        nSize = 100
-        A = sp.rand(nSize, nSize, 0.05, format='csr', random_state=100)
-        A.data = A.data + 1j*np.random.rand(A.nnz)
-        A = A.T.dot(A) + sp.spdiags(np.ones(nSize), 0, nSize, nSize)
-        A = A.tocsr()
-
-        np.random.seed(1)
-        xTrue = np.random.rand(nSize) + 1j*np.random.rand(nSize)
-        rhs = A.dot(xTrue)
-
-        pSolve = pardisoSolver(A, mtype=6)
-        pSolve.run_pardiso(12)
-        x = pSolve.run_pardiso(33, rhs)
-        pSolve.clear()
-
-        self.assertLess(np.linalg.norm(x-xTrue)/np.linalg.norm(xTrue), 1e-12)
-
-    def test_ComplexHerm(self):
-        nSize = 100
-        A = sp.rand(nSize, nSize, 0.05, format='csr', random_state=100)
-        A.data = A.data + 1j*np.random.rand(A.nnz)
-        A = A.T.dot(A.conj()) + sp.spdiags(np.ones(nSize), 0, nSize, nSize)
-        A = A.tocsr()
-
-        np.random.seed(1)
-        xTrue = np.random.rand(nSize) + 1j*np.random.rand(nSize)
-        rhs = A.dot(xTrue)
-
-        pSolve = pardisoSolver(A, mtype=4)
-        pSolve.run_pardiso(12)
-        x = pSolve.run_pardiso(33, rhs)
-        pSolve.clear()
-
-        self.assertLess(np.linalg.norm(x-xTrue)/np.linalg.norm(xTrue), 1e-12)
-
-class TestPardiso_multipleRHS(unittest.TestCase):
-    
-    nRHS = 20
-
-    def test_RealNonSym(self):
-        nSize = 100
-        A = sp.rand(nSize, nSize, 0.05, format='csr', random_state=100)
-        A = A + sp.spdiags(np.ones(nSize), 0, nSize, nSize)
-        A = A.tocsr()
-
-        np.random.seed(1)
-        xTrue = np.random.rand(nSize,self.nRHS)
-        rhs = A.dot(xTrue)
-
-        pSolve = pardisoSolver(A, mtype=11)
-
-        pSolve.run_pardiso(12)
-        x = pSolve.run_pardiso(33, rhs)
-        pSolve.clear()
-
-        for i in range(self.nRHS):
-            self.assertLess(np.linalg.norm(x[:,i]-xTrue[:,i])/np.linalg.norm(xTrue[:,i]), 1e-12)
-
-    def test_ComplexHerm(self):
-        nSize = 100
-        A = sp.rand(nSize, nSize, 0.05, format='csr', random_state=100)
-        A.data = A.data + 1j*np.random.rand(A.nnz)
-        A = A.T.dot(A.conj()) + sp.spdiags(np.ones(nSize), 0, nSize, nSize)
-        A = A.tocsr()
-
-        np.random.seed(1)
-        xTrue = np.random.rand(nSize, self.nRHS) + 1j*np.random.rand(nSize, self.nRHS)
-        rhs = A.dot(xTrue)
-
-        pSolve = pardisoSolver(A, mtype=4)
-        pSolve.run_pardiso(12)
-        x = pSolve.run_pardiso(33, rhs)
-        pSolve.clear()
-        
-        for i in range(self.nRHS):
-            self.assertLess(np.linalg.norm(x[:,i]-xTrue[:,i])/np.linalg.norm(xTrue[:,i]), 1e-12)
-
-    def test_FactorSolve(self):
-        nSize = 100
-        A = sp.rand(nSize, nSize, 0.05, format='csr', random_state=100)
-        A = A + sp.spdiags(np.ones(nSize), 0, nSize, nSize)
-        A = A.tocsr()
-
-        np.random.seed(1)
-        xTrue = np.random.rand(nSize)
-        rhs = A.dot(xTrue)
-
-        pSolve = pardisoSolver(A, mtype=11)
-
-        pSolve.factor()
-        x = pSolve.solve(rhs)
-        pSolve.clear()
-
-        self.assertLess(np.linalg.norm(x-xTrue)/np.linalg.norm(xTrue), 1e-12)
-
-
-if __name__ == '__main__':
-    unittest.main()
+# from __future__ import division
+# from __future__ import unicode_literals
+# from __future__ import print_function
+# from __future__ import absolute_import
+# from future import standard_library
+# standard_library.install_aliases()
+import unittest
+import numpy as np
+import scipy.sparse as sp
+from .. import pardisoSolver
+
+nSize = 100
+
+class TestPardiso_oneRHS(unittest.TestCase):
+
+    def test_RealNonSym(self):
+        nSize = 100
+        A = sp.rand(nSize, nSize, 0.05, format='csr', random_state=100)
+        A = A + sp.spdiags(np.ones(nSize), 0, nSize, nSize)
+        A = A.tocsr()
+
+        np.random.seed(1)
+        xTrue = np.random.rand(nSize)
+        rhs = A.dot(xTrue)
+
+        pSolve = pardisoSolver(A, mtype=11)
+
+        pSolve.run_pardiso(12)
+        x = pSolve.run_pardiso(33, rhs)
+        pSolve.clear()
+
+        self.assertLess(np.linalg.norm(x-xTrue)/np.linalg.norm(xTrue), 1e-12)
+
+    def test_RealSPD(self):
+
+        A = sp.rand(nSize, nSize, 0.05, format='csr', random_state=100)
+        A = A.T.dot(A) + sp.spdiags(np.ones(nSize), 0, nSize, nSize)
+        A = A.tocsr()
+
+        np.random.seed(1)
+        xTrue = np.random.rand(nSize)
+        rhs = A.dot(xTrue)
+
+        pSolve = pardisoSolver(A, mtype=2)
+
+        pSolve.run_pardiso(12)
+        x = pSolve.run_pardiso(33, rhs)
+        pSolve.clear()
+
+        self.assertLess(np.linalg.norm(x-xTrue)/np.linalg.norm(xTrue), 1e-12)
+
+    def test_RealPosInd(self):
+
+        A = sp.rand(nSize, nSize, 0.05, format='csr', random_state=100)
+        d = np.ones(nSize)
+        d[nSize//2:] = -1.
+        A = A.T.dot(A) + sp.spdiags(d, 0, nSize, nSize)
+        A = A.tocsr()
+
+        np.random.seed(1)
+        xTrue = np.random.rand(nSize)
+        rhs = A.dot(xTrue)
+
+        pSolve = pardisoSolver(A, mtype=-2)
+
+        pSolve.run_pardiso(12)
+        x = pSolve.run_pardiso(33, rhs)
+        pSolve.clear()
+
+        self.assertLess(np.linalg.norm(x-xTrue)/np.linalg.norm(xTrue), 1e-12)
+
+    def test_ComplexNonSym(self):
+        nSize = 100
+        A = sp.rand(nSize, nSize, 0.05, format='csr', random_state=100)
+        A = A + sp.spdiags(np.ones(nSize), 0, nSize, nSize)
+        A.data = A.data + 1j*np.random.rand(A.nnz)
+        A = A.tocsr()
+
+        np.random.seed(1)
+        xTrue = np.random.rand(nSize) + 1j*np.random.rand(nSize)
+        rhs = A.dot(xTrue)
+
+        pSolve = pardisoSolver(A, mtype=13)
+        pSolve.run_pardiso(12)
+        x = pSolve.run_pardiso(33, rhs)
+        pSolve.clear()
+
+        self.assertLess(np.linalg.norm(x-xTrue)/np.linalg.norm(xTrue), 1e-12)
+
+    def test_ComplexNonSym_RealRHS(self):
+        nSize = 100
+        A = sp.rand(nSize, nSize, 0.05, format='csr', random_state=100)
+        A = A + sp.spdiags(np.ones(nSize), 0, nSize, nSize)
+        A.data = A.data + 1j*np.random.rand(A.nnz)
+        A = A.tocsr()
+
+        np.random.seed(1)
+        rhs = np.random.rand(nSize)
+
+        pSolve = pardisoSolver(A, mtype=13)
+        pSolve.run_pardiso(12)
+        x = pSolve.run_pardiso(33, rhs)
+        pSolve.clear()
+
+        self.assertLess(np.linalg.norm(A.dot(x)-rhs), 1e-12)
+
+    def test_ComplexSym(self):
+        nSize = 100
+        A = sp.rand(nSize, nSize, 0.05, format='csr', random_state=100)
+        A.data = A.data + 1j*np.random.rand(A.nnz)
+        A = A.T.dot(A) + sp.spdiags(np.ones(nSize), 0, nSize, nSize)
+        A = A.tocsr()
+
+        np.random.seed(1)
+        xTrue = np.random.rand(nSize) + 1j*np.random.rand(nSize)
+        rhs = A.dot(xTrue)
+
+        pSolve = pardisoSolver(A, mtype=6)
+        pSolve.run_pardiso(12)
+        x = pSolve.run_pardiso(33, rhs)
+        pSolve.clear()
+
+        self.assertLess(np.linalg.norm(x-xTrue)/np.linalg.norm(xTrue), 1e-12)
+
+    def test_ComplexHerm(self):
+        nSize = 100
+        A = sp.rand(nSize, nSize, 0.05, format='csr', random_state=100)
+        A.data = A.data + 1j*np.random.rand(A.nnz)
+        A = A.T.dot(A.conj()) + sp.spdiags(np.ones(nSize), 0, nSize, nSize)
+        A = A.tocsr()
+
+        np.random.seed(1)
+        xTrue = np.random.rand(nSize) + 1j*np.random.rand(nSize)
+        rhs = A.dot(xTrue)
+
+        pSolve = pardisoSolver(A, mtype=4)
+        pSolve.run_pardiso(12)
+        x = pSolve.run_pardiso(33, rhs)
+        pSolve.clear()
+
+        self.assertLess(np.linalg.norm(x-xTrue)/np.linalg.norm(xTrue), 1e-12)
+
+class TestPardiso_multipleRHS(unittest.TestCase):
+    
+    nRHS = 20
+
+    def test_RealNonSym(self):
+        nSize = 100
+        A = sp.rand(nSize, nSize, 0.05, format='csr', random_state=100)
+        A = A + sp.spdiags(np.ones(nSize), 0, nSize, nSize)
+        A = A.tocsr()
+
+        np.random.seed(1)
+        xTrue = np.random.rand(nSize,self.nRHS)
+        rhs = A.dot(xTrue)
+
+        pSolve = pardisoSolver(A, mtype=11)
+
+        pSolve.run_pardiso(12)
+        x = pSolve.run_pardiso(33, rhs)
+        pSolve.clear()
+
+        for i in range(self.nRHS):
+            self.assertLess(np.linalg.norm(x[:,i]-xTrue[:,i])/np.linalg.norm(xTrue[:,i]), 1e-12)
+
+    def test_ComplexHerm(self):
+        nSize = 100
+        A = sp.rand(nSize, nSize, 0.05, format='csr', random_state=100)
+        A.data = A.data + 1j*np.random.rand(A.nnz)
+        A = A.T.dot(A.conj()) + sp.spdiags(np.ones(nSize), 0, nSize, nSize)
+        A = A.tocsr()
+
+        np.random.seed(1)
+        xTrue = np.random.rand(nSize, self.nRHS) + 1j*np.random.rand(nSize, self.nRHS)
+        rhs = A.dot(xTrue)
+
+        pSolve = pardisoSolver(A, mtype=4)
+        pSolve.run_pardiso(12)
+        x = pSolve.run_pardiso(33, rhs)
+        pSolve.clear()
+        
+        for i in range(self.nRHS):
+            self.assertLess(np.linalg.norm(x[:,i]-xTrue[:,i])/np.linalg.norm(xTrue[:,i]), 1e-12)
+
+    def test_FactorSolve(self):
+        nSize = 100
+        A = sp.rand(nSize, nSize, 0.05, format='csr', random_state=100)
+        A = A + sp.spdiags(np.ones(nSize), 0, nSize, nSize)
+        A = A.tocsr()
+
+        np.random.seed(1)
+        xTrue = np.random.rand(nSize)
+        rhs = A.dot(xTrue)
+
+        pSolve = pardisoSolver(A, mtype=11)
+
+        pSolve.factor()
+        x = pSolve.solve(rhs)
+        pSolve.clear()
+
+        self.assertLess(np.linalg.norm(x-xTrue)/np.linalg.norm(xTrue), 1e-12)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `tensorpowerflow-0.0.5/tensorpowerflow/pyMKL/__init__.py` & `tensorpowerflow-0.0.7/tensorpowerflow/pyMKL/__init__.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""
-The code for the pyMKL module is taken and modified from the work of David Marchant.
-From: https://github.com/dwfmarchant/pyMKL
-"""
-
-from __future__ import absolute_import
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import division
-# from future import standard_library
-# standard_library.install_aliases()
-
-import platform
-import numpy as np
-import scipy.sparse as sp
-from .loadMKL import _loadMKL
-
-MKLlib = _loadMKL()
-
-from .MKLutils import mkl_get_version, mkl_get_max_threads, mkl_set_num_threads
-from .pardisoInterface import pardisoinit, pardiso
-from .pardisoSolver import pardisoSolver
+"""
+The code for the pyMKL module is taken and modified from the work of David Marchant.
+From: https://github.com/dwfmarchant/pyMKL
+"""
+
+from __future__ import absolute_import
+from __future__ import unicode_literals
+from __future__ import print_function
+from __future__ import division
+# from future import standard_library
+# standard_library.install_aliases()
+
+import platform
+import numpy as np
+import scipy.sparse as sp
+from .loadMKL import _loadMKL
+
+MKLlib = _loadMKL()
+
+from .MKLutils import mkl_get_version, mkl_get_max_threads, mkl_set_num_threads
+from .pardisoInterface import pardisoinit, pardiso
+from .pardisoSolver import pardisoSolver
```

### Comparing `tensorpowerflow-0.0.5/tensorpowerflow/pyMKL/pardisoInterface.py` & `tensorpowerflow-0.0.7/tensorpowerflow/pyMKL/pardisoInterface.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import division
-from __future__ import absolute_import
-# from future import standard_library
-# standard_library.install_aliases()
-
-from . import MKLlib
-from ctypes import POINTER, c_int, c_longlong
-
-pardisoinit = MKLlib.pardisoinit
-
-pardisoinit.argtypes = [POINTER(c_longlong),
-                        POINTER(c_int),
-                        POINTER(c_int)]
-pardisoinit.restype = None
-
-pardiso = MKLlib.pardiso
-pardiso.argtypes = [POINTER(c_longlong), # pt
-                    POINTER(c_int),      # maxfct
-                    POINTER(c_int),      # mnum
-                    POINTER(c_int),      # mtype
-                    POINTER(c_int),      # phase
-                    POINTER(c_int),      # n
-                    POINTER(None),       # a
-                    POINTER(c_int),      # ia
-                    POINTER(c_int),      # ja
-                    POINTER(c_int),      # perm
-                    POINTER(c_int),      # nrhs
-                    POINTER(c_int),      # iparm
-                    POINTER(c_int),      # msglvl
-                    POINTER(None),       # b
-                    POINTER(None),       # x
-                    POINTER(c_int)]      # error)
-pardiso.restype = None
+from __future__ import unicode_literals
+from __future__ import print_function
+from __future__ import division
+from __future__ import absolute_import
+# from future import standard_library
+# standard_library.install_aliases()
+
+from . import MKLlib
+from ctypes import POINTER, c_int, c_longlong
+
+pardisoinit = MKLlib.pardisoinit
+
+pardisoinit.argtypes = [POINTER(c_longlong),
+                        POINTER(c_int),
+                        POINTER(c_int)]
+pardisoinit.restype = None
+
+pardiso = MKLlib.pardiso
+pardiso.argtypes = [POINTER(c_longlong), # pt
+                    POINTER(c_int),      # maxfct
+                    POINTER(c_int),      # mnum
+                    POINTER(c_int),      # mtype
+                    POINTER(c_int),      # phase
+                    POINTER(c_int),      # n
+                    POINTER(None),       # a
+                    POINTER(c_int),      # ia
+                    POINTER(c_int),      # ja
+                    POINTER(c_int),      # perm
+                    POINTER(c_int),      # nrhs
+                    POINTER(c_int),      # iparm
+                    POINTER(c_int),      # msglvl
+                    POINTER(None),       # b
+                    POINTER(None),       # x
+                    POINTER(c_int)]      # error)
+pardiso.restype = None
```

### Comparing `tensorpowerflow-0.0.5/tensorpowerflow/pyMKL/pardisoSolver.py` & `tensorpowerflow-0.0.7/tensorpowerflow/pyMKL/pardisoSolver.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,249 +1,250 @@
-from __future__ import unicode_literals
-from __future__ import print_function
-from __future__ import division
-from __future__ import absolute_import
-# from future import standard_library
-# standard_library.install_aliases()
-from builtins import object
-
-from .pardisoInterface import pardisoinit, pardiso
-from .MKLutils import mkl_get_version, mkl_get_max_threads
-from ctypes import POINTER, byref, c_longlong, c_int
-import numpy as np
-import scipy.sparse as sp
-from numpy import ctypeslib
-
-"""
-mtype options
-  1 -> real and structurally symmetric
-  2 -> real and symmetric positive definite
- -2 -> real and symmetric indefinite
-  3 -> complex and structurally symmetric
-  4 -> complex and Hermitian positive definite
- -4 -> complex and Hermitian indefinite
-  6 -> complex and symmetric
- 11 -> real and nonsymmetric
- 13 -> complex and nonsymmetric
-
-
-phase options
- 11 -> Analysis
- 12 -> Analysis, numerical factorization
- 13 -> Analysis, numerical factorization, solve, iterative refinement
- 22 -> Numerical factorization
- 23 -> Numerical factorization, solve, iterative refinement
- 33 -> Solve, iterative refinement
-331 -> like phase=33, but only forward substitution
-332 -> like phase=33, but only diagonal substitution (if available)
-333 -> like phase=33, but only backward substitution
-  0 -> Release internal memory for L and U matrix number mnum
- -1 -> Release all internal memory for all matrices
-"""
-
-__version__ = mkl_get_version()
-
-class pardisoSolver(object):
-    """Wrapper class for Intel MKL Pardiso solver. """
-    def __init__(self, A, mtype=11, verbose=False, singularity_check=True):
-        '''
-        Parameters
-        ----------
-        A : scipy.sparse.csr.csr_matrix
-            sparse matrix in csr format.
-        mtype : int, optional
-            flag specifying the matrix type. The possible types are:
-
-            - 1 : real and structurally symmetric (not supported)
-            - 2 : real and symmetric positive definite
-            - -2 : real and symmetric indefinite
-            - 3 : complex and structurally symmetric (not supported)
-            - 4 : complex and Hermitian positive definite
-            - -4 : complex and Hermitian indefinite
-            - 6 : complex and symmetric
-            - 11 : real and nonsymmetric (default)
-            - 13 : complex and nonsymmetric
-        verbose : bool, optional
-            flag for verbose output. Default is False.
-
-        Returns
-        -------
-        None
-
-        '''
-
-        self.mtype = mtype
-        if mtype in [1, 3]:
-            msg = "mtype = 1/3 - structurally symmetric matrices not supported"
-            raise NotImplementedError(msg)
-        elif mtype in [2, -2, 4, -4, 6, 11, 13]:
-            pass
-        else:
-            msg = "Invalid mtype: mtype={}".format(mtype)
-            raise ValueError(msg)
-            
-        self.singularity_check = singularity_check
-
-        self.n = A.shape[0]
-
-        if mtype in [4, -4, 6, 13]:
-            # Complex matrix
-            self.dtype = np.complex128
-        elif mtype in [2, -2, 11]:
-            # Real matrix
-            self.dtype = np.float64
-        self.ctypes_dtype = ctypeslib.ndpointer(self.dtype)
-
-        # If A is symmetric, store only the upper triangular portion 
-        if mtype in [2, -2, 4, -4, 6]:
-            A = sp.triu(A, format='csr')
-        elif mtype in [11, 13]:
-            A = A.tocsr()
-
-        if not A.has_sorted_indices:
-            A.sort_indices()
-
-        self.a = A.data
-        self.ia = A.indptr
-        self.ja = A.indices
-
-        self._MKL_a = self.a.ctypes.data_as(self.ctypes_dtype)
-        self._MKL_ia = self.ia.ctypes.data_as(POINTER(c_int))
-        self._MKL_ja = self.ja.ctypes.data_as(POINTER(c_int))
-
-        # Hardcode some parameters for now...
-        self.maxfct = 1
-        self.mnum = 1
-        self.perm = 0
-
-        if verbose:
-            self.msglvl = 1
-        else:
-            self.msglvl = 0
-
-        # Initialize handle to data structure
-        self.pt = np.zeros(64, np.int64)
-        self._MKL_pt = self.pt.ctypes.data_as(POINTER(c_longlong))
-
-        # Initialize parameters
-        self.iparm = np.zeros(64, dtype=np.int32)
-        self._MKL_iparm = self.iparm.ctypes.data_as(POINTER(c_int))
-
-        # Initialize pardiso
-        pardisoinit(self._MKL_pt, byref(c_int(self.mtype)), self._MKL_iparm)
-
-        verstring = mkl_get_version()
-        # Set iparm
-        if '11.3.3' in verstring:
-            self.iparm[1] = 0 
-        else:
-            self.iparm[1] = 3 # Use parallel nested dissection for reordering
-
-        self.iparm[23] = 1 # Use parallel factorization
-        self.iparm[34] = 1 # Zero base indexing
-
-        self.error = 0
-
-    def clear(self):
-        '''
-        Clear the memory allocated from the solver.
-        '''
-        self.run_pardiso(phase=-1)
-
-    @staticmethod
-    def get_version():
-        return mkl_get_version()
-
-    @staticmethod
-    def get_max_num_threads():
-        return mkl_get_max_threads()
-
-    def factor(self):
-        out = self.run_pardiso(phase=12)
-
-    def solve(self, rhs):
-        x = self.run_pardiso(phase=33, rhs=rhs)
-        return x
-
-    def solve_pardiso(self, dummy_A, rhs):
-        """Wrapper that has the same form of spsolve from scipy"""
-        x = self.run_pardiso(phase=33, rhs=rhs)
-        return x
-
-    def run_pardiso(self, phase, rhs=None):
-        '''
-        Run specified phase of the Pardiso solver.
-
-        Parameters
-        ----------
-        phase : int
-            Flag setting the analysis type of the solver:
-
-            -  11 : Analysis
-            -  12 : Analysis, numerical factorization
-            -  13 : Analysis, numerical factorization, solve, iterative refinement
-            -  22 : Numerical factorization
-            -  23 : Numerical factorization, solve, iterative refinement
-            -  33 : Solve, iterative refinement
-            - 331 : like phase=33, but only forward substitution
-            - 332 : like phase=33, but only diagonal substitution (if available)
-            - 333 : like phase=33, but only backward substitution
-            -   0 : Release internal memory for L and U matrix number mnum
-            -  -1 : Release all internal memory for all matrices
-        rhs : ndarray, optional
-            Right hand side of the equation `A x = rhs`. Can either be a vector
-            (array of dimension 1) or a matrix (array of dimension 2). Default
-            is None.
-
-        Returns
-        -------
-        x : ndarray
-            Solution of the system `A x = rhs`, if `rhs` is provided. Is either
-            a vector or a column matrix.
-
-        '''
-
-        if rhs is None:
-            nrhs = 0
-            x = np.zeros(1)
-            rhs = np.zeros(1)
-        else:
-            if rhs.ndim == 1:
-                nrhs = 1
-            elif rhs.ndim == 2:
-                nrhs = rhs.shape[1]
-            else:
-                msg = "Right hand side must either be a 1 or 2 dimensional "+\
-                      "array. Higher order right hand sides are not supported."
-                raise NotImplementedError(msg)
-            rhs = rhs.astype(self.dtype).flatten(order='f')
-            x = np.zeros(nrhs*self.n, dtype=self.dtype)
-
-        MKL_rhs = rhs.ctypes.data_as(self.ctypes_dtype)
-        MKL_x = x.ctypes.data_as(self.ctypes_dtype)
-        MKL_err = c_int(0)
-
-        pardiso(self._MKL_pt,               # pt
-                byref(c_int(self.maxfct)),  # maxfct
-                byref(c_int(self.mnum)),    # mnum
-                byref(c_int(self.mtype)),   # mtype
-                byref(c_int(phase)),        # phase
-                byref(c_int(self.n)),       # n
-                self._MKL_a,                # a
-                self._MKL_ia,               # ia
-                self._MKL_ja,               # ja
-                byref(c_int(self.perm)),    # perm
-                byref(c_int(nrhs)),         # nrhs
-                self._MKL_iparm,            # iparm
-                byref(c_int(self.msglvl)),  # msglvl
-                MKL_rhs,                    # b
-                MKL_x,                      # x
-                byref(MKL_err))             # error
-                
-        self.error = MKL_err.value
-            
-        if self.singularity_check and self.iparm[13] > 0:
-            raise RuntimeError("Pardiso - Number of perturbed pivot elements = " + repr(self.iparm[13]) + ". This could mean that the matrix is singular.")
-
-        if nrhs > 1:
-            x = x.reshape((self.n, nrhs), order='f')
-        return x
+from __future__ import unicode_literals
+from __future__ import print_function
+from __future__ import division
+from __future__ import absolute_import
+# from future import standard_library
+# standard_library.install_aliases()
+from builtins import object
+
+from .pardisoInterface import pardisoinit, pardiso
+from .MKLutils import mkl_get_version, mkl_get_max_threads
+from ctypes import POINTER, byref, c_longlong, c_int
+import numpy as np
+import scipy.sparse as sp
+from numpy import ctypeslib
+
+"""
+mtype options
+  1 -> real and structurally symmetric
+  2 -> real and symmetric positive definite
+ -2 -> real and symmetric indefinite
+  3 -> complex and structurally symmetric
+  4 -> complex and Hermitian positive definite
+ -4 -> complex and Hermitian indefinite
+  6 -> complex and symmetric
+ 11 -> real and nonsymmetric
+ 13 -> complex and nonsymmetric
+
+
+phase options
+ 11 -> Analysis
+ 12 -> Analysis, numerical factorization
+ 13 -> Analysis, numerical factorization, solve, iterative refinement
+ 22 -> Numerical factorization
+ 23 -> Numerical factorization, solve, iterative refinement
+ 33 -> Solve, iterative refinement
+331 -> like phase=33, but only forward substitution
+332 -> like phase=33, but only diagonal substitution (if available)
+333 -> like phase=33, but only backward substitution
+  0 -> Release internal memory for L and U matrix number mnum
+ -1 -> Release all internal memory for all matrices
+"""
+
+__version__ = mkl_get_version()
+
+class pardisoSolver(object):
+    """Wrapper class for Intel MKL Pardiso solver. """
+    def __init__(self, A, mtype=11, verbose=False, singularity_check=True):
+        '''
+        Parameters
+        ----------
+        A : scipy.sparse.csr.csr_matrix
+            sparse matrix in csr format.
+        mtype : int, optional
+            flag specifying the matrix type. The possible types are:
+
+            - 1 : real and structurally symmetric (not supported)
+            - 2 : real and symmetric positive definite
+            - -2 : real and symmetric indefinite
+            - 3 : complex and structurally symmetric (not supported)
+            - 4 : complex and Hermitian positive definite
+            - -4 : complex and Hermitian indefinite
+            - 6 : complex and symmetric
+            - 11 : real and nonsymmetric (default)
+            - 13 : complex and nonsymmetric
+        verbose : bool, optional
+            flag for verbose output. Default is False.
+
+        Returns
+        -------
+        None
+
+        '''
+
+        self.mtype = mtype
+        if mtype in [1, 3]:
+            msg = "mtype = 1/3 - structurally symmetric matrices not supported"
+            raise NotImplementedError(msg)
+        elif mtype in [2, -2, 4, -4, 6, 11, 13]:
+            pass
+        else:
+            msg = "Invalid mtype: mtype={}".format(mtype)
+            raise ValueError(msg)
+            
+        self.singularity_check = singularity_check
+
+        self.n = A.shape[0]
+
+        if mtype in [4, -4, 6, 13]:
+            # Complex matrix
+            self.dtype = np.complex128
+        elif mtype in [2, -2, 11]:
+            # Real matrix
+            self.dtype = np.float64
+        self.ctypes_dtype = ctypeslib.ndpointer(self.dtype)
+
+        # If A is symmetric, store only the upper triangular portion 
+        if mtype in [2, -2, 4, -4, 6]:
+            A = sp.triu(A, format='csr')
+        elif mtype in [11, 13]:
+            A = A.tocsr()
+
+        # 1. Step 1 direct solvers (reordering the matrix)
+        if not A.has_sorted_indices:
+            A.sort_indices()
+
+        self.a = A.data
+        self.ia = A.indptr
+        self.ja = A.indices
+
+        self._MKL_a = self.a.ctypes.data_as(self.ctypes_dtype)
+        self._MKL_ia = self.ia.ctypes.data_as(POINTER(c_int))
+        self._MKL_ja = self.ja.ctypes.data_as(POINTER(c_int))
+
+        # Hardcode some parameters for now...
+        self.maxfct = 1
+        self.mnum = 1
+        self.perm = 0
+
+        if verbose:
+            self.msglvl = 1
+        else:
+            self.msglvl = 0
+
+        # Initialize handle to data structure
+        self.pt = np.zeros(64, np.int64)
+        self._MKL_pt = self.pt.ctypes.data_as(POINTER(c_longlong))
+
+        # Initialize parameters
+        self.iparm = np.zeros(64, dtype=np.int32)
+        self._MKL_iparm = self.iparm.ctypes.data_as(POINTER(c_int))
+
+        # Initialize pardiso
+        pardisoinit(self._MKL_pt, byref(c_int(self.mtype)), self._MKL_iparm)
+
+        verstring = mkl_get_version()
+        # Set iparm
+        if '11.3.3' in verstring:
+            self.iparm[1] = 0 
+        else:
+            self.iparm[1] = 3 # Use parallel nested dissection for reordering
+
+        self.iparm[23] = 1 # Use parallel factorization
+        self.iparm[34] = 1 # Zero base indexing
+
+        self.error = 0
+
+    def clear(self):
+        '''
+        Clear the memory allocated from the solver.
+        '''
+        self.run_pardiso(phase=-1)
+
+    @staticmethod
+    def get_version():
+        return mkl_get_version()
+
+    @staticmethod
+    def get_max_num_threads():
+        return mkl_get_max_threads()
+
+    def factor(self):
+        out = self.run_pardiso(phase=12)
+
+    def solve(self, rhs):
+        x = self.run_pardiso(phase=33, rhs=rhs)
+        return x
+
+    def solve_pardiso(self, dummy_A, rhs):
+        """Wrapper that has the same form of spsolve from scipy"""
+        x = self.run_pardiso(phase=33, rhs=rhs)
+        return x
+
+    def run_pardiso(self, phase, rhs=None):
+        '''
+        Run specified phase of the Pardiso solver.
+
+        Parameters
+        ----------
+        phase : int
+            Flag setting the analysis type of the solver:
+
+            -  11 : Analysis
+            -  12 : Analysis, numerical factorization
+            -  13 : Analysis, numerical factorization, solve, iterative refinement
+            -  22 : Numerical factorization
+            -  23 : Numerical factorization, solve, iterative refinement
+            -  33 : Solve, iterative refinement
+            - 331 : like phase=33, but only forward substitution
+            - 332 : like phase=33, but only diagonal substitution (if available)
+            - 333 : like phase=33, but only backward substitution
+            -   0 : Release internal memory for L and U matrix number mnum
+            -  -1 : Release all internal memory for all matrices
+        rhs : ndarray, optional
+            Right hand side of the equation `A x = rhs`. Can either be a vector
+            (array of dimension 1) or a matrix (array of dimension 2). Default
+            is None.
+
+        Returns
+        -------
+        x : ndarray
+            Solution of the system `A x = rhs`, if `rhs` is provided. Is either
+            a vector or a column matrix.
+
+        '''
+
+        if rhs is None:
+            nrhs = 0
+            x = np.zeros(1)
+            rhs = np.zeros(1)
+        else:
+            if rhs.ndim == 1:
+                nrhs = 1
+            elif rhs.ndim == 2:
+                nrhs = rhs.shape[1]
+            else:
+                msg = "Right hand side must either be a 1 or 2 dimensional "+\
+                      "array. Higher order right hand sides are not supported."
+                raise NotImplementedError(msg)
+            rhs = rhs.astype(self.dtype).flatten(order='f')
+            x = np.zeros(nrhs*self.n, dtype=self.dtype)
+
+        MKL_rhs = rhs.ctypes.data_as(self.ctypes_dtype)
+        MKL_x = x.ctypes.data_as(self.ctypes_dtype)
+        MKL_err = c_int(0)
+
+        pardiso(self._MKL_pt,               # pt
+                byref(c_int(self.maxfct)),  # maxfct
+                byref(c_int(self.mnum)),    # mnum
+                byref(c_int(self.mtype)),   # mtype
+                byref(c_int(phase)),        # phase
+                byref(c_int(self.n)),       # n
+                self._MKL_a,                # a
+                self._MKL_ia,               # ia
+                self._MKL_ja,               # ja
+                byref(c_int(self.perm)),    # perm
+                byref(c_int(nrhs)),         # nrhs
+                self._MKL_iparm,            # iparm
+                byref(c_int(self.msglvl)),  # msglvl
+                MKL_rhs,                    # b
+                MKL_x,                      # x
+                byref(MKL_err))             # error
+                
+        self.error = MKL_err.value
+            
+        if self.singularity_check and self.iparm[13] > 0:
+            raise RuntimeError("Pardiso - Number of perturbed pivot elements = " + repr(self.iparm[13]) + ". This could mean that the matrix is singular.")
+
+        if nrhs > 1:
+            x = x.reshape((self.n, nrhs), order='f')
+        return x
```

### Comparing `tensorpowerflow-0.0.5/tensorpowerflow/tests/test_powerflows.py` & `tensorpowerflow-0.0.7/tensorpowerflow/tests/test_powerflows.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,85 @@
 from tensorpowerflow import GridTensor
 import numpy as np
 
 
 # Solution of the base test case (34-bus system):
-V_SOLUTION = [0.98965162+0.00180549j, 0.98060256+0.00337785j, 0.96828145+0.00704551j,
-              0.95767051+0.01019764j, 0.94765203+0.01316654j, 0.94090964+0.01600068j,
-              0.93719984+0.01754998j, 0.93283877+0.01937559j, 0.93073823+0.02026054j,
-              0.9299309 +0.02058985j, 0.92968994+0.02068728j, 0.98003142+0.00362498j,
-              0.97950885+0.00385019j, 0.97936712+0.00391065j, 0.97935604+0.0039148j,
-              0.93971131+0.01547898j, 0.93309482+0.01739656j, 0.92577912+0.01988823j,
-              0.91988489+0.02188907j, 0.91475251+0.02362566j, 0.90888169+0.02596304j,
-              0.90404908+0.02788248j, 0.89950353+0.02968449j, 0.89731375+0.03055177j,
-              0.89647201+0.03088507j, 0.89622055+0.03098473j, 0.94032081+0.01625577j,
-              0.93992817+0.01642583j, 0.93973182+0.01651086j, 0.9301316+0.02052908j,
-              0.92952481+0.02079761j, 0.92922137+0.02093188j, 0.92912022+0.02097663j]
+V_SOLUTION = [
+    0.98965162 + 0.00180549j,
+    0.98060256 + 0.00337785j,
+    0.96828145 + 0.00704551j,
+    0.95767051 + 0.01019764j,
+    0.94765203 + 0.01316654j,
+    0.94090964 + 0.01600068j,
+    0.93719984 + 0.01754998j,
+    0.93283877 + 0.01937559j,
+    0.93073823 + 0.02026054j,
+    0.92993090 + 0.02058985j,
+    0.92968994 + 0.02068728j,
+    0.98003142 + 0.00362498j,
+    0.97950885 + 0.00385019j,
+    0.97936712 + 0.00391065j,
+    0.97935604 + 0.0039148j,
+    0.93971131 + 0.01547898j,
+    0.93309482 + 0.01739656j,
+    0.92577912 + 0.01988823j,
+    0.91988489 + 0.02188907j,
+    0.91475251 + 0.02362566j,
+    0.90888169 + 0.02596304j,
+    0.90404908 + 0.02788248j,
+    0.89950353 + 0.02968449j,
+    0.89731375 + 0.03055177j,
+    0.89647201 + 0.03088507j,
+    0.89622055 + 0.03098473j,
+    0.94032081 + 0.01625577j,
+    0.93992817 + 0.01642583j,
+    0.93973182 + 0.01651086j,
+    0.93013160 + 0.02052908j,
+    0.92952481 + 0.02079761j,
+    0.92922137 + 0.02093188j,
+    0.92912022 + 0.02097663j,
+]
+
 
 def test_compute_correct_answer_sparse_sequential():
     network = GridTensor()
     V = network.run_pf(algorithm="hp")
     assert np.allclose(V["v"], V_SOLUTION)
 
+
 def test_compute_correct_answer_tensor_sequential():
     network = GridTensor()
     V = network.run_pf(algorithm="sequential")
     assert np.allclose(V["v"], V_SOLUTION)
 
+
 def test_compute_correct_answer_sam():
     network = GridTensor()
     V = network.run_pf(algorithm="sam")
     assert np.allclose(V["v"], V_SOLUTION)
 
+
 def test_compute_correct_answer_tensor_sparse():
     network = GridTensor()
     V = network.run_pf(algorithm="hp-tensor")
     assert np.allclose(V["v"], V_SOLUTION)
 
+
 def test_compute_correct_answer_tensor_dense():
     network = GridTensor()
     V = network.run_pf(algorithm="tensor")
     assert np.allclose(V["v"], V_SOLUTION)
 
+
 def test_compute_correct_answer_sam_sequential():
     network = GridTensor()
     V = network.run_pf_sam_sequential_juan()
     assert np.allclose(V["v"], V_SOLUTION)
 
 
 if __name__ == "__main__":
     test_compute_correct_answer_sparse_sequential()
     test_compute_correct_answer_tensor_sequential()
     test_compute_correct_answer_sam()
     test_compute_correct_answer_tensor_sparse()
     test_compute_correct_answer_tensor_dense()
-    test_compute_correct_answer_sam_sequential()
+    test_compute_correct_answer_sam_sequential()
```

### Comparing `tensorpowerflow-0.0.5/tensorpowerflow/tests/test_tensor_power_flow.py` & `tensorpowerflow-0.0.7/tensorpowerflow/tests/test_tensor_power_flow.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from tensorpowerflow import GridTensor
-import numpy as np
-
-def test_check_output_voltage_array_dimensions():
-    network = GridTensor()
-    active_ns = np.random.normal(50 ,
-                                 scale=10,
-                                 size=(10, 20, 33)).round(3) # Assume 1 slack variable
-    reactive_ns = (active_ns * .1).round(3)
-
-    solution = network.run_pf(active_power=active_ns, reactive_power=reactive_ns)
-
-    assert solution["v"].shape == active_ns.shape
-
-if __name__ == "__main__":
-    test_check_output_voltage_array_dimensions()
+# from tensorpowerflow import GridTensor
+# import numpy as np
+#
+# def test_check_output_voltage_array_dimensions():
+#     network = GridTensor()
+#     active_ns = np.random.normal(50 ,
+#                                  scale=10,
+#                                  size=(10, 20, 33)).round(3) # Assume 1 slack variable
+#     reactive_ns = (active_ns * .1).round(3)
+#
+#     solution = network.run_pf(active_power=active_ns, reactive_power=reactive_ns)
+#
+#     assert solution["v"].shape == active_ns.shape
+#
+# if __name__ == "__main__":
+#     test_check_output_voltage_array_dimensions()
```

### Comparing `tensorpowerflow-0.0.5/tensorpowerflow/utils.py` & `tensorpowerflow-0.0.7/tensorpowerflow/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,136 +6,214 @@
 import pkg_resources
 
 try:
     import pandapower as pp
 except ModuleNotFoundError:
     pass
 
+
 def _load_default_34_node_case():
+
     stream_node_data = pkg_resources.resource_stream(__name__, "data/Lines_34.csv")
     stream_line_data = pkg_resources.resource_stream(__name__, "data/Nodes_34.csv")
 
-    nodes_frame = pd.read_csv(stream_node_data, encoding='utf-8')
-    lines_frame = pd.read_csv(stream_line_data, encoding='utf-8')
+    nodes_frame = pd.read_csv(stream_node_data, encoding="utf-8")
+    lines_frame = pd.read_csv(stream_line_data, encoding="utf-8")
 
     return nodes_frame, lines_frame
 
+
 def _load_default_2_node_case():
     stream_node_data = pkg_resources.resource_stream(__name__, "data/Lines_2.csv")
     stream_line_data = pkg_resources.resource_stream(__name__, "data/Nodes_2.csv")
 
-    nodes_frame = pd.read_csv(stream_node_data, encoding='utf-8')
-    lines_frame = pd.read_csv(stream_line_data, encoding='utf-8')
+    nodes_frame = pd.read_csv(stream_node_data, encoding="utf-8")
+    lines_frame = pd.read_csv(stream_line_data, encoding="utf-8")
 
     return nodes_frame, lines_frame
 
+
 def generate_network(nodes, child=3, plot_graph=False, load_factor=2, line_factor=3):
     LINES = nodes - 1
     G = nx.full_rary_tree(child, nodes)
 
     if plot_graph:
         fig, ax = plt.subplots(1, 1, figsize=(10, 10))
-        nx.draw_kamada_kawai(G, node_size=100, with_labels=True, font_size='medium', ax=ax)
+        nx.draw_kamada_kawai(
+            G, node_size=100, with_labels=True, font_size="medium", ax=ax
+        )
 
     assert nodes == len(G.nodes)
     assert LINES == len(G.edges)
 
     # Generate a pandas dataframe
     PCT, ICT, ZCT = 1, 0, 0
     Tb, Pct, Ict, Zct = 0, PCT, ICT, ZCT
     nodes_ = pd.DataFrame(list(G.nodes), columns=["NODES"]) + 1
 
-
     active_ns = np.random.normal(50 * load_factor, scale=50, size=nodes).round(3)
-    reactive_ns = (active_ns * .1).round(3)
+    reactive_ns = (active_ns * 0.1).round(3)
 
-    power = pd.DataFrame({"PD": active_ns,
-                          "QD": reactive_ns})
-    nodes_properties_ = pd.DataFrame(np.tile([[Tb, Pct, Ict, Zct]], (nodes, 1)),
-                                     columns=["Tb", "Pct", "Ict", "Zct"])
+    power = pd.DataFrame({"PD": active_ns, "QD": reactive_ns})
+    nodes_properties_ = pd.DataFrame(
+        np.tile([[Tb, Pct, Ict, Zct]], (nodes, 1)), columns=["Tb", "Pct", "Ict", "Zct"]
+    )
     nodes_properties = pd.concat([power, nodes_properties_], axis=1)
     nodes_properties = nodes_properties.astype(
-        {"Tb": int, "PD": float, "QD": float, "Pct": int, "Ict": int, "Zct": int})
+        {"Tb": int, "PD": float, "QD": float, "Pct": int, "Ict": int, "Zct": int}
+    )
     nodes_properties = nodes_properties[["Tb", "PD", "QD", "Pct", "Ict", "Zct"]]
     nodes_properties.loc[0] = 1, 0.0, 0.0, PCT, ICT, ZCT  # Slack
     nodes_frame = pd.concat([nodes_, nodes_properties], axis=1)
 
     # R, X = 0.3144, 0.054
     R, X = 0.3144 / line_factor, 0.054 / line_factor
-    lines = pd.DataFrame.from_records(list(G.edges), columns=["FROM", "TO"]) + 1  # Count starts from 1
-    lines_properties = pd.DataFrame(np.tile([[R, X, 0, 1, 1]], (LINES, 1)),
-                                    columns=["R", "X", "B", "STATUS", "TAP"])
-    lines_properties = lines_properties.astype({"R": float, "X": float, "B": int, "STATUS": int, "TAP": int})
+    lines = (
+        pd.DataFrame.from_records(list(G.edges), columns=["FROM", "TO"]) + 1
+    )  # Count starts from 1
+    lines_properties = pd.DataFrame(
+        np.tile([[R, X, 0, 1, 1]], (LINES, 1)), columns=["R", "X", "B", "STATUS", "TAP"]
+    )
+    lines_properties = lines_properties.astype(
+        {"R": float, "X": float, "B": int, "STATUS": int, "TAP": int}
+    )
     lines_frame = pd.concat([lines, lines_properties], axis=1)
 
     return nodes_frame, lines_frame
 
 
 def create_pandapower_net(branch_info_: pd.DataFrame, bus_info_: pd.DataFrame):
     branch_info = branch_info_.copy()
     bus_info = bus_info_.copy()
 
     start = perf_counter()
     net = pp.create_empty_network()
     # Add buses
     bus_dict = {}
     for i, (idx, bus_name) in enumerate(bus_info["NODES"].iteritems()):
-        bus_dict[bus_name] = pp.create_bus(net, vn_kv=11., name=f"Bus {bus_name}")
+        bus_dict[bus_name] = pp.create_bus(net, vn_kv=11.0, name=f"Bus {bus_name}")
 
     # Slack
     bus_slack = bus_info[bus_info["Tb"] == 1]["NODES"].values
-    assert len(bus_slack.shape) == 1 and bus_slack.shape[0] == 1, "Only one slack bus supported"
-    pp.create_ext_grid(net, bus=bus_dict[bus_slack.item()], vm_pu=1.00, name="Grid Connection")
+    assert (
+        len(bus_slack.shape) == 1 and bus_slack.shape[0] == 1
+    ), "Only one slack bus supported"
+    pp.create_ext_grid(
+        net, bus=bus_dict[bus_slack.item()], vm_pu=1.00, name="Grid Connection"
+    )
 
     # Lines
     for i, (idx, (from_bus, to_bus, res, x_react, b_susceptance)) in enumerate(
-            branch_info[["FROM", "TO", "R", "X", "B"]].iterrows()):
-        pp.create_line_from_parameters(net,
-                                       from_bus=bus_dict[from_bus], to_bus=bus_dict[to_bus],
-                                       length_km=1, r_ohm_per_km=res, x_ohm_per_km=x_react, c_nf_per_km=b_susceptance,
-                                       max_i_ka=10, name=f"Line {i + 1}")
+        branch_info[["FROM", "TO", "R", "X", "B"]].iterrows()
+    ):
+        pp.create_line_from_parameters(
+            net,
+            from_bus=bus_dict[from_bus],
+            to_bus=bus_dict[to_bus],
+            length_km=1,
+            r_ohm_per_km=res,
+            x_ohm_per_km=x_react,
+            c_nf_per_km=b_susceptance,
+            max_i_ka=10,
+            name=f"Line {i + 1}",
+        )
 
     # Loads:
-    for i, (idx, (node, p_kw, q_kvar)) in enumerate(bus_info[["NODES", "PD", "QD"]].iterrows()):
-        pp.create_load(net, bus=bus_dict[node], p_mw=p_kw / 1000., q_mvar=q_kvar / 1000., name=f"Load")
+    for i, (idx, (node, p_kw, q_kvar)) in enumerate(
+        bus_info[["NODES", "PD", "QD"]].iterrows()
+    ):
+        pp.create_load(
+            net,
+            bus=bus_dict[node],
+            p_mw=p_kw / 1000.0,
+            q_mvar=q_kvar / 1000.0,
+            name=f"Load",
+        )
     # print(f"Create net time: {perf_counter() - start}")
 
     return net
 
+
 def net_test(net):
     """Compute the voltage for the base case using pandapower. This only works for the net of 34 buses"""
 
-    v_solution = [0.98965162 + 0.00180549j, 0.98060256 + 0.00337785j, 0.96828145 + 0.00704551j,
-                  0.95767051 + 0.01019764j, 0.94765203 + 0.01316654j, 0.94090964 + 0.01600068j,
-                  0.93719984 + 0.01754998j, 0.93283877 + 0.01937559j, 0.93073823 + 0.02026054j,
-                  0.9299309 + 0.02058985j, 0.92968994 + 0.02068728j, 0.98003142 + 0.00362498j,
-                  0.97950885 + 0.00385019j, 0.97936712 + 0.00391065j, 0.97935604 + 0.0039148j,
-                  0.93971131 + 0.01547898j, 0.93309482 + 0.01739656j, 0.92577912 + 0.01988823j,
-                  0.91988489 + 0.02188907j, 0.91475251 + 0.02362566j, 0.90888169 + 0.02596304j,
-                  0.90404908 + 0.02788248j, 0.89950353 + 0.02968449j, 0.89731375 + 0.03055177j,
-                  0.89647201 + 0.03088507j, 0.89622055 + 0.03098473j, 0.94032081 + 0.01625577j,
-                  0.93992817 + 0.01642583j, 0.93973182 + 0.01651086j, 0.9301316 + 0.02052908j,
-                  0.92952481 + 0.02079761j, 0.92922137 + 0.02093188j, 0.92912022 + 0.02097663j]
+    v_solution = [
+        0.98965162 + 0.00180549j,
+        0.98060256 + 0.00337785j,
+        0.96828145 + 0.00704551j,
+        0.95767051 + 0.01019764j,
+        0.94765203 + 0.01316654j,
+        0.94090964 + 0.01600068j,
+        0.93719984 + 0.01754998j,
+        0.93283877 + 0.01937559j,
+        0.93073823 + 0.02026054j,
+        0.9299309 + 0.02058985j,
+        0.92968994 + 0.02068728j,
+        0.98003142 + 0.00362498j,
+        0.97950885 + 0.00385019j,
+        0.97936712 + 0.00391065j,
+        0.97935604 + 0.0039148j,
+        0.93971131 + 0.01547898j,
+        0.93309482 + 0.01739656j,
+        0.92577912 + 0.01988823j,
+        0.91988489 + 0.02188907j,
+        0.91475251 + 0.02362566j,
+        0.90888169 + 0.02596304j,
+        0.90404908 + 0.02788248j,
+        0.89950353 + 0.02968449j,
+        0.89731375 + 0.03055177j,
+        0.89647201 + 0.03088507j,
+        0.89622055 + 0.03098473j,
+        0.94032081 + 0.01625577j,
+        0.93992817 + 0.01642583j,
+        0.93973182 + 0.01651086j,
+        0.9301316 + 0.02052908j,
+        0.92952481 + 0.02079761j,
+        0.92922137 + 0.02093188j,
+        0.92912022 + 0.02097663j,
+    ]
     v_solution = np.array(v_solution, dtype="complex128")
 
     for pf_algorithm in ["nr", "bfsw"]:
         print(f"Testing: {pf_algorithm} - Algorithm")
         start = perf_counter()
         if pf_algorithm == "bfsw":
-            pp.runpp(net, algorithm=pf_algorithm, numba=False, v_debug=True, VERBOSE=False, tolerance_mva=1e-6)
-            print(f"BFSW. Iterations: {net._ppc['iterations']}. PF time: {net._ppc['et']}")
+            pp.runpp(
+                net,
+                algorithm=pf_algorithm,
+                numba=False,
+                v_debug=True,
+                VERBOSE=False,
+                tolerance_mva=1e-6,
+            )
+            print(
+                f"BFSW. Iterations: {net._ppc['iterations']}. PF time: {net._ppc['et']}"
+            )
         elif pf_algorithm == "nr":
-            pp.runpp(net, algorithm=pf_algorithm, numba=False, v_debug=True, VERBOSE=False, tolerance_mva=1e-6)
-            print(f"NR. Iterations: {net._ppc['iterations']}. PF time: {net._ppc['et']}")
+            pp.runpp(
+                net,
+                algorithm=pf_algorithm,
+                numba=False,
+                v_debug=True,
+                VERBOSE=False,
+                tolerance_mva=1e-6,
+            )
+            print(
+                f"NR. Iterations: {net._ppc['iterations']}. PF time: {net._ppc['et']}"
+            )
         print(f"Total pf time: {perf_counter() - start}.")
 
-        v_real = net.res_bus["vm_pu"].values * np.cos(np.deg2rad(net.res_bus["va_degree"].values))
-        v_img = net.res_bus["vm_pu"].values * np.sin(np.deg2rad(net.res_bus["va_degree"].values))
+        v_real = net.res_bus["vm_pu"].values * np.cos(
+            np.deg2rad(net.res_bus["va_degree"].values)
+        )
+        v_img = net.res_bus["vm_pu"].values * np.sin(
+            np.deg2rad(net.res_bus["va_degree"].values)
+        )
         v_result = v_real + 1j * v_img
         assert np.allclose(v_result[1:], v_solution)
         print("Test OK.")
 
     return True
 
+
 if __name__ == "__main__":
     _load_default_34_node_case()
-
```

### Comparing `tensorpowerflow-0.0.5/tensorpowerflow.egg-info/PKG-INFO` & `tensorpowerflow-0.0.7/tensorpowerflow.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,134 +1,129 @@
-Metadata-Version: 2.1
-Name: tensorpowerflow
-Version: 0.0.5
-Summary: Ultra fast power flow based in Laurent series expansion.
-Author-email: e.m.salazar.duque@tue.nl
-License: MIT
-Project-URL: repository, https://github.com/MauricioSalazare/tensorpowerflow
-Keywords: power flow,power systems,time series loading
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.0
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-Provides-Extra: test
-Provides-Extra: doc
-License-File: LICENSE
-
-.. Binder
-.. image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/MauricioSalazare/tensorpowerflow/master?urlpath=lab/tree/examples
-   :alt: binder
-
-.. License
-.. image:: https://img.shields.io/github/license/MauricioSalazare/tensorpowerflow
-   :target: https://github.com/MauricioSalazare/tensorpowerflow/blob/master/LICENSE
-
-.. Python versions supported
-.. image:: https://img.shields.io/pypi/pyversions/tensorpowerflow.svg
-   :target: https://pypi.python.org/pypi/tensorpowerflow/
-
-.. Downloads per month
-.. image:: https://img.shields.io/pypi/dm/tensorpowerflow.svg
-   :target: https://pypi.python.org/pypi/tensorpowerflow/
-
-.. Code size
-.. image:: https://img.shields.io/github/languages/code-size/MauricioSalazare/tensorpowerflow
-   :target: https://github.com/MauricioSalazare/tensorpowerflow
-
-.. PyPi version
-.. image:: https://img.shields.io/pypi/v/tensorpowerflow
-   :target: https://pypi.python.org/pypi/tensorpowerflow/
-
-.. Build (GithubActions)
-.. image:: https://img.shields.io/github/workflow/status/MauricioSalazare/tensorpowerflow/Python%20package/master
-   :target: https://github.com/MauricioSalazare/tensorpowerflow/actions
-
-.. Test (GithubActions)
-.. image:: https://img.shields.io/github/workflow/status/MauricioSalazare/tensorpowerflow/Python%20package/master?label=tests
-   :target: https://github.com/MauricioSalazare/tensorpowerflow/actions
-
-
-
-
-TensorPowerFlow
-===============
-
-
-What is TensorPowerFlow?
-------------------------
-
-An ultra-fast power flow based on Laurent series expansion. The power flow is intended for applications where massive
-amounts of power flow computations are required. e.g., electrical load time series, metaheuristics, electrical grid
-environments for reinforcement learning.
-
-How to install
---------------
-The package can be installed via pip using:
-
-.. code:: shell
-
-    pip install tensorpowerflow
-
-Example:
---------
-Run the load base case as:
-
-.. code-block:: python
-
-    from tensorpowerflow import GridTensor
-    import numpy as np
-    from time import perf_counter
-
-    #%% Solve base case (34 node bus)
-    network = GridTensor()
-    solution = network.run_pf()
-    print(solution["v"])
-
-    #%% Solve 10_000 power flows on the 34 node bus case.
-    network_size = network.nb - 1  # Size of network without slack bus.
-    active_ns = np.random.normal(50, scale=1, size=(10_000, network_size)) # Power in kW
-    reactive_ns = active_ns * 0.1  # kVAr
-    solution_tensor = network.run_pf(active_power=active_ns, reactive_power=reactive_ns)
-    print(solution_tensor["v"])
-
-    #%% Generate random radial network of 100 nodes and a maximum of 1 to 3 branches per node.
-    network_rnd = GridTensor.generate_from_graph(nodes=100, child=3, plot_graph=True)
-    solution_rnd = network_rnd.run_pf()
-    print(solution_rnd["v"])
-
-    #%% Solve a tensor power flow. For 10 scenarios, 8_760 time steps (one year - 1 hr res), for the 33 PQ nodes.
-    # Meaning that the dimensions of the tensor is (10, 8_760, 33)
-
-    network = GridTensor(numba=True)  # Loads the basic 34 bus node network.
-    active_ns = np.random.normal(50,  # Power in kW
-                                 scale=10,
-                                 size=(10, 8_760, 33)).round(3)  # Assume 1 slack variable
-    reactive_ns = (active_ns * .1).round(3)  # Constant PF of 0.1
-
-    start_tensor_dense = perf_counter()
-    solution = network.run_pf(active_power=active_ns, reactive_power=reactive_ns, algorithm="tensor")
-    t_tensor_dense = perf_counter() - start_tensor_dense
-    assert solution["convergence"], "Algorithm did not converge."
-    assert solution["v"].shape == active_ns.shape
-    print(f"Time tensor dense: {t_tensor_dense:.3f} sec.")
-
-More examples can be found in the `examples folder <https://github.com/MauricioSalazare/tensorpowerflow/tree/master/examples>`_ (under development).
-Also, you can try the package via jupyter lab clicking in the binder icon:
-
-.. image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/MauricioSalazare/tensorpowerflow/master?urlpath=lab/tree/examples
-   :alt: binder
-
-Reading and citations:
-----------------------
-The mathematical formulation of the power flow can be found at:
-
-*"A Fixed-Point Current Injection Power Flow for Electric Distribution Systems using Laurent Series."* J.S. Giraldo,
-O.D. Montoya, P.P. Vergara, F. Milano. Power Systems Computational Conference (PSCC) 2022. `link <http://faraday1.ucd.ie/archive/papers/laurent.pdf>`_
-
-
-How to contact us
------------------
-Any questions, suggestions or collaborations contact Juan S. Giraldo at <jnse@ieee.org>
+Metadata-Version: 2.1
+Name: tensorpowerflow
+Version: 0.0.7
+Summary: Ultra fast power flow based in Laurent series expansion.
+Author-email: Mauricio Salazar <e.m.salazar.duque@tue.nl>
+License: MIT
+Project-URL: repository, https://github.com/MauricioSalazare/tensorpowerflow
+Keywords: power flow,power systems,time series loading
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: scipy
+Requires-Dist: tqdm
+Requires-Dist: numba>=0.53.0
+Requires-Dist: networkx
+Requires-Dist: seaborn
+Requires-Dist: pandapower
+Requires-Dist: mkl; platform_system != "Darwin"
+Requires-Dist: psutil
+Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: matplotlib; extra == "dev"
+Requires-Dist: jupyterlab; extra == "dev"
+Requires-Dist: tox; extra == "dev"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Provides-Extra: doc
+Requires-Dist: sphinx; extra == "doc"
+
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/MauricioSalazare/tensorpowerflow/master?urlpath=lab/tree/examples)
+[![MIT License](https://img.shields.io/badge/License-MIT-yellow)](https://github.com/MauricioSalazare/tensorpowerflow/blob/master/LICENSE)
+[![Python versions supported](https://img.shields.io/pypi/pyversions/tensorpowerflow.svg)](https://pypi.python.org/pypi/tensorpowerflow/)
+[![Downloads per month](https://img.shields.io/pypi/dm/tensorpowerflow.svg)](https://pypi.python.org/pypi/tensorpowerflow/)
+[![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/MauricioSalazare/tensorpowerflow)](https://github.com/MauricioSalazare/tensorpowerflow)
+[![PyPI - Version](https://img.shields.io/pypi/v/tensorpowerflow)](https://pypi.python.org/pypi/tensorpowerflow/)
+[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/MauricioSalazare/tensorpowerflow/python-package.yml)](https://github.com/MauricioSalazare/tensorpowerflow/actions)
+
+
+# TensorPowerFlow
+
+## What is TensorPowerFlow?
+An ultra-fast power flow based on a fixed-point iteration algorithm. The power flow is intended for applications requiring massive
+amounts of power flow computations. e.g., electrical load time series, metaheuristics, and electrical grid
+environments for reinforcement learning.
+
+## How to install
+
+The package can be installed via pip using:
+
+```shell
+pip install tensorpowerflow
+```
+
+## Example:
+
+Here we show four examples of what can be done with the packages:
+1. *Example 1:* The package comes with a preloaded network case of 34 nodes that can be solved by default. 
+2. *Example 2:* Solve 10.000 PF for the default network case. The active power for the nodes is generated by sampling a Normal 
+    distribution.
+3. *Example 3:* The GridTensor class can generate a random grid using the `GridTensor.generate_from_graph()` method.
+    The parameters `nodes` and `child`, respectively, can control the number of nodes and branching per node.
+4. *Example 4:* We test the grid with a tensor of 3 dimensions. The first dimension is the number of scenarios 
+    (10 in the example). The second dimension is the number of time steps (8.760 to simulate a 30-minute resolution 
+    consumption for one year). The third dimension is the number of PQ nodes in the grid (33 PQ nodes for the base 
+    grid case).
+
+```python
+from tensorpowerflow import GridTensor
+import numpy as np
+from time import perf_counter
+
+#%% Example 1: Solve base case (34 node bus)
+network = GridTensor(gpu_mode=False)
+solution = network.run_pf()
+print(solution["v"])
+
+#%% Example 2: Solve 10_000 power flows on the 34 node bus network case.
+network_size = network.nb - 1 # Size of the network without the slack bus.
+active_ns = np.random.normal(50, scale=1, size=(10_000, network_size)) # Power in kW
+reactive_ns = active_ns * 0.1  # kVAr
+solution_tensor = network.run_pf(active_power=active_ns, reactive_power=reactive_ns)
+print(solution_tensor["v"])
+
+#%% Example 3: Generate a random radial network of 100 nodes and a maximum of 1 to 3 branches per node.
+network_rnd = GridTensor.generate_from_graph(nodes=100, child=3, plot_graph=True)
+solution_rnd = network_rnd.run_pf()
+print(solution_rnd["v"])
+
+#%% Example 4: Solve a tensor power flow. For 10 scenarios, 8_760 time steps (one year - 1 hr res) for the 33 PQ nodes.
+# Meaning that the dimensions of the tensor are (10, 8_760, 33)
+
+network = GridTensor(numba=True)  # Loads the basic 34 bus node network.
+active_ns = np.random.normal(50,  # Power in kW
+                             scale=10,
+                             size=(10, 8_760, 33)).round(3)  # Assume 1 slack variable
+reactive_ns = (active_ns * .1).round(3)  # Constant PF of 0.1
+
+start_tensor_dense = perf_counter()
+solution = network.run_pf(active_power=active_ns, reactive_power=reactive_ns, algorithm="tensor")
+t_tensor_dense = perf_counter() - start_tensor_dense
+assert solution["convergence"], "Algorithm did not converge."
+assert solution["v"].shape == active_ns.shape
+print(f"Time tensor dense: {t_tensor_dense:.3f} sec.")
+
+
+```
+
+More examples can be found in the [examples folder](examples) (under development).
+Also, you can try the package via Jupyter lab by clicking on the binder icon:
+
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/MauricioSalazare/tensorpowerflow/master?urlpath=lab/tree/examples)
+
+## Reading and citations:
+
+The mathematical formulation of the power flow can be found at:
+
+> *"Tensor Power Flow Formulations for Multidimensional Analyses in Distribution Systems."* E.M. Salazar Duque,
+Juan S. Giraldo, Pedro P. Vergara, Phuong H. Nguyen, and Han (J.G.) Slootweg. [arXiv:2403.04578 (2024)](https://arxiv.org/pdf/2403.04578).
+
+## How to contact us
+
+For any questions, suggestions or collaborations, contact Juan S. Giraldo at <jnse@ieee.org>
```

### Comparing `tensorpowerflow-0.0.5/tensorpowerflow.egg-info/SOURCES.txt` & `tensorpowerflow-0.0.7/tensorpowerflow.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE
 MANIFEST.in
-README.rst
+README.md
 pyproject.toml
 setup.py
 tensorpowerflow/__init__.py
 tensorpowerflow/grid.py
 tensorpowerflow/numbarize.py
 tensorpowerflow/utils.py
 tensorpowerflow.egg-info/PKG-INFO
@@ -20,13 +20,13 @@
 tensorpowerflow/gpu_tensor/gpu_interface.py
 tensorpowerflow/pyMKL/MKLutils.py
 tensorpowerflow/pyMKL/README.txt
 tensorpowerflow/pyMKL/__init__.py
 tensorpowerflow/pyMKL/loadMKL.py
 tensorpowerflow/pyMKL/pardisoInterface.py
 tensorpowerflow/pyMKL/pardisoSolver.py
-tensorpowerflow/pyMKL/Tests/test_MKLUtils.py
-tensorpowerflow/pyMKL/Tests/test_Pardiso.py
+tensorpowerflow/pyMKL/Tests/trial_MKLUtils.py
+tensorpowerflow/pyMKL/Tests/trial_Pardiso.py
 tensorpowerflow/tests/__init__.py
 tensorpowerflow/tests/test_powerflows.py
 tensorpowerflow/tests/test_powerflows_pardiso_gpu.py
 tensorpowerflow/tests/test_tensor_power_flow.py
```

