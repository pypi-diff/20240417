# Comparing `tmp/qtealeaves-0.5.13.tar.gz` & `tmp/qtealeaves-0.5.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtealeaves-0.5.13.tar", last modified: Mon Feb 26 14:55:26 2024, max compression
+gzip compressed data, was "qtealeaves-0.5.14.tar", last modified: Wed Apr 17 12:37:20 2024, max compression
```

## Comparing `qtealeaves-0.5.13.tar` & `qtealeaves-0.5.14.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-02-26 14:55:26.325085 qtealeaves-0.5.13/
--rw-r--r--   0 quantum    (128) quantum    (128)    10764 2022-11-30 17:54:07.000000 qtealeaves-0.5.13/LICENSE
--rw-r--r--   0 quantum    (128) quantum    (128)     3286 2024-02-26 14:55:26.325085 qtealeaves-0.5.13/PKG-INFO
--rw-r--r--   0 quantum    (128) quantum    (128)     2572 2023-12-13 17:32:06.000000 qtealeaves-0.5.13/README.md
--rw-r--r--   0 quantum    (128) quantum    (128)       42 2022-11-30 17:54:07.000000 qtealeaves-0.5.13/pyproject.toml
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-02-26 14:55:26.317085 qtealeaves-0.5.13/qtealeaves/
--rw-r--r--   0 quantum    (128) quantum    (128)     1222 2022-11-30 17:54:07.000000 qtealeaves-0.5.13/qtealeaves/__init__.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-02-26 14:55:26.317085 qtealeaves-0.5.13/qtealeaves/convergence_parameters/
--rw-r--r--   0 quantum    (128) quantum    (128)      758 2022-11-30 17:54:07.000000 qtealeaves-0.5.13/qtealeaves/convergence_parameters/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)    14801 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/qtealeaves/convergence_parameters/conv_params.py
--rw-r--r--   0 quantum    (128) quantum    (128)     6745 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/qtealeaves/convergence_parameters/conv_params_finite_temp.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-02-26 14:55:26.321085 qtealeaves-0.5.13/qtealeaves/emulator/
--rw-r--r--   0 quantum    (128) quantum    (128)     1098 2023-10-26 07:55:27.000000 qtealeaves-0.5.13/qtealeaves/emulator/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)    75181 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/qtealeaves/emulator/abstract_tn.py
--rw-r--r--   0 quantum    (128) quantum    (128)     7902 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/qtealeaves/emulator/ed_simulation.py
--rw-r--r--   0 quantum    (128) quantum    (128)    35555 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/qtealeaves/emulator/lptn_simulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)    19885 2023-10-26 07:55:27.000000 qtealeaves-0.5.13/qtealeaves/emulator/mpi_mps_simulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)    83620 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/qtealeaves/emulator/mps_simulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)    16308 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/qtealeaves/emulator/state_simulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)   149524 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/qtealeaves/emulator/ttn_simulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)    45441 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/qtealeaves/emulator/tto_simulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)    17831 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/qtealeaves/fortran_interfaces.py
--rw-r--r--   0 quantum    (128) quantum    (128)    47759 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/qtealeaves/hilbert_curvature.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5854 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/qtealeaves/lattice_layout.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-02-26 14:55:26.321085 qtealeaves-0.5.13/qtealeaves/modeling/
--rw-r--r--   0 quantum    (128) quantum    (128)     1381 2024-02-26 14:53:18.000000 qtealeaves-0.5.13/qtealeaves/modeling/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)     6102 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/qtealeaves/modeling/baseterm.py
--rw-r--r--   0 quantum    (128) quantum    (128)     7597 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/qtealeaves/modeling/blockterm2d.py
--rw-r--r--   0 quantum    (128) quantum    (128)    13591 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/qtealeaves/modeling/localterm.py
--rw-r--r--   0 quantum    (128) quantum    (128)     7351 2023-10-26 07:55:27.000000 qtealeaves-0.5.13/qtealeaves/modeling/plaquetteterm2d.py
--rw-r--r--   0 quantum    (128) quantum    (128)    27889 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/qtealeaves/modeling/quantummodel.py
--rw-r--r--   0 quantum    (128) quantum    (128)     9928 2023-10-26 07:55:27.000000 qtealeaves-0.5.13/qtealeaves/modeling/sparsematrixoperator.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2566 2023-10-26 07:55:27.000000 qtealeaves-0.5.13/qtealeaves/modeling/sparsematrixproductoperator.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5632 2024-02-26 14:53:18.000000 qtealeaves-0.5.13/qtealeaves/modeling/stringterm1d.py
--rw-r--r--   0 quantum    (128) quantum    (128)     8769 2024-02-26 14:53:18.000000 qtealeaves-0.5.13/qtealeaves/modeling/tensorproductoperator.py
--rw-r--r--   0 quantum    (128) quantum    (128)    12414 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/qtealeaves/modeling/twobodyterm1d.py
--rw-r--r--   0 quantum    (128) quantum    (128)    13003 2022-11-30 17:54:07.000000 qtealeaves-0.5.13/qtealeaves/modeling/twobodyterm2d.py
--rw-r--r--   0 quantum    (128) quantum    (128)    10416 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/qtealeaves/modeling/twobodyterm3d.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-02-26 14:55:26.321085 qtealeaves-0.5.13/qtealeaves/models/
--rw-r--r--   0 quantum    (128) quantum    (128)      766 2022-11-30 17:54:07.000000 qtealeaves-0.5.13/qtealeaves/models/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2720 2022-11-30 17:54:07.000000 qtealeaves-0.5.13/qtealeaves/models/bosehubbard.py
--rw-r--r--   0 quantum    (128) quantum    (128)     4682 2023-10-26 07:55:27.000000 qtealeaves-0.5.13/qtealeaves/models/quantumising.py
--rw-r--r--   0 quantum    (128) quantum    (128)     1736 2022-11-30 17:54:07.000000 qtealeaves-0.5.13/qtealeaves/models/xxzmodel.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-02-26 14:55:26.321085 qtealeaves-0.5.13/qtealeaves/observables/
--rw-r--r--   0 quantum    (128) quantum    (128)     1530 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/qtealeaves/observables/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5892 2023-10-26 07:55:27.000000 qtealeaves-0.5.13/qtealeaves/observables/bond_entropy.py
--rw-r--r--   0 quantum    (128) quantum    (128)    13865 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/qtealeaves/observables/correlation.py
--rw-r--r--   0 quantum    (128) quantum    (128)    12681 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/qtealeaves/observables/custom_correlation.py
--rw-r--r--   0 quantum    (128) quantum    (128)     4688 2023-10-26 07:55:27.000000 qtealeaves-0.5.13/qtealeaves/observables/distance2pure.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5853 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/qtealeaves/observables/local.py
--rw-r--r--   0 quantum    (128) quantum    (128)     7296 2023-10-26 07:55:27.000000 qtealeaves-0.5.13/qtealeaves/observables/probabilities.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5172 2023-10-26 07:55:27.000000 qtealeaves-0.5.13/qtealeaves/observables/projective.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5098 2023-10-26 07:55:27.000000 qtealeaves-0.5.13/qtealeaves/observables/state2file.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5821 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/qtealeaves/observables/tensor_product.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5595 2023-10-26 07:55:27.000000 qtealeaves-0.5.13/qtealeaves/observables/timecorrelator.py
--rw-r--r--   0 quantum    (128) quantum    (128)     6348 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/qtealeaves/observables/tnobase.py
--rw-r--r--   0 quantum    (128) quantum    (128)    18241 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/qtealeaves/observables/tnobservables.py
--rw-r--r--   0 quantum    (128) quantum    (128)     7681 2023-10-26 07:55:27.000000 qtealeaves-0.5.13/qtealeaves/observables/weighted_sum.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-02-26 14:55:26.321085 qtealeaves-0.5.13/qtealeaves/operators/
--rw-r--r--   0 quantum    (128) quantum    (128)     1004 2023-10-26 07:55:27.000000 qtealeaves-0.5.13/qtealeaves/operators/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2904 2022-11-30 17:54:07.000000 qtealeaves-0.5.13/qtealeaves/operators/bosonicoperators.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2622 2023-10-26 07:55:27.000000 qtealeaves-0.5.13/qtealeaves/operators/combinedoperators.py
--rw-r--r--   0 quantum    (128) quantum    (128)     4143 2022-11-30 17:54:07.000000 qtealeaves-0.5.13/qtealeaves/operators/quditoperators.py
--rw-r--r--   0 quantum    (128) quantum    (128)     1358 2022-11-30 17:54:07.000000 qtealeaves-0.5.13/qtealeaves/operators/spinoperators.py
--rw-r--r--   0 quantum    (128) quantum    (128)     8367 2022-11-30 17:54:07.000000 qtealeaves-0.5.13/qtealeaves/operators/tnoperators.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2856 2022-11-30 17:54:07.000000 qtealeaves-0.5.13/qtealeaves/parameterized.py
--rw-r--r--   0 quantum    (128) quantum    (128)    60390 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/qtealeaves/simulation_setup.py
--rw-r--r--   0 quantum    (128) quantum    (128)      532 2024-02-26 14:53:18.000000 qtealeaves-0.5.13/qtealeaves/version.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-02-26 14:55:26.325085 qtealeaves-0.5.13/qtealeaves.egg-info/
--rw-r--r--   0 quantum    (128) quantum    (128)     3286 2024-02-26 14:55:26.000000 qtealeaves-0.5.13/qtealeaves.egg-info/PKG-INFO
--rw-r--r--   0 quantum    (128) quantum    (128)     2608 2024-02-26 14:55:26.000000 qtealeaves-0.5.13/qtealeaves.egg-info/SOURCES.txt
--rw-r--r--   0 quantum    (128) quantum    (128)        1 2024-02-26 14:55:26.000000 qtealeaves-0.5.13/qtealeaves.egg-info/dependency_links.txt
--rw-r--r--   0 quantum    (128) quantum    (128)       42 2024-02-26 14:55:26.000000 qtealeaves-0.5.13/qtealeaves.egg-info/requires.txt
--rw-r--r--   0 quantum    (128) quantum    (128)       11 2024-02-26 14:55:26.000000 qtealeaves-0.5.13/qtealeaves.egg-info/top_level.txt
--rw-r--r--   0 quantum    (128) quantum    (128)       38 2024-02-26 14:55:26.325085 qtealeaves-0.5.13/setup.cfg
--rw-r--r--   0 quantum    (128) quantum    (128)     2660 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/setup.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-02-26 14:55:26.325085 qtealeaves-0.5.13/tests/
--rw-r--r--   0 quantum    (128) quantum    (128)     1332 2022-11-30 17:54:07.000000 qtealeaves-0.5.13/tests/tests_formatting.py
--rw-r--r--   0 quantum    (128) quantum    (128)     1504 2023-10-26 07:55:27.000000 qtealeaves-0.5.13/tests/tests_fortran_interface.py
--rw-r--r--   0 quantum    (128) quantum    (128)     9311 2023-10-26 07:55:27.000000 qtealeaves-0.5.13/tests/tests_hilbert_curvature.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2739 2022-11-30 17:54:07.000000 qtealeaves-0.5.13/tests/tests_lattice_layout.py
--rw-r--r--   0 quantum    (128) quantum    (128)    24306 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/tests/tests_linter.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5818 2023-10-26 07:55:27.000000 qtealeaves-0.5.13/tests/tests_model_terms.py
--rw-r--r--   0 quantum    (128) quantum    (128)     1858 2023-01-26 15:54:33.000000 qtealeaves-0.5.13/tests/tests_operators.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2785 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/tests/tests_quantum_trajectories.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2553 2022-11-30 17:54:07.000000 qtealeaves-0.5.13/tests/tests_rydberg_model.py
--rw-r--r--   0 quantum    (128) quantum    (128)     4429 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/tests/tests_simulation_setup.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5531 2024-01-12 22:24:30.000000 qtealeaves-0.5.13/tests/tests_ttn_simulation.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-17 12:37:20.027526 qtealeaves-0.5.14/
+-rw-r--r--   0 quantum    (128) quantum    (128)    10764 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/LICENSE
+-rw-r--r--   0 quantum    (128) quantum    (128)     3286 2024-04-17 12:37:20.027526 qtealeaves-0.5.14/PKG-INFO
+-rw-r--r--   0 quantum    (128) quantum    (128)     2572 2023-12-13 17:32:06.000000 qtealeaves-0.5.14/README.md
+-rw-r--r--   0 quantum    (128) quantum    (128)       42 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/pyproject.toml
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-17 12:37:20.019526 qtealeaves-0.5.14/qtealeaves/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1222 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/qtealeaves/__init__.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-17 12:37:20.019526 qtealeaves-0.5.14/qtealeaves/convergence_parameters/
+-rw-r--r--   0 quantum    (128) quantum    (128)      758 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/qtealeaves/convergence_parameters/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    14801 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/convergence_parameters/conv_params.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     6745 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/convergence_parameters/conv_params_finite_temp.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-17 12:37:20.019526 qtealeaves-0.5.14/qtealeaves/emulator/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1098 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/emulator/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    75181 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/emulator/abstract_tn.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     7902 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/emulator/ed_simulation.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    35555 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/emulator/lptn_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    19885 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/emulator/mpi_mps_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    83620 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/emulator/mps_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    16308 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/emulator/state_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)   149524 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/emulator/ttn_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    45441 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/emulator/tto_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    17831 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/fortran_interfaces.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    47759 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/hilbert_curvature.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5854 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/lattice_layout.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-17 12:37:20.023526 qtealeaves-0.5.14/qtealeaves/modeling/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1381 2024-02-26 14:55:43.000000 qtealeaves-0.5.14/qtealeaves/modeling/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     6102 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/modeling/baseterm.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     7597 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/modeling/blockterm2d.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    13591 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/modeling/localterm.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     7351 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/modeling/plaquetteterm2d.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    27889 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/modeling/quantummodel.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     9928 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/modeling/sparsematrixoperator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2566 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/modeling/sparsematrixproductoperator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5632 2024-02-26 14:55:43.000000 qtealeaves-0.5.14/qtealeaves/modeling/stringterm1d.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     8769 2024-02-26 14:55:43.000000 qtealeaves-0.5.14/qtealeaves/modeling/tensorproductoperator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    12414 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/modeling/twobodyterm1d.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    13003 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/qtealeaves/modeling/twobodyterm2d.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    10416 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/modeling/twobodyterm3d.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-17 12:37:20.023526 qtealeaves-0.5.14/qtealeaves/models/
+-rw-r--r--   0 quantum    (128) quantum    (128)      766 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/qtealeaves/models/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2720 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/qtealeaves/models/bosehubbard.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     4682 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/models/quantumising.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1736 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/qtealeaves/models/xxzmodel.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-17 12:37:20.023526 qtealeaves-0.5.14/qtealeaves/observables/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1530 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/observables/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5892 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/observables/bond_entropy.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    13865 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/observables/correlation.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    12681 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/observables/custom_correlation.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     4688 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/observables/distance2pure.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5853 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/observables/local.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     7296 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/observables/probabilities.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5172 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/observables/projective.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5098 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/observables/state2file.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5821 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/observables/tensor_product.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5595 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/observables/timecorrelator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     6348 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/observables/tnobase.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    18241 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/observables/tnobservables.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     7681 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/observables/weighted_sum.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-17 12:37:20.023526 qtealeaves-0.5.14/qtealeaves/operators/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1004 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/operators/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2904 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/qtealeaves/operators/bosonicoperators.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2622 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/operators/combinedoperators.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     4143 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/qtealeaves/operators/quditoperators.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1358 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/qtealeaves/operators/spinoperators.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     8367 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/qtealeaves/operators/tnoperators.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2856 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/qtealeaves/parameterized.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    60390 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/simulation_setup.py
+-rw-r--r--   0 quantum    (128) quantum    (128)      532 2024-04-17 12:35:13.000000 qtealeaves-0.5.14/qtealeaves/version.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-17 12:37:20.023526 qtealeaves-0.5.14/qtealeaves.egg-info/
+-rw-r--r--   0 quantum    (128) quantum    (128)     3286 2024-04-17 12:37:20.000000 qtealeaves-0.5.14/qtealeaves.egg-info/PKG-INFO
+-rw-r--r--   0 quantum    (128) quantum    (128)     2608 2024-04-17 12:37:20.000000 qtealeaves-0.5.14/qtealeaves.egg-info/SOURCES.txt
+-rw-r--r--   0 quantum    (128) quantum    (128)        1 2024-04-17 12:37:20.000000 qtealeaves-0.5.14/qtealeaves.egg-info/dependency_links.txt
+-rw-r--r--   0 quantum    (128) quantum    (128)       42 2024-04-17 12:37:20.000000 qtealeaves-0.5.14/qtealeaves.egg-info/requires.txt
+-rw-r--r--   0 quantum    (128) quantum    (128)       11 2024-04-17 12:37:20.000000 qtealeaves-0.5.14/qtealeaves.egg-info/top_level.txt
+-rw-r--r--   0 quantum    (128) quantum    (128)       38 2024-04-17 12:37:20.027526 qtealeaves-0.5.14/setup.cfg
+-rw-r--r--   0 quantum    (128) quantum    (128)     2660 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/setup.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-17 12:37:20.023526 qtealeaves-0.5.14/tests/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1332 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/tests/tests_formatting.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1504 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/tests/tests_fortran_interface.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     9311 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/tests/tests_hilbert_curvature.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2739 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/tests/tests_lattice_layout.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    24306 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/tests/tests_linter.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5818 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/tests/tests_model_terms.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1858 2023-01-26 15:54:33.000000 qtealeaves-0.5.14/tests/tests_operators.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2785 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/tests/tests_quantum_trajectories.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2553 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/tests/tests_rydberg_model.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     4429 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/tests/tests_simulation_setup.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5531 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/tests/tests_ttn_simulation.py
```

### Comparing `qtealeaves-0.5.13/LICENSE` & `qtealeaves-0.5.14/LICENSE`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/PKG-INFO` & `qtealeaves-0.5.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtealeaves
-Version: 0.5.13
+Version: 0.5.14
 Summary: Quantum TEA's python tensor network library
 Home-page: https://baltig.infn.it/quantum_tea_leaves/py_api_quantum_tea_leaves.git
 Author: Marco Ballarin, Giovanni Cataldi, Aurora Costantini, Daniel Jaschke, Giuseppe Magnifico, Simone Notarnicola, Alice Pagano, Luka Pavesic, Marco Rigobello, Nora Reinić, Simone Scarlatella
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `qtealeaves-0.5.13/README.md` & `qtealeaves-0.5.14/README.md`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/__init__.py` & `qtealeaves-0.5.14/qtealeaves/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/convergence_parameters/__init__.py` & `qtealeaves-0.5.14/qtealeaves/convergence_parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/convergence_parameters/conv_params.py` & `qtealeaves-0.5.14/qtealeaves/convergence_parameters/conv_params.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/convergence_parameters/conv_params_finite_temp.py` & `qtealeaves-0.5.14/qtealeaves/convergence_parameters/conv_params_finite_temp.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/emulator/__init__.py` & `qtealeaves-0.5.14/qtealeaves/emulator/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/emulator/abstract_tn.py` & `qtealeaves-0.5.14/qtealeaves/emulator/abstract_tn.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/emulator/ed_simulation.py` & `qtealeaves-0.5.14/qtealeaves/emulator/ed_simulation.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/emulator/lptn_simulator.py` & `qtealeaves-0.5.14/qtealeaves/emulator/lptn_simulator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/emulator/mpi_mps_simulator.py` & `qtealeaves-0.5.14/qtealeaves/emulator/mpi_mps_simulator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/emulator/mps_simulator.py` & `qtealeaves-0.5.14/qtealeaves/emulator/mps_simulator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/emulator/state_simulator.py` & `qtealeaves-0.5.14/qtealeaves/emulator/state_simulator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/emulator/ttn_simulator.py` & `qtealeaves-0.5.14/qtealeaves/emulator/ttn_simulator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/emulator/tto_simulator.py` & `qtealeaves-0.5.14/qtealeaves/emulator/tto_simulator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/fortran_interfaces.py` & `qtealeaves-0.5.14/qtealeaves/fortran_interfaces.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/hilbert_curvature.py` & `qtealeaves-0.5.14/qtealeaves/hilbert_curvature.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/lattice_layout.py` & `qtealeaves-0.5.14/qtealeaves/lattice_layout.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/modeling/__init__.py` & `qtealeaves-0.5.14/qtealeaves/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/modeling/baseterm.py` & `qtealeaves-0.5.14/qtealeaves/modeling/baseterm.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/modeling/blockterm2d.py` & `qtealeaves-0.5.14/qtealeaves/modeling/blockterm2d.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/modeling/localterm.py` & `qtealeaves-0.5.14/qtealeaves/modeling/localterm.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/modeling/plaquetteterm2d.py` & `qtealeaves-0.5.14/qtealeaves/modeling/plaquetteterm2d.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/modeling/quantummodel.py` & `qtealeaves-0.5.14/qtealeaves/modeling/quantummodel.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/modeling/sparsematrixoperator.py` & `qtealeaves-0.5.14/qtealeaves/modeling/sparsematrixoperator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/modeling/sparsematrixproductoperator.py` & `qtealeaves-0.5.14/qtealeaves/modeling/sparsematrixproductoperator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/modeling/stringterm1d.py` & `qtealeaves-0.5.14/qtealeaves/modeling/stringterm1d.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/modeling/tensorproductoperator.py` & `qtealeaves-0.5.14/qtealeaves/modeling/tensorproductoperator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/modeling/twobodyterm1d.py` & `qtealeaves-0.5.14/qtealeaves/modeling/twobodyterm1d.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/modeling/twobodyterm2d.py` & `qtealeaves-0.5.14/qtealeaves/modeling/twobodyterm2d.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/modeling/twobodyterm3d.py` & `qtealeaves-0.5.14/qtealeaves/modeling/twobodyterm3d.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/models/__init__.py` & `qtealeaves-0.5.14/qtealeaves/models/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/models/bosehubbard.py` & `qtealeaves-0.5.14/qtealeaves/models/bosehubbard.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/models/quantumising.py` & `qtealeaves-0.5.14/qtealeaves/models/quantumising.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/models/xxzmodel.py` & `qtealeaves-0.5.14/qtealeaves/models/xxzmodel.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/observables/__init__.py` & `qtealeaves-0.5.14/qtealeaves/observables/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/observables/bond_entropy.py` & `qtealeaves-0.5.14/qtealeaves/observables/bond_entropy.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/observables/correlation.py` & `qtealeaves-0.5.14/qtealeaves/observables/correlation.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/observables/custom_correlation.py` & `qtealeaves-0.5.14/qtealeaves/observables/custom_correlation.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/observables/distance2pure.py` & `qtealeaves-0.5.14/qtealeaves/observables/distance2pure.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/observables/local.py` & `qtealeaves-0.5.14/qtealeaves/observables/local.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/observables/probabilities.py` & `qtealeaves-0.5.14/qtealeaves/observables/probabilities.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/observables/projective.py` & `qtealeaves-0.5.14/qtealeaves/observables/projective.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/observables/state2file.py` & `qtealeaves-0.5.14/qtealeaves/observables/state2file.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/observables/tensor_product.py` & `qtealeaves-0.5.14/qtealeaves/observables/tensor_product.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/observables/timecorrelator.py` & `qtealeaves-0.5.14/qtealeaves/observables/timecorrelator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/observables/tnobase.py` & `qtealeaves-0.5.14/qtealeaves/observables/tnobase.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/observables/tnobservables.py` & `qtealeaves-0.5.14/qtealeaves/observables/tnobservables.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/observables/weighted_sum.py` & `qtealeaves-0.5.14/qtealeaves/observables/weighted_sum.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/operators/__init__.py` & `qtealeaves-0.5.14/qtealeaves/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/operators/bosonicoperators.py` & `qtealeaves-0.5.14/qtealeaves/operators/bosonicoperators.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/operators/combinedoperators.py` & `qtealeaves-0.5.14/qtealeaves/operators/combinedoperators.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/operators/quditoperators.py` & `qtealeaves-0.5.14/qtealeaves/operators/quditoperators.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/operators/spinoperators.py` & `qtealeaves-0.5.14/qtealeaves/operators/spinoperators.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/operators/tnoperators.py` & `qtealeaves-0.5.14/qtealeaves/operators/tnoperators.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/parameterized.py` & `qtealeaves-0.5.14/qtealeaves/parameterized.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/simulation_setup.py` & `qtealeaves-0.5.14/qtealeaves/simulation_setup.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/qtealeaves/version.py` & `qtealeaves-0.5.14/qtealeaves/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """
 Version string, e.g., for installation script.
 """
-__version__ = "0.5.13"
+__version__ = "0.5.14"
```

