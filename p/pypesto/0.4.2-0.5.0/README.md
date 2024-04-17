# Comparing `tmp/pypesto-0.4.2.tar.gz` & `tmp/pypesto-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypesto-0.4.2.tar", last modified: Mon Apr 15 18:09:01 2024, max compression
+gzip compressed data, was "pypesto-0.5.0.tar", last modified: Wed Apr 17 07:59:10 2024, max compression
```

## Comparing `pypesto-0.4.2.tar` & `pypesto-0.5.0.tar`

### file list

```diff
@@ -1,193 +1,198 @@
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.160216 pypesto-0.4.2/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1484 2024-04-15 18:06:52.000000 pypesto-0.4.2/LICENSE
--rw-r--r--   0 dweindl   (1000) dweindl   (1000)    12948 2024-04-15 18:09:01.160216 pypesto-0.4.2/PKG-INFO
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3976 2024-04-15 18:06:52.000000 pypesto-0.4.2/README.md
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.145217 pypesto-0.4.2/pypesto/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9483 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/C.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      950 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/__init__.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.146216 pypesto-0.4.2/pypesto/engine/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      401 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/engine/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      593 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/engine/base.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1520 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/engine/mpi_pool.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2400 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/engine/multi_process.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2014 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/engine/multi_thread.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      922 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/engine/single_core.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      456 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/engine/task.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.146216 pypesto-0.4.2/pypesto/ensemble/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      673 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/ensemble/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    11818 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/ensemble/covariance_analysis.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9071 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/ensemble/dimension_reduction.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    43707 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/ensemble/ensemble.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      918 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/ensemble/task.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    11582 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/ensemble/util.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.146216 pypesto-0.4.2/pypesto/hierarchical/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1284 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     4256 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/base_parameter.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8607 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/base_problem.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1317 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/base_solver.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    20724 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/inner_calculator_collector.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.147216 pypesto-0.4.2/pypesto/hierarchical/ordinal/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1466 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/ordinal/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7146 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/ordinal/calculator.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2716 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/ordinal/parameter.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    27982 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/ordinal/problem.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    42258 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/ordinal/solver.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    24360 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/petab.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.147216 pypesto-0.4.2/pypesto/hierarchical/relative/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1256 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/relative/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    12343 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/relative/calculator.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9797 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/relative/problem.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    21213 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/relative/solver.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    15533 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/relative/util.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.147216 pypesto-0.4.2/pypesto/hierarchical/semiquantitative/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      801 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/semiquantitative/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     6978 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/semiquantitative/calculator.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1981 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/semiquantitative/parameter.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    15869 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/semiquantitative/problem.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    36195 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/semiquantitative/solver.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.147216 pypesto-0.4.2/pypesto/history/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      654 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/history/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7865 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/history/amici.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    15341 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/history/base.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9866 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/history/csv.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1471 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/history/generate.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    16392 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/history/hdf5.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3872 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/history/memory.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9808 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/history/optimizer.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3497 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/history/options.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1762 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/history/util.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1902 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/logging.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.148216 pypesto-0.4.2/pypesto/objective/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      313 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/__init__.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.148216 pypesto-0.4.2/pypesto/objective/aesara/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)       77 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/aesara/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8974 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/aesara/base.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5267 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/aggregated.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.148216 pypesto-0.4.2/pypesto/objective/amici/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      141 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/amici/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    23449 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/amici/amici.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7665 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/amici/amici_calculator.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    13240 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/amici/amici_util.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    22972 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/base.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    24326 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/finite_difference.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7744 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/function.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.148216 pypesto-0.4.2/pypesto/objective/jax/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)       71 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/jax/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8662 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/jax/base.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.148216 pypesto-0.4.2/pypesto/objective/julia/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      136 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/julia/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     6169 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/julia/base.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7289 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/julia/petabJl.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9836 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/julia/petab_jl_importer.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     4259 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/pre_post_process.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    17150 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/priors.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.149217 pypesto-0.4.2/pypesto/optimize/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      699 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/optimize/__init__.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.149217 pypesto-0.4.2/pypesto/optimize/ess/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      328 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/optimize/ess/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    11596 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/optimize/ess/cess.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    23679 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/optimize/ess/ess.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9279 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/optimize/ess/function_evaluator.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7051 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/optimize/ess/refset.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    35269 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/optimize/ess/sacess.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8254 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/optimize/load.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5327 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/optimize/optimize.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    43623 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/optimize/optimizer.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1963 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/optimize/options.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2000 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/optimize/task.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5523 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/optimize/util.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.149217 pypesto-0.4.2/pypesto/petab/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      601 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/petab/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    37717 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/petab/importer.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.149217 pypesto-0.4.2/pypesto/predict/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      211 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/predict/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    18014 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/predict/amici_predictor.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1304 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/predict/task.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.149217 pypesto-0.4.2/pypesto/problem/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      207 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/problem/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    18549 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/problem/base.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2709 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/problem/hierarchical.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.150216 pypesto-0.4.2/pypesto/profile/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      288 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/profile/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3536 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/profile/approximate.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     4205 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/profile/options.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5832 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/profile/profile.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    15436 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/profile/profile_next_guess.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2440 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/profile/task.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     6840 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/profile/util.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5230 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/profile/validation_intervals.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5524 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/profile/walk_along_profile.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.150216 pypesto-0.4.2/pypesto/result/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      415 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/result/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    13868 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/result/optimize.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    12263 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/result/predict.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8066 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/result/profile.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1409 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/result/result.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3753 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/result/sample.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.150216 pypesto-0.4.2/pypesto/sample/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      644 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7431 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/adaptive_metropolis.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1988 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/adaptive_parallel_tempering.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1762 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/auto_correlation.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3742 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/diagnostics.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9649 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/dynesty.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7835 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/emcee.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5653 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/geweke_test.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7031 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/metropolis.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     6133 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/parallel_tempering.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8004 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/pymc.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3169 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/sample.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     4143 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/sampler.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3352 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/util.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.151216 pypesto-0.4.2/pypesto/select/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      582 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/select/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    18540 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/select/method.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5492 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/select/misc.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7769 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/select/model_problem.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5522 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/select/postprocessors.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9881 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/select/problem.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.151216 pypesto-0.4.2/pypesto/startpoint/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      483 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/startpoint/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7756 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/startpoint/base.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2895 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/startpoint/latin_hypercube.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1263 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/startpoint/uniform.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      455 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/startpoint/util.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.151216 pypesto-0.4.2/pypesto/store/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      486 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/store/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2553 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/store/auto.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2239 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/store/hdf5.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    10876 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/store/read_from_hdf5.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    10049 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/store/save_to_hdf5.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.151216 pypesto-0.4.2/pypesto/testing/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)       49 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/testing/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     4020 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/testing/examples.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8964 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/util.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)       22 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/version.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.152216 pypesto-0.4.2/pypesto/visualize/
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1738 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/__init__.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     6832 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/clust_color.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8800 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/dimension_reduction.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    12766 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/ensemble.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    12196 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/misc.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    13183 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/model_fit.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    13029 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/optimization_stats.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1813 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/optimizer_convergence.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    15923 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/optimizer_history.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    32126 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/ordinal_categories.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    20133 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/parameters.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2684 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/profile_cis.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    15189 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/profiles.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5722 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/reference_points.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    46051 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/sampling.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     6219 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/select.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    17460 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/spline_approximation.py
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    14103 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/waterfall.py
-drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.152216 pypesto-0.4.2/pypesto.egg-info/
--rw-r--r--   0 dweindl   (1000) dweindl   (1000)    12948 2024-04-15 18:09:01.000000 pypesto-0.4.2/pypesto.egg-info/PKG-INFO
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5058 2024-04-15 18:09:01.000000 pypesto-0.4.2/pypesto.egg-info/SOURCES.txt
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)        1 2024-04-15 18:09:01.000000 pypesto-0.4.2/pypesto.egg-info/dependency_links.txt
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2186 2024-04-15 18:09:01.000000 pypesto-0.4.2/pypesto.egg-info/requires.txt
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)        8 2024-04-15 18:09:01.000000 pypesto-0.4.2/pypesto.egg-info/top_level.txt
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      377 2024-04-15 18:06:52.000000 pypesto-0.4.2/pyproject.toml
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3041 2024-04-15 18:09:01.161216 pypesto-0.4.2/setup.cfg
--rw-rw-r--   0 dweindl   (1000) dweindl   (1000)       88 2024-04-15 18:06:52.000000 pypesto-0.4.2/setup.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.727579 pypesto-0.5.0/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1484 2024-04-17 07:58:06.000000 pypesto-0.5.0/LICENSE
+-rw-r--r--   0 dweindl   (1000) dweindl   (1000)    13455 2024-04-17 07:59:10.727579 pypesto-0.5.0/PKG-INFO
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3976 2024-04-17 07:58:06.000000 pypesto-0.5.0/README.md
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.712579 pypesto-0.5.0/pypesto/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    10042 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/C.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      950 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/__init__.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.713579 pypesto-0.5.0/pypesto/engine/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      401 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/engine/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      593 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/engine/base.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1520 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/engine/mpi_pool.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2400 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/engine/multi_process.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2014 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/engine/multi_thread.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      922 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/engine/single_core.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      456 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/engine/task.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.713579 pypesto-0.5.0/pypesto/ensemble/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      673 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/ensemble/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    11811 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/ensemble/covariance_analysis.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9064 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/ensemble/dimension_reduction.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    43778 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/ensemble/ensemble.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      912 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/ensemble/task.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    11609 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/ensemble/util.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.713579 pypesto-0.5.0/pypesto/hierarchical/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1284 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/hierarchical/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     4256 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/hierarchical/base_parameter.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8617 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/hierarchical/base_problem.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1317 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/hierarchical/base_solver.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    20815 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/hierarchical/inner_calculator_collector.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.714579 pypesto-0.5.0/pypesto/hierarchical/ordinal/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1466 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/hierarchical/ordinal/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     6877 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/hierarchical/ordinal/calculator.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2716 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/hierarchical/ordinal/parameter.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    27980 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/hierarchical/ordinal/problem.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    42338 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/hierarchical/ordinal/solver.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    24318 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/hierarchical/petab.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.714579 pypesto-0.5.0/pypesto/hierarchical/relative/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1256 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/hierarchical/relative/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    12359 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/hierarchical/relative/calculator.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9797 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/hierarchical/relative/problem.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    21213 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/hierarchical/relative/solver.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    15487 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/hierarchical/relative/util.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.714579 pypesto-0.5.0/pypesto/hierarchical/semiquantitative/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      801 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/hierarchical/semiquantitative/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     6907 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/hierarchical/semiquantitative/calculator.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1981 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/hierarchical/semiquantitative/parameter.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    17607 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/hierarchical/semiquantitative/problem.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    36208 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/hierarchical/semiquantitative/solver.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.714579 pypesto-0.5.0/pypesto/history/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      654 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/history/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7892 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/history/amici.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    15368 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/history/base.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9696 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/history/csv.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1480 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/history/generate.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    16419 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/history/hdf5.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3899 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/history/memory.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9808 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/history/optimizer.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3507 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/history/options.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1789 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/history/util.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1902 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/logging.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.715579 pypesto-0.5.0/pypesto/objective/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      313 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/objective/__init__.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.715579 pypesto-0.5.0/pypesto/objective/aesara/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)       77 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/objective/aesara/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8954 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/objective/aesara/base.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5281 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/objective/aggregated.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.715579 pypesto-0.5.0/pypesto/objective/amici/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      141 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/objective/amici/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    23234 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/objective/amici/amici.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7677 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/objective/amici/amici_calculator.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    13242 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/objective/amici/amici_util.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    22677 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/objective/base.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    24307 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/objective/finite_difference.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7764 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/objective/function.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.715579 pypesto-0.5.0/pypesto/objective/jax/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)       71 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/objective/jax/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     6578 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/objective/jax/base.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.715579 pypesto-0.5.0/pypesto/objective/julia/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      136 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/objective/julia/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     6179 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/objective/julia/base.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7334 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/objective/julia/petabJl.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9757 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/objective/julia/petab_jl_importer.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     4262 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/objective/pre_post_process.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    17128 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/objective/priors.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.715579 pypesto-0.5.0/pypesto/objective/roadrunner/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      279 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/objective/roadrunner/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    13983 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/objective/roadrunner/petab_importer_roadrunner.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     4864 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/objective/roadrunner/road_runner.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    15757 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/objective/roadrunner/roadrunner_calculator.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    14675 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/objective/roadrunner/utils.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.716579 pypesto-0.5.0/pypesto/optimize/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      678 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/optimize/__init__.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.716579 pypesto-0.5.0/pypesto/optimize/ess/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      296 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/optimize/ess/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    23962 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/optimize/ess/ess.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9348 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/optimize/ess/function_evaluator.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7045 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/optimize/ess/refset.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    35553 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/optimize/ess/sacess.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8254 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/optimize/load.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5395 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/optimize/optimize.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    44942 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/optimize/optimizer.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1967 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/optimize/options.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2000 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/optimize/task.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5526 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/optimize/util.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.716579 pypesto-0.5.0/pypesto/petab/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      647 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/petab/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    37790 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/petab/importer.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.716579 pypesto-0.5.0/pypesto/predict/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      211 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/predict/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    17993 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/predict/amici_predictor.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1306 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/predict/task.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.716579 pypesto-0.5.0/pypesto/problem/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      207 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/problem/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    18562 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/problem/base.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3146 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/problem/hierarchical.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.716579 pypesto-0.5.0/pypesto/profile/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      288 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/profile/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3545 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/profile/approximate.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     4210 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/profile/options.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5859 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/profile/profile.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    15436 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/profile/profile_next_guess.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2440 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/profile/task.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     6867 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/profile/util.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5230 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/profile/validation_intervals.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5524 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/profile/walk_along_profile.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.717579 pypesto-0.5.0/pypesto/result/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      415 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/result/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    14017 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/result/optimize.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    12314 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/result/predict.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8076 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/result/profile.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1409 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/result/result.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3772 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/result/sample.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.717579 pypesto-0.5.0/pypesto/sample/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      644 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/sample/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7400 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/sample/adaptive_metropolis.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2797 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/sample/adaptive_parallel_tempering.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1760 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/sample/auto_correlation.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3991 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/sample/diagnostics.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    14140 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/sample/dynesty.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7790 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/sample/emcee.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5624 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/sample/geweke_test.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7052 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/sample/metropolis.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    11554 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/sample/parallel_tempering.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7965 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/sample/pymc.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3163 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/sample/sample.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     4131 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/sample/sampler.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3327 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/sample/util.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.717579 pypesto-0.5.0/pypesto/select/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      605 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/select/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    18540 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/select/method.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5501 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/select/misc.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7769 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/select/model_problem.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5522 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/select/postprocessors.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9975 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/select/problem.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.718579 pypesto-0.5.0/pypesto/startpoint/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      483 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/startpoint/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7744 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/startpoint/base.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2895 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/startpoint/latin_hypercube.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1263 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/startpoint/uniform.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      455 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/startpoint/util.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.718579 pypesto-0.5.0/pypesto/store/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      486 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/store/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2553 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/store/auto.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2248 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/store/hdf5.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    10907 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/store/read_from_hdf5.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    10049 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/store/save_to_hdf5.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.718579 pypesto-0.5.0/pypesto/testing/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)       49 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/testing/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     4020 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/testing/examples.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8984 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/util.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)       22 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/version.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.719579 pypesto-0.5.0/pypesto/visualize/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1738 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/visualize/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     6826 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/visualize/clust_color.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8804 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/visualize/dimension_reduction.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    12751 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/visualize/ensemble.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    12318 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/visualize/misc.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    13201 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/visualize/model_fit.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    13035 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/visualize/optimization_stats.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1806 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/visualize/optimizer_convergence.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    15936 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/visualize/optimizer_history.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    32168 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/visualize/ordinal_categories.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    20147 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/visualize/parameters.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2711 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/visualize/profile_cis.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    15247 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/visualize/profiles.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5759 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/visualize/reference_points.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    46091 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/visualize/sampling.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     6174 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/visualize/select.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    18239 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/visualize/spline_approximation.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    14548 2024-04-17 07:58:06.000000 pypesto-0.5.0/pypesto/visualize/waterfall.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-17 07:59:10.719579 pypesto-0.5.0/pypesto.egg-info/
+-rw-r--r--   0 dweindl   (1000) dweindl   (1000)    13455 2024-04-17 07:59:10.000000 pypesto-0.5.0/pypesto.egg-info/PKG-INFO
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5264 2024-04-17 07:59:10.000000 pypesto-0.5.0/pypesto.egg-info/SOURCES.txt
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)        1 2024-04-17 07:59:10.000000 pypesto-0.5.0/pypesto.egg-info/dependency_links.txt
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2313 2024-04-17 07:59:10.000000 pypesto-0.5.0/pypesto.egg-info/requires.txt
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)        8 2024-04-17 07:59:10.000000 pypesto-0.5.0/pypesto.egg-info/top_level.txt
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1321 2024-04-17 07:58:06.000000 pypesto-0.5.0/pyproject.toml
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3172 2024-04-17 07:59:10.728579 pypesto-0.5.0/setup.cfg
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)       88 2024-04-17 07:58:06.000000 pypesto-0.5.0/setup.py
```

### Comparing `pypesto-0.4.2/LICENSE` & `pypesto-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.2/PKG-INFO` & `pypesto-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypesto
-Version: 0.4.2
+Version: 0.5.0
 Summary: python-based Parameter EStimation TOolbox
 Home-page: https://github.com/icb-dcm/pypesto
 Download-URL: https://github.com/icb-dcm/pypesto/releases
 Author: The pyPESTO developers
 Author-email: yannik.schaelte@gmail.com
 Maintainer: Paul Jonas Jost, Maren Philipps, Domagoj Dorešić, Fabian Fröhlich
 Maintainer-email: paul.jost@uni-bonn.de, maren.philipps@uni-bonn.de, domagoj.doresic@uni-bonn.de, fabian.frohlich@crick.ac.uk
@@ -30,25 +30,26 @@
 Requires-Dist: matplotlib>=3.6.2
 Requires-Dist: more-itertools>=9.0.0
 Requires-Dist: seaborn>=0.11.2
 Requires-Dist: h5py>=3.1.0
 Requires-Dist: tqdm>=4.46.0
 Requires-Dist: tabulate>=0.8.10
 Provides-Extra: all
-Requires-Dist: amici>=0.18.0; extra == "all"
+Requires-Dist: amici>=0.21.0; extra == "all"
 Requires-Dist: petab>=0.2.0; extra == "all"
 Requires-Dist: cyipopt>=1.3.0; extra == "all"
 Requires-Dist: dlib>=19.19.0; extra == "all"
 Requires-Dist: nlopt>=2.6.2; extra == "all"
 Requires-Dist: pyswarm>=0.6; extra == "all"
 Requires-Dist: cma>=3.0.3; extra == "all"
 Requires-Dist: pyswarms>=1.3.0; extra == "all"
 Requires-Dist: fides>=0.6.1; extra == "all"
 Requires-Dist: mpi4py>=3.0.3; extra == "all"
 Requires-Dist: arviz>=0.12.1; extra == "all"
+Requires-Dist: scipy<1.13.0; extra == "all"
 Requires-Dist: aesara>=2.8.6; extra == "all"
 Requires-Dist: pymc>=4.2.1; extra == "all"
 Requires-Dist: aesara>=2.0.5; extra == "all"
 Requires-Dist: jax>=0.4.1; extra == "all"
 Requires-Dist: jaxlib>=0.4.1; extra == "all"
 Requires-Dist: julia>=0.5.7; extra == "all"
 Requires-Dist: ipython>=8.4.0; extra == "all"
@@ -66,77 +67,84 @@
 Requires-Dist: ipython>=8.4.0; extra == "all"
 Requires-Dist: myst-parser>=0.18.0; extra == "all"
 Requires-Dist: ipykernel==6.23.1; extra == "all"
 Requires-Dist: julia>=0.5.7; extra == "all"
 Requires-Dist: ipython>=8.4.0; extra == "all"
 Requires-Dist: pygments>=2.12.0; extra == "all"
 Requires-Dist: arviz>=0.12.1; extra == "all"
+Requires-Dist: scipy<1.13.0; extra == "all"
 Requires-Dist: aesara>=2.8.6; extra == "all"
 Requires-Dist: pymc>=4.2.1; extra == "all"
 Requires-Dist: emcee>=3.0.2; extra == "all"
 Requires-Dist: dynesty>=2.0.3; extra == "all"
 Requires-Dist: nlopt>=2.6.2; extra == "all"
 Requires-Dist: pyswarm>=0.6; extra == "all"
 Requires-Dist: notebook>=6.1.4; extra == "all"
 Requires-Dist: networkx>=2.5.1; extra == "all"
 Requires-Dist: petab-select>=0.1.12; extra == "all"
 Requires-Dist: fides>=0.6.1; extra == "all"
-Requires-Dist: amici>=0.18.0; extra == "all"
+Requires-Dist: amici>=0.21.0; extra == "all"
 Requires-Dist: petab>=0.2.0; extra == "all"
 Requires-Dist: aesara>=2.0.5; extra == "all"
 Requires-Dist: jax>=0.4.1; extra == "all"
 Requires-Dist: jaxlib>=0.4.1; extra == "all"
+Requires-Dist: libroadrunner>=2.6.0; extra == "all"
 Requires-Dist: julia>=0.5.7; extra == "all"
 Requires-Dist: ipython>=8.4.0; extra == "all"
 Requires-Dist: pygments>=2.12.0; extra == "all"
 Requires-Dist: arviz>=0.12.1; extra == "all"
+Requires-Dist: scipy<1.13.0; extra == "all"
 Requires-Dist: aesara>=2.8.6; extra == "all"
 Requires-Dist: pymc>=4.2.1; extra == "all"
 Requires-Dist: emcee>=3.0.2; extra == "all"
 Requires-Dist: dynesty>=2.0.3; extra == "all"
 Requires-Dist: nlopt>=2.6.2; extra == "all"
 Requires-Dist: pyswarm>=0.6; extra == "all"
 Requires-Dist: notebook>=6.1.4; extra == "all"
 Requires-Dist: networkx>=2.5.1; extra == "all"
 Requires-Dist: petab-select>=0.1.12; extra == "all"
 Requires-Dist: pytest>=5.4.3; extra == "all"
 Requires-Dist: pytest-cov>=2.10.0; extra == "all"
 Requires-Dist: gitpython>=3.1.7; extra == "all"
 Requires-Dist: pytest-rerunfailures>=9.1.1; extra == "all"
 Requires-Dist: autograd>=1.3; extra == "all"
+Requires-Dist: libroadrunner>=2.6.0; extra == "all"
 Provides-Extra: all-optimizers
 Requires-Dist: cyipopt>=1.3.0; extra == "all-optimizers"
 Requires-Dist: dlib>=19.19.0; extra == "all-optimizers"
 Requires-Dist: nlopt>=2.6.2; extra == "all-optimizers"
 Requires-Dist: pyswarm>=0.6; extra == "all-optimizers"
 Requires-Dist: cma>=3.0.3; extra == "all-optimizers"
 Requires-Dist: pyswarms>=1.3.0; extra == "all-optimizers"
 Requires-Dist: fides>=0.6.1; extra == "all-optimizers"
 Provides-Extra: amici
-Requires-Dist: amici>=0.18.0; extra == "amici"
+Requires-Dist: amici>=0.21.0; extra == "amici"
+Provides-Extra: roadrunner
+Requires-Dist: libroadrunner>=2.6.0; extra == "roadrunner"
 Provides-Extra: petab
 Requires-Dist: petab>=0.2.0; extra == "petab"
 Provides-Extra: ipopt
 Requires-Dist: cyipopt>=1.3.0; extra == "ipopt"
 Provides-Extra: dlib
 Requires-Dist: dlib>=19.19.0; extra == "dlib"
 Provides-Extra: nlopt
 Requires-Dist: nlopt>=2.6.2; extra == "nlopt"
 Provides-Extra: pyswarm
 Requires-Dist: pyswarm>=0.6; extra == "pyswarm"
-Provides-Extra: cmaes
-Requires-Dist: cma>=3.0.3; extra == "cmaes"
+Provides-Extra: cma
+Requires-Dist: cma>=3.0.3; extra == "cma"
 Provides-Extra: pyswarms
 Requires-Dist: pyswarms>=1.3.0; extra == "pyswarms"
 Provides-Extra: fides
 Requires-Dist: fides>=0.6.1; extra == "fides"
 Provides-Extra: mpi
 Requires-Dist: mpi4py>=3.0.3; extra == "mpi"
 Provides-Extra: pymc
 Requires-Dist: arviz>=0.12.1; extra == "pymc"
+Requires-Dist: scipy<1.13.0; extra == "pymc"
 Requires-Dist: aesara>=2.8.6; extra == "pymc"
 Requires-Dist: pymc>=4.2.1; extra == "pymc"
 Provides-Extra: aesara
 Requires-Dist: aesara>=2.0.5; extra == "aesara"
 Provides-Extra: jax
 Requires-Dist: jax>=0.4.1; extra == "jax"
 Requires-Dist: jaxlib>=0.4.1; extra == "jax"
@@ -161,34 +169,37 @@
 Requires-Dist: ipython>=8.4.0; extra == "doc"
 Requires-Dist: myst-parser>=0.18.0; extra == "doc"
 Requires-Dist: ipykernel==6.23.1; extra == "doc"
 Requires-Dist: julia>=0.5.7; extra == "doc"
 Requires-Dist: ipython>=8.4.0; extra == "doc"
 Requires-Dist: pygments>=2.12.0; extra == "doc"
 Requires-Dist: arviz>=0.12.1; extra == "doc"
+Requires-Dist: scipy<1.13.0; extra == "doc"
 Requires-Dist: aesara>=2.8.6; extra == "doc"
 Requires-Dist: pymc>=4.2.1; extra == "doc"
 Requires-Dist: emcee>=3.0.2; extra == "doc"
 Requires-Dist: dynesty>=2.0.3; extra == "doc"
 Requires-Dist: nlopt>=2.6.2; extra == "doc"
 Requires-Dist: pyswarm>=0.6; extra == "doc"
 Requires-Dist: notebook>=6.1.4; extra == "doc"
 Requires-Dist: networkx>=2.5.1; extra == "doc"
 Requires-Dist: petab-select>=0.1.12; extra == "doc"
 Requires-Dist: fides>=0.6.1; extra == "doc"
-Requires-Dist: amici>=0.18.0; extra == "doc"
+Requires-Dist: amici>=0.21.0; extra == "doc"
 Requires-Dist: petab>=0.2.0; extra == "doc"
 Requires-Dist: aesara>=2.0.5; extra == "doc"
 Requires-Dist: jax>=0.4.1; extra == "doc"
 Requires-Dist: jaxlib>=0.4.1; extra == "doc"
+Requires-Dist: libroadrunner>=2.6.0; extra == "doc"
 Provides-Extra: example
 Requires-Dist: julia>=0.5.7; extra == "example"
 Requires-Dist: ipython>=8.4.0; extra == "example"
 Requires-Dist: pygments>=2.12.0; extra == "example"
 Requires-Dist: arviz>=0.12.1; extra == "example"
+Requires-Dist: scipy<1.13.0; extra == "example"
 Requires-Dist: aesara>=2.8.6; extra == "example"
 Requires-Dist: pymc>=4.2.1; extra == "example"
 Requires-Dist: emcee>=3.0.2; extra == "example"
 Requires-Dist: dynesty>=2.0.3; extra == "example"
 Requires-Dist: nlopt>=2.6.2; extra == "example"
 Requires-Dist: pyswarm>=0.6; extra == "example"
 Requires-Dist: notebook>=6.1.4; extra == "example"
```

### Comparing `pypesto-0.4.2/README.md` & `pypesto-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.2/pypesto/C.py` & `pypesto-0.5.0/pypesto/C.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 """
 Constants
 =========
 Package-wide consistent constant definitions.
 """
 
 from enum import Enum
-from typing import Literal, Tuple, Union
+from typing import Literal, Union
 
 ###############################################################################
 # ENSEMBLE
 
-PREDICTOR = 'predictor'
-PREDICTION_ID = 'prediction_id'
-PREDICTION_RESULTS = 'prediction_results'
-PREDICTION_ARRAYS = 'prediction_arrays'
-PREDICTION_SUMMARY = 'prediction_summary'
-
-HISTORY = 'history'
-OPTIMIZE = 'optimize'
-SAMPLE = 'sample'
-
-MEAN = 'mean'
-MEDIAN = 'median'
-STANDARD_DEVIATION = 'std'
-PERCENTILE = 'percentile'
-SUMMARY = 'summary'
-WEIGHTED_SIGMA = 'weighted_sigma'
-
-X_NAMES = 'x_names'
-NX = 'n_x'
-X_VECTOR = 'x_vectors'
-NVECTORS = 'n_vectors'
-VECTOR_TAGS = 'vector_tags'
-ENSEMBLE_TYPE = 'ensemble_type'
-PREDICTIONS = 'predictions'
-
-SIMULTANEOUS = 'simultaneous'
-POINTWISE = 'pointwise'
-
-LOWER_BOUND = 'lower_bound'
-UPPER_BOUND = 'upper_bound'
-PREEQUILIBRATION_CONDITION_ID = 'preequilibrationConditionId'
-SIMULATION_CONDITION_ID = 'simulationConditionId'
+PREDICTOR = "predictor"
+PREDICTION_ID = "prediction_id"
+PREDICTION_RESULTS = "prediction_results"
+PREDICTION_ARRAYS = "prediction_arrays"
+PREDICTION_SUMMARY = "prediction_summary"
+
+HISTORY = "history"
+OPTIMIZE = "optimize"
+SAMPLE = "sample"
+
+MEAN = "mean"
+MEDIAN = "median"
+STANDARD_DEVIATION = "std"
+PERCENTILE = "percentile"
+SUMMARY = "summary"
+WEIGHTED_SIGMA = "weighted_sigma"
+
+X_NAMES = "x_names"
+NX = "n_x"
+X_VECTOR = "x_vectors"
+NVECTORS = "n_vectors"
+VECTOR_TAGS = "vector_tags"
+ENSEMBLE_TYPE = "ensemble_type"
+PREDICTIONS = "predictions"
+
+SIMULTANEOUS = "simultaneous"
+POINTWISE = "pointwise"
+
+LOWER_BOUND = "lower_bound"
+UPPER_BOUND = "upper_bound"
+PREEQUILIBRATION_CONDITION_ID = "preequilibrationConditionId"
+SIMULATION_CONDITION_ID = "simulationConditionId"
 
 COLOR_HIT_BOTH_BOUNDS = [0.6, 0.0, 0.0, 0.9]
 COLOR_HIT_ONE_BOUND = [0.95, 0.6, 0.0, 0.9]
 COLOR_HIT_NO_BOUNDS = [0.0, 0.8, 0.0, 0.9]
 
 
 class EnsembleType(Enum):
@@ -55,170 +55,172 @@
     sample = 2
     unprocessed_chain = 3
 
 
 ###############################################################################
 # OBJECTIVE
 
-MODE_FUN = 'mode_fun'  # mode for function values
-MODE_RES = 'mode_res'  # mode for residuals
-ModeType = Literal['mode_fun', 'mode_res']  # type for `mode` argument
-FVAL = 'fval'  # function value
-FVAL0 = 'fval0'  # function value at start
-GRAD = 'grad'  # gradient
-HESS = 'hess'  # Hessian
-HESSP = 'hessp'  # Hessian vector product
-RES = 'res'  # residual
-SRES = 'sres'  # residual sensitivities
-RDATAS = 'rdatas'  # returned simulated data sets
-
-TIME = 'time'  # time
-N_FVAL = 'n_fval'  # number of function evaluations
-N_GRAD = 'n_grad'  # number of gradient evaluations
-N_HESS = 'n_hess'  # number of Hessian evaluations
-N_RES = 'n_res'  # number of residual evaluations
-N_SRES = 'n_sres'  # number of residual sensitivity evaluations
-START_TIME = 'start_time'  # start time
-X = 'x'
-X0 = 'x0'
-ID = 'id'
+MODE_FUN = "mode_fun"  # mode for function values
+MODE_RES = "mode_res"  # mode for residuals
+ModeType = Literal["mode_fun", "mode_res"]  # type for `mode` argument
+FVAL = "fval"  # function value
+FVAL0 = "fval0"  # function value at start
+GRAD = "grad"  # gradient
+HESS = "hess"  # Hessian
+HESSP = "hessp"  # Hessian vector product
+RES = "res"  # residual
+SRES = "sres"  # residual sensitivities
+RDATAS = "rdatas"  # returned simulated data sets
+OBJECTIVE_NEGLOGPOST = "neglogpost"  # objective is negative log-posterior
+OBJECTIVE_NEGLOGLIKE = "negloglike"  # objective is negative log-likelihood
+
+TIME = "time"  # time
+N_FVAL = "n_fval"  # number of function evaluations
+N_GRAD = "n_grad"  # number of gradient evaluations
+N_HESS = "n_hess"  # number of Hessian evaluations
+N_RES = "n_res"  # number of residual evaluations
+N_SRES = "n_sres"  # number of residual sensitivity evaluations
+START_TIME = "start_time"  # start time
+X = "x"
+X0 = "x0"
+ID = "id"
 
 
 ###############################################################################
 # HIERARCHICAL SCALING + OFFSET
 
-INNER_PARAMETERS = 'inner_parameters'
-INNER_RDATAS = 'inner_rdatas'
-PARAMETER_TYPE = 'parameterType'
-X_INNER_OPT = 'x_inner_opt'
-RELATIVE = 'relative'
+INNER_PARAMETERS = "inner_parameters"
+INNER_RDATAS = "inner_rdatas"
+PARAMETER_TYPE = "parameterType"
+RELATIVE = "relative"
 
 
 class InnerParameterType(str, Enum):
     """Specifies different inner parameter types."""
 
-    OFFSET = 'offset'
-    SCALING = 'scaling'
-    SIGMA = 'sigma'
-    ORDINAL = 'ordinal'
-    SPLINE = 'spline'
+    OFFSET = "offset"
+    SCALING = "scaling"
+    SIGMA = "sigma"
+    ORDINAL = "ordinal"
+    SPLINE = "spline"
 
 
 DUMMY_INNER_VALUE = {
     InnerParameterType.OFFSET: 0.0,
     InnerParameterType.SCALING: 1.0,
     InnerParameterType.SIGMA: 1.0,
     InnerParameterType.ORDINAL: 0.0,
     InnerParameterType.SPLINE: 0.0,
 }
 
 INNER_PARAMETER_BOUNDS = {
     InnerParameterType.OFFSET: {
-        LOWER_BOUND: -float('inf'),
-        UPPER_BOUND: float('inf'),
+        LOWER_BOUND: -float("inf"),
+        UPPER_BOUND: float("inf"),
     },
     InnerParameterType.SCALING: {
-        LOWER_BOUND: -float('inf'),
-        UPPER_BOUND: float('inf'),
+        LOWER_BOUND: -float("inf"),
+        UPPER_BOUND: float("inf"),
     },
     InnerParameterType.SIGMA: {
         LOWER_BOUND: 0,
-        UPPER_BOUND: float('inf'),
+        UPPER_BOUND: float("inf"),
     },
     InnerParameterType.ORDINAL: {
-        LOWER_BOUND: -float('inf'),
-        UPPER_BOUND: float('inf'),
+        LOWER_BOUND: -float("inf"),
+        UPPER_BOUND: float("inf"),
     },
     InnerParameterType.SPLINE: {
-        LOWER_BOUND: -float('inf'),
-        UPPER_BOUND: float('inf'),
+        LOWER_BOUND: -float("inf"),
+        UPPER_BOUND: float("inf"),
     },
 }
 
 ###############################################################################
 # OPTIMAL SCALING
 
 # Should go to PEtab constants at some point
-MEASUREMENT_CATEGORY = 'measurementCategory'
-MEASUREMENT_TYPE = 'measurementType'
-CENSORING_BOUNDS = 'censoringBounds'
-
-ORDINAL = 'ordinal'
-CENSORED = 'censored'
-LEFT_CENSORED = 'left-censored'
-RIGHT_CENSORED = 'right-censored'
-INTERVAL_CENSORED = 'interval-censored'
+MEASUREMENT_CATEGORY = "measurementCategory"
+MEASUREMENT_TYPE = "measurementType"
+CENSORING_BOUNDS = "censoringBounds"
+
+ORDINAL = "ordinal"
+CENSORED = "censored"
+LEFT_CENSORED = "left-censored"
+RIGHT_CENSORED = "right-censored"
+INTERVAL_CENSORED = "interval-censored"
 CENSORING_TYPES = [LEFT_CENSORED, RIGHT_CENSORED, INTERVAL_CENSORED]
 
-REDUCED = 'reduced'
-STANDARD = 'standard'
-MAXMIN = 'max-min'
-MAX = 'max'
-
-METHOD = 'method'
-REPARAMETERIZED = 'reparameterized'
-INTERVAL_CONSTRAINTS = 'interval_constraints'
-MIN_GAP = 'min_gap'
+REDUCED = "reduced"
+STANDARD = "standard"
+MAXMIN = "max-min"
+MAX = "max"
+
+METHOD = "method"
+REPARAMETERIZED = "reparameterized"
+INTERVAL_CONSTRAINTS = "interval_constraints"
+MIN_GAP = "min_gap"
 ORDINAL_OPTIONS = [
     METHOD,
     REPARAMETERIZED,
     INTERVAL_CONSTRAINTS,
     MIN_GAP,
 ]
 
-CAT_LB = 'cat_lb'
-CAT_UB = 'cat_ub'
+CAT_LB = "cat_lb"
+CAT_UB = "cat_ub"
 
-NUM_CATEGORIES = 'num_categories'
-NUM_DATAPOINTS = 'num_datapoints'
-SURROGATE_DATA = 'surrogate_data'
-NUM_INNER_PARAMS = 'num_inner_params'
-LB_INDICES = 'lb_indices'
-UB_INDICES = 'ub_indices'
-
-QUANTITATIVE_IXS = 'quantitative_ixs'
-QUANTITATIVE_DATA = 'quantitative_data'
-NUM_CONSTR_FULL = 'num_constr_full'
-C_MATRIX = 'C_matrix'
-W_MATRIX = 'W_matrix'
-W_DOT_MATRIX = 'W_dot_matrix'
-
-SCIPY_SUCCESS = 'success'
-SCIPY_FUN = 'fun'
-SCIPY_X = 'x'
+NUM_CATEGORIES = "num_categories"
+NUM_DATAPOINTS = "num_datapoints"
+SURROGATE_DATA = "surrogate_data"
+NUM_INNER_PARAMS = "num_inner_params"
+LB_INDICES = "lb_indices"
+UB_INDICES = "ub_indices"
+
+QUANTITATIVE_IXS = "quantitative_ixs"
+QUANTITATIVE_DATA = "quantitative_data"
+NUM_CONSTR_FULL = "num_constr_full"
+C_MATRIX = "C_matrix"
+W_MATRIX = "W_matrix"
+W_DOT_MATRIX = "W_dot_matrix"
+
+SCIPY_SUCCESS = "success"
+SCIPY_FUN = "fun"
+SCIPY_X = "x"
 
 ###############################################################################
 # SPLINE APPROXIMATION FOR SEMIQUANTITATIVE DATA
 
-MEASUREMENT_TYPE = 'measurementType'
+MEASUREMENT_TYPE = "measurementType"
 
-SEMIQUANTITATIVE = 'semiquantitative'
+SEMIQUANTITATIVE = "semiquantitative"
 
-SPLINE_RATIO = 'spline_ratio'
-MIN_DIFF_FACTOR = 'min_diff_factor'
-REGULARIZE_SPLINE = 'regularize_spline'
-REGULARIZATION_FACTOR = 'regularization_factor'
+SPLINE_RATIO = "spline_ratio"
+MIN_DIFF_FACTOR = "min_diff_factor"
+REGULARIZE_SPLINE = "regularize_spline"
+REGULARIZATION_FACTOR = "regularization_factor"
 SPLINE_APPROXIMATION_OPTIONS = [
     SPLINE_RATIO,
     MIN_DIFF_FACTOR,
     REGULARIZE_SPLINE,
     REGULARIZATION_FACTOR,
 ]
 
 MIN_SIM_RANGE = 1e-16
 
-SPLINE_PAR_TYPE = 'spline'
-N_SPLINE_PARS = 'n_spline_pars'
-DATAPOINTS = 'datapoints'
-MIN_DATAPOINT = 'min_datapoint'
-MAX_DATAPOINT = 'max_datapoint'
-EXPDATA_MASK = 'expdata_mask'
-CURRENT_SIMULATION = 'current_simulation'
-INNER_NOISE_PARS = 'inner_noise_pars'
-OPTIMIZE_NOISE = 'optimize_noise'
+SPLINE_PAR_TYPE = "spline"
+SPLINE_KNOTS = "spline_knots"
+N_SPLINE_PARS = "n_spline_pars"
+DATAPOINTS = "datapoints"
+MIN_DATAPOINT = "min_datapoint"
+MAX_DATAPOINT = "max_datapoint"
+EXPDATA_MASK = "expdata_mask"
+CURRENT_SIMULATION = "current_simulation"
+INNER_NOISE_PARS = "inner_noise_pars"
+OPTIMIZE_NOISE = "optimize_noise"
 
 
 ###############################################################################
 # HISTORY
 
 HISTORY = "history"
 TRACE = "trace"
@@ -228,103 +230,114 @@
 EXITFLAG = "exitflag"
 TRACE_SAVE_ITER = "trace_save_iter"
 
 SUFFIXES_CSV = ["csv"]
 SUFFIXES_HDF5 = ["hdf5", "h5"]
 SUFFIXES = SUFFIXES_CSV + SUFFIXES_HDF5
 
-CPU_TIME_TOTAL = 'cpu_time_total'
-PREEQ_CPU_TIME = 'preeq_cpu_time'
-PREEQ_CPU_TIME_BACKWARD = 'preeq_cpu_timeB'
-POSTEQ_CPU_TIME = 'posteq_cpu_time'
-POSTEQ_CPU_TIME_BACKWARD = 'posteq_cpu_timeB'
+CPU_TIME_TOTAL = "cpu_time_total"
+PREEQ_CPU_TIME = "preeq_cpu_time"
+PREEQ_CPU_TIME_BACKWARD = "preeq_cpu_timeB"
+POSTEQ_CPU_TIME = "posteq_cpu_time"
+POSTEQ_CPU_TIME_BACKWARD = "posteq_cpu_timeB"
 
 
 ###############################################################################
 # PRIOR
 
-LIN = 'lin'  # linear
-LOG = 'log'  # logarithmic to basis e
-LOG10 = 'log10'  # logarithmic to basis 10
-
-UNIFORM = 'uniform'
-PARAMETER_SCALE_UNIFORM = 'parameterScaleUniform'
-NORMAL = 'normal'
-PARAMETER_SCALE_NORMAL = 'parameterScaleNormal'
-LAPLACE = 'laplace'
-PARAMETER_SCALE_LAPLACE = 'parameterScaleLaplace'
-LOG_UNIFORM = 'logUniform'
-LOG_NORMAL = 'logNormal'
-LOG_LAPLACE = 'logLaplace'
+LIN = "lin"  # linear
+LOG = "log"  # logarithmic to basis e
+LOG10 = "log10"  # logarithmic to basis 10
+
+UNIFORM = "uniform"
+PARAMETER_SCALE_UNIFORM = "parameterScaleUniform"
+NORMAL = "normal"
+PARAMETER_SCALE_NORMAL = "parameterScaleNormal"
+LAPLACE = "laplace"
+PARAMETER_SCALE_LAPLACE = "parameterScaleLaplace"
+LOG_UNIFORM = "logUniform"
+LOG_NORMAL = "logNormal"
+LOG_LAPLACE = "logLaplace"
+
+###############################################################################
+# SAMPLING
 
+EXPONENTIAL_DECAY = (
+    "exponential_decay"  # temperature schedule for parallel tempering
+)
+BETA_DECAY = "beta_decay"  # temperature schedule for parallel tempering
 
 ###############################################################################
 # PREDICT
 
-OUTPUT_IDS = 'output_ids'  # data member in PredictionConditionResult
-PARAMETER_IDS = 'x_names'  # data member in PredictionConditionResult
-TIMEPOINTS = 'timepoints'  # data member in PredictionConditionResult
-OUTPUT = 'output'  # field in the return dict of AmiciPredictor
-OUTPUT_SENSI = 'output_sensi'  # field in the return dict of AmiciPredictor
-OUTPUT_WEIGHT = 'output_weight'  # field in the return dict of AmiciPredictor
-OUTPUT_SIGMAY = 'output_sigmay'  # field in the return dict of AmiciPredictor
+OUTPUT_IDS = "output_ids"  # data member in PredictionConditionResult
+PARAMETER_IDS = "x_names"  # data member in PredictionConditionResult
+TIMEPOINTS = "timepoints"  # data member in PredictionConditionResult
+OUTPUT = "output"  # field in the return dict of AmiciPredictor
+OUTPUT_SENSI = "output_sensi"  # field in the return dict of AmiciPredictor
+OUTPUT_WEIGHT = "output_weight"  # field in the return dict of AmiciPredictor
+OUTPUT_SIGMAY = "output_sigmay"  # field in the return dict of AmiciPredictor
 
 # separator in the conditions_ids between preequilibration and simulation
 # condition
-CONDITION_SEP = '::'
+CONDITION_SEP = "::"
 
-AMICI_T = 't'  # return field in amici simulation result
-AMICI_X = 'x'  # return field in amici simulation result
-AMICI_SX = 'sx'  # return field in amici simulation result
-AMICI_Y = 'y'  # return field in amici simulation result
-AMICI_SY = 'sy'  # return field in amici simulation result
-AMICI_LLH = 'llh'  # return field in amici simulation result
-AMICI_STATUS = 'status'  # return field in amici simulation result
-AMICI_SIGMAY = 'sigmay'  # return field in amici simulation result
-AMICI_SSIGMAY = 'ssigmay'  # return field in amici simulation result
-AMICI_SSIGMAZ = 'ssigmaz'  # return field in amici simulation result
+AMICI_T = "t"  # return field in amici simulation result
+AMICI_X = "x"  # return field in amici simulation result
+AMICI_SX = "sx"  # return field in amici simulation result
+AMICI_Y = "y"  # return field in amici simulation result
+AMICI_SY = "sy"  # return field in amici simulation result
+AMICI_LLH = "llh"  # return field in amici simulation result
+AMICI_STATUS = "status"  # return field in amici simulation result
+AMICI_SIGMAY = "sigmay"  # return field in amici simulation result
+AMICI_SSIGMAY = "ssigmay"  # return field in amici simulation result
+AMICI_SSIGMAZ = "ssigmaz"  # return field in amici simulation result
+
+ROADRUNNER_LLH = "llh"  # return field in roadrunner objective
+ROADRUNNER_INSTANCE = "roadrunner_instance"
+ROADRUNNER_SIMULATION = "simulation_results"
 
-CONDITION = 'condition'
-CONDITION_IDS = 'condition_ids'
+CONDITION = "condition"
+CONDITION_IDS = "condition_ids"
 
-CSV = 'csv'  # return file format
-H5 = 'h5'  # return file format
+CSV = "csv"  # return file format
+H5 = "h5"  # return file format
 
 ###############################################################################
 # VISUALIZE
 
 LEN_RGB = 3  # number of elements in an RGB color
 LEN_RGBA = 4  # number of elements in an RGBA color
-RGB = Tuple[(float,) * LEN_RGB]  # typing of an RGB color
-RGBA = Tuple[(float,) * LEN_RGBA]  # typing of an RGBA color
+RGB = tuple[(float,) * LEN_RGB]  # typing of an RGB color
+RGBA = tuple[(float,) * LEN_RGBA]  # typing of an RGBA color
 RGB_RGBA = Union[RGB, RGBA]  # typing of an RGB or RGBA color
 RGBA_MIN = 0  # min value for an RGBA element
 RGBA_MAX = 1  # max value for an RGBA element
 RGBA_ALPHA = 3  # zero-indexed fourth element in RGBA
 RGBA_WHITE = (RGBA_MAX, RGBA_MAX, RGBA_MAX, RGBA_MAX)  # white as an RGBA color
 RGBA_BLACK = (RGBA_MIN, RGBA_MIN, RGBA_MIN, RGBA_MAX)  # black as an RGBA color
 
 # optimizer history
-TRACE_X_TIME = 'time'
-TRACE_X_STEPS = 'steps'
+TRACE_X_TIME = "time"
+TRACE_X_STEPS = "steps"
 # supported values to plot on x-axis
 TRACE_X = (TRACE_X_TIME, TRACE_X_STEPS)
 
-TRACE_Y_FVAL = 'fval'
-TRACE_Y_GRADNORM = 'gradnorm'
+TRACE_Y_FVAL = "fval"
+TRACE_Y_GRADNORM = "gradnorm"
 # supported values to plot on y-axis
 TRACE_Y = (TRACE_Y_FVAL, TRACE_Y_GRADNORM)
 
 # parameter indices
-FREE_ONLY = 'free_only'  # only estimated parameters
-ALL = 'all'  # all parameters, also for start indices
+FREE_ONLY = "free_only"  # only estimated parameters
+ALL = "all"  # all parameters, also for start indices
 
 # start indices
-ALL_CLUSTERED = 'all_clustered'  # best + all that are in a cluster of size > 1
-FIRST_CLUSTER = 'first_cluster'  # all starts that belong to the first cluster
+ALL_CLUSTERED = "all_clustered"  # best + all that are in a cluster of size > 1
+FIRST_CLUSTER = "first_cluster"  # all starts that belong to the first cluster
 
 # waterfall max value
 WATERFALL_MAX_VALUE = 1e100
 
 
 ###############################################################################
 # ENVIRONMENT VARIABLES
```

### Comparing `pypesto-0.4.2/pypesto/__init__.py` & `pypesto-0.5.0/pypesto/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.2/pypesto/engine/base.py` & `pypesto-0.5.0/pypesto/engine/base.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.2/pypesto/engine/mpi_pool.py` & `pypesto-0.5.0/pypesto/engine/mpi_pool.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.2/pypesto/engine/multi_process.py` & `pypesto-0.5.0/pypesto/engine/multi_process.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.2/pypesto/engine/multi_thread.py` & `pypesto-0.5.0/pypesto/engine/multi_thread.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.2/pypesto/engine/single_core.py` & `pypesto-0.5.0/pypesto/engine/single_core.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.2/pypesto/ensemble/__init__.py` & `pypesto-0.5.0/pypesto/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.2/pypesto/ensemble/covariance_analysis.py` & `pypesto-0.5.0/pypesto/ensemble/covariance_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple, Union
+from typing import Union
 
 import numpy as np
 
 from .ensemble import Ensemble, EnsemblePrediction
 from .util import get_prediction_dataset
 
 
@@ -56,15 +56,15 @@
     normalize: bool = False,
     only_separable_directions: bool = False,
     cutoff_absolute_separable: float = 1e-16,
     cutoff_relative_separable: float = 1e-16,
     only_identifiable_directions: bool = False,
     cutoff_absolute_identifiable: float = 1e-16,
     cutoff_relative_identifiable: float = 1e-16,
-) -> Tuple[np.ndarray, np.ndarray]:
+) -> tuple[np.ndarray, np.ndarray]:
     """
     Compute the spectral decomposition of ensemble parameters.
 
     Parameters
     ----------
     ens:
         Ensemble object containing a set of parameter vectors
@@ -124,15 +124,15 @@
     normalize: bool = False,
     only_separable_directions: bool = False,
     cutoff_absolute_separable: float = 1e-16,
     cutoff_relative_separable: float = 1e-16,
     only_identifiable_directions: bool = False,
     cutoff_absolute_identifiable: float = 1e-16,
     cutoff_relative_identifiable: float = 1e-16,
-) -> Tuple[np.ndarray, np.ndarray]:
+) -> tuple[np.ndarray, np.ndarray]:
     """
     Compute the spectral decomposition of ensemble predictions.
 
     Parameters
     ----------
     ens:
         Ensemble object containing a set of parameter vectors and a set of
@@ -187,15 +187,15 @@
     normalize: bool = False,
     only_separable_directions: bool = False,
     cutoff_absolute_separable: float = 1e-16,
     cutoff_relative_separable: float = 1e-16,
     only_identifiable_directions: bool = False,
     cutoff_absolute_identifiable: float = 1e-16,
     cutoff_relative_identifiable: float = 1e-16,
-) -> Tuple[np.ndarray, np.ndarray]:
+) -> tuple[np.ndarray, np.ndarray]:
     """
     Compute the spectral decomposition of ensemble parameters or predictions.
 
     Parameters
     ----------
     matrix:
         symmetric matrix (typically a covariance matrix) of parameters or
@@ -262,16 +262,16 @@
             )
         elif cutoff_absolute_separable is not None:
             above_cutoff = eigenvalues > cutoff_absolute_separable
         elif cutoff_relative_separable is not None:
             above_cutoff = rel_eigenvalues > cutoff_relative_separable
         else:
             raise Exception(
-                'Need a lower cutoff (absolute or relative, '
-                'e.g., 1e-16, to compute separable directions.'
+                "Need a lower cutoff (absolute or relative, "
+                "e.g., 1e-16, to compute separable directions."
             )
 
         # restrict to those above cutoff
         eigenvalues = eigenvalues[above_cutoff]
         eigenvectors = eigenvectors[:, above_cutoff]
         # apply normlization
         if normalize:
@@ -293,16 +293,16 @@
         )
     elif cutoff_absolute_identifiable is not None:
         below_cutoff = 1 / eigenvalues > cutoff_absolute_identifiable
     elif cutoff_relative_identifiable is not None:
         below_cutoff = 1 / rel_eigenvalues > cutoff_relative_identifiable
     else:
         raise Exception(
-            'Need an inverse upper cutoff (absolute or relative, '
-            'e.g., 1e-16, to compute identifiable directions.'
+            "Need an inverse upper cutoff (absolute or relative, "
+            "e.g., 1e-16, to compute identifiable directions."
         )
 
     # restrict to those below cutoff
     eigenvalues = eigenvalues[below_cutoff]
     eigenvectors = eigenvectors[:, below_cutoff]
     # apply normlization
     if normalize:
```

### Comparing `pypesto-0.4.2/pypesto/ensemble/dimension_reduction.py` & `pypesto-0.5.0/pypesto/ensemble/dimension_reduction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import Callable, Tuple, Union
+from typing import Callable, Union
 
 import numpy as np
 
 from .ensemble import Ensemble, EnsemblePrediction
 from .util import get_prediction_dataset
 
 
 def get_umap_representation_parameters(
     ens: Ensemble,
     n_components: int = 2,
     normalize_data: bool = False,
     **kwargs,
-) -> Tuple:
+) -> tuple:
     """
     UMAP of parameter ensemble.
 
     Compute the representation with reduced dimensionality via umap
     (with a given number of umap components) of the parameter ensemble.
     Allows to pass on additional keyword arguments to the umap routine.
 
@@ -47,15 +47,15 @@
 
 def get_umap_representation_predictions(
     ens: Union[Ensemble, EnsemblePrediction],
     prediction_index: int = 0,
     n_components: int = 2,
     normalize_data: bool = False,
     **kwargs,
-) -> Tuple:
+) -> tuple:
     """
     UMAP of ensemble prediction.
 
     Compute the representation with reduced dimensionality via umap
     (with a given number of umap components) of the ensemble predictions.
     Allows to pass on additional keyword arguments to the umap routine.
 
@@ -93,15 +93,15 @@
 
 
 def get_pca_representation_parameters(
     ens: Ensemble,
     n_components: int = 2,
     rescale_data: bool = True,
     rescaler: Union[Callable, None] = None,
-) -> Tuple:
+) -> tuple:
     """
     PCA of parameter ensemble.
 
     Compute the representation with reduced dimensionality via principal
     component analysis (with a given number of principal components) of the
     parameter ensemble.
 
@@ -135,15 +135,15 @@
 
 def get_pca_representation_predictions(
     ens: Union[Ensemble, EnsemblePrediction],
     prediction_index: int = 0,
     n_components: int = 2,
     rescale_data: bool = True,
     rescaler: Union[Callable, None] = None,
-) -> Tuple:
+) -> tuple:
     """
     PCA of ensemble prediction.
 
     Compute the representation with reduced dimensionality via principal
     component analysis (with a given number of principal components) of the
     ensemble prediction.
 
@@ -184,15 +184,15 @@
 
 
 def _get_umap_representation_lowlevel(
     dataset: np.ndarray,
     n_components: int = 2,
     normalize_data: bool = False,
     **kwargs,
-) -> Tuple:
+) -> tuple:
     """
     Low level UMAP of parameter ensemble.
 
     Compute the representation with reduced dimensionality via uniform
     manifold approximation and projection (with a given number of principal
     components) of the parameter ensemble.
 
@@ -235,15 +235,15 @@
 
 
 def _get_pca_representation_lowlevel(
     dataset: np.ndarray,
     n_components: int = 2,
     rescale_data: bool = True,
     rescaler: Union[Callable, None] = None,
-) -> Tuple:
+) -> tuple:
     """
     Low level PCA of parameter ensemble.
 
     Compute the representation with reduced dimensionality via principal
     component analysis (with a given number of principal components) of the
     parameter ensemble.
```

### Comparing `pypesto-0.4.2/pypesto/ensemble/ensemble.py` & `pypesto-0.5.0/pypesto/ensemble/ensemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import logging
+from collections.abc import Sequence
 from functools import partial
-from typing import TYPE_CHECKING, Callable, Optional, Sequence, Union
+from typing import TYPE_CHECKING, Any, Callable
 
 import numpy as np
 import pandas as pd
 from scipy.stats import chi2
 
 from ..C import (
     ENSEMBLE_TYPE,
@@ -63,15 +64,15 @@
     An ensemble prediction consists of an ensemble, i.e., a set of parameter
     vectors and their identifiers such as a sample, and a prediction function.
     It can be attached to an ensemble-type object.
     """
 
     def __init__(
         self,
-        predictor: Optional[Callable[[Sequence], PredictionResult]] = None,
+        predictor: Callable[[Sequence], PredictionResult] | None = None,
         prediction_id: str = None,
         prediction_results: Sequence[PredictionResult] = None,
         lower_bound: Sequence[np.ndarray] = None,
         upper_bound: Sequence[np.ndarray] = None,
     ):
         """
         Initialize.
@@ -121,18 +122,21 @@
 
         Allows to apply functions such as __dict__ to them.
         """
         yield PREDICTOR, self.predictor
         yield PREDICTION_ID, self.prediction_id
         yield PREDICTION_RESULTS, self.prediction_results
         yield PREDICTION_ARRAYS, self.prediction_arrays
-        yield PREDICTION_SUMMARY, {
-            i_key: dict(self.prediction_summary[i_key])
-            for i_key in self.prediction_summary.keys()
-        }
+        yield (
+            PREDICTION_SUMMARY,
+            {
+                i_key: dict(self.prediction_summary[i_key])
+                for i_key in self.prediction_summary.keys()
+            },
+        )
         yield LOWER_BOUND, self.lower_bound
         yield UPPER_BOUND, self.upper_bound
 
     def condense_to_arrays(self):
         """
         Add prediction result to EnsemblePrediction object.
 
@@ -215,22 +219,22 @@
         -------
         dictionary of predictions results with the keys mean, std, median,
         percentiles, ...
         """
         # check if prediction results are available
         if not self.prediction_results:
             raise ArithmeticError(
-                'Cannot compute summary statistics from '
-                'empty prediction results.'
+                "Cannot compute summary statistics from "
+                "empty prediction results."
             )
         # if weightings shall be used, check whether weights are there
         if weighting:
             if not self.prediction_results[0].conditions[0].output_weight:
                 raise ValueError(
-                    'There are no weights in the prediction results.'
+                    "There are no weights in the prediction results."
                 )
 
         n_conditions = len(self.prediction_results[0].conditions)
 
         def _stack_outputs(ic: int) -> np.array:
             """
             Stack outputs.
@@ -265,15 +269,15 @@
             output_sensi_list = [
                 prediction.conditions[ic].output_sensi
                 for prediction in self.prediction_results
             ]
             # stack into one numpy array
             return np.stack(output_sensi_list, axis=-1)
 
-        def _stack_weights(ic: int) -> Union[np.ndarray, None]:
+        def _stack_weights(ic: int) -> np.ndarray | None:
             """
             Stack weights.
 
             Group weights for different parameter vectors of one ensemble
             together, if they belong to the same simulation condition, and
             stack them in one array
 
@@ -428,15 +432,15 @@
             self.prediction_summary[WEIGHTED_SIGMA] is None
         ):
             try:
                 self.compute_summary(
                     weighting=True, compute_weighted_sigma=True
                 )
             except TypeError:
-                raise ValueError('Computing a summary failed.')
+                raise ValueError("Computing a summary failed.") from None
         n_conditions = len(self.prediction_results[0].conditions)
         chi_2 = []
         for i_cond in range(n_conditions):
             # get measurements and put into right form
             y_meas = amici_objective.edatas[i_cond].getObservedData()
             y_meas = np.array(y_meas)
             # bring into shape (n_t,n_y)
@@ -448,16 +452,16 @@
             weighted_sigmas = (
                 self.prediction_summary[WEIGHTED_SIGMA]
                 .conditions[i_cond]
                 .output
             )
             if y_meas.shape != mean_traj.shape:
                 raise ValueError(
-                    'Shape of trajectory and shape '
-                    'of measurements does not match.'
+                    "Shape of trajectory and shape "
+                    "of measurements does not match."
                 )
             chi_2.append(
                 np.nansum(((y_meas - mean_traj) / weighted_sigmas) ** 2)
             )
         return np.sum(chi_2)
 
 
@@ -473,15 +477,15 @@
     other.
     """
 
     def __init__(
         self,
         x_vectors: np.ndarray,
         x_names: Sequence[str] = None,
-        vector_tags: Sequence[tuple[int, int]] = None,
+        vector_tags: Sequence[Any] = None,
         ensemble_type: EnsembleType = None,
         predictions: Sequence[EnsemblePrediction] = None,
         lower_bound: np.ndarray = None,
         upper_bound: np.ndarray = None,
     ):
         """
         Initialize.
@@ -515,15 +519,15 @@
         if ensemble_type is not None:
             self.ensemble_type = ensemble_type
 
         # handle parameter vectors and sizes
         self.x_vectors = x_vectors
         self.n_x = x_vectors.shape[0]
         self.n_vectors = x_vectors.shape[1]
-        self.vector_tags = vector_tags
+        self.vector_tags = list(vector_tags) if vector_tags is not None else []
         self.summary = None
 
         # store bounds
         self.lower_bound = np.full((self.n_x,), np.nan)
         if lower_bound is not None:
             if np.array(lower_bound).size == 1:
                 self.lower_bound = np.full((x_vectors.shape[0],), lower_bound)
@@ -536,15 +540,15 @@
             else:
                 self.upper_bound = upper_bound
 
         # handle parameter names
         if x_names is not None:
             self.x_names = x_names
         else:
-            self.x_names = [f'x_{ix}' for ix in range(self.n_x)]
+            self.x_names = [f"x_{ix}" for ix in range(self.n_x)]
 
         # Do we have predictions for this ensemble?
         self.predictions = []
         if predictions is not None:
             self.predictions = predictions
 
     @staticmethod
@@ -638,56 +642,56 @@
         """
         if rel_cutoff is None and percentile is None:
             abs_cutoff = np.inf
         elif rel_cutoff is not None:
             abs_cutoff = result.optimize_result[0].fval + rel_cutoff
             if percentile is not None:
                 logger.warning(
-                    'percentile is going to be ignored as '
-                    'rel_cutoff is not `None`.'
+                    "percentile is going to be ignored as "
+                    "rel_cutoff is not `None`."
                 )
         else:
             abs_cutoff = calculate_cutoff(result=result, percentile=percentile)
         x_vectors = []
         vector_tags = []
         x_names = [
             result.problem.x_names[i] for i in result.problem.x_free_indices
         ]
 
         for start in result.optimize_result.list:
             # add the parameters from the next start as long as we
             # did not reach maximum size and the next value is still
             # lower than the cutoff value
             if (
-                start['fval'] <= abs_cutoff
+                start["fval"] <= abs_cutoff
                 and len(x_vectors) < max_size
                 # 'x' can be None if optimization failed at the startpoint
-                and start['x'] is not None
+                and start["x"] is not None
             ):
-                x_vectors.append(start['x'][result.problem.x_free_indices])
+                x_vectors.append(start["x"][result.problem.x_free_indices])
 
                 # the vector tag will be a -1 to indicate it is the last step
-                vector_tags.append((int(start['id']), -1))
+                vector_tags.append((start["id"], -1))
             else:
                 break
 
         # print a warning if there are no vectors within the ensemble
         if len(x_vectors) == 0:
             raise ValueError(
-                'The ensemble does not contain any vectors. '
-                'Either the cutoff value was too small\n or the '
-                'result.optimize_result object might be empty.'
+                "The ensemble does not contain any vectors. "
+                "Either the cutoff value was too small\n or the "
+                "result.optimize_result object might be empty."
             )
         elif len(x_vectors) < max_size:
             logger.info(
-                f'The ensemble contains {len(x_vectors)} parameter '
-                'vectors, which is less than the maximum size.\nIf '
-                'you want to include more \nvectors, you can consider '
-                'raising the cutoff value or including parameters '
-                'from \nthe history with the `from_history` function.'
+                f"The ensemble contains {len(x_vectors)} parameter "
+                "vectors, which is less than the maximum size.\nIf "
+                "you want to include more \nvectors, you can consider "
+                "raising the cutoff value or including parameters "
+                "from \nthe history with the `from_history` function."
             )
 
         x_vectors = np.stack(x_vectors, axis=1)
         return Ensemble(
             x_vectors=x_vectors,
             x_names=x_names,
             vector_tags=vector_tags,
@@ -738,19 +742,19 @@
         """
         if rel_cutoff is None and percentile is None:
             abs_cutoff = np.inf
         elif rel_cutoff is not None:
             abs_cutoff = result.optimize_result[0].fval + rel_cutoff
         else:
             abs_cutoff = calculate_cutoff(result=result, percentile=percentile)
-        if not result.optimize_result.list[0].history.options['trace_record']:
+        if not result.optimize_result.list[0].history.options["trace_record"]:
             logger.warning(
-                'The optimize result has no trace. The Ensemble '
-                'will automatically be created through '
-                'from_optimization_endpoints().'
+                "The optimize result has no trace. The Ensemble "
+                "will automatically be created through "
+                "from_optimization_endpoints()."
             )
             return Ensemble.from_optimization_endpoints(
                 result=result,
                 rel_cutoff=rel_cutoff,
                 max_size=max_size,
                 **kwargs,
             )
@@ -760,15 +764,15 @@
             result.problem.x_names[i] for i in result.problem.x_free_indices
         ]
         lb = result.problem.lb
         ub = result.problem.ub
 
         # calculate the number of starts whose final nllh is below cutoff
         n_starts = sum(
-            start['fval'] <= abs_cutoff
+            start["fval"] <= abs_cutoff
             for start in result.optimize_result.list
         )
 
         fval_trace = [
             np.array(
                 result.optimize_result.list[i_ms][HISTORY].get_fval_trace()
             )
@@ -793,26 +797,26 @@
                 cutoff=abs_cutoff,
                 n_vectors=n_per_starts[start],
                 distribute=distribute,
             )
             x_vectors.extend([x_trace[start][ind] for ind in indices])
             vector_tags.extend(
                 [
-                    (int(result.optimize_result.list[start]['id']), ind)
+                    (result.optimize_result.list[start]["id"], ind)
                     for ind in indices
                 ]
             )
 
         # raise a `ValueError` if there are no vectors within the ensemble
         if len(x_vectors) == 0:
             raise ValueError(
-                'The ensemble does not contain any vectors. '
-                'Either the `cutoff` value was too \nsmall '
-                'or the `result.optimize_result` object might '
-                'be empty.'
+                "The ensemble does not contain any vectors. "
+                "Either the `cutoff` value was too \nsmall "
+                "or the `result.optimize_result` object might "
+                "be empty."
             )
 
         x_vectors = np.stack(x_vectors, axis=1)
         return Ensemble(
             x_vectors=x_vectors,
             x_names=x_names,
             vector_tags=vector_tags,
@@ -838,15 +842,15 @@
         yield LOWER_BOUND, self.lower_bound
         yield UPPER_BOUND, self.upper_bound
 
     def _map_parameters_by_objective(
         self,
         predictor: Callable,
         default_value: float = None,
-    ) -> list[Union[int, float]]:
+    ) -> list[int | float]:
         """
         Create mapping for parameters from ensemble to predictor.
 
         The parameters of the ensemble don't need to have the same ordering as
         in the predictor.
         """
         # create short hands
@@ -1030,57 +1034,57 @@
             ub = self.upper_bound[ix]
             mean = self.summary[MEAN][ix]
             std = self.summary[STANDARD_DEVIATION][ix]
             median = self.summary[MEAN][ix]
             perc_list = [
                 int(i_key[11:])
                 for i_key in self.summary.keys()
-                if i_key[0:4] == 'perc'
+                if i_key[0:4] == "perc"
             ]
             perc_lower = [perc for perc in perc_list if perc < 50]
             perc_upper = [perc for perc in perc_list if perc > 50]
 
             # create dict of identifiability
             tmp_identifiability = {
-                'parameterId': x_name,
-                'lowerBound': lb,
-                'upperBound': ub,
-                'ensemble_mean': mean,
-                'ensemble_std': std,
-                'ensemble_median': median,
-                'within lb: 1 std': lb < mean - std,
-                'within ub: 1 std': ub > mean + std,
-                'within lb: 2 std': lb < mean - 2 * std,
-                'within ub: 2 std': ub > mean + 2 * std,
-                'within lb: 3 std': lb < mean - 3 * std,
-                'within ub: 3 std': ub > mean + 3 * std,
+                "parameterId": x_name,
+                "lowerBound": lb,
+                "upperBound": ub,
+                "ensemble_mean": mean,
+                "ensemble_std": std,
+                "ensemble_median": median,
+                "within lb: 1 std": lb < mean - std,
+                "within ub: 1 std": ub > mean + std,
+                "within lb: 2 std": lb < mean - 2 * std,
+                "within ub: 2 std": ub > mean + 2 * std,
+                "within lb: 3 std": lb < mean - 3 * std,
+                "within ub: 3 std": ub > mean + 3 * std,
             }
             # handle percentiles
             for perc in perc_lower:
-                tmp_identifiability[f'within lb: perc {perc}'] = (
+                tmp_identifiability[f"within lb: perc {perc}"] = (
                     lb < self.summary[get_percentile_label(perc)][ix]
                 )
             for perc in perc_upper:
-                tmp_identifiability[f'within ub: perc {perc}'] = (
+                tmp_identifiability[f"within ub: perc {perc}"] = (
                     ub > self.summary[get_percentile_label(perc)][ix]
                 )
 
             parameter_identifiability.append(tmp_identifiability)
 
         # create DataFrame
         parameter_identifiability = pd.DataFrame(parameter_identifiability)
         parameter_identifiability.index = parameter_identifiability[
-            'parameterId'
+            "parameterId"
         ]
 
         return parameter_identifiability
 
 
 def entries_per_start(
-    fval_traces: list['np.ndarray'],
+    fval_traces: list[np.ndarray],
     cutoff: float,
     max_size: int,
     max_per_start: int,
 ) -> list[int]:
     """
     Create the indices of each start that will be included in the ensemble.
 
@@ -1161,15 +1165,15 @@
     if distribute:
         indices = np.round(np.linspace(0, len(candidates) - 1, n_vectors))
         return candidates[indices.astype(int)]
     else:
         return sorted(candidates, key=lambda i: trace_start[i])[:n_vectors]
 
 
-def get_percentile_label(percentile: Union[float, int, str]) -> str:
+def get_percentile_label(percentile: float | int | str) -> str:
     """Convert a percentile to a label.
 
     Labels for percentiles are used at different locations (e.g. ensemble
     prediction code, and visualization code). This method ensures that the same
     percentile is labeled identically everywhere.
 
     The percentile is rounded to two decimal places in the label representation
@@ -1187,20 +1191,20 @@
     The label of the (possibly rounded) percentile.
     """
     if isinstance(percentile, str):
         percentile = float(percentile)
         if percentile == round(percentile):
             percentile = round(percentile)
     if isinstance(percentile, float):
-        percentile_str = f'{percentile:.2f}'
+        percentile_str = f"{percentile:.2f}"
         # Add `...` to the label if the percentile value changed after rounding
         if float(percentile_str) != percentile:
-            percentile_str += '...'
+            percentile_str += "..."
         percentile = percentile_str
-    return f'{PERCENTILE} {percentile}'
+    return f"{PERCENTILE} {percentile}"
 
 
 def calculate_cutoff(
     result: Result,
     percentile: float = 95,
     cr_option: str = SIMULTANEOUS,
 ):
```

### Comparing `pypesto-0.4.2/pypesto/ensemble/task.py` & `pypesto-0.5.0/pypesto/ensemble/task.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Any, Callable, List
+from typing import Any, Callable
 
 import numpy as np
 
 from ..engine import Task
 
 logger = logging.getLogger(__name__)
 
@@ -28,14 +28,14 @@
         id: str,
     ):
         super().__init__()
         self.method = method
         self.vectors = vectors
         self.id = id
 
-    def execute(self) -> List[Any]:
+    def execute(self) -> list[Any]:
         """Execute the task."""
         logger.debug(f"Executing task {self.id}.")
         results = []
         for index in range(self.vectors.shape[1]):
             results.append(self.method(self.vectors[:, index]))
         return results
```

### Comparing `pypesto-0.4.2/pypesto/ensemble/util.py` & `pypesto-0.5.0/pypesto/ensemble/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Ensemble utilities."""
 
 import os
+from collections.abc import Sequence
 from pathlib import Path
-from typing import Callable, Literal, Sequence, Union
+from typing import Callable, Literal, Union
 
 import h5py
 import numpy as np
 import pandas as pd
 
 from ..C import (
     LOWER_BOUND,
@@ -27,15 +28,15 @@
 from ..result import PredictionConditionResult, PredictionResult
 from ..store import read_result, write_array
 from .ensemble import Ensemble, EnsemblePrediction
 
 
 def read_from_csv(
     path: str,
-    sep: str = '\t',
+    sep: str = "\t",
     index_col: int = 0,
     headline_parser: Callable = None,
     ensemble_type: EnsembleType = None,
     lower_bound: np.ndarray = None,
     upper_bound: np.ndarray = None,
 ):
     """
@@ -78,15 +79,15 @@
         lower_bound=lower_bound,
         upper_bound=upper_bound,
     )
 
 
 def read_ensemble_from_hdf5(
     filename: str,
-    input_type: Literal['optimize', 'sample'] = OPTIMIZE,
+    input_type: Literal["optimize", "sample"] = OPTIMIZE,
     remove_burn_in: bool = True,
     chain_slice: slice = None,
     cutoff: float = np.inf,
     max_size: int = np.inf,
 ):
     """
     Create an ensemble from an HDF5 storage file.
@@ -116,18 +117,18 @@
         return Ensemble.from_sample(
             result=result,
             remove_burn_in=remove_burn_in,
             chain_slice=chain_slice,
         )
     else:
         raise ValueError(
-            'The type you provided was neither '
+            "The type you provided was neither "
             f'"{SAMPLE}" nor "{OPTIMIZE}". Those are '
-            'currently the only supported types. '
-            'Please choose one of them.'
+            "currently the only supported types. "
+            "Please choose one of them."
         )
 
 
 def read_from_df(
     dataframe: pd.DataFrame,
     headline_parser: Callable = None,
     ensemble_type: EnsembleType = None,
@@ -188,20 +189,20 @@
         The prediciton to be saved.
     output_file:
         The filename of the hdf5 file.
     base_path:
         An optional filepath where the file should be saved to.
     """
     # parse base path
-    base = Path('')
+    base = Path("")
     if base_path is not None:
         base = Path(base_path)
 
     # open file
-    with h5py.File(output_file, 'a') as f:
+    with h5py.File(output_file, "a") as f:
         # write prediction ID if available
         if ensemble_prediction.prediction_id is not None:
             f.create_dataset(
                 os.path.join(base, PREDICTION_ID),
                 data=ensemble_prediction.prediction_id,
             )
 
@@ -240,24 +241,24 @@
         # write summary statistics to h5 file
         for (
             summary_id,
             summary,
         ) in ensemble_prediction.prediction_summary.items():
             if summary is None:
                 continue
-            tmp_base_path = os.path.join(base, f'{SUMMARY}_{summary_id}')
+            tmp_base_path = os.path.join(base, f"{SUMMARY}_{summary_id}")
             f.create_group(tmp_base_path)
             summary.write_to_h5(output_file, base_path=tmp_base_path)
 
         # write the single prediction results
         for i_result, result in enumerate(
             ensemble_prediction.prediction_results
         ):
             tmp_base_path = os.path.join(
-                base, f'{PREDICTION_RESULTS}_{i_result}'
+                base, f"{PREDICTION_RESULTS}_{i_result}"
             )
             result.write_to_h5(output_file, base_path=tmp_base_path)
 
 
 def get_prediction_dataset(
     ens: Union[Ensemble, EnsemblePrediction], prediction_index: int = 0
 ) -> np.ndarray:
@@ -284,60 +285,60 @@
     if isinstance(ens, Ensemble):
         dataset = ens.predictions[prediction_index]
     elif isinstance(ens, EnsemblePrediction):
         ens.condense_to_arrays()
         dataset = ens.prediction_arrays[OUTPUT].transpose()
     else:
         raise Exception(
-            'Need either an Ensemble object with predictions or '
-            'an EnsemblePrediction object as input. Stopping.'
+            "Need either an Ensemble object with predictions or "
+            "an EnsemblePrediction object as input. Stopping."
         )
 
     return dataset
 
 
 def read_ensemble_prediction_from_h5(
     predictor: Union[Callable[[Sequence], PredictionResult], None],
     input_file: str,
 ):
     """Read an ensemble prediction from an HDF5 File."""
     # open file
-    with h5py.File(input_file, 'r') as f:
+    with h5py.File(input_file, "r") as f:
         pred_res_list = []
         bounds = {}
         for key in f.keys():
             if key.startswith(SUMMARY):
                 continue
             if key == PREDICTION_ID:
                 prediction_id = f[key][()].decode()
                 continue
             if key in {LOWER_BOUND, UPPER_BOUND}:
                 if isinstance(f[key], h5py._hl.dataset.Dataset):
                     bounds[key] = f[key][:]
                     continue
                 bounds[key] = [
-                    f[f'{key}/{cond}'][()] for cond in f[key].keys()
+                    f[f"{key}/{cond}"][()] for cond in f[key].keys()
                 ]
                 bounds[key] = np.array(bounds[key])
                 continue
-            x_names = list(decode_array(f[f'{key}/{X_NAMES}'][()]))
-            condition_ids = list(decode_array(f[f'{key}/condition_ids'][()]))
+            x_names = list(decode_array(f[f"{key}/{X_NAMES}"][()]))
+            condition_ids = list(decode_array(f[f"{key}/condition_ids"][()]))
             pred_cond_res_list = []
             for id, _ in enumerate(condition_ids):
-                output = f[f'{key}/{id}/{OUTPUT}'][:]
+                output = f[f"{key}/{id}/{OUTPUT}"][:]
                 output_ids = tuple(
-                    decode_array(f[f'{key}/{id}' f'/{OUTPUT_IDS}'][:])
+                    decode_array(f[f"{key}/{id}" f"/{OUTPUT_IDS}"][:])
                 )
-                timepoints = f[f'{key}/{id}/{TIMEPOINTS}'][:]
+                timepoints = f[f"{key}/{id}/{TIMEPOINTS}"][:]
                 try:
-                    output_weight = f[f'{key}/{id}/{OUTPUT_WEIGHT}'][()]
+                    output_weight = f[f"{key}/{id}/{OUTPUT_WEIGHT}"][()]
                 except KeyError:
                     output_weight = None
                 try:
-                    output_sigmay = f[f'{key}/{id}/{OUTPUT_SIGMAY}'][:]
+                    output_sigmay = f[f"{key}/{id}/{OUTPUT_SIGMAY}"][:]
                 except KeyError:
                     output_sigmay = None
                 pred_cond_res_list.append(
                     PredictionConditionResult(
                         timepoints=timepoints,
                         output_ids=output_ids,
                         output=output,
```

### Comparing `pypesto-0.4.2/pypesto/hierarchical/__init__.py` & `pypesto-0.5.0/pypesto/hierarchical/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.2/pypesto/hierarchical/base_parameter.py` & `pypesto-0.5.0/pypesto/hierarchical/base_parameter.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.2/pypesto/hierarchical/base_problem.py` & `pypesto-0.5.0/pypesto/hierarchical/base_problem.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,24 +50,24 @@
         for i in range(len(self.data)):
             self.data[i][~self.data_mask[i]] = np.nan
 
         logger.debug(f"Created InnerProblem with ids {self.get_x_ids()}")
 
         if self.is_empty():
             raise ValueError(
-                'There are no parameters in the inner problem of hierarchical '
-                'optimization.'
+                "There are no parameters in the inner problem of hierarchical "
+                "optimization."
             )
 
     @staticmethod
     def from_petab_amici(
-        petab_problem: 'petab.Problem',
-        amici_model: 'amici.Model',
-        edatas: list['amici.ExpData'],
-    ) -> 'InnerProblem':
+        petab_problem: "petab.Problem",
+        amici_model: "amici.Model",
+        edatas: list["amici.ExpData"],
+    ) -> "InnerProblem":
         """Create an InnerProblem from a PEtab problem and AMICI objects."""
 
     def get_x_ids(self) -> list[str]:
         """Get IDs of inner parameters."""
         return list(self.xs.keys())
 
     def get_interpretable_x_ids(self) -> list[str]:
@@ -114,15 +114,15 @@
         }
 
     def get_for_id(self, inner_parameter_id: str) -> InnerParameter:
         """Get InnerParameter for the given parameter ID."""
         try:
             return self.xs[inner_parameter_id]
         except KeyError:
-            raise KeyError(f"Cannot find parameter with id {id}.")
+            raise KeyError(f"Cannot find parameter with id {id}.") from None
 
     def is_empty(self) -> bool:
         """Check for emptiness.
 
         Returns
         -------
         ``True`` if there aren't any parameters associated with this problem,
@@ -186,15 +186,15 @@
         Returns
         -------
         Whether the data sets are consistent.
         """
         # TODO replace but edata1==edata2 once this makes it into amici
         #  https://github.com/AMICI-dev/AMICI/issues/1880
         data = [
-            amici.numpy.ExpDataView(edata)['observedData'] for edata in edatas
+            amici.numpy.ExpDataView(edata)["observedData"] for edata in edatas
         ]
 
         if len(self.data) != len(data):
             return False
 
         for data0, data1 in zip(self.data, data):
             if not np.array_equal(data0, data1, equal_nan=True):
@@ -214,19 +214,19 @@
     return scaled_dct
 
 
 def scale_value(
     val: Union[float, np.array], scale: str
 ) -> Union[float, np.array]:
     """Scale a single value."""
-    if scale == 'lin':
+    if scale == "lin":
         return val
-    if scale == 'log':
+    if scale == "log":
         return np.log(val)
-    if scale == 'log10':
+    if scale == "log10":
         return np.log10(val)
     raise ValueError(f"Scale {scale} not recognized.")
 
 
 def ix_matrices_from_arrays(
     ixs: dict[str, list[tuple[int, int, int]]], edatas: list[np.array]
 ) -> dict[str, list[np.array]]:
```

### Comparing `pypesto-0.4.2/pypesto/hierarchical/base_solver.py` & `pypesto-0.5.0/pypesto/hierarchical/base_solver.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.2/pypesto/hierarchical/inner_calculator_collector.py` & `pypesto-0.5.0/pypesto/hierarchical/inner_calculator_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 In case of semi-quantitative or qualitative measurements, this class is used
 to collect hierarchical inner calculators for each data type and merge their results.
 """
 
 from __future__ import annotations
 
 import copy
-from typing import Sequence, Union
+from collections.abc import Sequence
+from typing import Union
 
 import numpy as np
 
 from ..C import (
     AMICI_SIGMAY,
     AMICI_SSIGMAY,
     AMICI_SSIGMAZ,
@@ -27,17 +28,18 @@
     ORDINAL,
     ORDINAL_OPTIONS,
     RDATAS,
     RELATIVE,
     RES,
     SEMIQUANTITATIVE,
     SPLINE_APPROXIMATION_OPTIONS,
+    SPLINE_KNOTS,
     SPLINE_RATIO,
     SRES,
-    X_INNER_OPT,
+    InnerParameterType,
     ModeType,
 )
 from ..objective.amici.amici_calculator import AmiciCalculator
 from ..objective.amici.amici_util import (
     add_sim_grad_to_opt_grad,
     filter_return_dict,
     init_return_values,
@@ -55,16 +57,16 @@
 from .relative import RelativeAmiciCalculator, RelativeInnerProblem
 from .semiquantitative import (
     SemiquantCalculator,
     SemiquantInnerSolver,
     SemiquantProblem,
 )
 
-AmiciModel = Union['amici.Model', 'amici.ModelPtr']
-AmiciSolver = Union['amici.Solver', 'amici.SolverPtr']
+AmiciModel = Union["amici.Model", "amici.ModelPtr"]
+AmiciSolver = Union["amici.Solver", "amici.SolverPtr"]
 
 
 class InnerCalculatorCollector(AmiciCalculator):
     """Class to collect inner calculators in case of non-quantitative data types.
 
     Upon import of a petab problem, the PEtab importer checks whether there are
     non-quantitative data types. If so, it creates an instance of this class
@@ -84,52 +86,49 @@
     inner_options:
         Options for the inner problems and solvers.
     """
 
     def __init__(
         self,
         data_types: set[str],
-        petab_problem: 'petab.Problem',
+        petab_problem: petab.Problem,
         model: AmiciModel,
-        edatas: list['amici.ExpData'],
+        edatas: list[amici.ExpData],
         inner_options: dict,
     ):
         super().__init__()
         self.validate_options(inner_options)
 
         self.data_types = data_types
         self.inner_calculators: list[
             AmiciCalculator
-        ] = (
-            []
-        )  # TODO make into a dictionary (future PR, together with .hierarchical of Problem)
+        ] = []  # TODO make into a dictionary (future PR, together with .hierarchical of Problem)
         self.construct_inner_calculators(
             petab_problem, model, edatas, inner_options
         )
 
         self.quantitative_data_mask = self._get_quantitative_data_mask(edatas)
 
         self._known_least_squares_safe = False
+        self.semiquant_observable_ids = None
 
     def initialize(self):
         """Initialize."""
-        self.best_fval = np.inf
         for calculator in self.inner_calculators:
             calculator.initialize()
 
     def construct_inner_calculators(
         self,
-        petab_problem: 'petab.Problem',
+        petab_problem: petab.Problem,
         model: AmiciModel,
-        edatas: list['amici.ExpData'],
+        edatas: list[amici.ExpData],
         inner_options: dict,
     ):
         """Construct inner calculators for each data type."""
         self.necessary_par_dummy_values = {}
-        self.best_fval = np.inf
 
         if RELATIVE in self.data_types:
             relative_inner_problem = RelativeInnerProblem.from_petab_amici(
                 petab_problem, model, edatas
             )
             self.necessary_par_dummy_values.update(
                 relative_inner_problem.get_dummy_values(scaled=True)
@@ -175,14 +174,20 @@
             semiquant_calculator = SemiquantCalculator(
                 semiquant_problem, semiquant_inner_solver
             )
             self.necessary_par_dummy_values.update(
                 semiquant_problem.get_noise_dummy_values(scaled=True)
             )
             self.inner_calculators.append(semiquant_calculator)
+            self.semiquant_observable_ids = [
+                model.getObservableIds()[group - 1]
+                for group in semiquant_problem.get_groups_for_xs(
+                    InnerParameterType.SPLINE
+                )
+            ]
 
         if self.data_types - {
             RELATIVE,
             ORDINAL,
             CENSORED,
             SEMIQUANTITATIVE,
         }:
@@ -209,19 +214,19 @@
                 key not in ORDINAL_OPTIONS
                 and key not in SPLINE_APPROXIMATION_OPTIONS
             ):
                 raise ValueError(f"Unknown inner option {key}.")
 
     def _get_quantitative_data_mask(
         self,
-        edatas: list['amici.ExpData'],
+        edatas: list[amici.ExpData],
     ) -> list[np.ndarray]:
         # transform experimental data
         edatas = [
-            amici.numpy.ExpDataView(edata)['observedData'] for edata in edatas
+            amici.numpy.ExpDataView(edata)["observedData"] for edata in edatas
         ]
 
         quantitative_data_mask = [
             np.ones_like(edata, dtype=bool) for edata in edatas
         ]
 
         # iterate over inner problems
@@ -230,14 +235,18 @@
             # Remove inner parameter masks from quantitative data mask
             for inner_par in inner_parameters:
                 for cond_idx, condition_mask in enumerate(
                     quantitative_data_mask
                 ):
                     condition_mask[inner_par.ixs[cond_idx]] = False
 
+        # Put to False all entries that have a nan value in the edata
+        for condition_mask, edata in zip(quantitative_data_mask, edatas):
+            condition_mask[np.isnan(edata)] = False
+
         # If there is no quantitative data, return None
         if not all(mask.any() for mask in quantitative_data_mask):
             return None
 
         return quantitative_data_mask
 
     def get_inner_par_ids(self) -> list[str]:
@@ -368,27 +377,24 @@
                 amici_solver=amici_solver,
                 edatas=edatas,
                 n_threads=n_threads,
                 x_ids=x_ids,
                 parameter_mapping=parameter_mapping,
                 fim_for_hess=fim_for_hess,
             )
-            # only return inner parameters if the objective value improved
-            if ret[FVAL] > self.best_fval:
-                ret[INNER_PARAMETERS] = None
             return filter_return_dict(ret)
 
         # get dimension of outer problem
         dim = len(x_ids)
 
         # initialize return values
         nllh, snllh, s2nllh, chi2, res, sres = init_return_values(
             sensi_orders, mode, dim
         )
-        all_inner_pars = {}
+        spline_knots = None
         interpretable_inner_pars = []
 
         # set order in solver
         sensi_order = 0
         if sensi_orders:
             sensi_order = max(sensi_orders)
 
@@ -419,15 +425,15 @@
             ret = {
                 FVAL: nllh,
                 GRAD: snllh,
                 HESS: s2nllh,
                 RES: res,
                 SRES: sres,
                 RDATAS: rdatas,
-                X_INNER_OPT: all_inner_pars,
+                SPLINE_KNOTS: None,
                 INNER_PARAMETERS: None,
             }
             ret[FVAL] = np.inf
             # if the gradient was requested,
             # we need to provide some value for it
             if 1 in sensi_orders:
                 ret[GRAD] = np.full(shape=len(x_ids), fill_value=np.nan)
@@ -445,18 +451,18 @@
                         r[AMICI_SSIGMAZ] is not None
                         and np.any(r[AMICI_SSIGMAZ])
                     )
                 )
                 for r in rdatas
             ):
                 raise RuntimeError(
-                    'Cannot use least squares solver with'
-                    'parameter dependent sigma! Support can be '
-                    'enabled via '
-                    'amici_model.setAddSigmaResiduals().'
+                    "Cannot use least squares solver with"
+                    "parameter dependent sigma! Support can be "
+                    "enabled via "
+                    "amici_model.setAddSigmaResiduals()."
                 )
             self._known_least_squares_safe = True  # don't check this again
 
         # call inner calculators and collect results
         for calculator in self.inner_calculators:
             inner_result = calculator(
                 x_dct=x_dct,
@@ -471,17 +477,19 @@
                 fim_for_hess=fim_for_hess,
                 rdatas=rdatas,
             )
             nllh += inner_result[FVAL]
             if 1 in sensi_orders:
                 snllh += inner_result[GRAD]
 
-            all_inner_pars.update(inner_result[X_INNER_OPT])
-            if INNER_PARAMETERS in inner_result:
-                interpretable_inner_pars.extend(inner_result[INNER_PARAMETERS])
+            inner_pars = inner_result.get(INNER_PARAMETERS)
+            if inner_pars is not None:
+                interpretable_inner_pars.extend(inner_pars)
+            if SPLINE_KNOTS in inner_result:
+                spline_knots = inner_result[SPLINE_KNOTS]
 
         # add the quantitative data contribution
         if self.quantitative_data_mask is not None:
             quantitative_result = calculate_quantitative_result(
                 rdatas=rdatas,
                 sensi_orders=sensi_orders,
                 edatas=edatas,
@@ -501,24 +509,20 @@
             GRAD: snllh,
             HESS: s2nllh,
             RES: res,
             SRES: sres,
             RDATAS: rdatas,
         }
 
-        # Add inner parameters to return dict
-        # only if the objective value improved.
-        if ret[FVAL] < self.best_fval:
-            ret[X_INNER_OPT] = all_inner_pars
-            ret[INNER_PARAMETERS] = (
-                interpretable_inner_pars
-                if len(interpretable_inner_pars) > 0
-                else None
-            )
-            self.best_fval = ret[FVAL]
+        ret[INNER_PARAMETERS] = (
+            interpretable_inner_pars
+            if len(interpretable_inner_pars) > 0
+            else None
+        )
+        ret[SPLINE_KNOTS] = spline_knots
 
         return filter_return_dict(ret)
 
 
 def calculate_quantitative_result(
     rdatas: list[amici.ReturnDataView],
     edatas: list[amici.ExpData],
@@ -533,26 +537,25 @@
     """Calculate the function values from rdatas and return as dict."""
     nllh, snllh, s2nllh, chi2, res, sres = init_return_values(
         sensi_orders, mode, dim
     )
 
     # transform experimental data
     edatas = [
-        amici.numpy.ExpDataView(edata)['observedData'] for edata in edatas
+        amici.numpy.ExpDataView(edata)["observedData"] for edata in edatas
     ]
 
     # calculate the function value
     for rdata, edata, mask in zip(rdatas, edatas, quantitative_data_mask):
         data_i = edata[mask]
         sim_i = rdata[AMICI_Y][mask]
         sigma_i = rdata[AMICI_SIGMAY][mask]
 
         nllh += 0.5 * np.nansum(
-            np.log(2 * np.pi * sigma_i**2)
-            + (data_i - sim_i) ** 2 / sigma_i**2
+            np.log(2 * np.pi * sigma_i**2) + (data_i - sim_i) ** 2 / sigma_i**2
         )
 
     # calculate the gradient if requested
     if 1 in sensi_orders:
         parameter_map_sim_var = [
             cond_par_map.map_sim_var for cond_par_map in parameter_mapping
         ]
@@ -597,17 +600,15 @@
                             - (data_i - sim_i) ** 2 / sigma_i**2
                         )
                         / sigma_i
                     ),
                 ),
                 axis=1,
             ) + np.nansum(
-                np.multiply(
-                    sensitivities_i, ((sim_i - data_i) / sigma_i**2)
-                ),
+                np.multiply(sensitivities_i, ((sim_i - data_i) / sigma_i**2)),
                 axis=1,
             )
             add_sim_grad_to_opt_grad(
                 par_opt_ids=par_opt_ids,
                 par_sim_ids=par_sim_ids,
                 condition_map_sim_var=condition_map_sim_var,
                 sim_grad=gradient_for_condition,
```

### Comparing `pypesto-0.4.2/pypesto/hierarchical/ordinal/__init__.py` & `pypesto-0.5.0/pypesto/hierarchical/ordinal/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.2/pypesto/hierarchical/ordinal/calculator.py` & `pypesto-0.5.0/pypesto/hierarchical/ordinal/calculator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Definition of an optimal scaling calculator class."""
 
 import copy
-from typing import Sequence
+from collections.abc import Sequence
 
 import numpy as np
 
 from ...C import (
     AMICI_SIGMAY,
     AMICI_SSIGMAY,
     AMICI_SY,
@@ -13,15 +13,14 @@
     FVAL,
     GRAD,
     HESS,
     MODE_RES,
     RDATAS,
     RES,
     SRES,
-    X_INNER_OPT,
 )
 from ...objective.amici.amici_calculator import (
     AmiciCalculator,
     AmiciModel,
     AmiciSolver,
 )
 from ...objective.amici.amici_util import (
@@ -64,15 +63,15 @@
         self.inner_problem = inner_problem
 
         if inner_solver is None:
             inner_solver = OrdinalInnerSolver()
         self.inner_solver = inner_solver
         if (
             self.inner_problem.method
-            is not self.inner_solver.options['method']
+            is not self.inner_solver.options["method"]
         ):
             raise ValueError(
                 f"The inner problem method {self.inner_problem.method} and the inner solver method {self.inner_solver.options['method']} have to coincide."
             )
 
     def initialize(self):
         """Initialize."""
@@ -82,20 +81,20 @@
     def __call__(
         self,
         x_dct: dict,
         sensi_orders: tuple[int, ...],
         mode: str,
         amici_model: AmiciModel,
         amici_solver: AmiciSolver,
-        edatas: list['amici.ExpData'],
+        edatas: list["amici.ExpData"],
         n_threads: int,
         x_ids: Sequence[str],
         parameter_mapping: ParameterMapping,
         fim_for_hess: bool,
-        rdatas: list['amici.ReturnData'] = None,
+        rdatas: list["amici.ReturnData"] = None,
     ):
         """Perform the actual AMICI call.
 
         Parameters
         ----------
         x_dct:
             Parameters for which to compute function value and derivatives.
@@ -122,15 +121,15 @@
             AMICI simulation return data. In case the calculator is part of
             the :class:`pypesto.objective.amici.InnerCalculatorCollector`,
             it will already simulate the model and pass the results here.
 
         Returns
         -------
         inner_result:
-            A dict containing the calculation results: FVAL, GRAD, RDATAS and X_INNER_OPT.
+            A dict containing the calculation results: FVAL, GRAD, RDATAS.
         """
         if mode == MODE_RES:
             raise ValueError(
                 "Optimal scaling method cannot be called with residual mode."
             )
         if 2 in sensi_orders:
             raise ValueError(
@@ -174,15 +173,14 @@
         inner_result = {
             FVAL: nllh,
             GRAD: snllh,
             HESS: s2nllh,
             RES: res,
             SRES: sres,
             RDATAS: rdatas,
-            X_INNER_OPT: self.inner_problem.get_inner_parameter_dictionary(),
         }
 
         # if any amici simulation failed, it's unlikely we can compute
         # meaningful inner parameters, so we better just fail early.
         if any(rdata.status != amici.AMICI_SUCCESS for rdata in rdatas):
             inner_result[FVAL] = np.inf
             # if the gradient was requested,
@@ -197,21 +195,17 @@
         sigma = [rdata[AMICI_SIGMAY] for rdata in rdatas]
 
         # compute optimal inner parameters
         x_inner_opt = self.inner_solver.solve(self.inner_problem, sim, sigma)
         inner_result[FVAL] = self.inner_solver.calculate_obj_function(
             x_inner_opt
         )
-        inner_result[
-            X_INNER_OPT
-        ] = self.inner_problem.get_inner_parameter_dictionary()
 
         # calculate analytical gradients if requested
         if sensi_order > 0:
-            # print([opt['fun'] for opt in x_inner_opt])
             sy = [rdata[AMICI_SY] for rdata in rdatas]
             ssigma = [rdata[AMICI_SSIGMAY] for rdata in rdatas]
             inner_result[GRAD] = self.inner_solver.calculate_gradients(
                 problem=self.inner_problem,
                 x_inner_opt=x_inner_opt,
                 sim=sim,
                 sy=sy,
```

### Comparing `pypesto-0.4.2/pypesto/hierarchical/ordinal/parameter.py` & `pypesto-0.5.0/pypesto/hierarchical/ordinal/parameter.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.2/pypesto/hierarchical/ordinal/problem.py` & `pypesto-0.5.0/pypesto/hierarchical/ordinal/problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,16 +149,16 @@
                 self.groups[group][C_MATRIX] = self.initialize_c(group)
 
                 self.groups[group][W_MATRIX] = self.initialize_w(group)
 
                 self.groups[group][W_DOT_MATRIX] = self.initialize_w(group)
             else:
                 raise ValueError(
-                    'Censoring types of optimal scaling parameters of a group '
-                    'have to either be all None, or all not None.'
+                    "Censoring types of optimal scaling parameters of a group "
+                    "have to either be all None, or all not None."
                 )
 
     def initialize(self) -> None:
         """Initialize the subproblem."""
         # Initialize all parameter values.
         for x in self.xs.values():
             x.initialize()
@@ -168,18 +168,18 @@
             self.groups[group][SURROGATE_DATA] = np.zeros(
                 self.groups[group][NUM_DATAPOINTS]
             )
 
     @staticmethod
     def from_petab_amici(
         petab_problem: petab.Problem,
-        amici_model: 'amici.Model',
-        edatas: list['amici.ExpData'],
+        amici_model: "amici.Model",
+        edatas: list["amici.ExpData"],
         method: str = None,
-    ) -> 'OrdinalProblem':
+    ) -> "OrdinalProblem":
         """Construct the inner problem from the `petab_problem`."""
         if not method:
             method = REDUCED
 
         return optimal_scaling_inner_problem_from_petab_problem(
             petab_problem, amici_model, edatas, method
         )
@@ -384,18 +384,18 @@
 
         interval_range = max_simulation / (2 * len(xs) + 1)
         interval_gap = max_simulation / (4 * (len(xs) - 1) + 1)
 
         d = np.zeros(self.groups[group][NUM_CONSTR_FULL])
 
         d[
-            2 * self.groups[group][NUM_DATAPOINTS]
-            + 1 : 2 * self.groups[group][NUM_DATAPOINTS]
+            2 * self.groups[group][NUM_DATAPOINTS] + 1 : 2
+            * self.groups[group][NUM_DATAPOINTS]
             + self.groups[group][NUM_CATEGORIES]
-        ] = (interval_gap + eps)
+        ] = interval_gap + eps
 
         d[
             2 * self.groups[group][NUM_DATAPOINTS]
             + self.groups[group][NUM_CATEGORIES] :
         ] = interval_range
         return d
 
@@ -411,16 +411,16 @@
         max_sy = sy_all[max_sim_idx]
         dd_dtheta = np.zeros(self.groups[group][NUM_CONSTR_FULL])
 
         dinterval_range_dtheta = max_sy / (2 * len(xs) + 1)
         dinterval_gap_dtheta = max_sy / (4 * (len(xs) - 1) + 1)
 
         dd_dtheta[
-            2 * self.groups[group][NUM_DATAPOINTS]
-            + 1 : 2 * self.groups[group][NUM_DATAPOINTS]
+            2 * self.groups[group][NUM_DATAPOINTS] + 1 : 2
+            * self.groups[group][NUM_DATAPOINTS]
             + self.groups[group][NUM_CATEGORIES]
         ] = dinterval_gap_dtheta
 
         dd_dtheta[
             2 * self.groups[group][NUM_DATAPOINTS]
             + self.groups[group][NUM_CATEGORIES] :
         ] = dinterval_range_dtheta
@@ -471,31 +471,31 @@
         for x_id, x in self.xs.items():
             inner_par_dict[x_id] = x.value
         return inner_par_dict
 
 
 def optimal_scaling_inner_problem_from_petab_problem(
     petab_problem: petab.Problem,
-    amici_model: 'amici.Model',
-    edatas: list['amici.ExpData'],
+    amici_model: "amici.Model",
+    edatas: list["amici.ExpData"],
     method: str,
 ):
     """Construct the inner problem from the `petab_problem`."""
     # inner parameters
     inner_parameters = optimal_scaling_inner_parameters_from_measurement_df(
         petab_problem.measurement_df, method, amici_model
     )
 
     # used indices for all measurement specific parameters
     ixs = optimal_scaling_ixs_for_measurement_specific_parameters(
         petab_problem, amici_model, inner_parameters
     )
 
     # transform experimental data
-    data = [amici.numpy.ExpDataView(edata)['observedData'] for edata in edatas]
+    data = [amici.numpy.ExpDataView(edata)["observedData"] for edata in edatas]
 
     # matrixify
     ix_matrices = ix_matrices_from_arrays(ixs, data)
 
     # assign matrices
     for par in inner_parameters:
         par.ixs = ix_matrices[par.inner_parameter_id]
@@ -507,15 +507,15 @@
         method=method,
     )
 
 
 def optimal_scaling_inner_parameters_from_measurement_df(
     df: pd.DataFrame,
     method: str,
-    amici_model: 'amici.Model',
+    amici_model: "amici.Model",
 ) -> list[OrdinalParameter]:
     """Create list of inner free parameters from PEtab measurement table dependent on the method provided."""
     df = df.reset_index()
 
     observable_ids = amici_model.getObservableIds()
 
     estimate = get_estimate_for_method(method)
@@ -529,15 +529,15 @@
 
         observable_df = df[df[OBSERVABLE_ID] == observable_id]
 
         if all(observable_df[MEASUREMENT_TYPE] == ORDINAL):
             # Add optimal scaling parameters for ordinal measurements.
             for par_type, par_estimate in zip(par_types, estimate):
                 for _, row in observable_df.iterrows():
-                    par_id = f'{par_type}_{observable_id}_{row[MEASUREMENT_TYPE]}_{int(row[MEASUREMENT_CATEGORY])}'
+                    par_id = f"{par_type}_{observable_id}_{row[MEASUREMENT_TYPE]}_{int(row[MEASUREMENT_CATEGORY])}"
 
                     # Create only one set of bound parameters per category of a group.
                     if par_id not in [
                         inner_par.inner_parameter_id
                         for inner_par in inner_parameters
                     ]:
                         inner_parameters.append(
@@ -566,15 +566,15 @@
             )
             for par_type in par_types:
                 for _, row in censored_df.iterrows():
                     category = int(
                         unique_censoring_bounds.index(row[CENSORING_BOUNDS])
                         + 1
                     )
-                    par_id = f'{par_type}_{observable_id}_{row[MEASUREMENT_TYPE]}_{category}'
+                    par_id = f"{par_type}_{observable_id}_{row[MEASUREMENT_TYPE]}_{category}"
                     # Create only one set of bound parameters per category of a group.
                     if par_id not in [
                         inner_par.inner_parameter_id
                         for inner_par in inner_parameters
                     ]:
                         inner_parameters.append(
                             OrdinalParameter(
@@ -607,16 +607,16 @@
     if method == STANDARD:
         estimate_lb = True
 
     return estimate_lb, estimate_ub
 
 
 def optimal_scaling_ixs_for_measurement_specific_parameters(
-    petab_problem: 'petab.Problem',
-    amici_model: 'amici.Model',
+    petab_problem: "petab.Problem",
+    amici_model: "amici.Model",
     inner_parameters: list[OrdinalParameter],
 ) -> dict[str, list[tuple[int, int, int]]]:
     """Create mapping of parameters to measurements.
 
     Returns
     -------
     A dictionary mapping parameter ID to a list of
```

### Comparing `pypesto-0.4.2/pypesto/hierarchical/ordinal/solver.py` & `pypesto-0.5.0/pypesto/hierarchical/ordinal/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,37 +71,38 @@
 
     def validate_options(self):
         """Validate the current options dictionary."""
         if self.options[METHOD] not in [STANDARD, REDUCED]:
             raise ValueError(
                 f"Inner solver method cannot be {self.options[METHOD]}. Please enter either {STANDARD} or {REDUCED}"
             )
-        elif type(self.options[REPARAMETERIZED]) is not bool:
+        elif not isinstance(self.options[REPARAMETERIZED], bool):
             raise ValueError(
                 f"Inner solver option 'reparameterized' has to be boolean, not {type(self.options[REPARAMETERIZED])}."
             )
         elif self.options[INTERVAL_CONSTRAINTS] not in [MAX, MAXMIN]:
             raise ValueError(
                 f"Inner solver method cannot be {self.options[INTERVAL_CONSTRAINTS]}. Please enter either {MAX} or {MAXMIN}"
             )
-        elif type(self.options[MIN_GAP]) is not float:
+        elif not isinstance(self.options[MIN_GAP], float):
             raise ValueError(
                 f"Inner solver option 'reparameterized' has to be a float, not {type(self.options[MIN_GAP])}."
             )
         elif (
             self.options[METHOD] == STANDARD and self.options[REPARAMETERIZED]
         ):
             raise NotImplementedError(
-                'Combining standard approach with '
-                'reparameterization not implemented.'
+                "Combining standard approach with "
+                "reparameterization not implemented."
             )
         elif self.options[METHOD] == STANDARD:
             warnings.warn(
-                'Standard approach is not recommended, as it is less efficient.'
-                'Please consider using the reduced approach instead.'
+                "Standard approach is not recommended, as it is less efficient."
+                "Please consider using the reduced approach instead.",
+                stacklevel=2,
             )
         # Check for any other options
         for key in self.options:
             if key not in self.get_default_options():
                 raise ValueError(
                     f"Unknown OptimalScalingInnerSolver option {key}."
                 )
@@ -181,15 +182,15 @@
         -------
         Inner objective function value.
         """
         if False in [
             x_inner_opt[idx][SCIPY_SUCCESS] for idx in range(len(x_inner_opt))
         ]:
             obj = np.inf
-            warnings.warn("Inner optimization failed.")
+            warnings.warn("Inner optimization failed.", stacklevel=2)
         else:
             obj = np.sum(
                 [
                     x_inner_opt[idx][SCIPY_FUN]
                     for idx in range(len(x_inner_opt))
                 ]
             )
@@ -459,15 +460,15 @@
         Residual for group.
     """
     from scipy import linalg
 
     mu = linalg.lstsq(
         problem.groups[group][C_MATRIX].transpose(),
         -2 * residual.dot(problem.groups[group][W_MATRIX]),
-        lapack_driver='gelsy',
+        lapack_driver="gelsy",
     )
     return mu[0]
 
 
 def get_xi(
     group: int,
     problem: OrdinalProblem,
@@ -561,17 +562,18 @@
         interval_gap,
         options,
     )
     try:
         results = minimize(obj_surr, jac=grad_surr, **inner_options)
     except ValueError:
         warnings.warn(
-            "x0 violate bound constraints. Retrying with array of zeros."
+            "x0 violate bound constraints. Retrying with array of zeros.",
+            stacklevel=2,
         )
-        inner_options['x0'] = np.zeros(len(inner_options['x0']))
+        inner_options["x0"] = np.zeros(len(inner_options["x0"]))
         results = minimize(obj_surr, jac=grad_surr, **inner_options)
 
     return results
 
 
 def get_inner_optimization_options(
     category_upper_bounds: list[OrdinalParameter],
@@ -608,15 +610,15 @@
         last_opt_values = np.asarray([x.value for x in category_upper_bounds])
     elif options[METHOD] == STANDARD:
         last_opt_values = np.ravel(
             [
                 np.asarray([x.value for x in category_lower_bounds]),
                 np.asarray([x.value for x in category_upper_bounds]),
             ],
-            'F',
+            "F",
         )
 
     if options[METHOD] == REDUCED:
         parameter_length = len(category_upper_bounds)
         if len(np.nonzero(last_opt_values)) > 0:
             x0 = last_opt_values
         else:
@@ -647,29 +649,29 @@
 
         bounds = Bounds(
             [0.0] * parameter_length,
             [max_all + (interval_range + interval_gap) * parameter_length]
             * parameter_length,
         )
         inner_options = {
-            'x0': x0,
-            'method': 'L-BFGS-B',
-            'options': {'maxiter': 2000, 'ftol': 1e-10},
-            'bounds': bounds,
+            "x0": x0,
+            "method": "L-BFGS-B",
+            "options": {"maxiter": 2000, "ftol": 1e-10},
+            "bounds": bounds,
         }
     else:
         constraints = get_constraints_for_optimization(
             category_upper_bounds, sim, options
         )
 
         inner_options = {
-            'x0': x0,
-            'method': 'SLSQP',
-            'options': {'maxiter': 2000, 'ftol': 1e-10, 'disp': None},
-            'constraints': constraints,
+            "x0": x0,
+            "method": "SLSQP",
+            "options": {"maxiter": 2000, "ftol": 1e-10, "disp": None},
+            "constraints": constraints,
         }
     return inner_options
 
 
 def get_min_max(
     inner_parameters: list[OrdinalParameter], sim: list[np.ndarray]
 ) -> tuple[float, float]:
@@ -995,15 +997,15 @@
     if options[METHOD] == REDUCED:
         x_upper = optimal_scaling_bounds[x_category - 1]
         if x_category == 1:
             x_lower = 0
         elif x_category > 1:
             x_lower = optimal_scaling_bounds[x_category - 2] + interval_gap
         else:
-            raise ValueError('Category value needs to be larger than 0.')
+            raise ValueError("Category value needs to be larger than 0.")
     elif options[METHOD] == STANDARD:
         x_lower = optimal_scaling_bounds[2 * x_category - 2]
         x_upper = optimal_scaling_bounds[2 * x_category - 1]
     else:
         raise NotImplementedError(
             f"Unknown optimal scaling method {options[METHOD]}. "
             f"Please use {REDUCED} or {STANDARD}."
@@ -1032,15 +1034,15 @@
             np.ones(2 * num_categories + 1)
         )
         a = a[:-1, :-1]
         b = np.empty((2 * num_categories,))
         b[0] = 0
         b[1::2] = interval_range
         b[2::2] = interval_gap
-    ineq_cons = {'type': 'ineq', 'fun': lambda x: a.dot(x) - b}
+    ineq_cons = {"type": "ineq", "fun": lambda x: a.dot(x) - b}
 
     return ineq_cons
 
 
 def save_inner_parameters_to_inner_problem(
     category_upper_bounds: list[OrdinalParameter],
     group: int,
@@ -1138,15 +1140,15 @@
         np.log(2 * np.pi * quantitative_sigma**2)
         + (quantitative_data - quantitative_sim) ** 2 / quantitative_sigma**2
     )
 
     return_dictionary = {
         SCIPY_SUCCESS: True,
         SCIPY_FUN: obj,
-        SCIPY_X: np.ravel([cat_lb_values, cat_ub_values], order='F'),
+        SCIPY_X: np.ravel([cat_lb_values, cat_ub_values], order="F"),
     }
     return return_dictionary
 
 
 def calculate_censored_grad(
     category_upper_bounds: list[OrdinalParameter],
     category_lower_bounds: list[OrdinalParameter],
```

### Comparing `pypesto-0.4.2/pypesto/hierarchical/petab.py` & `pypesto-0.5.0/pypesto/hierarchical/petab.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,45 +2,44 @@
 
 from typing import Literal
 
 import pandas as pd
 import petab
 import sympy as sp
 from more_itertools import one
-from petab.C import ESTIMATE, LIN
-from petab.C import LOWER_BOUND as PETAB_LOWER_BOUND
 from petab.C import (
+    ESTIMATE,
+    LIN,
     NOISE_PARAMETERS,
     OBSERVABLE_ID,
     OBSERVABLE_PARAMETERS,
     OBSERVABLE_TRANSFORMATION,
     PARAMETER_SEPARATOR,
 )
+from petab.C import LOWER_BOUND as PETAB_LOWER_BOUND
 from petab.C import UPPER_BOUND as PETAB_UPPER_BOUND
 from petab.observables import get_formula_placeholders
 
 from ..C import (
     CENSORING_BOUNDS,
     CENSORING_TYPES,
     INNER_PARAMETER_BOUNDS,
     INTERVAL_CENSORED,
     LEFT_CENSORED,
-)
-from ..C import LOWER_BOUND as PYPESTO_LOWER_BOUND
-from ..C import (
     MEASUREMENT_CATEGORY,
     MEASUREMENT_TYPE,
     ORDINAL,
     PARAMETER_TYPE,
     RELATIVE,
     RIGHT_CENSORED,
     SEMIQUANTITATIVE,
+    InnerParameterType,
 )
+from ..C import LOWER_BOUND as PYPESTO_LOWER_BOUND
 from ..C import UPPER_BOUND as PYPESTO_UPPER_BOUND
-from ..C import InnerParameterType
 
 
 def correct_parameter_df_bounds(parameter_df: pd.DataFrame) -> pd.DataFrame:
     """Correct the bounds of inner parameters in a PEtab parameters table.
 
     Parameters
     ----------
@@ -300,15 +299,15 @@
 
     Returns
     -------
     The offset and scaling parameters.
     """
     formula, formula_inner_parameters = _get_symbolic_formula_from_measurement(
         measurement=measurement,
-        formula_type='observable',
+        formula_type="observable",
         petab_problem=petab_problem,
         inner_parameters=inner_parameters,
     )
 
     offset = None
     scaling = None
 
@@ -385,15 +384,15 @@
 
     Returns
     -------
     The sigma parameter.
     """
     formula, formula_inner_parameters = _get_symbolic_formula_from_measurement(
         measurement=measurement,
-        formula_type='noise',
+        formula_type="noise",
         petab_problem=petab_problem,
         inner_parameters=inner_parameters,
     )
 
     sigma = None
 
     for (
@@ -416,15 +415,15 @@
             raise ValueError("Unknown error: unexpected inner parameter type.")
 
     return sigma
 
 
 def _get_symbolic_formula_from_measurement(
     measurement: pd.Series,
-    formula_type: Literal['observable', 'noise'],
+    formula_type: Literal["observable", "noise"],
     petab_problem: petab.Problem,
     inner_parameters: dict[str, InnerParameterType],
 ) -> tuple[sp.Expr, dict[sp.Symbol, InnerParameterType]]:
     """Get a symbolic representation of a formula, with overrides overridden.
 
     Also performs some checks to ensure only valid numbers and types of inner
     parameters are in the formula.
@@ -443,43 +442,43 @@
     Returns
     -------
     The symbolic formula, and its inner parameters.
     """
     observable_id = measurement[OBSERVABLE_ID]
 
     formula_string = petab_problem.observable_df.loc[
-        observable_id, formula_type + 'Formula'
+        observable_id, formula_type + "Formula"
     ]
     symbolic_formula = sp.sympify(formula_string)
 
     formula_placeholders = get_formula_placeholders(
         formula_string=formula_string,
         observable_id=observable_id,
         override_type=formula_type,
     )
     if formula_placeholders:
-        overrides = measurement[formula_type + 'Parameters']
+        overrides = measurement[formula_type + "Parameters"]
         overrides = (
             overrides.split(PARAMETER_SEPARATOR)
             if isinstance(overrides, str)
             else [overrides]
         )
         subs = dict(zip(formula_placeholders, overrides))
         symbolic_formula = symbolic_formula.subs(subs)
 
     symbolic_formula_inner_parameters = {
         sp.Symbol(inner_parameter_id): inner_parameter_type
         for inner_parameter_id, inner_parameter_type in inner_parameters.items()
         if sp.Symbol(inner_parameter_id) in symbolic_formula.free_symbols
     }
 
-    if formula_type == 'noise':
+    if formula_type == "noise":
         max_parameters = 1
         expected_inner_parameter_types = [InnerParameterType.SIGMA]
-    elif formula_type == 'observable':
+    elif formula_type == "observable":
         max_parameters = 2
         expected_inner_parameter_types = [
             InnerParameterType.OFFSET,
             InnerParameterType.SCALING,
         ]
 
     if len(symbolic_formula_inner_parameters) > max_parameters:
```

### Comparing `pypesto-0.4.2/pypesto/hierarchical/relative/__init__.py` & `pypesto-0.5.0/pypesto/hierarchical/relative/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.2/pypesto/hierarchical/relative/calculator.py` & `pypesto-0.5.0/pypesto/hierarchical/relative/calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import copy
-from typing import Optional, Sequence
+from collections.abc import Sequence
 
 import numpy as np
 
 try:
     import amici
     import amici.parameter_mapping
     from amici.parameter_mapping import ParameterMapping
@@ -21,15 +21,14 @@
     GRAD,
     HESS,
     INNER_PARAMETERS,
     INNER_RDATAS,
     RDATAS,
     RES,
     SRES,
-    X_INNER_OPT,
     ModeType,
 )
 from ...objective.amici.amici_calculator import (
     AmiciCalculator,
     AmiciModel,
     AmiciSolver,
 )
@@ -43,15 +42,15 @@
 
 class RelativeAmiciCalculator(AmiciCalculator):
     """A calculator that is passed as `calculator` to the pypesto.AmiciObjective."""
 
     def __init__(
         self,
         inner_problem: AmiciInnerProblem,
-        inner_solver: Optional[InnerSolver] = None,
+        inner_solver: InnerSolver | None = None,
     ):
         """Initialize the calculator from the given problem.
 
         Arguments
         ---------
         inner_problem:
             The inner problem of a hierarchical optimization problem.
@@ -80,15 +79,15 @@
         amici_model: AmiciModel,
         amici_solver: AmiciSolver,
         edatas: list[amici.ExpData],
         n_threads: int,
         x_ids: Sequence[str],
         parameter_mapping: ParameterMapping,
         fim_for_hess: bool,
-        rdatas: list['amici.ReturnData'] = None,
+        rdatas: list[amici.ReturnData] = None,
     ):
         """Perform the actual AMICI call, with hierarchical optimization.
 
         The return object also includes the simulation results that were
         generated to solve the inner problem, as well as the parameters that
         solver the inner problem.
 
@@ -119,28 +118,28 @@
             AMICI simulation return data. In case the calculator is part of
             the :class:`pypesto.objective.amici.InnerCalculatorCollector`,
             it will already simulate the model and pass the results here.
 
         Returns
         -------
         inner_result:
-            A dict containing the calculation results: FVAL, GRAD, RDATAS and X_INNER_OPT.
+            A dict containing the calculation results: FVAL, GRAD, RDATAS and INNER_PARAMETERS.
         """
         if not self.inner_problem.check_edatas(edatas=edatas):
             raise ValueError(
-                'The experimental data provided to this call differs from '
-                'the experimental data used to setup the hierarchical '
-                'optimizer.'
+                "The experimental data provided to this call differs from "
+                "the experimental data used to setup the hierarchical "
+                "optimizer."
             )
 
         if (
-            amici_solver.getSensitivityMethod()
-            == amici.SensitivityMethod_adjoint
-            or 2 in sensi_orders
-        ):
+            1 in sensi_orders
+            and amici_solver.getSensitivityMethod()
+            == amici.SensitivityMethod.adjoint
+        ) or 2 in sensi_orders:
             inner_result, inner_parameters = self.call_amici_twice(
                 x_dct=x_dct,
                 sensi_orders=sensi_orders,
                 mode=mode,
                 amici_model=amici_model,
                 amici_solver=amici_solver,
                 edatas=edatas,
@@ -160,19 +159,24 @@
                 n_threads=n_threads,
                 x_ids=x_ids,
                 parameter_mapping=parameter_mapping,
                 fim_for_hess=fim_for_hess,
                 rdatas=rdatas,
             )
 
-        inner_result[X_INNER_OPT] = {}
-        inner_result[INNER_PARAMETERS] = np.array(
-            [inner_parameters[x_id] for x_id in self.inner_problem.get_x_ids()]
+        inner_result[INNER_PARAMETERS] = (
+            np.array(
+                [
+                    inner_parameters[x_id]
+                    for x_id in self.inner_problem.get_x_ids()
+                ]
+            )
+            if inner_parameters is not None
+            else None
         )
-        # print("relative_inner_parameters: ", inner_parameters)
 
         return inner_result
 
     def call_amici_twice(
         self,
         x_dct: dict,
         sensi_orders: tuple[int],
@@ -218,16 +222,15 @@
             # for it
             if 1 in sensi_orders:
                 inner_result[GRAD] = np.full(shape=dim, fill_value=np.nan)
             if 2 in sensi_orders:
                 inner_result[HESS] = np.full(
                     shape=(dim, dim), fill_value=np.nan
                 )
-            inner_result[INNER_PARAMETERS] = None
-            return inner_result
+            return inner_result, None
 
         inner_parameters = self.inner_solver.solve(
             problem=self.inner_problem,
             sim=[rdata[AMICI_Y] for rdata in rdatas],
             sigma=[rdata[AMICI_SIGMAY] for rdata in rdatas],
             scaled=True,
         )
@@ -262,15 +265,15 @@
         amici_model: AmiciModel,
         amici_solver: AmiciSolver,
         edatas: list[amici.ExpData],
         n_threads: int,
         x_ids: Sequence[str],
         parameter_mapping: ParameterMapping,
         fim_for_hess: bool,
-        rdatas: list['amici.ReturnData'] = None,
+        rdatas: list[amici.ReturnData] = None,
     ):
         """Calculate directly via solver calculate methods.
 
         This is possible if the forward method is used, and the Hessian is not
         requested. In this case, the objective function and gradient are computed
         directly using the solver methods.
         """
@@ -321,15 +324,15 @@
         # meaningful inner parameters, so we better just fail early.
         if any(rdata.status != amici.AMICI_SUCCESS for rdata in rdatas):
             inner_result[FVAL] = np.inf
             if 1 in sensi_orders:
                 inner_result[GRAD] = np.full(
                     shape=len(x_ids), fill_value=np.nan
                 )
-            return filter_return_dict(inner_result)
+            return filter_return_dict(inner_result), None
 
         inner_parameters = self.inner_solver.solve(
             problem=self.inner_problem,
             sim=[rdata[AMICI_Y] for rdata in rdatas],
             sigma=[rdata[AMICI_SIGMAY] for rdata in rdatas],
             scaled=True,
         )
```

### Comparing `pypesto-0.4.2/pypesto/hierarchical/relative/problem.py` & `pypesto-0.5.0/pypesto/hierarchical/relative/problem.py`

 * *Files 14% similar despite different names*

```diff
@@ -53,18 +53,18 @@
     """
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     @staticmethod
     def from_petab_amici(
-        petab_problem: 'petab.Problem',
-        amici_model: 'amici.Model',
-        edatas: list['amici.ExpData'],
-    ) -> 'RelativeInnerProblem':
+        petab_problem: "petab.Problem",
+        amici_model: "amici.Model",
+        edatas: list["amici.ExpData"],
+    ) -> "RelativeInnerProblem":
         """Create an InnerProblem from a PEtab problem and AMICI objects."""
         return inner_problem_from_petab_problem(
             petab_problem, amici_model, edatas
         )
 
     def check_edatas(self, edatas: list[amici.ExpData]) -> bool:
         """Check for consistency in data.
@@ -81,31 +81,31 @@
         Returns
         -------
         Whether the data sets are consistent.
         """
         # TODO replace but edata1==edata2 once this makes it into amici
         #  https://github.com/AMICI-dev/AMICI/issues/1880
         data = [
-            amici.numpy.ExpDataView(edata)['observedData'] for edata in edatas
+            amici.numpy.ExpDataView(edata)["observedData"] for edata in edatas
         ]
 
         if len(self.data) != len(data):
             return False
 
         for data0, data1 in zip(self.data, data):
             if not np.array_equal(data0, data1, equal_nan=True):
                 return False
 
         return True
 
 
 def inner_problem_from_petab_problem(
-    petab_problem: 'petab.Problem',
-    amici_model: 'amici.Model',
-    edatas: list['amici.ExpData'],
+    petab_problem: "petab.Problem",
+    amici_model: "amici.Model",
+    edatas: list["amici.ExpData"],
 ) -> AmiciInnerProblem:
     """
     Create inner problem from PEtab problem.
 
     Hierarchical optimization is a pypesto-specific PEtab extension.
     """
     import amici
@@ -119,32 +119,32 @@
 
     # used indices for all measurement specific parameters
     ixs = ixs_for_measurement_specific_parameters(
         petab_problem, amici_model, x_ids
     )
 
     # transform experimental data
-    data = [amici.numpy.ExpDataView(edata)['observedData'] for edata in edatas]
+    data = [amici.numpy.ExpDataView(edata)["observedData"] for edata in edatas]
 
     # matrixify
     ix_matrices = ix_matrices_from_arrays(ixs, data)
 
     # assign matrices
     for par in inner_parameters:
         par.ixs = ix_matrices[par.inner_parameter_id]
 
     par_group_types = {
-        tuple(obs_pars.split(';')): (
+        tuple(obs_pars.split(";")): (
             petab_problem.parameter_df.loc[obs_par, PARAMETER_TYPE]
-            for obs_par in obs_pars.split(';')
+            for obs_par in obs_pars.split(";")
         )
         for (obs_id, obs_pars), _ in petab_problem.measurement_df.groupby(
             [petab.OBSERVABLE_ID, petab.OBSERVABLE_PARAMETERS], dropna=True
         )
-        if ';' in obs_pars  # prefilter for at least 2 observable parameters
+        if ";" in obs_pars  # prefilter for at least 2 observable parameters
     }
 
     coupled_pars = {
         group
         for group, types in par_group_types.items()
         if (
             (InnerParameterType.SCALING in types)
@@ -228,16 +228,16 @@
             )
         )
 
     return parameters
 
 
 def ixs_for_measurement_specific_parameters(
-    petab_problem: 'petab.Problem',
-    amici_model: 'amici.Model',
+    petab_problem: "petab.Problem",
+    amici_model: "amici.Model",
     x_ids: list[str],
 ) -> dict[str, list[tuple[int, int, int]]]:
     """
     Create mapping of parameters to measurements.
 
     Returns
     -------
```

### Comparing `pypesto-0.4.2/pypesto/hierarchical/relative/solver.py` & `pypesto-0.5.0/pypesto/hierarchical/relative/solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,16 +222,16 @@
         problem:
             The inner problem to solve.
         rdatas:
             The rdatas to apply the inner parameters to.
         inner_parameters:
             The inner parameters to apply to the rdatas.
         """
-        sim = [rdata['y'] for rdata in rdatas]
-        sigma = [rdata['sigmay'] for rdata in rdatas]
+        sim = [rdata["y"] for rdata in rdatas]
+        sigma = [rdata["sigmay"] for rdata in rdatas]
 
         # apply offsets, scalings and sigmas
         for x in problem.get_xs_for_type(InnerParameterType.SCALING):
             apply_scaling(
                 scaling_value=inner_parameters[x.inner_parameter_id],
                 sim=sim,
                 mask=x.ixs,
@@ -418,19 +418,19 @@
         if self.minimize_kwargs is None:
             self.minimize_kwargs = {}
         self.n_cached = n_cached
         self.problem_kwargs = problem_kwargs
         if self.problem_kwargs is None:
             self.problem_kwargs = {}
 
-        self.minimize_kwargs['n_starts'] = self.minimize_kwargs.get(
-            'n_starts', 1
+        self.minimize_kwargs["n_starts"] = self.minimize_kwargs.get(
+            "n_starts", 1
         )
-        self.minimize_kwargs['progress_bar'] = self.minimize_kwargs.get(
-            'progress_bar', False
+        self.minimize_kwargs["progress_bar"] = self.minimize_kwargs.get(
+            "progress_bar", False
         )
 
         self.x_guesses = None
         self.dummy_lb = -1e20
         self.dummy_ub = +1e20
         self.user_specified_lb = None
         self.user_specified_ub = None
@@ -513,15 +513,15 @@
         )
         pypesto_problem.set_x_guesses(
             x_guesses[:, pypesto_problem.x_free_indices]
         )
 
         # perform the actual optimization
         result = minimize(pypesto_problem, **self.minimize_kwargs)
-        best_par = result.optimize_result.list[0]['x']
+        best_par = result.optimize_result.list[0]["x"]
 
         # Check if the index of an optimized parameter on the dummy bound
         # is not in the list of specified bounds. If so, raise an error.
         if any(
             (
                 i not in self.user_specified_lb
                 for i, x in enumerate(best_par)
@@ -541,15 +541,15 @@
             )
 
         x_opt = dict(zip(pypesto_problem.x_names, best_par))
 
         # cache
         self.x_guesses = np.array(
             [
-                entry['x']
+                entry["x"]
                 for entry in result.optimize_result.list[: self.n_cached]
             ]
         )
 
         # scale
         if scaled:
             x_opt = scale_value_dict(x_opt, problem)
@@ -571,22 +571,22 @@
         pars:
             The inner parameters to sample startpoints for.
 
         Returns
         -------
         The sampled startpoints appended to the cached startpoints.
         """
-        if self.minimize_kwargs['n_starts'] == 1 and self.x_guesses is None:
+        if self.minimize_kwargs["n_starts"] == 1 and self.x_guesses is None:
             return np.array(
                 [list(problem.get_dummy_values(scaled=False).values())]
             )
         elif self.x_guesses is not None:
-            n_samples = self.minimize_kwargs['n_starts'] - len(self.x_guesses)
+            n_samples = self.minimize_kwargs["n_starts"] - len(self.x_guesses)
         else:
-            n_samples = self.minimize_kwargs['n_starts'] - 1
+            n_samples = self.minimize_kwargs["n_starts"] - 1
 
         if n_samples <= 0:
             return self.x_guesses
 
         lb = np.nan_to_num([x.lb for x in pars], neginf=self.dummy_lb)
         ub = np.nan_to_num([x.ub for x in pars], posinf=self.dummy_ub)
```

### Comparing `pypesto-0.4.2/pypesto/hierarchical/relative/util.py` & `pypesto-0.5.0/pypesto/hierarchical/relative/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     Returns
     -------
     `num / den` if it's finite, else a dummy value.
     """
     try:
         with warnings.catch_warnings():
-            warnings.filterwarnings('error')
+            warnings.filterwarnings("error")
             quotient = float(numerator / denominator)
         if not np.isfinite(quotient):
             raise ValueError
         return quotient
     except Exception:
         return DUMMY_INNER_VALUE[inner_parameter_type]
 
@@ -473,17 +473,14 @@
     Compute gradient of negative log-likelihood function with respect to
     outer optimization parameters for a condition, given the model outputs,
     relevant data and sigmas.
     """
     return np.nansum(
         np.multiply(
             ssigma,
-            (
-                (np.full(data.shape, 1) - (data - sim) ** 2 / sigma**2)
-                / sigma
-            ),
+            ((np.full(data.shape, 1) - (data - sim) ** 2 / sigma**2) / sigma),
         ),
         axis=(1, 2),
     ) + np.nansum(
         np.multiply(ssim, (sim - data) / sigma**2),
         axis=(1, 2),
     )
```

### Comparing `pypesto-0.4.2/pypesto/hierarchical/semiquantitative/__init__.py` & `pypesto-0.5.0/pypesto/hierarchical/semiquantitative/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.2/pypesto/hierarchical/semiquantitative/calculator.py` & `pypesto-0.5.0/pypesto/hierarchical/semiquantitative/calculator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import copy
-from typing import Sequence
+from collections.abc import Sequence
 
 import numpy as np
 
 from ...C import (
     AMICI_SIGMAY,
     AMICI_SSIGMAY,
     AMICI_SY,
@@ -11,16 +11,16 @@
     FVAL,
     GRAD,
     HESS,
     INNER_PARAMETERS,
     MODE_RES,
     RDATAS,
     RES,
+    SPLINE_KNOTS,
     SRES,
-    X_INNER_OPT,
 )
 from ...objective.amici.amici_calculator import (
     AmiciCalculator,
     AmiciModel,
     AmiciSolver,
 )
 from ...objective.amici.amici_util import (
@@ -74,20 +74,20 @@
     def __call__(
         self,
         x_dct: dict,
         sensi_orders: tuple[int, ...],
         mode: str,
         amici_model: AmiciModel,
         amici_solver: AmiciSolver,
-        edatas: list['amici.ExpData'],
+        edatas: list["amici.ExpData"],
         n_threads: int,
         x_ids: Sequence[str],
         parameter_mapping: ParameterMapping,
         fim_for_hess: bool,
-        rdatas: list['amici.ReturnData'] = None,
+        rdatas: list["amici.ReturnData"] = None,
     ):
         """Perform the actual AMICI call.
 
         Parameters
         ----------
         x_dct:
             Parameters for which to compute function value and derivatives.
@@ -115,15 +115,16 @@
             the :class:`pypesto.objective.amici.InnerCalculatorCollector`,
             it will already simulate the model and pass the results here.
 
 
         Returns
         -------
         inner_result:
-            A dict containing the calculation results: FVAL, GRAD, RDATAS and X_INNER_OPT.
+            A dict containing the calculation results: FVAL, GRAD, RDATAS,
+            INNER_PARAMETERS, and SPLINE_KNOTS.
         """
         if mode == MODE_RES:
             raise ValueError(
                 "Spline approximation cannot be called with residual mode."
             )
         if 2 in sensi_orders:
             raise ValueError(
@@ -171,15 +172,14 @@
         inner_result = {
             FVAL: nllh,
             GRAD: snllh,
             HESS: s2nllh,
             RES: res,
             SRES: sres,
             RDATAS: rdatas,
-            X_INNER_OPT: self.inner_problem.get_inner_parameter_dictionary(),
         }
 
         # if any amici simulation failed, it's unlikely we can compute
         # meaningful inner parameters, so we better just fail early.
         if any(rdata.status != amici.AMICI_SUCCESS for rdata in rdatas):
             inner_result[FVAL] = np.inf
             if 1 in sensi_orders:
@@ -194,17 +194,15 @@
             sim[i] = sim[i].clip(min=0)
 
         # compute optimal inner parameters
         x_inner_opt = self.inner_solver.solve(self.inner_problem, sim, sigma)
         inner_result[FVAL] = self.inner_solver.calculate_obj_function(
             x_inner_opt
         )
-        inner_result[
-            X_INNER_OPT
-        ] = self.inner_problem.get_inner_parameter_dictionary()
+        inner_result[SPLINE_KNOTS] = self.inner_problem.get_spline_knots()
 
         inner_result[
             INNER_PARAMETERS
         ] = self.inner_problem.get_inner_noise_parameters()
 
         # Calculate analytical gradients if requested
         if sensi_order > 0:
```

### Comparing `pypesto-0.4.2/pypesto/hierarchical/semiquantitative/parameter.py` & `pypesto-0.5.0/pypesto/hierarchical/semiquantitative/parameter.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.2/pypesto/hierarchical/semiquantitative/problem.py` & `pypesto-0.5.0/pypesto/hierarchical/semiquantitative/problem.py`

 * *Files 10% similar despite different names*

```diff
@@ -120,18 +120,18 @@
                 self.groups[group][NUM_DATAPOINTS]
             )
             self.groups[group][INNER_NOISE_PARS] = 1
 
     @staticmethod
     def from_petab_amici(
         petab_problem: petab.Problem,
-        amici_model: 'amici.Model',
-        edatas: list['amici.ExpData'],
+        amici_model: "amici.Model",
+        edatas: list["amici.ExpData"],
         spline_ratio: float = None,
-    ) -> 'SemiquantProblem':
+    ) -> "SemiquantProblem":
         """Construct the inner problem from the `petab_problem`."""
         if spline_ratio is None:
             spline_ratio = get_default_options()
         return spline_inner_problem_from_petab_problem(
             petab_problem, amici_model, edatas, spline_ratio
         )
 
@@ -201,14 +201,58 @@
     def get_inner_parameter_dictionary(self) -> dict:
         """Get a dictionary with all inner parameter ids and their values."""
         inner_par_dict = {}
         for x_id, x in self.xs.items():
             inner_par_dict[x_id] = x.value
         return inner_par_dict
 
+    def get_spline_knots(
+        self,
+    ) -> list[list[np.ndarray[float], np.ndarray[float]]]:
+        """Get spline knots of all semiquantitative observables.
+
+        Returns
+        -------
+        list[list[np.ndarray[float], np.ndarray[float]]]
+            A list of lists with two arrays. Each list in the first level corresponds
+            to a semiquantitative observable. Each of these lists contains two arrays:
+            the first array contains the spline bases, the second array contains the
+            spline knot values. The ordering of the observable lists is the same
+            as in `pypesto.problem.hierarchical.semiquant_observable_ids`.
+        """
+        # We need the solver only for the rescaling function.
+        from .solver import SemiquantInnerSolver
+
+        all_spline_knots = []
+
+        for group in self.get_groups_for_xs(InnerParameterType.SPLINE):
+            group_dict = self.groups[group]
+            n_spline_pars = group_dict[N_SPLINE_PARS]
+            n_data_points = group_dict[NUM_DATAPOINTS]
+
+            inner_pars = np.array(
+                [x.value for x in self.get_xs_for_group(group)]
+            )
+
+            # Utility matrix for the spline knot calculation
+            lower_trian = np.tril(np.ones((n_spline_pars, n_spline_pars)))
+            knot_values = np.dot(lower_trian, inner_pars)
+
+            _, knot_bases, _ = SemiquantInnerSolver._rescale_spline_bases(
+                sim_all=group_dict[CURRENT_SIMULATION],
+                N=n_spline_pars,
+                K=n_data_points,
+            )
+
+            spline_knots_for_observable = [knot_bases, knot_values]
+
+            all_spline_knots.append(spline_knots_for_observable)
+
+        return all_spline_knots
+
     def get_measurements_for_group(self, gr) -> np.ndarray:
         """Get measurements for a group."""
         # Taking the ixs of first inner parameter since
         # all of them are the same for the same group.
         ixs = self.get_xs_for_group(gr)[0].ixs
 
         return np.concatenate(
@@ -231,16 +275,16 @@
     """Return the default spline problem options dictionary."""
     spline_ratio = 1 / 2
     return spline_ratio
 
 
 def spline_inner_problem_from_petab_problem(
     petab_problem: petab.Problem,
-    amici_model: 'amici.Model',
-    edatas: list['amici.ExpData'],
+    amici_model: "amici.Model",
+    edatas: list["amici.ExpData"],
     spline_ratio: float = None,
 ):
     """Construct the inner problem from the `petab_problem`."""
     if spline_ratio is None:
         spline_ratio = get_default_options()
     elif spline_ratio <= 0:
         raise ValueError("Spline ratio must be a positive float.")
@@ -258,15 +302,15 @@
 
     # used indices for all measurement specific parameters
     ixs = spline_ixs_for_measurement_specific_parameters(
         petab_problem, amici_model, inner_parameters
     )
 
     # transform experimental data
-    data = [amici.numpy.ExpDataView(edata)['observedData'] for edata in edatas]
+    data = [amici.numpy.ExpDataView(edata)["observedData"] for edata in edatas]
 
     # matrixify
     ix_matrices = ix_matrices_from_arrays(ixs, data)
 
     # assign matrices
     for par in inner_parameters:
         par.ixs = ix_matrices[par.inner_parameter_id]
@@ -278,15 +322,15 @@
         spline_ratio=spline_ratio,
     )
 
 
 def spline_inner_parameters_from_measurement_df(
     df: pd.DataFrame,
     spline_ratio: float,
-    amici_model: 'amici.Model',
+    amici_model: "amici.Model",
 ) -> list[SplineInnerParameter]:
     """Create list of inner free spline parameters from PEtab measurement table."""
     df = df.reset_index()
 
     observable_ids = amici_model.getObservableIds()
 
     par_type = SPLINE_PAR_TYPE
@@ -303,15 +347,15 @@
         group = observable_ids.index(observable_id) + 1
         df_for_group = df[df[OBSERVABLE_ID] == observable_id]
 
         n_spline_parameters = int(np.ceil(len(df_for_group) * spline_ratio))
 
         # Create n_spline_parameters number of spline inner parameters.
         for par_index in range(n_spline_parameters):
-            par_id = f'{par_type}_{observable_id}_{group}_{par_index+1}'
+            par_id = f"{par_type}_{observable_id}_{group}_{par_index+1}"
             inner_parameters.append(
                 SplineInnerParameter(
                     inner_parameter_id=par_id,
                     inner_parameter_type=InnerParameterType.SPLINE,
                     scale=LIN,
                     lb=lb,
                     ub=ub,
@@ -324,16 +368,16 @@
 
     inner_parameters.sort(key=lambda x: (x.group, x.index))
 
     return inner_parameters
 
 
 def noise_inner_parameters_from_parameter_df(
-    petab_problem: 'petab.Problem',
-    amici_model: 'amici.Model',
+    petab_problem: "petab.Problem",
+    amici_model: "amici.Model",
 ) -> list[SplineInnerParameter]:
     """Create list of inner free noise parameters from PEtab parameter table."""
     # Select the semiquantitative measurements.
     measurement_df = petab_problem.measurement_df
     measurement_df = measurement_df[
         measurement_df[MEASUREMENT_TYPE] == SEMIQUANTITATIVE
     ]
@@ -374,16 +418,16 @@
             )
         )
 
     return noise_parameters
 
 
 def spline_ixs_for_measurement_specific_parameters(
-    petab_problem: 'petab.Problem',
-    amici_model: 'amici.Model',
+    petab_problem: "petab.Problem",
+    amici_model: "amici.Model",
     inner_parameters: list[SplineInnerParameter],
 ) -> dict[str, list[tuple[int, int, int]]]:
     """Create mapping of parameters to measurements.
 
     Returns
     -------
     A dictionary mapping parameter ID to a list of
```

### Comparing `pypesto-0.4.2/pypesto/hierarchical/semiquantitative/solver.py` & `pypesto-0.5.0/pypesto/hierarchical/semiquantitative/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,23 +48,23 @@
             **self.get_default_options(),
             **(options or {}),
         }
         self.validate_options()
 
     def validate_options(self):
         """Validate the current options dictionary."""
-        if type(self.options[MIN_DIFF_FACTOR]) is not float:
+        if not isinstance(self.options[MIN_DIFF_FACTOR], float):
             raise TypeError(f"{MIN_DIFF_FACTOR} must be of type float.")
         elif self.options[MIN_DIFF_FACTOR] < 0:
             raise ValueError(f"{MIN_DIFF_FACTOR} must not be negative.")
 
-        elif type(self.options[REGULARIZE_SPLINE]) is not bool:
+        elif not isinstance(self.options[REGULARIZE_SPLINE], bool):
             raise TypeError(f"{REGULARIZE_SPLINE} must be of type bool.")
         if self.options[REGULARIZE_SPLINE]:
-            if type(self.options[REGULARIZATION_FACTOR]) is not float:
+            if not isinstance(self.options[REGULARIZATION_FACTOR], float):
                 raise TypeError(
                     f"{REGULARIZATION_FACTOR} must be of type float."
                 )
             elif self.options[REGULARIZATION_FACTOR] < 0:
                 raise ValueError(
                     f"{REGULARIZATION_FACTOR} must not be negative."
                 )
@@ -138,15 +138,18 @@
         -------
         Inner objective function value.
         """
         if False in (
             x_inner_opt[idx][SCIPY_SUCCESS] for idx in range(len(x_inner_opt))
         ):
             obj = np.inf
-            warnings.warn("Inner optimization failed.")
+            warnings.warn(
+                "Inner optimization failed.",
+                stacklevel=2,
+            )
         else:
             obj = np.sum(
                 [
                     x_inner_opt[idx][SCIPY_FUN]
                     for idx in range(len(x_inner_opt))
                 ]
             )
@@ -327,16 +330,15 @@
                             measurements=measurements,
                             N=N,
                             delta_c=delta_c,
                             c=c,
                             n=n,
                         )
                         dJ_dsigma2 = (
-                            K / (2 * sigma**2)
-                            - residual_squared / sigma**4
+                            K / (2 * sigma**2) - residual_squared / sigma**4
                         )
                         dsigma2_dtheta = ssigma_all[0] * sigma
                         dsigma_grad_term = dJ_dsigma2 * dsigma2_dtheta
                     # If we optimize the noise hierarchically,
                     # the last term (dJ_dsigma^2 * dsigma^2_dtheta) is always 0
                     # since the sigma is optimized such that dJ_dsigma2=0.
                     else:
@@ -434,15 +436,16 @@
             objective_function_wrapper,
             jac=inner_gradient_wrapper,
             **inner_options,
         )
 
         return results
 
-    def _rescale_spline_bases(self, sim_all: np.ndarray, N: int, K: int):
+    @staticmethod
+    def _rescale_spline_bases(sim_all: np.ndarray, N: int, K: int):
         """Rescale the spline bases.
 
         Before the optimization of the spline parameters, we have to fix the
         spline bases to some values. We choose to scale them to the current
         simulation. In case of simulations that are very close to each other,
         we choose to scale closely around the average value of the simulations,
         to avoid numerical problems (as we often divide by delta_c).
@@ -488,15 +491,17 @@
                 )
             # Set the n(k) values for the simulations
             for i in range(len(sim_all)):
                 n[i] = np.ceil((sim_all[i] - c[0]) / delta_c) + 1
                 if n[i] > N:
                     n[i] = N
                     warnings.warn(
-                        "Interval for a simulation has been set to a larger value than the number of spline parameters."
+                        "Interval for a simulation has been set to a larger "
+                        "value than the number of spline parameters.",
+                        stacklevel=2,
                     )
         # In case the simulations are sufficiently apart:
         else:
             delta_c = (max_all - min_all) / (N - 1)
             c = np.linspace(min_all, max_all, N)
             for i in range(len(sim_all)):
                 if i == max_idx:
@@ -571,15 +576,15 @@
             x0[0] = np.max([min_meas - 0.3 * range_all, 0])
 
         from scipy.optimize import Bounds
 
         inner_options = {
             "x0": x0,
             "method": "L-BFGS-B",
-            "options": {"ftol": 1e-16, "disp": None},
+            "options": {"disp": None},
             "bounds": Bounds(lb=constraint_min_diff),
         }
 
         return inner_options
 
 
 def _calculate_nllh_for_group(
@@ -753,16 +758,15 @@
             )
         )
     else:
         regularization_term_gradient = np.zeros_like(s)
 
     # Combine all terms into the gradient of the negative log-likelihood
     nllh_gradient = (
-        residuals_squared_gradient / (sigma**2)
-        + regularization_term_gradient
+        residuals_squared_gradient / (sigma**2) + regularization_term_gradient
     )
     return nllh_gradient
 
 
 def _calculate_sigma_for_group(
     residuals_squared: float,
     n_datapoints: int,
@@ -1082,19 +1086,16 @@
     """
     group_dict = inner_problem.groups[group]
     inner_spline_parameters = inner_problem.get_xs_for_group(group)
     inner_noise_parameters = inner_problem.get_noise_parameters_for_group(
         group
     )
 
-    lower_trian = np.tril(np.ones((len(s), len(s))))
-    xi = np.dot(lower_trian, s)
-
     for idx in range(len(inner_spline_parameters)):
-        inner_spline_parameters[idx].value = xi[idx]
+        inner_spline_parameters[idx].value = s[idx]
 
     sigma = group_dict[INNER_NOISE_PARS]
 
     if group_dict[OPTIMIZE_NOISE]:
         inner_noise_parameters[0].value = sigma
```

### Comparing `pypesto-0.4.2/pypesto/history/__init__.py` & `pypesto-0.5.0/pypesto/history/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.2/pypesto/history/amici.py` & `pypesto-0.5.0/pypesto/history/amici.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from collections.abc import Sequence
 from pathlib import Path
-from typing import Sequence, Union
+from typing import Union
 
 import numpy as np
 
 from ..C import (
     CPU_TIME_TOTAL,
     POSTEQ_CPU_TIME,
     POSTEQ_CPU_TIME_BACKWARD,
```

### Comparing `pypesto-0.4.2/pypesto/history/base.py` & `pypesto-0.5.0/pypesto/history/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Base history class."""
 
 import numbers
 import time
 from abc import ABC, abstractmethod
-from typing import Sequence, Union
+from collections.abc import Sequence
+from typing import Union
 
 import numpy as np
 
 from ..C import (
     FVAL,
     GRAD,
     HESS,
@@ -531,12 +532,12 @@
     Result reduced to what is intended to be stored in history.
     """
     result = result.copy()
 
     # apply options to result
     for key in HistoryBase.RESULT_KEYS:
         if result.get(key) is None or not options.get(
-            f'trace_record_{key}', True
+            f"trace_record_{key}", True
         ):
             result[key] = np.nan
 
     return result
```

### Comparing `pypesto-0.4.2/pypesto/history/csv.py` & `pypesto-0.5.0/pypesto/history/csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """CSV history."""
 
 import copy
 import os
 import time
-from typing import Sequence, Union
+from collections.abc import Sequence
+from typing import Union
 
 import numpy as np
 import pandas as pd
 
 from ..C import (
     FVAL,
     GRAD,
@@ -16,15 +17,14 @@
     N_GRAD,
     N_HESS,
     N_RES,
     N_SRES,
     RES,
     SRES,
     TIME,
-    X_INNER_OPT,
     ModeType,
     X,
 )
 from .base import CountHistoryBase, add_fun_from_res, reduce_result_via_options
 from .options import HistoryOptions
 from .util import MaybeArray, ResultDict, trace_wrap
 
@@ -61,15 +61,15 @@
             dirname = os.path.dirname(self.file)
             os.makedirs(dirname, exist_ok=True)
 
         if load_from_file and os.path.exists(self.file):
             trace = pd.read_csv(self.file, header=[0, 1], index_col=0)
             # replace 'nan' in cols with np.NAN
             cols = pd.DataFrame(trace.columns.to_list())
-            cols[cols == 'nan'] = np.NaN
+            cols[cols == "nan"] = np.NaN
             trace.columns = pd.MultiIndex.from_tuples(
                 cols.to_records(index=False).tolist()
             )
             for col in trace.columns:
                 # transform strings to np.ndarrays
                 trace[col] = trace[col].apply(string2ndarray)
 
@@ -134,35 +134,31 @@
             add_fun_from_res(result), self.options
         )
 
         used_time = time.time() - self._start_time
 
         # create table row
         row = pd.Series(
-            name=len(self._trace), index=self._trace.columns, dtype='object'
+            name=len(self._trace), index=self._trace.columns, dtype="object"
         )
 
         values = self._simulation_to_values(result, used_time)
 
         for var, val in values.items():
             row[(var, np.nan)] = val
 
         for var, val in {
             X: x,
             GRAD: result[GRAD],
         }.items():
-            if var == X or self.options[f'trace_record_{var}']:
+            if var == X or self.options[f"trace_record_{var}"]:
                 row[var] = val
             else:
                 row[(var, np.nan)] = np.nan
 
-        if X_INNER_OPT in result:
-            for x_inner_id, x_inner_opt_value in result[X_INNER_OPT].items():
-                row[(X_INNER_OPT, x_inner_id)] = x_inner_opt_value
-
         self._trace = pd.concat(
             (self._trace, pd.DataFrame([row])),
         )
 
         # save trace to file
         self._save_trace()
 
@@ -182,39 +178,39 @@
                 HESS,
             ]
         ]
 
     def _init_trace(self, x: np.ndarray):
         """Initialize the trace."""
         if self.x_names is None:
-            self.x_names = [f'x{i}' for i, _ in enumerate(x)]
+            self.x_names = [f"x{i}" for i, _ in enumerate(x)]
 
         columns = self._trace_columns()
 
         for var in [X, GRAD]:
-            if var == X or self.options[f'trace_record_{var}']:
+            if var == X or self.options[f"trace_record_{var}"]:
                 columns.extend([(var, x_name) for x_name in self.x_names])
             else:
                 columns.extend([(var,)])
 
         # TODO: multi-index for res, sres, hess
         self._trace = pd.DataFrame(
-            columns=pd.MultiIndex.from_tuples(columns), dtype='float64'
+            columns=pd.MultiIndex.from_tuples(columns), dtype="float64"
         )
 
         # only non-float64
         trace_dtypes = {
-            RES: 'object',
-            SRES: 'object',
-            HESS: 'object',
-            N_FVAL: 'int64',
-            N_GRAD: 'int64',
-            N_HESS: 'int64',
-            N_RES: 'int64',
-            N_SRES: 'int64',
+            RES: "object",
+            SRES: "object",
+            HESS: "object",
+            N_FVAL: "int64",
+            N_GRAD: "int64",
+            N_HESS: "int64",
+            N_RES: "int64",
+            N_SRES: "int64",
         }
 
         for var, dtype in trace_dtypes.items():
             self._trace[(var, np.nan)] = self._trace[(var, np.nan)].astype(
                 dtype
             )
 
@@ -327,13 +323,13 @@
 
     Returns
     -------
     Array as :class:`numpy.ndarray`.
     """
     if not isinstance(x, str):
         return x
-    if x.startswith('[['):
+    if x.startswith("[["):
         return np.vstack(
-            [np.fromstring(xx, sep=' ') for xx in x[2:-2].split(']\n [')]
+            [np.fromstring(xx, sep=" ") for xx in x[2:-2].split("]\n [")]
         )
     else:
-        return np.fromstring(x[1:-1], sep=' ')
+        return np.fromstring(x[1:-1], sep=" ")
```

### Comparing `pypesto-0.4.2/pypesto/history/generate.py` & `pypesto-0.5.0/pypesto/history/generate.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Generate a history from options and inputs."""
 
+from collections.abc import Sequence
 from pathlib import Path
-from typing import Sequence
 
 from ..C import SUFFIXES_CSV, SUFFIXES_HDF5
 from .base import CountHistory, HistoryBase
 from .csv import CsvHistory
 from .hdf5 import Hdf5History
 from .memory import MemoryHistory
 from .options import HistoryOptions
```

### Comparing `pypesto-0.4.2/pypesto/history/hdf5.py` & `pypesto-0.5.0/pypesto/history/hdf5.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """HDF5 history."""
 
 import contextlib
 import time
+from collections.abc import Sequence
 from functools import wraps
 from pathlib import Path
-from typing import Sequence, Union
+from typing import Union
 
 import h5py
 import numpy as np
 
 from ..C import (
     EXITFLAG,
     FVAL,
@@ -138,26 +139,26 @@
     @with_h5_file("a")
     @check_editable
     def finalize(self, message: str = None, exitflag: str = None) -> None:
         """See :class:`HistoryBase.finalize`."""
         super().finalize()
 
         # add message and exitflag to trace
-        grp = self._f.require_group(f'{HISTORY}/{self.id}/{MESSAGES}/')
+        grp = self._f.require_group(f"{HISTORY}/{self.id}/{MESSAGES}/")
         if message is not None:
             grp.attrs[MESSAGE] = message
         if exitflag is not None:
             grp.attrs[EXITFLAG] = exitflag
 
     @staticmethod
     def load(
         id: str,
         file: Union[str, Path],
         options: Union[HistoryOptions, dict] = None,
-    ) -> 'Hdf5History':
+    ) -> "Hdf5History":
         """Load the History object from memory."""
         history = Hdf5History(id=id, file=file, options=options)
         if options is None:
             history.recover_options(file)
         return history
 
     def recover_options(self, file: Union[str, Path]):
@@ -284,24 +285,24 @@
             return np.nan
 
     @property
     @with_h5_file("r")
     def message(self) -> str:
         """Optimizer message in case of finished optimization."""
         try:
-            return self._f[f'{HISTORY}/{self.id}/{MESSAGES}/'].attrs[MESSAGE]
+            return self._f[f"{HISTORY}/{self.id}/{MESSAGES}/"].attrs[MESSAGE]
         except KeyError:
             return None
 
     @property
     @with_h5_file("r")
     def exitflag(self) -> str:
         """Optimizer exitflag in case of finished optimization."""
         try:
-            return self._f[f'{HISTORY}/{self.id}/{MESSAGES}/'].attrs[EXITFLAG]
+            return self._f[f"{HISTORY}/{self.id}/{MESSAGES}/"].attrs[EXITFLAG]
         except KeyError:
             return None
 
     @staticmethod
     def _simulation_to_values(x, result, used_time):
         values = {
             X: x,
@@ -336,30 +337,30 @@
 
         values = self._simulation_to_values(x, result, used_time)
 
         iteration = self._require_group().attrs[N_ITERATIONS]
 
         for key in values.keys():
             if values[key] is not None:
-                self._require_group()[f'{iteration}/{key}'] = values[key]
+                self._require_group()[f"{iteration}/{key}"] = values[key]
 
         self._require_group().attrs[N_ITERATIONS] += 1
 
     @with_h5_file("r")
     def _get_group(self) -> h5py.Group:
         """Get the HDF5 group for the current history."""
-        return self._f[f'{HISTORY}/{self.id}/{TRACE}/']
+        return self._f[f"{HISTORY}/{self.id}/{TRACE}/"]
 
     @with_h5_file("a")
     def _require_group(self) -> h5py.Group:
         """Get, or if necessary create, the group in the hdf5 file."""
         with contextlib.suppress(KeyError):
-            return self._f[f'{HISTORY}/{self.id}/{TRACE}/']
+            return self._f[f"{HISTORY}/{self.id}/{TRACE}/"]
 
-        grp = self._f.create_group(f'{HISTORY}/{self.id}/{TRACE}/')
+        grp = self._f.create_group(f"{HISTORY}/{self.id}/{TRACE}/")
         grp.attrs[N_ITERATIONS] = 0
         grp.attrs[N_FVAL] = 0
         grp.attrs[N_GRAD] = 0
         grp.attrs[N_HESS] = 0
         grp.attrs[N_RES] = 0
         grp.attrs[N_SRES] = 0
         grp.attrs[START_TIME] = time.time()
@@ -392,15 +393,15 @@
         if ix is None:
             ix = range(len(self))
         trace_result = []
 
         for iteration in ix:
             try:
                 dataset = self._f[
-                    f'{HISTORY}/{self.id}/{TRACE}/{iteration}/{entry_id}'
+                    f"{HISTORY}/{self.id}/{TRACE}/{iteration}/{entry_id}"
                 ]
                 if dataset.shape == ():
                     entry = dataset[()]  # scalar
                 else:
                     entry = np.array(dataset)
                 trace_result.append(entry)
             except KeyError:
```

### Comparing `pypesto-0.4.2/pypesto/history/memory.py` & `pypesto-0.5.0/pypesto/history/memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """In-memory history."""
 
 import time
-from typing import Any, Sequence, Union
+from collections.abc import Sequence
+from typing import Any, Union
 
 import numpy as np
 
 from ..C import FVAL, GRAD, HESS, RES, SRES, TIME, ModeType, X
 from .base import (
     CountHistoryBase,
     HistoryBase,
```

### Comparing `pypesto-0.4.2/pypesto/history/optimizer.py` & `pypesto-0.5.0/pypesto/history/optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,28 +152,28 @@
             # issue a warning, as if this happens, then something may be wrong
             logger.warning(
                 f"History has a better point {fval} than the current best "
                 f"point {self.fval_min}."
             )
             # update everything
             for key in self.MIN_KEYS:
-                setattr(self, key + '_min', result[key])
+                setattr(self, key + "_min", result[key])
 
         # check if history has same point
         if (
             isclose(fval, self.fval_min)
             and self.x_min is not None
             and allclose(result[X], self.x_min)
         ):
             # update only missing entries
             #  (e.g. grad and hess may be recorded but not in history)
             for key in self.MIN_KEYS:
                 if result[key] is not None:
                     # if getattr(self, f'{key}_min') is None:
-                    setattr(self, f'{key}_min', result[key])
+                    setattr(self, f"{key}_min", result[key])
 
     def _update_vals(self, x: np.ndarray, result: ResultDict) -> None:
         """Update initial and best function values."""
         # update initial point
         if is_none_or_nan(self.fval0) and np.array_equal(x, self.x0):
             self.fval0 = result.get(FVAL)
 
@@ -184,27 +184,27 @@
         # update if fval is better
         if (
             not is_none_or_nan(fval := result.get(FVAL))
             and fval < self.fval_min
         ):
             # need to update all values, as better fval found
             for key in HistoryBase.RESULT_KEYS:
-                setattr(self, f'{key}_min', result.get(key))
+                setattr(self, f"{key}_min", result.get(key))
             self.x_min = x
             return
 
         # Sometimes sensitivities are evaluated on subsequent calls. We can
         # identify this situation by checking that x hasn't changed.
         if self.x_min is not None and np.array_equal(self.x_min, x):
             for key in (GRAD, HESS, SRES):
-                val_min = getattr(self, f'{key}_min', None)
+                val_min = getattr(self, f"{key}_min", None)
                 if is_none_or_nan_array(val_min) and not is_none_or_nan_array(
                     val := result.get(key)
                 ):
-                    setattr(self, f'{key}_min', val)
+                    setattr(self, f"{key}_min", val)
 
     def _maybe_compute_init_and_min_vals_from_trace(self) -> None:
         """Try to set initial and best function value from trace.
 
         .. note:: Only possible if history has a trace.
         """
         if not len(self.history):
@@ -221,15 +221,15 @@
                 break
 
         # find best fval
         result = self._get_optimal_point_from_history()
 
         # assign values
         for key in OptimizerHistory.MIN_KEYS:
-            setattr(self, f'{key}_min', result[key])
+            setattr(self, f"{key}_min", result[key])
 
     def _admissible(self, x: np.ndarray) -> bool:
         """Check whether point `x` is admissible (i.e. within bounds).
 
         Parameters
         ----------
         x: A single parameter vector.
@@ -260,30 +260,30 @@
         if isinstance(ix_min, np.ndarray):
             ix_min = ix_min[0]
         # select index in original array
         ix_min = ixs_admit[ix_min]
 
         # fill in parameter and function value from that index
         for var in (X, FVAL, RES):
-            val = getattr(self.history, f'get_{var}_trace')(ix_min)
+            val = getattr(self.history, f"get_{var}_trace")(ix_min)
             if val is not None and not np.all(np.isnan(val)):
                 result[var] = val
             # convert to float if var is FVAL to be sure
             if var == FVAL:
                 result[var] = float(result[var])
 
         # derivatives may be evaluated at different indices, therefore
         #  iterate over all and check whether any has the same parameter
         #  and the desired field filled
         for var in (GRAD, HESS, SRES):
             for ix in range(len(self.history)):
                 if not allclose(result[X], self.history.get_x_trace(ix)):
                     # different parameter
                     continue
-                val = getattr(self.history, f'get_{var}_trace')(ix)
+                val = getattr(self.history, f"get_{var}_trace")(ix)
                 if not is_none_or_nan_array(val):
                     result[var] = val
                     # successfuly found
                     break
 
         # fill remaining keys with None
         for key in OptimizerHistory.MIN_KEYS:
```

### Comparing `pypesto-0.4.2/pypesto/history/options.py` & `pypesto-0.5.0/pypesto/history/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         self._sanity_check()
 
     def __getattr__(self, key):
         """Allow to use keys as attributes."""
         try:
             return self[key]
         except KeyError:
-            raise AttributeError(key)
+            raise AttributeError(key) from None
 
     __setattr__ = dict.__setitem__
     __delattr__ = dict.__delitem__
 
     def _sanity_check(self):
         """Apply basic sanity checks."""
         if self.storage_file is None:
@@ -87,16 +87,16 @@
 
         # check csv histories are parametrized
         if suffix in SUFFIXES_CSV and "{id}" not in self.storage_file:
             raise CsvHistoryTemplateError(self.storage_file)
 
     @staticmethod
     def assert_instance(
-        maybe_options: Union['HistoryOptions', dict],
-    ) -> 'HistoryOptions':
+        maybe_options: Union["HistoryOptions", dict],
+    ) -> "HistoryOptions":
         """
         Return a valid options object.
 
         Parameters
         ----------
         maybe_options: :class:`HistoryOptions` or dict
         """
```

### Comparing `pypesto-0.4.2/pypesto/history/util.py` & `pypesto-0.5.0/pypesto/history/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """History utility functions."""
 
 import numbers
+from collections.abc import Sequence
 from functools import wraps
-from typing import Sequence, Union
+from typing import Union
 
 import numpy as np
 
 from ..C import SUFFIXES
 
 ResultDict = dict[str, Union[float, np.ndarray]]
-MaybeArray = Union[np.ndarray, 'np.nan']
+MaybeArray = Union[np.ndarray, "np.nan"]
 
 
 class HistoryTypeError(ValueError):
     """Error raised when an unsupported history type is requested."""
 
     def __init__(self, history_type: str):
         super().__init__(
```

### Comparing `pypesto-0.4.2/pypesto/logging.py` & `pypesto-0.5.0/pypesto/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 Logging convenience functions.
 """
 
 import logging
 
 
 def log(
-    name: str = 'pypesto',
+    name: str = "pypesto",
     level: int = logging.INFO,
     console: bool = True,
-    filename: str = '',
+    filename: str = "",
 ):
     """
     Log messages from `name` with `level` to any combination of console/file.
 
     Parameters
     ----------
     name:
@@ -50,15 +50,15 @@
     ----------
     See the `log` method.
     """
     log(level=level, console=True)
 
 
 def log_to_file(
-    level: int = logging.INFO, filename: str = '.pypesto_logging.log'
+    level: int = logging.INFO, filename: str = ".pypesto_logging.log"
 ):
     """
     Log to file.
 
     Parameters
     ----------
     See the `log` method.
```

### Comparing `pypesto-0.4.2/pypesto/objective/aesara/base.py` & `pypesto-0.5.0/pypesto/objective/aesara/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 Adds an interface for the construction of loss functions
 incorporating aesara models. This permits computation of derivatives using a
 combination of objective based methods and aesara based backpropagation.
 """
 
 import copy
-from typing import Optional, Sequence, Tuple
+from collections.abc import Sequence
+from typing import Optional
 
 import numpy as np
 
 from ...C import FVAL, GRAD, HESS, MODE_FUN, RDATAS, ModeType
 from ..base import ObjectiveBase, ResultDict
 
 try:
@@ -20,15 +21,15 @@
     from aesara.tensor import Op
     from aesara.tensor.var import TensorVariable
 except ImportError:
     raise ImportError(
         "Using an aeasara objective requires an installation of "
         "the python package aesara. Please install aesara via "
         "`pip install aesara`."
-    )
+    ) from None
 
 
 class AesaraObjective(ObjectiveBase):
     """
     Wrapper around an ObjectiveBase.
 
     Computes the gradient at each evaluation, caching it for later calls.
@@ -53,18 +54,18 @@
         objective: ObjectiveBase,
         aet_x: TensorVariable,
         aet_fun: TensorVariable,
         coeff: Optional[float] = 1.0,
         x_names: Sequence[str] = None,
     ):
         if not isinstance(objective, ObjectiveBase):
-            raise TypeError('objective must be an ObjectiveBase instance')
+            raise TypeError("objective must be an ObjectiveBase instance")
         if not objective.check_mode(MODE_FUN):
             raise NotImplementedError(
-                f'objective must support mode={MODE_FUN}'
+                f"objective must support mode={MODE_FUN}"
             )
         super().__init__(x_names)
         self.base_objective = objective
 
         self.aet_x = aet_x
         self.aet_fun = aet_fun
         self._coeff = coeff
@@ -103,15 +104,15 @@
             return False
         else:
             return self.base_objective.check_sensi_orders(sensi_orders, mode)
 
     def call_unprocessed(
         self,
         x: np.ndarray,
-        sensi_orders: Tuple[int, ...],
+        sensi_orders: tuple[int, ...],
         mode: ModeType,
         **kwargs,
     ) -> ResultDict:
         """
         See `ObjectiveBase` for more documentation.
 
         Main method to overwrite from the base class. It handles and
@@ -121,22 +122,22 @@
         if 2 in sensi_orders and 1 not in sensi_orders:
             sensi_orders = (1, *sensi_orders)
 
         # this computes all the results from the inner objective, rendering
         # them accessible to aesara compiled functions
 
         set_return_dict, return_dict = (
-            'return_dict' in kwargs,
-            kwargs.pop('return_dict', False),
+            "return_dict" in kwargs,
+            kwargs.pop("return_dict", False),
         )
         self.cached_base_ret = self.base_objective(
             self.infun(x), sensi_orders, mode, return_dict=True, **kwargs
         )
         if set_return_dict:
-            kwargs['return_dict'] = return_dict
+            kwargs["return_dict"] = return_dict
         ret = {}
         if RDATAS in self.cached_base_ret:
             ret[RDATAS] = self.cached_base_ret[RDATAS]
         if 0 in sensi_orders:
             ret[FVAL] = float(self.afun(x))
         if 1 in sensi_orders:
             ret[GRAD] = self.agrad(x)[0]
@@ -192,15 +193,15 @@
         """
         Calculate the hessian.
 
         Actually returns the vector-hessian product - g[0] is a vector of
         parameter values.
         """
         if self._log_prob_grad is None:
-            return super(AesaraObjectiveOp, self).grad(inputs, g)
+            return super().grad(inputs, g)
         (theta,) = inputs
         log_prob_grad = self._log_prob_grad(theta)
         return [g[0] * log_prob_grad]
 
 
 class AesaraObjectiveGradOp(Op):
     """
@@ -240,15 +241,15 @@
         """
         Calculate the hessian.
 
         Actually returns the vector-hessian product - g[0] is a vector of
         parameter values.
         """
         if self._log_prob_hess is None:
-            return super(AesaraObjectiveGradOp, self).grad(inputs, g)
+            return super().grad(inputs, g)
         (theta,) = inputs
         log_prob_hess = self._log_prob_hess(theta)
         return [g[0].dot(log_prob_hess)]
 
 
 class AesaraObjectiveHessOp(Op):
     """
```

### Comparing `pypesto-0.4.2/pypesto/objective/aggregated.py` & `pypesto-0.5.0/pypesto/objective/aggregated.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from collections.abc import Sequence
 from copy import deepcopy
-from typing import Any, Dict, Sequence, Tuple
+from typing import Any
 
 import numpy as np
 
 from ..C import FVAL, GRAD, HESS, HESSP, RDATAS, RES, SRES, ModeType
 from .base import ObjectiveBase, ResultDict
 
 
@@ -26,66 +27,66 @@
             Sequence of names of the (optimized) parameters.
             (Details see documentation of x_names in
             :class:`pypesto.ObjectiveBase`)
         """
         # input typechecks
         if not isinstance(objectives, Sequence):
             raise TypeError(
-                f'Objectives must be a Sequence, ' f'was {type(objectives)}.'
+                f"Objectives must be a Sequence, " f"was {type(objectives)}."
             )
 
         if not all(
             isinstance(objective, ObjectiveBase) for objective in objectives
         ):
             raise TypeError(
-                'Objectives must only contain elements of type'
-                'pypesto.Objective'
+                "Objectives must only contain elements of type"
+                "pypesto.Objective"
             )
 
         if not objectives:
-            raise ValueError('Length of objectives must be at least one')
+            raise ValueError("Length of objectives must be at least one")
 
         self._objectives = objectives
 
         super().__init__(x_names=x_names)
 
     def __deepcopy__(self, memodict=None):
         """Create copy of objective."""
         other = AggregatedObjective(
             objectives=[deepcopy(objective) for objective in self._objectives],
             x_names=deepcopy(self.x_names),
         )
-        for key in set(self.__dict__.keys()) - {'_objectives', 'x_names'}:
+        for key in set(self.__dict__.keys()) - {"_objectives", "x_names"}:
             other.__dict__[key] = deepcopy(self.__dict__[key])
 
         return other
 
     def check_mode(self, mode: ModeType) -> bool:
         """See `ObjectiveBase` documentation."""
         return all(
             objective.check_mode(mode) for objective in self._objectives
         )
 
     def check_sensi_orders(
         self,
-        sensi_orders: Tuple[int, ...],
+        sensi_orders: tuple[int, ...],
         mode: ModeType,
     ) -> bool:
         """See `ObjectiveBase` documentation."""
         return all(
             objective.check_sensi_orders(sensi_orders, mode)
             for objective in self._objectives
         )
 
     def call_unprocessed(
         self,
         x: np.ndarray,
-        sensi_orders: Tuple[int, ...],
+        sensi_orders: tuple[int, ...],
         mode: ModeType,
-        kwargs_list: Sequence[Dict[str, Any]] = None,
+        kwargs_list: Sequence[dict[str, Any]] = None,
         **kwargs,
     ) -> ResultDict:
         """
         See `ObjectiveBase` for more documentation.
 
         Main method to overwrite from the base class. It handles and
         delegates the actual objective evaluation.
@@ -121,15 +122,15 @@
         for objective in self._objectives:
             objective.initialize()
 
     def get_config(self) -> dict:
         """Return basic information of the objective configuration."""
         info = super().get_config()
         for n_obj, obj in enumerate(self._objectives):
-            info[f'objective_{n_obj}'] = obj.get_config()
+            info[f"objective_{n_obj}"] = obj.get_config()
         return info
 
 
 def aggregate_results(rvals: Sequence[ResultDict]) -> ResultDict:
     """
     Aggregate the results from the provided ResultDicts into a single one.
```

### Comparing `pypesto-0.4.2/pypesto/objective/amici/amici.py` & `pypesto-0.5.0/pypesto/objective/amici/amici.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import abc
 import copy
 import os
 import tempfile
 from collections import OrderedDict
+from collections.abc import Sequence
 from pathlib import Path
-from typing import TYPE_CHECKING, Dict, Optional, Sequence, Tuple, Union
+from typing import TYPE_CHECKING, Optional, Union
 
 import numpy as np
 
 from ...C import (
     FVAL,
-    INNER_PARAMETERS,
     MODE_FUN,
     MODE_RES,
     RDATAS,
     SUFFIXES_CSV,
     SUFFIXES_HDF5,
     ModeType,
 )
@@ -32,20 +32,20 @@
     create_identity_parameter_mapping,
     map_par_opt_to_par_sim,
 )
 
 if TYPE_CHECKING:
     try:
         import amici
-        from amici.parameter_mapping import ParameterMapping
+        from amici.petab.parameter_mapping import ParameterMapping
     except ImportError:
         pass
 
-AmiciModel = Union['amici.Model', 'amici.ModelPtr']
-AmiciSolver = Union['amici.Solver', 'amici.SolverPtr']
+AmiciModel = Union["amici.Model", "amici.ModelPtr"]
+AmiciSolver = Union["amici.Solver", "amici.SolverPtr"]
 
 
 class AmiciObjectBuilder(abc.ABC):
     """Allows to build AMICI model, solver, and edatas.
 
     This class is useful for pickling an :class:`pypesto.AmiciObjective`,
     which is required in some parallelization schemes. Therefore, this
@@ -57,36 +57,36 @@
         """Create an AMICI model."""
 
     @abc.abstractmethod
     def create_solver(self, model: AmiciModel) -> AmiciSolver:
         """Create an AMICI solver."""
 
     @abc.abstractmethod
-    def create_edatas(self, model: AmiciModel) -> Sequence['amici.ExpData']:
+    def create_edatas(self, model: AmiciModel) -> Sequence["amici.ExpData"]:
         """Create AMICI experimental data."""
 
 
 class AmiciObjective(ObjectiveBase):
     """Allows to create an objective directly from an amici model."""
 
     def __init__(
         self,
         amici_model: AmiciModel,
         amici_solver: AmiciSolver,
-        edatas: Union[Sequence['amici.ExpData'], 'amici.ExpData'],
+        edatas: Union[Sequence["amici.ExpData"], "amici.ExpData"],
         max_sensi_order: Optional[int] = None,
         x_ids: Optional[Sequence[str]] = None,
         x_names: Optional[Sequence[str]] = None,
-        parameter_mapping: Optional['ParameterMapping'] = None,
+        parameter_mapping: Optional["ParameterMapping"] = None,
         guess_steadystate: Optional[Optional[bool]] = None,
         n_threads: Optional[int] = 1,
         fim_for_hess: Optional[bool] = True,
         amici_object_builder: Optional[AmiciObjectBuilder] = None,
         calculator: Optional[AmiciCalculator] = None,
-        amici_reporting: Optional['amici.RDataReporting'] = None,
+        amici_reporting: Optional["amici.RDataReporting"] = None,
     ):
         """
         Initialize objective.
 
         Parameters
         ----------
         amici_model:
@@ -102,15 +102,16 @@
         x_ids:
             Ids of optimization parameters. In the simplest case, this will be
             the AMICI model parameters (default).
         x_names:
             Names of optimization parameters.
         parameter_mapping:
             Mapping of optimization parameters to model parameters. Format
-            as created by `amici.petab_objective.create_parameter_mapping`.
+            as created by
+            `amici.petab.parameter_mapping.create_parameter_mapping`.
             The default is just to assume that optimization and simulation
             parameters coincide.
         guess_steadystate:
             Whether to guess steadystates based on previous steadystates and
             respective derivatives. This option may lead to unexpected
             results for models with conservation laws and should accordingly
             be deactivated for those models.
@@ -177,41 +178,41 @@
         #  supported, disable by default. If requested but unsupported, raise.
         if (
             self.guess_steadystate is not False
             and self.amici_model.nx_solver_reinit > 0
         ):
             if self.guess_steadystate:
                 raise ValueError(
-                    'Steadystate prediction is not supported '
-                    'for models with conservation laws!'
+                    "Steadystate prediction is not supported "
+                    "for models with conservation laws!"
                 )
             self.guess_steadystate = False
 
         if (
             self.guess_steadystate is not False
             and self.amici_model.getSteadyStateSensitivityMode()
             == amici.SteadyStateSensitivityMode.integrationOnly
         ):
             if self.guess_steadystate:
                 raise ValueError(
-                    'Steadystate guesses cannot be enabled '
-                    'when `integrationOnly` as '
-                    'SteadyStateSensitivityMode!'
+                    "Steadystate guesses cannot be enabled "
+                    "when `integrationOnly` as "
+                    "SteadyStateSensitivityMode!"
                 )
             self.guess_steadystate = False
 
         if self.guess_steadystate is not False:
             self.guess_steadystate = True
 
         if self.guess_steadystate:
             # preallocate guesses, construct a dict for every edata for which
             #  we need to do preequilibration
             self.steadystate_guesses = {
-                'fval': np.inf,
-                'data': {
+                "fval": np.inf,
+                "data": {
                     iexp: {}
                     for iexp, edata in enumerate(self.edatas)
                     if len(edata.fixedParametersPreequilibration)
                 },
             }
         # optimization parameter names
         if x_names is None:
@@ -228,24 +229,21 @@
         self.calculator = calculator
         super().__init__(x_names=x_names)
 
         # Custom (condition-specific) timepoints. See the
         # `set_custom_timepoints` method for more information.
         self.custom_timepoints = None
 
-        # Initialize the dictionary for saving of inner parameters.
-        self.inner_parameters: list[float] = None
-
     def get_config(self) -> dict:
         """Return basic information of the objective configuration."""
         info = super().get_config()
-        info['x_names'] = self.x_names
-        info['model_name'] = self.amici_model.getName()
-        info['solver'] = str(type(self.amici_solver))
-        info['sensi_order'] = self.max_sensi_order
+        info["x_names"] = self.x_names
+        info["model_name"] = self.amici_model.getName()
+        info["solver"] = str(type(self.amici_solver))
+        info["sensi_order"] = self.max_sensi_order
 
         return info
 
     def create_history(
         self, id: str, x_names: Sequence[str], options: HistoryOptions
     ):
         """See `history.generate.create_history` documentation."""
@@ -274,47 +272,47 @@
 
     def initialize(self):
         """See `ObjectiveBase` documentation."""
         super().initialize()
         self.reset_steadystate_guesses()
         self.calculator.initialize()
 
-    def __deepcopy__(self, memodict: Dict = None) -> 'AmiciObjective':
+    def __deepcopy__(self, memodict: dict = None) -> "AmiciObjective":
         import amici
 
         other = self.__class__.__new__(self.__class__)
 
         for key in set(self.__dict__.keys()) - {
-            'amici_model',
-            'amici_solver',
-            'edatas',
+            "amici_model",
+            "amici_solver",
+            "edatas",
         }:
             other.__dict__[key] = copy.deepcopy(self.__dict__[key])
 
         # copy objects that do not have __deepcopy__
         other.amici_model = self.amici_model.clone()
         other.amici_solver = self.amici_solver.clone()
         other.edatas = [amici.ExpData(data) for data in self.edatas]
 
         return other
 
-    def __getstate__(self) -> Dict:
+    def __getstate__(self) -> dict:
         import amici
 
         if self.amici_object_builder is None:
             raise NotImplementedError(
                 "AmiciObjective does not support __getstate__ without "
                 "an `amici_object_builder`."
             )
 
         state = {}
         for key in set(self.__dict__.keys()) - {
-            'amici_model',
-            'amici_solver',
-            'edatas',
+            "amici_model",
+            "amici_solver",
+            "edatas",
         }:
             state[key] = self.__dict__[key]
 
         _fd, _file = tempfile.mkstemp()
         try:
             # write amici solver settings to file
             try:
@@ -322,53 +320,53 @@
             except AttributeError as e:
                 e.args += (
                     "Pickling the AmiciObjective requires an AMICI "
                     "installation with HDF5 support.",
                 )
                 raise
             # read in byte stream
-            with open(_fd, 'rb', closefd=False) as f:
-                state['amici_solver_settings'] = f.read()
+            with open(_fd, "rb", closefd=False) as f:
+                state["amici_solver_settings"] = f.read()
         finally:
             # close file descriptor and remove temporary file
             os.close(_fd)
             os.remove(_file)
 
-        state['AMICI_model_settings'] = amici.get_model_settings(
+        state["AMICI_model_settings"] = amici.get_model_settings(
             self.amici_model
         )
 
         return state
 
-    def __setstate__(self, state: Dict) -> None:
+    def __setstate__(self, state: dict) -> None:
         import amici
 
-        if state['amici_object_builder'] is None:
+        if state["amici_object_builder"] is None:
             raise NotImplementedError(
                 "AmiciObjective does not support __setstate__ without "
                 "an `amici_object_builder`."
             )
         self.__dict__.update(state)
 
         # note: attributes not defined in the builder are lost
         model = self.amici_object_builder.create_model()
         solver = self.amici_object_builder.create_solver(model)
         edatas = self.amici_object_builder.create_edatas(model)
 
         _fd, _file = tempfile.mkstemp()
         try:
             # write solver settings to temporary file
-            with open(_fd, 'wb', closefd=False) as f:
-                f.write(state['amici_solver_settings'])
+            with open(_fd, "wb", closefd=False) as f:
+                f.write(state["amici_solver_settings"])
             # read in solver settings
             try:
                 amici.readSolverSettingsFromHDF5(_file, solver)
             except AttributeError as err:
                 if not err.args:
-                    err.args = ('',)
+                    err.args = ("",)
                 err.args += (
                     "Unpickling an AmiciObjective requires an AMICI "
                     "installation with HDF5 support.",
                 )
                 raise
         finally:
             # close file descriptor and remove temporary file
@@ -378,20 +376,20 @@
         self.amici_model = model
         self.amici_solver = solver
         self.edatas = edatas
 
         self.apply_custom_timepoints()
         amici.set_model_settings(
             self.amici_model,
-            state['AMICI_model_settings'],
+            state["AMICI_model_settings"],
         )
 
     def check_sensi_orders(
         self,
-        sensi_orders: Tuple[int, ...],
+        sensi_orders: tuple[int, ...],
         mode: ModeType,
     ) -> bool:
         """See `ObjectiveBase` documentation."""
         import amici
 
         if not sensi_orders:
             return True
@@ -416,41 +414,41 @@
     def check_mode(self, mode: ModeType) -> bool:
         """See `ObjectiveBase` documentation."""
         return mode in [MODE_FUN, MODE_RES]
 
     def __call__(
         self,
         x: np.ndarray,
-        sensi_orders: Tuple[int, ...] = (0,),
+        sensi_orders: tuple[int, ...] = (0,),
         mode: ModeType = MODE_FUN,
         return_dict: bool = False,
         **kwargs,
-    ) -> Union[float, np.ndarray, Tuple, ResultDict]:
+    ) -> Union[float, np.ndarray, tuple, ResultDict]:
         """See `ObjectiveBase` documentation."""
         import amici
 
         # Use AMICI full reporting if amici.ReturnDatas are returned and no
         #  other reporting mode was set
         if (
             return_dict
             and self.amici_reporting is None
-            and 'amici_reporting' not in kwargs
+            and "amici_reporting" not in kwargs
         ):
-            kwargs['amici_reporting'] = amici.RDataReporting.full
+            kwargs["amici_reporting"] = amici.RDataReporting.full
 
         return super().__call__(x, sensi_orders, mode, return_dict, **kwargs)
 
     def call_unprocessed(
         self,
         x: np.ndarray,
-        sensi_orders: Tuple[int, ...],
+        sensi_orders: tuple[int, ...],
         mode: ModeType,
-        edatas: Sequence['amici.ExpData'] = None,
-        parameter_mapping: 'ParameterMapping' = None,
-        amici_reporting: Optional['amici.RDataReporting'] = None,
+        edatas: Sequence["amici.ExpData"] = None,
+        parameter_mapping: "ParameterMapping" = None,
+        amici_reporting: Optional["amici.RDataReporting"] = None,
     ):
         """
         Call objective function without pre- or post-processing and formatting.
 
         Returns
         -------
         result:
@@ -473,15 +471,15 @@
                 else amici.RDataReporting.residuals
             )
         self.amici_solver.setReturnDataReportingMode(amici_reporting)
 
         # update steady state
         if (
             self.guess_steadystate
-            and self.steadystate_guesses['fval'] < np.inf
+            and self.steadystate_guesses["fval"] < np.inf
         ):
             for data_ix in range(len(self.edatas)):
                 self.apply_steadystate_guess(data_ix, x_dct)
 
         if edatas is None:
             edatas = self.edatas
         if parameter_mapping is None:
@@ -497,118 +495,116 @@
             x_ids=self.x_ids,
             parameter_mapping=parameter_mapping,
             fim_for_hess=self.fim_for_hess,
         )
 
         nllh = ret[FVAL]
         rdatas = ret[RDATAS]
-        if ret.get(INNER_PARAMETERS, None) is not None:
-            self.inner_parameters = ret[INNER_PARAMETERS]
 
         # check whether we should update data for preequilibration guesses
         if (
             self.guess_steadystate
-            and nllh <= self.steadystate_guesses['fval']
+            and nllh <= self.steadystate_guesses["fval"]
             and nllh < np.inf
         ):
-            self.steadystate_guesses['fval'] = nllh
+            self.steadystate_guesses["fval"] = nllh
             for data_ix, rdata in enumerate(rdatas):
                 self.store_steadystate_guess(data_ix, x_dct, rdata)
 
         return ret
 
-    def par_arr_to_dct(self, x: Sequence[float]) -> Dict[str, float]:
+    def par_arr_to_dct(self, x: Sequence[float]) -> dict[str, float]:
         """Create dict from parameter vector."""
         return OrderedDict(zip(self.x_ids, x))
 
-    def apply_steadystate_guess(self, condition_ix: int, x_dct: Dict) -> None:
+    def apply_steadystate_guess(self, condition_ix: int, x_dct: dict) -> None:
         """
         Apply steady state guess to `edatas[condition_ix].x0`.
 
         Use the stored steadystate as well as the respective sensitivity (
         if available) and parameter value to approximate the steadystate at
         the current parameters using a zeroth or first order taylor
         approximation:
         x_ss(x') = x_ss(x) [+ dx_ss/dx(x)*(x'-x)]
         """
         mapping = self.parameter_mapping[condition_ix].map_sim_var
         x_sim = map_par_opt_to_par_sim(mapping, x_dct, self.amici_model)
         x_ss_guess = []  # resets initial state by default
-        if condition_ix in self.steadystate_guesses['data']:
-            guess_data = self.steadystate_guesses['data'][condition_ix]
-            if guess_data['x_ss'] is not None:
-                x_ss_guess = guess_data['x_ss']
-            if guess_data['sx_ss'] is not None:
+        if condition_ix in self.steadystate_guesses["data"]:
+            guess_data = self.steadystate_guesses["data"][condition_ix]
+            if guess_data["x_ss"] is not None:
+                x_ss_guess = guess_data["x_ss"]
+            if guess_data["sx_ss"] is not None:
                 linear_update = (
-                    guess_data['sx_ss']
+                    guess_data["sx_ss"]
                     .transpose()
                     .dot(
-                        (x_sim - guess_data['x'])[
+                        (x_sim - guess_data["x"])[
                             np.asarray(self.edatas[condition_ix].plist)
                         ]
                     )
                 )
                 # limit linear updates to max 20 % elementwise change
                 if (linear_update / (x_ss_guess + np.spacing(1))).max() < 0.2:
                     x_ss_guess += linear_update
 
         self.edatas[condition_ix].x0 = tuple(x_ss_guess)
 
     def store_steadystate_guess(
         self,
         condition_ix: int,
-        x_dct: Dict,
-        rdata: 'amici.ReturnData',
+        x_dct: dict,
+        rdata: "amici.ReturnData",
     ) -> None:
         """
         Store condition parameter, steadystate and steadystate sensitivity.
 
         Stored in steadystate_guesses if steadystate guesses are enabled for
         this condition.
         """
-        if condition_ix not in self.steadystate_guesses['data']:
+        if condition_ix not in self.steadystate_guesses["data"]:
             return
-        preeq_guesses = self.steadystate_guesses['data'][condition_ix]
+        preeq_guesses = self.steadystate_guesses["data"][condition_ix]
 
         # update parameter
         condition_map_sim_var = self.parameter_mapping[
             condition_ix
         ].map_sim_var
         x_sim = map_par_opt_to_par_sim(
             condition_map_sim_var, x_dct, self.amici_model
         )
-        preeq_guesses['x'] = x_sim
+        preeq_guesses["x"] = x_sim
 
         # update steadystates
-        preeq_guesses['x_ss'] = rdata['x_ss']
-        preeq_guesses['sx_ss'] = rdata['sx_ss']
+        preeq_guesses["x_ss"] = rdata["x_ss"]
+        preeq_guesses["sx_ss"] = rdata["sx_ss"]
 
     def reset_steadystate_guesses(self) -> None:
         """Reset all steadystate guess data."""
         if not self.guess_steadystate:
             return
 
-        self.steadystate_guesses['fval'] = np.inf
-        for condition in self.steadystate_guesses['data']:
-            self.steadystate_guesses['data'][condition] = {}
+        self.steadystate_guesses["fval"] = np.inf
+        for condition in self.steadystate_guesses["data"]:
+            self.steadystate_guesses["data"][condition] = {}
 
     def apply_custom_timepoints(self) -> None:
         """Apply custom timepoints, if applicable.
 
         See the `set_custom_timepoints` method for more information.
         """
         if self.custom_timepoints is not None:
             for index in range(len(self.edatas)):
                 self.edatas[index].setTimepoints(self.custom_timepoints[index])
 
     def set_custom_timepoints(
         self,
         timepoints: Sequence[Sequence[Union[float, int]]] = None,
         timepoints_global: Sequence[Union[float, int]] = None,
-    ) -> 'AmiciObjective':
+    ) -> "AmiciObjective":
         """
         Create a copy of this objective that is evaluated at custom timepoints.
 
         The intended use is to aid in predictions at unmeasured timepoints.
 
         Parameters
         ----------
@@ -620,26 +616,26 @@
             conditions.
 
         Returns
         -------
         The customized copy of this objective.
         """
         if timepoints is None and timepoints_global is None:
-            raise KeyError('Timepoints were not specified.')
+            raise KeyError("Timepoints were not specified.")
 
         amici_objective = copy.deepcopy(self)
 
         if timepoints is not None:
             if len(timepoints) != len(amici_objective.edatas):
                 raise ValueError(
-                    'The number of condition-specific timepoints `timepoints` '
-                    'does not match the number of experimental conditions.\n'
-                    f'Number of provided timepoints: {len(timepoints)}. '
-                    'Number of experimental conditions: '
-                    f'{len(amici_objective.edatas)}.'
+                    "The number of condition-specific timepoints `timepoints` "
+                    "does not match the number of experimental conditions.\n"
+                    f"Number of provided timepoints: {len(timepoints)}. "
+                    "Number of experimental conditions: "
+                    f"{len(amici_objective.edatas)}."
                 )
             custom_timepoints = timepoints
         else:
             custom_timepoints = [
                 copy.deepcopy(timepoints_global)
                 for _ in range(len(amici_objective.edatas))
             ]
@@ -658,13 +654,13 @@
         x: The parameters for which to evaluate the gradient.
 
         Returns
         -------
         bool
             Indicates whether gradients match (True) FDs or not (False)
         """
-        if x is None and 'petab_problem' in dir(self.amici_object_builder):
+        if x is None and "petab_problem" in dir(self.amici_object_builder):
             x = self.amici_object_builder.petab_problem.x_nominal_scaled
             x_free = self.amici_object_builder.petab_problem.x_free_indices
         return super().check_gradients_match_finite_differences(
             *args, x=x, x_free=x_free, **kwargs
         )
```

### Comparing `pypesto-0.4.2/pypesto/objective/amici/amici_calculator.py` & `pypesto-0.5.0/pypesto/objective/amici/amici_calculator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Dict, List, Sequence, Tuple, Union
+from collections.abc import Sequence
+from typing import TYPE_CHECKING, Union
 
 import numpy as np
 
 from ...C import (
     FVAL,
     GRAD,
     HESS,
@@ -24,39 +25,39 @@
     log_simulation,
     sim_sres_to_opt_sres,
 )
 
 if TYPE_CHECKING:
     try:
         import amici
-        from amici.parameter_mapping import ParameterMapping
+        from amici.petab.parameter_mapping import ParameterMapping
     except ImportError:
         ParameterMapping = None
 
-AmiciModel = Union['amici.Model', 'amici.ModelPtr']
-AmiciSolver = Union['amici.Solver', 'amici.SolverPtr']
+AmiciModel = Union["amici.Model", "amici.ModelPtr"]
+AmiciSolver = Union["amici.Solver", "amici.SolverPtr"]
 
 
 class AmiciCalculator:
     """Class to perform the AMICI call and obtain objective function values."""
 
     def __init__(self):
         self._known_least_squares_safe = False
 
     def initialize(self):
         """Initialize the calculator. Default: Do nothing."""
 
     def __call__(
         self,
-        x_dct: Dict,
-        sensi_orders: Tuple[int],
+        x_dct: dict,
+        sensi_orders: tuple[int],
         mode: ModeType,
         amici_model: AmiciModel,
         amici_solver: AmiciSolver,
-        edatas: List[amici.ExpData],
+        edatas: list[amici.ExpData],
         n_threads: int,
         x_ids: Sequence[str],
         parameter_mapping: ParameterMapping,
         fim_for_hess: bool,
     ):
         """Perform the actual AMICI call.
 
@@ -82,29 +83,29 @@
             Ids of optimization parameters.
         parameter_mapping:
             Mapping of optimization to simulation parameters.
         fim_for_hess:
             Whether to use the FIM (if available) instead of the Hessian (if
             requested).
         """
-        import amici.parameter_mapping
+        import amici.petab.conditions
 
         # set order in solver
         sensi_order = 0
         if sensi_orders:
             sensi_order = max(sensi_orders)
 
         if sensi_order == 2 and fim_for_hess:
             # we use the FIM
             amici_solver.setSensitivityOrder(sensi_order - 1)
         else:
             amici_solver.setSensitivityOrder(sensi_order)
 
         # fill in parameters
-        amici.parameter_mapping.fill_in_parameters(
+        amici.petab.conditions.fill_in_parameters(
             edatas=edatas,
             problem_parameters=x_dct,
             scaled_parameters=True,
             parameter_mapping=parameter_mapping,
             amici_model=amici_model,
         )
 
@@ -118,24 +119,24 @@
         if (
             not self._known_least_squares_safe
             and mode == MODE_RES
             and 1 in sensi_orders
         ):
             if not amici_model.getAddSigmaResiduals() and any(
                 (
-                    (r['ssigmay'] is not None and np.any(r['ssigmay']))
-                    or (r['ssigmaz'] is not None and np.any(r['ssigmaz']))
+                    (r["ssigmay"] is not None and np.any(r["ssigmay"]))
+                    or (r["ssigmaz"] is not None and np.any(r["ssigmaz"]))
                 )
                 for r in rdatas
             ):
                 raise RuntimeError(
-                    'Cannot use least squares solver with'
-                    'parameter dependent sigma! Support can be '
-                    'enabled via '
-                    'amici_model.setAddSigmaResiduals().'
+                    "Cannot use least squares solver with"
+                    "parameter dependent sigma! Support can be "
+                    "enabled via "
+                    "amici_model.setAddSigmaResiduals()."
                 )
             self._known_least_squares_safe = True  # don't check this again
 
         return calculate_function_values(
             rdatas=rdatas,
             sensi_orders=sensi_orders,
             mode=mode,
@@ -146,31 +147,31 @@
             parameter_mapping=parameter_mapping,
             fim_for_hess=fim_for_hess,
         )
 
 
 def calculate_function_values(
     rdatas,
-    sensi_orders: Tuple[int, ...],
+    sensi_orders: tuple[int, ...],
     mode: ModeType,
     amici_model: AmiciModel,
     amici_solver: AmiciSolver,
-    edatas: List[amici.ExpData],
+    edatas: list[amici.ExpData],
     x_ids: Sequence[str],
     parameter_mapping: ParameterMapping,
     fim_for_hess: bool,
 ):
     """Calculate the function values from rdatas and return as dict."""
     import amici
 
     # full optimization problem dimension (including fixed parameters)
     dim = len(x_ids)
 
     # check if the simulation failed
-    if any(rdata['status'] < 0.0 for rdata in rdatas):
+    if any(rdata["status"] < 0.0 for rdata in rdatas):
         return get_error_output(
             amici_model, edatas, rdatas, sensi_orders, mode, dim
         )
 
     nllh, snllh, s2nllh, chi2, res, sres = init_return_values(
         sensi_orders, mode, dim
     )
@@ -181,29 +182,29 @@
     # iterate over return data
     for data_ix, rdata in enumerate(rdatas):
         log_simulation(data_ix, rdata)
 
         condition_map_sim_var = parameter_mapping[data_ix].map_sim_var
 
         # add objective value
-        nllh -= rdata['llh']
+        nllh -= rdata["llh"]
 
         if mode == MODE_FUN:
             if not np.isfinite(nllh):
                 return get_error_output(
                     amici_model, edatas, rdatas, sensi_orders, mode, dim
                 )
 
             if 1 in sensi_orders:
                 # add gradient
                 add_sim_grad_to_opt_grad(
                     x_ids,
                     par_sim_ids,
                     condition_map_sim_var,
-                    rdata['sllh'],
+                    rdata["sllh"],
                     snllh,
                     coefficient=-1.0,
                 )
 
                 if not np.isfinite(snllh).all():
                     return get_error_output(
                         amici_model, edatas, rdatas, sensi_orders, mode, dim
@@ -217,37 +218,37 @@
                 ):
                     raise ValueError("AMICI cannot compute Hessians yet.")
                     # add FIM for Hessian
                 add_sim_hess_to_opt_hess(
                     x_ids,
                     par_sim_ids,
                     condition_map_sim_var,
-                    rdata['FIM'],
+                    rdata["FIM"],
                     s2nllh,
                     coefficient=+1.0,
                 )
                 if not np.isfinite(s2nllh).all():
                     return get_error_output(
                         amici_model, edatas, rdatas, sensi_orders, mode, dim
                     )
 
         elif mode == MODE_RES:
             if 0 in sensi_orders:
-                chi2 += rdata['chi2']
+                chi2 += rdata["chi2"]
                 res = (
-                    np.hstack([res, rdata['res']])
+                    np.hstack([res, rdata["res"]])
                     if res.size
-                    else rdata['res']
+                    else rdata["res"]
                 )
             if 1 in sensi_orders:
                 opt_sres = sim_sres_to_opt_sres(
                     x_ids,
                     par_sim_ids,
                     condition_map_sim_var,
-                    rdata['sres'],
+                    rdata["sres"],
                     coefficient=1.0,
                 )
                 sres = np.vstack([sres, opt_sres]) if sres.size else opt_sres
 
     ret = {
         FVAL: nllh,
         GRAD: snllh,
```

### Comparing `pypesto-0.4.2/pypesto/objective/amici/amici_util.py` & `pypesto-0.5.0/pypesto/objective/amici/amici_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import logging
 import numbers
 import warnings
-from typing import TYPE_CHECKING, Dict, Sequence, Tuple, Union
+from collections.abc import Sequence
+from typing import TYPE_CHECKING, Union
 
 import numpy as np
 
 from ...C import (
     FVAL,
     GRAD,
     HESS,
@@ -26,23 +27,23 @@
         from amici.parameter_mapping import (
             ParameterMapping,
             ParameterMappingForCondition,
         )
     except ImportError:
         ParameterMapping = ParameterMappingForCondition = None
 
-AmiciModel = Union['amici.Model', 'amici.ModelPtr']
-AmiciSolver = Union['amici.Solver', 'amici.SolverPtr']
+AmiciModel = Union["amici.Model", "amici.ModelPtr"]
+AmiciSolver = Union["amici.Solver", "amici.SolverPtr"]
 
 logger = logging.getLogger(__name__)
 
 
 def map_par_opt_to_par_sim(
-    condition_map_sim_var: Dict[str, Union[float, str]],
-    x_dct: Dict[str, float],
+    condition_map_sim_var: dict[str, float | str],
+    x_dct: dict[str, float],
     amici_model: AmiciModel,
 ) -> np.ndarray:
     """
     Create simulation vector from optimization vector using the mapping.
 
     Parameters
     ----------
@@ -97,14 +98,15 @@
     plist: array-like of float
         List of parameter indices for which the sensitivity needs to be
         computed
     """
     warnings.warn(
         "This function will be removed in future releases. ",
         DeprecationWarning,
+        stacklevel=2,
     )
     plist = []
 
     # iterate over simulation parameter indices
     for j_par_sim, val in enumerate(mapping_par_opt_to_par_sim):
         if not isinstance(val, numbers.Number):
             plist.append(j_par_sim)
@@ -144,16 +146,16 @@
         parameter_mapping.append(mapping_for_condition)
     return parameter_mapping
 
 
 def par_index_slices(
     par_opt_ids: Sequence[str],
     par_sim_ids: Sequence[str],
-    condition_map_sim_var: Dict[str, Union[float, str]],
-) -> Tuple[np.ndarray, np.ndarray]:
+    condition_map_sim_var: dict[str, float | str],
+) -> tuple[np.ndarray, np.ndarray]:
     """
     Generate numpy arrays for indexing based on `mapping_par_opt_to_par_sim`.
 
     Parameters
     ----------
     par_opt_ids:
         The optimization parameter ids. Needed for order.
@@ -205,15 +207,15 @@
     par_opt_slice = np.fromiter(next(zip_iterator), dtype=int)
     return par_sim_slice, par_opt_slice
 
 
 def add_sim_grad_to_opt_grad(
     par_opt_ids: Sequence[str],
     par_sim_ids: Sequence[str],
-    condition_map_sim_var: Dict[str, Union[float, str]],
+    condition_map_sim_var: dict[str, float | str],
     sim_grad: np.ndarray,
     opt_grad: np.ndarray,
     coefficient: float = 1.0,
 ) -> None:
     """
     Sum simulation gradients to objective gradient.
 
@@ -253,15 +255,15 @@
                     coefficient * sim_grad[par_sim_slice[idx]]
                 )
 
 
 def add_sim_hess_to_opt_hess(
     par_opt_ids: Sequence[str],
     par_sim_ids: Sequence[str],
-    condition_map_sim_var: Dict[str, Union[float, str]],
+    condition_map_sim_var: dict[str, float | str],
     sim_hess: np.ndarray,
     opt_hess: np.ndarray,
     coefficient: float = 1.0,
 ) -> None:
     """
     Sum simulation hessians to objective hessian.
 
@@ -304,15 +306,15 @@
                     * sim_hess[par_sim_slice[idx], par_sim_slice[jdx]]
                 )
 
 
 def sim_sres_to_opt_sres(
     par_opt_ids: Sequence[str],
     par_sim_ids: Sequence[str],
-    condition_map_sim_var: Dict[str, Union[float, str]],
+    condition_map_sim_var: dict[str, float | str],
     sim_sres: np.ndarray,
     coefficient: float = 1.0,
 ) -> np.ndarray:
     """
 
     Sum simulation residual sensitivities to objective residual sensitivities.
 
@@ -346,27 +348,27 @@
 
 def log_simulation(data_ix, rdata) -> None:
     """Log the simulation results."""
     logger.debug(f"=== DATASET {data_ix} ===")
     logger.debug(f"status: {rdata['status']}")
     logger.debug(f"llh: {rdata['llh']}")
 
-    t_steadystate = 't_steadystate'
+    t_steadystate = "t_steadystate"
     if t_steadystate in rdata and rdata[t_steadystate] != np.nan:
         logger.debug(f"t_steadystate: {rdata[t_steadystate]}")
 
     if log_level_active(logger, logging.DEBUG):
         logger.debug(f"res: {rdata['res']}")
 
 
 def get_error_output(
     amici_model: AmiciModel,
-    edatas: Sequence['amici.ExpData'],
-    rdatas: Sequence['amici.ReturnData'],
-    sensi_orders: Tuple[int, ...],
+    edatas: Sequence[amici.ExpData],
+    rdatas: Sequence[amici.ReturnData],
+    sensi_orders: tuple[int, ...],
     mode: ModeType,
     dim: int,
 ) -> dict:
     """Get default output upon error.
 
     Returns values indicative of an error, that is with nan entries in all
     vectors, and a function value, i.e. nllh, of `np.inf`.
@@ -397,15 +399,15 @@
         SRES: sres,
         RDATAS: rdatas,
     }
     return filter_return_dict(ret)
 
 
 def init_return_values(
-    sensi_orders: Tuple[int, ...],
+    sensi_orders: tuple[int, ...],
     mode: ModeType,
     dim: int,
     error: bool = False,
 ):
     """Initialize return values."""
     if error:
         fval = np.inf
```

### Comparing `pypesto-0.4.2/pypesto/objective/base.py` & `pypesto-0.5.0/pypesto/objective/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import copy
 import logging
 from abc import ABC, abstractmethod
-from typing import Dict, Iterable, List, Optional, Sequence, Tuple, Union
+from collections.abc import Iterable, Sequence
+from typing import Optional, Union
 
 import numpy as np
 import pandas as pd
 
 from ..C import FVAL, GRAD, HESS, MODE_FUN, MODE_RES, RES, SRES, ModeType
 from ..history import NoHistory, create_history
 from .pre_post_process import FixedParametersProcessor, PrePostProcessor
 
-ResultDict = Dict[str, Union[float, np.ndarray, Dict]]
+ResultDict = dict[str, Union[float, np.ndarray, dict]]
 
 logger = logging.getLogger(__name__)
 
 
 class ObjectiveBase(ABC):
     """
     Abstract objective class.
@@ -51,21 +52,14 @@
         x_names: Optional[Sequence[str]] = None,
     ):
         self._x_names = x_names
 
         self.pre_post_processor = PrePostProcessor()
         self.history = NoHistory()
 
-    def __deepcopy__(self, memodict=None) -> 'ObjectiveBase':
-        """Create deepcopy of objective object."""
-        other = type(self)()  # maintain type for derived classes
-        for attr, val in self.__dict__.items():
-            other.__dict__[attr] = copy.deepcopy(val)
-        return other
-
     # The following has_ properties can be used to find out what values
     # the objective supports.
     @property
     def has_fun(self) -> bool:
         """Check whether function is defined."""
         return self.check_sensi_orders((0,), MODE_FUN)
 
@@ -92,15 +86,15 @@
 
     @property
     def has_sres(self) -> bool:
         """Check whether residual sensitivities are defined."""
         return self.check_sensi_orders((1,), MODE_RES)
 
     @property
-    def x_names(self) -> Union[List[str], None]:
+    def x_names(self) -> Union[list[str], None]:
         """Parameter names."""
         if self._x_names is None:
             return self._x_names
 
         # change from numpy array with `str_` dtype to list with `str` dtype
         # to avoid issues when writing to hdf (and correctness of typehint)
         return [
@@ -122,19 +116,19 @@
     def create_history(self, id, x_names, options):
         """See `history.generate.create_history` documentation."""
         return create_history(id, x_names, options)
 
     def __call__(
         self,
         x: np.ndarray,
-        sensi_orders: Tuple[int, ...] = (0,),
+        sensi_orders: tuple[int, ...] = (0,),
         mode: ModeType = MODE_FUN,
         return_dict: bool = False,
         **kwargs,
-    ) -> Union[float, np.ndarray, Tuple, ResultDict]:
+    ) -> Union[float, np.ndarray, tuple, ResultDict]:
         """
         Obtain arbitrary sensitivities.
 
         This is the central method which is always called, also by the
         get_* methods.
 
         There are different ways in which an optimizer calls the objective
@@ -204,15 +198,15 @@
 
         return result
 
     @abstractmethod
     def call_unprocessed(
         self,
         x: np.ndarray,
-        sensi_orders: Tuple[int, ...],
+        sensi_orders: tuple[int, ...],
         mode: ModeType,
         **kwargs,
     ) -> ResultDict:
         """
         Call objective function without pre- or post-processing and formatting.
 
         Parameters
@@ -256,20 +250,20 @@
 
     def get_config(self) -> dict:
         """
         Get the configuration information of the objective function.
 
         Return it as a dictionary.
         """
-        info = {'type': self.__class__.__name__}
+        info = {"type": self.__class__.__name__}
         return info
 
     def check_sensi_orders(
         self,
-        sensi_orders: Tuple[int, ...],
+        sensi_orders: tuple[int, ...],
         mode: ModeType,
     ) -> bool:
         """
         Check if the objective is able to compute the requested sensitivities.
 
         Either `check_sensi_orders` or the `fun_...` functions
         must be overwritten in derived classes.
@@ -313,18 +307,18 @@
         ):
             return False
 
         return True
 
     @staticmethod
     def output_to_tuple(
-        sensi_orders: Tuple[int, ...],
+        sensi_orders: tuple[int, ...],
         mode: ModeType,
         **kwargs: Union[float, np.ndarray],
-    ) -> Tuple:
+    ) -> tuple:
         """
         Return values as requested by the caller.
 
         Usually only a subset of outputs is demanded. One output is returned
         as-is, more than one output are returned as a tuple in order (fval,
         grad, hess).
         """
@@ -414,15 +408,15 @@
             x_fixed_vals=x_fixed_vals,
         )
 
     def check_grad_multi_eps(
         self,
         *args,
         multi_eps: Optional[Iterable] = None,
-        label: str = 'rel_err',
+        label: str = "rel_err",
         **kwargs,
     ):
         """
         Compare gradient evaluation.
 
         Equivalent to the `ObjectiveBase.check_grad` method, except multiple
         finite difference step sizes are tested. The result contains the
@@ -435,32 +429,32 @@
         multi_eps:
             The finite difference step sizes to be tested.
         label:
             The label of the column that will be minimized for each parameter.
             Valid options are the column labels of the dataframe returned by
             the `ObjectiveBase.check_grad` method.
         """
-        if 'eps' in kwargs:
+        if "eps" in kwargs:
             raise KeyError(
-                'Please use the `multi_eps` (not the `eps`) argument with '
-                '`check_grad_multi_eps` to specify step sizes.'
+                "Please use the `multi_eps` (not the `eps`) argument with "
+                "`check_grad_multi_eps` to specify step sizes."
             )
 
         if multi_eps is None:
             multi_eps = {1e-1, 1e-3, 1e-5, 1e-7, 1e-9}
 
         results = {}
         for eps in multi_eps:
             results[eps] = self.check_grad(*args, **kwargs, eps=eps)
 
         # The combined result is, for each parameter, the gradient check from
         # the step size (`eps`) that produced the smallest error (`label`).
         combined_result = None
         for eps, result in results.items():
-            result['eps'] = eps
+            result["eps"] = eps
             if combined_result is None:
                 combined_result = result
                 continue
             # Replace rows in `combined_result` with corresponding rows
             # in `result` that have an improved value in column `label`.
             mask_improvements = result[label] < combined_result[label]
             combined_result.loc[mask_improvements, :] = result.loc[
@@ -570,22 +564,22 @@
                         abs(fd_b_ix - fd_c_ix),
                     ]
                 )
 
             # log for dimension ix
             if verbosity > 1:
                 logger.info(
-                    f'index:    {ix}\n'
-                    f'grad:     {grad_ix}\n'
-                    f'fd_f:     {fd_f_ix}\n'
-                    f'fd_b:     {fd_b_ix}\n'
-                    f'fd_c:     {fd_c_ix}\n'
-                    f'fd_err:   {fd_err_ix}\n'
-                    f'abs_err:  {abs_err_ix}\n'
-                    f'rel_err:  {rel_err_ix}\n'
+                    f"index:    {ix}\n"
+                    f"grad:     {grad_ix}\n"
+                    f"fd_f:     {fd_f_ix}\n"
+                    f"fd_b:     {fd_b_ix}\n"
+                    f"fd_c:     {fd_c_ix}\n"
+                    f"fd_err:   {fd_err_ix}\n"
+                    f"abs_err:  {abs_err_ix}\n"
+                    f"rel_err:  {rel_err_ix}\n"
                 )
 
             # append to lists
             grad_list.append(grad_ix)
             fd_f_list.append(fd_f_ix)
             fd_b_list.append(fd_b_ix)
             fd_c_list.append(fd_c_ix)
@@ -596,43 +590,43 @@
                 fval_p_list.append(fval_p)
                 fval_m_list.append(fval_m)
                 std_check_list.append(std_check_ix)
                 mean_check_list.append(mean_check_ix)
 
         # create data dictionary for dataframe
         data = {
-            'grad': grad_list,
-            'fd_f': fd_f_list,
-            'fd_b': fd_b_list,
-            'fd_c': fd_c_list,
-            'fd_err': fd_err_list,
-            'abs_err': abs_err_list,
-            'rel_err': rel_err_list,
+            "grad": grad_list,
+            "fd_f": fd_f_list,
+            "fd_b": fd_b_list,
+            "fd_c": fd_c_list,
+            "fd_err": fd_err_list,
+            "abs_err": abs_err_list,
+            "rel_err": rel_err_list,
         }
 
         # update data dictionary if detailed output is requested
         if detailed:
             prefix_data = {
-                'fval': [fval] * len(x_indices),
-                'fval_p': fval_p_list,
-                'fval_m': fval_m_list,
+                "fval": [fval] * len(x_indices),
+                "fval_p": fval_p_list,
+                "fval_m": fval_m_list,
             }
-            std_str = '(grad-fd_c)/std({fd_f,fd_b,fd_c})'
-            mean_str = '|grad-fd_c|/mean(|fd_f-fd_b|,|fd_f-fd_c|,|fd_b-fd_c|)'
+            std_str = "(grad-fd_c)/std({fd_f,fd_b,fd_c})"
+            mean_str = "|grad-fd_c|/mean(|fd_f-fd_b|,|fd_f-fd_c|,|fd_b-fd_c|)"
             postfix_data = {
                 std_str: std_check_list,
                 mean_str: mean_check_list,
             }
             data = {**prefix_data, **data, **postfix_data}
 
         # create dataframe
         result = pd.DataFrame(
             data=data,
             index=[
-                self.x_names[ix] if self.x_names is not None else f'x_{ix}'
+                self.x_names[ix] if self.x_names is not None else f"x_{ix}"
                 for ix in x_indices
             ],
         )
 
         # log full result
         if verbosity > 0:
             logger.info(result)
```

### Comparing `pypesto-0.4.2/pypesto/objective/finite_difference.py` & `pypesto-0.5.0/pypesto/objective/finite_difference.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Finite differences."""
 
 import copy
 import logging
-from typing import Callable, Dict, List, Tuple, Union
+from typing import Callable, Union
 
 import numpy as np
 
 from ..C import FVAL, GRAD, HESS, MODE_FUN, MODE_RES, RES, SRES, ModeType
 from .base import ObjectiveBase, ResultDict
 
 logger = logging.getLogger(__name__)
@@ -311,15 +311,15 @@
         hess: Union[bool, None] = None,
         sres: Union[bool, None] = None,
         hess_via_fval: bool = True,
         delta_fun: Union[FDDelta, np.ndarray, float, str] = 1e-6,
         delta_grad: Union[FDDelta, np.ndarray, float, str] = 1e-6,
         delta_res: Union[FDDelta, float, np.ndarray, str] = 1e-6,
         method: str = CENTRAL,
-        x_names: List[str] = None,
+        x_names: list[str] = None,
     ):
         super().__init__(x_names=x_names)
         self.obj: ObjectiveBase = obj
         self.grad: Union[bool, None] = grad
         self.hess: Union[bool, None] = hess
         self.sres: Union[bool, None] = sres
         self.hess_via_fval: bool = hess_via_fval
@@ -331,16 +331,16 @@
         if method not in FD.METHODS:
             raise ValueError(
                 f"Method must be one of {FD.METHODS}.",
             )
 
     def __deepcopy__(
         self,
-        memodict: Dict = None,
-    ) -> 'FD':
+        memodict: dict = None,
+    ) -> "FD":
         """Create deepcopy of Objective."""
         other = self.__class__.__new__(self.__class__)
         for attr, val in self.__dict__.items():
             other.__dict__[attr] = copy.deepcopy(val)
         return other
 
     @property
@@ -367,15 +367,15 @@
     def has_sres(self) -> bool:
         """Check whether residual sensitivities are defined."""
         return self.sres is not False and self.obj.has_res
 
     def call_unprocessed(
         self,
         x: np.ndarray,
-        sensi_orders: Tuple[int, ...],
+        sensi_orders: tuple[int, ...],
         mode: ModeType,
         **kwargs,
     ) -> ResultDict:
         """
         See `ObjectiveBase` for more documentation.
 
         Main method to overwrite from the base class. It handles and
@@ -393,15 +393,15 @@
             raise ValueError("This mode is not supported.")
 
         return result
 
     def _call_mode_fun(
         self,
         x: np.ndarray,
-        sensi_orders: Tuple[int, ...],
+        sensi_orders: tuple[int, ...],
         **kwargs,
     ) -> ResultDict:
         """Handle calls in function value mode.
 
         Delegated from `call_unprocessed`.
         """
         # get from objective what it can and should deliver
@@ -482,15 +482,15 @@
                 result[HESS] = 0.5 * (hess + hess.T)
 
         return result
 
     def _call_mode_res(
         self,
         x: np.ndarray,
-        sensi_orders: Tuple[int, ...],
+        sensi_orders: tuple[int, ...],
         **kwargs,
     ) -> ResultDict:
         """Handle calls in residual mode.
 
         Delegated from `call_unprocessed`.
         """
         # get from objective what it can and should deliver
@@ -527,17 +527,17 @@
         result[SRES] = sres.T
 
         return result
 
     def _call_from_obj_fun(
         self,
         x: np.ndarray,
-        sensi_orders: Tuple[int, ...],
+        sensi_orders: tuple[int, ...],
         **kwargs,
-    ) -> Tuple[Tuple[int, ...], ResultDict]:
+    ) -> tuple[tuple[int, ...], ResultDict]:
         """
         Call objective function for sensitivities.
 
         Calculate from the objective the sensitivities that are supposed to
         be calculated from the objective and not via FDs.
         """
         # define objective sensis
@@ -556,17 +556,17 @@
                 x=x, sensi_orders=sensi_orders_obj, mode=MODE_FUN, **kwargs
             )
         return sensi_orders_obj, result
 
     def _call_from_obj_res(
         self,
         x: np.ndarray,
-        sensi_orders: Tuple[int, ...],
+        sensi_orders: tuple[int, ...],
         **kwargs,
-    ) -> Tuple[Tuple[int, ...], ResultDict]:
+    ) -> tuple[tuple[int, ...], ResultDict]:
         """
         Call objective function for sensitivities in residual mode.
 
         Calculate from the objective the sensitivities that are supposed to
         be calculated from the objective and not via FDs.
         """
         # define objective sensis
```

### Comparing `pypesto-0.4.2/pypesto/objective/function.py` & `pypesto-0.5.0/pypesto/objective/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Callable, Sequence, Tuple, Union
+from collections.abc import Sequence
+from typing import Callable, Union
 
 import numpy as np
 
 from ..C import FVAL, GRAD, HESS, MODE_FUN, MODE_RES, RES, SRES, ModeType
 from .base import ObjectiveBase, ResultDict
 
 
@@ -115,27 +116,27 @@
     def has_sres(self) -> bool:
         """Check whether residual sensitivities are defined."""
         return callable(self.sres) or self.sres is True
 
     def get_config(self) -> dict:
         """Return basic information of the objective configuration."""
         info = super().get_config()
-        info['x_names'] = self.x_names
+        info["x_names"] = self.x_names
         sensi_order = 0
         while self.check_sensi_orders(
             sensi_orders=(sensi_order,), mode=MODE_FUN
         ):
             sensi_order += 1
-        info['sensi_order'] = sensi_order - 1
+        info["sensi_order"] = sensi_order - 1
         return info
 
     def call_unprocessed(
         self,
         x: np.ndarray,
-        sensi_orders: Tuple[int, ...],
+        sensi_orders: tuple[int, ...],
         mode: ModeType,
         **kwargs,
     ) -> ResultDict:
         """
         Call objective function without pre- or post-processing and formatting.
 
         Returns
@@ -150,15 +151,15 @@
         else:
             raise ValueError("This mode is not supported.")
         return result
 
     def _call_mode_fun(
         self,
         x: np.ndarray,
-        sensi_orders: Tuple[int, ...],
+        sensi_orders: tuple[int, ...],
     ) -> ResultDict:
         if not sensi_orders:
             result = {}
 
         elif sensi_orders == (0,):
             if self.grad is True:
                 fval = self.fun(x)[0]
@@ -220,15 +221,15 @@
             raise ValueError("These sensitivity orders are not supported.")
 
         return result
 
     def _call_mode_res(
         self,
         x: np.ndarray,
-        sensi_orders: Tuple[int, ...],
+        sensi_orders: tuple[int, ...],
     ) -> ResultDict:
         if not sensi_orders:
             result = {}
 
         elif sensi_orders == (0,):
             if self.sres is True:
                 res = self.res(x)[0]
```

### Comparing `pypesto-0.4.2/pypesto/objective/jax/base.py` & `pypesto-0.5.0/pypesto/objective/jax/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,268 +4,215 @@
 Adds an interface for the construction of loss functions
 incorporating jax models. This permits computation of derivatives using a
 combination of objective based methods and jax based autodiff.
 """
 
 import copy
 from functools import partial
-from typing import Callable, Sequence, Tuple
+from typing import Union
 
 import numpy as np
 
-from ...C import FVAL, GRAD, HESS, MODE_FUN, RDATAS, ModeType
+from ...C import MODE_FUN, ModeType
 from ..base import ObjectiveBase, ResultDict
 
 try:
     import jax
-    import jax.experimental.host_callback as hcb
     import jax.numpy as jnp
-    from jax import custom_jvp, grad
+    from jax import custom_jvp
 except ImportError:
     raise ImportError(
         "Using a jax objective requires an installation of "
         "the python package jax. Please install jax via "
         "`pip install jax jaxlib`."
-    )
+    ) from None
 
-# jax compatible (jittable) objective function using host callback, see
-# https://jax.readthedocs.io/en/latest/jax.experimental.host_callback.html
+# jax compatible (jit-able) objective function using external callback, see
+# https://jax.readthedocs.io/en/latest/notebooks/external_callbacks.html
 
 
 @partial(custom_jvp, nondiff_argnums=(0,))
-def _device_fun(obj: 'JaxObjective', x: jnp.array):
-    """Jax compatible objective function execution using host callback.
-
-    This function does not actually call the underlying objective function,
-    but instead extracts cached return values. Thus it must only be called
-    from within obj.call_unprocessed, and obj.cached_base_ret must be populated.
+def _device_fun(base_objective: ObjectiveBase, x: jnp.array):
+    """Jax compatible objective function execution using external callback.
 
     Parameters
     ----------
     obj:
         The wrapped jax objective.
     x:
         jax computed input array.
-
-    Note
-    ----
-    This function should rather be implemented as class method of JaxObjective,
-    but this is not possible at the time of writing as this is not supported
-    by signature inspection in the underlying bind call.
     """
-    return hcb.call(
-        obj.cached_fval,
+    return jax.pure_callback(
+        partial(base_objective, sensi_orders=(0,)),
+        jax.ShapeDtypeStruct((), x.dtype),
         x,
-        result_shape=jax.ShapeDtypeStruct((), np.float64),
     )
 
 
-@partial(custom_jvp, nondiff_argnums=(0,))
-def _device_fun_grad(obj: 'JaxObjective', x: jnp.array):
-    """Jax compatible objective gradient execution using host callback.
+def _device_fun_value_and_grad(base_objective: ObjectiveBase, x: jnp.array):
+    """Jax compatible objective gradient execution using external callback.
 
-    This function does not actually call the underlying objective function,
-    but instead extracts cached return values. Thus it must only be called
-    from within obj.call_unprocessed and obj.cached_base_ret must be populated.
+    This function will be called when computing the gradient of the
+    `JaxObjective` using `jax.grad` or `jax.value_and_grad`. In the latter
+    case, the function will return both the function value and the gradient,
+    so no caching is necessary. For higher order derivatives, caching would
+    be advantageous, but unclear how to implement this.
 
     Parameters
     ----------
     obj:
         The wrapped jax objective.
     x:
         jax computed input array.
-
-    Note
-    ----
-    This function should rather be implemented as class method of JaxObjective,
-    but this is not possible at the time of writing as this is not supported
-    by signature inspection in the underlying bind call.
     """
-    return hcb.call(
-        obj.cached_grad,
-        x,
-        result_shape=jax.ShapeDtypeStruct(
-            obj.cached_base_ret[GRAD].shape,  # bootstrap from cached value
-            np.float64,
+    return jax.pure_callback(
+        partial(
+            base_objective,
+            sensi_orders=(
+                0,
+                1,
+            ),
         ),
-    )
-
-
-def _device_fun_hess(obj: 'JaxObjective', x: jnp.array):
-    """Jax compatible objective Hessian execution using host callback.
-
-    This function does not actually call the underlying objective function,
-    but instead extracts cached return values. Thus it must only be called
-    from within obj.call_unprocessed and obj.cached_base_ret must be populated.
-
-    Parameters
-    ----------
-    obj:
-        The wrapped jax objective.
-    x:
-        jax computed input array.
-
-    Note
-    ----
-    This function should rather be implemented as class method of JaxObjective,
-    but this is not possible at the time of writing as this is not supported
-    by signature inspection in the underlying bind call.
-    """
-    return hcb.call(
-        obj.cached_hess,
-        x,
-        result_shape=jax.ShapeDtypeStruct(
-            obj.cached_base_ret[HESS].shape,  # bootstrap from cached value
-            np.float64,
+        (
+            jax.ShapeDtypeStruct((), x.dtype),
+            jax.ShapeDtypeStruct(
+                x.shape,  # bootstrap from cached value
+                x.dtype,
+            ),
         ),
+        x,
     )
 
 
-# define custom jvp for device_fun & device_fun_grad to enable autodiff, see
+# define custom jvp for device_fun to enable autodiff, see
 # https://jax.readthedocs.io/en/latest/notebooks/Custom_derivative_rules_for_Python_code.html
 
 
 @_device_fun.defjvp
 def _device_fun_jvp(
-    obj: 'JaxObjective', primals: jnp.array, tangents: jnp.array
+    obj: "JaxObjective", primals: jnp.array, tangents: jnp.array
 ):
     """JVP implementation for device_fun."""
     (x,) = primals
     (x_dot,) = tangents
-    return _device_fun(obj, x), _device_fun_grad(obj, x).dot(x_dot)
-
-
-@_device_fun_grad.defjvp
-def _device_fun_grad_jvp(
-    obj: 'JaxObjective', primals: jnp.array, tangents: jnp.array
-):
-    """JVP implementation for device_fun_grad."""
-    (x,) = primals
-    (x_dot,) = tangents
-    return _device_fun_grad(obj, x), _device_fun_hess(obj, x).dot(x_dot)
+    value, grad = _device_fun_value_and_grad(obj, x)
+    return value, grad @ x_dot
 
 
 class JaxObjective(ObjectiveBase):
-    """Objective function that combines pypesto objectives with jax functions.
+    """Objective function that enables use of pypesto objectives in jax models.
 
-    The generated objective function will evaluate objective(jax_fun(x)).
+    The generated function should generally be compatible with jax, but cannot
+    compute higher order derivatives and is not vectorized (but still
+    compatible with jax.vmap)
 
     Parameters
     ----------
     objective:
-        pyPESTO objective
-    jax_fun:
-        jax function (not jitted) that computes input to the pyPESTO objective
+        pyPESTO objective to be wrapped.
+
+    Note
+    ----
+    Currently only implements MODE_FUN and sensi_orders=(0,). Support for
+    MODE_RES should be straightforward to add.
     """
 
     def __init__(
         self,
         objective: ObjectiveBase,
-        jax_fun: Callable,
-        x_names: Sequence[str] = None,
     ):
         if not isinstance(objective, ObjectiveBase):
-            raise TypeError('objective must be an ObjectiveBase instance')
+            raise TypeError("objective must be an ObjectiveBase instance")
         if not objective.check_mode(MODE_FUN):
             raise NotImplementedError(
-                f'objective must support mode={MODE_FUN}'
+                f"objective must support mode={MODE_FUN}"
             )
-        super().__init__(x_names)
         self.base_objective = objective
 
-        self.jax_fun = jax_fun
-
         # would be cleaner to also have this as class method, but not supported
         # by signature inspection in bind call.
-        def jax_objective(x):
-            # device fun doesn't actually need the value of y, but we need to
-            # compute this here for autodiff to work
-            y = jax_fun(x)
-            return _device_fun(self, y)
-
-        # jit objective & derivatives (not integrated)
-        self.jax_objective = jax.jit(jax_objective)
-        self.jax_objective_grad = jax.jit(grad(jax_objective))
-        self.jax_objective_hess = jax.jit(jax.hessian(jax_objective))
-
-        # jit input function
-        self.infun = jax.jit(self.jax_fun)
-
-        # temporary storage for evaluation results of objective
-        self.cached_base_ret: ResultDict = {}
-
-    def cached_fval(self, _):
-        """Return cached function value."""
-        return self.cached_base_ret[FVAL]
-
-    def cached_grad(self, _):
-        """Return cached gradient."""
-        return self.cached_base_ret[GRAD]
-
-    def cached_hess(self, _):
-        """Return cached Hessian."""
-        return self.cached_base_ret[HESS]
+        self.jax_objective = partial(_device_fun, self.base_objective)
 
     def check_mode(self, mode: ModeType) -> bool:
         """See `ObjectiveBase` documentation."""
         return mode == MODE_FUN
 
     def check_sensi_orders(self, sensi_orders, mode: ModeType) -> bool:
         """See `ObjectiveBase` documentation."""
         if not self.check_mode(mode):
             return False
         else:
-            return self.base_objective.check_sensi_orders(sensi_orders, mode)
+            return (
+                self.base_objective.check_sensi_orders(sensi_orders, mode)
+                and max(sensi_orders) == 0
+            )
 
-    def call_unprocessed(
+    def __call__(
         self,
-        x: np.ndarray,
-        sensi_orders: Tuple[int, ...],
-        mode: ModeType,
+        x: jnp.ndarray,
+        sensi_orders: tuple[int, ...] = (0,),
+        mode: ModeType = MODE_FUN,
+        return_dict: bool = False,
         **kwargs,
-    ) -> ResultDict:
+    ) -> Union[jnp.ndarray, tuple, ResultDict]:
         """
-        See `ObjectiveBase` for more documentation.
+        See :class:`ObjectiveBase` for more documentation.
 
-        Main method to overwrite from the base class. It handles and
-        delegates the actual objective evaluation.
+        Note that this function delegates pre- and post-processing as well as
+        history handling to the inner objective.
         """
-        # derivative computation in jax always requires lower order
-        # derivatives, see jvp rules for device_fun and device_fun_grad.
-        if 2 in sensi_orders:
-            sensi_orders = (0, 1, 2)
-        elif 1 in sensi_orders:
-            sensi_orders = (0, 1)
-        else:
-            sensi_orders = (0,)
+
+        if not self.check_mode(mode):
+            raise ValueError(
+                f"This Objective cannot be called with mode" f"={mode}."
+            )
+        if not self.check_sensi_orders(sensi_orders, mode):
+            raise ValueError(
+                f"This Objective cannot be called with "
+                f"sensi_orders= {sensi_orders} and mode={mode}."
+            )
 
         # this computes all the results from the inner objective, rendering
         # them accessible as cached values for device_fun, etc.
-        set_return_dict, return_dict = (
-            'return_dict' in kwargs,
-            kwargs.pop('return_dict', False),
-        )
-        self.cached_base_ret = self.base_objective(
-            self.infun(x), sensi_orders, mode, return_dict=True, **kwargs
-        )
-        if set_return_dict:
-            kwargs['return_dict'] = return_dict
-        ret = {}
-        if RDATAS in self.cached_base_ret:
-            ret[RDATAS] = self.cached_base_ret[RDATAS]
-        if 0 in sensi_orders:
-            ret[FVAL] = float(self.jax_objective(x))
-        if 1 in sensi_orders:
-            ret[GRAD] = self.jax_objective_grad(x)
-        if 2 in sensi_orders:
-            ret[HESS] = self.jax_objective_hess(x)
+        if kwargs.pop("return_dict", False):
+            raise ValueError(
+                "return_dict=True is not available for JaxObjective evaluation"
+            )
 
-        return ret
+        return self.jax_objective(x)
+
+    def call_unprocessed(
+        self,
+        x: np.ndarray,
+        sensi_orders: tuple[int, ...],
+        mode: ModeType,
+        **kwargs,
+    ) -> ResultDict:
+        """
+        See :class:`ObjectiveBase` for more documentation.
+
+        This function is not implemented for JaxObjective as it is not called
+        in the override for __call__. However, it's marked as abstract so we
+        need to implement it.
+        """
+        pass
 
     def __deepcopy__(self, memodict=None):
         other = JaxObjective(
             copy.deepcopy(self.base_objective),
-            copy.deepcopy(self.jax_fun),
-            copy.deepcopy(self.x_names),
         )
-
         return other
+
+    @property
+    def history(self):
+        """Exposes the history of the inner objective."""
+        return self.base_objective.history
+
+    @property
+    def pre_post_processor(self):
+        """Exposes the pre_post_processor of inner objective."""
+        return self.base_objective.pre_post_processor
+
+    @property
+    def x_names(self):
+        """Exposes the x_names of inner objective."""
+        return self.base_objective.x_names
```

### Comparing `pypesto-0.4.2/pypesto/objective/julia/base.py` & `pypesto-0.5.0/pypesto/objective/julia/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         # lazy imports
         try:
             from julia import Main  # noqa: F401
         except ImportError:
             raise ImportError(
                 "Install PyJulia, e.g. via `pip install pypesto[julia]`, "
                 "and see the class documentation",
-            )
+            ) from None
 
         # store module name and source file
         self.module: str = module
         if source_file is None:
             source_file = module + ".jl"
         self.source_file: str = source_file
         _read_source(self.module, self.source_file)
@@ -166,15 +166,15 @@
         for key, val in d.items():
             setattr(self, key, val)
         _read_source(self.module, self.source_file)
 
         fun, grad, hess, res, sres = self._get_callables()
         super().__init__(fun=fun, grad=grad, hess=hess, res=res, sres=sres)
 
-    def __deepcopy__(self, memodict=None) -> 'JuliaObjective':
+    def __deepcopy__(self, memodict=None) -> "JuliaObjective":
         return JuliaObjective(
             module=self.module,
             source_file=self.source_file,
             fun=self._fun,
             grad=self._grad,
             hess=self._hess,
             res=self._res,
@@ -191,11 +191,11 @@
 
     with open(source_file) as f:
         code = f.read()
 
     formatter = HtmlFormatter()
     return display.HTML(
         '<style type="text/css">{}</style>{}'.format(
-            formatter.get_style_defs('.highlight'),
+            formatter.get_style_defs(".highlight"),
             highlight(code, JuliaLexer(), formatter),
         )
     )
```

### Comparing `pypesto-0.4.2/pypesto/objective/julia/petabJl.py` & `pypesto-0.5.0/pypesto/objective/julia/petabJl.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             from julia import Main, Pkg  # noqa: F401
 
             Pkg.activate(".")
         except ImportError:
             raise ImportError(
                 "Install PyJulia, e.g. via `pip install pypesto[julia]`, "
                 "and see the class documentation",
-            )
+            ) from None
 
         self.module = module
         self.source_file = source_file
         self._petab_problem_name = petab_problem_name
         if precompile:
             self.precompile_model(force_compile=force_compile)
 
@@ -72,34 +72,36 @@
             fun=fun, grad=grad, hess=hess, x_names=x_names
         )
 
     def __getstate__(self):
         """Get state for pickling."""
         # if not dumped, dump it via JLD2
         return {
-            'module': self.module,
-            'source_file': self.source_file,
-            '_petab_problem_name': self._petab_problem_name,
+            "module": self.module,
+            "source_file": self.source_file,
+            "_petab_problem_name": self._petab_problem_name,
         }
 
     def __setstate__(self, state):
         """Set state from pickling."""
         for key, value in state.items():
             setattr(self, key, value)
         # lazy imports
         try:
-            from julia import Main  # noqa: F401
-            from julia import Pkg
+            from julia import (
+                Main,  # noqa: F401
+                Pkg,
+            )
 
             Pkg.activate(".")
         except ImportError:
             raise ImportError(
                 "Install PyJulia, e.g. via `pip install pypesto[julia]`, "
                 "and see the class documentation",
-            )
+            ) from None
         # Include module if not already included
         _read_source(self.module, self.source_file)
 
         petab_jl_problem = self.get(self._petab_problem_name)
         self.petab_jl_problem = petab_jl_problem
 
         # get functions
@@ -137,15 +139,15 @@
         # lazy imports
         try:
             from julia import Main  # noqa: F401
         except ImportError:
             raise ImportError(
                 "Install PyJulia, e.g. via `pip install pypesto[julia]`, "
                 "and see the class documentation",
-            )
+            ) from None
         # setting up a local project, where the precompilation will be done in
         from julia import Pkg
 
         Pkg.activate(".")
         # create a Project f"{self.module}_pre".
         try:
             Pkg.generate(f"{directory}/{self.module}_pre")
@@ -154,15 +156,15 @@
         # Adjust the precompilation file
         write_precompilation_module(
             module=self.module,
             source_file_orig=self.source_file,
         )
         # add a new line at the top of the original module to use the
         # precompiled module
-        with open(self.source_file, "r") as read_f:
+        with open(self.source_file) as read_f:
             if read_f.readline().endswith("_pre\n"):
                 with open("dummy_temp_file.jl", "w+") as write_f:
                     write_f.write(f"using {self.module}_pre\n\n")
                     write_f.write(read_f.read())
                 os.remove(self.source_file)
                 os.rename("dummy_temp_file.jl", self.source_file)
```

### Comparing `pypesto-0.4.2/pypesto/objective/julia/petab_jl_importer.py` & `pypesto-0.5.0/pypesto/objective/julia/petab_jl_importer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Contains the PetabJlImporter class."""
 
 from __future__ import annotations
 
 import logging
 import os.path
-from typing import Iterable, List, Optional, Tuple, Union
+from collections.abc import Iterable
 
 import numpy as np
 
 from pypesto.objective.julia import PEtabJlObjective
 from pypesto.problem import Problem
 
 logger = logging.getLogger(__name__)
@@ -47,20 +47,20 @@
         self._petab_problem_name = petab_problem_name
         # placeholder for the petab.jl problem
         self.petab_jl_problem = None
 
     @staticmethod
     def from_yaml(
         yaml_file: str,
-        ode_solver_options: Optional[dict] = None,
-        gradient_method: Optional[str] = None,
-        hessian_method: Optional[str] = None,
-        sparse_jacobian: Optional[bool] = None,
-        verbose: Optional[bool] = None,
-        directory: Optional[str] = None,
+        ode_solver_options: dict | None = None,
+        gradient_method: str | None = None,
+        hessian_method: str | None = None,
+        sparse_jacobian: bool | None = None,
+        verbose: bool | None = None,
+        directory: str | None = None,
     ) -> PetabJlImporter:
         """
         Create a `PetabJlImporter` from a yaml file.
 
         Writes the Julia module to a file in `directory` and returns a
         `PetabJlImporter` for that module.
 
@@ -96,37 +96,36 @@
 
         return PetabJlImporter(
             module=module,
             source_file=source_file,
         )
 
     def create_objective(
-        self, precompile: Optional[bool] = True
+        self, precompile: bool | None = True
     ) -> PEtabJlObjective:
         """
         Create a `pypesto.objective.PEtabJlObjective` from the PEtab.jl problem.
 
         The objective function will be the negative log likelihood or the
         negative log posterior, depending on the PEtab.jl problem.
 
         Parameters
         ----------
         precompile:
             Whether to precompile the julia module for speed up in
             multistart optimization.
-
         """
         # lazy imports
         try:
             from julia import Main  # noqa: F401
         except ImportError:
             raise ImportError(
                 "Install PyJulia, e.g. via `pip install pypesto[julia]`, "
                 "and see the class documentation",
-            )
+            ) from None
         if self.source_file is None:
             self.source_file = f"{self.module}.jl"
 
         if not os.path.exists(self.source_file):
             raise ValueError(
                 "The julia file does not exist. You can create "
                 "it from a petab yaml file path using "
@@ -141,18 +140,18 @@
         )
 
         self.petab_jl_problem = obj.petab_jl_problem
         return obj
 
     def create_problem(
         self,
-        x_guesses: Optional[Iterable[float]] = None,
-        lb_init: Union[np.ndarray, List[float], None] = None,
-        ub_init: Union[np.ndarray, List[float], None] = None,
-        precompile: Optional[bool] = True,
+        x_guesses: Iterable[float] | None = None,
+        lb_init: np.ndarray | list[float] | None = None,
+        ub_init: np.ndarray | list[float] | None = None,
+        precompile: bool | None = True,
     ) -> Problem:
         """
         Create a `pypesto.Problem` from the PEtab.jl problem.
 
         Parameters
         ----------
         x_guesses:
@@ -178,19 +177,19 @@
             x_names=obj.x_names,
             lb_init=lb_init,
             ub_init=ub_init,
         )
 
 
 def _get_default_options(
-    ode_solver_options: Union[dict, None] = None,
-    gradient_method: Union[str, None] = None,
-    hessian_method: Union[str, None] = None,
-    sparse_jacobian: Union[str, None] = None,
-    verbose: Union[str, None] = None,
+    ode_solver_options: dict | None = None,
+    gradient_method: str | None = None,
+    hessian_method: str | None = None,
+    sparse_jacobian: str | None = None,
+    verbose: str | None = None,
 ) -> dict:
     """
     If values are not specified, get default values for the options.
 
     Additionally check that the values are valid.
 
     Parameters
@@ -260,15 +259,15 @@
         "verbose": verbose,
     }
     return options
 
 
 def _write_julia_file(
     yaml_file: str, options: dict, directory: str
-) -> Tuple[str, str]:
+) -> tuple[str, str]:
     """
     Write the Julia file.
 
     Parameters
     ----------
     yaml_file:
         The yaml file of the PEtab problem.
```

### Comparing `pypesto-0.4.2/pypesto/objective/pre_post_process.py` & `pypesto-0.5.0/pypesto/objective/pre_post_process.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Sequence
+from collections.abc import Sequence
 
 import numpy as np
 
 from ..C import GRAD, HESS, RES, SRES
 
 
 class PrePostProcessor:
@@ -32,15 +32,15 @@
         Returns
         -------
         x:
             Parameter vector for simulation.
         """
         return x
 
-    def postprocess(self, result: Dict) -> Dict:  # pylint: disable=R0201
+    def postprocess(self, result: dict) -> dict:  # pylint: disable=R0201
         """
         Convert all arrays into np.ndarrays if necessary, and return them.
 
         Parameters
         ----------
         result:
             The result object to finalize.
@@ -61,15 +61,15 @@
         -------
         x:
             Parameter vector for optimization.
         """
         return x
 
     @staticmethod
-    def as_ndarrays(result: Dict) -> Dict:
+    def as_ndarrays(result: dict) -> dict:
         """
         Convert all array_like objects to np.ndarrays.
 
         This has the advantage of a uniform output datatype which offers
         various methods to assess the data.
         """
         keys = [GRAD, HESS, RES, SRES]
@@ -124,15 +124,15 @@
         x = super().reduce(x)
 
         if x.size:
             return x[self.x_free_indices]
         else:
             return x
 
-    def postprocess(self, result: Dict) -> Dict:
+    def postprocess(self, result: dict) -> dict:
         """Constrain results to optimization parameter dimensions."""
         result = super().postprocess(result)
 
         if result.get(GRAD, None) is not None:
             grad = result[GRAD]
             if grad.size == self.dim_full:
                 grad = grad[self.x_free_indices]
```

### Comparing `pypesto-0.4.2/pypesto/objective/priors.py` & `pypesto-0.5.0/pypesto/objective/priors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import math
+from collections.abc import Sequence
 from copy import deepcopy
-from typing import Callable, Dict, List, Sequence, Tuple, Union
+from typing import Callable, Union
 
 import numpy as np
 
 from .. import C
 from .aggregated import AggregatedObjective
 from .base import ResultDict
 from .function import ObjectiveBase
@@ -46,15 +47,15 @@
     log-densities and their corresponding derivatives.
     Internally, values are multiplied by -1, since pyPESTO expects the
     Objective function to be of a negative log-density type.
     """
 
     def __init__(
         self,
-        prior_list: List[Dict],
+        prior_list: list[dict],
         x_names: Sequence[str] = None,
     ):
         """
         Initialize.
 
         Parameters
         ----------
@@ -71,15 +72,15 @@
         """Create deepcopy of object."""
         other = NegLogParameterPriors(deepcopy(self.prior_list))
         return other
 
     def call_unprocessed(
         self,
         x: np.ndarray,
-        sensi_orders: Tuple[int, ...],
+        sensi_orders: tuple[int, ...],
         mode: C.ModeType,
         **kwargs,
     ) -> ResultDict:
         """
         Call objective function without pre- or post-processing and formatting.
 
         Returns
@@ -96,130 +97,130 @@
                 if order == 0:
                     continue
                 elif order == 1:
                     res[C.GRAD] = self.gradient_neg_log_density(x)
                 elif order == 2:
                     res[C.HESS] = self.hessian_neg_log_density(x)
                 else:
-                    raise ValueError(f'Invalid sensi order {order}.')
+                    raise ValueError(f"Invalid sensi order {order}.")
 
         if mode == C.MODE_RES:
             for order in sensi_orders:
                 if order == 0:
                     res[C.RES] = self.residual(x)
                 elif order == 1:
                     res[C.SRES] = self.residual_jacobian(x)
                 else:
-                    raise ValueError(f'Invalid sensi order {order}.')
+                    raise ValueError(f"Invalid sensi order {order}.")
 
         return res
 
     def check_sensi_orders(
         self,
-        sensi_orders: Tuple[int, ...],
+        sensi_orders: tuple[int, ...],
         mode: C.ModeType,
     ) -> bool:
         """See `ObjectiveBase` documentation."""
         if mode == C.MODE_FUN:
             for order in sensi_orders:
                 if not (0 <= order <= 2):
                     return False
         elif mode == C.MODE_RES:
             for order in sensi_orders:
                 if order == 0:
                     return all(
-                        prior.get('residual', None) is not None
+                        prior.get("residual", None) is not None
                         for prior in self.prior_list
                     )
                 elif order == 1:
                     return all(
-                        prior.get('residual_dx', None) is not None
+                        prior.get("residual_dx", None) is not None
                         for prior in self.prior_list
                     )
                 else:
                     return False
         else:
             raise ValueError(
-                f'Invalid input: Expected mode {C.MODE_FUN} or '
-                f'{C.MODE_RES}, received {mode} instead.'
+                f"Invalid input: Expected mode {C.MODE_FUN} or "
+                f"{C.MODE_RES}, received {mode} instead."
             )
 
         return True
 
     def check_mode(self, mode: C.ModeType) -> bool:
         """See `ObjectiveBase` documentation."""
         if mode == C.MODE_FUN:
             return True
         elif mode == C.MODE_RES:
             return all(
-                prior.get('residual', None) is not None
+                prior.get("residual", None) is not None
                 for prior in self.prior_list
             )
         else:
             raise ValueError(
-                f'Invalid input: Expected mode {C.MODE_FUN} or '
-                f'{C.MODE_RES}, received {mode} instead.'
+                f"Invalid input: Expected mode {C.MODE_FUN} or "
+                f"{C.MODE_RES}, received {mode} instead."
             )
 
     def neg_log_density(self, x):
         """Evaluate the negative log-density at x."""
         density_val = 0
         for prior in self.prior_list:
-            density_val -= prior['density_fun'](x[prior['index']])
+            density_val -= prior["density_fun"](x[prior["index"]])
 
         return density_val
 
     def gradient_neg_log_density(self, x):
         """Evaluate the gradient of the negative log-density at x."""
         grad = np.zeros_like(x)
 
         for prior in self.prior_list:
-            grad[prior['index']] -= prior['density_dx'](x[prior['index']])
+            grad[prior["index"]] -= prior["density_dx"](x[prior["index"]])
 
         return grad
 
     def hessian_neg_log_density(self, x):
         """Evaluate the hessian of the negative log-density at x."""
         hessian = np.zeros((len(x), len(x)))
 
         for prior in self.prior_list:
-            hessian[prior['index'], prior['index']] -= prior['density_ddx'](
-                x[prior['index']]
+            hessian[prior["index"], prior["index"]] -= prior["density_ddx"](
+                x[prior["index"]]
             )
 
         return hessian
 
     def hessian_vp_neg_log_density(self, x, p):
         """Compute vector product of the hessian at x with a vector p."""
         h_dot_p = np.zeros_like(p)
 
         for prior in self.prior_list:
-            h_dot_p[prior['index']] -= (
-                prior['density_ddx'](x[prior['index']]) * p[prior['index']]
+            h_dot_p[prior["index"]] -= (
+                prior["density_ddx"](x[prior["index"]]) * p[prior["index"]]
             )
 
         return h_dot_p
 
     def residual(self, x):
         """Evaluate the residual representation of the prior at x."""
         return np.asarray(
-            [prior['residual'](x[prior['index']]) for prior in self.prior_list]
+            [prior["residual"](x[prior["index"]]) for prior in self.prior_list]
         )
 
     def residual_jacobian(self, x):
         """
         Evaluate residual Jacobian.
 
         Evaluate the Jacobian of the residual representation of the prior
         for a parameter vector x w.r.t. x, if available.
         """
         sres = np.zeros((len(self.prior_list), len(x)))
         for iprior, prior in enumerate(self.prior_list):
-            sres[iprior, prior['index']] = prior['residual_dx'](
-                x[prior['index']]
+            sres[iprior, prior["index"]] = prior["residual_dx"](
+                x[prior["index"]]
             )
 
         return sres
 
 
 def get_parameter_prior_dict(
     index: int,
@@ -245,22 +246,22 @@
         log-transformed, while the prior is always defined in the linear
         space, unless it starts with "parameterScale")
     """
     log_f, d_log_f_dx, dd_log_f_ddx, res, d_res_dx = _prior_densities(
         prior_type, prior_parameters
     )
 
-    if parameter_scale == C.LIN or prior_type.startswith('parameterScale'):
+    if parameter_scale == C.LIN or prior_type.startswith("parameterScale"):
         return {
-            'index': index,
-            'density_fun': log_f,
-            'density_dx': d_log_f_dx,
-            'density_ddx': dd_log_f_ddx,
-            'residual': res,
-            'residual_dx': d_res_dx,
+            "index": index,
+            "density_fun": log_f,
+            "density_dx": d_log_f_dx,
+            "density_ddx": dd_log_f_ddx,
+            "residual": res,
+            "residual_dx": d_res_dx,
         }
 
     elif parameter_scale == C.LOG:
 
         def log_f_log(x_log):
             """Log-prior for log-parameters."""
             return log_f(np.exp(x_log))
@@ -291,20 +292,20 @@
                 """Residual-prior for log-parameters."""
                 return d_res_dx(np.exp(x_log)) * np.exp(x_log)
 
         else:
             d_res_log = None
 
         return {
-            'index': index,
-            'density_fun': log_f_log,
-            'density_dx': d_log_f_log,
-            'density_ddx': dd_log_f_log,
-            'residual': res_log,
-            'residual_dx': d_res_log,
+            "index": index,
+            "density_fun": log_f_log,
+            "density_dx": d_log_f_log,
+            "density_ddx": dd_log_f_log,
+            "residual": res_log,
+            "residual_dx": d_res_log,
         }
 
     elif parameter_scale == C.LOG10:
         log10 = np.log(10)
 
         def log_f_log10(x_log10):
             """Log-prior for log10-parameters."""
@@ -336,20 +337,20 @@
         if d_res_dx is not None:
 
             def d_res_log(x_log10):
                 """Residual-prior for log10-parameters."""
                 return d_res_dx(10**x_log10) * log10 * 10**x_log10
 
         return {
-            'index': index,
-            'density_fun': log_f_log10,
-            'density_dx': d_log_f_log10,
-            'density_ddx': dd_log_f_log10,
-            'residual': res_log,
-            'residual_dx': d_res_log,
+            "index": index,
+            "density_fun": log_f_log10,
+            "density_dx": d_log_f_log10,
+            "density_ddx": dd_log_f_log10,
+            "residual": res_log,
+            "residual_dx": d_res_log,
         }
 
     else:
         raise ValueError(
             "NegLogPriors in parameters in scale "
             f"{parameter_scale} are currently not supported."
         )
@@ -517,26 +518,24 @@
                 2 * sigma**2
             )
 
         def d_log_f_dx(x):
             return -1 / x - (np.log(x) - mean) / (sigma**2 * x)
 
         def dd_log_f_ddx(x):
-            return 1 / (x**2) - (1 - np.log(x) + mean) / (
-                sigma**2 * x**2
-            )
+            return 1 / (x**2) - (1 - np.log(x) + mean) / (sigma**2 * x**2)
 
         return log_f, d_log_f_dx, dd_log_f_ddx, None, None
 
     elif prior_type == C.LOG_LAPLACE:
         # when implementing: add to tests
         raise NotImplementedError
     else:
         raise ValueError(
-            f'NegLogPriors of type {prior_type} are currently ' 'not supported'
+            f"NegLogPriors of type {prior_type} are currently " "not supported"
         )
 
 
 def _get_linear_function(
     slope: float,
     intercept: float = 0.0,
 ):
```

### Comparing `pypesto-0.4.2/pypesto/optimize/__init__.py` & `pypesto-0.5.0/pypesto/optimize/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,28 @@
 Optimize
 ========
 
 Multistart optimization with support for various optimizers.
 """
 
 from .ess import (
-    CESSOptimizer,
     ESSOptimizer,
     SacessFidesFactory,
     SacessOptimizer,
     get_default_ess_options,
 )
 from .load import (
     fill_result_from_history,
     optimization_result_from_history,
     read_result_from_file,
     read_results_from_file,
 )
 from .optimize import minimize
 from .optimizer import (
-    CmaesOptimizer,
+    CmaOptimizer,
     DlibOptimizer,
     FidesOptimizer,
     IpoptOptimizer,
     NLoptOptimizer,
     Optimizer,
     PyswarmOptimizer,
     PyswarmsOptimizer,
```

### Comparing `pypesto-0.4.2/pypesto/optimize/ess/ess.py` & `pypesto-0.5.0/pypesto/optimize/ess/ess.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from pypesto.startpoint import StartpointMethod
 
 from .function_evaluator import FunctionEvaluator, create_function_evaluator
 from .refset import RefSet
 
 logger = logging.getLogger(__name__)
 
-__all__ = ['ESSOptimizer', 'ESSExitFlag']
+__all__ = ["ESSOptimizer", "ESSExitFlag"]
 
 
 class ESSExitFlag(int, enum.Enum):
     """Exit flags used by :class:`ESSOptimizer`."""
 
     # ESS did not run/finish yet
     DID_NOT_RUN = 0
@@ -163,19 +163,20 @@
         """(Re-)Initialize."""
         # RefSet
         self.refset: Optional[RefSet] = None
         # Overall best parameters found so far
         self.x_best: Optional[np.array] = None
         # Overall best function value found so far
         self.fx_best: float = np.inf
-        # Results from local searches
+        # Results from local searches (only those with finite fval)
         self.local_solutions: list[OptimizerResult] = []
         # Index of current iteration
         self.n_iter: int = 0
         # ESS iteration at which the last local search took place
+        # (only local searches with a finite result are counted)
         self.last_local_search_niter: int = 0
         # Whether self.x_best has changed in the current iteration
         self.x_best_has_changed: bool = False
         self.exit_flag: ESSExitFlag = ESSExitFlag.DID_NOT_RUN
         self.evaluator: Optional[FunctionEvaluator] = None
         self.starttime: Optional[float] = None
         self.history: MemoryHistory = MemoryHistory()
@@ -188,16 +189,18 @@
     ):
         """Initialize for optimizations.
 
         Create initial refset, start timer, ... .
         """
         if startpoint_method is not None:
             warn(
-                "Passing `startpoint_method` directly is deprecated, use `problem.startpoint_method` instead.",
+                "Passing `startpoint_method` directly is deprecated, "
+                "use `problem.startpoint_method` instead.",
                 DeprecationWarning,
+                stacklevel=1,
             )
 
         self._initialize()
         self.starttime = time.time()
 
         if (refset is None and problem is None) or (
             refset is not None and problem is not None
@@ -297,20 +300,20 @@
 
     def _create_result(self) -> pypesto.Result:
         """Create the result object.
 
         Currently, this returns the overall best value and the final RefSet.
         """
         common_result_fields = {
-            'exitflag': self.exit_flag,
+            "exitflag": self.exit_flag,
             # meaningful? this is the overall time, and identical for all
             #  reported points
-            'time': time.time() - self.starttime,
-            'n_fval': self.evaluator.n_eval,
-            'optimizer': str(self),
+            "time": time.time() - self.starttime,
+            "n_fval": self.evaluator.n_eval,
+            "optimizer": str(self),
         }
         i_result = 0
         result = pypesto.Result(problem=self.evaluator.problem)
 
         # save global best
         optimizer_result = pypesto.OptimizerResult(
             id=str(i_result),
@@ -463,22 +466,22 @@
 
         See [PenasGon2017]_ Algorithm 2.
         """
         if self.local_only_best_sol and self.x_best_has_changed:
             self.logger.debug("Local search only from best point.")
             local_search_x0_fx0_candidates = ((self.x_best, self.fx_best),)
         # first local search?
-        elif not self.local_solutions and self.n_iter >= self.local_n1:
+        elif self.n_iter == self.local_n1:
             self.logger.debug(
                 "First local search from best point due to "
                 f"local_n1={self.local_n1}."
             )
             local_search_x0_fx0_candidates = ((self.x_best, self.fx_best),)
         elif (
-            self.local_solutions
+            self.n_iter >= self.local_n1
             and self.n_iter - self.last_local_search_niter >= self.local_n2
         ):
             quality_order = np.argsort(fx_best_children)
             # compute minimal distance between the best children and all local
             #  optima found so far
             min_distances = np.array(
                 np.min(
@@ -537,14 +540,19 @@
                 self.local_solutions.append(optimizer_result)
 
                 self._maybe_update_global_best(
                     optimizer_result.x[optimizer_result.free_indices],
                     optimizer_result.fval,
                 )
                 break
+        else:
+            self.logger.debug(
+                "Local search: No finite value found in any local search."
+            )
+            return
 
         self.last_local_search_niter = self.n_iter
         self.evaluator.reset_round_counter()
 
     def _maybe_update_global_best(self, x, fx):
         """Update the global best value if the provided value is better."""
         if fx < self.fx_best:
@@ -612,15 +620,15 @@
             )
             if not self._keep_going():
                 break
 
     def _report_iteration(self):
         """Log the current iteration."""
         if self.n_iter == 0:
-            self.logger.info("iter | best | nf | refset         |")
+            self.logger.info("iter | best | nf | refset         | nlocal")
 
         with np.printoptions(
             edgeitems=5,
             threshold=8,
             linewidth=100000,
             formatter={"float": lambda x: "%.3g" % x},
         ):
```

### Comparing `pypesto-0.4.2/pypesto/optimize/ess/function_evaluator.py` & `pypesto-0.5.0/pypesto/optimize/ess/function_evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Helper for objective evaluation during scatter search."""
 
 import multiprocessing
 import threading
+from collections.abc import Sequence
 from concurrent.futures import ThreadPoolExecutor
 from copy import deepcopy
-from typing import Optional, Sequence, Tuple
+from typing import Optional
 from warnings import warn
 
 import numpy as np
 
 from pypesto import Problem
 from pypesto.startpoint import StartpointMethod
 
@@ -42,16 +43,18 @@
             The problem
         startpoint_method:
             Method for choosing feasible parameters
             **Deprecated. Use ``problem.startpoint_method`` instead.**
         """
         if startpoint_method is not None:
             warn(
-                "Passing `startpoint_method` directly is deprecated, use `problem.startpoint_method` instead.",
+                "Passing `startpoint_method` directly is deprecated, "
+                "use `problem.startpoint_method` instead.",
                 DeprecationWarning,
+                stacklevel=1,
             )
 
         self.problem: Problem = problem
         self.startpoint_method: StartpointMethod = (
             startpoint_method or problem.startpoint_method
         )
         self.n_eval: int = 0
@@ -81,15 +84,15 @@
         The objective function values in the same order as the inputs.
         """
         res = np.fromiter(map(self.single, xs), dtype=float)
         self.n_eval += len(xs)
         self.n_eval_round += len(xs)
         return res
 
-    def single_random(self) -> Tuple[np.array, float]:
+    def single_random(self) -> tuple[np.array, float]:
         """Evaluate objective at a random point.
 
         The point is generated by the given``startpoint_method``. A new point
         will be generated until a finite objective value is obtained.
 
         Returns
         -------
@@ -98,15 +101,15 @@
         """
         x = fx = np.nan
         while not np.isfinite(fx):
             x = self.startpoint_method(n_starts=1, problem=self.problem)[0]
             fx = self.single(x)
         return x, fx
 
-    def multiple_random(self, n: int) -> Tuple[np.array, np.array]:
+    def multiple_random(self, n: int) -> tuple[np.array, np.array]:
         """Evaluate objective at ``n`` random points.
 
         The points are generated by the given``startpoint_method``. New points
         will be generated until only finite objective values are obtained.
 
         Returns
         -------
@@ -164,15 +167,15 @@
 
         self._init_threading()
 
     def __getstate__(self):
         return {
             k: v
             for k, v in vars(self).items()
-            if k not in {'_thread_local', '_executor'}
+            if k not in {"_thread_local", "_executor"}
         }
 
     def __setstate__(self, state):
         vars(self).update(state)
         self._init_threading()
 
     def _init_threading(self):
```

### Comparing `pypesto-0.4.2/pypesto/optimize/ess/refset.py` & `pypesto-0.5.0/pypesto/optimize/ess/refset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ReferenceSet functionality for scatter search."""
 
-from typing import Any, Dict, Optional
+from typing import Any, Optional
 
 import numpy as np
 
 from .function_evaluator import FunctionEvaluator
 
 
 class RefSet:
@@ -61,15 +61,15 @@
         if x is None:
             self.x = self.fx = None
         else:
             self.x = x
             self.fx = fx
 
         self.n_stuck = np.zeros(shape=[dim])
-        self.attributes: Dict[Any, np.array] = {}
+        self.attributes: dict[Any, np.array] = {}
 
     def sort(self):
         """Sort RefSet by quality."""
         order = np.argsort(self.fx)
         self.fx = self.fx[order]
         self.x = self.x[order]
         self.n_stuck = self.n_stuck[order]
@@ -132,15 +132,15 @@
         Assumes RefSet is sorted.
         """
         x = self.x
         for i in range(self.dim):
             for j in range(i + 1, self.dim):
                 # check proximity
                 # zero-division may occur here
-                with np.errstate(divide='ignore', invalid='ignore'):
+                with np.errstate(divide="ignore", invalid="ignore"):
                     while (
                         np.max(np.abs((x[i] - x[j]) / x[j]))
                         <= self.proximity_threshold
                     ):
                         # too close. replace x_j.
                         x[j], self.fx[j] = self.evaluator.single_random()
                         self.sort()
```

### Comparing `pypesto-0.4.2/pypesto/optimize/ess/sacess.py` & `pypesto-0.5.0/pypesto/optimize/ess/sacess.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import itertools
 import logging
 import logging.handlers
 import multiprocessing
 import os
 import time
 from math import ceil, sqrt
-from multiprocessing import Manager, Process
+from multiprocessing import get_context
 from multiprocessing.managers import SyncManager
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+from typing import Any, Callable, Optional, Union
 from uuid import uuid1
 from warnings import warn
 
 import numpy as np
 
 import pypesto
 
@@ -58,19 +58,20 @@
         See :func:`pypesto.visualize.optimizer_history.sacess_history` for
         visualization.
     """
 
     def __init__(
         self,
         num_workers: Optional[int] = None,
-        ess_init_args: Optional[List[Dict[str, Any]]] = None,
+        ess_init_args: Optional[list[dict[str, Any]]] = None,
         max_walltime_s: float = np.inf,
         sacess_loglevel: int = logging.INFO,
         ess_loglevel: int = logging.WARNING,
         tmpdir: Union[Path, str] = None,
+        mp_start_method: str = "spawn",
     ):
         """Construct.
 
         Parameters
         ----------
         ess_init_args:
             List of argument dictionaries passed to
@@ -101,14 +102,17 @@
         sacess_loglevel:
             Loglevel for SACESS runs.
         tmpdir:
             Directory for temporary files. This defaults to a directory in the
             current working directory named ``SacessOptimizerTemp-{random suffix}``.
             When setting this option, make sure any optimizers running in
             parallel have a unique `tmpdir`.
+        mp_start_method:
+            The start method for the multiprocessing context.
+            See :mod:`multiprocessing` for details.
         """
         if (num_workers is None and ess_init_args is None) or (
             num_workers is not None and ess_init_args is not None
         ):
             raise ValueError(
                 "Exactly one of `num_workers` or `ess_init_args` "
                 "has to be provided."
@@ -131,14 +135,15 @@
             while self._tmpdir is None or self._tmpdir.exists():
                 self._tmpdir = Path(f"SacessOptimizerTemp-{str(uuid1())[:8]}")
         self._tmpdir = Path(self._tmpdir).absolute()
         self._tmpdir.mkdir(parents=True, exist_ok=True)
         self.histories: Optional[
             list["pypesto.history.memory.MemoryHistory"]
         ] = None
+        self.mp_ctx = get_context(mp_start_method)
 
     def minimize(
         self,
         problem: Problem,
         startpoint_method: StartpointMethod = None,
     ) -> pypesto.Result:
         """Solve the given optimization problem.
@@ -169,40 +174,42 @@
         :attr:`pypesto.Result.optimize_result`.
         Results are sorted by objective. At least the best parameters are
         included. Additional results may be included - this is subject to
         change.
         """
         if startpoint_method is not None:
             warn(
-                "Passing `startpoint_method` directly is deprecated, use `problem.startpoint_method` instead.",
+                "Passing `startpoint_method` directly is deprecated, "
+                "use `problem.startpoint_method` instead.",
                 DeprecationWarning,
+                stacklevel=1,
             )
 
         start_time = time.time()
         logger.debug(
             f"Running {self.__class__.__name__} with {self.num_workers} "
             f"workers: {self.ess_init_args}"
         )
         ess_init_args = self.ess_init_args or get_default_ess_options(
             num_workers=self.num_workers, dim=problem.dim
         )
 
         logging_handler = logging.StreamHandler()
         logging_handler.setFormatter(
             logging.Formatter(
-                '%(asctime)s %(name)s %(levelname)-8s %(message)s'
+                "%(asctime)s %(name)s %(levelname)-8s %(message)s"
             )
         )
         logging_thread = logging.handlers.QueueListener(
-            multiprocessing.Queue(-1), logging_handler
+            self.mp_ctx.Queue(-1), logging_handler
         )
 
         # shared memory manager to handle shared state
         # (simulates the sacess manager process)
-        with Manager() as shmem_manager:
+        with self.mp_ctx.Manager() as shmem_manager:
             sacess_manager = SacessManager(
                 shmem_manager=shmem_manager,
                 ess_options=ess_init_args,
                 dim=problem.dim,
             )
             # create workers
             workers = [
@@ -217,15 +224,15 @@
                         worker_idx, self._tmpdir
                     ),
                 )
                 for worker_idx, ess_kwargs in enumerate(ess_init_args)
             ]
             # launch worker processes
             worker_processes = [
-                Process(
+                self.mp_ctx.Process(
                     name=f"{self.__class__.__name__}-worker-{i:02d}",
                     target=_run_worker,
                     args=(
                         worker,
                         problem,
                         startpoint_method,
                         logging_thread.queue,
@@ -334,15 +341,15 @@
     _lock: Lock for accessing shared state.
     _logger: A logger instance
     """
 
     def __init__(
         self,
         shmem_manager: SyncManager,
-        ess_options: List[Dict[str, Any]],
+        ess_options: list[dict[str, Any]],
         dim: int,
     ):
         self._num_workers = len(ess_options)
         self._ess_options = [shmem_manager.dict(o) for o in ess_options]
         self._best_known_fx = shmem_manager.Value("d", np.inf)
         self._best_known_x = shmem_manager.Array("d", [np.nan] * dim)
         self._rejections = shmem_manager.Value("i", 0)
@@ -354,20 +361,20 @@
             "d", range(self._num_workers)
         )
         self._worker_comms = shmem_manager.Array("i", [0] * self._num_workers)
         self._lock = shmem_manager.RLock()
         self._logger = logging.getLogger()
         self._result_queue = shmem_manager.Queue()
 
-    def get_best_solution(self) -> Tuple[np.array, float]:
+    def get_best_solution(self) -> tuple[np.array, float]:
         """Get the best objective value and corresponding parameters."""
         with self._lock:
             return np.array(self._best_known_x), self._best_known_fx.value
 
-    def reconfigure_worker(self, worker_idx: int) -> Dict:
+    def reconfigure_worker(self, worker_idx: int) -> dict:
         """Reconfigure the given worker.
 
         Updates the ESS options for the given worker to those of the worker at
         the top of the scoreboard and returns those settings.
         """
         with self._lock:
             leader_options = self._ess_options[
@@ -484,15 +491,15 @@
     _ess_loglevel: Logging level for ESS runs
     _tmp_result_file: Path of a temporary file to be created.
     """
 
     def __init__(
         self,
         manager: SacessManager,
-        ess_kwargs: Dict[str, Any],
+        ess_kwargs: dict[str, Any],
         worker_idx: int,
         max_walltime_s: float = np.inf,
         loglevel: int = logging.INFO,
         ess_loglevel: int = logging.WARNING,
         tmp_result_file: str = None,
     ):
         self._manager = manager
@@ -525,25 +532,25 @@
         self._logger.debug(
             f"#{self._worker_idx} starting " f"({self._ess_kwargs})."
         )
 
         evaluator = create_function_evaluator(
             problem,
             startpoint_method,
-            n_procs=self._ess_kwargs.get('n_procs'),
-            n_threads=self._ess_kwargs.get('n_threads'),
+            n_procs=self._ess_kwargs.get("n_procs"),
+            n_threads=self._ess_kwargs.get("n_threads"),
         )
 
         # create initial refset
         self._refset = RefSet(
-            dim=self._ess_kwargs['dim_refset'], evaluator=evaluator
+            dim=self._ess_kwargs["dim_refset"], evaluator=evaluator
         )
         self._refset.initialize_random(
             n_diverse=max(
-                self._ess_kwargs.get('n_diverse', 10 * problem.dim),
+                self._ess_kwargs.get("n_diverse", 10 * problem.dim),
                 self._refset.dim,
             )
         )
 
         ess = self._setup_ess(startpoint_method)
 
         # run ESS until exit criteria are met, but start at least one iteration
@@ -577,16 +584,16 @@
         self._manager._result_queue.put(ess.history)
         ess._report_final()
 
     def _setup_ess(self, startpoint_method: StartpointMethod) -> ESSOptimizer:
         """Run ESS."""
         ess_kwargs = self._ess_kwargs.copy()
         # account for sacess walltime limit
-        ess_kwargs['max_walltime_s'] = min(
-            ess_kwargs.get('max_walltime_s', np.inf),
+        ess_kwargs["max_walltime_s"] = min(
+            ess_kwargs.get("max_walltime_s", np.inf),
             self._max_walltime_s - (time.time() - self._start_time),
         )
 
         ess = ESSOptimizer(**ess_kwargs)
         ess.logger = self._logger.getChild(
             f"sacess-{self._worker_idx:02d}-ess"
         )
@@ -631,15 +638,15 @@
         if (
             self._n_received_solutions > 10 * self._n_sent_solutions + 20
             and self._neval > problem.dim * 5000
         ):
             self._ess_kwargs = self._manager.reconfigure_worker(
                 self._worker_idx
             )
-            self._refset.resize(self._ess_kwargs['dim_refset'])
+            self._refset.resize(self._ess_kwargs["dim_refset"])
             self._logger.debug(
                 f"Updated settings on worker {self._worker_idx} to "
                 f"{self._ess_kwargs}"
             )
 
     def maybe_update_best(self, x: np.array, fx: float):
         """Maybe update the best known solution and send it to the manager."""
@@ -752,15 +759,15 @@
     num_workers: int,
     dim: int,
     local_optimizer: Union[
         bool,
         "pypesto.optimize.Optimizer",
         Callable[..., "pypesto.optimize.Optimizer"],
     ] = True,
-) -> List[Dict]:
+) -> list[dict]:
     """Get default ESS settings for (SA)CESS.
 
     Returns settings for ``num_workers`` parallel scatter searches, combining
     more aggressive and more conservative configurations. Mainly intended for
     use with :class:`SacessOptimizer`. For details on the different options,
     see keyword arguments of :meth:`ESSOptimizer.__init__`.
 
@@ -785,169 +792,169 @@
 
     def dim_refset(x):
         return max(min_dimrefset, ceil((1 + sqrt(4 * dim * x)) / 2))
 
     settings = [
         # settings for first worker
         {
-            'dim_refset': dim_refset(10),
-            'balance': 0.5,
-            'local_n2': 10,
+            "dim_refset": dim_refset(10),
+            "balance": 0.5,
+            "local_n2": 10,
         },
         # for the remaining workers, cycle through these settings
         # 1
         {
-            'dim_refset': dim_refset(1),
-            'balance': 0.0,
-            'local_n1': 1,
-            'local_n2': 1,
+            "dim_refset": dim_refset(1),
+            "balance": 0.0,
+            "local_n1": 1,
+            "local_n2": 1,
         },
         # 2
         {
-            'dim_refset': dim_refset(3),
-            'balance': 0.0,
-            'local_n1': 1000,
-            'local_n2': 1000,
+            "dim_refset": dim_refset(3),
+            "balance": 0.0,
+            "local_n1": 1000,
+            "local_n2": 1000,
         },
         # 3
         {
-            'dim_refset': dim_refset(5),
-            'balance': 0.25,
-            'local_n1': 10,
-            'local_n2': 10,
+            "dim_refset": dim_refset(5),
+            "balance": 0.25,
+            "local_n1": 10,
+            "local_n2": 10,
         },
         # 4
         {
-            'dim_refset': dim_refset(10),
-            'balance': 0.5,
-            'local_n1': 20,
-            'local_n2': 20,
+            "dim_refset": dim_refset(10),
+            "balance": 0.5,
+            "local_n1": 20,
+            "local_n2": 20,
         },
         # 5
         {
-            'dim_refset': dim_refset(15),
-            'balance': 0.25,
-            'local_n1': 100,
-            'local_n2': 100,
+            "dim_refset": dim_refset(15),
+            "balance": 0.25,
+            "local_n1": 100,
+            "local_n2": 100,
         },
         # 6
         {
-            'dim_refset': dim_refset(12),
-            'balance': 0.25,
-            'local_n1': 1000,
-            'local_n2': 1000,
+            "dim_refset": dim_refset(12),
+            "balance": 0.25,
+            "local_n1": 1000,
+            "local_n2": 1000,
         },
         # 7
         {
-            'dim_refset': dim_refset(7.5),
-            'balance': 0.25,
-            'local_n1': 15,
-            'local_n2': 15,
+            "dim_refset": dim_refset(7.5),
+            "balance": 0.25,
+            "local_n1": 15,
+            "local_n2": 15,
         },
         # 8
         {
-            'dim_refset': dim_refset(5),
-            'balance': 0.25,
-            'local_n1': 7,
-            'local_n2': 7,
+            "dim_refset": dim_refset(5),
+            "balance": 0.25,
+            "local_n1": 7,
+            "local_n2": 7,
         },
         # 9
         {
-            'dim_refset': dim_refset(2),
-            'balance': 0.0,
-            'local_n1': 1000,
-            'local_n2': 1000,
+            "dim_refset": dim_refset(2),
+            "balance": 0.0,
+            "local_n1": 1000,
+            "local_n2": 1000,
         },
         # 10
         {
-            'dim_refset': dim_refset(0.5),
-            'balance': 0.0,
-            'local_n1': 1,
-            'local_n2': 1,
+            "dim_refset": dim_refset(0.5),
+            "balance": 0.0,
+            "local_n1": 1,
+            "local_n2": 1,
         },
         # 11
         {
-            'dim_refset': dim_refset(1.5),
-            'balance': 1.0,
-            'local_n1': 1,
-            'local_n2': 1,
+            "dim_refset": dim_refset(1.5),
+            "balance": 1.0,
+            "local_n1": 1,
+            "local_n2": 1,
         },
         # 12
         {
-            'dim_refset': dim_refset(3.5),
-            'balance': 1.0,
-            'local_n1': 4,
-            'local_n2': 4,
+            "dim_refset": dim_refset(3.5),
+            "balance": 1.0,
+            "local_n1": 4,
+            "local_n2": 4,
         },
         # 13
         {
-            'dim_refset': dim_refset(5.5),
-            'balance': 0.1,
-            'local_n1': 10,
-            'local_n2': 10,
+            "dim_refset": dim_refset(5.5),
+            "balance": 0.1,
+            "local_n1": 10,
+            "local_n2": 10,
         },
         # 14
         {
-            'dim_refset': dim_refset(10.5),
-            'balance': 0.3,
-            'local_n1': 20,
-            'local_n2': 20,
+            "dim_refset": dim_refset(10.5),
+            "balance": 0.3,
+            "local_n1": 20,
+            "local_n2": 20,
         },
         # 15
         {
-            'dim_refset': dim_refset(15.5),
-            'balance': 0.2,
-            'local_n1': 1000,
-            'local_n2': 1000,
+            "dim_refset": dim_refset(15.5),
+            "balance": 0.2,
+            "local_n1": 1000,
+            "local_n2": 1000,
         },
         # 16
         {
-            'dim_refset': dim_refset(12.5),
-            'balance': 0.2,
-            'local_n1': 10,
-            'local_n2': 10,
+            "dim_refset": dim_refset(12.5),
+            "balance": 0.2,
+            "local_n1": 10,
+            "local_n2": 10,
         },
         # 17
         {
-            'dim_refset': dim_refset(8),
-            'balance': 0.75,
-            'local_n1': 15,
-            'local_n2': 15,
+            "dim_refset": dim_refset(8),
+            "balance": 0.75,
+            "local_n1": 15,
+            "local_n2": 15,
         },
         # 18
         {
-            'dim_refset': dim_refset(5.5),
-            'balance': 0.75,
-            'local_n1': 1000,
-            'local_n2': 1000,
+            "dim_refset": dim_refset(5.5),
+            "balance": 0.75,
+            "local_n1": 1000,
+            "local_n2": 1000,
         },
         # 19
         {
-            'dim_refset': dim_refset(2.2),
-            'balance': 1.0,
-            'local_n1': 2,
-            'local_n2': 2,
+            "dim_refset": dim_refset(2.2),
+            "balance": 1.0,
+            "local_n1": 2,
+            "local_n2": 2,
         },
         # 20
         {
-            'dim_refset': dim_refset(1),
-            'balance': 1.0,
-            'local_n1': 1,
-            'local_n2': 1,
+            "dim_refset": dim_refset(1),
+            "balance": 1.0,
+            "local_n1": 1,
+            "local_n2": 1,
         },
     ]
 
     # Set local optimizer
     for cur_settings in settings:
         if local_optimizer is True:
-            cur_settings['local_optimizer'] = SacessFidesFactory(
+            cur_settings["local_optimizer"] = SacessFidesFactory(
                 fides_kwargs={"verbose": logging.WARNING}
             )
         elif local_optimizer is not False:
-            cur_settings['local_optimizer'] = local_optimizer
+            cur_settings["local_optimizer"] = local_optimizer
 
     return [
         settings[0],
         *(itertools.islice(itertools.cycle(settings[1:]), num_workers - 1)),
     ]
 
 
@@ -963,15 +970,14 @@
     ----------
     fides_options:
         Options for the :class:`FidesOptimizer`.
         See :class:`fides.constants.Options`.
     fides_kwargs:
         Keyword arguments for the :class:`FidesOptimizer`. See
         :meth:`FidesOptimizer.__init__`. Must not include ``options``.
-
     """
 
     def __init__(
         self,
         fides_options: Optional[dict[str, Any]] = None,
         fides_kwargs: Optional[dict[str, Any]] = None,
     ):
@@ -985,15 +991,15 @@
 
         # Check if fides is installed
         try:
             import fides  # noqa F401
         except ImportError:
             from ..optimizer import OptimizerImportError
 
-            raise OptimizerImportError("fides")
+            raise OptimizerImportError("fides") from None
 
     def __call__(
         self, max_walltime_s: int, max_eval: int
     ) -> "pypesto.optimize.FidesOptimizer":
         """Create a :class:`FidesOptimizer` instance."""
 
         from fides.constants import Options as FidesOptions
```

### Comparing `pypesto-0.4.2/pypesto/optimize/load.py` & `pypesto-0.5.0/pypesto/optimize/load.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         Optimizer history options.
     """
     opt_hist = read_history_from_file(
         problem=problem, history_options=history_options, identifier=identifier
     )
     result = OptimizerResult(
         id=identifier,
-        message='loaded from file',
+        message="loaded from file",
         exitflag=EXITFLAG_LOADED_FROM_FILE,
         time=(
             max(opt_hist.history.get_time_trace())
             if len(opt_hist.history)
             else 0.0
         ),
     )
@@ -268,17 +268,17 @@
 
     Returns
     -------
         A result object in which the optimization result is constructed from
         history. But missing "Time, Message and Exitflag" keys.
     """
     result = Result()
-    with h5py.File(filename, 'r') as f:
+    with h5py.File(filename, "r") as f:
         ids = list(f[HISTORY].keys())
-        x0s = [f[f'{HISTORY}/{id}/{TRACE}/0/{X}'][()] for id in ids]
+        x0s = [f[f"{HISTORY}/{id}/{TRACE}/0/{X}"][()] for id in ids]
 
     for id, x0 in zip(ids, x0s):
         history = Hdf5History(id=id, file=filename)
         history.recover_options(filename)
         optimizer_history = OptimizerHistory(
             history=history,
             x0=x0,
```

### Comparing `pypesto-0.4.2/pypesto/optimize/optimize.py` & `pypesto-0.5.0/pypesto/optimize/optimize.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
-from typing import Callable, Iterable, Union
+from collections.abc import Iterable
+from typing import Callable, Union
 from warnings import warn
 
 from ..engine import Engine, SingleCoreEngine
 from ..history import HistoryOptions
 from ..problem import Problem
 from ..result import Result
 from ..startpoint import StartpointMethod, to_startpoint_method, uniform
@@ -91,16 +92,18 @@
     if startpoint_method is None:
         if problem.startpoint_method is None:
             startpoint_method = uniform
         else:
             startpoint_method = problem.startpoint_method
     else:
         warn(
-            "Passing `startpoint_method` directly is deprecated, use `problem.startpoint_method` instead.",
+            "Passing `startpoint_method` directly is deprecated, "
+            "use `problem.startpoint_method` instead.",
             DeprecationWarning,
+            stacklevel=2,
         )
 
     # convert startpoint method to class instance
     startpoint_method = to_startpoint_method(startpoint_method)
 
     # check options
     if options is None:
```

### Comparing `pypesto-0.4.2/pypesto/optimize/optimizer.py` & `pypesto-0.5.0/pypesto/optimize/optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 import abc
 import logging
 import re
 import time
 import warnings
 from functools import wraps
-from typing import TYPE_CHECKING, Dict, Optional
+from typing import TYPE_CHECKING
 
 import numpy as np
 import scipy.optimize
 
-from ..C import FVAL, GRAD, INNER_PARAMETERS, MODE_FUN, MODE_RES
+from ..C import FVAL, GRAD, INNER_PARAMETERS, MODE_FUN, MODE_RES, SPLINE_KNOTS
 from ..history import HistoryOptions, NoHistory, OptimizerHistory
 from ..objective import Objective
-from ..problem import Problem
+from ..problem import HierarchicalProblem, Problem
 from ..result import OptimizerResult
 from .load import fill_result_from_history
 from .options import OptimizeOptions
 from .util import check_finite_bounds
 
 if TYPE_CHECKING:
     import fides
@@ -57,20 +57,25 @@
             problem=problem,
             x0=x0,
             id=id,
             history_options=history_options,
             optimize_options=optimize_options,
         )
 
-        # add inner parameters
-        if (
-            hasattr(problem.objective, INNER_PARAMETERS)
-            and problem.objective.inner_parameters is not None
-        ):
-            result[INNER_PARAMETERS] = problem.objective.inner_parameters
+        if isinstance(problem, HierarchicalProblem):
+            # Call the objective to obtain inner parameters of
+            # the optimal outer optimization parameters
+            return_dict = problem.objective(
+                result.x,
+                return_dict=True,
+            )
+            if INNER_PARAMETERS in return_dict:
+                result[INNER_PARAMETERS] = return_dict[INNER_PARAMETERS]
+            if SPLINE_KNOTS in return_dict:
+                result[SPLINE_KNOTS] = return_dict[SPLINE_KNOTS]
 
         return result
 
     return wrapped_minimize
 
 
 def history_decorator(minimize):
@@ -129,15 +134,15 @@
         except Exception as err:
             if optimize_options and optimize_options.allow_failed_starts:
                 import sys
                 import traceback
 
                 trace = "\n".join(traceback.format_exception(*sys.exc_info()))
 
-                logger.error(f'start {id} failed:\n{trace}')
+                logger.error(f"start {id} failed:\n{trace}")
                 result = OptimizerResult(
                     x0=x0, exitflag=-1, message=str(err), id=id
                 )
             else:
                 raise
 
         # maybe override results from history depending on options
@@ -229,16 +234,16 @@
 
 def minimize_decorator_collection(minimize):
     """Collect all decorators for the minimize() method."""
 
     @wraps(minimize)
     @fix_decorator
     @time_decorator
-    @history_decorator
     @hierarchical_decorator
+    @history_decorator
     def wrapped_minimize(
         self,
         problem: Problem,
         x0: np.ndarray,
         id: str,
         history_options: HistoryOptions = None,
         optimize_options: OptimizeOptions = None,
@@ -316,17 +321,17 @@
     .. note::
         Least-squares optimizers may face errors in case of non-continuous
         differentiable objective functions (e.g. Laplace priors).
     """  # noqa
 
     def __init__(
         self,
-        method: str = 'L-BFGS-B',
+        method: str = "L-BFGS-B",
         tol: float = None,
-        options: Dict = None,
+        options: dict = None,
     ):
         super().__init__()
 
         self.method = method
 
         self.options = options
         if self.options is None:
@@ -368,46 +373,46 @@
                     "must be able to compute residuals."
                 )
 
             ls_method = self.method[3:]
             bounds = (lb, ub)
 
             fun = objective.get_res
-            jac = objective.get_sres if objective.has_sres else '2-point'
+            jac = objective.get_sres if objective.has_sres else "2-point"
             # TODO: pass jac computing methods in options
 
             if self.options is not None:
                 ls_options = self.options.copy()
-                ls_options['verbose'] = (
+                ls_options["verbose"] = (
                     2
-                    if 'disp' in ls_options.keys() and ls_options['disp']
+                    if "disp" in ls_options.keys() and ls_options["disp"]
                     else 0
                 )
-                ls_options.pop('disp', None)
-                ls_options['max_nfev'] = ls_options.pop('maxfun', None)
+                ls_options.pop("disp", None)
+                ls_options["max_nfev"] = ls_options.pop("maxfun", None)
             else:
                 ls_options = {}
 
             # optimize
             res = scipy.optimize.least_squares(
                 fun=fun,
                 x0=x0,
                 method=ls_method,
                 jac=jac,
                 bounds=bounds,
                 tr_solver=ls_options.pop(
-                    'tr_solver', 'lsmr' if len(x0) > 1 else 'exact'
+                    "tr_solver", "lsmr" if len(x0) > 1 else "exact"
                 ),
-                loss='linear',
+                loss="linear",
                 ftol=tol,
                 **ls_options,
             )
             # extract fval/grad from result, note that fval is not available
             # from least squares solvers
-            grad = getattr(res, 'grad', None)
+            grad = getattr(res, "grad", None)
             fval = None
         else:
             # is an fval based optimization method
 
             if not objective.has_fun:
                 raise Exception(
                     "For this optimizer, the objective must "
@@ -417,57 +422,58 @@
             bounds = scipy.optimize.Bounds(lb, ub)
 
             # fun_may_return_tuple = self.method.lower() in \
             #    ['cg', 'bfgs', 'newton-cg', 'l-bfgs-b', 'tnc', 'slsqp',
             #        'dogleg', 'trust-ncg']
             # TODO: is it more efficient to have tuple as output of fun?
             method_supports_grad = self.method.lower() in [
-                'cg',
-                'bfgs',
-                'newton-cg',
-                'l-bfgs-b',
-                'tnc',
-                'slsqp',
-                'dogleg',
-                'trust-ncg',
-                'trust-krylov',
-                'trust-exact',
-                'trust-constr',
+                "cg",
+                "bfgs",
+                "newton-cg",
+                "l-bfgs-b",
+                "tnc",
+                "slsqp",
+                "dogleg",
+                "trust-ncg",
+                "trust-krylov",
+                "trust-exact",
+                "trust-constr",
             ]
             method_supports_hess = self.method.lower() in [
-                'newton-cg',
-                'dogleg',
-                'trust-ncg',
-                'trust-krylov',
-                'trust-exact',
-                'trust-constr',
+                "newton-cg",
+                "dogleg",
+                "trust-ncg",
+                "trust-krylov",
+                "trust-exact",
+                "trust-constr",
             ]
             method_supports_hessp = self.method.lower() in [
-                'newton-cg',
-                'trust-ncg',
-                'trust-krylov',
-                'trust-constr',
+                "newton-cg",
+                "trust-ncg",
+                "trust-krylov",
+                "trust-constr",
             ]
             # switch off passing over functions if not applicable (e.g.
             # NegLogParameterPrior) since grad/hess attributes do not exist
             if not isinstance(objective, Objective):
-                if not hasattr(objective, 'grad'):
+                if not hasattr(objective, "grad"):
                     objective.grad = False
-                if not hasattr(objective, 'hess'):
+                if not hasattr(objective, "hess"):
                     objective.hess = False
             # Todo Resolve warning by implementing saving of hess temporarily
             #  in objective and pass to scipy seperately
             if objective.hess is True:
                 warnings.warn(
                     "scipy.optimize.minimize does not support "
                     "passing fun and hess as one function. Hence "
                     "for each evaluation of hess, fun will be "
                     "evaluated again. This can lead to increased "
                     "computation times. If possible, separate fun "
-                    "and hess."
+                    "and hess.",
+                    stacklevel=2,
                 )
             if objective.grad is True:
 
                 def fun(x):
                     return objective(x, sensi_orders=(0, 1))
 
             else:
@@ -502,58 +508,62 @@
                 hess=hess,
                 hessp=hessp,
                 bounds=bounds,
                 options=self.options,
                 tol=self.tol,
             )
             # extract fval/grad from result
-            grad = getattr(res, 'jac', None)
+            grad = getattr(res, "jac", None)
             fval = res.fun
 
         # fill in everything known, although some parts will be overwritten
         optimizer_result = OptimizerResult(
             x=np.array(res.x),
             fval=fval,
             grad=grad,
-            hess=getattr(res, 'hess', None),
+            hess=getattr(res, "hess", None),
             exitflag=res.status,
             message=res.message,
         )
 
         return optimizer_result
 
     def is_least_squares(self):
         """Check whether optimizer is a least squares optimizer."""
-        return re.match(r'(?i)^(ls_)', self.method)
+        return re.match(r"(?i)^(ls_)", self.method)
 
     def get_default_options(self):
         """Create default options specific for the optimizer."""
-        options = {'disp': False}
+        options = {"disp": False}
         if self.is_least_squares():
-            options['max_nfev'] = 1000
-        elif self.method.lower() in ('l-bfgs-b', 'tnc'):
-            options['maxfun'] = 1000
-        elif self.method.lower() in ('nelder-mead', 'powell'):
-            options['maxfev'] = 1000
+            options["max_nfev"] = 1000
+        elif self.method.lower() in ("l-bfgs-b", "tnc"):
+            options["maxfun"] = 1000
+        elif self.method.lower() in ("nelder-mead", "powell"):
+            options["maxfev"] = 1000
         return options
 
 
 class IpoptOptimizer(Optimizer):
     """Use IpOpt (https://pypi.org/project/ipopt/) for optimization."""
 
-    def __init__(self, options: Dict = None):
+    def __init__(self, options: dict = None):
         """
         Initialize.
 
         Parameters
         ----------
         options:
-            Options are directly passed on to `cyipopt.minimize_ipopt`.
+            Options are directly passed on to `cyipopt.minimize_ipopt`, except
+            for the `approx_grad` option, which is handled separately.
         """
         super().__init__()
+        self.approx_grad = False
+        if (options is not None) and "approx_grad" in options:
+            self.approx_grad = options.pop("approx_grad")
         self.options = options
 
     def __repr__(self) -> str:
         rep = f"<{self.__class__.__name__}"
         # print everything that is customized
         if self.options is not None:
             rep += f" options={self.options}"
@@ -568,25 +578,35 @@
         history_options: HistoryOptions = None,
         optimize_options: OptimizeOptions = None,
     ) -> OptimizerResult:
         """Perform optimization. Parameters: see `Optimizer` documentation."""
         try:
             import cyipopt
         except ImportError:
-            raise OptimizerImportError("ipopt")
+            raise OptimizerImportError("ipopt") from None
 
         objective = problem.objective
 
         bounds = np.array([problem.lb, problem.ub]).T
 
+        if self.approx_grad:
+            jac = None
+        elif objective.has_grad:
+            jac = objective.get_grad
+        else:
+            raise ValueError(
+                "For IPOPT, the objective must either be able to return "
+                "gradients or the `approx_grad` must be set to True."
+            )
+
         ret = cyipopt.minimize_ipopt(
             fun=objective.get_fval,
             x0=x0,
             method=None,  # ipopt does not use this argument for anything
-            jac=objective.get_grad,
+            jac=jac,
             hess=None,  # ipopt does not support Hessian yet
             hessp=None,  # ipopt does not support Hessian vector product yet
             bounds=bounds,
             tol=None,  # can be set via options
             options=self.options,
         )
 
@@ -599,22 +619,22 @@
         """Check whether optimizer is a least squares optimizer."""
         return False
 
 
 class DlibOptimizer(Optimizer):
     """Use the Dlib toolbox for optimization."""
 
-    def __init__(self, options: Dict = None):
+    def __init__(self, options: dict = None):
         super().__init__()
 
         self.options = options
         if self.options is None:
             self.options = DlibOptimizer.get_default_options(self)
-        elif 'maxiter' not in self.options:
-            raise KeyError('Dlib options are missing the key word ' 'maxiter.')
+        elif "maxiter" not in self.options:
+            raise KeyError("Dlib options are missing the key word " "maxiter.")
 
     def __repr__(self) -> str:
         rep = f"<{self.__class__.__name__}"
         # print everything that is customized
         if self.options is not None:
             rep += f" options={self.options}"
         return rep + ">"
@@ -633,15 +653,15 @@
         ub = problem.ub
         check_finite_bounds(lb, ub)
         objective = problem.objective
 
         try:
             import dlib
         except ImportError:
-            raise OptimizerImportError("dlib")
+            raise OptimizerImportError("dlib") from None
 
         if not objective.has_fun:
             raise ValueError(
                 "For this optimizer, the objective must "
                 "be able to return function values."
             )
 
@@ -649,45 +669,45 @@
         def get_fval_vararg(*x):
             return objective.get_fval(x)
 
         dlib.find_min_global(
             get_fval_vararg,
             list(lb),
             list(ub),
-            int(self.options['maxiter']),
+            int(self.options["maxiter"]),
             0.002,
         )
 
         optimizer_result = OptimizerResult()
 
         return optimizer_result
 
     def is_least_squares(self):
         """Check whether optimizer is a least squares optimizer."""
         return False
 
     def get_default_options(self):
         """Create default options specific for the optimizer."""
-        return {'maxiter': 10000}
+        return {"maxiter": 10000}
 
     def check_x0_support(self, x_guesses: np.ndarray = None) -> bool:
         """Check whether optimizer supports x0."""
         if x_guesses is not None and x_guesses.size > 0:
             logger.warning("The Dlib optimizer does not support x0.")
         return False
 
 
 class PyswarmOptimizer(Optimizer):
     """Global optimization using pyswarm."""
 
-    def __init__(self, options: Dict = None):
+    def __init__(self, options: dict = None):
         super().__init__()
 
         if options is None:
-            options = {'maxiter': 200}
+            options = {"maxiter": 200}
         self.options = options
 
     def __repr__(self) -> str:
         rep = f"<{self.__class__.__name__}"
         # print everything that is customized
         if self.options is not None:
             rep += f" options={self.options}"
@@ -705,15 +725,15 @@
         """Perform optimization. Parameters: see `Optimizer` documentation."""
         lb = problem.lb
         ub = problem.ub
 
         try:
             import pyswarm
         except ImportError:
-            raise OptimizerImportError("pyswarm")
+            raise OptimizerImportError("pyswarm") from None
 
         check_finite_bounds(lb, ub)
 
         xopt, fopt = pyswarm.pso(
             problem.objective.get_fval, lb, ub, **self.options
         )
 
@@ -728,23 +748,23 @@
     def check_x0_support(self, x_guesses: np.ndarray = None) -> bool:
         """Check whether optimizer supports x0."""
         if x_guesses is not None and x_guesses.size > 0:
             logger.warning("The pyswarm optimizer does not support x0.")
         return False
 
 
-class CmaesOptimizer(Optimizer):
+class CmaOptimizer(Optimizer):
     """
     Global optimization using covariance matrix adaptation evolutionary search.
 
     This optimizer interfaces the cma package
     (https://github.com/CMA-ES/pycma).
     """
 
-    def __init__(self, par_sigma0: float = 0.25, options: Dict = None):
+    def __init__(self, par_sigma0: float = 0.25, options: dict = None):
         """
         Initialize.
 
         Parameters
         ----------
         par_sigma0:
             scalar, initial standard deviation in each coordinate.
@@ -752,15 +772,15 @@
             (where the optimum is to be expected)
         options:
             Optimizer options that are directly passed on to cma.
         """
         super().__init__()
 
         if options is None:
-            options = {'maxiter': 10000}
+            options = {"maxiter": 10000}
         self.options = options
         self.par_sigma0 = par_sigma0
 
     def __repr__(self) -> str:
         rep = f"<{self.__class__.__name__} par_sigma0={self.par_sigma0}"
         # print everything that is customized
         if self.options is not None:
@@ -779,20 +799,20 @@
         """Perform optimization. Parameters: see `Optimizer` documentation."""
         lb = problem.lb
         ub = problem.ub
 
         check_finite_bounds(lb, ub)
 
         sigma0 = self.par_sigma0 * np.median(ub - lb)
-        self.options['bounds'] = [lb, ub]
+        self.options["bounds"] = [lb, ub]
 
         try:
             import cma
         except ImportError:
-            raise OptimizerImportError("cma")
+            raise OptimizerImportError("cma") from None
 
         result = (
             cma.CMAEvolutionStrategy(
                 x0,
                 sigma0,
                 inopts=self.options,
             )
@@ -807,14 +827,27 @@
         return optimizer_result
 
     def is_least_squares(self):
         """Check whether optimizer is a least squares optimizer."""
         return False
 
 
+class CmaesOptimizer(CmaOptimizer):
+    """Deprecated, use CmaOptimizer instead."""
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        warnings.warn(
+            "`CmaesOptimizer` has been renamed to `CmaOptimizer`, "
+            "please update your code.",
+            DeprecationWarning,
+            stacklevel=1,
+        )
+
+
 class ScipyDifferentialEvolutionOptimizer(Optimizer):
     """
     Global optimization using scipy's differential evolution optimizer.
 
     See: :func:`scipy.optimize.differential_evolution`.
 
     Parameters
@@ -830,19 +863,19 @@
         used to calculate the maximal number of function evaluations by
         ``maxfevals = (maxiter + 1) * popsize * len(x)``
         Default: 100
     popsize:
         population size, default value 15
     """
 
-    def __init__(self, options: Dict = None):
+    def __init__(self, options: dict = None):
         super().__init__()
 
         if options is None:
-            options = {'maxiter': 100}
+            options = {"maxiter": 100}
         self.options = options
 
     def __repr__(self) -> str:
         rep = f"<{self.__class__.__name__}"
         # print everything that is customized
         if self.options is not None:
             rep += f" options={self.options}"
@@ -901,18 +934,18 @@
     Arguments that can be passed to options:
 
     maxiter:
         used to calculate the maximal number of funcion evaluations.
         Default: 1000
     """
 
-    def __init__(self, par_popsize: float = 10, options: Dict = None):
+    def __init__(self, par_popsize: float = 10, options: dict = None):
         super().__init__()
 
-        all_options = {'maxiter': 1000, 'c1': 0.5, 'c2': 0.3, 'w': 0.9}
+        all_options = {"maxiter": 1000, "c1": 0.5, "c2": 0.3, "w": 0.9}
         if options is None:
             options = {}
         all_options.update(options)
         self.options = all_options
         self.par_popsize = par_popsize
 
     def __repr__(self) -> str:
@@ -934,15 +967,15 @@
         """Perform optimization. Parameters: see `Optimizer` documentation."""
         lb = problem.lb
         ub = problem.ub
 
         try:
             import pyswarms
         except ImportError:
-            raise OptimizerImportError("pyswarms")
+            raise OptimizerImportError("pyswarms") from None
 
         # check for finite values for the bounds
         if np.isfinite(lb).all() is np.False_:
             raise ValueError(
                 "This optimizer can only handle finite lower bounds."
             )
         if np.isfinite(ub).all() is np.False_:
@@ -975,15 +1008,15 @@
             for i_particle, par in enumerate(swarm):
                 result[i_particle] = problem.objective.get_fval(par)
 
             return result
 
         cost, pos = optimizer.optimize(
             successively_working_fval,
-            iters=self.options['maxiter'],
+            iters=self.options["maxiter"],
             verbose=False,
         )
 
         optimizer_result = OptimizerResult(
             x=pos,
             fval=float(cost),
         )
@@ -1008,16 +1041,16 @@
     Package homepage: https://nlopt.readthedocs.io/en/latest/
     """
 
     def __init__(
         self,
         method=None,
         local_method=None,
-        options: Dict = None,
-        local_options: Dict = None,
+        options: dict = None,
+        local_options: dict = None,
     ):
         """
         Initialize.
 
         Parameters
         ----------
         method:
@@ -1032,25 +1065,25 @@
         local_options:
             Optimizer options for the local method
         """
         super().__init__()
 
         if options is None:
             options = {}
-        elif 'maxiter' in options:
-            options['maxeval'] = options.pop('maxiter')
+        elif "maxiter" in options:
+            options["maxeval"] = options.pop("maxiter")
         if local_options is None:
             local_options = {}
         self.options = options
         self.local_options = local_options
 
         try:
             import nlopt
         except ImportError:
-            raise OptimizerImportError("nlopt")
+            raise OptimizerImportError("nlopt") from None
 
         if method is None:
             method = nlopt.LD_LBFGS
 
         needs_local_method = [
             nlopt.G_MLSL,
             nlopt.G_MLSL_LDS,
@@ -1062,15 +1095,15 @@
 
         if local_method is None and method in needs_local_method:
             local_method = nlopt.LD_LBFGS
 
         if local_method is not None and method not in needs_local_method:
             raise ValueError(
                 f'Method "{method}" does not allow a local '
-                f'method. Please set `local_method` to None.'
+                f"method. Please set `local_method` to None."
             )
 
         self.local_methods = [
             nlopt.LD_VAR1,
             nlopt.LD_VAR2,
             nlopt.LD_TNEWTON_PRECOND_RESTART,
             nlopt.LD_TNEWTON_PRECOND,
@@ -1111,23 +1144,23 @@
         methods = (
             self.local_methods + self.global_methods + self.hybrid_methods
         )
 
         if method not in methods:
             raise ValueError(
                 f'"{method}" is not a valid method. Valid '
-                f'methods are: {methods}'
+                f"methods are: {methods}"
             )
 
         self.method = method
 
         if local_method is not None and local_method not in self.local_methods:
             raise ValueError(
                 f'"{local_method}" is not a valid method. Valid '
-                f'methods are: {self.local_methods}'
+                f"methods are: {self.local_methods}"
             )
 
         self.local_method = local_method
 
     def __repr__(self) -> str:
         rep = f"<{self.__class__.__name__} method={self.method}"
         # print everything that is customized
@@ -1150,33 +1183,33 @@
     ) -> OptimizerResult:
         """Perform optimization. Parameters: see `Optimizer` documentation."""
         import nlopt
 
         opt = nlopt.opt(self.method, problem.dim)
 
         valid_options = [
-            'ftol_abs',
-            'ftol_rel',
-            'xtol_abs',
-            'xtol_rel',
-            'stopval',
-            'x_weights',
-            'maxeval',
-            'maxtime',
-            'initial_step',
+            "ftol_abs",
+            "ftol_rel",
+            "xtol_abs",
+            "xtol_rel",
+            "stopval",
+            "x_weights",
+            "maxeval",
+            "maxtime",
+            "initial_step",
         ]
 
         def set_options(o, options):
             for option, value in options.items():
                 if option not in valid_options:
                     raise ValueError(
                         f'"{option}" is not a valid option. Valid '
-                        f'options are: {valid_options}'
+                        f"options are: {valid_options}"
                     )
-                getattr(o, f'set_{option}')(value)
+                getattr(o, f"set_{option}")(value)
 
         if self.local_method is not None:
             local_opt = nlopt.opt(self.local_method, problem.dim)
             set_options(local_opt, self.local_options)
             opt.set_local_optimizer(local_opt)
 
         if self.method in self.global_methods:
@@ -1196,15 +1229,15 @@
             return r[FVAL]
 
         opt.set_min_objective(nlopt_objective)
 
         set_options(opt, self.options)
         try:
             result = opt.optimize(x0)
-            msg = 'Finished Successfully.'
+            msg = "Finished Successfully."
         except (
             nlopt.RoundoffLimited,
             nlopt.ForcedStop,
             ValueError,
             RuntimeError,
             MemoryError,
         ) as e:
@@ -1254,19 +1287,18 @@
     Global/Local optimization using the trust region optimizer fides.
 
     Package Homepage: https://fides-optimizer.readthedocs.io/en/latest
     """
 
     def __init__(
         self,
-        hessian_update: Optional[
-            fides.hessian_approximation.HessianApproximation
-        ] = 'default',
-        options: Optional[Dict] = None,
-        verbose: Optional[int] = logging.INFO,
+        hessian_update: None
+        | (fides.hessian_approximation.HessianApproximation) = "default",
+        options: dict | None = None,
+        verbose: int | None = logging.INFO,
     ):
         """
         Initialize.
 
         Parameters
         ----------
         options:
@@ -1278,42 +1310,42 @@
             approximation) to a BFGS approximation will be used.
         """
         super().__init__()
 
         try:
             import fides
         except ImportError:
-            raise OptimizerImportError("fides")
+            raise OptimizerImportError("fides") from None
 
         if (
             (hessian_update is not None)
-            and (hessian_update != 'default')
+            and (hessian_update != "default")
             and not isinstance(
                 hessian_update,
                 fides.hessian_approximation.HessianApproximation,
             )
         ):
             raise ValueError(
-                'Incompatible type for hessian update. '
-                'Must be a HessianApproximation, '
-                f'was {type(hessian_update)}.'
+                "Incompatible type for hessian update. "
+                "Must be a HessianApproximation, "
+                f"was {type(hessian_update)}."
             )
 
         if options is None:
             options = {}
 
         self.verbose = verbose
         self.options = options
         self.hessian_update = hessian_update
 
     def __repr__(self) -> str:
         rep = f"<{self.__class__.__name__} "
         # print everything that is customized
         if self.hessian_update is not None:
-            if self.hessian_update == 'default':
+            if self.hessian_update == "default":
                 rep += f" hessian_update={self.hessian_update}"
             else:
                 rep += (
                     f" hessian_update="
                     f"{self.hessian_update.__class__.__name__}"
                 )
         if self.verbose is not None:
@@ -1330,55 +1362,56 @@
         id: str,
         history_options: HistoryOptions = None,
         optimize_options: OptimizeOptions = None,
     ) -> OptimizerResult:
         """Perform optimization. Parameters: see `Optimizer` documentation."""
         import fides
 
-        if self.hessian_update == 'default':
+        if self.hessian_update == "default":
             if not problem.objective.has_hess:
                 warnings.warn(
-                    'Fides is using BFGS as hessian approximation, '
-                    'as the problem does not provide a Hessian. '
-                    'Specify a Hessian to use a more efficient '
-                    'hybrid approximation scheme.'
+                    "Fides is using BFGS as hessian approximation, "
+                    "as the problem does not provide a Hessian. "
+                    "Specify a Hessian to use a more efficient "
+                    "hybrid approximation scheme.",
+                    stacklevel=1,
                 )
                 _hessian_update = fides.BFGS()
             else:
                 _hessian_update = fides.HybridFixed()
         else:
             _hessian_update = self.hessian_update
 
         resfun = (
             _hessian_update.requires_resfun
             if _hessian_update is not None
             else False
         )
 
-        args = {'mode': MODE_RES if resfun else MODE_FUN}
+        args = {"mode": MODE_RES if resfun else MODE_FUN}
 
         if not problem.objective.has_grad:
             raise ValueError(
-                'Fides cannot be applied to problems '
-                'with objectives that do not support '
-                'gradient evaluation.'
+                "Fides cannot be applied to problems "
+                "with objectives that do not support "
+                "gradient evaluation."
             )
 
         if _hessian_update is None or (
             _hessian_update.requires_hess and not resfun
         ):
             if not problem.objective.has_hess:
                 raise ValueError(
-                    'Specified hessian update scheme cannot be '
-                    'used with objectives that do not support '
-                    'Hessian computation.'
+                    "Specified hessian update scheme cannot be "
+                    "used with objectives that do not support "
+                    "Hessian computation."
                 )
-            args['sensi_orders'] = (0, 1, 2)
+            args["sensi_orders"] = (0, 1, 2)
         else:
-            args['sensi_orders'] = (0, 1)
+            args["sensi_orders"] = (0, 1)
 
         opt = fides.Optimizer(
             fun=problem.objective,
             funargs=args,
             ub=problem.ub,
             lb=problem.lb,
             verbose=self.verbose,
```

### Comparing `pypesto-0.4.2/pypesto/optimize/options.py` & `pypesto-0.5.0/pypesto/optimize/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Union
+from typing import Union
 
 
 class OptimizeOptions(dict):
     """
     Options for the multistart optimization.
 
     Parameters
@@ -38,23 +38,23 @@
         self.report_hess: bool = report_hess
         self.history_beats_optimizer: bool = history_beats_optimizer
 
     def __getattr__(self, key):
         try:
             return self[key]
         except KeyError:
-            raise AttributeError(key)
+            raise AttributeError(key) from None
 
     __setattr__ = dict.__setitem__
     __delattr__ = dict.__delitem__
 
     @staticmethod
     def assert_instance(
-        maybe_options: Union['OptimizeOptions', Dict],
-    ) -> 'OptimizeOptions':
+        maybe_options: Union["OptimizeOptions", dict],
+    ) -> "OptimizeOptions":
         """
         Return a valid options object.
 
         Parameters
         ----------
         maybe_options: OptimizeOptions or dict
         """
```

### Comparing `pypesto-0.4.2/pypesto/optimize/task.py` & `pypesto-0.5.0/pypesto/optimize/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 
 
 class OptimizerTask(Task):
     """A multistart optimization task, performed in `pypesto.minimize`."""
 
     def __init__(
         self,
-        optimizer: 'pypesto.optimize.Optimizer',
+        optimizer: "pypesto.optimize.Optimizer",
         problem: Problem,
         x0: np.ndarray,
         id: str,
         history_options: HistoryOptions,
-        optimize_options: 'pypesto.optimize.OptimizeOptions',
+        optimize_options: "pypesto.optimize.OptimizeOptions",
     ):
         """Create the task object.
 
         Parameters
         ----------
         optimizer:
             The optimizer to use.
```

### Comparing `pypesto-0.4.2/pypesto/optimize/util.py` & `pypesto-0.5.0/pypesto/optimize/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Utility functions for :py:func:`pypesto.optimize.minimize`."""
 
 import logging
 import os
+from collections.abc import Iterable
 from pathlib import Path
-from typing import Iterable, List
 
 import h5py
 import numpy as np
 
 from .. import C
 from ..engine import Engine, SingleCoreEngine
 from ..history import CsvHistoryTemplateError, HistoryOptions, HistoryTypeError
@@ -75,15 +75,15 @@
     # set history file to template path
     history_options.storage_file = str(template_path)
 
     return True
 
 
 def postprocess_hdf5_history(
-    ret: List[OptimizerResult],
+    ret: list[OptimizerResult],
     storage_file: str,
     history_options: HistoryOptions,
 ) -> None:
     """Create single history file pointing to files of multiple starts.
 
     Create links in `storage_file` to the history of each start contained in
     `ret`, the results of the optimization.
@@ -97,22 +97,22 @@
         are to be gathered.
     history_options:
         History options used in the optimization.
     """
     # create hdf5 file that gathers the others within history group
     if "{id}" in storage_file:
         storage_file = storage_file.replace("{id}", "")
-    with h5py.File(storage_file, mode='w') as f:
+    with h5py.File(storage_file, mode="w") as f:
         # create file and group
         f.require_group("history")
         # append links to each single result file
         for result in ret:
-            id = result['id']
-            f[f'history/{id}'] = h5py.ExternalLink(
-                result['history'].file, f'history/{id}'
+            id = result["id"]
+            f[f"history/{id}"] = h5py.ExternalLink(
+                result["history"].file, f"history/{id}"
             )
 
     # reset storage file (undo preprocessing changes)
     history_options.storage_file = storage_file
 
 
 def bound_n_starts_from_env(n_starts: int):
@@ -181,10 +181,10 @@
     return ids
 
 
 def check_finite_bounds(lb, ub):
     """Raise if bounds are not finite."""
     if not np.isfinite(lb).all() or not np.isfinite(ub).all():
         raise ValueError(
-            'Selected optimizer cannot work with unconstrained '
-            'optimization problems.'
+            "Selected optimizer cannot work with unconstrained "
+            "optimization problems."
         )
```

### Comparing `pypesto-0.4.2/pypesto/petab/importer.py` & `pypesto-0.5.0/pypesto/petab/importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 """Contains the PetabImporter class."""
 
 from __future__ import annotations
 
-import importlib
 import logging
 import os
 import shutil
 import sys
 import tempfile
 import warnings
+from collections.abc import Iterable, Sequence
 from dataclasses import dataclass
 from functools import partial
 from importlib.metadata import version
 from typing import (
     Any,
     Callable,
-    Dict,
-    Iterable,
-    List,
-    Optional,
-    Sequence,
-    Tuple,
-    Union,
 )
 
 import numpy as np
 import pandas as pd
 
 from ..C import (
     CENSORED,
@@ -49,18 +42,20 @@
 from ..predict import AmiciPredictor
 from ..problem import HierarchicalProblem, Problem
 from ..result import PredictionResult
 from ..startpoint import CheckedStartpoints, StartpointMethod
 
 try:
     import amici
-    import amici.parameter_mapping
-    import amici.petab_import
-    import amici.petab_objective
+    import amici.petab
+    import amici.petab.conditions
+    import amici.petab.parameter_mapping
+    import amici.petab.simulations
     import petab
+    from amici.petab.import_helpers import check_model
     from petab.C import (
         ESTIMATE,
         NOISE_PARAMETERS,
         OBSERVABLE_ID,
         PREEQUILIBRATION_CONDITION_ID,
         SIMULATION_CONDITION_ID,
     )
@@ -89,15 +84,15 @@
         self,
         petab_problem: petab.Problem,
         output_folder: str = None,
         model_name: str = None,
         validate_petab: bool = True,
         validate_petab_hierarchical: bool = True,
         hierarchical: bool = False,
-        inner_options: Dict = None,
+        inner_options: dict = None,
     ):
         """Initialize importer.
 
         Parameters
         ----------
         petab_problem:
             Managing access to the model and data.
@@ -174,15 +169,15 @@
 
         if model_name is None:
             model_name = _find_model_name(self.output_folder)
         self.model_name = model_name
 
     @staticmethod
     def from_yaml(
-        yaml_config: Union[dict, str],
+        yaml_config: dict | str,
         output_folder: str = None,
         model_name: str = None,
     ) -> PetabImporter:
         """Simplified constructor using a petab yaml file."""
         petab_problem = petab.Problem.from_yaml(yaml_config)
 
         return PetabImporter(
@@ -198,15 +193,15 @@
                 raise ValueError(f"Unknown inner option {key}.")
 
     def check_gradients(
         self,
         *args,
         rtol: float = 1e-2,
         atol: float = 1e-3,
-        mode: Union[str, List[str]] = None,
+        mode: str | list[str] = None,
         multi_eps=None,
         **kwargs,
     ) -> bool:
         """
         Check if gradients match finite differences (FDs).
 
         Parameters
@@ -327,15 +322,15 @@
     def _create_model(self) -> amici.Model:
         """Load model module and return the model, no checks/compilation."""
         # load moduĺe
         module = amici.import_model_module(
             module_name=self.model_name, module_path=self.output_folder
         )
         model = module.getModel()
-        amici.petab_import.check_model(
+        check_model(
             amici_model=model,
             petab_problem=self.petab_problem,
         )
 
         return model
 
     def _must_compile(self, force_compile: bool):
@@ -349,15 +344,15 @@
             self.output_folder
         ):
             return True
 
         # try to import (in particular checks version)
         try:
             # importing will already raise an exception if version wrong
-            importlib.import_module(self.model_name)
+            amici.import_model_module(self.model_name, self.output_folder)
         except ModuleNotFoundError:
             return True
         except amici.AmiciVersionError as e:
             logger.info(
                 "amici model will be re-imported due to version "
                 f"mismatch: {e}"
             )
@@ -378,15 +373,15 @@
             Extra arguments passed to :meth:`amici.sbml_import.SbmlImporter.sbml2amici`
             or :func:`amici.pysb_import.pysb2amici`.
         """
         # delete output directory
         if os.path.exists(self.output_folder):
             shutil.rmtree(self.output_folder)
 
-        amici.petab_import.import_petab_problem(
+        amici.petab.import_petab_problem(
             petab_problem=self.petab_problem,
             model_name=self.model_name,
             model_output_dir=self.output_folder,
             **kwargs,
         )
 
     def create_solver(
@@ -403,21 +398,21 @@
         return solver
 
     def create_edatas(
         self,
         model: amici.Model = None,
         simulation_conditions=None,
         verbose: bool = True,
-    ) -> List[amici.ExpData]:
+    ) -> list[amici.ExpData]:
         """Create list of :class:`amici.amici.ExpData` objects."""
         # create model
         if model is None:
             model = self.create_model(verbose=verbose)
 
-        return amici.petab_objective.create_edatas(
+        return amici.petab.conditions.create_edatas(
             amici_model=model,
             petab_problem=self.petab_problem,
             simulation_conditions=simulation_conditions,
         )
 
     def create_objective(
         self,
@@ -468,45 +463,47 @@
             solver = self.create_solver(model)
         # create conditions and edatas from measurement data
         if edatas is None:
             edatas = self.create_edatas(
                 model=model, simulation_conditions=simulation_conditions
             )
 
-        parameter_mapping = amici.petab_objective.create_parameter_mapping(
-            petab_problem=self.petab_problem,
-            simulation_conditions=simulation_conditions,
-            scaled_parameters=True,
-            amici_model=model,
-            fill_fixed_parameters=False,
+        parameter_mapping = (
+            amici.petab.parameter_mapping.create_parameter_mapping(
+                petab_problem=self.petab_problem,
+                simulation_conditions=simulation_conditions,
+                scaled_parameters=True,
+                amici_model=model,
+                fill_fixed_parameters=False,
+            )
         )
 
         par_ids = self.petab_problem.x_ids
 
         # fill in dummy parameters (this is needed since some objective
         #  initialization e.g. checks for preeq parameters)
         problem_parameters = dict(
             zip(self.petab_problem.x_ids, self.petab_problem.x_nominal_scaled)
         )
-        amici.parameter_mapping.fill_in_parameters(
+        amici.petab.conditions.fill_in_parameters(
             edatas=edatas,
             problem_parameters=problem_parameters,
             scaled_parameters=True,
             parameter_mapping=parameter_mapping,
             amici_model=model,
         )
 
         calculator = None
         amici_reporting = None
 
         if (
             self._non_quantitative_data_types is not None
             and self._hierarchical
         ):
-            inner_options = kwargs.pop('inner_options', None)
+            inner_options = kwargs.pop("inner_options", None)
             inner_options = (
                 inner_options
                 if inner_options is not None
                 else self.inner_options
             )
             calculator = InnerCalculatorCollector(
                 self._non_quantitative_data_types,
@@ -514,23 +511,25 @@
                 model,
                 edatas,
                 inner_options,
             )
             amici_reporting = amici.RDataReporting.full
 
             # FIXME: currently not supported with hierarchical
-            if 'guess_steadystate' in kwargs and kwargs['guess_steadystate']:
+            if "guess_steadystate" in kwargs and kwargs["guess_steadystate"]:
                 warnings.warn(
-                    "`guess_steadystate` not supported with hierarchical optimization. Disabling `guess_steadystate`."
+                    "`guess_steadystate` not supported with hierarchical "
+                    "optimization. Disabling `guess_steadystate`.",
+                    stacklevel=1,
                 )
-            kwargs['guess_steadystate'] = False
+            kwargs["guess_steadystate"] = False
             inner_parameter_ids = calculator.get_inner_par_ids()
             par_ids = [x for x in par_ids if x not in inner_parameter_ids]
 
-        max_sensi_order = kwargs.get('max_sensi_order', None)
+        max_sensi_order = kwargs.get("max_sensi_order", None)
 
         if (
             self._non_quantitative_data_types is not None
             and any(
                 data_type in self._non_quantitative_data_types
                 for data_type in [ORDINAL, CENSORED, SEMIQUANTITATIVE]
             )
@@ -559,18 +558,18 @@
 
         return obj
 
     def create_predictor(
         self,
         objective: AmiciObjective = None,
         amici_output_fields: Sequence[str] = None,
-        post_processor: Union[Callable, None] = None,
-        post_processor_sensi: Union[Callable, None] = None,
-        post_processor_time: Union[Callable, None] = None,
-        max_chunk_size: Union[int, None] = None,
+        post_processor: Callable | None = None,
+        post_processor_sensi: Callable | None = None,
+        post_processor_time: Callable | None = None,
+        max_chunk_size: int | None = None,
         output_ids: Sequence[str] = None,
         condition_ids: Sequence[str] = None,
     ) -> AmiciPredictor:
         """Create a :class:`pypesto.predict.AmiciPredictor`.
 
         The `AmiciPredictor` facilitates generation of predictions from
         parameter vectors.
@@ -618,19 +617,17 @@
         """
         # if the user didn't pass an objective function, we create it first
         if objective is None:
             objective = self.create_objective()
 
         # create a identifiers of preequilibration and simulation condition ids
         # which can then be stored in the prediction result
-        edata_conditions = (
-            objective.amici_object_builder.petab_problem.get_simulation_conditions_from_measurement_df()
-        )
+        edata_conditions = objective.amici_object_builder.petab_problem.get_simulation_conditions_from_measurement_df()
         if PREEQUILIBRATION_CONDITION_ID not in list(edata_conditions.columns):
-            preeq_dummy = [''] * edata_conditions.shape[0]
+            preeq_dummy = [""] * edata_conditions.shape[0]
             edata_conditions[PREEQUILIBRATION_CONDITION_ID] = preeq_dummy
         edata_conditions.drop_duplicates(inplace=True)
 
         if condition_ids is None:
             condition_ids = [
                 edata_conditions.loc[id, PREEQUILIBRATION_CONDITION_ID]
                 + CONDITION_SEP
@@ -648,15 +645,15 @@
             max_chunk_size=max_chunk_size,
             output_ids=output_ids,
             condition_ids=condition_ids,
         )
 
         return predictor
 
-    def create_prior(self) -> Union[NegLogParameterPriors, None]:
+    def create_prior(self) -> NegLogParameterPriors | None:
         """
         Create a prior from the parameter table.
 
         Returns None, if no priors are defined.
         """
         prior_list = []
 
@@ -670,15 +667,15 @@
                     isinstance(prior_type_entry, str)
                     and prior_type_entry != petab.PARAMETER_SCALE_UNIFORM
                 ):
                     prior_params = [
                         float(param)
                         for param in self.petab_problem.parameter_df.loc[
                             x_id, petab.OBJECTIVE_PRIOR_PARAMETERS
-                        ].split(';')
+                        ].split(";")
                     ]
 
                     scale = self.petab_problem.parameter_df.loc[
                         x_id, petab.PARAMETER_SCALE
                     ]
 
                     prior_list.append(
@@ -702,17 +699,17 @@
             :meth:`pypesto.startpoint.FunctionStartpoints.__init__`.
         """
         return PetabStartpoints(petab_problem=self.petab_problem, **kwargs)
 
     def create_problem(
         self,
         objective: AmiciObjective = None,
-        x_guesses: Optional[Iterable[float]] = None,
-        problem_kwargs: Dict[str, Any] = None,
-        startpoint_kwargs: Dict[str, Any] = None,
+        x_guesses: Iterable[float] | None = None,
+        problem_kwargs: dict[str, Any] = None,
+        startpoint_kwargs: dict[str, Any] = None,
         **kwargs,
     ) -> Problem:
         """Create a :class:`pypesto.problem.Problem`.
 
         Parameters
         ----------
         objective:
@@ -832,15 +829,15 @@
         """
         # create model
         if model is None:
             model = self.create_model(verbose=verbose)
 
         measurement_df = self.petab_problem.measurement_df
 
-        return amici.petab_objective.rdatas_to_measurement_df(
+        return amici.petab.simulations.rdatas_to_measurement_df(
             rdatas, model, measurement_df
         )
 
     def rdatas_to_simulation_df(
         self,
         rdatas: Sequence[amici.ReturnData],
         model: amici.Model = None,
@@ -1036,16 +1033,16 @@
     Samples optimization startpoints from the distributions defined in the
     provided PEtab problem. The PEtab-problem is copied.
     """
 
     def __init__(self, petab_problem: petab.Problem, **kwargs):
         super().__init__(**kwargs)
         self._parameter_df = petab_problem.parameter_df.copy()
-        self._priors: Optional[List[Tuple]] = None
-        self._free_ids: Optional[List[str]] = None
+        self._priors: list[tuple] | None = None
+        self._free_ids: list[str] | None = None
 
     def _setup(
         self,
         pypesto_problem: Problem,
     ):
         """Update priors if necessary.
```

### Comparing `pypesto-0.4.2/pypesto/predict/amici_predictor.py` & `pypesto-0.5.0/pypesto/predict/amici_predictor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
+from collections.abc import Sequence
 from copy import deepcopy
-from typing import TYPE_CHECKING, Callable, Sequence, Union
+from typing import TYPE_CHECKING, Callable
 
 import numpy as np
 
 from ..C import (
     AMICI_LLH,
     AMICI_SIGMAY,
     AMICI_STATUS,
@@ -52,21 +53,21 @@
     output, these checks are also left to the user. An example for such a check
     is provided in the default output (see :meth:`_default_output()`).
     """
 
     def __init__(
         self,
         amici_objective: AmiciObjective,
-        amici_output_fields: Union[Sequence[str], None] = None,
-        post_processor: Union[PostProcessor, None] = None,
-        post_processor_sensi: Union[PostProcessor, None] = None,
-        post_processor_time: Union[PostProcessor, None] = None,
-        max_chunk_size: Union[int, None] = None,
-        output_ids: Union[Sequence[str], None] = None,
-        condition_ids: Union[Sequence[str], None] = None,
+        amici_output_fields: Sequence[str] | None = None,
+        post_processor: PostProcessor | None = None,
+        post_processor_sensi: PostProcessor | None = None,
+        post_processor_time: PostProcessor | None = None,
+        max_chunk_size: int | None = None,
+        output_ids: Sequence[str] | None = None,
+        condition_ids: Sequence[str] | None = None,
     ):
         """
         Initialize predictor.
 
         Parameters
         ----------
         amici_objective:
@@ -152,15 +153,15 @@
         self.amici_output_fields = amici_output_fields
 
     def __call__(
         self,
         x: np.ndarray,
         sensi_orders: tuple[int, ...] = (0,),
         mode: ModeType = MODE_FUN,
-        output_file: str = '',
+        output_file: str = "",
         output_format: str = CSV,
         include_llh_weights: bool = False,
         include_sigmay: bool = False,
     ) -> PredictionResult:
         """
         Call the predictor.
 
@@ -195,16 +196,16 @@
         -------
         PredictionResult object containing timepoints, outputs, and
         output sensitivities if requested.
         """
         # sanity check for output
         if 2 in sensi_orders:
             raise Exception(
-                'Prediction simulation does currently not support '
-                'second order output.'
+                "Prediction simulation does currently not support "
+                "second order output."
             )
         # add llh and sigmay to amici output fields if requested
         if include_llh_weights and AMICI_LLH not in self.amici_output_fields:
             self.amici_output_fields.append(AMICI_LLH)
         if include_sigmay and AMICI_SIGMAY not in self.amici_output_fields:
             self.amici_output_fields.append(AMICI_SIGMAY)
 
@@ -253,16 +254,16 @@
             if output_format == CSV:
                 results.write_to_csv(output_file=output_file)
             # Do we want an h5 file?
             elif output_format == H5:
                 results.write_to_h5(output_file=output_file)
             else:
                 raise ValueError(
-                    f'Call to unknown format {output_format} for '
-                    f'output of pyPESTO prediction.'
+                    f"Call to unknown format {output_format} for "
+                    f"output of pyPESTO prediction."
                 )
 
         # return dependent on sensitivity order
         return results
 
     def _get_outputs(
         self,
@@ -341,15 +342,15 @@
                 sensi_orders=sensi_orders,
                 parameter_mapping=self.amici_objective.parameter_mapping[ids],
                 edatas=self.amici_objective.edatas[ids],
                 mode=mode,
             )
 
         def _default_output(
-            amici_outputs: list[dict[str, np.array]]
+            amici_outputs: list[dict[str, np.array]],
         ) -> tuple[
             list[np.array],
             list[np.array],
             list[np.array],
             list[np.array],
             list[np.array],
         ]:
```

### Comparing `pypesto-0.4.2/pypesto/predict/task.py` & `pypesto-0.5.0/pypesto/predict/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Sequence, Tuple
+from collections.abc import Sequence
 
 from ..C import ModeType
 from ..engine import Task
 
 logger = logging.getLogger(__name__)
 
 
@@ -26,15 +26,15 @@
         The input ID.
     """
 
     def __init__(
         self,
         predictor,  #: 'pypesto.predict.Predictor',  # noqa: F821
         x: Sequence[float],
-        sensi_orders: Tuple[int, ...],
+        sensi_orders: tuple[int, ...],
         mode: ModeType,
         id: str,
     ):
         super().__init__()
         self.predictor = predictor
         self.x = x
         self.sensi_orders = sensi_orders
```

### Comparing `pypesto-0.4.2/pypesto/problem/base.py` & `pypesto-0.5.0/pypesto/problem/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import copy
 import logging
+from collections.abc import Iterable
 from typing import (
     Callable,
-    Iterable,
-    List,
     Optional,
     SupportsFloat,
     SupportsInt,
     Union,
 )
 
 import numpy as np
@@ -86,25 +85,25 @@
     the full representation is needed, the methods get_full_vector() and
     get_full_matrix() can be used.
     """
 
     def __init__(
         self,
         objective: ObjectiveBase,
-        lb: Union[np.ndarray, List[float]],
-        ub: Union[np.ndarray, List[float]],
+        lb: Union[np.ndarray, list[float]],
+        ub: Union[np.ndarray, list[float]],
         dim_full: Optional[int] = None,
         x_fixed_indices: Optional[SupportsIntIterableOrValue] = None,
         x_fixed_vals: Optional[SupportsFloatIterableOrValue] = None,
         x_guesses: Optional[Iterable[float]] = None,
         x_names: Optional[Iterable[str]] = None,
         x_scales: Optional[Iterable[str]] = None,
         x_priors_defs: Optional[NegLogParameterPriors] = None,
-        lb_init: Union[np.ndarray, List[float], None] = None,
-        ub_init: Union[np.ndarray, List[float], None] = None,
+        lb_init: Union[np.ndarray, list[float], None] = None,
+        ub_init: Union[np.ndarray, list[float], None] = None,
         copy_objective: bool = True,
         startpoint_method: Union[StartpointMethod, Callable, bool] = None,
     ):
         if copy_objective:
             objective = copy.deepcopy(objective)
         self.objective = objective
 
@@ -119,44 +118,44 @@
 
         self.dim_full: int = (
             dim_full if dim_full is not None else self.lb_full.size
         )
 
         if x_fixed_indices is None:
             x_fixed_indices = []
-        x_fixed_indices = _make_iterable_if_value(x_fixed_indices, 'int')
-        self.x_fixed_indices: List[int] = [
-            _type_conversion_with_check(idx, ix, 'fixed indices', 'int')
+        x_fixed_indices = _make_iterable_if_value(x_fixed_indices, "int")
+        self.x_fixed_indices: list[int] = [
+            _type_conversion_with_check(idx, ix, "fixed indices", "int")
             for idx, ix in enumerate(x_fixed_indices)
         ]
 
         # We want the fixed values to be a list, since we might need to add
         # or remove values during profile computation
         if x_fixed_vals is None:
             x_fixed_vals = []
-        x_fixed_vals = _make_iterable_if_value(x_fixed_vals, 'float')
-        self.x_fixed_vals: List[float] = [
-            _type_conversion_with_check(idx, x, 'fixed values', 'float')
+        x_fixed_vals = _make_iterable_if_value(x_fixed_vals, "float")
+        self.x_fixed_vals: list[float] = [
+            _type_conversion_with_check(idx, x, "fixed values", "float")
             for idx, x in enumerate(x_fixed_vals)
         ]
 
         if x_guesses is None:
             x_guesses = np.zeros((0, self.dim_full))
         self.x_guesses_full: np.ndarray = np.array(x_guesses)
 
         if x_names is None and objective.x_names is not None:
             x_names = objective.x_names
         elif x_names is None:
-            x_names = [f'x{j}' for j in range(0, self.dim_full)]
+            x_names = [f"x{j}" for j in range(0, self.dim_full)]
         if len(set(x_names)) != len(x_names):
             raise ValueError("Parameter names x_names must be unique")
-        self.x_names: List[str] = list(x_names)
+        self.x_names: list[str] = list(x_names)
 
         if x_scales is None:
-            x_scales = ['lin'] * self.dim_full
+            x_scales = ["lin"] * self.dim_full
         self.x_scales = x_scales
 
         self.x_priors = x_priors_defs
 
         self.normalize()
         self._check_x_guesses()
 
@@ -193,26 +192,26 @@
 
     @property
     def dim(self) -> int:
         """Return dimension only considering non fixed parameters."""
         return self.dim_full - len(self.x_fixed_indices)
 
     @property
-    def x_free_indices(self) -> List[int]:
+    def x_free_indices(self) -> list[int]:
         """Return non fixed parameters."""
         return sorted(set(range(0, self.dim_full)) - set(self.x_fixed_indices))
 
     def normalize(self) -> None:
         """
         Process vectors.
 
         Reduce all vectors to dimension dim and have the objective accept
         vectors of dimension dim.
         """
-        for attr in ['lb_full', 'lb_init_full', 'ub_full', 'ub_init_full']:
+        for attr in ["lb_full", "lb_init_full", "ub_full", "ub_init_full"]:
             value = self.__getattribute__(attr)
             if value.size == 1:
                 self.__setattr__(attr, value * np.ones(self.dim_full))
             elif value.size == self.dim:
                 # in this case the bounds only holds the values of the
                 # reduced bounds.
                 self.__setattr__(
@@ -244,19 +243,19 @@
         if len(self.x_names) != self.dim_full:
             raise AssertionError("x_names must be of length dim_full.")
         if len(self.x_fixed_indices) != len(self.x_fixed_vals):
             raise AssertionError(
                 "x_fixed_indices and x_fixed_vals must have the same length."
             )
         if np.isnan(self.lb).any():
-            raise ValueError('lb must not contain nan values')
+            raise ValueError("lb must not contain nan values")
         if np.isnan(self.ub).any():
-            raise ValueError('ub must not contain nan values')
+            raise ValueError("ub must not contain nan values")
         if np.any(self.lb >= self.ub):
-            raise ValueError('lb<ub not fulfilled.')
+            raise ValueError("lb<ub not fulfilled.")
 
     def _check_x_guesses(self):
         """Check whether the supplied x_guesses adhere to the bounds."""
         if self.x_guesses.size == 0:
             return
         adheres_ub = self.x_guesses <= self.ub
         adheres_lb = self.x_guesses >= self.lb
@@ -275,59 +274,59 @@
         Parameters
         ----------
         x_guesses:
         """
         x_guesses_full = np.array(x_guesses)
         if x_guesses_full.shape[1] != self.dim_full:
             raise ValueError(
-                'The dimension of individual x_guesses must be ' 'dim_full.'
+                "The dimension of individual x_guesses must be " "dim_full."
             )
         self.x_guesses_full = x_guesses_full
         self._check_x_guesses()
 
     def fix_parameters(
         self,
         parameter_indices: SupportsIntIterableOrValue,
         parameter_vals: SupportsFloatIterableOrValue,
     ) -> None:
         """Fix specified parameters to specified values."""
-        parameter_indices = _make_iterable_if_value(parameter_indices, 'int')
-        parameter_vals = _make_iterable_if_value(parameter_vals, 'float')
+        parameter_indices = _make_iterable_if_value(parameter_indices, "int")
+        parameter_vals = _make_iterable_if_value(parameter_vals, "float")
 
         # first clean to-be-fixed indices to avoid redundancies
         for iter_index, (x_index, x_value) in enumerate(
             zip(parameter_indices, parameter_vals)
         ):
             # check if parameter was already fixed, otherwise add it to the
             # fixed parameters
             index = _type_conversion_with_check(
-                iter_index, x_index, 'indices', 'int'
+                iter_index, x_index, "indices", "int"
             )
             val = _type_conversion_with_check(
-                iter_index, x_value, 'values', 'float'
+                iter_index, x_value, "values", "float"
             )
             if index in self.x_fixed_indices:
                 self.x_fixed_vals[self.x_fixed_indices.index(index)] = val
             else:
                 self.x_fixed_indices.append(index)
                 self.x_fixed_vals.append(val)
 
         self.normalize()
 
     def unfix_parameters(
         self, parameter_indices: SupportsIntIterableOrValue
     ) -> None:
         """Free specified parameters."""
         # check and adapt input
-        parameter_indices = _make_iterable_if_value(parameter_indices, 'int')
+        parameter_indices = _make_iterable_if_value(parameter_indices, "int")
 
         # first clean to-be-freed indices
         for iter_index, x_index in enumerate(parameter_indices):
             index = _type_conversion_with_check(
-                iter_index, x_index, 'indices', 'int'
+                iter_index, x_index, "indices", "int"
             )
             if index in self.x_fixed_indices:
                 fixed_x_index = self.x_fixed_indices.index(index)
                 self.x_fixed_indices.pop(fixed_x_index)
                 self.x_fixed_vals.pop(fixed_x_index)
 
         self.normalize()
@@ -390,15 +389,15 @@
         x_full[np.ix_(self.x_free_indices, self.x_free_indices)] = x
 
         return x_full
 
     def get_reduced_vector(
         self,
         x_full: Union[np.ndarray, None],
-        x_indices: Optional[List[int]] = None,
+        x_indices: Optional[list[int]] = None,
     ) -> Union[np.ndarray, None]:
         """
         Keep only those elements, which indices are specified in x_indices.
 
         If x_indices is not provided, delete fixed indices.
 
         Parameters
@@ -466,28 +465,28 @@
 
         Include what parameters are being optimized and parameter boundaries.
         """
         print(  # noqa: T201 (print)
             pd.DataFrame(
                 index=self.x_names,
                 data={
-                    'free': [
+                    "free": [
                         idx in self.x_free_indices
                         for idx in range(self.dim_full)
                     ],
-                    'lb_full': self.lb_full,
-                    'ub_full': self.ub_full,
+                    "lb_full": self.lb_full,
+                    "ub_full": self.ub_full,
                 },
             )
         )
 
 
 _convtypes = {
-    'float': {'attr': '__float__', 'conv': float},
-    'int': {'attr': '__int__', 'conv': int},
+    "float": {"attr": "__float__", "conv": float},
+    "int": {"attr": "__int__", "conv": int},
 }
 
 
 def _type_conversion_with_check(
     index: int,
     value: Union[SupportsFloat, SupportsInt],
     valuename: str,
@@ -495,39 +494,39 @@
 ) -> Union[float, int]:
     """
     Convert values to the requested type.
 
     Raises and appropriate error if not possible.
     """
     if convtype not in _convtypes:
-        raise ValueError(f'Unsupported type {convtype}')
+        raise ValueError(f"Unsupported type {convtype}")
 
-    can_convert = hasattr(value, _convtypes[convtype]['attr'])
+    can_convert = hasattr(value, _convtypes[convtype]["attr"])
     # this may fail for weird custom ypes that can be converted to int but
     # not float, but we probably don't want those as indiced anyways
-    lossless_conversion = not convtype == 'int' or (
-        hasattr(value, _convtypes['float']['attr'])
+    lossless_conversion = not convtype == "int" or (
+        hasattr(value, _convtypes["float"]["attr"])
         and (float(value) - int(value) == 0.0)
     )
 
     if not can_convert or not lossless_conversion:
         raise ValueError(
-            f'All {valuename} must support lossless conversion to {convtype}. '
-            f'Found type {type(value)} at index {index}, which cannot '
-            f'be converted to {convtype}.'
+            f"All {valuename} must support lossless conversion to {convtype}. "
+            f"Found type {type(value)} at index {index}, which cannot "
+            f"be converted to {convtype}."
         )
 
-    return _convtypes[convtype]['conv'](value)
+    return _convtypes[convtype]["conv"](value)
 
 
 def _make_iterable_if_value(
     value: Union[SupportsFloatIterableOrValue, SupportsIntIterableOrValue],
     convtype: str,
 ) -> Union[Iterable[SupportsFloat], Iterable[SupportsInt]]:
     """Convert scalar values to iterables for scalar input, may update type."""
     if convtype not in _convtypes:
-        raise ValueError(f'Unsupported type {convtype}')
+        raise ValueError(f"Unsupported type {convtype}")
 
-    if not hasattr(value, '__iter__'):
-        return [_type_conversion_with_check(0, value, 'values', convtype)]
+    if not hasattr(value, "__iter__"):
+        return [_type_conversion_with_check(0, value, "values", convtype)]
     else:
         return value
```

### Comparing `pypesto-0.4.2/pypesto/problem/hierarchical.py` & `pypesto-0.5.0/pypesto/problem/hierarchical.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
-from typing import Iterable, List, Optional, SupportsFloat, SupportsInt, Union
+from collections.abc import Iterable
+from typing import Optional, SupportsFloat, SupportsInt, Union
 
 import numpy as np
 
 from .base import Problem
 
 SupportsFloatIterableOrValue = Union[Iterable[SupportsFloat], SupportsFloat]
 SupportsIntIterableOrValue = Union[Iterable[SupportsInt], SupportsInt]
@@ -30,21 +31,26 @@
         hierarchical is True. Contains the names of easily interpretable
         inner parameters only, e.g. noise parameters, scaling factors, offsets.
     inner_lb, inner_ub:
         The lower and upper bounds for the inner optimization parameters.
         Only relevant if hierarchical is True. Contains the bounds of easily
         interpretable inner parameters only, e.g. noise parameters, scaling
         factors, offsets.
+    semiquant_observable_ids:
+        The ids of semiquantitative observables. Only relevant if hierarchical
+        is True. If not None, the optimization result's `spline_knots` will be
+        a list of lists of spline knots for each semiquantitative observable in
+        the order of these ids.
     """
 
     def __init__(
         self,
         inner_x_names: Optional[Iterable[str]] = None,
-        inner_lb: Optional[Union[np.ndarray, List[float]]] = None,
-        inner_ub: Optional[Union[np.ndarray, List[float]]] = None,
+        inner_lb: Optional[Union[np.ndarray, list[float]]] = None,
+        inner_ub: Optional[Union[np.ndarray, list[float]]] = None,
         **problem_kwargs: dict,
     ):
         super().__init__(**problem_kwargs)
 
         if inner_x_names is None:
             inner_x_names = (
                 self.objective.calculator.get_interpretable_inner_par_ids()
@@ -66,7 +72,11 @@
         if len(inner_lb) != len(inner_x_names):
             raise ValueError(
                 "Parameter bounds must have same length as parameter names"
             )
 
         self.inner_lb = np.array(inner_lb)
         self.inner_ub = np.array(inner_ub)
+
+        self.semiquant_observable_ids = (
+            self.objective.calculator.semiquant_observable_ids
+        )
```

### Comparing `pypesto-0.4.2/pypesto/profile/approximate.py` & `pypesto-0.5.0/pypesto/profile/approximate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Iterable
+from collections.abc import Iterable
 
 import numpy as np
 from scipy.stats import multivariate_normal
 
 from ..problem import Problem
 from ..result import ProfilerResult, Result
 from .util import initialize_profile
```

### Comparing `pypesto-0.4.2/pypesto/profile/options.py` & `pypesto-0.5.0/pypesto/profile/options.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Union
+from typing import Union
 
 
 class ProfileOptions(dict):
     """
     Options for optimization based profiling.
 
     Attributes
@@ -69,23 +69,23 @@
         self.validate()
 
     def __getattr__(self, key):
         """Allow usage of keys like attributes."""
         try:
             return self[key]
         except KeyError:
-            raise AttributeError(key)
+            raise AttributeError(key) from None
 
     __setattr__ = dict.__setitem__
     __delattr__ = dict.__delitem__
 
     @staticmethod
     def create_instance(
-        maybe_options: Union['ProfileOptions', Dict]
-    ) -> 'ProfileOptions':
+        maybe_options: Union["ProfileOptions", dict],
+    ) -> "ProfileOptions":
         """
         Return a valid options object.
 
         Parameters
         ----------
         maybe_options: ProfileOptions or dict
         """
```

### Comparing `pypesto-0.4.2/pypesto/profile/profile.py` & `pypesto-0.5.0/pypesto/profile/profile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import copy
 import logging
-from typing import Callable, Iterable, Union
+from collections.abc import Iterable
+from typing import Callable, Union
 
 from ..engine import Engine, SingleCoreEngine
 from ..optimize import Optimizer
 from ..problem import Problem
 from ..result import Result
 from ..store import autosave
 from .options import ProfileOptions
@@ -19,15 +20,15 @@
     problem: Problem,
     result: Result,
     optimizer: Optimizer,
     engine: Engine = None,
     profile_index: Iterable[int] = None,
     profile_list: int = None,
     result_index: int = 0,
-    next_guess_method: Union[Callable, str] = 'adaptive_step_regression',
+    next_guess_method: Union[Callable, str] = "adaptive_step_regression",
     profile_options: ProfileOptions = None,
     progress_bar: bool = None,
     filename: Union[str, Callable, None] = None,
     overwrite: bool = False,
 ) -> Result:
     """
     Compute parameter profiles.
@@ -113,19 +114,19 @@
                 current_profile_,
                 problem_,
                 global_opt_,
             )
 
     elif callable(next_guess_method):
         raise NotImplementedError(
-            'Passing function handles for computation of next '
-            'profiling point is not yet supported.'
+            "Passing function handles for computation of next "
+            "profiling point is not yet supported."
         )
     else:
-        raise ValueError('Unsupported input for next_guess_method.')
+        raise ValueError("Unsupported input for next_guess_method.")
 
     # create the profile result object (retrieve global optimum) or append to
     # existing list of profiles
     global_opt = initialize_profile(
         problem, result, result_index, profile_index, profile_list
     )
     # if engine==None set SingleCoreEngine() as default
@@ -162,16 +163,16 @@
 
     # execute the tasks with Engine
     indexed_profiles = engine.execute(tasks, progress_bar=progress_bar)
 
     # fill in the ProfilerResults at the right index
     for indexed_profile in indexed_profiles:
         result.profile_result.list[-1][
-            indexed_profile['index']
-        ] = indexed_profile['profile']
+            indexed_profile["index"]
+        ] = indexed_profile["profile"]
 
     autosave(
         filename=filename,
         result=result,
         store_type="profile",
         overwrite=overwrite,
     )
```

### Comparing `pypesto-0.4.2/pypesto/profile/profile_next_guess.py` & `pypesto-0.5.0/pypesto/profile/profile_next_guess.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 import numpy as np
 
 from ..problem import Problem
 from ..result import ProfilerResult
 from .options import ProfileOptions
 
-__all__ = ['next_guess', 'fixed_step', 'adaptive_step']
+__all__ = ["next_guess", "fixed_step", "adaptive_step"]
 
 
 def next_guess(
     x: np.ndarray,
     par_index: int,
     par_direction: Literal[1, -1],
     profile_options: ProfileOptions,
     update_type: Literal[
-        'fixed_step',
-        'adaptive_step_order_0',
-        'adaptive_step_order_1',
-        'adaptive_step_regression',
+        "fixed_step",
+        "adaptive_step_order_0",
+        "adaptive_step_order_1",
+        "adaptive_step_regression",
     ],
     current_profile: ProfilerResult,
     problem: Problem,
     global_opt: float,
 ) -> np.ndarray:
     """
     Create the next initial guess for the optimizer.
@@ -54,28 +54,28 @@
     global_opt:
         Log-posterior value of the global optimum.
 
     Returns
     -------
     The next initial guess as base for the next profile point.
     """
-    if update_type == 'fixed_step':
+    if update_type == "fixed_step":
         return fixed_step(
             x, par_index, par_direction, profile_options, problem
         )
 
-    if update_type == 'adaptive_step_order_0':
+    if update_type == "adaptive_step_order_0":
         order = 0
-    elif update_type == 'adaptive_step_order_1':
+    elif update_type == "adaptive_step_order_1":
         order = 1
-    elif update_type == 'adaptive_step_regression':
+    elif update_type == "adaptive_step_regression":
         order = np.nan
     else:
         raise ValueError(
-            f'Unsupported `update_type` {update_type} for `next_guess`.'
+            f"Unsupported `update_type` {update_type} for `next_guess`."
         )
 
     return adaptive_step(
         x,
         par_index,
         par_direction,
         profile_options,
@@ -433,46 +433,46 @@
     Returns
     -------
     Parameter vector that is expected to yield the objective function value
     closest to `next_obj_target`.
     """
     # Was the initial step too big or too small?
     direction = "decrease" if next_obj_target < next_obj else "increase"
-    if direction == 'increase':
+    if direction == "increase":
         adapt_factor = options.step_size_factor
     else:
         adapt_factor = 1 / options.step_size_factor
 
     # Loop until correct step size was found
     while True:
         # Adapt step size of guess
         last_x = next_x
         step_size_guess = clip_to_minmax(step_size_guess * adapt_factor)
         next_x = clip_to_bounds(par_extrapol(step_size_guess))
 
         # Check if we hit the bounds
         if (
-            direction == 'decrease'
+            direction == "decrease"
             and step_size_guess == options.min_step_size
         ):
             return next_x
         if (
-            direction == 'increase'
+            direction == "increase"
             and step_size_guess == options.max_step_size
         ):
             return next_x
 
         # compute new objective value
         problem.fix_parameters(par_index, next_x[par_index])
         last_obj = next_obj
         next_obj = problem.objective(problem.get_reduced_vector(next_x))
 
         # check for root crossing and compute correct step size in case
-        if (direction == 'decrease' and next_obj_target >= next_obj) or (
-            direction == 'increase' and next_obj_target <= next_obj
+        if (direction == "decrease" and next_obj_target >= next_obj) or (
+            direction == "increase" and next_obj_target <= next_obj
         ):
             return next_x_interpolate(
                 next_obj, last_obj, next_x, last_x, next_obj_target
             )
 
 
 def next_x_interpolate(
```

### Comparing `pypesto-0.4.2/pypesto/profile/task.py` & `pypesto-0.5.0/pypesto/profile/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def __init__(
         self,
         current_profile: ProfilerResult,
         problem: Problem,
         options: ProfileOptions,
         i_par: int,
         global_opt: float,
-        optimizer: 'pypesto.optimize.Optimizer',
+        optimizer: "pypesto.optimize.Optimizer",
         create_next_guess: Callable,
     ):
         """
         Create the task object.
 
         Parameters
         ----------
@@ -72,8 +72,8 @@
                 options=self.options,
                 create_next_guess=self.create_next_guess,
                 global_opt=self.global_opt,
                 i_par=self.i_par,
             )
 
         # return the ProfilerResult and the index of the parameter profiled
-        return {'profile': self.current_profile, 'index': self.i_par}
+        return {"profile": self.current_profile, "index": self.i_par}
```

### Comparing `pypesto-0.4.2/pypesto/profile/util.py` & `pypesto-0.5.0/pypesto/profile/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Utility function for profile module."""
 
-from typing import Any, Iterable
+from collections.abc import Iterable
+from typing import Any
 
 import numpy as np
 import scipy.stats
 
 from ..C import GRAD
 from ..problem import Problem
 from ..result import ProfileResult, ProfilerResult, Result
```

### Comparing `pypesto-0.4.2/pypesto/profile/validation_intervals.py` & `pypesto-0.5.0/pypesto/profile/validation_intervals.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.2/pypesto/profile/walk_along_profile.py` & `pypesto-0.5.0/pypesto/profile/walk_along_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
                 raise RuntimeError(
                     f"Computing profile point failed. Could not find a finite solution after {max_tries} attempts."
                 )
         else:
             # if too many parameters are fixed, there is nothing to do ...
             fval = problem.objective(np.array([]))
             optimizer_result = OptimizerResult(
-                id='0',
+                id="0",
                 x=np.array([]),
                 fval=fval,
                 n_fval=0,
                 n_grad=0,
                 n_res=0,
                 n_hess=0,
                 n_sres=0,
```

### Comparing `pypesto-0.4.2/pypesto/result/optimize.py` & `pypesto-0.5.0/pypesto/result/optimize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Optimization result."""
 
 import logging
 import warnings
 from collections import Counter
+from collections.abc import Sequence
 from copy import deepcopy
-from typing import Sequence, Union
+from typing import Union
 
 import numpy as np
 import pandas as pd
 
 from ..history import HistoryBase
 from ..problem import Problem
 from ..util import assign_clusters, delete_nan_inf
 
-OptimizationResult = Union['OptimizerResult', 'OptimizeResult']
+OptimizationResult = Union["OptimizerResult", "OptimizeResult"]
 logger = logging.getLogger(__name__)
 
 
 class OptimizerResult(dict):
     """
     The result of an optimizer run.
 
@@ -113,20 +114,21 @@
         self.history: HistoryBase = history
         self.exitflag: int = exitflag
         self.time: float = time
         self.message: str = message
         self.optimizer = optimizer
         self.free_indices = None
         self.inner_parameters = None
+        self.spline_knots = None
 
     def __getattr__(self, key):
         try:
             return self[key]
         except KeyError:
-            raise AttributeError(key)
+            raise AttributeError(key) from None
 
     __setattr__ = dict.__setitem__
     __delattr__ = dict.__delitem__
 
     def summary(self, full: bool = False, show_hess: bool = True) -> str:
         """
         Get summary of the object.
@@ -208,25 +210,25 @@
         return other
 
     def __getattr__(self, key):
         """Define `optimize_result.key`."""
         try:
             return [res[key] for res in self.list]
         except KeyError:
-            raise AttributeError(key)
+            raise AttributeError(key) from None
 
     def __getitem__(self, index):
         """Define `optimize_result[i]` to access the i-th result."""
         try:
             return self.list[index]
         except IndexError:
             raise IndexError(
                 f"{index} out of range for optimize result of "
                 f"length {len(self.list)}."
-            )
+            ) from None
 
     def __getstate__(self):
         # while we override __getattr__ as we do now, this is required to keep
         # instances pickle-able
         return vars(self)
 
     def __setstate__(self, state):
@@ -270,19 +272,19 @@
         )
         counter_message = message_counts_df[["Count", "Message"]].to_markdown(
             index=False
         )
         counter_message = "  " + counter_message.replace("\n", "\n  ")
 
         times_message = (
-            f'\t* Mean execution time: {np.mean(self.time):0.3f}s\n'
-            f'\t* Maximum execution time: {np.max(self.time):0.3f}s,'
-            f'\tid={self[np.argmax(self.time)].id}\n'
-            f'\t* Minimum execution time: {np.min(self.time):0.3f}s,\t'
-            f'id={self[np.argmin(self.time)].id}'
+            f"\t* Mean execution time: {np.mean(self.time):0.3f}s\n"
+            f"\t* Maximum execution time: {np.max(self.time):0.3f}s,"
+            f"\tid={self[np.argmax(self.time)].id}\n"
+            f"\t* Minimum execution time: {np.min(self.time):0.3f}s,\t"
+            f"id={self[np.argmin(self.time)].id}"
         )
 
         # special handling in case there are only non-finite fvals
         num_best_value = int(clustsize[0]) if len(clustsize) else len(self)
         num_plateaus = (
             (1 + max(clust) - sum(clustsize == 1)) if len(clustsize) else 0
         )
@@ -311,15 +313,15 @@
             )
         return summary
 
     def append(
         self,
         optimize_result: OptimizationResult,
         sort: bool = True,
-        prefix: str = '',
+        prefix: str = "",
     ):
         """
         Append an OptimizerResult or an OptimizeResult to the result object.
 
         Parameters
         ----------
         optimize_result:
@@ -406,15 +408,17 @@
         return lst
 
     def get_for_key(self, key) -> list:
         """Extract the list of values for the specified key as a list."""
         warnings.warn(
             "get_for_key() is deprecated in favour of "
             "optimize_result.key and will be removed in future "
-            "releases."
+            "releases.",
+            DeprecationWarning,
+            stacklevel=1,
         )
         return [res[key] for res in self.list]
 
     def get_by_id(self, ores_id: str):
         """Get OptimizationResult with the specified id."""
         for res in self.list:
             if res.id == ores_id:
```

### Comparing `pypesto-0.4.2/pypesto/result/predict.py` & `pypesto-0.5.0/pypesto/result/predict.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """PredictionResult and PredictionConditionResult."""
 
 import os
+from collections.abc import Sequence
 from pathlib import Path
 from time import time
-from typing import Dict, Sequence, Union
+from typing import Union
 from warnings import warn
 
 import h5py
 import numpy as np
 import pandas as pd
 
 from ..C import (
@@ -68,26 +69,26 @@
         self.output = output
         self.output_sensi = output_sensi
         self.output_weight = output_weight
         self.output_sigmay = output_sigmay
         self.x_names = x_names
         if x_names is None and output_sensi is not None:
             self.x_names = [
-                f'parameter_{i_par}' for i_par in range(output_sensi.shape[1])
+                f"parameter_{i_par}" for i_par in range(output_sensi.shape[1])
             ]
 
     def __iter__(self):
         """Allow usage like a dict."""
-        yield 'timepoints', self.timepoints
-        yield 'output_ids', self.output_ids
-        yield 'x_names', self.x_names
-        yield 'output', self.output
-        yield 'output_sensi', self.output_sensi
-        yield 'output_weight', self.output_weight
-        yield 'output_sigmay', self.output_sigmay
+        yield "timepoints", self.timepoints
+        yield "output_ids", self.output_ids
+        yield "x_names", self.x_names
+        yield "output", self.output
+        yield "output_sensi", self.output_sensi
+        yield "output_weight", self.output_weight
+        yield "output_sigmay", self.output_sigmay
 
     def __eq__(self, other):
         """Check equality of two PredictionConditionResults."""
 
         def to_bool(expr):
             if isinstance(expr, bool):
                 return expr
@@ -118,15 +119,15 @@
     should be stored, read, and handled: as predictions are a very flexible
     format anyway, they should at least have a common definition,
     which allows to work with them in a reasonable way.
     """
 
     def __init__(
         self,
-        conditions: Sequence[Union[PredictionConditionResult, Dict]],
+        conditions: Sequence[Union[PredictionConditionResult, dict]],
         condition_ids: Sequence[str] = None,
         comment: str = None,
     ):
         """
         Initialize PredictionResult.
 
         Parameters
@@ -162,18 +163,18 @@
 
     def __iter__(self):
         """Allow usage like an iterator."""
         parameter_ids = None
         if self.conditions:
             parameter_ids = self.conditions[0].x_names
 
-        yield 'conditions', [dict(cond) for cond in self.conditions]
-        yield 'condition_ids', self.condition_ids
-        yield 'comment', self.comment
-        yield 'parameter_ids', parameter_ids
+        yield "conditions", [dict(cond) for cond in self.conditions]
+        yield "condition_ids", self.condition_ids
+        yield "comment", self.comment
+        yield "parameter_ids", parameter_ids
 
     def __eq__(self, other):
         """Check equality of two PredictionResults."""
         if not isinstance(other, PredictionResult):
             return False
         if self.comment != other.comment:
             return False
@@ -202,68 +203,68 @@
             with a suiting name: csv's are by default 2-dimensional, but the
             output will have the format n_conditions x n_timepoints x n_outputs
             For sensitivities, we even have x n_parameters. This makes it
             necessary to create multiple files and hence, a folder of its own
             makes sense. Returns a pathlib.Path object of the output.
             """
             # allow entering with names with and without file type endings
-            if '.' in output_file:
-                output_path, output_suffix = output_file.split('.')
+            if "." in output_file:
+                output_path, output_suffix = output_file.split(".")
             else:
                 output_path = output_file
                 output_suffix = CSV
 
             # parse path and check whether the file exists
             output_path = Path(output_path)
             output_path = self._check_existence(output_path)
 
             # create
             output_path.mkdir(parents=True, exist_ok=False)
             # add the suffix
             output_dummy = Path(output_path.stem).with_suffix(
-                f'.{output_suffix}'
+                f".{output_suffix}"
             )
 
             return output_path, output_dummy
 
         # process the name of the output file, create a folder
         output_path, output_dummy = _prepare_csv_output(output_file)
 
         # loop over conditions (i.e., amici edata objects)
         for i_cond, cond in enumerate(self.conditions):
             timepoints = pd.Series(name=TIME, data=cond.timepoints)
             # handle outputs, if computed
             if cond.output is not None:
                 # create filename for this condition
                 filename = output_path.joinpath(
-                    output_dummy.stem + f'_{i_cond}' + output_dummy.suffix
+                    output_dummy.stem + f"_{i_cond}" + output_dummy.suffix
                 )
                 # create DataFrame and write to file
                 result = pd.DataFrame(
                     index=timepoints, columns=cond.output_ids, data=cond.output
                 )
-                result.to_csv(filename, sep='\t')
+                result.to_csv(filename, sep="\t")
 
             # handle output sensitivities, if computed
             if cond.output_sensi is not None:
                 # loop over parameters
                 for i_par in range(cond.output_sensi.shape[1]):
                     # create filename for this condition and parameter
                     filename = output_path.joinpath(
                         output_dummy.stem
-                        + f'_{i_cond}__s{i_par}'
+                        + f"_{i_cond}__s{i_par}"
                         + output_dummy.suffix
                     )
                     # create DataFrame and write to file
                     result = pd.DataFrame(
                         index=timepoints,
                         columns=cond.output_ids,
                         data=cond.output_sensi[:, i_par, :],
                     )
-                    result.to_csv(filename, sep='\t')
+                    result.to_csv(filename, sep="\t")
 
     def write_to_h5(self, output_file: str, base_path: str = None):
         """
         Save predictions to an h5 file.
 
         It appends to the file if the file already exists.
 
@@ -272,19 +273,19 @@
         output_file:
             path to file/folder to which results will be written
         base_path:
             base path in the h5 file
         """
         # check if the file exists and append to it in case it does
         output_path = Path(output_file)
-        filemode = 'w'
+        filemode = "w"
         if os.path.exists(output_path):
-            filemode = 'r+'
+            filemode = "r+"
 
-        base = Path('.')
+        base = Path(".")
         if base_path is not None:
             base = Path(base_path)
 
         with h5py.File(output_path, filemode) as f:
             # loop over conditions (i.e., amici edata objects)
             if self.conditions and self.conditions[0].x_names is not None:
                 f.create_dataset(
@@ -335,15 +336,16 @@
         Check whether a file or a folder already exists.
 
         Append a timestamp if this is the case.
         """
         output_path_out = output_path
         while output_path_out.exists():
             output_path_out = output_path_out.with_name(
-                output_path_out.stem + f'_{round(time() * 1000)}'
+                output_path_out.stem + f"_{round(time() * 1000)}"
             )
             warn(
-                'Output name already existed! Changed the name of the output '
-                'by appending the unix timestampp to make it unique!'
+                "Output name already existed! Changed the name of the output "
+                "by appending the unix timestamp to make it unique!",
+                stacklevel=3,
             )
 
         return output_path_out
```

### Comparing `pypesto-0.4.2/pypesto/result/profile.py` & `pypesto-0.5.0/pypesto/result/profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         self.message = message
 
     def __getattr__(self, key):
         """Allow usage of keys like attributes."""
         try:
             return self[key]
         except KeyError:
-            raise AttributeError(key)
+            raise AttributeError(key) from None
 
     __setattr__ = dict.__setitem__
     __delattr__ = dict.__delitem__
 
     def append_profile_point(
         self,
         x: np.ndarray,
```

### Comparing `pypesto-0.4.2/pypesto/result/result.py` & `pypesto-0.5.0/pypesto/result/result.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.2/pypesto/result/sample.py` & `pypesto-0.5.0/pypesto/result/sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Sampling result."""
 
-from typing import Iterable
+from collections.abc import Iterable
 
 import numpy as np
 
 
 class McmcPtResult(dict):
     """
     The result of a sampler run using Markov-chain Monte Carlo.
@@ -101,15 +101,15 @@
             )  # noqa
 
     def __getattr__(self, key):
         """Allow usage of keys like attributes."""
         try:
             return self[key]
         except KeyError:
-            raise AttributeError(key)
+            raise AttributeError(key) from None
 
     __setattr__ = dict.__setitem__
     __delattr__ = dict.__delitem__
 
 
 class SampleResult:
     """Result of the sample() function."""
```

### Comparing `pypesto-0.4.2/pypesto/sample/__init__.py` & `pypesto-0.5.0/pypesto/sample/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.2/pypesto/sample/adaptive_metropolis.py` & `pypesto-0.5.0/pypesto/sample/adaptive_metropolis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numbers
-from typing import Dict, Tuple
 
 import numpy as np
 
 from ..problem import Problem
 from .metropolis import MetropolisSampler
 
 
@@ -53,73 +52,73 @@
 
     For reference matlab implementations see:
 
     * https://github.com/ICB-DCM/PESTO/blob/master/private/performPT.m
     * https://github.com/ICB-DCM/PESTO/blob/master/private/updateStatistics.m
     """
 
-    def __init__(self, options: Dict = None):
+    def __init__(self, options: dict = None):
         super().__init__(options)
         self._cov = None
         self._mean_hist = None
         self._cov_hist = None
         self._cov_scale = None
 
     @classmethod
     def default_options(cls):
         """Return the default options for the sampler."""
         return {
             # controls adaptation degeneration velocity of the proposals
             # in [0, 1], with 0 -> no adaptation, i.e. classical
             # Metropolis-Hastings
-            'decay_constant': 0.51,
+            "decay_constant": 0.51,
             # number of samples before adaptation decreases significantly.
             # a higher value reduces the impact of early adaptation
-            'threshold_sample': 1,
+            "threshold_sample": 1,
             # regularization factor for ill-conditioned cov matrices of
             # the adapted proposal density. regularization might happen if the
             # eigenvalues of the cov matrix strongly differ in order
             # of magnitude. in this case, the algorithm adds a small
             # diag matrix to the cov matrix with elements of this factor
-            'reg_factor': 1e-6,
+            "reg_factor": 1e-6,
             # initial covariance matrix. defaults to a unit matrix
-            'cov0': None,
+            "cov0": None,
             # target acceptance rate
-            'target_acceptance_rate': 0.234,
+            "target_acceptance_rate": 0.234,
             # show progress
-            'show_progress': None,
+            "show_progress": None,
         }
 
     def initialize(self, problem: Problem, x0: np.ndarray):
         """Initialize the sampler."""
         super().initialize(problem, x0)
 
-        if self.options['cov0'] is not None:
-            cov0 = self.options['cov0']
+        if self.options["cov0"] is not None:
+            cov0 = self.options["cov0"]
             if isinstance(cov0, numbers.Real):
                 cov0 = float(cov0) * np.eye(len(x0))
         else:
             cov0 = np.eye(len(x0))
-        self._cov = regularize_covariance(cov0, self.options['reg_factor'])
+        self._cov = regularize_covariance(cov0, self.options["reg_factor"])
         self._mean_hist = self.trace_x[-1]
         self._cov_hist = self._cov
         self._cov_scale = 1.0
 
     def _propose_parameter(self, x: np.ndarray):
         x_new = np.random.multivariate_normal(x, self._cov)
         return x_new
 
     def _update_proposal(
         self, x: np.ndarray, lpost: float, log_p_acc: float, n_sample_cur: int
     ):
         # parse options
-        decay_constant = self.options['decay_constant']
-        threshold_sample = self.options['threshold_sample']
-        reg_factor = self.options['reg_factor']
-        target_acceptance_rate = self.options['target_acceptance_rate']
+        decay_constant = self.options["decay_constant"]
+        threshold_sample = self.options["threshold_sample"]
+        reg_factor = self.options["reg_factor"]
+        target_acceptance_rate = self.options["target_acceptance_rate"]
 
         # compute historical mean and covariance
         self._mean_hist, self._cov_hist = update_history_statistics(
             mean=self._mean_hist,
             cov=self._cov_hist,
             x_new=x,
             n_cur_sample=max(n_sample_cur + 1, threshold_sample),
@@ -142,15 +141,15 @@
 
 def update_history_statistics(
     mean: np.ndarray,
     cov: np.ndarray,
     x_new: np.ndarray,
     n_cur_sample: int,
     decay_constant: float,
-) -> Tuple[np.ndarray, np.ndarray]:
+) -> tuple[np.ndarray, np.ndarray]:
     """Update sampling mean and covariance matrix via weighted average.
 
     Update sampling mean and covariance matrix based on the previous
     estimate and the most recent sample via a weighted average,
     with gradually decaying update rate.
 
     Parameters
```

### Comparing `pypesto-0.4.2/pypesto/sample/auto_correlation.py` & `pypesto-0.5.0/pypesto/sample/auto_correlation.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     Returns
     -------
         tau_est: An estimate of the integrated autocorrelation time of
         the MCMC chain.
     """
     nsamples, npar = chain.shape
-    tau_est = np.zeros((npar))
+    tau_est = np.zeros(npar)
 
     # Calculate the fast Fourier transform
     x = np.fft.fft(chain, axis=0)
     # Get the real part
     xr = np.real(x)
     # Get the imaginary part
     xi = np.imag(x)
```

### Comparing `pypesto-0.4.2/pypesto/sample/diagnostics.py` & `pypesto-0.5.0/pypesto/sample/diagnostics.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,43 +7,48 @@
 from ..result import Result
 from .auto_correlation import autocorrelation_sokal
 from .geweke_test import burn_in_by_sequential_geweke
 
 logger = logging.getLogger(__name__)
 
 
-def geweke_test(result: Result, zscore: float = 2.0) -> int:
+def geweke_test(
+    result: Result, zscore: float = 2.0, chain_number: int = 0
+) -> int:
     """
     Calculate the burn-in of MCMC chains.
 
     Parameters
     ----------
     result:
         The pyPESTO result object with filled sample result.
     zscore:
         The Geweke test threshold.
+    chain_number:
+        The chain number to be used for the Geweke test (in a parallel tempering setting).
+        Usually we are only interested in the first chain.
 
     Returns
     -------
     burn_in:
         Iteration where the first and the last fraction of the chain
         do not differ significantly regarding Geweke test -> Burn-In
-
     """
     # Get parameter samples as numpy arrays
-    chain = np.asarray(result.sample_result.trace_x[0])
+    chain = np.asarray(result.sample_result.trace_x[chain_number])
 
     # Calculate burn in index
     burn_in = burn_in_by_sequential_geweke(chain=chain, zscore=zscore)
 
-    # Log
-    logger.info(f'Geweke burn-in index: {burn_in}')
+    if chain_number == 0:
+        # Log
+        logger.info(f"Geweke burn-in index: {burn_in}")
 
-    # Fill in burn-in value into result
-    result.sample_result.burn_in = burn_in
+        # Fill in burn-in value into result
+        result.sample_result.burn_in = burn_in
 
     return burn_in
 
 
 def auto_correlation(result: Result) -> float:
     """
     Calculate the autocorrelation of the MCMC chains.
@@ -85,15 +90,15 @@
     # Calculate autocorrelation
     auto_correlation_vector = autocorrelation_sokal(chain=chain)
 
     # Take the maximum over all components
     _auto_correlation = max(auto_correlation_vector)
 
     # Log
-    logger.info(f'Estimated chain autocorrelation: {_auto_correlation}')
+    logger.info(f"Estimated chain autocorrelation: {_auto_correlation}")
 
     # Fill in autocorrelation value into result
     result.sample_result.auto_correlation = _auto_correlation
 
     return _auto_correlation
 
 
@@ -132,13 +137,13 @@
     # Get length of the converged chain
     N = chain.shape[0]
 
     # Calculate effective sample size
     ess = N / (1 + _auto_correlation)
 
     # Log
-    logger.info(f'Estimated effective sample size: {ess}')
+    logger.info(f"Estimated effective sample size: {ess}")
 
     # Fill in effective sample size value into result
     result.sample_result.effective_sample_size = ess
 
     return ess
```

### Comparing `pypesto-0.4.2/pypesto/sample/dynesty.py` & `pypesto-0.5.0/pypesto/sample/dynesty.py`

 * *Files 25% similar despite different names*

```diff
@@ -21,36 +21,48 @@
 #        - need to provide gradients, hopefully without additional obj call
 #        - or use `compute_jac` option, probably expensive
 #      - multivariate slice for large problems (D > 20) without gradients
 # TODO consider reflective boundaries
 
 from __future__ import annotations
 
+import importlib
 import logging
-from typing import List, Union
+import warnings
 
+import cloudpickle  # noqa: S403
 import numpy as np
 
+from ..C import OBJECTIVE_NEGLOGLIKE, OBJECTIVE_NEGLOGPOST
 from ..problem import Problem
 from ..result import McmcPtResult
 from .sampler import Sampler, SamplerImportError
 
+dynesty_pickle = cloudpickle
+if importlib.util.find_spec("dynesty") is None:
+    dynesty = type("", (), {})()
+    dynesty.results = type("", (), {})()
+    dynesty.results.Results = None
+else:
+    import dynesty
+
+    dynesty.utils.pickle_module = dynesty_pickle
 logger = logging.getLogger(__name__)
 
 
 class DynestySampler(Sampler):
     """Use dynesty for sampling.
 
     NB: `get_samples` returns MCMC-like samples, by resampling original
     `dynesty` samples according to their importance weights. This is because
     the original samples contain many low-likelihood samples.
     To work with the original samples, modify the results object with
     `pypesto_result.sample_result = sampler.get_original_samples()`, where
     `sampler` is an instance of `pypesto.sample.DynestySampler`. The original
-    dynesty results object is available at `sampler.results`.
+    dynesty results object is available at `sampler.raw_results`.
 
     NB: the dynesty samplers can be customized significantly, by providing
     `sampler_args` and `run_args` to your `pypesto.sample.DynestySampler()`
     call. For example, code to parallelize dynesty is provided in pyPESTO's
     `sampler_study.ipynb` notebook.
 
     Wrapper around https://dynesty.readthedocs.io/en/stable/, see there for
@@ -58,66 +70,74 @@
     """
 
     def __init__(
         self,
         sampler_args: dict = None,
         run_args: dict = None,
         dynamic: bool = True,
+        objective_type: str = OBJECTIVE_NEGLOGPOST,
     ):
         """
         Initialize sampler.
 
         Parameters
         ----------
         sampler_args:
             Further keyword arguments that are passed on to the `__init__`
             method of the dynesty sampler.
         run_args:
             Further keyword arguments that are passed on to the `run_nested`
             method of the dynesty sampler.
         dynamic:
             Whether to use dynamic or static nested sampling.
+        objective_type:
+            The objective to optimize (as defined in `pypesto.problem`). Either
+            `pypesto.C.OBJECTIVE_NEGLOGLIKE` or
+            `pypesto.C.OBJECTIVE_NEGLOGPOST`. If
+            `pypesto.C.OBJECTIVE_NEGLOGPOST`, then `x_priors` have to
+            be defined in the problem.
         """
-        # check dependencies
-        import dynesty
-
-        setup_dynesty()
+        if importlib.util.find_spec("dynesty") is None:
+            raise SamplerImportError("dynesty")
 
         super().__init__()
 
         self.dynamic = dynamic
 
         if sampler_args is None:
             sampler_args = {}
         self.sampler_args: dict = sampler_args
 
         if run_args is None:
             run_args = {}
         self.run_args: dict = run_args
 
+        if objective_type not in [OBJECTIVE_NEGLOGPOST, OBJECTIVE_NEGLOGLIKE]:
+            raise ValueError(
+                f"Objective has to be either '{OBJECTIVE_NEGLOGPOST}' or '{OBJECTIVE_NEGLOGLIKE}' "
+                f"as defined in pypesto.problem."
+            )
+        self.objective_type = objective_type
+
         # set in initialize
-        self.problem: Union[Problem, None] = None
-        self.sampler: Union[
-            dynesty.DynamicNestedSampler,
-            dynesty.NestedSampler,
-            None,
-        ] = None
+        self.problem: Problem | None = None
+        self.sampler: (
+            dynesty.DynamicNestedSampler | dynesty.NestedSampler | None
+        ) = None
 
     def prior_transform(self, prior_sample: np.ndarray) -> np.ndarray:
         """Transform prior sample from unit cube to pyPESTO prior.
 
         TODO support priors that are not uniform.
              raise warning in `self.initialize` for now.
 
         Parameters
         ----------
         prior_sample:
             The prior sample, provided by dynesty.
-        problem:
-            The pyPESTO problem.
 
         Returns
         -------
         The transformed prior sample.
         """
         return (
             prior_sample * (self.problem.ub - self.problem.lb)
@@ -126,33 +146,57 @@
 
     def loglikelihood(self, x):
         """Log-probability density function."""
         # check if parameter lies within bounds
         if any(x < self.problem.lb) or any(x > self.problem.ub):
             return -np.inf
         # invert sign
-        # TODO this is possibly the posterior if priors are defined
+        if self.objective_type == OBJECTIVE_NEGLOGPOST:
+            # problem.objective returns negative log-posterior
+            # compute log-likelihood by subtracting log-prior
+            return -1.0 * (
+                self.problem.objective(x) - self.problem.x_priors(x)
+            )
+        # problem.objective returns negative log-likelihood
         return -1.0 * self.problem.objective(x)
 
     def initialize(
         self,
         problem: Problem,
-        x0: Union[np.ndarray, List[np.ndarray]],
+        x0: np.ndarray | list[np.ndarray] = None,
     ) -> None:
         """Initialize the sampler."""
-        import dynesty
-
-        setup_dynesty()
-
         self.problem = problem
 
         sampler_class = dynesty.NestedSampler
         if self.dynamic:
             sampler_class = dynesty.DynamicNestedSampler
 
+        # check if objective fits to the pyPESTO problem
+        if self.objective_type == OBJECTIVE_NEGLOGPOST:
+            if self.problem.x_priors is None:
+                # objective is the negative log-posterior, but no priors are defined
+                # sampler needs the likelihood
+                raise ValueError(
+                    f"x_priors have to be defined in the problem if objective is '{OBJECTIVE_NEGLOGPOST}'."
+                )
+        else:
+            # if objective is the negative log likelihood, we will ignore x_priors even if they are defined
+            if self.problem.x_priors is not None:
+                logger.warning(
+                    f"Assuming '{OBJECTIVE_NEGLOGLIKE}' as objective. "
+                    f"'x_priors' defined in the problem will be ignored."
+                )
+
+        # if priors are uniform, we can use the default prior transform (assuming that bounds are set correctly)
+        logger.warning(
+            "Assuming 'prior_transform' is correctly specified. If 'x_priors' is not uniform, 'prior_transform'"
+            " has to be adjusted accordingly."
+        )
+
         # initialize sampler
         self.sampler = sampler_class(
             loglikelihood=self.loglikelihood,
             prior_transform=self.prior_transform,
             ndim=len(self.problem.x_free_indices),
             **self.sampler_args,
         )
@@ -170,85 +214,158 @@
         if beta is not None:
             logger.warning(
                 "The temperature of a `dynesty` sampler was set, but this is "
                 "irrelevant for `dynesty` samplers."
             )
 
         self.sampler.run_nested(**self.run_args)
-        self.results = self.sampler.results
+
+    @property
+    def results(self):
+        """Deprecated in favor of `raw_results`."""
+        warnings.warn(
+            "Accessing dynesty results via `sampler.results` is "
+            "deprecated. Please use `sampler.raw_results` instead.",
+            DeprecationWarning,
+            stacklevel=1,
+        )
+        return self.raw_results
+
+    @property
+    def raw_results(self):
+        """Get the raw dynesty results."""
+        return self.sampler.results
 
     def save_internal_sampler(self, filename: str) -> None:
         """Save the state of the internal dynesty sampler.
 
         This makes it easier to analyze the original dynesty samples, after
         sampling, with `restore_internal`.
 
         Parameters
         ----------
         filename:
             The internal sampler will be saved here.
         """
-        import dynesty
-
-        setup_dynesty()
-
         dynesty.utils.save_sampler(
             sampler=self.sampler,
             fname=filename,
         )
 
     def restore_internal_sampler(self, filename: str) -> None:
         """Restore the state of the internal dynesty sampler.
 
         Parameters
         ----------
         filename:
             The internal sampler will be saved here.
         """
-        import dynesty
-
-        setup_dynesty()
-
-        self.sampler = dynesty.utils.restore_sampler(fname=filename)
+        pool = self.sampler_args.get("pool", None)
+        self.sampler = dynesty.utils.restore_sampler(
+            fname=filename,
+            pool=pool,
+        )
 
     def get_original_samples(self) -> McmcPtResult:
         """Get the samples into the fitting pypesto format.
 
         Returns
         -------
         The pyPESTO sample result.
         """
-        return get_original_dynesty_samples(sampler=self.sampler)
+        return get_original_dynesty_samples(sampler=self)
 
     def get_samples(self) -> McmcPtResult:
         """Get MCMC-like samples into the fitting pypesto format.
 
         Returns
         -------
         The pyPESTO sample result.
         """
-        return get_mcmc_like_dynesty_samples(sampler=self.sampler)
+        return get_mcmc_like_dynesty_samples(sampler=self)
 
 
-def get_original_dynesty_samples(sampler) -> McmcPtResult:
+def _get_raw_results(
+    sampler: DynestySampler,
+    raw_results: dynesty.result.Results,
+) -> dynesty.results.Results:
+    if (sampler is None) == (raw_results is None):
+        raise ValueError(
+            "Please supply exactly one of `sampler` or `raw_results`."
+        )
+
+    if raw_results is not None:
+        return raw_results
+
+    if not isinstance(sampler, DynestySampler):
+        raise ValueError(
+            "Please provide a pyPESTO `DynestySampler` if using "
+            "the `sampler` argument of this method."
+        )
+
+    return sampler.raw_results
+
+
+def save_raw_results(sampler: DynestySampler, filename: str) -> None:
+    """Save dynesty sampler results to file.
+
+    Restoring the dynesty sampler on a different computer than the one that
+    samples were generated is problematic (e.g. an AMICI model might get
+    compiled automatically). This method should avoid that, by only saving
+    the results.
+
+    Parameters
+    ----------
+    sampler:
+        The pyPESTO `DynestySampler` object used during sampling.
+    filename:
+        The file where the results will be saved.
+    """
+    raw_results = _get_raw_results(sampler=sampler, raw_results=None)
+    with open(filename, "wb") as f:
+        dynesty_pickle.dump(raw_results, f)
+
+
+def load_raw_results(filename: str) -> dynesty.results.Results:
+    """Load dynesty sample results from file.
+
+    Parameters
+    ----------
+    filename:
+        The file where the results will be loaded from.
+    """
+    with open(filename, "rb") as f:
+        raw_results = dynesty_pickle.load(f)
+    return raw_results
+
+
+def get_original_dynesty_samples(
+    sampler: DynestySampler = None,
+    raw_results: dynesty.results.Results = None,
+) -> McmcPtResult:
     """Get original dynesty samples.
 
+    Only one of `sampler` or `raw_results` should be provided.
+
     Parameters
     ----------
     sampler:
-        The (internal!) dynesty sampler. See
-        `pypesto.sample.DynestySampler.__init__`, specifically the
-        `save_internal` argument, for more details.
+        The pyPESTO `DynestySampler` object with sampling results.
+    raw_results:
+        The raw results. See :func:`save_raw_results` and
+        :func:`load_raw_results`.
 
     Returns
     -------
     The sample result.
     """
-    trace_x = np.array([sampler.results.samples])
-    trace_neglogpost = -np.array([sampler.results.logl])
+    raw_results = _get_raw_results(sampler=sampler, raw_results=raw_results)
+
+    trace_x = np.array([raw_results.samples])
+    trace_neglogpost = -np.array([raw_results.logl])
 
     # the sampler uses custom adaptive priors
     trace_neglogprior = np.full(trace_neglogpost.shape, np.nan)
     # the sampler uses temperature 1
     betas = np.array([1.0])
 
     result = McmcPtResult(
@@ -257,59 +374,52 @@
         trace_neglogprior=trace_neglogprior,
         betas=betas,
     )
 
     return result
 
 
-def get_mcmc_like_dynesty_samples(sampler) -> McmcPtResult:
+def get_mcmc_like_dynesty_samples(
+    sampler: DynestySampler = None,
+    raw_results: dynesty.results.Results = None,
+) -> McmcPtResult:
     """Get MCMC-like samples.
 
+    Only one of `sampler` or `raw_results` should be provided.
+
     Parameters
     ----------
     sampler:
-        The (internal!) dynesty sampler. See
-        `pypesto.sample.DynestySampler.__init__`, specifically the
-        `save_internal` argument, for more details.
+        The pyPESTO `DynestySampler` object with sampling results.
+    raw_results:
+        The raw results. See :func:`save_raw_results` and
+        :func:`load_raw_results`.
 
     Returns
     -------
     The sample result.
     """
-    import dynesty
+    raw_results = _get_raw_results(sampler=sampler, raw_results=raw_results)
 
-    setup_dynesty()
-
-    if len(sampler.results.importance_weights().shape) != 1:
+    if len(raw_results.importance_weights().shape) != 1:
         raise ValueError(
             "Unknown error. The dynesty importance weights are not a 1D array."
         )
     # resample according to importance weights
     indices = dynesty.utils.resample_equal(
-        np.arange(sampler.results.importance_weights().shape[0]),
-        sampler.results.importance_weights(),
+        np.arange(raw_results.importance_weights().shape[0]),
+        raw_results.importance_weights(),
     )
 
-    trace_x = np.array([sampler.results.samples[indices]])
-    trace_neglogpost = -np.array([sampler.results.logl[indices]])
+    trace_x = np.array([raw_results.samples[indices]])
+    trace_neglogpost = -np.array([raw_results.logl[indices]])
 
     trace_neglogprior = np.array([np.full((len(indices),), np.nan)])
     betas = np.array([1.0])
 
     result = McmcPtResult(
         trace_x=trace_x,
         trace_neglogpost=trace_neglogpost,
         trace_neglogprior=trace_neglogprior,
         betas=betas,
     )
     return result
-
-
-def setup_dynesty() -> None:
-    """Import dynesty."""
-    try:
-        import cloudpickle  # noqa: S403
-        import dynesty.utils
-
-        dynesty.utils.pickle_module = cloudpickle
-    except ImportError:
-        raise SamplerImportError("dynesty")
```

### Comparing `pypesto-0.4.2/pypesto/sample/emcee.py` & `pypesto-0.5.0/pypesto/sample/emcee.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """EmceeSampler class."""
 
 from __future__ import annotations
 
 import logging
-from typing import List, Union
 
 import numpy as np
 
 from ..problem import Problem
 from ..result import McmcPtResult
 from ..startpoint import UniformStartpoints, uniform
 from .sampler import Sampler, SamplerImportError
@@ -42,31 +41,31 @@
             Further keyword arguments that are passed on to
             ``emcee.EnsembleSampler.run_mcmc``.
         """
         # check dependencies
         try:
             import emcee
         except ImportError:
-            raise SamplerImportError("emcee")
+            raise SamplerImportError("emcee") from None
 
         super().__init__()
         self.nwalkers: int = nwalkers
 
         if sampler_args is None:
             sampler_args = {}
         self.sampler_args: dict = sampler_args
 
         if run_args is None:
             run_args = {}
         self.run_args: dict = run_args
 
         # set in initialize
-        self.problem: Union[Problem, None] = None
-        self.sampler: Union[emcee.EnsembleSampler, None] = None
-        self.state: Union[emcee.State, None] = None
+        self.problem: Problem | None = None
+        self.sampler: emcee.EnsembleSampler | None = None
+        self.state: emcee.State | None = None
 
     def get_epsilon_ball_initial_state(
         self,
         center: np.ndarray,
         problem: Problem,
         epsilon: float = 1e-3,
     ):
@@ -119,15 +118,15 @@
         )
 
         return initial_state
 
     def initialize(
         self,
         problem: Problem,
-        x0: Union[np.ndarray, List[np.ndarray]],
+        x0: np.ndarray | list[np.ndarray],
     ) -> None:
         """Initialize the sampler.
 
         It is recommended to initialize walkers
 
         Parameters
         ----------
```

### Comparing `pypesto-0.4.2/pypesto/sample/geweke_test.py` & `pypesto-0.5.0/pypesto/sample/geweke_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Helper function for `geweke_test`."""
 
 import logging
 import warnings
-from typing import Tuple
 
 import numpy as np
 from scipy.stats import norm
 
 logger = logging.getLogger(__name__)
 
 
@@ -47,15 +46,15 @@
         n = nw
 
     # Number of windows
     k = np.floor((n - n_overlap) / (nw - n_overlap)).astype(int)
     index = np.arange(nw)
     # Normalizing scale factor
     kmu = k * np.linalg.norm(w) ** 2
-    spectral_density = np.zeros((nfft))
+    spectral_density = np.zeros(nfft)
 
     for _ in range(k):
         xw = w * x[index]
         index += nw - n_overlap
         Xx = np.absolute(np.fft.fft(xw, n=nfft, axis=0)) ** 2
         spectral_density += Xx
 
@@ -91,15 +90,15 @@
         if len(_spectral_density_zero) > 0:
             spectral_density_zero[:, i] = _spectral_density_zero[0]
     return spectral_density_zero
 
 
 def calculate_zscore(
     chain: np.ndarray, a: float = 0.1, b: float = 0.5
-) -> Tuple[float, float]:
+) -> tuple[float, float]:
     """
     Perform a Geweke test on a chain.
 
     Use the first "a" fraction and the last "b" fraction of it for
     comparison. Test for equality of the means of the first a% and last b%
     of a Markov chain.
 
@@ -193,15 +192,15 @@
         # Calculate z-score
         z[i, :], _ = calculate_zscore(chain[indices:, :])
 
     # Sort z-score for Bonferroni-Holm inverse
     # to sorting p-values
     max_z = np.max(np.absolute(z), axis=1)
     idxs = max_z.argsort()[::-1]  # sort descend
-    alpha2 = zscore * np.ones((len(idxs)))
+    alpha2 = zscore * np.ones(len(idxs))
 
     for i in range(len(max_z)):
         alpha2[idxs[i]] /= len(fragments) - np.argwhere(idxs == i).item(0) + 1
 
     if np.any(alpha2 > max_z):
         burn_in = (np.where(alpha2 > max_z)[0][0]) * step
     else:
```

### Comparing `pypesto-0.4.2/pypesto/sample/metropolis.py` & `pypesto-0.5.0/pypesto/sample/metropolis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Dict, Sequence, Union
+from collections.abc import Sequence
+from typing import Union
 
 import numpy as np
 
 from ..history import NoHistory
 from ..objective import NegLogPriors, ObjectiveBase
 from ..problem import Problem
 from ..result import McmcPtResult
@@ -32,30 +33,30 @@
 
     For reference matlab implementations see:
 
     * https://en.wikipedia.org/wiki/Metropolis%E2%80%93Hastings_algorithm
     * https://github.com/ICB-DCM/PESTO/blob/master/private/performPT.m
     """
 
-    def __init__(self, options: Dict = None):
+    def __init__(self, options: dict = None):
         super().__init__(options)
         self.problem: Union[Problem, None] = None
         self.neglogpost: Union[ObjectiveBase, None] = None
         self.neglogprior: Union[NegLogPriors, None] = None
         self.trace_x: Union[Sequence[np.ndarray], None] = None
         self.trace_neglogpost: Union[Sequence[float], None] = None
         self.trace_neglogprior: Union[Sequence[float], None] = None
         self.temper_lpost: bool = False
 
     @classmethod
     def default_options(cls):
         """Return the default options for the sampler."""
         return {
-            'std': 1.0,  # the proposal standard deviation
-            'show_progress': None,  # whether to show the progress
+            "std": 1.0,  # the proposal standard deviation
+            "show_progress": None,  # whether to show the progress
         }
 
     def initialize(self, problem: Problem, x0: np.ndarray):
         """Initialize the sampler."""
         self.problem = problem
         self.neglogpost = problem.objective
         self.neglogpost.history = NoHistory()
@@ -69,15 +70,15 @@
 
     def sample(self, n_samples: int, beta: float = 1.0):
         """Load last recorded particle."""
         x = self.trace_x[-1]
         lpost = -self.trace_neglogpost[-1]
         lprior = -self.trace_neglogprior[-1]
 
-        show_progress = self.options.get('show_progress', None)
+        show_progress = self.options.get("show_progress", None)
 
         # loop over iterations
         for _ in tqdm(range(int(n_samples)), enable=show_progress):
             # perform step
             x, lpost, lprior = self._perform_step(
                 x=x, lpost=lpost, lprior=lprior, beta=beta
             )
@@ -94,15 +95,15 @@
         Default: Do nothing.
 
         Parameters
         ----------
         temper_lpost:
             Whether to temperate the posterior or only the likelihood.
         """
-        self.options['show_progress'] = False
+        self.options["show_progress"] = False
         self.temper_lpost = temper_lpost
 
     def _perform_step(
         self, x: np.ndarray, lpost: np.ndarray, lprior: np.ndarray, beta: float
     ):
         """
         Perform a step.
@@ -157,15 +158,15 @@
             x, lpost, log_p_acc, len(self.trace_neglogpost) + 1
         )
 
         return x, lpost, lprior
 
     def _propose_parameter(self, x: np.ndarray):
         """Propose a step."""
-        x_new: np.ndarray = x + self.options['std'] * np.random.randn(len(x))
+        x_new: np.ndarray = x + self.options["std"] * np.random.randn(len(x))
         return x_new
 
     def _update_proposal(
         self, x: np.ndarray, lpost: float, log_p_acc: float, n_sample_cur: int
     ):
         """Update the proposal density. Default: Do nothing."""
```

### Comparing `pypesto-0.4.2/pypesto/sample/pymc.py` & `pypesto-0.5.0/pypesto/sample/pymc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Pymc v4 Sampler."""
 
 from __future__ import annotations
 
 import logging
-from typing import Union
 
 import arviz as az
 import numpy as np
 import pymc
 import pytensor.tensor as pt
 
 from ..history import MemoryHistory
@@ -108,31 +107,31 @@
         self,
         step_function=None,
         post_compute_fval: bool = True,
         **kwargs,
     ):
         super().__init__(kwargs)
         self.step_function = step_function
-        self.problem: Union[Problem, None] = None
-        self.x0: Union[np.ndarray, None] = None
-        self.trace: Union[pymc.backends.Text, None] = None
-        self.data: Union[az.InferenceData, None] = None
+        self.problem: Problem | None = None
+        self.x0: np.ndarray | None = None
+        self.trace: pymc.backends.Text | None = None
+        self.data: az.InferenceData | None = None
 
     @classmethod
     def translate_options(cls, options):
         """
         Translate options and fill in defaults.
 
         Parameters
         ----------
         options:
             Options configuring the sampler.
         """
         if not options:
-            options = {'chains': 1}
+            options = {"chains": 1}
         return options
 
     def initialize(self, problem: Problem, x0: np.ndarray):
         """
         Initialize the sampler.
 
         Parameters
@@ -160,15 +159,15 @@
         ----------
         n_samples:
             Number of samples to be computed.
         """
         try:
             import pymc
         except ImportError:
-            raise SamplerImportError("pymc")
+            raise SamplerImportError("pymc") from None
 
         problem = self.problem
         log_post = PymcObjectiveOp.create_instance(problem.objective, beta)
         trace = self.trace
 
         x0 = None
         x_names_free = problem.get_reduced_vector(problem.x_names)
```

### Comparing `pypesto-0.4.2/pypesto/sample/sample.py` & `pypesto-0.5.0/pypesto/sample/sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from time import process_time
-from typing import Callable, List, Optional, Union
+from typing import Callable, Optional, Union
 
 import numpy as np
 
 from ..problem import Problem
 from ..result import Result
 from ..store import autosave
 from .adaptive_metropolis import AdaptiveMetropolisSampler
@@ -14,15 +14,15 @@
 logger = logging.getLogger(__name__)
 
 
 def sample(
     problem: Problem,
     n_samples: Optional[int],
     sampler: Sampler = None,
-    x0: Union[np.ndarray, List[np.ndarray]] = None,
+    x0: Union[np.ndarray, list[np.ndarray]] = None,
     result: Result = None,
     filename: Union[str, Callable, None] = None,
     overwrite: bool = False,
 ) -> Result:
     """
     Call to do parameter sampling.
 
@@ -68,15 +68,15 @@
         n_samples = bound_n_samples_from_env(n_samples)
 
     # try to find initial parameters
     if x0 is None:
         result.optimize_result.sort()
         if len(result.optimize_result.list) > 0:
             x0 = problem.get_reduced_vector(
-                result.optimize_result.list[0]['x']
+                result.optimize_result.list[0]["x"]
             )
         # TODO multiple x0 for PT, #269
 
     # set sampler
     if sampler is None:
         sampler = AdaptiveMetropolisSampler()
```

### Comparing `pypesto-0.4.2/pypesto/sample/sampler.py` & `pypesto-0.5.0/pypesto/sample/sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Various Sampler classes."""
 
 import abc
-from typing import Dict, List, Union
+from typing import Union
 
 import numpy as np
 
 from ..problem import Problem
 from ..result import McmcPtResult
 
 
@@ -22,20 +22,20 @@
 class Sampler(abc.ABC):
     """Sampler base class, not functional on its own.
 
     The sampler maintains an internal chain, which is initialized in
     `initialize`, and updated in `sample`.
     """
 
-    def __init__(self, options: Dict = None):
+    def __init__(self, options: dict = None):
         self.options = self.__class__.translate_options(options)
 
     @abc.abstractmethod
     def initialize(
-        self, problem: Problem, x0: Union[np.ndarray, List[np.ndarray]]
+        self, problem: Problem, x0: Union[np.ndarray, list[np.ndarray]]
     ):
         """Initialize the sampler.
 
         Parameters
         ----------
         problem:
             The problem for which to sample.
@@ -60,15 +60,15 @@
         """
 
     @abc.abstractmethod
     def get_samples(self) -> McmcPtResult:
         """Get the generated samples."""
 
     @classmethod
-    def default_options(cls) -> Dict:
+    def default_options(cls) -> dict:
         """
         Set/Get default options.
 
         Returns
         -------
         default_options:
             Default sampler options.
```

### Comparing `pypesto-0.4.2/pypesto/sample/util.py` & `pypesto-0.5.0/pypesto/sample/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """A set of helper functions."""
 
 import logging
 import os
-from typing import Tuple
 
 import numpy as np
 
 from ..C import PYPESTO_MAX_N_SAMPLES
 from ..result import Result
 from .diagnostics import geweke_test
 
 logger = logging.getLogger(__name__)
 
 
 def calculate_ci_mcmc_sample(
     result: Result,
     ci_level: float = 0.95,
     exclude_burn_in: bool = True,
-) -> Tuple[np.ndarray, np.ndarray]:
+) -> tuple[np.ndarray, np.ndarray]:
     """Calculate parameter credibility intervals based on MCMC samples.
 
     Parameters
     ----------
     result:
         The pyPESTO result object with filled sample result.
     ci_level:
@@ -47,15 +46,15 @@
     lb, ub = calculate_ci(chain, ci_level=ci_level, axis=0)
     return lb, ub
 
 
 def calculate_ci_mcmc_sample_prediction(
     simulated_values: np.ndarray,
     ci_level: float = 0.95,
-) -> Tuple[np.ndarray, np.ndarray]:
+) -> tuple[np.ndarray, np.ndarray]:
     """Calculate prediction credibility intervals based on MCMC samples.
 
     Parameters
     ----------
     simulated_values:
         Simulated model states or model observables.
     ci_level:
@@ -70,15 +69,15 @@
     return lb, ub
 
 
 def calculate_ci(
     values: np.ndarray,
     ci_level: float,
     **kwargs,
-) -> Tuple[np.ndarray, np.ndarray]:
+) -> tuple[np.ndarray, np.ndarray]:
     """Calculate confidence/credibility levels using percentiles.
 
     Parameters
     ----------
     values:
         The values used to calculate percentiles.
     ci_level:
```

### Comparing `pypesto-0.4.2/pypesto/select/__init__.py` & `pypesto-0.5.0/pypesto/select/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,9 +16,10 @@
     del petab_select
 except ImportError:
     import warnings
 
     warnings.warn(
         "pyPESTO's model selection methods require an installation of PEtab "
         "Select (https://github.com/PEtab-dev/petab_select). Install via "
-        "`pip3 install petab-select` or `pip3 install pypesto[select]`."
+        "`pip3 install petab-select` or `pip3 install pypesto[select]`.",
+        stacklevel=1,
     )
```

### Comparing `pypesto-0.4.2/pypesto/select/method.py` & `pypesto-0.5.0/pypesto/select/method.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 from .model_problem import TYPE_POSTPROCESSOR, ModelProblem
 
 
 class MethodSignalProceed(str, Enum):
     """Indicators for how a model selection method should proceed."""
 
     # TODO move to PEtab Select?
-    STOP = 'stop'
-    CONTINUE = 'continue'
+    STOP = "stop"
+    CONTINUE = "continue"
 
 
 @dataclass
 class MethodSignal:
     """The state of a model selection method after a single model calibration.
 
     Attributes
@@ -58,15 +58,15 @@
     logger:
         A logger from the :mod:`logging` module.
     """
 
     column_width: int = 12
     column_sep: str = " | "
 
-    def __init__(self, level: str = 'info'):
+    def __init__(self, level: str = "info"):
         self.logger = logging.getLogger(__name__)
         self.level = level
 
     def log(self, message, level: str = None) -> None:
         """Log a message.
 
         Parameters
@@ -80,15 +80,15 @@
         if level is None:
             level = self.level
         getattr(self.logger, level)(message)
 
     def new_selection(self) -> None:
         """Start logging a new model selection."""
         padding = 20
-        self.log('-' * padding + 'New Selection' + '-' * padding)
+        self.log("-" * padding + "New Selection" + "-" * padding)
         columns = {
             "Predecessor model subspace:ID": "model0",
             "Model subspace:ID": "model",
             "Criterion ID": "crit",
             "Predecessor model criterion": "model0_crit",
             "Model criterion": "model_crit",
             "Criterion difference": "crit_diff",
@@ -137,17 +137,17 @@
             model:
                 The model.
 
             Returns
             -------
             The ID.
             """
-            model_subspace_id = model.model_subspace_id or ''
+            model_subspace_id = model.model_subspace_id or ""
             original_model_id = model.model_id or model.get_hash()
-            model_id = model_subspace_id + ':' + original_model_id
+            model_id = model_subspace_id + ":" + original_model_id
             return model_id
 
         def float_to_str(value: float, precision: int = 3) -> str:
             return f"{value:.{precision}e}"
 
         if isinstance(predecessor_model, Model):
             predecessor_model_id = get_model_id(predecessor_model)
@@ -257,64 +257,64 @@
         self.startpoint_latest_mle = startpoint_latest_mle
 
         self.logger = MethodLogger()
 
         # TODO deprecated
         old_model_problem_options = {}
         for key, value in [
-            ('postprocessor', model_postprocessor),
+            ("postprocessor", model_postprocessor),
             (
-                'model_to_pypesto_problem_method',
+                "model_to_pypesto_problem_method",
                 model_to_pypesto_problem_method,
             ),
-            ('minimize_options', minimize_options),
-            ('objective_customizer', objective_customizer),
+            ("minimize_options", minimize_options),
+            ("objective_customizer", objective_customizer),
         ]:
             if value is not None:
                 old_model_problem_options[key] = value
                 self.logger.log(
-                    f'Specifying `{key}` as an individual argument is '
-                    'deprecated. Please instead specify it within some '
-                    '`model_problem_options` dictionary, e.g. '
+                    f"Specifying `{key}` as an individual argument is "
+                    "deprecated. Please instead specify it within some "
+                    "`model_problem_options` dictionary, e.g. "
                     f'`model_problem_options={{"{key}": ...}}`.',
-                    level='warning',
+                    level="warning",
                 )
         self.model_problem_options = {}
         self.model_problem_options |= old_model_problem_options
         if model_problem_options is not None:
             self.model_problem_options |= model_problem_options
 
         self.criterion = criterion
         if self.criterion is None:
             self.criterion = self.petab_select_problem.criterion
 
         # Forbid specification of both a candidate space and a method.
         if candidate_space is not None and method is not None:
             self.logger.log(
                 (
-                    'Both `candidate_space` and `method` were provided. '
-                    'Please only provide one. The method will be ignored here.'
+                    "Both `candidate_space` and `method` were provided. "
+                    "Please only provide one. The method will be ignored here."
                 ),
-                level='warning',
+                level="warning",
             )
         # Get method.
         self.method = (
             method
             if method is not None
             else (
                 candidate_space.method
                 if candidate_space is not None
                 else self.petab_select_problem.method
             )
         )
         # Require either a candidate space or a method.
         if candidate_space is None and self.method is None:
             raise ValueError(
-                'Please provide one of either `candidate_space` or `method`, '
-                'or specify the `method` in the PEtab Select problem.'
+                "Please provide one of either `candidate_space` or `method`, "
+                "or specify the `method` in the PEtab Select problem."
             )
         # Use candidate space if provided.
         if candidate_space is not None:
             self.candidate_space = candidate_space
             if predecessor_model is not None:
                 candidate_space.set_predecessor_model(predecessor_model)
         # Else generate one based on the PEtab Select problem.
@@ -525,18 +525,18 @@
             and model.predecessor_model_hash in self.calibrated_models
         ):
             predecessor_model = self.calibrated_models[
                 model.predecessor_model_hash
             ]
             if str(model.petab_yaml) != str(predecessor_model.petab_yaml):
                 raise NotImplementedError(
-                    'The PEtab YAML files differ between the model and its '
-                    'predecessor model. This may imply different (fixed union '
-                    'estimated) parameter sets. Support for this is not yet '
-                    'implemented.'
+                    "The PEtab YAML files differ between the model and its "
+                    "predecessor model. This may imply different (fixed union "
+                    "estimated) parameter sets. Support for this is not yet "
+                    "implemented."
                 )
             x_guess = {
                 **predecessor_model.parameters,
                 **predecessor_model.estimated_parameters,
             }
 
         return ModelProblem(
```

### Comparing `pypesto-0.4.2/pypesto/select/misc.py` & `pypesto-0.5.0/pypesto/select/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Miscellaneous methods."""
 
 import logging
-from typing import Iterable
+from collections.abc import Iterable
 
 import pandas as pd
 import petab
 import petab_select.ui
 from petab.C import ESTIMATE, NOMINAL_VALUE
 from petab_select import Model, parameter_string_to_value
 from petab_select.constants import PETAB_PROBLEM
```

### Comparing `pypesto-0.4.2/pypesto/select/model_problem.py` & `pypesto-0.5.0/pypesto/select/model_problem.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.2/pypesto/select/postprocessors.py` & `pypesto-0.5.0/pypesto/select/postprocessors.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 import numpy as np
 from petab_select.constants import ESTIMATE, TYPE_PATH, Criterion
 
 from .. import store, visualize
 from .model_problem import TYPE_POSTPROCESSOR, ModelProblem
 
 __all__ = [
-    'model_id_binary_postprocessor',
-    'multi_postprocessor',
-    'report_postprocessor',
-    'save_postprocessor',
-    'waterfall_plot_postprocessor',
+    "model_id_binary_postprocessor",
+    "multi_postprocessor",
+    "report_postprocessor",
+    "save_postprocessor",
+    "waterfall_plot_postprocessor",
 ]
 
 
 def multi_postprocessor(
     problem: ModelProblem,
     postprocessors: list[TYPE_POSTPROCESSOR] = None,
 ):
@@ -146,38 +146,38 @@
         ]
 
     start_optimization_times = problem.minimize_result.optimize_result.time
 
     header = []
     row = []
 
-    header.append('model_id')
+    header.append("model_id")
     row.append(problem.model.model_id)
 
-    header.append('total_time')
+    header.append("total_time")
     row.append(str(sum(start_optimization_times)))
 
     for criterion in criteria:
         header.append(criterion.value)
         row.append(str(problem.model.get_criterion(criterion)))
 
     # Arbitrary convergence criterion
-    header.append('n_converged')
+    header.append("n_converged")
     row.append(
         str(
             (
                 np.array(problem.minimize_result.optimize_result.fval)
                 < (problem.minimize_result.optimize_result.list[0].fval + 0.1)
             ).sum()
         )
     )
 
     for start_index, start_optimization_time in enumerate(
         start_optimization_times
     ):
-        header.append(f'start_time_{start_index}')
+        header.append(f"start_time_{start_index}")
         row.append(str(start_optimization_time))
 
-    with open(output_filepath, 'a+') as f:
+    with open(output_filepath, "a+") as f:
         if write_header:
-            f.write('\t'.join(header) + '\n')
-        f.write('\t'.join(row) + '\n')
+            f.write("\t".join(header) + "\n")
+        f.write("\t".join(row) + "\n")
```

### Comparing `pypesto-0.4.2/pypesto/select/problem.py` & `pypesto-0.5.0/pypesto/select/problem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Manage all components of a pyPESTO model selection problem."""
 
 import warnings
-from typing import Any, Iterable, Optional
+from collections.abc import Iterable
+from typing import Any, Optional
 
 import petab_select
 from petab_select import Model
 
 from .method import MethodCaller
 from .model_problem import TYPE_POSTPROCESSOR, ModelProblem  # noqa: F401
 
@@ -46,19 +47,21 @@
 
         self.model_problem_options = {}
         if model_problem_options is not None:
             self.model_problem_options = model_problem_options
         # TODO deprecated
         if model_postprocessor is not None:
             warnings.warn(
-                'Specifying `model_postprocessor` directly is deprecated. '
-                'Please specify it with `model_problem_options`, e.g. '
-                'model_problem_options={"postprocessor": ...}`.'
+                "Specifying `model_postprocessor` directly is deprecated. "
+                "Please specify it with `model_problem_options`, e.g. "
+                'model_problem_options={"postprocessor": ...}`.',
+                DeprecationWarning,
+                stacklevel=1,
             )
-            self.model_problem_options['postprocessor'] = model_postprocessor
+            self.model_problem_options["postprocessor"] = model_postprocessor
 
         self.set_state(
             calibrated_models={},
             newly_calibrated_models={},
         )
 
         # TODO default caller, based on petab_select.Problem
@@ -71,15 +74,15 @@
 
         Returns
         -------
         A :class:`MethodCaller` instance.
         """
         kwargs = kwargs.copy()
         model_problem_options = self.model_problem_options | kwargs.pop(
-            'model_problem_options', {}
+            "model_problem_options", {}
         )
 
         return MethodCaller(
             petab_select_problem=self.petab_select_problem,
             calibrated_models=self.calibrated_models,
             model_problem_options=model_problem_options,
             **kwargs,
@@ -113,21 +116,21 @@
     def handle_select_kwargs(
         self,
         kwargs: dict[str, Any],
     ):
         """Check keyword arguments to select calls."""
         if "newly_calibrated_models" in kwargs:
             raise ValueError(
-                'Please supply `newly_calibrated_models` via '
-                '`pypesto.select.Problem.set_state`.'
+                "Please supply `newly_calibrated_models` via "
+                "`pypesto.select.Problem.set_state`."
             )
         if "calibrated_models" in kwargs:
             raise ValueError(
-                'Please supply `calibrated_models` via '
-                '`pypesto.select.Problem.set_state`.'
+                "Please supply `calibrated_models` via "
+                "`pypesto.select.Problem.set_state`."
             )
 
     def select(
         self,
         **kwargs,
     ) -> tuple[Model, dict[str, Model], dict[str, Model]]:
         """Run a single iteration of a model selection algorithm.
```

### Comparing `pypesto-0.4.2/pypesto/startpoint/base.py` & `pypesto-0.5.0/pypesto/startpoint/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Startpoint base classes."""
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Callable, Union
+from typing import TYPE_CHECKING, Callable
 
 import numpy as np
 
 from ..C import FVAL, GRAD
 from ..objective import ObjectiveBase
 
 if TYPE_CHECKING:
@@ -239,15 +239,15 @@
         ub: np.ndarray,
     ) -> np.ndarray:
         """Call function."""
         return self.function(n_starts=n_starts, lb=lb, ub=ub)
 
 
 def to_startpoint_method(
-    maybe_startpoint_method: Union[StartpointMethod, Callable, bool],
+    maybe_startpoint_method: StartpointMethod | Callable | bool,
 ) -> StartpointMethod:
     """Create StartpointMethod instance if possible, otherwise raise.
 
     Parameters
     ----------
     maybe_startpoint_method:
         A StartpointMethod instance, or a Callable as expected by
```

### Comparing `pypesto-0.4.2/pypesto/startpoint/latin_hypercube.py` & `pypesto-0.5.0/pypesto/startpoint/latin_hypercube.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.2/pypesto/startpoint/uniform.py` & `pypesto-0.5.0/pypesto/startpoint/uniform.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.2/pypesto/store/auto.py` & `pypesto-0.5.0/pypesto/store/auto.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     if isinstance(filename, Path):
         filename = str(filename)
 
     if filename == "Auto":
         filename = default_filename
     elif isinstance(filename, str):
         if os.path.exists(filename) and not overwrite:
-            with h5py.File(filename, 'r') as f:
+            with h5py.File(filename, "r") as f:
                 storage_used = store_type in f.keys()
             if storage_used:
                 logger.warning(
                     f"There is already a {store_type}-result saved in "
                     f"{filename}. Please choose a different filename or set "
                     f"overwrite=True. File will be saved as in AUTO mode."
                 )
```

### Comparing `pypesto-0.4.2/pypesto/store/hdf5.py` & `pypesto-0.5.0/pypesto/store/hdf5.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Convenience functions for working with HDF5 files."""
 
+from collections.abc import Collection
 from numbers import Integral, Number, Real
-from typing import Collection
 
 import h5py
 import numpy as np
 
 
 def write_array(f: h5py.Group, path: str, values: Collection) -> None:
     """
@@ -43,19 +43,19 @@
     strings:
         list of strings to be written to f
     """
     dt = h5py.special_dtype(vlen=str)
     dset = f.create_dataset(path, (len(strings),), dtype=dt)
 
     if len(strings):
-        dset[:] = [s.encode('utf8') for s in strings]
+        dset[:] = [s.encode("utf8") for s in strings]
 
 
 def write_float_array(
-    f: h5py.Group, path: str, values: Collection[Number], dtype='f8'
+    f: h5py.Group, path: str, values: Collection[Number], dtype="f8"
 ) -> None:
     """
     Write float array to hdf5.
 
     Parameters
     ----------
     f:
@@ -73,15 +73,15 @@
         dset = f[path]
 
     if len(values):
         dset[:] = values
 
 
 def write_int_array(
-    f: h5py.Group, path: str, values: Collection[int], dtype='<i4'
+    f: h5py.Group, path: str, values: Collection[int], dtype="<i4"
 ):
     """
     Write integer array to hdf5.
 
     Parameters
     ----------
     f:
```

### Comparing `pypesto-0.4.2/pypesto/store/read_from_hdf5.py` & `pypesto-0.5.0/pypesto/store/read_from_hdf5.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 logger = logging.getLogger(__name__)
 
 
 def read_hdf5_profile(
     f: h5py.File,
     profile_id: str,
     parameter_id: str,
-) -> 'ProfilerResult':
+) -> "ProfilerResult":
     """Read HDF5 results per start.
 
     Parameters
     ----------
     f:
         The HDF5 result file
     profile_id:
@@ -34,56 +34,56 @@
     parameter_id:
         specifies the profile index that is read
         from the HDF5 file
     """
     result = ProfilerResult(np.empty((0, 0)), np.array([]), np.array([]))
 
     for profile_key in result.keys():
-        if profile_key in f[f'/profiling/{profile_id}/{parameter_id}']:
+        if profile_key in f[f"/profiling/{profile_id}/{parameter_id}"]:
             result[profile_key] = f[
-                f'/profiling/{profile_id}/{parameter_id}/{profile_key}'
+                f"/profiling/{profile_id}/{parameter_id}/{profile_key}"
             ][:]
-        elif profile_key in f[f'/profiling/{profile_id}/{parameter_id}'].attrs:
+        elif profile_key in f[f"/profiling/{profile_id}/{parameter_id}"].attrs:
             result[profile_key] = f[
-                f'/profiling/{profile_id}/{parameter_id}'
+                f"/profiling/{profile_id}/{parameter_id}"
             ].attrs[profile_key]
     return result
 
 
 def read_hdf5_optimization(
     f: h5py.File,
     file_name: Union[Path, str],
     opt_id: str,
-) -> 'OptimizerResult':
+) -> "OptimizerResult":
     """Read HDF5 results per start.
 
     Parameters
     ----------
     f:
         The HDF5 result file
     file_name:
         The name of the HDF5 file, needed to create HDF5History
     opt_id:
         Specifies the start that is read from the HDF5 file
     """
     result = OptimizerResult()
 
     for optimization_key in result.keys():
-        if optimization_key == 'history':
+        if optimization_key == "history":
             if optimization_key in f:
-                result['history'] = Hdf5History(id=opt_id, file=file_name)
-                result['history'].recover_options(file_name)
+                result["history"] = Hdf5History(id=opt_id, file=file_name)
+                result["history"].recover_options(file_name)
                 continue
-        if optimization_key in f[f'/optimization/results/{opt_id}']:
+        if optimization_key in f[f"/optimization/results/{opt_id}"]:
             result[optimization_key] = f[
-                f'/optimization/results/{opt_id}/{optimization_key}'
+                f"/optimization/results/{opt_id}/{optimization_key}"
             ][:]
-        elif optimization_key in f[f'/optimization/results/{opt_id}'].attrs:
+        elif optimization_key in f[f"/optimization/results/{opt_id}"].attrs:
             result[optimization_key] = f[
-                f'/optimization/results/{opt_id}'
+                f"/optimization/results/{opt_id}"
             ].attrs[optimization_key]
     return result
 
 
 class ProblemHDF5Reader:
     """
     Reader of the HDF5 problem files written by ProblemHDF5Writer.
@@ -118,27 +118,28 @@
             A problem instance with all attributes read in.
         """
         # create empty problem
         if objective is None:
             objective = Objective()
             # raise warning that objective is not loaded.
             warnings.warn(
-                'You are loading a problem. This problem is not to be used '
-                'without a separately created objective.'
+                "You are loading a problem. This problem is not to be used "
+                "without a separately created objective.",
+                stacklevel=2,
             )
         problem = Problem(objective, [], [])
 
-        with h5py.File(self.storage_filename, 'r') as f:
-            for problem_key in f['/problem']:
-                if problem_key == 'config':
+        with h5py.File(self.storage_filename, "r") as f:
+            for problem_key in f["/problem"]:
+                if problem_key == "config":
                     continue
-                setattr(problem, problem_key, f[f'/problem/{problem_key}'][:])
-            for problem_attr in f['/problem'].attrs:
+                setattr(problem, problem_key, f[f"/problem/{problem_key}"][:])
+            for problem_attr in f["/problem"].attrs:
                 setattr(
-                    problem, problem_attr, f['/problem'].attrs[problem_attr]
+                    problem, problem_attr, f["/problem"].attrs[problem_attr]
                 )
 
         # h5 uses numpy for everything; convert to lists where necessary
         problem.x_fixed_vals = [float(val) for val in problem.x_fixed_vals]
         problem.x_fixed_indices = [int(ix) for ix in problem.x_fixed_indices]
         problem.x_names = [name.decode() for name in problem.x_names]
 
@@ -166,15 +167,15 @@
         """
         self.storage_filename = storage_filename
         self.results = Result()
 
     def read(self) -> Result:
         """Read HDF5 result file and return pyPESTO result object."""
         with h5py.File(self.storage_filename, "r") as f:
-            for opt_id in f['/optimization/results']:
+            for opt_id in f["/optimization/results"]:
                 result = read_hdf5_optimization(
                     f, self.storage_filename, opt_id
                 )
                 self.results.optimize_result.append(result)
             self.results.optimize_result.sort()
         return self.results
 
@@ -200,18 +201,18 @@
         self.storage_filename = storage_filename
         self.results = Result()
 
     def read(self) -> Result:
         """Read HDF5 result file and return pyPESTO result object."""
         sample_result = {}
         with h5py.File(self.storage_filename, "r") as f:
-            for key in f['/sampling/results']:
-                sample_result[key] = f[f'/sampling/results/{key}'][:]
-            for key in f['/sampling/results'].attrs:
-                sample_result[key] = f['/sampling/results'].attrs[key]
+            for key in f["/sampling/results"]:
+                sample_result[key] = f[f"/sampling/results/{key}"][:]
+            for key in f["/sampling/results"].attrs:
+                sample_result[key] = f["/sampling/results"].attrs[key]
         try:
             self.results.sample_result = McmcPtResult(**sample_result)
         except TypeError:
             logger.warning(
                 "Warning: You tried loading a non-existent " "sampling result."
             )
 
@@ -240,21 +241,21 @@
         self.storage_filename = storage_filename
         self.results = Result()
 
     def read(self) -> Result:
         """Read HDF5 result file and return pyPESTO result object."""
         profiling_list = []
         with h5py.File(self.storage_filename, "r") as f:
-            for profile_id in f['/profiling']:
+            for profile_id in f["/profiling"]:
                 profiling_list.append(
-                    [None for _ in f[f'/profiling/{profile_id}']]
+                    [None for _ in f[f"/profiling/{profile_id}"]]
                 )
-                for parameter_id in f[f'/profiling/{profile_id}']:
-                    if f[f'/profiling/{profile_id}/' f'{parameter_id}'].attrs[
-                        'IsNone'
+                for parameter_id in f[f"/profiling/{profile_id}"]:
+                    if f[f"/profiling/{profile_id}/" f"{parameter_id}"].attrs[
+                        "IsNone"
                     ]:
                         continue
                     profiling_list[int(profile_id)][
                         int(parameter_id)
                     ] = read_hdf5_profile(
                         f, profile_id=profile_id, parameter_id=parameter_id
                     )
@@ -305,41 +306,41 @@
     if optimize:
         pypesto_opt_reader = OptimizationResultHDF5Reader(filename)
         try:
             temp_result = pypesto_opt_reader.read()
             result.optimize_result = temp_result.optimize_result
         except KeyError:
             logger.warning(
-                'Loading the optimization result failed. It is '
-                'highly likely that no optimization result exists '
-                f'within {filename}.'
+                "Loading the optimization result failed. It is "
+                "highly likely that no optimization result exists "
+                f"within {filename}."
             )
 
     if profile:
         pypesto_profile_reader = ProfileResultHDF5Reader(filename)
         try:
             temp_result = pypesto_profile_reader.read()
             result.profile_result = temp_result.profile_result
         except KeyError:
             logger.warning(
-                'Loading the profiling result failed. It is '
-                'highly likely that no profiling result exists '
-                f'within {filename}.'
+                "Loading the profiling result failed. It is "
+                "highly likely that no profiling result exists "
+                f"within {filename}."
             )
 
     if sample:
         pypesto_sample_reader = SamplingResultHDF5Reader(filename)
         try:
             temp_result = pypesto_sample_reader.read()
             result.sample_result = temp_result.sample_result
         except KeyError:
             logger.warning(
-                'Loading the sampling result failed. It is '
-                'highly likely that no sampling result exists '
-                f'within {filename}.'
+                "Loading the sampling result failed. It is "
+                "highly likely that no sampling result exists "
+                f"within {filename}."
             )
 
     return result
 
 
 def load_objective_config(filename: Union[str, Path]):
     """Load the objective information stored in f.
@@ -350,11 +351,11 @@
         The name of the file in which the information are stored.
 
     Returns
     -------
         A dictionary of the information, stored instead of the
         actual objective in problem.objective.
     """
-    with h5py.File(filename, 'r') as f:
-        info_str = f['problem/config'][()].decode()
+    with h5py.File(filename, "r") as f:
+        info_str = f["problem/config"][()].decode()
         info = ast.literal_eval(info_str)
         return info
```

### Comparing `pypesto-0.4.2/pypesto/store/save_to_hdf5.py` & `pypesto-0.5.0/pypesto/store/save_to_hdf5.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,26 +69,26 @@
         # Create destination directory
         if isinstance(self.storage_filename, str):
             basedir = os.path.dirname(self.storage_filename)
             if basedir:
                 os.makedirs(basedir, exist_ok=True)
 
         with h5py.File(self.storage_filename, "a") as f:
-            check_overwrite(f, overwrite, 'problem')
+            check_overwrite(f, overwrite, "problem")
             attrs_to_save = [
                 a
                 for a in dir(problem)
-                if not a.startswith('__')
+                if not a.startswith("__")
                 and not callable(getattr(problem, a))
                 and not hasattr(type(problem), a)
             ]
 
             problem_grp = f.create_group("problem")
             # save the configuration
-            f['problem/config'] = str(problem.objective.get_config())
+            f["problem/config"] = str(problem.objective.get_config())
 
             for problem_attr in attrs_to_save:
                 value = getattr(problem, problem_attr)
                 if isinstance(value, (list, np.ndarray)):
                     value = np.asarray(value)
                     if value.size:
                         write_array(problem_grp, problem_attr, value)
@@ -122,25 +122,25 @@
         # Create destination directory
         if isinstance(self.storage_filename, str):
             basedir = os.path.dirname(self.storage_filename)
             if basedir:
                 os.makedirs(basedir, exist_ok=True)
 
         with h5py.File(self.storage_filename, "a") as f:
-            check_overwrite(f, overwrite, 'optimization')
+            check_overwrite(f, overwrite, "optimization")
             optimization_grp = f.require_group("optimization")
             # settings =
             # optimization_grp.create_dataset("settings", settings, dtype=)
             results_grp = optimization_grp.require_group("results")
 
             for start in result.optimize_result.list:
-                start_id = start['id']
+                start_id = start["id"]
                 start_grp = results_grp.require_group(start_id)
                 for key in start.keys():
-                    if key == 'history':
+                    if key == "history":
                         continue
                     if isinstance(start[key], np.ndarray):
                         write_array(start_grp, key, start[key])
                     elif start[key] is not None:
                         start_grp.attrs[key] = start[key]
                 f.flush()
 
@@ -181,15 +181,15 @@
         # Create destination directory
         if isinstance(self.storage_filename, str):
             basedir = os.path.dirname(self.storage_filename)
             if basedir:
                 os.makedirs(basedir, exist_ok=True)
 
         with h5py.File(self.storage_filename, "a") as f:
-            check_overwrite(f, overwrite, 'sampling')
+            check_overwrite(f, overwrite, "sampling")
             results_grp = f.require_group("sampling/results")
 
             for key in result.sample_result.keys():
                 if isinstance(result.sample_result[key], np.ndarray):
                     write_float_array(
                         results_grp, key, result.sample_result[key]
                     )
@@ -224,15 +224,15 @@
         # Create destination directory
         if isinstance(self.storage_filename, str):
             basedir = os.path.dirname(self.storage_filename)
             if basedir:
                 os.makedirs(basedir, exist_ok=True)
 
         with h5py.File(self.storage_filename, "a") as f:
-            check_overwrite(f, overwrite, 'profiling')
+            check_overwrite(f, overwrite, "profiling")
             profiling_grp = f.require_group("profiling")
 
             for profile_id, profile in enumerate(result.profile_result.list):
                 profile_grp = profiling_grp.require_group(str(profile_id))
                 for parameter_id, parameter_profile in enumerate(profile):
                     result_grp = profile_grp.require_group(str(parameter_id))
                     self._write_profiler_result(parameter_profile, result_grp)
@@ -244,18 +244,18 @@
         parameter_profile: Union[ProfilerResult, None], result_grp: h5py.Group
     ) -> None:
         """Write a single ProfilerResult to hdf5.
 
         Writes a single profile for a single parameter to the provided HDF5 group.
         """
         if parameter_profile is None:
-            result_grp.attrs['IsNone'] = True
+            result_grp.attrs["IsNone"] = True
             return
 
-        result_grp.attrs['IsNone'] = False
+        result_grp.attrs["IsNone"] = False
 
         for key, value in parameter_profile.items():
             try:
                 if isinstance(value, np.ndarray):
                     write_float_array(result_grp, key, value)
                 elif value is not None:
                     result_grp.attrs[key] = value
```

### Comparing `pypesto-0.4.2/pypesto/testing/examples.py` & `pypesto-0.5.0/pypesto/testing/examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import pandas as pd
 
 from pypesto.C import InnerParameterType
 
 
 def get_Boehm_JProteomeRes2014_hierarchical_petab() -> (
-    'petab.Problem'  # noqa: F821
+    "petab.Problem"  # noqa: F821
 ):
     """
     Get Boehm_JProteomeRes2014 problem with scaled/offset observables.
 
     Creates a modified version of the Boehm_JProteomeRes2014 benchmark problem,
     suitable for hierarchical optimization.
     """
@@ -45,34 +45,34 @@
             petab.PARAMETER_SCALE: petab.LIN,
             petab.LOWER_BOUND: -100,
             petab.UPPER_BOUND: 100,
             petab.NOMINAL_VALUE: 0,
             petab.ESTIMATE: 1,
         }
         for par_id in (
-            'offset_pSTAT5A_rel',
-            'offset_pSTAT5B_rel',
-            'offset_rSTAT5A_rel',
+            "offset_pSTAT5A_rel",
+            "offset_pSTAT5B_rel",
+            "offset_rSTAT5A_rel",
         )
     ]
 
     extra_parameters.extend(
         {
             petab.PARAMETER_ID: par_id,
             petab.PARAMETER_SCALE: petab.LIN,
             petab.LOWER_BOUND: 1e-5,
             petab.UPPER_BOUND: 1e5,
             petab.NOMINAL_VALUE: nominal_value,
             petab.ESTIMATE: 1,
         }
         for par_id, nominal_value in zip(
             (
-                'scaling_pSTAT5A_rel',
-                'scaling_pSTAT5B_rel',
-                'scaling_rSTAT5A_rel',
+                "scaling_pSTAT5A_rel",
+                "scaling_pSTAT5B_rel",
+                "scaling_rSTAT5A_rel",
             ),
             (3.85261197844677, 6.59147818673419, 3.15271275648527),
         )
     )
 
     petab_problem.parameter_df = pd.concat(
         [
@@ -104,15 +104,15 @@
 
     petab.lint_problem(petab_problem)
 
     return petab_problem
 
 
 def get_Boehm_JProteomeRes2014_hierarchical_petab_corrected_bounds() -> (
-    'petab.Problem'  # noqa: F821
+    "petab.Problem"  # noqa: F821
 ):
     """
     See `get_Boehm_JProteomeRes2014_hierarchical_petab`.
 
     Adjusts this PEtab problem to have correct bounds for inner parameters.
     """
     from ..hierarchical.petab import correct_parameter_df_bounds
```

### Comparing `pypesto-0.4.2/pypesto/util.py` & `pypesto-0.5.0/pypesto/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 Utilities
 =========
 
 Package-wide utilities.
 
 """
 
+from collections.abc import Sequence
 from numbers import Number
 from operator import itemgetter
-from typing import Any, Callable, Optional, Sequence, Tuple, Union
+from typing import Any, Callable, Optional, Union
 
 import numpy as np
 from scipy import cluster
 from tqdm import tqdm as _tqdm
 
 
 def _check_none(fun: Callable[..., Any]) -> Callable[..., Union[Any, None]]:
@@ -187,15 +188,15 @@
     condition_id:
         The condition ID that will be used to generate a label.
 
     Returns
     -------
     The condition label.
     """
-    return f'condition_{condition_id}'
+    return f"condition_{condition_id}"
 
 
 def assign_clusters(vals):
     """
     Find clustering.
 
     Parameters
@@ -222,15 +223,15 @@
 
     # however: clusters are sorted by size, not by value... Resort.
     # Create preallocated object first
     cluster_indices = np.zeros(vals.size, dtype=int)
 
     # get clustering based on distance
     clust = cluster.hierarchy.fcluster(
-        cluster.hierarchy.linkage(vals), t=0.1, criterion='distance'
+        cluster.hierarchy.linkage(vals), t=0.1, criterion="distance"
     )
 
     # get unique clusters
     _, ind_clust = np.unique(clust, return_index=True)
     unique_clust = clust[np.sort(ind_clust)]
     cluster_size = np.zeros(unique_clust.size, dtype=int)
 
@@ -243,15 +244,15 @@
 
 
 def delete_nan_inf(
     fvals: np.ndarray,
     x: Optional[Sequence[Union[np.ndarray, list[float]]]] = None,
     xdim: Optional[int] = 1,
     magnitude_bound: Optional[float] = np.inf,
-) -> Tuple[np.ndarray, np.ndarray]:
+) -> tuple[np.ndarray, np.ndarray]:
     """
     Delete nan and inf values in fvals.
 
     If parameters 'x' are passed, also the corresponding entries are deleted.
 
     Parameters
     ----------
```

### Comparing `pypesto-0.4.2/pypesto/visualize/__init__.py` & `pypesto-0.5.0/pypesto/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.2/pypesto/visualize/clust_color.py` & `pypesto-0.5.0/pypesto/visualize/clust_color.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional, Union
+from typing import Optional, Union
 
 import matplotlib.cm as cm
 import numpy as np
 
 from pypesto.util import assign_clusters
 
 # for typehints
@@ -148,24 +148,24 @@
     if colors.shape[0] == 4:
         colors = np.transpose(colors)
         if n_vals == colors.shape[0]:
             return colors
 
     # Shape of array did not match n_vals. Error due to size mismatch:
     raise ValueError(
-        'Incorrect color input. Colors must be specified either as '
-        'list of `[r, g, b, alpha]` with length equal to that of `vals` '
-        f'(here: {n_vals}), or as a single `[r, g, b, alpha]`.'
+        "Incorrect color input. Colors must be specified either as "
+        "list of `[r, g, b, alpha]` with length equal to that of `vals` "
+        f"(here: {n_vals}), or as a single `[r, g, b, alpha]`."
     )
 
 
 def assign_colors_for_list(
     num_entries: int,
-    colors: Optional[Union[RGBA, List[RGBA], np.ndarray]] = None,
-) -> Union[List[List[float]], np.ndarray]:
+    colors: Optional[Union[RGBA, list[RGBA], np.ndarray]] = None,
+) -> Union[list[list[float]], np.ndarray]:
     """
     Create a list of colors for a list of items.
 
     Can also check a user-provided list of colors and use this if
     everything is ok.
 
     Parameters
@@ -194,14 +194,14 @@
         # dummy cluster had twice as many entries as really there. Reduce.
         real_indices = np.arange(int(colors.shape[0] / 2))
         return colors[real_indices]
 
     # if the user specified color lies does not match the number of results
     if len(colors) != num_entries:
         raise (
-            'Incorrect color input. Colors must be specified either as '
-            'list of [r, g, b, alpha] with length equal to function '
-            'values Number of function (here: ' + str(num_entries) + '), '
-            'or as one single [r, g, b, alpha] color.'
+            "Incorrect color input. Colors must be specified either as "
+            "list of [r, g, b, alpha] with length equal to function "
+            "values Number of function (here: " + str(num_entries) + "), "
+            "or as one single [r, g, b, alpha] color."
         )
 
     return colors
```

### Comparing `pypesto-0.4.2/pypesto/visualize/dimension_reduction.py` & `pypesto-0.5.0/pypesto/visualize/dimension_reduction.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Optional, Sequence, Tuple
+from collections.abc import Sequence
+from typing import TYPE_CHECKING
 
 import matplotlib.pyplot as plt
 import numpy as np
 
 from .clust_color import RGBA
 
 if TYPE_CHECKING:
@@ -39,27 +40,27 @@
     axs:
         Either one axes object, or a dictionary of plot axes (depending on the
         number of coordinates passed)
     """
     n_components = len(components)
     if n_components == 2:
         # handle components
-        x_label = f'UMAP component {components[0] + 1}'
-        y_label = f'UMAP component {components[1] + 1}'
+        x_label = f"UMAP component {components[0] + 1}"
+        y_label = f"UMAP component {components[1] + 1}"
         dataset = umap_coordinates[:, components]
 
         # call lowlevel routine
         return ensemble_scatter_lowlevel(
             dataset, x_label=x_label, y_label=y_label, **kwargs
         )
     else:
         # We got more than two components. Plot a cross-classification table
         # Create the labels first
         component_labels = [
-            f'UMAP component {components[i_comp] + 1}'
+            f"UMAP component {components[i_comp] + 1}"
             for i_comp in range(n_components)
         ]
         # reduce pca components
         dataset = umap_coordinates[:, components]
         # run lowlevel plot
         return ensemble_crosstab_scatter_lowlevel(
             dataset, component_labels, **kwargs
@@ -95,15 +96,15 @@
     """
     import umap.plot
 
     # reduce, if necessary
     umap_object.embedding_ = umap_object.embedding_[:, components]
 
     # use umap's original plotting routine to visualize
-    umap.plot.points(umap_object, values=color_by, theme='viridis', **kwargs)
+    umap.plot.points(umap_object, values=color_by, theme="viridis", **kwargs)
 
 
 def projection_scatter_pca(
     pca_coordinates: np.ndarray, components: Sequence[int] = (0, 1), **kwargs
 ):
     """
     Plot a scatter plot for PCA coordinates.
@@ -124,28 +125,28 @@
     axs:
         Either one axes object, or a dictionary of plot axes (depending on the
         number of coordinates passed)
     """
     n_components = len(components)
     if n_components == 2:
         # handle components
-        x_label = f'PCA component {components[0] + 1}'
-        y_label = f'PCA component {components[1] + 1}'
+        x_label = f"PCA component {components[0] + 1}"
+        y_label = f"PCA component {components[1] + 1}"
 
         dataset = pca_coordinates[:, components]
 
         # call lowlevel routine
         return ensemble_scatter_lowlevel(
             dataset, x_label=x_label, y_label=y_label, **kwargs
         )
     else:
         # We got more than two components. Plot a cross-classification table
         # Create the labels first
         component_labels = [
-            f'PCA component {components[i_comp] + 1}'
+            f"PCA component {components[i_comp] + 1}"
             for i_comp in range(n_components)
         ]
         # reduce pca components
         dataset = pca_coordinates[:, components]
         # run lowlevel plot
         return ensemble_crosstab_scatter_lowlevel(
             dataset, component_labels, **kwargs
@@ -175,22 +176,22 @@
     """
     # We got more than two components. Create a cross-classification table
     n_components = dataset.shape[1]
     axs = _create_crosstab_axes(n_components)
 
     # wo don't even try to plot this into an existing axes object.
     # Overplotting a multi-axes figure is asking for trouble...
-    if 'ax' in kwargs.keys():
-        del kwargs['ax']
+    if "ax" in kwargs.keys():
+        del kwargs["ax"]
 
     for x_comp in range(0, n_components - 1):
         for y_comp in range(x_comp + 1, n_components):
             # handle axis labels
-            x_label = ''
-            y_label = ''
+            x_label = ""
+            y_label = ""
             if x_comp == 0:
                 y_label = component_labels[y_comp]
             if y_comp == n_components - 1:
                 x_label = component_labels[x_comp]
 
             # extract the wanted columns
             tmp_dataset = dataset[:, [x_comp, y_comp]]
@@ -205,22 +206,22 @@
             )
     # return dict of axes
     return axs
 
 
 def ensemble_scatter_lowlevel(
     dataset,
-    ax: Optional[plt.Axes] = None,
-    size: Optional[Tuple[float]] = (12, 6),
-    x_label: str = 'component 1',
-    y_label: str = 'component 2',
+    ax: plt.Axes | None = None,
+    size: tuple[float] | None = (12, 6),
+    x_label: str = "component 1",
+    y_label: str = "component 2",
     color_by: Sequence[float] = None,
-    color_map: str = 'viridis',
+    color_map: str = "viridis",
     background_color: RGBA = (0.0, 0.0, 0.0, 1.0),
-    marker_type: str = '.',
+    marker_type: str = ".",
     scatter_size: float = 0.5,
     invert_scatter_order: bool = False,
 ):
     """
     Create a scatter plot.
 
     Parameters
```

### Comparing `pypesto-0.4.2/pypesto/visualize/ensemble.py` & `pypesto-0.5.0/pypesto/visualize/ensemble.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Optional, Tuple
+from typing import Optional
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from matplotlib.collections import PatchCollection
 from matplotlib.patches import Rectangle
 
 from ..C import COLOR_HIT_BOTH_BOUNDS, COLOR_HIT_NO_BOUNDS, COLOR_HIT_ONE_BOUND
 from ..ensemble import Ensemble
 
 
 def ensemble_identifiability(
     ensemble: Ensemble,
     ax: Optional[plt.Axes] = None,
-    size: Optional[Tuple[float]] = (12, 6),
+    size: Optional[tuple[float]] = (12, 6),
 ):
     """
     Visualize identifiablity of parameter ensemble.
 
     Plot an overview about how many parameters hit the parameter bounds based
     on an ensemble of parameters. confidence intervals/credible ranges are
     computed via the ensemble mean plus/minus 1 standard deviation.
@@ -54,15 +54,15 @@
 
 def ensemble_identifiability_lowlevel(
     none_hit: np.ndarray,
     lb_hit: np.ndarray,
     ub_hit: np.ndarray,
     both_hit: np.ndarray,
     ax: Optional[plt.Axes] = None,
-    size: Optional[Tuple[float]] = (16, 10),
+    size: Optional[tuple[float]] = (16, 10),
 ):
     """
     Low-level identifiablity routine.
 
     Plot an overview about how many parameters hit the parameter bounds based
     on a ensemble of parameters. Confidence intervals/credible ranges are
     computed via the ensemble mean plus/minus 1 standard deviation.
@@ -129,90 +129,90 @@
     if patches_ub_hit:
         ax.add_collection(patches_ub_hit)
     if patches_none_hit:
         ax.add_collection(patches_none_hit)
 
     # plot dashed lines indicating the number rof non-identifiable parameters
     vert = [-0.05, 1.05]
-    ax.plot([x_both, x_both], vert, 'k--', linewidth=1.5)
-    ax.plot([x_both + x_lb, x_both + x_lb], vert, 'k--', linewidth=1.5)
+    ax.plot([x_both, x_both], vert, "k--", linewidth=1.5)
+    ax.plot([x_both + x_lb, x_both + x_lb], vert, "k--", linewidth=1.5)
     ax.plot(
         [x_both + x_lb + x_ub, x_both + x_lb + x_ub],
         vert,
-        'k--',
+        "k--",
         linewidth=1.5,
     )
 
     # add text
     if patches_both_hit:
         ax.text(
             x_both / 2,
             -0.05,
-            'both bounds hit',
+            "both bounds hit",
             color=COLOR_HIT_BOTH_BOUNDS,
             rotation=-90,
-            va='top',
-            ha='center',
+            va="top",
+            ha="center",
         )
     if patches_lb_hit:
         ax.text(
             x_both + x_lb / 2,
             -0.05,
-            'lower bound hit',
+            "lower bound hit",
             color=COLOR_HIT_ONE_BOUND,
             rotation=-90,
-            va='top',
-            ha='center',
+            va="top",
+            ha="center",
         )
     if patches_ub_hit:
         ax.text(
             x_both + x_lb + x_ub / 2,
             -0.05,
-            'upper bound hit',
+            "upper bound hit",
             color=COLOR_HIT_ONE_BOUND,
             rotation=-90,
-            va='top',
-            ha='center',
+            va="top",
+            ha="center",
         )
     if patches_none_hit:
         ax.text(
             1 - x_none / 2,
             -0.05,
-            'no bounds hit',
+            "no bounds hit",
             color=COLOR_HIT_NO_BOUNDS,
             rotation=-90,
-            va='top',
-            ha='center',
+            va="top",
+            ha="center",
         )
     ax.text(
         0,
         -0.7,
-        'identifiable parameters: {:4.1f}%'.format(x_none * 100),
-        va='top',
+        f"identifiable parameters: {x_none * 100:4.1f}%",
+        va="top",
     )
 
     # plot upper and lower bounds
-    ax.text(-0.03, 1.0, 'upper\nbound', ha='right', va='center')
-    ax.text(-0.03, 0.0, 'lower\nbound', ha='right', va='center')
-    ax.plot([-0.02, 1.03], [0, 0], 'k:', linewidth=1.5)
-    ax.plot([-0.02, 1.03], [1, 1], 'k:', linewidth=1.5)
+    ax.text(-0.03, 1.0, "upper\nbound", ha="right", va="center")
+    ax.text(-0.03, 0.0, "lower\nbound", ha="right", va="center")
+    ax.plot([-0.02, 1.03], [0, 0], "k:", linewidth=1.5)
+    ax.plot([-0.02, 1.03], [1, 1], "k:", linewidth=1.5)
     plt.xticks([])
     plt.yticks([])
 
     # plot frame
-    ax.plot([0, 0], vert, 'k-', linewidth=1.5)
-    ax.plot([1, 1], vert, 'k-', linewidth=1.5)
+    ax.plot([0, 0], vert, "k-", linewidth=1.5)
+    ax.plot([1, 1], vert, "k-", linewidth=1.5)
 
     # beautify axes
     plt.xlim((-0.15, 1.1))
     plt.ylim((-0.78, 1.15))
-    ax.spines['right'].set_visible(False)
-    ax.spines['left'].set_visible(False)
-    ax.spines['bottom'].set_visible(False)
-    ax.spines['top'].set_visible(False)
+    ax.spines["right"].set_visible(False)
+    ax.spines["left"].set_visible(False)
+    ax.spines["bottom"].set_visible(False)
+    ax.spines["top"].set_visible(False)
 
     return ax
 
 
 def _prepare_identifiability_plot(id_df: pd.DataFrame):
     """
     Group model parameters based on an ensemble object .
@@ -251,18 +251,18 @@
     both_hit = []
     lb_hit = []
     ub_hit = []
     none_hit = []
 
     def _affine_transform(par_info):
         # rescale parameters to bounds
-        lb = par_info['lowerBound']
-        ub = par_info['upperBound']
-        val_l = par_info['ensemble_mean'] - par_info['ensemble_std']
-        val_u = par_info['ensemble_mean'] + par_info['ensemble_std']
+        lb = par_info["lowerBound"]
+        ub = par_info["upperBound"]
+        val_l = par_info["ensemble_mean"] - par_info["ensemble_std"]
+        val_u = par_info["ensemble_mean"] + par_info["ensemble_std"]
         # check if parameter confidence intervals/credible ranges hit bound
         if val_l <= lb:
             lower_val = 0.0
         else:
             lower_val = (val_l - lb) / (ub - lb)
         if val_u >= ub:
             upper_val = 1.0
@@ -270,21 +270,21 @@
             upper_val = (val_u - lb) / (ub - lb)
 
         return lower_val, upper_val
 
     for par_id in list(id_df.index):
         # check which of the parameters seems to be identifiable and group them
         if (
-            id_df.loc[par_id, 'within lb: 1 std']
-            and id_df.loc[par_id, 'within ub: 1 std']
+            id_df.loc[par_id, "within lb: 1 std"]
+            and id_df.loc[par_id, "within ub: 1 std"]
         ):
             none_hit.append(_affine_transform(id_df.loc[par_id, :]))
-        elif id_df.loc[par_id, 'within lb: 1 std']:
+        elif id_df.loc[par_id, "within lb: 1 std"]:
             ub_hit.append(_affine_transform(id_df.loc[par_id, :]))
-        elif id_df.loc[par_id, 'within ub: 1 std']:
+        elif id_df.loc[par_id, "within ub: 1 std"]:
             lb_hit.append(_affine_transform(id_df.loc[par_id, :]))
         else:
             both_hit.append(_affine_transform(id_df.loc[par_id, :]))
 
     return (
         np.array(none_hit),
         np.array(lb_hit),
```

### Comparing `pypesto-0.4.2/pypesto/visualize/misc.py` & `pypesto-0.5.0/pypesto/visualize/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import warnings
+from collections.abc import Iterable
 from numbers import Number
-from typing import Iterable, List, Optional, Union
+from typing import Optional, Union
 
 import numpy as np
 
 from ..C import (
     ALL,
     ALL_CLUSTERED,
     FIRST_CLUSTER,
@@ -20,15 +21,15 @@
 )
 from ..result import Result
 from ..util import assign_clusters, delete_nan_inf
 from .clust_color import assign_colors_for_list
 
 
 def process_result_list(
-    results: Union[Result, List[Result]], colors=None, legends=None
+    results: Union[Result, list[Result]], colors=None, legends=None
 ):
     """
     Assign colors and legends to a list of results, check user provided lists.
 
     Parameters
     ----------
     results: list or pypesto.Result
@@ -77,24 +78,24 @@
         colors = assign_colors_for_list(len(results), colors)
 
         # check whether list of legends has the correct length
         if legends is None:
             # No legends were passed: create some custom legends
             legends = []
             for i_leg in range(len(results)):
-                legends.append('Result ' + str(i_leg))
+                legends.append("Result " + str(i_leg))
         else:
             # legends were passed by user: check length
             try:
                 if isinstance(legends, str):
                     legends = [legends]
                 if len(legends) != len(results):
                     raise ValueError(
-                        'List of results passed and list of labels do '
-                        'not have the same length.'
+                        "List of results passed and list of labels do "
+                        "not have the same length."
                     )
             except TypeError:
                 legend_type_error = True
 
     if legend_type_error:
         raise TypeError("Unexpected legend type.")
 
@@ -122,26 +123,27 @@
     -------
     offset_y: float
        value for offsetting the later plotted values, in order to ensure
        positivity if a semilog-plot is used
     """
     # check whether the offset specified by the user is sufficient
     if offset_y is not None:
-        if (scale_y == 'log10') and (min_val + offset_y <= 0.0):
+        if (scale_y == "log10") and (min_val + offset_y <= 0.0):
             warnings.warn(
                 "Offset specified by user is insufficient. "
                 "Ignoring specified offset and using "
                 + str(np.abs(min_val) + 1.0)
-                + " instead."
+                + " instead.",
+                stacklevel=2,
             )
         else:
             return offset_y
     else:
         # check whether scaling is lin or log10
-        if scale_y == 'lin':
+        if scale_y == "lin":
             # linear scaling doesn't need any offset
             return 0.0
 
     return 1.0 - min_val
 
 
 def process_y_limits(ax, y_limits):
@@ -171,42 +173,44 @@
             # if the user specified only an upper bound
             tmp_y_limits = ax.get_ylim()
             y_limits = [tmp_y_limits[0], y_limits]
         elif y_limits.size > 1:
             y_limits = [y_limits[0], y_limits[1]]
 
         # check validity of bounds if plotting in log-scale
-        if ax.get_yscale() == 'log' and y_limits[0] <= 0.0:
+        if ax.get_yscale() == "log" and y_limits[0] <= 0.0:
             tmp_y_limits = ax.get_ylim()
             if y_limits[1] <= 0.0:
                 y_limits = tmp_y_limits
                 warnings.warn(
                     "Invalid bounds for plotting in "
-                    "log-scale. Using defaults bounds."
+                    "log-scale. Using defaults bounds.",
+                    stacklevel=2,
                 )
             else:
                 y_limits = [tmp_y_limits[0], y_limits[1]]
                 warnings.warn(
                     "Invalid lower bound for plotting in "
-                    "log-scale. Using only upper bound."
+                    "log-scale. Using only upper bound.",
+                    stacklevel=2,
                 )
 
         # set limits
         ax.set_ylim(y_limits)
 
     else:
         # No limits passed, but if we have a result list: check the limits
         ax_limits = np.array(ax.get_ylim())
         data_limits = ax.dataLim.ymin, ax.dataLim.ymax
 
         # Check if data fits to axes and adapt limits, if necessary
         if ax_limits[0] > data_limits[0] or ax_limits[1] < data_limits[1]:
             # Get range of data
             data_range = data_limits[1] - data_limits[0]
-            if ax.get_yscale() == 'log':
+            if ax.get_yscale() == "log":
                 data_range = np.log10(data_range)
                 new_limits = (
                     np.power(10, np.log10(data_limits[0]) - 0.02 * data_range),
                     np.power(10, np.log10(data_limits[1]) + 0.02 * data_range),
                 )
             else:
                 new_limits = (
@@ -239,24 +243,24 @@
     if len(bg) == LEN_RGBA:
         # return foreground if background is fully transparent
         if bg[RGBA_ALPHA] == RGBA_MIN:
             return fg
     else:
         if len(bg) != LEN_RGB:
             raise IndexError(
-                'A background color of unexpected length was provided: {bg}'
+                "A background color of unexpected length was provided: {bg}"
             )
         bg = (*bg, RGBA_MAX)
 
     # return the foreground color if has no transparency
     if len(fg) == LEN_RGB or fg[RGBA_ALPHA] == RGBA_MAX:
         return fg
     if len(fg) != LEN_RGBA:
         raise IndexError(
-            'A foreground color of unexpected length was provided: {fg}'
+            "A foreground color of unexpected length was provided: {fg}"
         )
 
     def apparent_composite_color_component(
         fg_component: float,
         bg_component: float,
         fg_alpha: float = fg[RGBA_ALPHA],
         bg_alpha: float = bg[RGBA_ALPHA],
```

### Comparing `pypesto-0.4.2/pypesto/visualize/model_fit.py` & `pypesto-0.5.0/pypesto/visualize/model_fit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """
 Visualization of the model fit after optimization.
 
 Currently only for PEtab problems.
 """
 
 import copy
-from typing import Sequence, Union
+from collections.abc import Sequence
+from typing import Union
 
 import amici
 import amici.plotting
 import matplotlib.axes
 import matplotlib.pyplot as plt
 import numpy as np
 import petab
-from amici.petab_objective import rdatas_to_simulation_df
+from amici.petab.simulations import rdatas_to_simulation_df
 from petab.visualize import plot_problem
 
 from ..C import CENSORED, ORDINAL, RDATAS, SEMIQUANTITATIVE
-from ..hierarchical.relative.calculator import RelativeAmiciCalculator
 from ..petab.importer import get_petab_non_quantitative_data_types
-from ..problem import Problem
+from ..problem import HierarchicalProblem, Problem
 from ..result import Result
 from .ordinal_categories import plot_categories_from_pypesto_result
 from .spline_approximation import _add_spline_mapped_simulations_to_model_fit
 
-AmiciModel = Union['amici.Model', 'amici.ModelPtr']
+AmiciModel = Union["amici.Model", "amici.ModelPtr"]
 
 __all__ = ["visualize_optimized_model_fit", "time_trajectory_model"]
 
 
 def visualize_optimized_model_fit(
     petab_problem: petab.Problem,
     result: Union[Result, Sequence[Result]],
@@ -67,15 +67,15 @@
         Passed to :func:`petab.visualize.plot_problem`.
 
     Returns
     -------
     axes: `matplotlib.axes.Axes` object of the created plot.
     None: In case subplots are saved to file
     """
-    x = result.optimize_result.list[start_index]['x'][
+    x = result.optimize_result.list[start_index]["x"][
         pypesto_problem.x_free_indices
     ]
     objective_result = pypesto_problem.objective(x, return_dict=True)
 
     simulation_df = rdatas_to_simulation_df(
         objective_result[RDATAS],
         pypesto_problem.objective.amici_model,
@@ -118,17 +118,17 @@
                 pypesto_problem=pypesto_problem,
                 start_index=start_index,
                 axes=axes,
             )
 
     if return_dict:
         return {
-            'axes': axes,
-            'objective_result': objective_result,
-            'simulation_df': simulation_df,
+            "axes": axes,
+            "objective_result": objective_result,
+            "simulation_df": simulation_df,
         }
     return axes
 
 
 def time_trajectory_model(
     result: Union[Result, Sequence[Result]],
     problem: Problem = None,
@@ -231,34 +231,36 @@
     """
     # add timepoints as needed
     if simulation_timepoints is None:
         end_time = max(problem.objective.edatas[0].getTimepoints())
         simulation_timepoints = np.linspace(start=0, stop=end_time, num=1000)
 
     # get optimization result
-    parameters = result.optimize_result.list[start_index]['x']
+    parameters = result.optimize_result.list[start_index]["x"]
 
     # reduce vector to only include free indices. Needed downstream.
     parameters = problem.get_reduced_vector(parameters)
 
     # simulate with custom timepoints for hierarchical model
-    if isinstance(problem.objective.calculator, RelativeAmiciCalculator):
+    if isinstance(problem, HierarchicalProblem):
         # get parameter dictionary
         x_dct = dict(
             zip(problem.x_names, result.optimize_result.list[start_index].x)
         )
 
         # evaluate objective with return dict = True to get inner parameters
         ret = problem.objective(
-            parameters, mode='mode_fun', sensi_orders=(0,), return_dict=True
+            parameters, mode="mode_fun", sensi_orders=(0,), return_dict=True
         )
 
         # update parameter dictionary with inner parameters
-        inner_parameters = ret['inner_parameters']
-        x_dct.update(inner_parameters)
+        inner_parameter_dict = dict(
+            zip(problem.inner_x_names, ret["inner_parameters"])
+        )
+        x_dct.update(inner_parameter_dict)
 
         parameter_mapping = problem.objective.parameter_mapping
         edatas = copy.deepcopy(problem.objective.edatas)
         amici_model = problem.objective.amici_model
 
         # disable sensitivities to improve computation time
         amici_solver = copy.deepcopy(problem.objective.amici_solver)
@@ -284,24 +286,24 @@
         # set custom timepoints
         obj = problem.objective.set_custom_timepoints(
             timepoints_global=simulation_timepoints
         )
 
         # evaluate objective with return dict = True to get data
         ret = obj(
-            parameters, mode='mode_fun', sensi_orders=(0,), return_dict=True
+            parameters, mode="mode_fun", sensi_orders=(0,), return_dict=True
         )
-        rdatas = ret['rdatas']
+        rdatas = ret["rdatas"]
 
     return rdatas
 
 
 def _time_trajectory_model_with_states(
     model: AmiciModel,
-    rdatas: Union['amici.ReturnData', Sequence['amici.ReturnData']],
+    rdatas: Union["amici.ReturnData", Sequence["amici.ReturnData"]],
     state_ids: Sequence[str],
     state_names: Sequence[str],
     observable_ids: Union[str, Sequence[str]],
 ):
     """
     Visualizes both, states and observables.
 
@@ -368,15 +370,15 @@
             model=model,
         )
     return axes
 
 
 def _time_trajectory_model_without_states(
     model: AmiciModel,
-    rdatas: Union['amici.ReturnData', Sequence['amici.ReturnData']],
+    rdatas: Union["amici.ReturnData", Sequence["amici.ReturnData"]],
     observable_ids: Union[str, Sequence[str]],
 ):
     """
     Visualize both, states and observables.
 
     Helper function for time_trajectory_model.
```

### Comparing `pypesto-0.4.2/pypesto/visualize/optimization_stats.py` & `pypesto-0.5.0/pypesto/visualize/optimization_stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
+from collections.abc import Iterable, Sequence
 from numbers import Real
-from typing import Dict, Iterable, List, Optional, Sequence, Tuple, Union
+from typing import Optional, Union
 
 import matplotlib.axes
 import matplotlib.pyplot as plt
 import numpy as np
 
 from pypesto.util import delete_nan_inf
 
 from ..result import Result
 from .clust_color import assign_colors, assign_colors_for_list
 from .misc import process_result_list, process_start_indices
 
 
 def optimization_run_properties_one_plot(
     results: Result,
-    properties_to_plot: Optional[List[str]] = None,
-    size: Tuple[float, float] = (18.5, 10.5),
+    properties_to_plot: Optional[list[str]] = None,
+    size: tuple[float, float] = (18.5, 10.5),
     start_indices: Optional[Union[int, Iterable[int]]] = None,
-    colors: Optional[Union[List[float], List[List[float]]]] = None,
-    legends: Optional[Union[str, List[str]]] = None,
-    plot_type: str = 'line',
+    colors: Optional[Union[list[float], list[list[float]]]] = None,
+    legends: Optional[Union[str, list[str]]] = None,
+    plot_type: str = "line",
 ) -> matplotlib.axes.Axes:
     """
     Plot stats for allproperties specified in properties_to_plot on one plot.
 
     Parameters
     ----------
     results:
@@ -60,42 +61,42 @@
     optimization_properties_per_multistart(
         result1,
         properties_to_plot=['time', 'n_grad'],
         colors=[[.5, .9, .9, .3], [.2, .1, .9, .5]])
     """
     if properties_to_plot is None:
         properties_to_plot = [
-            'time',
-            'n_fval',
-            'n_grad',
-            'n_hess',
-            'n_res',
-            'n_sres',
+            "time",
+            "n_fval",
+            "n_grad",
+            "n_hess",
+            "n_res",
+            "n_sres",
         ]
 
     if colors is None:
         colors = assign_colors_for_list(len(properties_to_plot))
     elif len(colors) == 4 and isinstance(colors[0], Real):
         colors = [colors]
 
     if len(colors) != len(properties_to_plot):
         raise ValueError(
-            'Number of RGBA colors should be the same as number '
-            'of optimization properties to plot'
+            "Number of RGBA colors should be the same as number "
+            "of optimization properties to plot"
         )
 
     if legends is None:
         legends = properties_to_plot
     elif not isinstance(legends, list):
         legends = [legends]
 
     if len(legends) != len(properties_to_plot):
         raise ValueError(
-            'Number of legends should be the same as number of '
-            'optimization properties to plot'
+            "Number of legends should be the same as number of "
+            "optimization properties to plot"
         )
 
     ax = plt.subplots()[1]
     fig = plt.gcf()
     fig.set_size_inches(*size)
 
     for idx, prop_name in enumerate(properties_to_plot):
@@ -113,21 +114,21 @@
     ax.set_ylabel("property value")
     ax.set_title("Optimization properties per optimization run")
     return ax
 
 
 def optimization_run_properties_per_multistart(
     results: Union[Result, Sequence[Result]],
-    properties_to_plot: Optional[List[str]] = None,
-    size: Tuple[float, float] = (18.5, 10.5),
+    properties_to_plot: Optional[list[str]] = None,
+    size: tuple[float, float] = (18.5, 10.5),
     start_indices: Optional[Union[int, Iterable[int]]] = None,
-    colors: Optional[Union[List[float], List[List[float]]]] = None,
-    legends: Optional[Union[str, List[str]]] = None,
-    plot_type: str = 'line',
-) -> Dict[str, plt.Subplot]:
+    colors: Optional[Union[list[float], list[list[float]]]] = None,
+    legends: Optional[Union[str, list[str]]] = None,
+    plot_type: str = "line",
+) -> dict[str, plt.Subplot]:
     """
     One plot per optimization property in properties_to_plot.
 
     Parameters
     ----------
     results:
         Optimization result obtained by 'optimize.py' or list of those
@@ -172,20 +173,20 @@
 
     optimization_properties_per_multistart(
         [result1, result2], properties_to_plot=['time', 'n_fval'],
         colors=[[.5, .9, .9, .3], [.2, .1, .9, .5]])
     """
     if properties_to_plot is None:
         properties_to_plot = [
-            'time',
-            'n_fval',
-            'n_grad',
-            'n_hess',
-            'n_res',
-            'n_sres',
+            "time",
+            "n_fval",
+            "n_grad",
+            "n_hess",
+            "n_res",
+            "n_sres",
         ]
 
     num_subplot = len(properties_to_plot)
     # compute, how many rows and columns we need for the subplots
     num_row = int(np.round(np.sqrt(num_subplot)))
     num_col = int(np.ceil(num_subplot / num_row))
     fig, axes = plt.subplots(num_row, num_col, squeeze=False)
@@ -209,19 +210,19 @@
     return axes
 
 
 def optimization_run_property_per_multistart(
     results: Union[Result, Sequence[Result]],
     opt_run_property: str,
     axes: Optional[matplotlib.axes.Axes] = None,
-    size: Tuple[float, float] = (18.5, 10.5),
+    size: tuple[float, float] = (18.5, 10.5),
     start_indices: Optional[Union[int, Iterable[int]]] = None,
-    colors: Optional[Union[List[float], List[List[float]]]] = None,
-    legends: Optional[Union[str, List[str]]] = None,
-    plot_type: str = 'line',
+    colors: Optional[Union[list[float], list[list[float]]]] = None,
+    legends: Optional[Union[str, list[str]]] = None,
+    plot_type: str = "line",
 ) -> matplotlib.axes.Axes:
     """
     Plot stats for an optimization run property specified by opt_run_property.
 
     It is possible to plot a histogram or a line plot. In a line plot,
     on the x axis are the numbers of the multistarts, where the multistarts are
     ordered with respect to a function value. On the y axis of the line plot
@@ -253,48 +254,48 @@
 
     Returns
     -------
     axes:
         The plot axes.
     """
     supported_properties = {
-        'time': 'Wall-clock time (seconds)',
-        'n_fval': 'Number of function evaluations',
-        'n_grad': 'Number of gradient evaluations',
-        'n_hess': 'Number of Hessian evaluations',
-        'n_res': 'Number of residuals evaluations',
-        'n_sres': 'Number of residual sensitivity evaluations',
+        "time": "Wall-clock time (seconds)",
+        "n_fval": "Number of function evaluations",
+        "n_grad": "Number of gradient evaluations",
+        "n_hess": "Number of Hessian evaluations",
+        "n_res": "Number of residuals evaluations",
+        "n_sres": "Number of residual sensitivity evaluations",
     }
 
     if opt_run_property not in supported_properties:
         raise ValueError(
             "Wrong value of opt_run_property. Only the following "
             "values are allowed: 'time', 'n_fval', 'n_grad', "
             "'n_hess', 'n_res', 'n_sres'"
         )
 
     # parse input
     (results, colors, legends) = process_result_list(results, colors, legends)
 
     # axes
     if axes is None:
-        ncols = 2 if plot_type == 'both' else 1
+        ncols = 2 if plot_type == "both" else 1
         fig, axes = plt.subplots(1, ncols)
         fig.set_size_inches(*size)
         fig.suptitle(
-            f'{supported_properties[opt_run_property]} per optimizer run'
+            f"{supported_properties[opt_run_property]} per optimizer run"
         )
     else:
         axes.set_title(
-            f'{supported_properties[opt_run_property]} per optimizer run'
+            f"{supported_properties[opt_run_property]} per optimizer run"
         )
 
     # loop over results
     for j, result in enumerate(results):
-        if plot_type == 'both':
+        if plot_type == "both":
             axes[0] = stats_lowlevel(
                 result,
                 opt_run_property,
                 supported_properties[opt_run_property],
                 axes[0],
                 start_indices,
                 colors[j],
@@ -305,47 +306,47 @@
                 result,
                 opt_run_property,
                 supported_properties[opt_run_property],
                 axes[1],
                 start_indices,
                 colors[j],
                 legends[j],
-                plot_type='hist',
+                plot_type="hist",
             )
         else:
             axes = stats_lowlevel(
                 result,
                 opt_run_property,
                 supported_properties[opt_run_property],
                 axes,
                 start_indices,
                 colors[j],
                 legends[j],
                 plot_type,
             )
 
-    if sum((legend is not None for legend in legends)) > 0:
-        if plot_type == 'both':
+    if sum(legend is not None for legend in legends) > 0:
+        if plot_type == "both":
             for ax in axes:
                 ax.legend()
         else:
             axes.legend()
 
     return axes
 
 
 def stats_lowlevel(
     result: Result,
     property_name: str,
     axis_label: str,
     ax: matplotlib.axes.Axes,
     start_indices: Optional[Union[int, Iterable[int]]] = None,
-    color: Union[str, List[float], List[List[float]]] = 'C0',
+    color: Union[str, list[float], list[list[float]]] = "C0",
     legend: Optional[str] = None,
-    plot_type: str = 'line',
+    plot_type: str = "line",
 ):
     """
     Plot values of the optimization run property across different multistarts.
 
     Parameters
     ----------
     result:
@@ -387,26 +388,26 @@
 
     # assign colors
     colors = assign_colors(vals=fvals, colors=color, balance_alpha=False)
 
     sorted_indices = sorted(range(n_starts), key=lambda j: fvals[j])
     values = values[sorted_indices]
 
-    if plot_type == 'line':
+    if plot_type == "line":
         # plot line
         ax.plot(range(n_starts), values, color=[0.7, 0.7, 0.7, 0.6])
 
         # plot points
         for i, v in enumerate(values):
             if i == 0:
                 tmp_legend = legend
             else:
                 tmp_legend = None
-            ax.scatter(i, v, color=colors[i], marker='o', label=tmp_legend)
-        ax.set_xlabel('Ordered optimizer run')
+            ax.scatter(i, v, color=colors[i], marker="o", label=tmp_legend)
+        ax.set_xlabel("Ordered optimizer run")
         ax.set_ylabel(axis_label)
     else:
-        ax.hist(values, color=color, bins='auto', label=legend)
+        ax.hist(values, color=color, bins="auto", label=legend)
         ax.set_xlabel(axis_label)
-        ax.set_ylabel('Number of multistarts')
+        ax.set_ylabel("Number of multistarts")
 
     return ax
```

### Comparing `pypesto-0.4.2/pypesto/visualize/optimizer_convergence.py` & `pypesto-0.5.0/pypesto/visualize/optimizer_convergence.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from typing import Optional, Tuple
+from typing import Optional
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
 from ..result import Result
 
 
 def optimizer_convergence(
     result: Result,
     ax: Optional[plt.Axes] = None,
-    xscale: str = 'symlog',
-    yscale: str = 'log',
-    size: Tuple[float] = (18.5, 10.5),
+    xscale: str = "symlog",
+    yscale: str = "log",
+    size: tuple[float] = (18.5, 10.5),
 ) -> plt.Axes:
     """
     Visualize to help spotting convergence issues.
 
     Scatter plot of function values and gradient values at the end of
     optimization. Optimizer exit-message is encoded by color. Can help
     identifying convergence issues in optimization and guide tolerance
@@ -62,15 +62,15 @@
             if grad is not None
             else np.NaN
         )
         for grad in result.optimize_result.grad
     ]
     msgs = result.optimize_result.message
     conv_data = pd.DataFrame(
-        {'fval': fvals, 'gradient norm': grad_norms, 'exit message': msgs}
+        {"fval": fvals, "gradient norm": grad_norms, "exit message": msgs}
     )
     sns.scatterplot(
-        x='fval', y='gradient norm', hue='exit message', data=conv_data, ax=ax
+        x="fval", y="gradient norm", hue="exit message", data=conv_data, ax=ax
     )
     ax.set_yscale(yscale)
     ax.set_xscale(xscale)
     return ax
```

### Comparing `pypesto-0.4.2/pypesto/visualize/optimizer_history.py` & `pypesto-0.5.0/pypesto/visualize/optimizer_history.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
-from typing import Iterable, List, Optional, Tuple, Union
+from collections.abc import Iterable
+from typing import Optional, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.ticker import MaxNLocator
 
 from ..C import (
     RGBA,
@@ -18,28 +19,28 @@
 from .misc import process_offset_y, process_result_list, process_y_limits
 from .reference_points import ReferencePoint, create_references
 
 logger = logging.getLogger(__name__)
 
 
 def optimizer_history(
-    results: Union[Result, List[Result]],
+    results: Union[Result, list[Result]],
     ax: Optional[plt.Axes] = None,
-    size: Tuple = (18.5, 10.5),
+    size: tuple = (18.5, 10.5),
     trace_x: str = TRACE_X_STEPS,
     trace_y: str = TRACE_Y_FVAL,
-    scale_y: str = 'log10',
+    scale_y: str = "log10",
     offset_y: Optional[float] = None,
-    colors: Optional[Union[RGBA, List[RGBA]]] = None,
-    y_limits: Optional[Union[float, List[float], np.ndarray]] = None,
-    start_indices: Optional[Union[int, List[int]]] = None,
+    colors: Optional[Union[RGBA, list[RGBA]]] = None,
+    y_limits: Optional[Union[float, list[float], np.ndarray]] = None,
+    start_indices: Optional[Union[int, list[int]]] = None,
     reference: Optional[
-        Union[ReferencePoint, dict, List[ReferencePoint], List[dict]]
+        Union[ReferencePoint, dict, list[ReferencePoint], list[dict]]
     ] = None,
-    legends: Optional[Union[str, List[str]]] = None,
+    legends: Optional[Union[str, list[str]]] = None,
 ) -> plt.Axes:
     """
     Plot history of optimizer.
 
     Can plot either the history of the cost function or of the gradient
     norm, over either the optimizer steps or the computation time.
 
@@ -120,21 +121,21 @@
     # handle options
     ax = handle_options(ax, vals, trace_y, ref, y_limits, offset_y)
 
     return ax
 
 
 def optimizer_history_lowlevel(
-    vals: List[np.ndarray],
-    scale_y: str = 'log10',
-    colors: Optional[Union[RGBA, List[RGBA]]] = None,
+    vals: list[np.ndarray],
+    scale_y: str = "log10",
+    colors: Optional[Union[RGBA, list[RGBA]]] = None,
     ax: Optional[plt.Axes] = None,
-    size: Tuple = (18.5, 10.5),
-    x_label: str = 'Optimizer steps',
-    y_label: str = 'Objective value',
+    size: tuple = (18.5, 10.5),
+    x_label: str = "Optimizer steps",
+    y_label: str = "Objective value",
     legend_text: Optional[str] = None,
 ) -> plt.Axes:
     """
     Plot optimizer history using list of numpy arrays.
 
     Parameters
     ----------
@@ -177,17 +178,17 @@
             val = np.asarray(val)
             fvals.append(val[1, -1])
     else:
         # convert to a list of numpy arrays
         vals = np.asarray(vals)
         if vals.shape[0] != 2 or vals.ndim != 2:
             raise ValueError(
-                'If numpy array is passed directly to lowlevel '
-                'routine of optimizer_history, shape needs to '
-                'be 2 x n.'
+                "If numpy array is passed directly to lowlevel "
+                "routine of optimizer_history, shape needs to "
+                "be 2 x n."
             )
         fvals = [vals[1, -1]]
         vals = [vals]
     n_fvals = len(fvals)
 
     # assign colors
     # note: this has to happen before sorting
@@ -205,32 +206,32 @@
         color = colors[j_fval]
         if j == 0:
             tmp_legend = legend_text
         else:
             tmp_legend = None
 
         # line plots
-        if scale_y == 'log10':
+        if scale_y == "log10":
             ax.semilogy(val[0, :], val[1, :], color=color, label=tmp_legend)
         else:
             ax.plot(val[0, :], val[1, :], color=color, label=tmp_legend)
 
     # set labels
     ax.set_xlabel(x_label)
     ax.set_ylabel(y_label)
-    ax.set_title('Optimizer history')
+    ax.set_title("Optimizer history")
     if legend_text is not None:
         ax.legend()
 
     return ax
 
 
 def get_trace(
     result: Result, trace_x: Optional[str], trace_y: Optional[str]
-) -> List[np.ndarray]:
+) -> list[np.ndarray]:
     """
     Get the values of the optimizer trace from the pypesto.Result object.
 
     Parameters
     ----------
     result: pypesto.Result
         Optimization result obtained by 'optimize.py'.
@@ -249,15 +250,15 @@
         list of (x,y)-values.
     x_label:
         label for x-axis to be plotted later.
     y_label:
         label for y-axis to be plotted later.
     """
     # get data frames
-    histories: List[HistoryBase] = result.optimize_result.history
+    histories: list[HistoryBase] = result.optimize_result.history
 
     vals = []
 
     for history in histories:
         options = history.options
         if trace_y == TRACE_Y_GRADNORM:
             # retrieve gradient trace, if saved
@@ -302,20 +303,20 @@
         # write down values
         vals.append(np.vstack([x_vals, y_vals]))
 
     return vals
 
 
 def get_vals(
-    vals: List[np.ndarray],
+    vals: list[np.ndarray],
     scale_y: Optional[str],
     offset_y: float,
     trace_y: str,
     start_indices: Iterable[int],
-) -> Tuple[List[np.ndarray], float]:
+) -> tuple[list[np.ndarray], float]:
     """
     Postprocess the values of the optimization history.
 
     Depending on the options set by the user (e.g. scale_y, offset_y,
     start_indices).
 
     Parameters
@@ -369,15 +370,15 @@
     if offset_y != 0:
         for val in vals:
             val[1, :] += offset_y * np.ones(val[1].shape)
 
     return vals, offset_y
 
 
-def get_labels(trace_x: str, trace_y: str, offset_y: float) -> Tuple[str, str]:
+def get_labels(trace_x: str, trace_y: str, offset_y: float) -> tuple[str, str]:
     """
     Generate labels for x and y axes of the history plot.
 
     Parameters
     ----------
     trace_x:
         What should be plotted on the x-axis. Possible values: TRACE_X.
@@ -385,40 +386,39 @@
         What should be plotted on the y-axis.
         Possible values: TRACE_Y_FVAL, TRACE_Y_GRADNORM.
     offset_y:
         Offset for the y-axis-values.
     Returns
     -------
     labels for x and y axes
-
     """
-    x_label = ''
-    y_label = ''
+    x_label = ""
+    y_label = ""
 
     if trace_x == TRACE_X_TIME:
-        x_label = 'Computation time [s]'
+        x_label = "Computation time [s]"
     else:
-        x_label = 'Optimizer steps'
+        x_label = "Optimizer steps"
 
     if trace_y == TRACE_Y_GRADNORM:
-        y_label = 'Gradient norm'
+        y_label = "Gradient norm"
     else:
-        y_label = 'Objective value'
+        y_label = "Objective value"
 
     if offset_y != 0:
-        y_label = 'Offsetted ' + y_label.lower()
+        y_label = "Offsetted " + y_label.lower()
 
     return x_label, y_label
 
 
 def handle_options(
     ax: plt.Axes,
-    vals: List[np.ndarray],
+    vals: list[np.ndarray],
     trace_y: str,
-    ref: List[ReferencePoint],
+    ref: list[ReferencePoint],
     y_limits: Union[float, np.ndarray, None],
     offset_y: float,
 ) -> plt.Axes:
     """
     Apply post-plotting transformations to the axis object.
 
     Get the limits for the y-axis, plots the reference points, will do
@@ -457,26 +457,26 @@
             for val in vals:
                 max_len = np.max([max_len, val[0, -1]])
 
             for i_ref in ref:
                 ax.plot(
                     [0, max_len],
                     [i_ref.fval + offset_y, i_ref.fval + offset_y],
-                    '--',
+                    "--",
                     color=i_ref.color,
                     label=i_ref.legend,
                 )
 
                 # create legend for reference points
                 if i_ref.legend is not None:
                     ax.legend()
     else:
         logger.warning(
-            f'Reference point is currently only implemented for trace_y == '
-            f'{TRACE_Y_FVAL} and will not be plotted for trace_y == {trace_y}.'
+            f"Reference point is currently only implemented for trace_y == "
+            f"{TRACE_Y_FVAL} and will not be plotted for trace_y == {trace_y}."
         )
 
     return ax
 
 
 def sacess_history(
     histories: list[HistoryBase],
```

### Comparing `pypesto-0.4.2/pypesto/visualize/ordinal_categories.py` & `pypesto-0.5.0/pypesto/visualize/ordinal_categories.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         The axes.
     """
 
     # Get the parameters from the pypesto result for the start_index.
     x_dct = dict(
         zip(
             pypesto_result.problem.objective.x_ids,
-            pypesto_result.optimize_result.list[start_index]['x'],
+            pypesto_result.optimize_result.list[start_index]["x"],
         )
     )
     x_dct.update(
         pypesto_result.problem.objective.calculator.necessary_par_dummy_values
     )
 
     # Get the needed objects from the pypesto problem.
@@ -101,15 +101,17 @@
         edatas,
         num_threads=min(n_threads, len(edatas)),
     )
 
     # If any amici simulation failed, raise warning and return None.
     if any(rdata.status != amici.AMICI_SUCCESS for rdata in inner_rdatas):
         warnings.warn(
-            'Warning: Some AMICI simulations failed. Cannot plot inner solutions.'
+            "Warning: Some AMICI simulations failed. Cannot plot inner "
+            "solutions.",
+            stacklevel=2,
         )
         return None
 
     # Get simulation and sigma.
     sim = [rdata[AMICI_Y] for rdata in inner_rdatas]
     sigma = [rdata[AMICI_SIGMAY] for rdata in inner_rdatas]
     timepoints = [rdata[AMICI_T] for rdata in inner_rdatas]
@@ -148,16 +150,16 @@
         measurement_df_observable_ordering,
         axes,
         **kwargs,
     )
 
 
 def plot_categories_from_inner_result(
-    inner_problem: 'pypesto.hierarchical.ordinal.problem.OrdinalProblem',
-    inner_solver: 'pypesto.hierarchical.ordinal.solver.OrdinalInnerSolver',
+    inner_problem: "pypesto.hierarchical.ordinal.problem.OrdinalProblem",
+    inner_solver: "pypesto.hierarchical.ordinal.solver.OrdinalInnerSolver",
     results: list[dict],
     simulation: list[np.ndarray],
     timepoints: list[np.ndarray],
     observable_ids: list[str] = None,
     condition_ids: list[str] = None,
     petab_condition_ordering: list[str] = None,
     measurement_df_observable_ordering: list[str] = None,
@@ -211,15 +213,15 @@
         if observable_ids is not None and use_given_axes:
             observable_id = observable_ids[group - 1]
             meas_obs_idx = measurement_df_observable_ordering.index(
                 observable_id
             )
 
             # Get the ax for the current observable.
-            ax = axes['plot' + str(meas_obs_idx + 1)]
+            ax = axes["plot" + str(meas_obs_idx + 1)]
         else:
             ax = axes[list(inner_problem.groups.keys()).index(group)]
 
         # For each group get the inner parameters and simulation
         xs = inner_problem.get_cat_ub_parameters_for_group(group)
 
         interval_range, interval_gap = compute_interval_constraints(
@@ -309,18 +311,18 @@
                     condition_ids,
                     use_given_axes,
                 )
 
             ax.legend()
 
             if not use_given_axes:
-                ax.set_title(f'Group {group}, {measurement_type} data')
+                ax.set_title(f"Group {group}, {measurement_type} data")
 
-            ax.set_xlabel('Timepoints')
-            ax.set_ylabel('Simulation/Surrogate data')
+            ax.set_xlabel("Timepoints")
+            ax.set_ylabel("Simulation/Surrogate data")
 
     if not use_given_axes:
         for ax in axes[len(results) :]:
             ax.remove()
 
     return axes
 
@@ -341,26 +343,26 @@
             timepoints.append(unique_timepoints[max_timepoint_unique_ind + 1])
 
         # Plot the category rectangle
         ax.fill_between(
             timepoints,
             [upper_bound] * len(timepoints),
             [lower_bound] * len(timepoints),
-            color='gray',
+            color="gray",
             alpha=0.5,
         )
 
     # Add to legend meaning of gray rectangles.
     ax.fill_between(
         [],
         [],
         [],
-        color='gray',
+        color="gray",
         alpha=0.5,
-        label='Categories',
+        label="Categories",
     )
 
 
 def _plot_category_rectangles(
     ax,
     timepoints,
     upper_bounds,
@@ -379,75 +381,75 @@
                         surrogate_data
                     )
                     middle_index = int((i - interval_length + i) / 2)
                     middle_timepoint = timepoints[middle_index]
                     # Draw a vertical short grey arrow at the middle point of the interval
                     # at the upper_bounds[i] height
                     ax.annotate(
-                        '',
+                        "",
                         xy=(middle_timepoint, upper_bounds[i]),
                         xytext=(
                             middle_timepoint,
                             upper_bounds[i] + 0.1 * max(surrogate_data),
                         ),
                         arrowprops={
-                            'arrowstyle': '<-',
-                            'color': 'gray',
-                            'linewidth': 2,
+                            "arrowstyle": "<-",
+                            "color": "gray",
+                            "linewidth": 2,
                         },
                     )
                     ax.text(
                         middle_timepoint,
                         upper_bounds[i] + 0.1 * max(surrogate_data),
-                        'INF',
-                        color='gray',
+                        "INF",
+                        color="gray",
                         fontsize=12,
                     )
                     # Extend the ax to contain the text
                     ax.set_ylim(
                         bottom=ax.get_ylim()[0],
                         top=max(
                             ax.get_ylim()[1],
                             upper_bounds[i] + 0.1 * max(surrogate_data),
                         ),
                     )
                 ax.fill_between(
                     timepoints[i - interval_length : i + 1],
                     upper_bounds[i - interval_length : i + 1],
                     lower_bounds[i - interval_length : i + 1],
-                    color='gray',
+                    color="gray",
                     alpha=0.5,
                 )
             else:
                 if upper_bounds[i] == np.inf:
                     upper_bounds[i - interval_length : i + 1] = 1.1 * max(
                         surrogate_data
                     )
                     middle_index = int((i - interval_length + i + 1) / 2)
                     middle_timepoint = timepoints[middle_index]
                     # Draw a vertical short grey arrow at the middle point of the interval
                     # at the upper_bounds[i] height
                     ax.annotate(
-                        '',
+                        "",
                         xy=(middle_timepoint, upper_bounds[i]),
                         xytext=(
                             middle_timepoint,
                             upper_bounds[i] + 0.1 * max(surrogate_data),
                         ),
                         arrowprops={
-                            'arrowstyle': '<-',
-                            'color': 'gray',
-                            'linewidth': 2,
+                            "arrowstyle": "<-",
+                            "color": "gray",
+                            "linewidth": 2,
                         },
                     )
                     ax.text(
                         middle_timepoint,
                         upper_bounds[i] + 0.1 * max(surrogate_data),
-                        'INF',
-                        color='gray',
+                        "INF",
+                        color="gray",
                         fontsize=12,
                     )
                     # Extend the ax to contain the text
                     ax.set_ylim(
                         bottom=ax.get_ylim()[0],
                         top=max(
                             ax.get_ylim()[1],
@@ -465,44 +467,44 @@
                     ),
                     np.concatenate(
                         (
                             lower_bounds[i - interval_length : i + 1],
                             [lower_bounds[i]],
                         )
                     ),
-                    color='gray',
+                    color="gray",
                     alpha=0.5,
                 )
             interval_length = 0
         else:
             interval_length += 1
     if measurement_type == ORDINAL:
         # Add to legend meaning of rectangles
         ax.fill_between(
             [],
             [],
             [],
-            color='gray',
+            color="gray",
             alpha=0.5,
-            label='Categories',
+            label="Categories",
         )
     elif measurement_type == CENSORED:
         # Add to legend meaning of rectangles
         ax.fill_between(
             [],
             [],
             [],
-            color='gray',
+            color="gray",
             alpha=0.5,
-            label='Censoring areas',
+            label="Censoring areas",
         )
 
 
 def _get_data_for_plotting(
-    inner_parameters: list['OrdinalParameter'],
+    inner_parameters: list["OrdinalParameter"],
     optimal_scaling_bounds: list,
     sim: list[np.ndarray],
     timepoints: list[np.ndarray],
     interval_range: float,
     interval_gap: float,
     options: dict,
     measurement_type: str,
@@ -708,24 +710,24 @@
             [sim_i[:, observable_index] for sim_i in simulation]
         )[petab_condition_ordering]
 
         if not use_given_axes:
             ax.plot(
                 condition_ids_from_petab,
                 whole_simulation,
-                linestyle='-',
-                marker='.',
-                color='b',
-                label='Simulation',
+                linestyle="-",
+                marker=".",
+                color="b",
+                label="Simulation",
             )
         ax.plot(
             petab_censored_conditions,
             surrogate_all,
-            'rx',
-            label='Surrogate data',
+            "rx",
+            label="Surrogate data",
         )
         _plot_category_rectangles(
             ax,
             petab_censored_conditions,
             upper_bounds_all,
             lower_bounds_all,
             surrogate_all,
@@ -735,59 +737,59 @@
         quantitative_data = inner_problem.groups[group][QUANTITATIVE_DATA]
         quantitative_data = quantitative_data[
             petab_quantitative_condition_ordering
         ]
         ax.plot(
             petab_quantitative_conditions,
             quantitative_data,
-            'gs',
-            label='Quantitative data',
+            "gs",
+            label="Quantitative data",
         )
 
     elif measurement_type == ORDINAL:
         # Change ordering of simulation, surrogate data and bounds to petab condition ordering
         simulation_all = simulation_all[petab_condition_ordering]
         surrogate_all = surrogate_all[petab_condition_ordering]
         upper_bounds_all = upper_bounds_all[petab_condition_ordering]
         lower_bounds_all = lower_bounds_all[petab_condition_ordering]
 
         # Plot the categories and surrogate data across conditions
         if not use_given_axes:
             ax.plot(
                 condition_ids_from_petab,
                 simulation_all,
-                linestyle='-',
-                marker='.',
-                color='b',
-                label='Simulation',
+                linestyle="-",
+                marker=".",
+                color="b",
+                label="Simulation",
             )
         ax.plot(
             condition_ids_from_petab,
             surrogate_all,
-            'rx',
-            label='Surrogate data',
+            "rx",
+            label="Surrogate data",
         )
 
         _plot_category_rectangles(
             ax,
             condition_ids_from_petab,
             upper_bounds_all,
             lower_bounds_all,
             surrogate_all,
             measurement_type,
         )
 
     # Set the condition xticks on an angle
-    ax.tick_params(axis='x', rotation=25)
+    ax.tick_params(axis="x", rotation=25)
     ax.legend()
     if not use_given_axes:
-        ax.set_title(f'Group {group}, {measurement_type} data')
+        ax.set_title(f"Group {group}, {measurement_type} data")
 
-    ax.set_xlabel('Conditions')
-    ax.set_ylabel('Simulation/Surrogate data')
+    ax.set_xlabel("Conditions")
+    ax.set_ylabel("Simulation/Surrogate data")
 
 
 def _plot_observable_fit_for_one_condition(
     ax,
     observable_index,
     group,
     inner_problem,
@@ -803,47 +805,47 @@
 ):
     """Plot the observable fit in case it has one condition."""
     if measurement_type == ORDINAL:
         if not use_given_axes:
             ax.plot(
                 timepoints_all[0],
                 simulation_all[0],
-                linestyle='-',
-                marker='.',
-                color='b',
-                label='Simulation',
+                linestyle="-",
+                marker=".",
+                color="b",
+                label="Simulation",
             )
     elif measurement_type == CENSORED:
         quantitative_data = inner_problem.groups[group][QUANTITATIVE_DATA]
         quantitative_ixs = inner_problem.groups[group][QUANTITATIVE_IXS]
         quantitative_timepoints = timepoints[0][
             quantitative_ixs[0].T[observable_index]
         ]
 
         if not use_given_axes:
             ax.plot(
                 timepoints[0],
                 simulation[0][:, observable_index],
-                linestyle='-',
-                marker='.',
-                color='b',
-                label='Simulation',
+                linestyle="-",
+                marker=".",
+                color="b",
+                label="Simulation",
             )
         ax.plot(
             quantitative_timepoints,
             quantitative_data,
-            'gs',
-            label='Quantitative data',
+            "gs",
+            label="Quantitative data",
         )
 
     ax.plot(
         timepoints_all[0],
         surrogate_all[0],
-        'rx',
-        label='Surrogate data',
+        "rx",
+        label="Surrogate data",
     )
 
     # Plot the categorie rectangles
     _plot_category_rectangles(
         ax,
         timepoints_all[0],
         upper_bounds_all[0],
@@ -870,15 +872,15 @@
     use_given_axes,
 ):
     """Plot the observable fit in case it has multiple conditions."""
     # Get the colors from the plotted simulations
     if use_given_axes:
         colors = []
         for line in ax.lines:
-            if 'simulation' in line.get_label():
+            if "simulation" in line.get_label():
                 colors.append(line.get_color())
     # Get as many colors as there are conditions
     else:
         colors = plt.cm.rainbow(np.linspace(0, 1, len(simulation_all)))
 
     if measurement_type == CENSORED:
         quantitative_data_flattened = inner_problem.groups[group][
@@ -906,40 +908,40 @@
     ):
         # Plot the categories and surrogate data for the current condition
         if measurement_type == ORDINAL:
             if not use_given_axes:
                 ax.plot(
                     timepoints_all[condition_index],
                     simulation_all[condition_index],
-                    linestyle='-',
-                    marker='.',
+                    linestyle="-",
+                    marker=".",
                     color=color,
                     label=condition_id,
                 )
         elif measurement_type == CENSORED:
             if not use_given_axes:
                 ax.plot(
                     timepoints[condition_index],
                     simulation[condition_index][:, observable_index],
-                    linestyle='-',
-                    marker='.',
+                    linestyle="-",
+                    marker=".",
                     color=color,
                     label=condition_id,
                 )
             ax.plot(
                 quantitative_timepoints[condition_index],
                 quantitative_data[condition_index],
-                marker='s',
+                marker="s",
                 color=color,
             )
 
         ax.plot(
             timepoints_all[condition_index],
             surrogate_all[condition_index],
-            'x',
+            "x",
             color=color,
         )
 
     # Get all unique timepoints in ascending order
     unique_timepoints = np.unique(np.concatenate(timepoints_all))
 
     # Gather timepoints for each category in a dictionary
@@ -971,28 +973,28 @@
         unique_timepoints,
     )
 
     # Add to legend meaning of x, and -o- markers.
     ax.plot(
         [],
         [],
-        'x',
-        color='black',
-        label='Surrogate data',
+        "x",
+        color="black",
+        label="Surrogate data",
     )
     if not use_given_axes:
         ax.plot(
             [],
             [],
-            linestyle='-',
-            marker='.',
-            color='black',
-            label='Simulation',
+            linestyle="-",
+            marker=".",
+            color="black",
+            label="Simulation",
         )
     if measurement_type == CENSORED:
         ax.plot(
             [],
             [],
-            marker='s',
-            color='black',
-            label='Quantitative data',
+            marker="s",
+            color="black",
+            label="Quantitative data",
         )
```

### Comparing `pypesto-0.4.2/pypesto/visualize/parameters.py` & `pypesto-0.5.0/pypesto/visualize/parameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
-from typing import Callable, Iterable, List, Optional, Sequence, Tuple, Union
+from collections.abc import Iterable, Sequence
+from typing import Callable, Optional, Union
 
 import matplotlib.axes
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from matplotlib.colors import Colormap
 from matplotlib.ticker import MaxNLocator
@@ -22,24 +23,24 @@
 
 logger = logging.getLogger(__name__)
 
 
 def parameters(
     results: Union[Result, Sequence[Result]],
     ax: Optional[matplotlib.axes.Axes] = None,
-    parameter_indices: Union[str, Sequence[int]] = 'free_only',
-    lb: Optional[Union[np.ndarray, List[float]]] = None,
-    ub: Optional[Union[np.ndarray, List[float]]] = None,
-    size: Optional[Tuple[float, float]] = None,
-    reference: Optional[List[ReferencePoint]] = None,
-    colors: Optional[Union[RGBA, List[RGBA]]] = None,
-    legends: Optional[Union[str, List[str]]] = None,
+    parameter_indices: Union[str, Sequence[int]] = "free_only",
+    lb: Optional[Union[np.ndarray, list[float]]] = None,
+    ub: Optional[Union[np.ndarray, list[float]]] = None,
+    size: Optional[tuple[float, float]] = None,
+    reference: Optional[list[ReferencePoint]] = None,
+    colors: Optional[Union[RGBA, list[RGBA]]] = None,
+    legends: Optional[Union[str, list[str]]] = None,
     balance_alpha: bool = True,
     start_indices: Optional[Union[int, Iterable[int]]] = None,
-    scale_to_interval: Optional[Tuple[float, float]] = None,
+    scale_to_interval: Optional[tuple[float, float]] = None,
     plot_inner_parameters: bool = True,
 ) -> matplotlib.axes.Axes:
     """
     Plot parameter values.
 
     Parameters
     ----------
@@ -82,17 +83,17 @@
     ax:
         The plot axes.
     """
     # parse input
     (results, colors, legends) = process_result_list(results, colors, legends)
 
     if isinstance(parameter_indices, str):
-        if parameter_indices == 'all':
+        if parameter_indices == "all":
             parameter_indices = range(0, results[0].problem.dim_full)
-        elif parameter_indices == 'free_only':
+        elif parameter_indices == "free_only":
             parameter_indices = results[0].problem.x_free_indices
         else:
             raise ValueError(
                 "Permissible values for parameter_indices are "
                 "'all', 'free_only' or a list of indices"
             )
 
@@ -147,44 +148,44 @@
 
     # plot reference points
     for i_ref in ref:
         # reduce parameter vector in reference point, if necessary
         if len(parameter_indices) < results[0].problem.dim_full:
             x_ref = np.array(
                 results[0].problem.get_reduced_vector(
-                    i_ref['x'], parameter_indices
+                    i_ref["x"], parameter_indices
                 )
             )
         else:
-            x_ref = np.array(i_ref['x'])
+            x_ref = np.array(i_ref["x"])
         x_ref = np.reshape(x_ref, (1, x_ref.size))
         x_ref = scale_parameters(x_ref)
 
         # plot reference parameters using lowlevel routine
         ax = parameters_lowlevel(
             x_ref,
-            [i_ref['fval']],
+            [i_ref["fval"]],
             ax=ax,
-            colors=i_ref['color'],
-            linestyle='--',
+            colors=i_ref["color"],
+            linestyle="--",
             legend_text=i_ref.legend,
             balance_alpha=balance_alpha,
         )
 
     return ax
 
 
 def parameter_hist(
     result: Result,
     parameter_name: str,
-    bins: Union[int, str] = 'auto',
-    ax: Optional['matplotlib.Axes'] = None,
-    size: Optional[Tuple[float]] = (18.5, 10.5),
-    color: Optional[List[float]] = None,
-    start_indices: Optional[Union[int, List[int]]] = None,
+    bins: Union[int, str] = "auto",
+    ax: Optional["matplotlib.Axes"] = None,
+    size: Optional[tuple[float]] = (18.5, 10.5),
+    color: Optional[list[float]] = None,
+    start_indices: Optional[Union[int, list[int]]] = None,
 ):
     """
     Plot parameter values as a histogram.
 
     Parameters
     ----------
     result:
@@ -232,21 +233,21 @@
 
     return ax
 
 
 def parameters_lowlevel(
     xs: np.ndarray,
     fvals: np.ndarray,
-    lb: Optional[Union[np.ndarray, List[float]]] = None,
-    ub: Optional[Union[np.ndarray, List[float]]] = None,
+    lb: Optional[Union[np.ndarray, list[float]]] = None,
+    ub: Optional[Union[np.ndarray, list[float]]] = None,
     x_labels: Optional[Iterable[str]] = None,
     ax: Optional[matplotlib.axes.Axes] = None,
-    size: Optional[Tuple[float, float]] = None,
-    colors: Optional[Sequence[Union[np.ndarray, List[float]]]] = None,
-    linestyle: str = '-',
+    size: Optional[tuple[float, float]] = None,
+    colors: Optional[Sequence[Union[np.ndarray, list[float]]]] = None,
+    linestyle: str = "-",
     legend_text: Optional[str] = None,
     balance_alpha: bool = True,
 ) -> matplotlib.axes.Axes:
     """
     Plot parameters plot using list of parameters.
 
     Parameters
@@ -305,48 +306,48 @@
         else:
             tmp_legend = None
         ax.plot(
             x,
             parameters_ind,
             linestyle,
             color=colors[j_x],
-            marker='o',
+            marker="o",
             label=tmp_legend,
         )
 
     ax.set_yticks(parameters_ind)
     if x_labels is not None:
         ax.set_yticklabels(x_labels)
 
     # draw bounds
     parameters_ind = np.array(parameters_ind).flatten()
     if lb is not None:
         lb = np.array(lb, dtype="float64")
-        ax.plot(lb.flatten(), parameters_ind, 'k--', marker='+')
+        ax.plot(lb.flatten(), parameters_ind, "k--", marker="+")
     if ub is not None:
         ub = np.array(ub, dtype="float64")
-        ax.plot(ub.flatten(), parameters_ind, 'k--', marker='+')
+        ax.plot(ub.flatten(), parameters_ind, "k--", marker="+")
 
-    ax.set_xlabel('Parameter value')
-    ax.set_ylabel('Parameter')
-    ax.set_title('Estimated parameters')
+    ax.set_xlabel("Parameter value")
+    ax.set_ylabel("Parameter")
+    ax.set_title("Estimated parameters")
     if legend_text is not None:
         ax.legend()
 
     return ax
 
 
 def handle_inputs(
     result: Result,
-    parameter_indices: List[int],
-    lb: Optional[Union[np.ndarray, List[float]]] = None,
-    ub: Optional[Union[np.ndarray, List[float]]] = None,
+    parameter_indices: list[int],
+    lb: Optional[Union[np.ndarray, list[float]]] = None,
+    ub: Optional[Union[np.ndarray, list[float]]] = None,
     start_indices: Optional[Union[int, Iterable[int]]] = None,
     plot_inner_parameters: bool = False,
-) -> Tuple[np.ndarray, np.ndarray, List[str], np.ndarray, List[np.ndarray]]:
+) -> tuple[np.ndarray, np.ndarray, list[str], np.ndarray, list[np.ndarray]]:
     """
     Compute the correct bounds for the parameter indices to be plotted.
 
     Outputs the corresponding parameters and their labels.
 
     Parameters
     ----------
@@ -430,16 +431,16 @@
 
     return lb, ub, x_labels, fvals_out, xs_out
 
 
 def _handle_inner_inputs(
     result: Result,
 ) -> Union[
-    Tuple[None, None, None, None],
-    Tuple[list[np.ndarray], list[str], np.ndarray, np.ndarray],
+    tuple[None, None, None, None],
+    tuple[list[np.ndarray], list[str], np.ndarray, np.ndarray],
 ]:
     """Handle inner parameters from hierarchical optimization, if available.
 
     Parameters
     ----------
     result:
         Optimization result obtained by 'optimize.py'.
@@ -485,19 +486,19 @@
         inner_xs = None
 
     return inner_xs, inner_xs_names, inner_lb, inner_ub
 
 
 def parameters_correlation_matrix(
     result: Result,
-    parameter_indices: Union[str, Sequence[int]] = 'free_only',
+    parameter_indices: Union[str, Sequence[int]] = "free_only",
     start_indices: Optional[Union[int, Iterable[int]]] = None,
-    method: Union[str, Callable] = 'pearson',
+    method: Union[str, Callable] = "pearson",
     cluster: bool = True,
-    cmap: Union[Colormap, str] = 'bwr',
+    cmap: Union[Colormap, str] = "bwr",
     return_table: bool = False,
 ) -> matplotlib.axes.Axes:
     """
     Plot correlation of optimized parameters.
 
     Parameters
     ----------
@@ -530,15 +531,15 @@
         start_indices=start_indices, result=result
     )
     parameter_indices = process_parameter_indices(
         parameter_indices=parameter_indices, result=result
     )
     # put all parameters into a dataframe, where columns are parameters
     parameters = [
-        result.optimize_result[i_start]['x'][parameter_indices]
+        result.optimize_result[i_start]["x"][parameter_indices]
         for i_start in start_indices
     ]
     x_labels = [
         result.problem.x_names[parameter_index]
         for parameter_index in parameter_indices
     ]
     df = pd.DataFrame(parameters, columns=x_labels)
@@ -554,19 +555,19 @@
     if return_table:
         return ax, df
     return ax
 
 
 def optimization_scatter(
     result: Result,
-    parameter_indices: Union[str, Sequence[int]] = 'free_only',
+    parameter_indices: Union[str, Sequence[int]] = "free_only",
     start_indices: Optional[Union[int, Iterable[int]]] = None,
     diag_kind: str = "kde",
     suptitle: str = None,
-    size: Tuple[float, float] = None,
+    size: tuple[float, float] = None,
     show_bounds: bool = False,
 ):
     """
     Plot a scatter plot of all pairs of parameters for the given starts.
 
     Parameters
     ----------
@@ -600,26 +601,26 @@
     parameter_indices = process_parameter_indices(
         parameter_indices=parameter_indices, result=result
     )
     # remove all start indices that encounter an inf value at the start
     # resulting in optimize_result[start]["x"] being None
     start_indices_finite = start_indices[
         [
-            result.optimize_result[i_start]['x'] is not None
+            result.optimize_result[i_start]["x"] is not None
             for i_start in start_indices
         ]
     ]
     # compare start_indices with start_indices_finite and log a warning
     if len(start_indices) != len(start_indices_finite):
         logger.warning(
-            'Some start indices were removed due to inf values at the start.'
+            "Some start indices were removed due to inf values at the start."
         )
     # put all parameters into a dataframe, where columns are parameters
     parameters = [
-        result.optimize_result[i_start]['x'][parameter_indices]
+        result.optimize_result[i_start]["x"][parameter_indices]
         for i_start in start_indices_finite
     ]
     x_labels = [
         result.problem.x_names[parameter_index]
         for parameter_index in parameter_indices
     ]
     df = pd.DataFrame(parameters, columns=x_labels)
```

### Comparing `pypesto-0.4.2/pypesto/visualize/profile_cis.py` & `pypesto-0.5.0/pypesto/visualize/profile_cis.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from typing import Sequence, Union
+from collections.abc import Sequence
+from typing import Union
 
 import matplotlib.axes
 import matplotlib.pyplot as plt
 import numpy as np
 
 from ..profile import calculate_approximate_ci, chi2_quantile_to_ratio
 from ..result import Result
 
 
 def profile_cis(
     result: Result,
     confidence_level: float = 0.95,
     profile_indices: Sequence[int] = None,
     profile_list: int = 0,
-    color: Union[str, tuple] = 'C0',
+    color: Union[str, tuple] = "C0",
     show_bounds: bool = False,
     ax: matplotlib.axes.Axes = None,
 ) -> matplotlib.axes.Axes:
     """
     Plot approximate confidence intervals based on profiles.
 
     Parameters
@@ -65,22 +66,22 @@
             xs=xs, ratios=ratios, confidence_ratio=confidence_ratio
         )
         intervals.append((lb, ub))
 
     x_names = [problem.x_names[ix] for ix in profile_indices]
 
     for ix, (lb, ub) in enumerate(intervals):
-        ax.plot([lb, ub], [ix + 1, ix + 1], marker='|', color=color)
+        ax.plot([lb, ub], [ix + 1, ix + 1], marker="|", color=color)
 
     parameters_ind = np.arange(1, len(intervals) + 1)
     ax.set_yticks(parameters_ind)
     ax.set_yticklabels(x_names)
     ax.set_ylabel("Parameter")
     ax.set_xlabel("Parameter value")
 
     if show_bounds:
         lb = problem.lb_full[profile_indices]
-        ax.plot(lb, parameters_ind, 'k--', marker='+')
+        ax.plot(lb, parameters_ind, "k--", marker="+")
         ub = problem.ub_full[profile_indices]
-        ax.plot(ub, parameters_ind, 'k--', marker='+')
+        ax.plot(ub, parameters_ind, "k--", marker="+")
 
     return ax
```

### Comparing `pypesto-0.4.2/pypesto/visualize/profiles.py` & `pypesto-0.5.0/pypesto/visualize/profiles.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Optional, Sequence, Union
+from collections.abc import Sequence
+from typing import Optional, Union
 from warnings import warn
 
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.ticker import MaxNLocator
 
 from ..result import Result
@@ -176,15 +177,15 @@
     if isinstance(fvals, Sequence):
         n_fvals = len(fvals)
     else:
         n_fvals = 1
         fvals = [fvals]
 
     # number of non-trivial profiles
-    n_profiles = sum((fval is not None for fval in fvals))
+    n_profiles = sum(fval is not None for fval in fvals)
 
     # if axes already exists, we have to match profiles to axes
     if not create_new_ax:
         if n_fvals != len(ax) and n_profiles != len(ax):
             raise ValueError(
                 "Number of axes does not match number of profiles. Stopping."
             )
@@ -239,26 +240,26 @@
                 show_bounds=show_bounds,
                 lb=lb,
                 ub=ub,
             )
 
         # labels
         if x_labels is None:
-            ax[counter].set_xlabel(f'Parameter {i_plot}')
+            ax[counter].set_xlabel(f"Parameter {i_plot}")
         else:
             ax[counter].set_xlabel(x_labels[counter])
 
         if counter % columns == 0:
-            ax[counter].set_ylabel('Log-posterior ratio')
+            ax[counter].set_ylabel("Log-posterior ratio")
         else:
             # fix pyPESTO/pyPESTO/pypesto/visualize/profiles.py:228:
             # UserWarning: FixedFormatter should only be used
             # together with FixedLocator. Fix from matplotlib #18848.
             ax[counter].set_yticks(ax[counter].get_yticks())
-            ax[counter].set_yticklabels(['' for _ in ax[counter].get_yticks()])
+            ax[counter].set_yticklabels(["" for _ in ax[counter].get_yticks()])
 
         # increase counter and cleanup legend
         counter += 1
 
     return ax
 
 
@@ -304,16 +305,16 @@
 
     # get colors
     color = assign_colors([1.0], color)
 
     # axes
     if ax is None:
         ax = plt.subplots()[1]
-        ax.set_xlabel('Parameter value')
-        ax.set_ylabel('Log-posterior ratio')
+        ax.set_xlabel("Parameter value")
+        ax.set_ylabel("Log-posterior ratio")
         fig = plt.gcf()
         fig.set_size_inches(*size)
 
     # plot
     if fvals.size != 0:
         ax.xaxis.set_major_locator(MaxNLocator(integer=True))
         ax.plot(fvals[0, :], fvals[1, :], color=color[0], label=legend_text)
@@ -341,15 +342,15 @@
     profile_indices: list of integer values
         List of integer values specifying which profiles should be plotted.
     """
     if len(ref) > 0:
         # loop over axes objects
         for i_par, i_ax in enumerate(ax):
             for i_ref in ref:
-                current_x = i_ref['x'][profile_indices[i_par]]
+                current_x = i_ref["x"][profile_indices[i_par]]
                 i_ax.plot(
                     [current_x, current_x],
                     [0.0, 1.0],
                     color=i_ref.color,
                     label=i_ref.legend,
                 )
 
@@ -496,12 +497,13 @@
         profile_indices_ret = list(plottable_indices)
     else:
         profile_indices_ret = list(profile_indices)
         for ind in profile_indices:
             if ind not in plottable_indices:
                 profile_indices_ret.remove(ind)
                 warn(
-                    'Requested to plot profile for parameter index %i, '
-                    'but profile has not been computed.' % ind
+                    f"Requested to plot profile for parameter index {ind}, "
+                    "but profile has not been computed.",
+                    stacklevel=2,
                 )
 
     return profile_indices_ret
```

### Comparing `pypesto-0.4.2/pypesto/visualize/reference_points.py` & `pypesto-0.5.0/pypesto/visualize/reference_points.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Optional, Sequence, Union
+from collections.abc import Sequence
+from typing import Optional, Union
 
 import numpy as np
 
 
 class ReferencePoint(dict):
     """
     Reference point for plotting.
@@ -75,39 +76,39 @@
                 self.color = None
                 self.auto_color = True
         if reference is None:
             if x is not None:
                 self.x = np.array(x)
             else:
                 raise ValueError(
-                    'Parameter vector x not passed, but is a '
-                    'mandatory input when creating a reference '
-                    'point. Stopping.'
+                    "Parameter vector x not passed, but is a "
+                    "mandatory input when creating a reference "
+                    "point. Stopping."
                 )
             if fval is not None:
                 self.fval = fval
             else:
                 raise ValueError(
-                    'Objective value fval not passed, but is a '
-                    'mandatory input when creating a reference '
-                    'point. Stopping.'
+                    "Objective value fval not passed, but is a "
+                    "mandatory input when creating a reference "
+                    "point. Stopping."
                 )
             if color is not None:
                 self.color = color
                 self.auto_color = False
             else:
                 self.color = None
                 self.auto_color = True
 
     def __getattr__(self, key):
         """Allow usage of keys as attributes."""
         try:
             return self[key]
         except KeyError:
-            raise AttributeError(key)
+            raise AttributeError(key) from None
 
     __setattr__ = dict.__setitem__
     __delattr__ = dict.__delitem__
 
 
 def assign_colors(ref: Sequence[ReferencePoint]) -> Sequence[ReferencePoint]:
     """
@@ -121,27 +122,27 @@
     Returns
     -------
     Reference points, which got their color property filled
     """
     # loop over reference points
     auto_color_count = 0
     for i_ref in ref:
-        if i_ref['auto_color']:
+        if i_ref["auto_color"]:
             auto_color_count += 1
 
     auto_colors = [
         [0.0, 0.5 * (1.0 + i_auto / auto_color_count), 0.0, 0.9]
         for i_auto in range(auto_color_count)
     ]
 
     # loop over reference points and assign auto_colors
     auto_color_count = 0
     for i_num, i_ref in enumerate(ref):
-        if i_ref['auto_color']:
-            i_ref['color'] = auto_colors[i_num]
+        if i_ref["auto_color"]:
+            i_ref["color"] = auto_colors[i_num]
             auto_color_count += 1
 
     return ref
 
 
 def create_references(
     references=None, x=None, fval=None, color=None, legend=None
```

### Comparing `pypesto-0.4.2/pypesto/visualize/sampling.py` & `pypesto-0.5.0/pypesto/visualize/sampling.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import warnings
+from collections.abc import Sequence
 from colorsys import rgb_to_hls
-from typing import Dict, Optional, Sequence, Tuple, Union
+from typing import Optional, Union
 
 import matplotlib.axes
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from matplotlib.collections import LineCollection
 from matplotlib.container import ErrorbarContainer
@@ -28,27 +29,27 @@
 from .misc import rgba2rgb
 
 cmap = matplotlib.cm.viridis
 logger = logging.getLogger(__name__)
 
 
 prediction_errorbar_settings = {
-    'fmt': 'none',
-    'color': 'k',
-    'capsize': 10,
+    "fmt": "none",
+    "color": "k",
+    "capsize": 10,
 }
 
 
 def sampling_fval_traces(
     result: Result,
     i_chain: int = 0,
     full_trace: bool = False,
     stepsize: int = 1,
     title: str = None,
-    size: Tuple[float, float] = None,
+    size: tuple[float, float] = None,
     ax: matplotlib.axes.Axes = None,
 ):
     """
     Plot log-posterior (=function value) over iterations.
 
     Parameters
     ----------
@@ -83,47 +84,47 @@
     )
 
     # set axes and figure
     if ax is None:
         _, ax = plt.subplots(figsize=size)
 
     sns.set(style="ticks")
-    kwargs = {'edgecolor': "w", 'linewidth': 0.3, 's': 10}  # for edge color
+    kwargs = {"edgecolor": "w", "linewidth": 0.3, "s": 10}  # for edge color
     if full_trace:
-        kwargs['hue'] = "converged"
-        if len(params_fval[kwargs['hue']].unique()) == 1:
-            kwargs['palette'] = ["#477ccd"]
-        elif len(params_fval[kwargs['hue']].unique()) == 2:
-            kwargs['palette'] = ["#868686", "#477ccd"]
-        kwargs['legend'] = False
+        kwargs["hue"] = "converged"
+        if len(params_fval[kwargs["hue"]].unique()) == 1:
+            kwargs["palette"] = ["#477ccd"]
+        elif len(params_fval[kwargs["hue"]].unique()) == 2:
+            kwargs["palette"] = ["#868686", "#477ccd"]
+        kwargs["legend"] = False
 
     sns.scatterplot(
         x="iteration", y="logPosterior", data=params_fval, ax=ax, **kwargs
     )
 
     if result.sample_result.burn_in is None:
         _burn_in = 0
     else:
         _burn_in = result.sample_result.burn_in
 
     if full_trace and _burn_in > 0:
-        ax.axvline(_burn_in, linestyle='--', linewidth=1.5, color='k')
+        ax.axvline(_burn_in, linestyle="--", linewidth=1.5, color="k")
 
-    ax.set_xlabel('iteration index')
-    ax.set_ylabel('log-posterior')
+    ax.set_xlabel("iteration index")
+    ax.set_ylabel("log-posterior")
 
     if title:
         ax.set_title(title)
 
     sns.despine()
 
     return ax
 
 
-def _get_level_percentiles(level: float) -> Tuple[float, float]:
+def _get_level_percentiles(level: float) -> tuple[float, float]:
     """Convert a credibility level to percentiles.
 
     Similar to the highest-density region of a symmetric, unimodal distribution
     (e.g. Gaussian distribution).
 
     For example, an credibility level of `95` will be converted to
     `(2.5, 97.5)`.
@@ -143,19 +144,19 @@
     The percentiles, with the lower percentile first.
     """
     lower_percentile = (100 - level) / 2
     return lower_percentile, 100 - lower_percentile
 
 
 def _get_statistic_data(
-    summary: Dict[str, PredictionResult],
+    summary: dict[str, PredictionResult],
     statistic: str,
     condition_id: str,
     output_id: str,
-) -> Tuple[Sequence[float], Sequence[float]]:
+) -> tuple[Sequence[float], Sequence[float]]:
     """Get statistic-, condition-, and output-specific data.
 
     Parameters
     ----------
     summary:
         A `pypesto.ensemble.EnsemblePrediction.prediction_summary`, used as the
         source of annotated data to subset.
@@ -178,26 +179,26 @@
     t = condition_result.timepoints
     output_index = condition_result.output_ids.index(output_id)
     y = condition_result.output[:, output_index]
     return (t, y)
 
 
 def _plot_trajectories_by_condition(
-    summary: Dict[str, PredictionResult],
+    summary: dict[str, PredictionResult],
     condition_ids: Sequence[str],
     output_ids: Sequence[str],
     axes: matplotlib.axes.Axes,
     levels: Sequence[float],
-    level_opacities: Dict[int, float],
-    labels: Dict[str, str],
+    level_opacities: dict[int, float],
+    labels: dict[str, str],
     variable_colors: Sequence[RGB],
     average: str = MEDIAN,
     add_sd: bool = False,
-    grouped_measurements: Dict[
-        Tuple[str, str], Sequence[Sequence[float]]
+    grouped_measurements: dict[
+        tuple[str, str], Sequence[Sequence[float]]
     ] = None,
 ) -> None:
     """Plot predicted trajectories, with subplots grouped by condition.
 
     Parameters
     ----------
     summary:
@@ -233,57 +234,57 @@
         Measurement data that has already been grouped by condition and output,
         where the keys are `(condition_id, output_id)` 2-tuples, and the values
         are `[sequence of x-axis values, sequence of y-axis values]`.
     """
     # Each subplot has all data for a single condition.
     for condition_index, condition_id in enumerate(condition_ids):
         ax = axes.flat[condition_index]
-        ax.set_title(f'Condition: {labels[condition_id]}')
+        ax.set_title(f"Condition: {labels[condition_id]}")
         # Each subplot has all data for all condition-specific outputs.
         for output_index, output_id in enumerate(output_ids):
             facecolor0 = variable_colors[output_index]
             # Plot the average for each output.
             t_average, y_average = _get_statistic_data(
                 summary,
                 average,
                 condition_id,
                 output_id,
             )
             ax.plot(
                 t_average,
                 y_average,
-                'k-',
+                "k-",
             )
             if add_sd:
                 t_std, y_std = _get_statistic_data(
                     summary,
                     STANDARD_DEVIATION,
                     condition_id,
                     output_id,
                 )
                 if (t_std != t_average).all():
                     raise ValueError(
-                        'Unknown error: timepoints for average and standard '
-                        'deviation do not match.'
+                        "Unknown error: timepoints for average and standard "
+                        "deviation do not match."
                     )
                 ax.errorbar(
                     t_average,
                     y_average,
                     yerr=y_std,
                     **prediction_errorbar_settings,
                 )
             # Plot the regions described by the credibility level,
             # for each output.
             for level_index, level in enumerate(levels):
                 # Get the percentiles that correspond to the credibility level,
                 # as their labels in the `summary`.
-                lower_label, upper_label = [
+                lower_label, upper_label = (
                     get_percentile_label(percentile)
                     for percentile in _get_level_percentiles(level)
-                ]
+                )
                 # Get the data for each percentile.
                 t_lower, lower_data = _get_statistic_data(
                     summary,
                     lower_label,
                     condition_id,
                     output_id,
                 )
@@ -293,16 +294,16 @@
                     condition_id,
                     output_id,
                 )
                 # Timepoints must match, or `upper_data` will be plotted at
                 # some incorrect time points.
                 if not (np.array(t_lower) == np.array(t_upper)).all():
                     raise ValueError(
-                        'The timepoints of the data for the upper and lower '
-                        'percentiles do not match.'
+                        "The timepoints of the data for the upper and lower "
+                        "percentiles do not match."
                     )
                 # Plot a shaded region between the data that correspond to the
                 # lower and upper percentiles.
                 ax.fill_between(
                     t_lower,
                     lower_data,
                     upper_data,
@@ -314,37 +315,37 @@
                 )
             if measurements := grouped_measurements.get(
                 (condition_id, output_id), False
             ):
                 ax.scatter(
                     measurements[0],
                     measurements[1],
-                    marker='o',
+                    marker="o",
                     facecolor=facecolor0,
                     edgecolor=(
-                        'white'
+                        "white"
                         if rgb_to_hls(*facecolor0)[1] < 0.5
-                        else 'black'
+                        else "black"
                     ),
                 )
 
 
 def _plot_trajectories_by_output(
-    summary: Dict[str, PredictionResult],
+    summary: dict[str, PredictionResult],
     condition_ids: Sequence[str],
     output_ids: Sequence[str],
     axes: matplotlib.axes.Axes,
     levels: Sequence[float],
-    level_opacities: Dict[int, float],
-    labels: Dict[str, str],
+    level_opacities: dict[int, float],
+    labels: dict[str, str],
     variable_colors: Sequence[RGB],
     average: str = MEDIAN,
     add_sd: bool = False,
-    grouped_measurements: Dict[
-        Tuple[str, str], Sequence[Sequence[float]]
+    grouped_measurements: dict[
+        tuple[str, str], Sequence[Sequence[float]]
     ] = None,
 ) -> None:
     """Plot predicted trajectories, with subplots grouped by output.
 
     Each subplot is further divided by conditions, such that all conditions
     are displayed side-by-side for a single output. Hence, in each subplot, the
     timepoints of each condition plot are shifted by the the end timepoint of
@@ -356,23 +357,23 @@
     """
     # Each subplot has all data for a single output.
     for output_index, output_id in enumerate(output_ids):
         # Store the end timepoint of the previous condition plot, such that the
         # next condition plot starts at the end of the previous condition plot.
         t0 = 0
         ax = axes.flat[output_index]
-        ax.set_title(f'Trajectory: {labels[output_id]}')
+        ax.set_title(f"Trajectory: {labels[output_id]}")
         # Each subplot is divided by conditions, with vertical lines.
         for condition_index, condition_id in enumerate(condition_ids):
             facecolor0 = variable_colors[condition_index]
             if condition_index != 0:
                 ax.axvline(
                     t0,
                     linewidth=2,
-                    color='k',
+                    color="k",
                 )
 
             t_max = t0
             t_average, y_average = _get_statistic_data(
                 summary,
                 average,
                 condition_id,
@@ -380,42 +381,42 @@
             )
             # Shift the timepoints for the average plot to start at the end of
             # the previous condition plot.
             t_average_shifted = t_average + t0
             ax.plot(
                 t_average_shifted,
                 y_average,
-                'k-',
+                "k-",
             )
             if add_sd:
                 t_std, y_std = _get_statistic_data(
                     summary,
                     STANDARD_DEVIATION,
                     condition_id,
                     output_id,
                 )
                 if (t_std != t_average).all():
                     raise ValueError(
-                        'Unknown error: timepoints for average and standard '
-                        'deviation do not match.'
+                        "Unknown error: timepoints for average and standard "
+                        "deviation do not match."
                     )
                 ax.errorbar(
                     t_average_shifted,
                     y_average,
                     yerr=y_std,
                     **prediction_errorbar_settings,
                 )
             t_max = max(t_max, *t_average_shifted)
             for level_index, level in enumerate(levels):
                 # Get the percentiles that correspond to the credibility level,
                 # as their labels in the `summary`.
-                lower_label, upper_label = [
+                lower_label, upper_label = (
                     get_percentile_label(percentile)
                     for percentile in _get_level_percentiles(level)
-                ]
+                )
                 # Get the data for each percentile.
                 t_lower, lower_data = _get_statistic_data(
                     summary,
                     lower_label,
                     condition_id,
                     output_id,
                 )
@@ -429,16 +430,16 @@
                 # the end of the previous condition plot.
                 t_lower_shifted = t_lower + t0
                 t_upper_shifted = t_upper + t0
                 # Timepoints must match, or `upper_data` will be plotted at
                 # some incorrect time points.
                 if not (np.array(t_lower) == np.array(t_upper)).all():
                     raise ValueError(
-                        'The timepoints of the data for the upper and lower '
-                        'percentiles do not match.'
+                        "The timepoints of the data for the upper and lower "
+                        "percentiles do not match."
                     )
                 # Plot a shaded region between the data that correspond to the
                 # lower and upper percentiles.
                 ax.fill_between(
                     t_lower_shifted,
                     lower_data,
                     upper_data,
@@ -450,30 +451,30 @@
                 t_max = max(t_max, *t_lower_shifted, *t_upper_shifted)
             if measurements := grouped_measurements.get(
                 (condition_id, output_id), False
             ):
                 ax.scatter(
                     [t0 + _t for _t in measurements[0]],
                     measurements[1],
-                    marker='o',
+                    marker="o",
                     facecolor=facecolor0,
                     edgecolor=(
-                        'white'
+                        "white"
                         if rgb_to_hls(*facecolor0)[1] < 0.5
-                        else 'black'
+                        else "black"
                     ),
                 )
             # Set t0 to the last plotted timepoint of the current condition
             # plot.
             t0 = t_max
 
 
 def _get_condition_and_output_ids(
-    summary: Dict[str, PredictionResult]
-) -> Tuple[Sequence[str], Sequence[str]]:
+    summary: dict[str, PredictionResult],
+) -> tuple[Sequence[str], Sequence[str]]:
     """Get all condition and output IDs in a prediction summary.
 
     Parameters
     ----------
     summary:
         The prediction summary to extract condition and output IDs from.
 
@@ -492,15 +493,15 @@
         np.array(
             [
                 set(condition_ids) == set(all_condition_ids[0])
                 for condition_ids in all_condition_ids
             ]
         ).all()
     ):
-        raise KeyError('All predictions must have the same set of conditions.')
+        raise KeyError("All predictions must have the same set of conditions.")
     condition_ids = all_condition_ids[0]
 
     output_ids = sorted(
         {
             output_id
             for prediction in summary.values()
             for condition in prediction.conditions
@@ -511,25 +512,25 @@
     return condition_ids, output_ids
 
 
 def _handle_legends(
     fig: matplotlib.figure.Figure,
     axes: matplotlib.axes.Axes,
     levels: Union[float, Sequence[float]],
-    labels: Dict[str, str],
+    labels: dict[str, str],
     level_opacities: Sequence[float],
     variable_names: Sequence[str],
     variable_colors: Sequence[RGB],
     groupby: str,
     artist_padding: float,
     n_col: int,
     average: str,
     add_sd: bool,
     grouped_measurements: Optional[
-        Dict[Tuple[str, str], Sequence[Sequence[float]]]
+        dict[tuple[str, str], Sequence[Sequence[float]]]
     ],
 ) -> None:
     """Add legends to a sampling prediction trajectories plot.
 
     Create a dummy plot from fake data such that it can be used to produce
     appropriate legends.
 
@@ -587,15 +588,15 @@
     # Assumes that different CI levels are represented as
     # different opacities of the same color.
     # Create a line object with fake data for each credibility level.
     ci_lines = []
     for index, level in enumerate(levels):
         ci_lines.append(
             [
-                f'{level}% CI',
+                f"{level}% CI",
                 Line2D(
                     *fake_data,
                     color=rgba2rgb(
                         [*RGBA_BLACK[:LEN_RGB], level_opacities[index]]
                     ),
                     lw=4,
                 ),
@@ -604,24 +605,24 @@
 
     # Create a line object with fake data for the average line.
     average_title = average.title()
     average_line_object_line2d = Line2D(*fake_data, color=RGBA_BLACK)
     if add_sd:
         capline = Line2D(
             *fake_data,
-            color=prediction_errorbar_settings['color'],
+            color=prediction_errorbar_settings["color"],
             # https://github.com/matplotlib/matplotlib/blob
             # /710fce3df95e22701bd68bf6af2c8adbc9d67a79/lib/matplotlib/
             # axes/_axes.py#L3424=
-            markersize=2.0 * prediction_errorbar_settings['capsize'],
+            markersize=2.0 * prediction_errorbar_settings["capsize"],
         )
-        average_title += ' + SD'
+        average_title += " + SD"
         barline = LineCollection(
             np.empty((2, 2, 2)),
-            color=prediction_errorbar_settings['color'],
+            color=prediction_errorbar_settings["color"],
         )
         average_line_object = ErrorbarContainer(
             (
                 average_line_object_line2d,
                 [capline],
                 [barline],
             ),
@@ -632,61 +633,61 @@
     average_line = [[average_title, average_line_object]]
 
     # Create a line object with fake data for the data points.
     data_line = []
     if grouped_measurements:
         data_line = [
             [
-                'Data',
+                "Data",
                 Line2D(
                     *fake_data,
                     linewidth=0,
-                    marker='o',
-                    markerfacecolor='grey',
-                    markeredgecolor='white',
+                    marker="o",
+                    markerfacecolor="grey",
+                    markeredgecolor="white",
                 ),
             ]
         ]
 
     level_lines = np.array(ci_lines + average_line + data_line)
 
     # CI level, and variable name, legends.
     legend_options_top_right = {
-        'bbox_to_anchor': (1 + artist_padding, 1),
-        'loc': 'upper left',
+        "bbox_to_anchor": (1 + artist_padding, 1),
+        "loc": "upper left",
     }
     legend_options_bottom_right = {
-        'bbox_to_anchor': (1 + artist_padding, 0),
-        'loc': 'lower left',
+        "bbox_to_anchor": (1 + artist_padding, 0),
+        "loc": "lower left",
     }
     legend_titles = {
-        OUTPUT: 'Conditions',
-        CONDITION: 'Trajectories',
+        OUTPUT: "Conditions",
+        CONDITION: "Trajectories",
     }
     legend_variables = axes.flat[n_col - 1].legend(
         variable_lines[:, 1],
         variable_lines[:, 0],
         **legend_options_top_right,
         title=legend_titles[groupby],
     )
     # Legend for CI levels
     axes.flat[-1].legend(
         level_lines[:, 1],
         level_lines[:, 0],
         **legend_options_bottom_right,
-        title='Prediction',
+        title="Prediction",
     )
     fig.add_artist(legend_variables)
 
 
 def _handle_colors(
     levels: Union[float, Sequence[float]],
     n_variables: int,
     reverse: bool = False,
-) -> Tuple[Sequence[float], Sequence[RGB]]:
+) -> tuple[Sequence[float], Sequence[RGB]]:
     """Calculate the colors for the prediction trajectories plot.
 
     Parameters
     ----------
     levels:
         The credibility levels.
     n_variables:
@@ -715,17 +716,17 @@
     return level_opacities, variable_colors
 
 
 def sampling_prediction_trajectories(
     ensemble_prediction: EnsemblePrediction,
     levels: Union[float, Sequence[float]],
     title: str = None,
-    size: Tuple[float, float] = None,
+    size: tuple[float, float] = None,
     axes: matplotlib.axes.Axes = None,
-    labels: Dict[str, str] = None,
+    labels: dict[str, str] = None,
     axis_label_padding: int = 50,
     groupby: str = CONDITION,
     condition_gap: float = 0.01,
     condition_ids: Sequence[str] = None,
     output_ids: Sequence[str] = None,
     weighting: bool = False,
     reverse_opacities: bool = False,
@@ -821,15 +822,15 @@
             if petab.PARAMETER_SEPARATOR in condition_id:
                 (
                     preequilibration_condition_id,
                     simulation_condition_id,
                 ) = condition_id.split(petab.PARAMETER_SEPARATOR)
             else:
                 preequilibration_condition_id, simulation_condition_id = (
-                    '',
+                    "",
                     condition_id,
                 )
             condition = {
                 petab.SIMULATION_CONDITION_ID: simulation_condition_id,
             }
             if preequilibration_condition_id:
                 condition[
@@ -854,15 +855,15 @@
         variable_names = output_ids
         n_subplots = len(condition_ids)
     elif groupby == OUTPUT:
         n_variables = len(condition_ids)
         variable_names = condition_ids
         n_subplots = len(output_ids)
     else:
-        raise ValueError(f'Unsupported groupby value: {groupby}')
+        raise ValueError(f"Unsupported groupby value: {groupby}")
 
     level_opacities, variable_colors = _handle_colors(
         levels=levels,
         n_variables=n_variables,
         reverse=reverse_opacities,
     )
 
@@ -874,16 +875,16 @@
             ax.remove()
     else:
         fig = axes.get_figure()
         if not isinstance(axes, np.ndarray):
             axes = np.array([[axes]])
         if len(axes.flat) < n_subplots:
             raise ValueError(
-                'Provided `axes` contains insufficient subplots. At least '
-                f'{n_subplots} are required.'
+                "Provided `axes` contains insufficient subplots. At least "
+                f"{n_subplots} are required."
             )
     artist_padding = axis_label_padding / (fig.get_size_inches() * fig.dpi)[0]
 
     if groupby == CONDITION:
         _plot_trajectories_by_condition(
             summary=summary,
             condition_ids=condition_ids,
@@ -931,47 +932,47 @@
         grouped_measurements=grouped_measurements,
     )
 
     # X and Y labels
     xmin = min(ax.get_position().xmin for ax in axes.flat)
     ymin = min(ax.get_position().ymin for ax in axes.flat)
     xlabel = (
-        'Cumulative time across all conditions'
+        "Cumulative time across all conditions"
         if groupby == OUTPUT
-        else 'Time'
+        else "Time"
     )
     fig.text(
         0.5,
         ymin - artist_padding,
         xlabel,
-        ha='center',
-        va='center',
+        ha="center",
+        va="center",
         transform=fig.transFigure,
     )
     fig.text(
         xmin - artist_padding,
         0.5,
-        'Simulated values',
-        ha='center',
-        va='center',
+        "Simulated values",
+        ha="center",
+        va="center",
         transform=fig.transFigure,
-        rotation='vertical',
+        rotation="vertical",
     )
 
     # plt.tight_layout()  # Ruins layout for `groupby == OUTPUT`.
     return axes
 
 
 def sampling_parameter_cis(
     result: Result,
     alpha: Sequence[int] = None,
     step: float = 0.05,
     show_median: bool = True,
     title: str = None,
-    size: Tuple[float, float] = None,
+    size: tuple[float, float] = None,
     ax: matplotlib.axes.Axes = None,
 ) -> matplotlib.axes.Axes:
     """
     Plot MCMC-based parameter credibility intervals.
 
     Parameters
     ----------
@@ -1027,38 +1028,38 @@
             y1 = [npar + _step, npar + _step]
             y2 = [npar - _step, npar - _step]
             # Plot boxes
             ax.fill(
                 np.append(x1, x1[::-1]),
                 np.append(y1, y2[::-1]),
                 color=colors[n],
-                label=str(level) + '% CI',
+                label=str(level) + "% CI",
             )
 
             if show_median:
                 if n == len(alpha_sorted) - 1:
                     burn_in = result.sample_result.burn_in
                     converged = result.sample_result.trace_x[0, burn_in:, npar]
                     _median = np.median(converged)
                     ax.plot(
                         [_median, _median],
                         [npar - _step, npar + _step],
-                        'k-',
-                        label='MCMC median',
+                        "k-",
+                        label="MCMC median",
                     )
 
             # increment height of boxes
             _step += step
 
     ax.set_yticks(range(n_pars))
     ax.set_yticklabels(
         result.problem.get_reduced_vector(result.problem.x_names)
     )
-    ax.set_xlabel('Parameter value')
-    ax.set_ylabel('Parameter name')
+    ax.set_xlabel("Parameter value")
+    ax.set_ylabel("Parameter name")
 
     if title:
         ax.set_title(title)
 
     # handle legend
     plt.gca().invert_yaxis()
     handles, labels = plt.gca().get_legend_handles_labels()
@@ -1072,15 +1073,15 @@
     result: Result,
     i_chain: int = 0,
     par_indices: Sequence[int] = None,
     full_trace: bool = False,
     stepsize: int = 1,
     use_problem_bounds: bool = True,
     suptitle: str = None,
-    size: Tuple[float, float] = None,
+    size: tuple[float, float] = None,
     ax: matplotlib.axes.Axes = None,
 ):
     """
     Plot parameter values over iterations.
 
     Parameters
     ----------
@@ -1130,23 +1131,23 @@
         fig, ax = plt.subplots(num_row, num_col, squeeze=False, figsize=size)
     else:
         fig = ax.get_figure()
 
     par_ax = dict(zip(param_names, ax.flat))
 
     sns.set(style="ticks")
-    kwargs = {'edgecolor': "w", 'linewidth': 0.3, 's': 10}  # for edge color
+    kwargs = {"edgecolor": "w", "linewidth": 0.3, "s": 10}  # for edge color
 
     if full_trace:
-        kwargs['hue'] = "converged"
-        if len(params_fval[kwargs['hue']].unique()) == 1:
-            kwargs['palette'] = ["#477ccd"]
-        elif len(params_fval[kwargs['hue']].unique()) == 2:
-            kwargs['palette'] = ["#868686", "#477ccd"]
-        kwargs['legend'] = False
+        kwargs["hue"] = "converged"
+        if len(params_fval[kwargs["hue"]].unique()) == 1:
+            kwargs["palette"] = ["#477ccd"]
+        elif len(params_fval[kwargs["hue"]].unique()) == 2:
+            kwargs["palette"] = ["#868686", "#477ccd"]
+        kwargs["legend"] = False
 
     if result.sample_result.burn_in is None:
         _burn_in = 0
     else:
         _burn_in = result.sample_result.burn_in
 
     for idx, plot_id in enumerate(param_names):
@@ -1159,20 +1160,20 @@
             ax=_ax,
             **kwargs,
         )
 
         if full_trace and _burn_in > 0:
             _ax.axvline(
                 _burn_in,
-                linestyle='--',
+                linestyle="--",
                 linewidth=1.5,
-                color='k',
+                color="k",
             )
 
-        _ax.set_xlabel('iteration index')
+        _ax.set_xlabel("iteration index")
         _ax.set_ylabel(param_names[idx])
         if use_problem_bounds:
             _ax.set_ylim([theta_lb[idx], theta_ub[idx]])
 
     if suptitle:
         fig.suptitle(suptitle)
 
@@ -1184,15 +1185,15 @@
 
 def sampling_scatter(
     result: Result,
     i_chain: int = 0,
     stepsize: int = 1,
     suptitle: str = None,
     diag_kind: str = "kde",
-    size: Tuple[float, float] = None,
+    size: tuple[float, float] = None,
     show_bounds: bool = True,
 ):
     """
     Parameter scatter plot.
 
     Parameters
     ----------
@@ -1223,15 +1224,15 @@
         result=result, i_chain=i_chain, stepsize=stepsize
     )
 
     sns.set(style="ticks")
 
     # TODO: Think this throws the axis errors in seaborn.
     ax = sns.pairplot(
-        params_fval.drop(['logPosterior', 'iteration'], axis=1),
+        params_fval.drop(["logPosterior", "iteration"], axis=1),
         diag_kind=diag_kind,
     )
 
     if size is not None:
         ax.fig.set_size_inches(size)
 
     if suptitle:
@@ -1248,18 +1249,18 @@
 
 
 def sampling_1d_marginals(
     result: Result,
     i_chain: int = 0,
     par_indices: Sequence[int] = None,
     stepsize: int = 1,
-    plot_type: str = 'both',
-    bw_method: str = 'scott',
+    plot_type: str = "both",
+    bw_method: str = "scott",
     suptitle: str = None,
-    size: Tuple[float, float] = None,
+    size: tuple[float, float] = None,
 ):
     """
     Plot marginals.
 
     Parameters
     ----------
     result:
@@ -1303,36 +1304,36 @@
     fig, ax = plt.subplots(num_row, num_col, squeeze=False, figsize=size)
 
     par_ax = dict(zip(param_names, ax.flat))
     sns.set(style="ticks")
 
     # fig, ax = plt.subplots(nr_params, figsize=size)[1]
     for idx, par_id in enumerate(param_names):
-        if plot_type == 'kde':
+        if plot_type == "kde":
             # TODO: add bw_adjust as option?
             sns.kdeplot(
                 params_fval[par_id], bw_method=bw_method, ax=par_ax[par_id]
             )
-        elif plot_type == 'hist':
+        elif plot_type == "hist":
             # fixes usage of sns distplot which throws a future warning
             sns.histplot(
-                x=params_fval[par_id], ax=par_ax[par_id], stat='density'
+                x=params_fval[par_id], ax=par_ax[par_id], stat="density"
             )
             sns.rugplot(x=params_fval[par_id], ax=par_ax[par_id])
-        elif plot_type == 'both':
+        elif plot_type == "both":
             sns.histplot(
                 x=params_fval[par_id],
                 kde=True,
                 ax=par_ax[par_id],
-                stat='density',
+                stat="density",
             )
             sns.rugplot(x=params_fval[par_id], ax=par_ax[par_id])
 
         par_ax[par_id].set_xlabel(param_names[idx])
-        par_ax[par_id].set_ylabel('Density')
+        par_ax[par_id].set_ylabel("Density")
 
     sns.despine()
 
     if suptitle:
         fig.suptitle(suptitle)
 
     fig.tight_layout()
@@ -1379,15 +1380,16 @@
     # get parameters and fval results as numpy arrays (trace_x is numpy array)
     arr_param = np.asarray(result.sample_result.trace_x[i_chain])
 
     if result.sample_result.burn_in is None:
         warnings.warn(
             "Burn in index not found in the results, the full chain "
             "will be shown.\nYou may want to use, e.g., "
-            "`pypesto.sample.geweke_test`."
+            "`pypesto.sample.geweke_test`.",
+            stacklevel=2,
         )
         _burn_in = 0
     else:
         _burn_in = result.sample_result.burn_in
 
     # Burn in index
     if full_trace is False:
@@ -1408,22 +1410,22 @@
     theta_ub = result.problem.ub
 
     # get parameter names from all non-fixed parameters
     param_names = result.problem.get_reduced_vector(result.problem.x_names)
 
     # transform ndarray to pandas for the use of seaborn
     pd_params = pd.DataFrame(arr_param, columns=param_names)
-    pd_fval = pd.DataFrame(data=arr_fval, columns=['logPosterior'])
+    pd_fval = pd.DataFrame(data=arr_fval, columns=["logPosterior"])
 
-    pd_iter = pd.DataFrame(data=indices, columns=['iteration'])
+    pd_iter = pd.DataFrame(data=indices, columns=["iteration"])
 
     if full_trace:
-        converged = np.zeros((len(arr_fval)))
+        converged = np.zeros(len(arr_fval))
         converged[_burn_in:] = 1
-        pd_conv = pd.DataFrame(data=converged, columns=['converged'])
+        pd_conv = pd.DataFrame(data=converged, columns=["converged"])
 
         params_fval = pd.concat(
             [pd_params, pd_fval, pd_iter, pd_conv], axis=1, ignore_index=False
         )
     else:
         params_fval = pd.concat(
             [pd_params, pd_fval, pd_iter], axis=1, ignore_index=False
```

### Comparing `pypesto-0.4.2/pypesto/visualize/select.py` & `pypesto-0.5.0/pypesto/visualize/select.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Visualization routines for model selection with pyPESTO."""
 
-from typing import Dict, List, Tuple
 
 import matplotlib.pyplot as plt
 import networkx as nx
 from petab_select import Model
 from petab_select.constants import VIRTUAL_INITIAL_MODEL, Criterion
 
 from .. import select as pypesto_select
@@ -16,20 +15,20 @@
 def default_label_maker(model: Model) -> str:
     """Create a model label, for plotting."""
     return model.model_hash[:4]
 
 
 # FIXME supply the problem to automatically detect the correct criterion?
 def plot_selected_models(
-    selected_models: List[Model],
+    selected_models: list[Model],
     criterion: str = Criterion.AIC,
     relative: bool = True,
     fz: int = 14,
-    size: Tuple[float, float] = (5, 4),
-    labels: Dict[str, str] = None,
+    size: tuple[float, float] = (5, 4),
+    labels: dict[str, str] = None,
     ax: plt.Axes = None,
 ) -> plt.Axes:
     """Plot criterion for calibrated models.
 
     Parameters
     ----------
     selected_models:
@@ -71,62 +70,61 @@
     selected_models = [
         model for model in selected_models if model != VIRTUAL_INITIAL_MODEL
     ]
 
     criterion_values = {
         labels.get(
             model.get_hash(), default_label_maker(model)
-        ): model.get_criterion(criterion)
-        - zero
+        ): model.get_criterion(criterion) - zero
         for model in selected_models
     }
 
     ax.plot(
         criterion_values.keys(),
         criterion_values.values(),
         linewidth=linewidth,
-        color='lightgrey',
+        color="lightgrey",
         # edgecolor='k'
     )
 
     ax.get_xticks()
     ax.set_xticks(list(range(len(criterion_values))))
     ax.set_ylabel(
-        criterion + ('(relative)' if relative else '(absolute)'), fontsize=fz
+        criterion + ("(relative)" if relative else "(absolute)"), fontsize=fz
     )
     # could change to compared_model_ids, if all models are plotted
     ax.set_xticklabels(
         criterion_values.keys(),
         fontsize=fz + RELATIVE_LABEL_FONTSIZE,
     )
     for tick in ax.yaxis.get_major_ticks():
         tick.label1.set_fontsize(fz + RELATIVE_LABEL_FONTSIZE)
     ytl = ax.get_yticks()
     ax.set_ylim([min(ytl), max(ytl)])
     # removing top and right borders
-    ax.spines['top'].set_visible(False)
-    ax.spines['right'].set_visible(False)
+    ax.spines["top"].set_visible(False)
+    ax.spines["right"].set_visible(False)
     return ax
 
 
 def plot_history_digraph(*args, **kwargs):
     """Ignore me. Renamed to `plot_calibrated_models_digraph`."""
     raise NotImplementedError(
         "This method is now `plot_calibrated_models_digraph`."
     )
 
 
 def plot_calibrated_models_digraph(
     problem: pypesto_select.Problem,
-    calibrated_models: Dict[str, Model] = None,
+    calibrated_models: dict[str, Model] = None,
     criterion: Criterion = None,
     optimal_distance: float = 1,
     relative: bool = True,
-    options: Dict = None,
-    labels: Dict[str, str] = None,
+    options: dict = None,
+    labels: dict[str, str] = None,
     ax: plt.Axes = None,
 ) -> plt.Axes:
     """Plot all calibrated models in the model space, as a directed graph.
 
     TODO replace magic numbers with options/constants
 
     Parameters
@@ -176,27 +174,27 @@
                 predecessor_model = calibrated_models[predecessor_model_hash]
                 from_ = labels.get(
                     predecessor_model.get_hash(),
                     default_label_maker(predecessor_model),
                 )
         else:
             raise NotImplementedError(
-                'Plots for models with `None` as their predecessor model are '
-                'not yet implemented.'
+                "Plots for models with `None` as their predecessor model are "
+                "not yet implemented."
             )
-            from_ = 'None'
+            from_ = "None"
         to = labels.get(model.get_hash(), default_label_maker(model))
         edges.append((from_, to))
 
     G.add_edges_from(edges)
     default_options = {
-        'node_color': 'lightgrey',
-        'arrowstyle': '-|>',
-        'node_shape': 's',
-        'node_size': 2500,
+        "node_color": "lightgrey",
+        "arrowstyle": "-|>",
+        "node_shape": "s",
+        "node_size": 2500,
     }
     if options is not None:
         default_options.update(options)
 
     if ax is None:
         _, ax = plt.subplots(figsize=(12, 12))
```

### Comparing `pypesto-0.4.2/pypesto/visualize/spline_approximation.py` & `pypesto-0.5.0/pypesto/visualize/spline_approximation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 import warnings
-from typing import Optional, Sequence, Union
+from collections.abc import Sequence
+from typing import Optional, Union
 
 import matplotlib.axes
 import matplotlib.pyplot as plt
 import numpy as np
 
 import pypesto
 
 from ..C import (
     AMICI_SIGMAY,
     AMICI_Y,
     CURRENT_SIMULATION,
     DATAPOINTS,
+    EXPDATA_MASK,
     REGULARIZE_SPLINE,
     SCIPY_X,
+    SPLINE_KNOTS,
 )
 from ..problem import Problem
 from ..result import Result
 
 try:
     import amici
 
     from ..hierarchical import InnerCalculatorCollector
     from ..hierarchical.semiquantitative.calculator import SemiquantCalculator
     from ..hierarchical.semiquantitative.solver import (
         SemiquantInnerSolver,
         _calculate_regularization_for_group,
+        extract_expdata_using_mask,
         get_spline_mapped_simulations,
     )
 except ImportError:
     pass
 
 
 def plot_splines_from_pypesto_result(
@@ -54,22 +58,41 @@
         The axes.
     """
     # Check the calculator is the InnerCalculatorCollector.
     if not isinstance(
         pypesto_result.problem.objective.calculator, InnerCalculatorCollector
     ):
         raise ValueError(
-            'The calculator must be an instance of the InnerCalculatorCollector.'
+            "The calculator must be an instance of the InnerCalculatorCollector."
         )
 
+    # Get the spline knot values from the pypesto result
+    spline_knot_values = [
+        obs_spline_knots[1]
+        for obs_spline_knots in pypesto_result.optimize_result.list[
+            start_index
+        ][SPLINE_KNOTS]
+    ]
+
+    # Get inner parameters per observable as differences of spline knot values
+    inner_parameters = [
+        np.concatenate([[obs_knot_values[0]], np.diff(obs_knot_values)])
+        for obs_knot_values in spline_knot_values
+    ]
+
+    inner_results = [
+        {SCIPY_X: obs_inner_parameter}
+        for obs_inner_parameter in inner_parameters
+    ]
+
     # Get the parameters from the pypesto result for the start_index.
     x_dct = dict(
         zip(
             pypesto_result.problem.objective.x_ids,
-            pypesto_result.optimize_result.list[start_index]['x'],
+            pypesto_result.optimize_result.list[start_index]["x"],
         )
     )
 
     x_dct.update(
         pypesto_result.problem.objective.calculator.necessary_par_dummy_values
     )
 
@@ -97,58 +120,73 @@
         edatas,
         num_threads=min(n_threads, len(edatas)),
     )
 
     # If any amici simulation failed, raise warning and return None.
     if any(rdata.status != amici.AMICI_SUCCESS for rdata in inner_rdatas):
         warnings.warn(
-            'Warning: Some AMICI simulations failed. Cannot plot inner solutions.'
+            "Warning: Some AMICI simulations failed. Cannot plot inner "
+            "solutions.",
+            stacklevel=2,
         )
         return None
 
-    # Get simulation and sigma.
+    # Get simulation.
     sim = [rdata[AMICI_Y] for rdata in inner_rdatas]
-    sigma = [rdata[AMICI_SIGMAY] for rdata in inner_rdatas]
 
     spline_calculator = None
     for (
         calculator
     ) in pypesto_result.problem.objective.calculator.inner_calculators:
         if isinstance(calculator, SemiquantCalculator):
             spline_calculator = calculator
             break
 
+    if spline_calculator is None:
+        raise ValueError(
+            "No SemiquantCalculator found in the inner_calculators of the objective. "
+            "Cannot plot splines."
+        )
+
     # Get the inner solver and problem.
     inner_solver = spline_calculator.inner_solver
     inner_problem = spline_calculator.inner_problem
 
-    inner_results = inner_solver.solve(inner_problem, sim, sigma)
-
     return plot_splines_from_inner_result(
-        inner_problem, inner_solver, inner_results, observable_ids, **kwargs
+        inner_problem,
+        inner_solver,
+        inner_results,
+        sim,
+        observable_ids,
+        **kwargs,
     )
 
 
 def plot_splines_from_inner_result(
-    inner_problem: 'pypesto.hierarchical.spline_approximation.problem.SplineInnerProblem',
-    inner_solver: 'pypesto.hierarchical.spline_approximation.solver.SplineInnerSolver',
+    inner_problem: "pypesto.hierarchical.spline_approximation.problem.SplineInnerProblem",
+    inner_solver: "pypesto.hierarchical.spline_approximation.solver.SplineInnerSolver",
     results: list[dict],
+    sim: list[np.ndarray],
     observable_ids=None,
     **kwargs,
 ):
     """Plot the inner solutions.
 
     Parameters
     ----------
     inner_problem:
         The inner problem.
     inner_solver:
         The inner solver.
     results:
         The results from the inner solver.
+    sim:
+        The simulated model output.
+    observable_ids:
+        The ids of the observables.
     kwargs:
         Additional arguments to pass to the plotting function.
 
     Returns
     -------
     fig:
         The figure.
@@ -181,75 +219,77 @@
         axs = axs.flatten()
 
     # for each result and group, plot the inner solution
     for result, group in zip(results, inner_problem.groups):
         group_idx = list(inner_problem.groups.keys()).index(group)
 
         # For each group get the inner parameters and simulation
-        xs = inner_problem.get_xs_for_group(group)
-
         s = result[SCIPY_X]
 
-        inner_parameters = np.array([x.value for x in xs])
+        # Utility matrix for the spline knot calculation
+        lower_trian = np.tril(np.ones((len(s), len(s))))
+        spline_knots = np.dot(lower_trian, s)
+
         measurements = inner_problem.groups[group][DATAPOINTS]
-        simulation = inner_problem.groups[group][CURRENT_SIMULATION]
+        simulation = extract_expdata_using_mask(
+            expdata=sim, mask=inner_problem.groups[group][EXPDATA_MASK]
+        )
 
         # For the simulation, get the spline bases
         (
             delta_c,
             spline_bases,
             n,
         ) = SemiquantInnerSolver._rescale_spline_bases(
-            self=None,
             sim_all=simulation,
-            N=len(inner_parameters),
+            N=len(spline_knots),
             K=len(simulation),
         )
         mapped_simulations = get_spline_mapped_simulations(
-            s, simulation, len(inner_parameters), delta_c, spline_bases, n
+            s, simulation, len(spline_knots), delta_c, spline_bases, n
         )
 
         axs[group_idx].plot(
-            simulation, measurements, 'bs', label='Measurements'
+            simulation, measurements, "bs", label="Measurements"
         )
         axs[group_idx].plot(
-            spline_bases, inner_parameters, 'g.', label='Spline knots'
+            spline_bases, spline_knots, "g.", label="Spline knots"
         )
         axs[group_idx].plot(
             spline_bases,
-            inner_parameters,
-            linestyle='-',
-            color='g',
-            label='Spline function',
+            spline_knots,
+            linestyle="-",
+            color="g",
+            label="Spline function",
         )
         if inner_solver.options[REGULARIZE_SPLINE]:
             alpha_opt, beta_opt = _calculate_optimal_regularization(
                 s=s,
-                N=len(inner_parameters),
+                N=len(spline_knots),
                 c=spline_bases,
             )
             axs[group_idx].plot(
                 spline_bases,
                 alpha_opt * spline_bases + beta_opt,
-                linestyle='--',
-                color='orange',
-                label='Regularization line',
+                linestyle="--",
+                color="orange",
+                label="Regularization line",
             )
 
         axs[group_idx].plot(
-            simulation, mapped_simulations, 'r^', label='Mapped simulation'
+            simulation, mapped_simulations, "r^", label="Mapped simulation"
         )
         axs[group_idx].legend()
         if observable_ids is not None:
-            axs[group_idx].set_title(f'{observable_ids[group-1]}')
+            axs[group_idx].set_title(f"{observable_ids[group-1]}")
         else:
-            axs[group_idx].set_title(f'Group {group}')
+            axs[group_idx].set_title(f"Group {group}")
 
-        axs[group_idx].set_xlabel('Model output')
-        axs[group_idx].set_ylabel('Measurements')
+        axs[group_idx].set_xlabel("Model output")
+        axs[group_idx].set_ylabel("Measurements")
 
     for ax in axs[len(results) :]:
         ax.remove()
 
     return fig, axs
 
 
@@ -321,15 +361,15 @@
     if axes is None:
         return None
 
     # Get the parameters from the pypesto result for the start_index.
     x_dct = dict(
         zip(
             pypesto_problem.objective.x_ids,
-            result.optimize_result.list[start_index]['x'],
+            result.optimize_result.list[start_index]["x"],
         )
     )
     x_dct.update(
         pypesto_problem.objective.calculator.necessary_par_dummy_values
     )
     # Get the needed objects from the pypesto problem.
     edatas = pypesto_problem.objective.edatas
@@ -354,15 +394,17 @@
         edatas,
         num_threads=min(n_threads, len(edatas)),
     )
 
     # If any amici simulation failed, raise warning and return None.
     if any(rdata.status != amici.AMICI_SUCCESS for rdata in inner_rdatas):
         warnings.warn(
-            'Warning: Some AMICI simulations failed. Cannot plot inner solutions.'
+            "Warning: Some AMICI simulations failed. Cannot plot inner "
+            "solutions.",
+            stacklevel=2,
         )
         return None
 
     # Get simulation and sigma.
     sim = [rdata[AMICI_Y] for rdata in inner_rdatas]
     sigma = [rdata[AMICI_SIGMAY] for rdata in inner_rdatas]
 
@@ -388,64 +430,60 @@
         ax = [
             ax
             for ax in axes.values()
             if observable_id in ax.legend().get_texts()[0].get_text().split()
         ][0]
 
         # Get the inner parameters and simulation.
-        xs = inner_problem.get_xs_for_group(group)
         s = inner_result[SCIPY_X]
-
-        inner_parameters = np.array([x.value for x in xs])
         simulation = inner_problem.groups[group][CURRENT_SIMULATION]
 
         # For the simulation, get the spline bases
         (
             delta_c,
             spline_bases,
             n,
         ) = SemiquantInnerSolver._rescale_spline_bases(
-            self=None,
             sim_all=simulation,
-            N=len(inner_parameters),
+            N=len(s),
             K=len(simulation),
         )
         # and the spline-mapped simulations.
         mapped_simulations = get_spline_mapped_simulations(
-            s, simulation, len(inner_parameters), delta_c, spline_bases, n
+            s, simulation, len(s), delta_c, spline_bases, n
         )
 
         # Plot the spline-mapped simulations to the ax with same color
         # and timepoints as the lines which have 'simulation' in their label.
         plotted_index = 0
         for line in ax.lines:
-            if 'simulation' in line.get_label():
+            if "simulation" in line.get_label():
                 color = line.get_color()
                 timepoints = line.get_xdata()
                 condition_mapped_simulations = mapped_simulations[
                     plotted_index : len(timepoints) + plotted_index
                 ]
                 plotted_index += len(timepoints)
 
                 ax.plot(
                     timepoints,
                     condition_mapped_simulations,
                     color=color,
-                    linestyle='dotted',
-                    marker='^',
+                    linestyle="dotted",
+                    marker="^",
                 )
 
         # Add linestyle='dotted' and marker='^' to the legend as black spline mapped simulations.
         ax.plot(
             [],
             [],
-            color='black',
-            linestyle='dotted',
-            marker='^',
-            label='Spline mapped simulation',
+            color="black",
+            linestyle="dotted",
+            marker="^",
+            label="Spline mapped simulation",
         )
 
     # Reset the legend.
     for ax in axes.values():
         ax.legend()
 
     return axes
@@ -470,15 +508,15 @@
     -------
     The regularization term of the objective function for the start index.
     """
     # Get the parameters from the pypesto result for the start_index.
     x_dct = dict(
         zip(
             pypesto_result.problem.objective.x_ids,
-            pypesto_result.optimize_result.list[start_index]['x'],
+            pypesto_result.optimize_result.list[start_index]["x"],
         )
     )
 
     x_dct.update(
         pypesto_result.problem.objective.calculator.necessary_par_dummy_values
     )
 
@@ -505,15 +543,17 @@
         edatas,
         num_threads=min(n_threads, len(edatas)),
     )
 
     # If any amici simulation failed, raise warning and return None.
     if any(rdata.status != amici.AMICI_SUCCESS for rdata in inner_rdatas):
         warnings.warn(
-            'Warning: Some AMICI simulations failed. Cannot plot inner solutions.'
+            "Warning: Some AMICI simulations failed. Cannot plot inner "
+            "solutions.",
+            stacklevel=2,
         )
         return None
 
     # Get simulation and sigma.
     sim = [rdata[AMICI_Y] for rdata in inner_rdatas]
     sigma = [rdata[AMICI_SIGMAY] for rdata in inner_rdatas]
 
@@ -532,38 +572,33 @@
     inner_results = inner_solver.solve(inner_problem, sim, sigma)
 
     reg_term_sum = 0
 
     # for each result and group, plot the inner solution
     for result, group in zip(inner_results, inner_problem.groups):
         # For each group get the inner parameters and simulation
-        xs = inner_problem.get_xs_for_group(group)
-
         s = result[SCIPY_X]
-
-        inner_parameters = np.array([x.value for x in xs])
         simulation = inner_problem.groups[group][CURRENT_SIMULATION]
 
         # For the simulation, get the spline bases
         (
-            delta_c,
+            _,
             spline_bases,
-            n,
+            _,
         ) = SemiquantInnerSolver._rescale_spline_bases(
-            self=None,
             sim_all=simulation,
-            N=len(inner_parameters),
+            N=len(s),
             K=len(simulation),
         )
 
         if inner_solver.options[REGULARIZE_SPLINE]:
             reg_term = _calculate_regularization_for_group(
                 s=s,
-                N=len(inner_parameters),
+                N=len(s),
                 c=spline_bases,
                 regularization_factor=inner_solver.options[
-                    'regularization_factor'
+                    "regularization_factor"
                 ],
             )
             reg_term_sum += reg_term
 
     return reg_term_sum
```

### Comparing `pypesto-0.4.2/pypesto/visualize/waterfall.py` & `pypesto-0.5.0/pypesto/visualize/waterfall.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from typing import List, Optional, Sequence, Tuple, Union
+from collections.abc import Sequence
+from typing import Optional, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.ticker import MaxNLocator
 from mpl_toolkits.axes_grid1 import inset_locator
 
 from pypesto.util import delete_nan_inf
 
-from ..C import WATERFALL_MAX_VALUE
+from ..C import ALL, WATERFALL_MAX_VALUE
 from ..result import Result
 from .clust_color import RGBA, assign_colors
 from .misc import (
     process_offset_y,
     process_result_list,
     process_start_indices,
     process_y_limits,
@@ -19,16 +20,16 @@
 from .reference_points import ReferencePoint, create_references
 
 
 def waterfall(
     results: Union[Result, Sequence[Result]],
     ax: Optional[plt.Axes] = None,
     size: Optional[tuple[float, float]] = (18.5, 10.5),
-    y_limits: Optional[Tuple[float]] = None,
-    scale_y: Optional[str] = 'log10',
+    y_limits: Optional[tuple[float]] = None,
+    scale_y: Optional[str] = "log10",
     offset_y: Optional[float] = None,
     start_indices: Optional[Union[Sequence[int], int]] = None,
     n_starts_to_zoom: int = 0,
     reference: Optional[Sequence[ReferencePoint]] = None,
     colors: Optional[Union[RGBA, Sequence[RGBA]]] = None,
     legends: Optional[Union[Sequence[str], str]] = None,
     order_by_id: bool = False,
@@ -81,26 +82,33 @@
         ax = plt.subplots()[1]
         fig = plt.gcf()
         fig.set_size_inches(*size)
 
     if n_starts_to_zoom:
         # create zoom in
         inset_axes = inset_locator.inset_axes(
-            ax, width="30%", height="30%", loc='center right'
+            ax, width="30%", height="30%", loc="center right"
         )
         inset_locator.mark_inset(ax, inset_axes, loc1=2, loc2=4)
     else:
         inset_axes = None
 
     # parse input
     (results, colors, legends) = process_result_list(results, colors, legends)
 
     # handle `order_by_id`
     if order_by_id:
         start_id_ordering = get_ordering_by_start_id(results)
+        # Set start indices to all, and save actual start indices for later,
+        # so that all fvals are retrieved by `process_offset_for_list`.
+        # This enables use of `order_by_id` with `start_indices`.
+        ordered_start_indices = process_start_indices(
+            result=results[0], start_indices=start_indices
+        )
+        start_indices = ALL
 
     refs = create_references(references=reference)
 
     # precompute y-offset, if needed and if a list of results was passed
     fvals_all, offset_y = process_offset_for_list(
         offset_y, results, scale_y, start_indices, refs
     )
@@ -129,14 +137,15 @@
             fvals = []
             for start_id in start_id_ordering:
                 start_index = start_ids.index(start_id)
                 if fvals_raw_is_finite[start_index]:
                     fvals.append(fvals_raw[start_index])
                 else:
                     fvals.append(None)
+            fvals = np.array(fvals)[ordered_start_indices]
         else:
             # remove nan or inf values in fvals
             # also remove extremely large values. These values result in `inf`
             # values in the output of `scipy.cluster.hierarchy.linkage` in the
             # method `pypesto.util.assign_clusters`, which raises errors.
             _, fvals = delete_nan_inf(
                 fvals=fvals_raw, magnitude_bound=WATERFALL_MAX_VALUE
@@ -171,28 +180,28 @@
         inset_axes = handle_options(
             inset_axes, n_starts_to_zoom, refs, None, offset_y
         )
 
     if any(legends):
         ax.legend()
     # labels
-    ax.set_xlabel('Ordered optimizer run')
+    ax.set_xlabel("Ordered optimizer run")
     if offset_y == 0.0:
-        ax.set_ylabel('Function value')
+        ax.set_ylabel("Function value")
     else:
-        ax.set_ylabel(f'Objective value (offset={offset_y:0.3e})')
-    ax.set_title('Waterfall plot')
+        ax.set_ylabel(f"Objective value (offset={offset_y:0.3e})")
+    ax.set_title("Waterfall plot")
     return ax
 
 
 def waterfall_lowlevel(
     fvals,
     ax: Optional[plt.Axes] = None,
-    size: Optional[Tuple[float]] = (18.5, 10.5),
-    scale_y: str = 'log10',
+    size: Optional[tuple[float]] = (18.5, 10.5),
+    scale_y: str = "log10",
     offset_y: float = 0.0,
     colors: Optional[Union[RGBA, Sequence[RGBA]]] = None,
     legend_text: Optional[str] = None,
 ):
     """
     Plot waterfall plot using list of function values.
 
@@ -235,15 +244,15 @@
 
     # assign colors
     colors = assign_colors(fvals, colors=colors)
 
     # plot
     ax.xaxis.set_major_locator(MaxNLocator(integer=True))
     # plot line
-    if scale_y == 'log10':
+    if scale_y == "log10":
         ax.semilogy(start_indices, fvals, color=[0.7, 0.7, 0.7, 0.6])
     else:
         ax.plot(start_indices, fvals, color=[0.7, 0.7, 0.7, 0.6])
 
     # plot points
     for j in start_indices:
         # parse data for plotting
@@ -251,56 +260,56 @@
         fval = fvals[start_indices.index(j)]
         if j == start_indices[0]:
             tmp_legend = legend_text
         else:
             tmp_legend = None
 
         # line plot (linear or logarithmic)
-        if scale_y == 'log10':
+        if scale_y == "log10":
             ax.semilogy(
-                j, fval, color=color, marker='o', label=tmp_legend, alpha=1.0
+                j, fval, color=color, marker="o", label=tmp_legend, alpha=1.0
             )
         else:
             ax.plot(
-                j, fval, color=color, marker='o', label=tmp_legend, alpha=1.0
+                j, fval, color=color, marker="o", label=tmp_legend, alpha=1.0
             )
 
     # check if y-axis has a reasonable scale
     y_min, y_max = ax.get_ylim()
-    if scale_y == 'log10':
+    if scale_y == "log10":
         if np.log10(y_max) - np.log10(y_min) < 1.0:
             ax.set_ylim(
                 ax.dataLim.y0 - 0.001 * abs(ax.dataLim.y0),
                 ax.dataLim.y1 + 0.001 * abs(ax.dataLim.y1),
             )
     else:
         if y_max - y_min < 1.0:
             y_mean = 0.5 * (y_min + y_max)
             ax.set_ylim(y_mean - 0.5, y_mean + 0.5)
 
     # labels
-    ax.set_xlabel('Ordered optimizer run')
+    ax.set_xlabel("Ordered optimizer run")
     if offset_y == 0.0:
-        ax.set_ylabel('Function value')
+        ax.set_ylabel("Function value")
     else:
-        ax.set_ylabel('Objective value (offset={offset_y:0.3e})')
-    ax.set_title('Waterfall plot')
+        ax.set_ylabel("Objective value (offset={offset_y:0.3e})")
+    ax.set_title("Waterfall plot")
     if legend_text is not None:
         ax.legend()
 
     return ax
 
 
 def process_offset_for_list(
     offset_y: float,
     results: Sequence[Result],
     scale_y: Optional[str],
     start_indices: Optional[Sequence[int]] = None,
     references: Optional[Sequence[ReferencePoint]] = None,
-) -> Tuple[List[np.ndarray], float]:
+) -> tuple[list[np.ndarray], float]:
     """
     Compute common offset_y and add it to `fvals` of results.
 
     Parameters
     ----------
     offset_y:
         User provided offset_y
@@ -333,23 +342,23 @@
         if np.isfinite(fvals).any():
             min_val = min(min_val, np.nanmin(fvals[np.isfinite(fvals)]))
 
         fvals_all.append(fvals)
 
     # if there are references, also account for those
     if references:
-        min_val = min(min_val, np.nanmin([r['fval'] for r in references]))
+        min_val = min(min_val, np.nanmin([r["fval"] for r in references]))
 
     offset_y = process_offset_y(offset_y, scale_y, float(min_val))
 
     # return offsetted values
     return [fvals + offset_y for fvals in fvals_all], offset_y
 
 
-def get_ordering_by_start_id(results: Sequence[Result]) -> List[int]:
+def get_ordering_by_start_id(results: Sequence[Result]) -> list[int]:
     """Get an ordering of start IDs.
 
     The ordering is generated by taking the best function value for each
     start across all results, then sorting these best function values.
     This means that the minimum value of the waterfall plot is
     monotonically increasing.
 
@@ -426,15 +435,15 @@
     """
     # handle reference points
     for i_ref in ref:
         # plot reference point as line
         ax.plot(
             [0, max_len_fvals - 1],
             [i_ref.fval + offset_y, i_ref.fval + offset_y],
-            '--',
+            "--",
             color=i_ref.color,
             label=i_ref.legend,
         )
 
         # create legend for reference points
         if i_ref.legend is not None:
             ax.legend()
```

### Comparing `pypesto-0.4.2/pypesto.egg-info/PKG-INFO` & `pypesto-0.5.0/pypesto.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypesto
-Version: 0.4.2
+Version: 0.5.0
 Summary: python-based Parameter EStimation TOolbox
 Home-page: https://github.com/icb-dcm/pypesto
 Download-URL: https://github.com/icb-dcm/pypesto/releases
 Author: The pyPESTO developers
 Author-email: yannik.schaelte@gmail.com
 Maintainer: Paul Jonas Jost, Maren Philipps, Domagoj Dorešić, Fabian Fröhlich
 Maintainer-email: paul.jost@uni-bonn.de, maren.philipps@uni-bonn.de, domagoj.doresic@uni-bonn.de, fabian.frohlich@crick.ac.uk
@@ -30,25 +30,26 @@
 Requires-Dist: matplotlib>=3.6.2
 Requires-Dist: more-itertools>=9.0.0
 Requires-Dist: seaborn>=0.11.2
 Requires-Dist: h5py>=3.1.0
 Requires-Dist: tqdm>=4.46.0
 Requires-Dist: tabulate>=0.8.10
 Provides-Extra: all
-Requires-Dist: amici>=0.18.0; extra == "all"
+Requires-Dist: amici>=0.21.0; extra == "all"
 Requires-Dist: petab>=0.2.0; extra == "all"
 Requires-Dist: cyipopt>=1.3.0; extra == "all"
 Requires-Dist: dlib>=19.19.0; extra == "all"
 Requires-Dist: nlopt>=2.6.2; extra == "all"
 Requires-Dist: pyswarm>=0.6; extra == "all"
 Requires-Dist: cma>=3.0.3; extra == "all"
 Requires-Dist: pyswarms>=1.3.0; extra == "all"
 Requires-Dist: fides>=0.6.1; extra == "all"
 Requires-Dist: mpi4py>=3.0.3; extra == "all"
 Requires-Dist: arviz>=0.12.1; extra == "all"
+Requires-Dist: scipy<1.13.0; extra == "all"
 Requires-Dist: aesara>=2.8.6; extra == "all"
 Requires-Dist: pymc>=4.2.1; extra == "all"
 Requires-Dist: aesara>=2.0.5; extra == "all"
 Requires-Dist: jax>=0.4.1; extra == "all"
 Requires-Dist: jaxlib>=0.4.1; extra == "all"
 Requires-Dist: julia>=0.5.7; extra == "all"
 Requires-Dist: ipython>=8.4.0; extra == "all"
@@ -66,77 +67,84 @@
 Requires-Dist: ipython>=8.4.0; extra == "all"
 Requires-Dist: myst-parser>=0.18.0; extra == "all"
 Requires-Dist: ipykernel==6.23.1; extra == "all"
 Requires-Dist: julia>=0.5.7; extra == "all"
 Requires-Dist: ipython>=8.4.0; extra == "all"
 Requires-Dist: pygments>=2.12.0; extra == "all"
 Requires-Dist: arviz>=0.12.1; extra == "all"
+Requires-Dist: scipy<1.13.0; extra == "all"
 Requires-Dist: aesara>=2.8.6; extra == "all"
 Requires-Dist: pymc>=4.2.1; extra == "all"
 Requires-Dist: emcee>=3.0.2; extra == "all"
 Requires-Dist: dynesty>=2.0.3; extra == "all"
 Requires-Dist: nlopt>=2.6.2; extra == "all"
 Requires-Dist: pyswarm>=0.6; extra == "all"
 Requires-Dist: notebook>=6.1.4; extra == "all"
 Requires-Dist: networkx>=2.5.1; extra == "all"
 Requires-Dist: petab-select>=0.1.12; extra == "all"
 Requires-Dist: fides>=0.6.1; extra == "all"
-Requires-Dist: amici>=0.18.0; extra == "all"
+Requires-Dist: amici>=0.21.0; extra == "all"
 Requires-Dist: petab>=0.2.0; extra == "all"
 Requires-Dist: aesara>=2.0.5; extra == "all"
 Requires-Dist: jax>=0.4.1; extra == "all"
 Requires-Dist: jaxlib>=0.4.1; extra == "all"
+Requires-Dist: libroadrunner>=2.6.0; extra == "all"
 Requires-Dist: julia>=0.5.7; extra == "all"
 Requires-Dist: ipython>=8.4.0; extra == "all"
 Requires-Dist: pygments>=2.12.0; extra == "all"
 Requires-Dist: arviz>=0.12.1; extra == "all"
+Requires-Dist: scipy<1.13.0; extra == "all"
 Requires-Dist: aesara>=2.8.6; extra == "all"
 Requires-Dist: pymc>=4.2.1; extra == "all"
 Requires-Dist: emcee>=3.0.2; extra == "all"
 Requires-Dist: dynesty>=2.0.3; extra == "all"
 Requires-Dist: nlopt>=2.6.2; extra == "all"
 Requires-Dist: pyswarm>=0.6; extra == "all"
 Requires-Dist: notebook>=6.1.4; extra == "all"
 Requires-Dist: networkx>=2.5.1; extra == "all"
 Requires-Dist: petab-select>=0.1.12; extra == "all"
 Requires-Dist: pytest>=5.4.3; extra == "all"
 Requires-Dist: pytest-cov>=2.10.0; extra == "all"
 Requires-Dist: gitpython>=3.1.7; extra == "all"
 Requires-Dist: pytest-rerunfailures>=9.1.1; extra == "all"
 Requires-Dist: autograd>=1.3; extra == "all"
+Requires-Dist: libroadrunner>=2.6.0; extra == "all"
 Provides-Extra: all-optimizers
 Requires-Dist: cyipopt>=1.3.0; extra == "all-optimizers"
 Requires-Dist: dlib>=19.19.0; extra == "all-optimizers"
 Requires-Dist: nlopt>=2.6.2; extra == "all-optimizers"
 Requires-Dist: pyswarm>=0.6; extra == "all-optimizers"
 Requires-Dist: cma>=3.0.3; extra == "all-optimizers"
 Requires-Dist: pyswarms>=1.3.0; extra == "all-optimizers"
 Requires-Dist: fides>=0.6.1; extra == "all-optimizers"
 Provides-Extra: amici
-Requires-Dist: amici>=0.18.0; extra == "amici"
+Requires-Dist: amici>=0.21.0; extra == "amici"
+Provides-Extra: roadrunner
+Requires-Dist: libroadrunner>=2.6.0; extra == "roadrunner"
 Provides-Extra: petab
 Requires-Dist: petab>=0.2.0; extra == "petab"
 Provides-Extra: ipopt
 Requires-Dist: cyipopt>=1.3.0; extra == "ipopt"
 Provides-Extra: dlib
 Requires-Dist: dlib>=19.19.0; extra == "dlib"
 Provides-Extra: nlopt
 Requires-Dist: nlopt>=2.6.2; extra == "nlopt"
 Provides-Extra: pyswarm
 Requires-Dist: pyswarm>=0.6; extra == "pyswarm"
-Provides-Extra: cmaes
-Requires-Dist: cma>=3.0.3; extra == "cmaes"
+Provides-Extra: cma
+Requires-Dist: cma>=3.0.3; extra == "cma"
 Provides-Extra: pyswarms
 Requires-Dist: pyswarms>=1.3.0; extra == "pyswarms"
 Provides-Extra: fides
 Requires-Dist: fides>=0.6.1; extra == "fides"
 Provides-Extra: mpi
 Requires-Dist: mpi4py>=3.0.3; extra == "mpi"
 Provides-Extra: pymc
 Requires-Dist: arviz>=0.12.1; extra == "pymc"
+Requires-Dist: scipy<1.13.0; extra == "pymc"
 Requires-Dist: aesara>=2.8.6; extra == "pymc"
 Requires-Dist: pymc>=4.2.1; extra == "pymc"
 Provides-Extra: aesara
 Requires-Dist: aesara>=2.0.5; extra == "aesara"
 Provides-Extra: jax
 Requires-Dist: jax>=0.4.1; extra == "jax"
 Requires-Dist: jaxlib>=0.4.1; extra == "jax"
@@ -161,34 +169,37 @@
 Requires-Dist: ipython>=8.4.0; extra == "doc"
 Requires-Dist: myst-parser>=0.18.0; extra == "doc"
 Requires-Dist: ipykernel==6.23.1; extra == "doc"
 Requires-Dist: julia>=0.5.7; extra == "doc"
 Requires-Dist: ipython>=8.4.0; extra == "doc"
 Requires-Dist: pygments>=2.12.0; extra == "doc"
 Requires-Dist: arviz>=0.12.1; extra == "doc"
+Requires-Dist: scipy<1.13.0; extra == "doc"
 Requires-Dist: aesara>=2.8.6; extra == "doc"
 Requires-Dist: pymc>=4.2.1; extra == "doc"
 Requires-Dist: emcee>=3.0.2; extra == "doc"
 Requires-Dist: dynesty>=2.0.3; extra == "doc"
 Requires-Dist: nlopt>=2.6.2; extra == "doc"
 Requires-Dist: pyswarm>=0.6; extra == "doc"
 Requires-Dist: notebook>=6.1.4; extra == "doc"
 Requires-Dist: networkx>=2.5.1; extra == "doc"
 Requires-Dist: petab-select>=0.1.12; extra == "doc"
 Requires-Dist: fides>=0.6.1; extra == "doc"
-Requires-Dist: amici>=0.18.0; extra == "doc"
+Requires-Dist: amici>=0.21.0; extra == "doc"
 Requires-Dist: petab>=0.2.0; extra == "doc"
 Requires-Dist: aesara>=2.0.5; extra == "doc"
 Requires-Dist: jax>=0.4.1; extra == "doc"
 Requires-Dist: jaxlib>=0.4.1; extra == "doc"
+Requires-Dist: libroadrunner>=2.6.0; extra == "doc"
 Provides-Extra: example
 Requires-Dist: julia>=0.5.7; extra == "example"
 Requires-Dist: ipython>=8.4.0; extra == "example"
 Requires-Dist: pygments>=2.12.0; extra == "example"
 Requires-Dist: arviz>=0.12.1; extra == "example"
+Requires-Dist: scipy<1.13.0; extra == "example"
 Requires-Dist: aesara>=2.8.6; extra == "example"
 Requires-Dist: pymc>=4.2.1; extra == "example"
 Requires-Dist: emcee>=3.0.2; extra == "example"
 Requires-Dist: dynesty>=2.0.3; extra == "example"
 Requires-Dist: nlopt>=2.6.2; extra == "example"
 Requires-Dist: pyswarm>=0.6; extra == "example"
 Requires-Dist: notebook>=6.1.4; extra == "example"
```

### Comparing `pypesto-0.4.2/pypesto.egg-info/SOURCES.txt` & `pypesto-0.5.0/pypesto.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -72,23 +72,27 @@
 pypesto/objective/amici/amici_util.py
 pypesto/objective/jax/__init__.py
 pypesto/objective/jax/base.py
 pypesto/objective/julia/__init__.py
 pypesto/objective/julia/base.py
 pypesto/objective/julia/petabJl.py
 pypesto/objective/julia/petab_jl_importer.py
+pypesto/objective/roadrunner/__init__.py
+pypesto/objective/roadrunner/petab_importer_roadrunner.py
+pypesto/objective/roadrunner/road_runner.py
+pypesto/objective/roadrunner/roadrunner_calculator.py
+pypesto/objective/roadrunner/utils.py
 pypesto/optimize/__init__.py
 pypesto/optimize/load.py
 pypesto/optimize/optimize.py
 pypesto/optimize/optimizer.py
 pypesto/optimize/options.py
 pypesto/optimize/task.py
 pypesto/optimize/util.py
 pypesto/optimize/ess/__init__.py
-pypesto/optimize/ess/cess.py
 pypesto/optimize/ess/ess.py
 pypesto/optimize/ess/function_evaluator.py
 pypesto/optimize/ess/refset.py
 pypesto/optimize/ess/sacess.py
 pypesto/petab/__init__.py
 pypesto/petab/importer.py
 pypesto/predict/__init__.py
```

### Comparing `pypesto-0.4.2/pypesto.egg-info/requires.txt` & `pypesto-0.5.0/pypesto.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,25 +9,26 @@
 tqdm>=4.46.0
 tabulate>=0.8.10
 
 [aesara]
 aesara>=2.0.5
 
 [all]
-amici>=0.18.0
+amici>=0.21.0
 petab>=0.2.0
 cyipopt>=1.3.0
 dlib>=19.19.0
 nlopt>=2.6.2
 pyswarm>=0.6
 cma>=3.0.3
 pyswarms>=1.3.0
 fides>=0.6.1
 mpi4py>=3.0.3
 arviz>=0.12.1
+scipy<1.13.0
 aesara>=2.8.6
 pymc>=4.2.1
 aesara>=2.0.5
 jax>=0.4.1
 jaxlib>=0.4.1
 julia>=0.5.7
 ipython>=8.4.0
@@ -43,14 +44,15 @@
 sphinx-autodoc-typehints>=1.18.3
 sphinxcontrib-bibtex>=2.5.0
 myst-parser>=0.18.0
 ipykernel==6.23.1
 notebook>=6.1.4
 networkx>=2.5.1
 petab-select>=0.1.12
+libroadrunner>=2.6.0
 pytest>=5.4.3
 pytest-cov>=2.10.0
 gitpython>=3.1.7
 pytest-rerunfailures>=9.1.1
 autograd>=1.3
 
 [all_optimizers]
@@ -59,17 +61,17 @@
 nlopt>=2.6.2
 pyswarm>=0.6
 cma>=3.0.3
 pyswarms>=1.3.0
 fides>=0.6.1
 
 [amici]
-amici>=0.18.0
+amici>=0.21.0
 
-[cmaes]
+[cma]
 cma>=3.0.3
 
 [dlib]
 dlib>=19.19.0
 
 [doc]
 sphinx>=6.2.1
@@ -80,41 +82,44 @@
 sphinxcontrib-bibtex>=2.5.0
 ipython>=8.4.0
 myst-parser>=0.18.0
 ipykernel==6.23.1
 julia>=0.5.7
 pygments>=2.12.0
 arviz>=0.12.1
+scipy<1.13.0
 aesara>=2.8.6
 pymc>=4.2.1
 emcee>=3.0.2
 dynesty>=2.0.3
 nlopt>=2.6.2
 pyswarm>=0.6
 notebook>=6.1.4
 networkx>=2.5.1
 petab-select>=0.1.12
 fides>=0.6.1
-amici>=0.18.0
+amici>=0.21.0
 petab>=0.2.0
 aesara>=2.0.5
 jax>=0.4.1
 jaxlib>=0.4.1
+libroadrunner>=2.6.0
 
 [dynesty]
 dynesty>=2.0.3
 
 [emcee]
 emcee>=3.0.2
 
 [example]
 julia>=0.5.7
 ipython>=8.4.0
 pygments>=2.12.0
 arviz>=0.12.1
+scipy<1.13.0
 aesara>=2.8.6
 pymc>=4.2.1
 emcee>=3.0.2
 dynesty>=2.0.3
 nlopt>=2.6.2
 pyswarm>=0.6
 notebook>=6.1.4
@@ -145,23 +150,27 @@
 nlopt>=2.6.2
 
 [petab]
 petab>=0.2.0
 
 [pymc]
 arviz>=0.12.1
+scipy<1.13.0
 aesara>=2.8.6
 pymc>=4.2.1
 
 [pyswarm]
 pyswarm>=0.6
 
 [pyswarms]
 pyswarms>=1.3.0
 
+[roadrunner]
+libroadrunner>=2.6.0
+
 [select]
 networkx>=2.5.1
 petab-select>=0.1.12
 
 [test]
 pytest>=5.4.3
 pytest-cov>=2.10.0
```

### Comparing `pypesto-0.4.2/setup.cfg` & `pypesto-0.5.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -65,44 +65,48 @@
 	%(emcee)s
 	%(dynesty)s
 	%(mltools)s
 	%(doc)s
 	%(example)s
 	%(select)s
 	%(test)s
+	%(roadrunner)s
 all_optimizers = 
 	%(ipopt)s
 	%(dlib)s
 	%(nlopt)s
 	%(pyswarm)s
-	%(cmaes)s
+	%(cma)s
 	%(pyswarms)s
 	%(fides)s
 amici = 
-	amici >= 0.18.0
+	amici >= 0.21.0
+roadrunner = 
+	libroadrunner >= 2.6.0
 petab = 
 	petab >= 0.2.0
 ipopt = 
 	cyipopt >= 1.3.0
 dlib = 
 	dlib >= 19.19.0
 nlopt = 
 	nlopt >= 2.6.2
 pyswarm = 
 	pyswarm >= 0.6
-cmaes = 
+cma = 
 	cma >= 3.0.3
 pyswarms = 
 	pyswarms >= 1.3.0
 fides = 
 	fides >= 0.6.1
 mpi = 
 	mpi4py >= 3.0.3
 pymc = 
 	arviz >= 0.12.1
+	scipy < 1.13.0 # https://github.com/ICB-DCM/pyPESTO/issues/1354
 	aesara >= 2.8.6
 	pymc >= 4.2.1
 aesara = 
 	aesara >= 2.0.5
 jax = 
 	jax >= 0.4.1
 	jaxlib >= 0.4.1
@@ -130,14 +134,15 @@
 	%(example)s
 	%(select)s
 	%(fides)s
 	%(amici)s
 	%(petab)s
 	%(aesara)s
 	%(jax)s
+	%(roadrunner)s
 example = 
 	%(julia)s
 	%(pymc)s
 	%(emcee)s
 	%(dynesty)s
 	%(nlopt)s
 	%(pyswarm)s
```