### Comparing `qtealeaves-0.5.13/qtealeaves.egg-info/PKG-INFO` & `qtealeaves-0.5.14/qtealeaves.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtealeaves
-Version: 0.5.13
+Version: 0.5.14
 Summary: Quantum TEA's python tensor network library
 Home-page: https://baltig.infn.it/quantum_tea_leaves/py_api_quantum_tea_leaves.git
 Author: Marco Ballarin, Giovanni Cataldi, Aurora Costantini, Daniel Jaschke, Giuseppe Magnifico, Simone Notarnicola, Alice Pagano, Luka Pavesic, Marco Rigobello, Nora Reinić, Simone Scarlatella
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `qtealeaves-0.5.13/qtealeaves.egg-info/SOURCES.txt` & `qtealeaves-0.5.14/qtealeaves.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/setup.py` & `qtealeaves-0.5.14/setup.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/tests/tests_formatting.py` & `qtealeaves-0.5.14/tests/tests_formatting.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/tests/tests_fortran_interface.py` & `qtealeaves-0.5.14/tests/tests_fortran_interface.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/tests/tests_hilbert_curvature.py` & `qtealeaves-0.5.14/tests/tests_hilbert_curvature.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/tests/tests_lattice_layout.py` & `qtealeaves-0.5.14/tests/tests_lattice_layout.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/tests/tests_linter.py` & `qtealeaves-0.5.14/tests/tests_linter.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/tests/tests_model_terms.py` & `qtealeaves-0.5.14/tests/tests_model_terms.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/tests/tests_operators.py` & `qtealeaves-0.5.14/tests/tests_operators.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/tests/tests_quantum_trajectories.py` & `qtealeaves-0.5.14/tests/tests_quantum_trajectories.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/tests/tests_rydberg_model.py` & `qtealeaves-0.5.14/tests/tests_rydberg_model.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/tests/tests_simulation_setup.py` & `qtealeaves-0.5.14/tests/tests_simulation_setup.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.13/tests/tests_ttn_simulation.py` & `qtealeaves-0.5.14/tests/tests_ttn_simulation.py`

 * *Files identical despite different names*

