# Comparing `tmp/mlpro-1.3.1.tar.gz` & `tmp/mlpro-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpro-1.3.1.tar", last modified: Sat Feb  3 15:20:01 2024, max compression
+gzip compressed data, was "mlpro-1.4.0.tar", last modified: Wed Apr 17 10:37:58 2024, max compression
```

## Comparing `mlpro-1.3.1.tar` & `mlpro-1.4.0.tar`

### file list

```diff
@@ -1,252 +1,249 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.625729 mlpro-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-02-03 15:19:46.000000 mlpro-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-03 15:19:46.000000 mlpro-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-02-03 15:20:01.625729 mlpro-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-02-03 15:19:46.000000 mlpro-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-03 15:19:46.000000 mlpro-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-02-03 15:20:01.629729 mlpro-1.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.585729 mlpro-1.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.593729 mlpro-1.3.1/src/mlpro/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.593729 mlpro-1.3.1/src/mlpro/bf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14747 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.593729 mlpro-1.3.1/src/mlpro/bf/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23793 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/datasets/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.593729 mlpro-1.3.1/src/mlpro/bf/math/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23130 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/math/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/math/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    12542 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/math/normalizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.597729 mlpro-1.3.1/src/mlpro/bf/ml/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53779 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/ml/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.597729 mlpro-1.3.1/src/mlpro/bf/ml/systems/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/ml/systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23245 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/ml/systems/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.597729 mlpro-1.3.1/src/mlpro/bf/ml/systems/pool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/ml/systems/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37878 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/mt.py
--rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.597729 mlpro-1.3.1/src/mlpro/bf/physics/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/physics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/physics/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14329 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/physics/unitconverter.py
--rw-r--r--   0 runner    (1001) docker     (127)    29371 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.597729 mlpro-1.3.1/src/mlpro/bf/streams/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    64843 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/streams/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.597729 mlpro-1.3.1/src/mlpro/bf/streams/samplers/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/streams/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/streams/samplers/min_wise.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/streams/samplers/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/streams/samplers/reservoir_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/streams/samplers/weighted_random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.601729 mlpro-1.3.1/src/mlpro/bf/streams/streams/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/streams/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14882 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/streams/streams/clouds.py
--rw-r--r--   0 runner    (1001) docker     (127)     8628 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/streams/streams/clouds2d_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/streams/streams/clouds2d_static.py
--rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/streams/streams/clouds3d_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/streams/streams/clouds3d_static.py
--rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/streams/streams/csv_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/streams/streams/doublespiral2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/streams/streams/provider_mlpro.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/streams/streams/rnd10d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.601729 mlpro-1.3.1/src/mlpro/bf/streams/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/streams/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8445 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/streams/tasks/deriver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/streams/tasks/rearranger.py
--rw-r--r--   0 runner    (1001) docker     (127)    19030 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/streams/tasks/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.601729 mlpro-1.3.1/src/mlpro/bf/streams/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/streams/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.601729 mlpro-1.3.1/src/mlpro/bf/systems/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    83676 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/systems/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.601729 mlpro-1.3.1/src/mlpro/bf/systems/pool/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/systems/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34965 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/systems/pool/doublependulum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/systems/pool/flipflops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.601729 mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.585729 mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.585729 mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.601729 mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)    37884 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Arrow.stl
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/X_letter.stl
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Y_letter.stl
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Z_letter.stl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.601729 mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/texture/
--rw-r--r--   0 runner    (1001) docker     (127)   322794 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/texture/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.585729 mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.605729 mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)    28984 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/base.stl
--rw-r--r--   0 runner    (1001) docker     (127)    52584 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/forearm.stl
--rw-r--r--   0 runner    (1001) docker     (127)    33784 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/shoulder.stl
--rw-r--r--   0 runner    (1001) docker     (127)    58884 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/upperarm.stl
--rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist1.stl
--rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist2.stl
--rw-r--r--   0 runner    (1001) docker     (127)    22384 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist3.stl
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/boxontable.xml
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/cartpole.xml
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/doublependulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/mlpro.xml
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/ur5.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.605729 mlpro-1.3.1/src/mlpro/bf/ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.605729 mlpro-1.3.1/src/mlpro/bf/ui/sciui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/ui/sciui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33615 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/ui/sciui/framework.py
--rw-r--r--   0 runner    (1001) docker     (127)    10903 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/ui/sciui/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.605729 mlpro-1.3.1/src/mlpro/bf/ui/sciui/pool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/ui/sciui/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24464 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/ui/sciui/pool/iis.py
--rw-r--r--   0 runner    (1001) docker     (127)    13746 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/ui/sciui/pool/iisbenchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.605729 mlpro-1.3.1/src/mlpro/bf/ui/sciui/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/ui/sciui/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/ui/sciui/templates/scenario_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    31658 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/bf/various.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.605729 mlpro-1.3.1/src/mlpro/gt/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/gt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.609729 mlpro-1.3.1/src/mlpro/gt/dynamicgames/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/gt/dynamicgames/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/gt/dynamicgames/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/gt/dynamicgames/potential.py
--rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/gt/dynamicgames/stackelberg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.609729 mlpro-1.3.1/src/mlpro/gt/native/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/gt/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    66293 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/gt/native/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.609729 mlpro-1.3.1/src/mlpro/gt/pool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/gt/pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.609729 mlpro-1.3.1/src/mlpro/gt/pool/boards/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/gt/pool/boards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/gt/pool/boards/bglp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/gt/pool/boards/multicartpole.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.609729 mlpro-1.3.1/src/mlpro/gt/pool/native/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/gt/pool/native/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.609729 mlpro-1.3.1/src/mlpro/gt/pool/native/games/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/gt/pool/native/games/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/gt/pool/native/games/prisonersdilemma_2p.py
--rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/gt/pool/native/games/prisonersdilemma_3p.py
--rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/gt/pool/native/games/rockpaperscissors.py
--rw-r--r--   0 runner    (1001) docker     (127)    12928 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/gt/pool/native/games/routingproblems_3p.py
--rw-r--r--   0 runner    (1001) docker     (127)    12811 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/gt/pool/native/games/supplydemand_3p.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.609729 mlpro-1.3.1/src/mlpro/gt/pool/native/solvers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/gt/pool/native/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/gt/pool/native/solvers/greedypolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/gt/pool/native/solvers/randomsolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.609729 mlpro-1.3.1/src/mlpro/gt/pool/policies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/gt/pool/policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.609729 mlpro-1.3.1/src/mlpro/oa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/oa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.609729 mlpro-1.3.1/src/mlpro/oa/sciui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/oa/sciui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31194 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/oa/sciui/iis.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/oa/sciui/runme.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/oa/sciui/scenario_oa1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.613729 mlpro-1.3.1/src/mlpro/oa/streams/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/oa/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13855 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/oa/streams/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.613729 mlpro-1.3.1/src/mlpro/oa/streams/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/oa/streams/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/oa/streams/tasks/anomalydetectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    11878 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/oa/streams/tasks/boundarydetectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    23367 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/oa/streams/tasks/clusteranalyzers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15142 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/oa/streams/tasks/normalizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.613729 mlpro-1.3.1/src/mlpro/oa/streams/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/oa/streams/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.613729 mlpro-1.3.1/src/mlpro/oa/systems/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/oa/systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40080 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/oa/systems/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.613729 mlpro-1.3.1/src/mlpro/oa/systems/pool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/oa/systems/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/oa/systems/pool/doublependulum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.613729 mlpro-1.3.1/src/mlpro/rl/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/rl/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    36302 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/rl/models_agents.py
--rw-r--r--   0 runner    (1001) docker     (127)    21239 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/rl/models_env.py
--rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/rl/models_env_ada.py
--rw-r--r--   0 runner    (1001) docker     (127)    15513 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/rl/models_env_oa.py
--rw-r--r--   0 runner    (1001) docker     (127)    48989 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/rl/models_train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.613729 mlpro-1.3.1/src/mlpro/rl/pool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/rl/pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.613729 mlpro-1.3.1/src/mlpro/rl/pool/actionplanner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/rl/pool/actionplanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/rl/pool/actionplanner/mpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.617729 mlpro-1.3.1/src/mlpro/rl/pool/envs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/rl/pool/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50258 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/rl/pool/envs/bglp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/rl/pool/envs/cartpole.py
--rw-r--r--   0 runner    (1001) docker     (127)    44837 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/rl/pool/envs/doublependulum.py
--rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/rl/pool/envs/gridworld.py
--rw-r--r--   0 runner    (1001) docker     (127)    13092 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/rl/pool/envs/multicartpole.py
--rw-r--r--   0 runner    (1001) docker     (127)    19097 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/rl/pool/envs/robotinhtm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.617729 mlpro-1.3.1/src/mlpro/rl/pool/policies/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/rl/pool/policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/rl/pool/policies/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/rl/pool/policies/randomgenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.617729 mlpro-1.3.1/src/mlpro/rl/pool/sarsbuffer/
--rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/rl/pool/sarsbuffer/PrioritizedBuffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/rl/pool/sarsbuffer/RandomSARSBuffer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/rl/pool/sarsbuffer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.617729 mlpro-1.3.1/src/mlpro/rl/pool/scenarios/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/rl/pool/scenarios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65877 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/rl/sciui_rl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.617729 mlpro-1.3.1/src/mlpro/sl/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/sl/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.617729 mlpro-1.3.1/src/mlpro/sl/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/sl/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/sl/examples/howto_sl_afct_100_train_and_reload_pytorch_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/sl/fnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/sl/models_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)    40710 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/sl/models_train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.617729 mlpro-1.3.1/src/mlpro/sl/pool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/sl/pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.621729 mlpro-1.3.1/src/mlpro/sl/pool/afct/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/sl/pool/afct/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.621729 mlpro-1.3.1/src/mlpro/sl/pool/afct/fnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/sl/pool/afct/fnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.621729 mlpro-1.3.1/src/mlpro/sl/pool/afct/fnn/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/sl/pool/afct/fnn/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22451 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/sl/pool/afct/fnn/pytorch/mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)    12154 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/sl/pool/afct/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.621729 mlpro-1.3.1/src/mlpro/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22809 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/wrappers/gymnasium.py
--rw-r--r--   0 runner    (1001) docker     (127)    11950 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/wrappers/hyperopt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/wrappers/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    38887 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/wrappers/mujoco.py
--rw-r--r--   0 runner    (1001) docker     (127)    13471 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/wrappers/openml.py
--rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/wrappers/optuna.py
--rw-r--r--   0 runner    (1001) docker     (127)    22931 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/wrappers/pettingzoo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.621729 mlpro-1.3.1/src/mlpro/wrappers/river/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/wrappers/river/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/wrappers/river/anomalydetectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/wrappers/river/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    32612 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/wrappers/river/clusteranalyzers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/wrappers/river/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)    22637 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/wrappers/sb3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.621729 mlpro-1.3.1/src/mlpro/wrappers/sklearn/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/wrappers/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9910 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/wrappers/sklearn/anomalydetectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-02-03 15:19:46.000000 mlpro-1.3.1/src/mlpro/wrappers/sklearn/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.625729 mlpro-1.3.1/src/mlpro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-02-03 15:20:01.000000 mlpro-1.3.1/src/mlpro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-02-03 15:20:01.000000 mlpro-1.3.1/src/mlpro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-03 15:20:01.000000 mlpro-1.3.1/src/mlpro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-03 15:20:01.000000 mlpro-1.3.1/src/mlpro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-03 15:20:01.000000 mlpro-1.3.1/src/mlpro.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 15:20:01.625729 mlpro-1.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-02-03 15:19:46.000000 mlpro-1.3.1/test/test_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-02-03 15:19:46.000000 mlpro-1.3.1/test/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-02-03 15:19:46.000000 mlpro-1.3.1/test/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-02-03 15:19:46.000000 mlpro-1.3.1/test/test_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-02-03 15:19:46.000000 mlpro-1.3.1/test/test_pool_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-02-03 15:19:46.000000 mlpro-1.3.1/test/test_sb3_policy_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-02-03 15:19:46.000000 mlpro-1.3.1/test/test_various.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.051833 mlpro-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-17 10:37:47.000000 mlpro-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-17 10:37:47.000000 mlpro-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-17 10:37:58.051833 mlpro-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-17 10:37:47.000000 mlpro-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-17 10:37:49.000000 mlpro-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-17 10:37:58.051833 mlpro-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.011834 mlpro-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.019834 mlpro-1.4.0/src/mlpro/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.019834 mlpro-1.4.0/src/mlpro/bf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14747 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.019834 mlpro-1.4.0/src/mlpro/bf/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23793 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/datasets/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.023834 mlpro-1.4.0/src/mlpro/bf/math/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23130 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/math/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/math/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12542 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/math/normalizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.023834 mlpro-1.4.0/src/mlpro/bf/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55808 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ml/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.023834 mlpro-1.4.0/src/mlpro/bf/ml/systems/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ml/systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23245 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ml/systems/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.023834 mlpro-1.4.0/src/mlpro/bf/ml/systems/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ml/systems/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37878 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/mt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.023834 mlpro-1.4.0/src/mlpro/bf/physics/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/physics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/physics/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14329 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/physics/unitconverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32607 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.023834 mlpro-1.4.0/src/mlpro/bf/streams/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64843 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.023834 mlpro-1.4.0/src/mlpro/bf/streams/samplers/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/samplers/min_wise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/samplers/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/samplers/reservoir_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/samplers/weighted_random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.027834 mlpro-1.4.0/src/mlpro/bf/streams/streams/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16799 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/streams/clouds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11195 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/streams/clouds_with_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/streams/csv_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/streams/doublespiral2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/streams/point_outliers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/streams/provider_mlpro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/streams/rnd10d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.027834 mlpro-1.4.0/src/mlpro/bf/streams/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8445 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/tasks/deriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/tasks/rearranger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19030 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/tasks/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.027834 mlpro-1.4.0/src/mlpro/bf/streams/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.027834 mlpro-1.4.0/src/mlpro/bf/systems/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83676 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.027834 mlpro-1.4.0/src/mlpro/bf/systems/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34965 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/doublependulum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/flipflops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.027834 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.011834 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.011834 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.027834 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)    37884 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Arrow.stl
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/X_letter.stl
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Y_letter.stl
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Z_letter.stl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.027834 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/texture/
+-rw-r--r--   0 runner    (1001) docker     (127)   322794 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/texture/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.011834 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.031834 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)    28984 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/base.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    52584 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/forearm.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    33784 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/shoulder.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    58884 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/upperarm.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist1.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist2.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    22384 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist3.stl
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/boxontable.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/cartpole.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/doublependulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/mlpro.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/ur5.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.031834 mlpro-1.4.0/src/mlpro/bf/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.031834 mlpro-1.4.0/src/mlpro/bf/ui/sciui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ui/sciui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33615 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ui/sciui/framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10903 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ui/sciui/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.031834 mlpro-1.4.0/src/mlpro/bf/ui/sciui/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ui/sciui/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24464 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ui/sciui/pool/iis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13746 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ui/sciui/pool/iisbenchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.031834 mlpro-1.4.0/src/mlpro/bf/ui/sciui/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ui/sciui/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ui/sciui/templates/scenario_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31658 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/various.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.031834 mlpro-1.4.0/src/mlpro/gt/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.035834 mlpro-1.4.0/src/mlpro/gt/dynamicgames/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/dynamicgames/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/dynamicgames/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/dynamicgames/potential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/dynamicgames/stackelberg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.035834 mlpro-1.4.0/src/mlpro/gt/native/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66293 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/native/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.035834 mlpro-1.4.0/src/mlpro/gt/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.035834 mlpro-1.4.0/src/mlpro/gt/pool/boards/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/boards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/boards/bglp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.035834 mlpro-1.4.0/src/mlpro/gt/pool/native/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/native/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.035834 mlpro-1.4.0/src/mlpro/gt/pool/native/games/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/native/games/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/native/games/prisonersdilemma_2p.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/native/games/prisonersdilemma_3p.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/native/games/rockpaperscissors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12928 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/native/games/routingproblems_3p.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12811 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/native/games/supplydemand_3p.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.035834 mlpro-1.4.0/src/mlpro/gt/pool/native/solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/native/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/native/solvers/greedypolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/native/solvers/randomsolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.035834 mlpro-1.4.0/src/mlpro/gt/pool/policies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.035834 mlpro-1.4.0/src/mlpro/oa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.035834 mlpro-1.4.0/src/mlpro/oa/sciui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/sciui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31194 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/sciui/iis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/sciui/runme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/sciui/scenario_oa1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.035834 mlpro-1.4.0/src/mlpro/oa/streams/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13855 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.039834 mlpro-1.4.0/src/mlpro/oa/streams/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.039834 mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.039834 mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/clusterbased.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/contextual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/drift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/cb_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/paga_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11878 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/boundarydetectors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.039834 mlpro-1.4.0/src/mlpro/oa/streams/tasks/clusteranalyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/clusteranalyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11422 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/clusteranalyzers/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.039834 mlpro-1.4.0/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14437 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15142 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/normalizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.039834 mlpro-1.4.0/src/mlpro/oa/streams/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.039834 mlpro-1.4.0/src/mlpro/oa/systems/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40080 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/systems/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.039834 mlpro-1.4.0/src/mlpro/oa/systems/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/systems/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/systems/pool/doublependulum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.043834 mlpro-1.4.0/src/mlpro/rl/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36302 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/models_agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21239 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/models_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/models_env_ada.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15513 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/models_env_oa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48989 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/models_train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.043834 mlpro-1.4.0/src/mlpro/rl/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.043834 mlpro-1.4.0/src/mlpro/rl/pool/actionplanner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/actionplanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/actionplanner/mpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.043834 mlpro-1.4.0/src/mlpro/rl/pool/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50258 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/envs/bglp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/envs/cartpole.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44837 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/envs/doublependulum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/envs/gridworld.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19097 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/envs/robotinhtm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.043834 mlpro-1.4.0/src/mlpro/rl/pool/policies/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/policies/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/policies/randomgenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.043834 mlpro-1.4.0/src/mlpro/rl/pool/sarsbuffer/
+-rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/sarsbuffer/PrioritizedBuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/sarsbuffer/RandomSARSBuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/sarsbuffer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.043834 mlpro-1.4.0/src/mlpro/rl/pool/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/scenarios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65877 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/sciui_rl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.047834 mlpro-1.4.0/src/mlpro/sl/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/sl/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.047834 mlpro-1.4.0/src/mlpro/sl/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/sl/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/sl/examples/howto_sl_afct_100_train_and_reload_pytorch_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/sl/fnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/sl/models_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40710 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/sl/models_train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.047834 mlpro-1.4.0/src/mlpro/sl/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/sl/pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.047834 mlpro-1.4.0/src/mlpro/sl/pool/afct/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/sl/pool/afct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.047834 mlpro-1.4.0/src/mlpro/sl/pool/afct/fnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/sl/pool/afct/fnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.047834 mlpro-1.4.0/src/mlpro/sl/pool/afct/fnn/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/sl/pool/afct/fnn/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22451 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/sl/pool/afct/fnn/pytorch/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12154 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/sl/pool/afct/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.047834 mlpro-1.4.0/src/mlpro/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/wrappers/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38971 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/wrappers/mujoco.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.047834 mlpro-1.4.0/src/mlpro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-17 10:37:57.000000 mlpro-1.4.0/src/mlpro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-17 10:37:58.000000 mlpro-1.4.0/src/mlpro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 10:37:57.000000 mlpro-1.4.0/src/mlpro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-17 10:37:57.000000 mlpro-1.4.0/src/mlpro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 10:37:57.000000 mlpro-1.4.0/src/mlpro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.047834 mlpro-1.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-17 10:37:49.000000 mlpro-1.4.0/test/test_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-17 10:37:49.000000 mlpro-1.4.0/test/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-17 10:37:49.000000 mlpro-1.4.0/test/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-17 10:37:49.000000 mlpro-1.4.0/test/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-17 10:37:49.000000 mlpro-1.4.0/test/test_pool_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-17 10:37:49.000000 mlpro-1.4.0/test/test_various.py
```

### Comparing `mlpro-1.3.1/LICENSE` & `mlpro-1.4.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,14 @@
 
 END OF TERMS AND CONDITIONS
 
 APPENDIX: How to apply the Apache License to your work
 
 To apply the Apache License to your work, attach the following boilerplate notice, with the fields enclosed by brackets "[]" replaced with your own identifying information. (Don't include the brackets!) The text should be enclosed in the appropriate comment syntax for the file format. We also recommend that a file or class name and description of purpose be included on the same "printed page" as the copyright notice for easier identification within third-party archives.
 
-Copyright [2021] [South Westphalia University of Applied Sciences, Germany]
+Copyright [2024] [South Westphalia University of Applied Sciences, Germany]
 
 Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at
 
 http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
```

### Comparing `mlpro-1.3.1/PKG-INFO` & `mlpro-1.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpro
-Version: 1.3.1
+Version: 1.4.0
 Summary: MLPro - The Integrative Middleware Framework for Standardized Machine Learning
 Home-page: https://mlpro.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,28 +13,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: full
 Requires-Dist: dill>=0.3.6; extra == "full"
 Requires-Dist: numpy>=1.24.2; extra == "full"
 Requires-Dist: torch>=2.0.0; extra == "full"
 Requires-Dist: matplotlib>=3.7.1; extra == "full"
-Requires-Dist: stable_baselines3>=2.1.0; extra == "full"
 Requires-Dist: scipy>=1.10.1; extra == "full"
-Requires-Dist: pettingzoo>=1.22.3; extra == "full"
-Requires-Dist: pygame>=2.1.3; extra == "full"
-Requires-Dist: pymunk>=6.4.0; extra == "full"
 Requires-Dist: multiprocess>=0.70.14; extra == "full"
-Requires-Dist: river!=0.20.0,!=0.20.1,>=0.15.0; extra == "full"
-Requires-Dist: scikit-learn>=1.2.2; extra == "full"
 Requires-Dist: optuna>=3.1.1; extra == "full"
 Requires-Dist: hyperopt>=0.2.7; extra == "full"
-Requires-Dist: pyglet>=1.5.27; extra == "full"
-Requires-Dist: mujoco>=2.3.3; extra == "full"
+Requires-Dist: mujoco!=3.1.4,>=2.3.3; extra == "full"
 Requires-Dist: lxml>=4.9.2; extra == "full"
-Requires-Dist: gymnasium>=0.29; extra == "full"
+Requires-Dist: pandas>=2.1.3; extra == "full"
 
 [![CI](https://github.com/fhswf/MLPro/actions/workflows/ci.yml/badge.svg)](https://github.com/fhswf/MLPro/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/mlpro/badge/?version=latest)](https://mlpro.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/mlpro.svg)](https://badge.fury.io/py/mlpro)
 [![Anaconda-Version Badge](https://anaconda.org/mlpro/mlpro/badges/version.svg)](https://anaconda.org/mlpro/mlpro)
 [![Anaconda-Downloads Badge](https://img.shields.io/conda/dn/mlpro/mlpro?color=green&label=Anaconda.org%20Total%20downloads&style=flat-square)](https://anaconda.org/mlpro/mlpro)
 [![PyPI Total Downloads](https://static.pepy.tech/personalized-badge/mlpro?period=total&units=international_system&left_color=blue&right_color=orange&left_text=PyPI%20Total%20Downloads)](https://pepy.tech/project/mlpro)
```

### Comparing `mlpro-1.3.1/README.md` & `mlpro-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/setup.cfg` & `mlpro-1.4.0/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mlpro
-version = 1.3.1
+version = 1.4.0
 author = MLPro Team
 author_email = mlpro@listen.fh-swf.de
 description = MLPro - The Integrative Middleware Framework for Standardized Machine Learning
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://mlpro.readthedocs.io
 project_urls = 
@@ -26,26 +26,19 @@
 
 [options.extras_require]
 full = 
 	dill>=0.3.6
 	numpy>=1.24.2
 	torch>=2.0.0
 	matplotlib>=3.7.1
-	stable_baselines3>=2.1.0
 	scipy>=1.10.1
-	pettingzoo>=1.22.3
-	pygame>=2.1.3
-	pymunk>=6.4.0
 	multiprocess>=0.70.14
-	river>=0.15.0,!=0.20.0,!=0.20.1
-	scikit-learn>=1.2.2
 	optuna>=3.1.1
 	hyperopt>=0.2.7
-	pyglet>=1.5.27
-	mujoco>=2.3.3
+	mujoco>=2.3.3,!=3.1.4
 	lxml>=4.9.2
-	gymnasium>=0.29
+	pandas>=2.1.3
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `mlpro-1.3.1/src/mlpro/bf/data.py` & `mlpro-1.4.0/src/mlpro/bf/data.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/datasets/basics.py` & `mlpro-1.4.0/src/mlpro/bf/datasets/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/events.py` & `mlpro-1.4.0/src/mlpro/bf/events.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/exceptions.py` & `mlpro-1.4.0/src/mlpro/bf/exceptions.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/math/basics.py` & `mlpro-1.4.0/src/mlpro/bf/math/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/math/geometry.py` & `mlpro-1.4.0/src/mlpro/bf/math/geometry.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 ## -- Package : mlpro.bf.math
 ## -- Module  : geometry.py
 ## -------------------------------------------------------------------------------------------------
 ## -- History :
 ## -- yyyy-mm-dd  Ver.      Auth.    Description
 ## -- 2023-04-18  0.0.0     DA       Creation
 ## -- 2023-12-28  1.0.0     DA       Finalized class Point
+## -- 2024-02-23  1.1.0     DA       Class Point: implementation of methods _renmove_plot*
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 1.0.0 (2023-12-28)
+Ver. 1.1.0 (2024-02-23)
 
 This module provides class for geometric objects like points, etc.
 
 """ 
 
 
 from mlpro.bf.plot import *
@@ -191,8 +192,24 @@
                                                   normalize = True,
                                                   color='red' )
     
 
 ## -------------------------------------------------------------------------------------------------
     def _update_plot_nd(self, p_settings: PlotSettings, **p_kwargs):
         pass
-    
+
+
+## -------------------------------------------------------------------------------------------------
+    def _remove_plot_2d(self):
+        if self._plot_pos is not None: self._plot_pos.remove()
+        if self._plot_vel is not None: self._plot_vel.remove()
+
+
+## -------------------------------------------------------------------------------------------------
+    def _remove_plot_3d(self):
+        if self._plot_pos is not None: self._plot_pos.remove()
+        if self._plot_vel is not None: self._plot_vel.remove()
+
+
+## -------------------------------------------------------------------------------------------------
+    def _remove_plot_nd(self):
+        pass
```

### Comparing `mlpro-1.3.1/src/mlpro/bf/math/normalizers.py` & `mlpro-1.4.0/src/mlpro/bf/math/normalizers.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/ml/basics.py` & `mlpro-1.4.0/src/mlpro/bf/ml/basics.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,23 +62,27 @@
 ## --                                - New methods get_training_path()
 ## -- 2023-03-09  2.1.1     DA       Class TrainingResults: removed parameter p_path
 ## -- 2023-03-10  2.1.2     DA       Class AdaptiveFunction: refactoring constructor parameters
 ## -- 2023-03-10  2.1.3     SY       Refactoring
 ## -- 2022-03-16  2.1.4     SY       Add _get_accuracy(), add_objective, _add_objective in Model
 ## -- 2023-03-29  2.2.0     DA       Classes Model, Scenario: refactoring of persistence
 ## -- 2023-04-10  2.2.1     SY       Update get_accuracy, add_objective in Model
+## -- 2023-07-24  2.3.0     LSB      New methods in context of hyperparameter tuning
+##                                   - _update_hyperparameters()
+##                                   - _hpt_updated
+##                                   - _hyperparameter_handler()
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 2.2.1 (2023-04-10)
+Ver. 2.3.0 (2023-07-24)
 
 This module provides the fundamental templates and processes for machine learning in MLPro.
 
 """
-
+import warnings
 
 from mlpro.bf.various import *
 from mlpro.bf.math import *
 from mlpro.bf.data import Buffer
 from mlpro.bf.mt import *
 from mlpro.bf.ops import Mode, ScenarioBase
 import random
@@ -251,14 +255,19 @@
 
         self._adapted           = False
         self.switch_adaptivity(p_ada)
         self._hyperparam_space  = HyperParamSpace()
         self._hyperparam_tuple  = None
         self._init_hyperparam(**p_par)
 
+        for hyper_param in self._hyperparam_space.get_dims():
+            hyper_param.register_event_handler(p_event_id=HyperParam.C_EVENT_VALUE_CHANGED, p_event_handler=self._hyperparam_handler)
+
+        self._hp_latest = True
+
         if p_buffer_size > 0:
             self._buffer = self.C_BUFFER_CLS(p_size=p_buffer_size)
         else:
             self._buffer = None
 
 
 ## -------------------------------------------------------------------------------------------------
@@ -285,14 +294,40 @@
         Returns the internal hyperparameter tuple to get access to single values.
         """
 
         return self._hyperparam_tuple
 
 
 ## -------------------------------------------------------------------------------------------------
+    def _hyperparam_handler(self, p_event_id, p_event_object:Event):
+        """
+        This is an event handler method for managing the updates of hyperparameters in the HPTuple.
+        Set's the flag hp_latest to false, as the hpt of the model are not latest to the tuple.
+        """
+        if p_event_id == HyperParam.C_EVENT_VALUE_CHANGED:
+            self._hp_latest = False
+
+
+## -------------------------------------------------------------------------------------------------
+    def _update_hyperparameters(self) -> bool:
+        """
+        Custom method to update the hyperparameters of a system with the latest value in the Hyperparameter Tuple.
+        This may be due to Hyperparameter Tuning. Please return True if the hyperparameters are updated successfully.
+
+        Returns
+        -------
+        bool:
+            True if the hyperparameters are updated successfully.
+
+        """
+
+        raise NotImplementedError
+
+
+## -------------------------------------------------------------------------------------------------
     def switch_adaptivity(self, p_ada:bool):
         """
         Switches adaption functionality on/off.
         
         Parameters
         ----------
         p_ada : bool
@@ -348,14 +383,23 @@
 
         Returns
         -------
         adapted : bool
             True, if something has been adapted. False otherwise.
 
         """
+        # Check if the hyperparameters are updated
+
+        if not self._hp_latest:
+            try:
+                self._hp_latest = self._update_hyperparameters()
+            except:
+                if not self._hp_latest:
+                    self.log(Log.C_LOG_TYPE_E, "No hyperparameter update mechanism provided. Runs will continue without update."
+                                  " Please read the documentation for method _update_hyperparameter() on Model class.")
 
         if not self._adaptivity: return False
         self.log(self.C_LOG_TYPE_S, 'Adaptation started')
         adapted = self._adapt(**p_kwargs)
         self._set_adapted(adapted)
         return adapted
```

### Comparing `mlpro-1.3.1/src/mlpro/bf/ml/systems/basics.py` & `mlpro-1.4.0/src/mlpro/bf/ml/systems/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/mt.py` & `mlpro-1.4.0/src/mlpro/bf/mt.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/ops.py` & `mlpro-1.4.0/src/mlpro/bf/ops.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/physics/basics.py` & `mlpro-1.4.0/src/mlpro/bf/physics/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/physics/unitconverter.py` & `mlpro-1.4.0/src/mlpro/bf/physics/unitconverter.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/plot.py` & `mlpro-1.4.0/src/mlpro/bf/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,18 +26,24 @@
 ## -- 2023-01-04  2.8.0     DA       Class PlotSettings: new parameters p_horizon, p_force_fg
 ## -- 2023-02-02  2.8.1     MRD      Disable Tkinter backend for macos https://bugs.python.org/issue46573
 ## -- 2023-02-17  2.8.2     SY       Add p_window_type in DataPlotting
 ## -- 2023-02-23  2.9.0     DA       Class PlotSettings: new parameter p_view_autoselect
 ## -- 2023-04-10  2.9.1     MRD      Turn on Tkinter backend for macos
 ## -- 2023-05-01  2.9.2     DA       Turn off Tkinter backend for macos due to workflow problems
 ## -- 2023-12-28  2.10.0    DA       Method Plottable._init_plot_3d(): init 3D view perspective
+## -- 2024-02-23  2.11.0    DA       Class Plottable: new methods
+## --                                - _remove_plot_2d(), _remove_plot_3d(), _remove_plot_nd()
+## --                                - __del__() 
+## -- 2024-02-24  2.11.1    DA       Class Plottable:
+## --                                - new methods remove_plot(), _remove_plot()
+## --                                - new methods refresh_plot(), _refresh_plot()
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 2.10.0 (2023-12-28)
+Ver. 2.11.1 (2024-02-24)
 
 This module provides various classes related to data plotting.
 """
 
 
 from operator import mod
 import numpy as np
@@ -261,17 +267,17 @@
 
          # 2 Prepare internal data structures
 
         # 2.1 Plot settings per view
         self.set_plot_settings( p_plot_settings=p_plot_settings )
 
         # 2.2 Dictionary with methods for initialization and update of a plot per view 
-        self._plot_methods = { PlotSettings.C_VIEW_2D : [ self._init_plot_2d, self._update_plot_2d ], 
-                               PlotSettings.C_VIEW_3D : [ self._init_plot_3d, self._update_plot_3d ], 
-                               PlotSettings.C_VIEW_ND : [ self._init_plot_nd, self._update_plot_nd ] }
+        self._plot_methods = { PlotSettings.C_VIEW_2D : [ self._init_plot_2d, self._update_plot_2d, self._remove_plot_2d ], 
+                               PlotSettings.C_VIEW_3D : [ self._init_plot_3d, self._update_plot_3d, self._remove_plot_3d ], 
+                               PlotSettings.C_VIEW_ND : [ self._init_plot_nd, self._update_plot_nd, self._remove_plot_nd ] }
 
 
         # 3 Setup the Matplotlib host figure if no one is provided as parameter
         if p_figure is None:
             self._figure : Figure   = self._init_figure()
             self._plot_own_figure   = True
         else:
@@ -303,14 +309,24 @@
 
 ## -------------------------------------------------------------------------------------------------
     def get_visualization(self) -> bool:
         return self._visualize
 
 
 ## -------------------------------------------------------------------------------------------------
+    def set_plot_step_rate(self, p_step_rate:int):
+        if p_step_rate > 0: self._plot_step_rate = p_step_rate
+
+
+## -------------------------------------------------------------------------------------------------
+    def set_plot_detail_level(self, p_detail_level:int):
+        self._plot_detail_level = max(0, p_detail_level)
+
+
+## -------------------------------------------------------------------------------------------------
     def _init_figure(self) -> Figure:
         """
         Custom method to initialize a suitable standalone Matplotlib figure.
 
         Returns
         -------
         figure : Matplotlib.figure.Figure
@@ -342,14 +358,53 @@
         backend = matplotlib.get_backend()
 
         if backend == 'TkAgg':
             p_fig.canvas.manager.window.attributes('-topmost', True)        
 
 
 ## -------------------------------------------------------------------------------------------------
+    def refresh_plot(self, p_force:bool=False):
+        """
+        Refreshes the plot.
+
+        Parameters
+        ----------
+        p_force : bool = False
+            On True the plot is updated even if it is embedded in a foreign host figure.
+        """
+    
+        # 1 Plot functionality turned on?
+        try:
+            if ( not self.C_PLOT_ACTIVE ) or ( not self._visualize ): return
+        except:
+            return
+        
+
+         # 1 Object has own figure or refresh is forced by caller?
+        if not self._plot_own_figure and not p_force: return
+            
+        if self._plot_own_figure:
+            self._plot_step_counter = mod(self._plot_step_counter+1, self._plot_settings.step_rate)
+        
+
+        # 2 Refresh plot
+        if ( self._plot_step_counter==0 ) or p_force: self._refresh_plot()
+            
+
+## -------------------------------------------------------------------------------------------------
+    def _refresh_plot(self):
+        """
+        Custom method to refresh the plot. Default implementation assumes standard use of Matplotlib.
+        """
+
+        self._figure.canvas.draw()
+        self._figure.canvas.flush_events()
+    
+
+## -------------------------------------------------------------------------------------------------
     def _init_plot_2d(self, p_figure:Figure, p_settings:PlotSettings):
         """
         Custom method to initialize a 2D plot. If attribute p_settings.axes is not None the 
         initialization shall be done there. Otherwise a new MatPlotLib Axes object shall be 
         created in the given figure and stored in p_settings.axes.
 
         Note: Please call this method in your custom implementation to create a default subplot.
@@ -433,19 +488,15 @@
             self.init_plot()
 
         # 2 Call of all required plot methods
         view = self._plot_settings.view
         self._plot_methods[view][1](p_settings=self._plot_settings, **p_kwargs)
 
         # 3 Update content of own(!) figure after self._plot_step_rate calls
-        if self._plot_own_figure:
-            self._plot_step_counter = mod(self._plot_step_counter+1, self._plot_settings.step_rate)
-            if self._plot_step_counter==0: 
-                self._figure.canvas.draw()
-                self._figure.canvas.flush_events()
+        self.refresh_plot(p_force=False)
 
 
 ## -------------------------------------------------------------------------------------------------
     def _update_plot_2d(self, p_settings:PlotSettings, **p_kwargs):
         """
         Custom method to update the 2d plot. The related MatPlotLib Axes object is stored in p_settings.
 
@@ -489,21 +540,68 @@
             Implementation-specific data and parameters.             
         """
 
         pass
 
 
 ## -------------------------------------------------------------------------------------------------
-    def set_plot_step_rate(self, p_step_rate:int):
-        if p_step_rate > 0: self._plot_step_rate = p_step_rate
+    def remove_plot(self, p_refresh:bool = True):
+        """"
+        Removes the plot and optionally refreshes the display.
+
+        Parameters
+        ----------
+        p_refresh : bool = True
+            On True the display is refreshed after removal
+        """
+
+        # 1 Plot functionality turned on?
+        try:
+            if ( not self.C_PLOT_ACTIVE ) or ( not self._visualize ): return
+        except:
+            return
+            
+         # 2 Call _remove_plot method of current view
+        view = self._plot_settings.view
+        self._plot_methods[view][2]()
 
+        # 3 Optionally refresh
+        if p_refresh: self.refresh_plot(p_force=False)
+    
 
 ## -------------------------------------------------------------------------------------------------
-    def set_plot_detail_level(self, p_detail_level:int):
-        self._plot_detail_level = max(0, p_detail_level)
+    def _remove_plot_2d(self):
+        """
+        Custom method to remove 2D plot artifacts when object is destroyed.
+        """
+
+        pass
+
+
+## -------------------------------------------------------------------------------------------------
+    def _remove_plot_3d(self):
+        """
+        Custom method to remove 3D plot artifacts when object is destroyed.
+        """
+
+        pass
+
+
+## -------------------------------------------------------------------------------------------------
+    def _remove_plot_nd(self):
+        """
+        Custom method to remove nd plot artifacts when object is destroyed.
+        """
+
+        pass
+
+
+## -------------------------------------------------------------------------------------------------
+    # def __del__(self):
+    #     self.remove_plot(p_refresh=True)
 
 
 
 
 
 ## -------------------------------------------------------------------------------------------------
 ## -------------------------------------------------------------------------------------------------
```

### Comparing `mlpro-1.3.1/src/mlpro/bf/streams/models.py` & `mlpro-1.4.0/src/mlpro/bf/streams/models.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/streams/samplers/min_wise.py` & `mlpro-1.4.0/src/mlpro/bf/streams/samplers/min_wise.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/streams/samplers/random.py` & `mlpro-1.4.0/src/mlpro/bf/streams/samplers/random.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/streams/samplers/reservoir_sampling.py` & `mlpro-1.4.0/src/mlpro/bf/streams/samplers/reservoir_sampling.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/streams/samplers/weighted_random.py` & `mlpro-1.4.0/src/mlpro/bf/streams/samplers/weighted_random.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/streams/streams/clouds.py` & `mlpro-1.4.0/src/mlpro/bf/streams/streams/clouds.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 ## -------------------------------------------------------------------------------------------------
 ## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
 ## -- Package : mlpro.bf.streams.streams
 ## -- Module  : clouds.py
 ## -------------------------------------------------------------------------------------------------
 ## -- History :
 ## -- yyyy-mm-dd  Ver.      Auth.    Description
-## -- 2023-08-29  0.0.0     SR       Creation
-## -- 2023-08-29  1.0.0     SR       First draft implementation
+## -- 2023-08-29  0.0.0     SK       Creation
+## -- 2023-08-29  1.0.0     SK       First draft implementation
 ## -- 2023-09-15  1.0.1     LSB      Bug Fix
 ## -- 2023-12-25  1.0.2     DA       Bugfix in StreamMLProClouds._get_next()
 ## -- 2023-12-26  1.0.3     DA       - Little refactoring of StreamMLProClouds._init_dataset()
 ## --                                - Bugfix in StreamMLProClouds._get_next()
 ## -- 2023-12-27  1.1.0     DA       Refactoring
 ## -- 2023-12-29  1.2.0     DA       Class StreamMLProClouds: new parameter p_weights
+## -- 2024-02-06  1.2.1     DA       Class StreamMLProClouds3D8C10000Dynamic: corrections on constants
+## -- 2024-02-09  1.2.2     DA       Completion of class documentations
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 1.2.0 (2023-12-29)
+Ver. 1.2.2 (2024-02-09)
 
 This module provides the native stream classes StreamMLProClouds, StreamMLProClouds2D4C1000Static,
 StreamMLProClouds3D8C2000Static, StreamMLProClouds2D4C5000Dynamic and StreamMLProClouds3D8C10000Dynamic.
 These stream provides instances with self.C_NUM_DIMENSIONS dimensional random feature data, placed around
 centers (can be defined by user) which may or maynot move over time.
 
 """
@@ -33,17 +35,19 @@
 
 
 
 ## -------------------------------------------------------------------------------------------------
 ## -------------------------------------------------------------------------------------------------
 class StreamMLProClouds (StreamMLProBase):
     """
-    This demo stream provides self.C_NUM_INSTANCES n-dimensional instances randomly positioned around
-    centers which may or may not move over time.
+    This benchmark stream class generates freely configurable random point clouds of any number, size
+    and dimensionality. Optionally, the centers of the clouds are static or in motion.
 
+    Parameters
+    ----------
     p_num_dim : int
         The number of dimensions or features of the data. Default = 3.
     p_num_instances : int
         Total number of instances. The value '0' means indefinite. Default = 1000.
     p_num_clouds : int
         Number of clouds. Default = 4.
     p_radii : list
@@ -222,16 +226,30 @@
 
 
 
 
 ## -------------------------------------------------------------------------------------------------
 ## -------------------------------------------------------------------------------------------------
 class StreamMLProClouds2D4C1000Static (StreamMLProClouds):
+    """
+    This benchmark stream generates 1000 2-dimensional instances that form 4 static random point clouds.
+
+    See also: class StreamMLProClouds
+
+    Parameters
+    ----------
+    p_radii : list
+        Radii of the clouds. Default = 20.
+    p_seed 
+        Seeding value for the random generator. Default = None (no seeding).
+    p_logging
+        Log level (see constants of class Log). Default: Log.C_LOG_ALL.
+    """
 
-    C_ID                    = 'StreamMLProClouds2D4C1000Static'
+    C_ID                    = 'Clouds2D4C1000Static'
     C_NAME                  = 'Static Clouds 2D'
     C_VERSION               = '1.0.1'
     C_NUM_DIMENSIONS        = 2
     C_NUM_INSTANCES         = 1000
     C_SCIREF_ABSTRACT       = 'Demo stream provides 1000 2D instances randomly positioned around four fixed centers.'
     C_BOUNDARIES            = [-100,100]
 
@@ -253,16 +271,30 @@
 
 
 
 
 ## -------------------------------------------------------------------------------------------------
 ## -------------------------------------------------------------------------------------------------
 class StreamMLProClouds3D8C2000Static (StreamMLProClouds):
+    """
+    This benchmark stream generates 2000 3-dimensional instances that form 8 static random point clouds.
 
-    C_ID                    = 'StreamMLProClouds3D8C2000Static'
+    See also: class StreamMLProClouds
+
+    Parameters
+    ----------
+    p_radii : list
+        Radii of the clouds. Default = 20.
+    p_seed 
+        Seeding value for the random generator. Default = None (no seeding).
+    p_logging
+        Log level (see constants of class Log). Default: Log.C_LOG_ALL.
+    """
+
+    C_ID                    = 'Clouds3D8C2000Static'
     C_NAME                  = 'Static Clouds 3D'
     C_VERSION               = '1.0.1'
     C_NUM_DIMENSIONS        = 3
     C_NUM_INSTANCES         = 2000
     C_SCIREF_ABSTRACT       = 'Demo stream provides 2000 3D instances randomly positioned around eight fixed centers.'
     C_BOUNDARIES            = [-100,100]
 
@@ -284,16 +316,30 @@
 
 
 
 
 ## -------------------------------------------------------------------------------------------------
 ## -------------------------------------------------------------------------------------------------
 class StreamMLProClouds2D4C5000Dynamic (StreamMLProClouds):
+    """
+    This benchmark stream generates 5000 2-dimensional instances that form 4 dynamic random point clouds.
+
+    See also: class StreamMLProClouds
 
-    C_ID                    = 'StreamMLProClouds2D4C5000Dynamic'
+    Parameters
+    ----------
+    p_radii : list
+        Radii of the clouds. Default = 100.
+    p_seed 
+        Seeding value for the random generator. Default = None (no seeding).
+    p_logging
+        Log level (see constants of class Log). Default: Log.C_LOG_ALL.
+    """
+
+    C_ID                    = 'Clouds2D4C5000Dynamic'
     C_NAME                  = 'Dynamic Clouds 2D'
     C_VERSION               = '1.0.1'
     C_NUM_DIMENSIONS        = 2
     C_NUM_INSTANCES         = 5000
     C_SCIREF_ABSTRACT       = 'Demo stream provides 2000 2D instances randomly positioned around four randomly moving centers.'
     C_BOUNDARIES            = [-1000,1000]
 
@@ -316,17 +362,31 @@
 
 
 
 
 ## -------------------------------------------------------------------------------------------------
 ## -------------------------------------------------------------------------------------------------
 class StreamMLProClouds3D8C10000Dynamic (StreamMLProClouds):
+    """
+    This benchmark stream generates 10000 3-dimensional instances that form 8 dynamic random point clouds.
 
-    C_ID                    = 'StreamMLProClouds3D8C10000Dynamic'
-    C_NAME                  = 'Static Clouds 2D'
+    See also: class StreamMLProClouds
+
+    Parameters
+    ----------
+    p_radii : list
+        Radii of the clouds. Default = 100.
+    p_seed 
+        Seeding value for the random generator. Default = None (no seeding).
+    p_logging
+        Log level (see constants of class Log). Default: Log.C_LOG_ALL.
+    """
+
+    C_ID                    = 'Clouds3D8C10000Dynamic'
+    C_NAME                  = 'Dynamic Clouds 3D'
     C_VERSION               = '1.0.1'
     C_NUM_DIMENSIONS        = 3
     C_NUM_INSTANCES         = 10000
     C_SCIREF_ABSTRACT       = 'Demo stream provides 10000 3D instances randomly positioned around eight randomly moving centers.'
     C_BOUNDARIES            = [-1000,1000]
 
 ## -------------------------------------------------------------------------------------------------
```

### Comparing `mlpro-1.3.1/src/mlpro/bf/streams/streams/clouds3d_static.py` & `mlpro-1.4.0/src/mlpro/bf/streams/streams/provider_mlpro.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,114 +1,143 @@
 ## -------------------------------------------------------------------------------------------------
 ## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
 ## -- Package : mlpro.bf.streams.streams
-## -- Module  : clouds23_static.py
+## -- Module  : provider_mlpro.py
 ## -------------------------------------------------------------------------------------------------
 ## -- History :
 ## -- yyyy-mm-dd  Ver.      Auth.    Description
-## -- 2022-12-15  0.0.0     DA       Creation 
-## -- 2022-12-15  1.0.0     DA       First draft implementation
-## -- 2023-05-02  1.0.1     DA       Removed boundaries from features
+## -- 2022-01-12  0.0.0     DA       Creation 
+## -- 2022-11-08  0.1.0     DA       First draft implementation
+## -- 2022-12-14  1.0.0     DA       First release
+## -- 2023-03-03  1.0.1     SY       Add p_kwargs in StreamProviderMLPro and StreamMLProBase
+## -- 2023-04-12  1.0.2     SY       Remove p_kwargs in StreamProviderMLPro
+## -- 2023-12-26  1.1.0     DA       StreamProviderMLPro.__init__(): recursive consideration of all 
+## --                                subclasses of class StreamMLProBase
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 1.0.1 (2023-05-02)
+Ver. 1.1.0 (2023-12-26)
+
+This module consists of a native stream provider and a template for builtin streams.
 
-This module provides the native stream class StreamMLProStaticClouds3D. This stream provides 2000 
-instances with 3-dimensional random feature data placed around eight fixed center points.
 """
 
-import numpy as np
-import math
+from mlpro.bf.various import Log, ScientificObject
+from mlpro.bf.ops import Mode
 from mlpro.bf.streams.models import *
-from mlpro.bf.streams.streams.provider_mlpro import StreamMLProBase
 
 
 
 
 ## -------------------------------------------------------------------------------------------------
 ## -------------------------------------------------------------------------------------------------
-class StreamMLProStaticClouds3D (StreamMLProBase):
+class StreamMLProBase (Stream): 
     """
-    This demo stream provides 2000 3-dimensional instances randomly positioned around four fixed centers.
+    Base class for MLPro's native data streams.
     """
 
-    C_ID                = 'StaticClouds3D'
-    C_NAME              = 'Static Clouds 3D'
-    C_VERSION           = '1.0.0'
-    C_NUM_INSTANCES     = 2000
-
-    C_SCIREF_ABSTRACT   = 'Demo stream provides 1000 2-dimensional instances randomly positioned around four fixed centers.'
-
-    C_BOUNDARIES        = [-10,10]
-
-## -------------------------------------------------------------------------------------------------
-    def _setup_feature_space(self) -> MSpace:
-        feature_space : MSpace = MSpace()
-
-        for i in range(3):
-            feature_space.add_dim( Feature( p_name_short = 'f' + str(i),
-                                            p_base_set = Feature.C_BASE_SET_R,
-                                            p_name_long = 'Feature #' + str(i),
-                                            p_name_latex = '',
-                                            # p_boundaries = self.C_BOUNDARIES,
-                                            p_description = '',
-                                            p_symmetrical = False,
-                                            p_logging=Log.C_LOG_NOTHING ) )
+    C_ID                = ''
+    C_NAME              = '????'
+    C_VERSION           = '0.0.0'
+    C_NUM_INSTANCES     = 0
+
+    C_SCIREF_TYPE       = ScientificObject.C_SCIREF_TYPE_ONLINE
+    C_SCIREF_AUTHOR     = 'MLPro'
+    C_SCIREF_URL        = 'https://mlpro.readthedocs.io'
 
-        return feature_space
+## -------------------------------------------------------------------------------------------------
+    def __init__( self, p_logging=Log.C_LOG_ALL, **p_kwargs ):
+
+        super().__init__( p_id = self.C_ID, 
+                          p_name = self.C_NAME, 
+                          p_num_instances = self.C_NUM_INSTANCES, 
+                          p_version = self.C_VERSION,
+                          p_feature_space = self._setup_feature_space(), 
+                          p_label_space = self._setup_label_space(), 
+                          p_mode=Mode.C_MODE_SIM,
+                          p_logging = p_logging,
+                          **p_kwargs )
+
+
+## -------------------------------------------------------------------------------------------------
+    def _reset(self):
+        self._index = 0
+        self._init_dataset()
 
 
 ## -------------------------------------------------------------------------------------------------
     def _init_dataset(self):
+        """
+        Custom method to generate stream data as a numpy array named self._dataset.
+        """
+
+        raise NotImplementedError
+
 
-        # 1 Preparation
-        try:
-            seed = self._random_seed
-        except:
-            self.set_random_seed()
-            seed = self._random_seed
-
-        self._dataset = np.empty( (self.C_NUM_INSTANCES, 3))
-
-
-        # 2 Create 4 fixed hotspots
-        dx1             = ( self.C_BOUNDARIES[1] - self.C_BOUNDARIES[0] ) / 4
-        x1_1            = self.C_BOUNDARIES[0] + dx1
-        x1_2            = self.C_BOUNDARIES[1] - dx1
-        
-        dx2             = ( self.C_BOUNDARIES[1] - self.C_BOUNDARIES[0] ) / 4
-        x2_1            = self.C_BOUNDARIES[0] + dx2
-        x2_2            = self.C_BOUNDARIES[1] - dx2
-        
-        dx3             = ( self.C_BOUNDARIES[1] - self.C_BOUNDARIES[0] ) / 4
-        x3_1            = self.C_BOUNDARIES[0] + dx3
-        x3_2            = self.C_BOUNDARIES[1] - dx3
-
-        hotspots        = [ [ x1_1, x2_1, x3_1 ], [ x1_2, x2_1, x3_1 ], 
-                            [ x1_1, x2_2, x3_1 ], [ x1_2, x2_2, x3_1 ], 
-                            [ x1_1, x2_1, x3_2 ], [ x1_2, x2_1, x3_2 ], 
-                            [ x1_1, x2_2, x3_2 ], [ x1_2, x2_2, x3_2 ] ]
-       
-        
-        # 2 Create 250 noisy inputs around each of the 4 fixed hotspots
-        a = np.random.RandomState(seed=seed).rand(self.C_NUM_INSTANCES, 3)**3
-        s = np.round(np.random.RandomState(seed=seed).rand(self.C_NUM_INSTANCES, 3))
-        s[s==0] = -1
-        fx1 = dx1 * 0.75
-        fx2 = dx2 * 0.75
-        fx3 = dx3 * 0.75
-        c = a*s * np.array([fx1, fx2, fx3]) 
-        
-        index  = 0
-        
-        for i in range(int(self.C_NUM_INSTANCES/ 8)):
-            for hsp in hotspots:
-                self._dataset[index][0] = hsp[0] + c[index][0]
-                self._dataset[index][1] = hsp[1] + c[index][1]
-                self._dataset[index][2] = hsp[2] + c[index][2]
-                index += 1
+## -------------------------------------------------------------------------------------------------
+    def _get_next(self) -> Instance:
+
+        if self._index == self.C_NUM_INSTANCES: raise StopIteration
+
+        feature_data = Element(self._feature_space)
+        feature_data.set_values(p_values=self._dataset[self._index])
+
+        self._index += 1
+
+        return Instance( p_feature_data=feature_data )
 
 
+
+
+
+## -------------------------------------------------------------------------------------------------
 ## -------------------------------------------------------------------------------------------------
-    def set_random_seed(self, p_seed=None):
-        self._random_seed = p_seed
+class StreamProviderMLPro (StreamProvider): 
+    """
+    MLPro's builtin provider class for native data streams.
+    """
+
+    C_NAME          = 'MLPro'
+
+    C_SCIREF_TYPE   = ScientificObject.C_SCIREF_TYPE_ONLINE
+    C_SCIREF_AUTHOR = 'MLPro'
+    C_SCIREF_URL    = 'https://mlpro.readthedocs.io'
+
+## -------------------------------------------------------------------------------------------------
+    def __init__(self, p_seed = None, p_logging=Log.C_LOG_ALL):
+        super().__init__(p_logging)
+
+        self._stream_list      = []
+        self._streams_by_id    = {}
+        self._streams_by_name  = {}
+
+        mlpro_stream_classes = StreamMLProBase.__subclasses__()
+        for cls in mlpro_stream_classes:
+            stream = cls(p_seed=p_seed, p_logging=p_logging)
+            self._stream_list.append(stream)
+            self._streams_by_id[stream.get_id()] = stream
+            self._streams_by_name[stream.get_name()] = stream
+            mlpro_stream_classes.extend(cls.__subclasses__())
+
+
+## -------------------------------------------------------------------------------------------------
+    def _get_stream_list(self, p_mode=Mode.C_MODE_SIM, p_logging=Log.C_LOG_ALL, **p_kwargs) -> list:
+        return self._stream_list
+
+
+## -------------------------------------------------------------------------------------------------
+    def _get_stream( self, 
+                     p_id: str = None, 
+                     p_name: str = None, 
+                     p_mode=Mode.C_MODE_SIM, 
+                     p_logging=Log.C_LOG_ALL, 
+                     **p_kwargs ) -> Stream:
+
+        if p_id is not None:
+            stream = self._streams_by_id[p_id]
+        else:
+            stream = self._streams_by_name[p_name]
+
+        stream.switch_logging(p_logging=p_logging)
+        stream.set_mode(p_mode=p_mode)
+        return stream
+
```

### Comparing `mlpro-1.3.1/src/mlpro/bf/streams/streams/csv_file.py` & `mlpro-1.4.0/src/mlpro/bf/streams/streams/csv_file.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/streams/streams/doublespiral2d.py` & `mlpro-1.4.0/src/mlpro/bf/streams/streams/doublespiral2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ## -------------------------------------------------------------------------------------------------
-## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
+## -- Project : MLPro - The integrative middleware framework for standardized machine learning
 ## -- Package : mlpro.bf.streams.streams
 ## -- Module  : doublespiral2d.py
 ## -------------------------------------------------------------------------------------------------
 ## -- History :
 ## -- yyyy-mm-dd  Ver.      Auth.    Description
 ## -- 2022-12-14  0.0.0     DA       Creation 
 ## -- 2022-12-14  1.0.0     DA       First implementation
```

### Comparing `mlpro-1.3.1/src/mlpro/bf/streams/streams/rnd10d.py` & `mlpro-1.4.0/src/mlpro/bf/streams/streams/rnd10d.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/streams/tasks/deriver.py` & `mlpro-1.4.0/src/mlpro/bf/streams/tasks/deriver.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/streams/tasks/rearranger.py` & `mlpro-1.4.0/src/mlpro/bf/streams/tasks/rearranger.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/streams/tasks/windows.py` & `mlpro-1.4.0/src/mlpro/bf/streams/tasks/windows.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/systems/basics.py` & `mlpro-1.4.0/src/mlpro/bf/systems/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/systems/pool/doublependulum.py` & `mlpro-1.4.0/src/mlpro/bf/systems/pool/doublependulum.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/systems/pool/flipflops.py` & `mlpro-1.4.0/src/mlpro/bf/systems/pool/flipflops.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Arrow.stl` & `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Arrow.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/X_letter.stl` & `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/X_letter.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Y_letter.stl` & `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Y_letter.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Z_letter.stl` & `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Z_letter.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/texture/logo.png` & `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/texture/logo.png`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/base.stl` & `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/base.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/forearm.stl` & `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/forearm.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/shoulder.stl` & `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/shoulder.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/upperarm.stl` & `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/upperarm.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist1.stl` & `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist1.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist2.stl` & `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist2.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist3.stl` & `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist3.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/boxontable.xml` & `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/boxontable.xml`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/cartpole.xml` & `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/cartpole.xml`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/doublependulum.xml` & `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/doublependulum.xml`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/mlpro.xml` & `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/mlpro.xml`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/pendulum.xml` & `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/pendulum.xml`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/systems/pool/mujoco/ur5.xml` & `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/ur5.xml`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/ui/sciui/framework.py` & `mlpro-1.4.0/src/mlpro/bf/ui/sciui/framework.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/ui/sciui/main.py` & `mlpro-1.4.0/src/mlpro/bf/ui/sciui/main.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/ui/sciui/pool/iis.py` & `mlpro-1.4.0/src/mlpro/bf/ui/sciui/pool/iis.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/ui/sciui/pool/iisbenchmark.py` & `mlpro-1.4.0/src/mlpro/bf/ui/sciui/pool/iisbenchmark.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/ui/sciui/templates/scenario_test.py` & `mlpro-1.4.0/src/mlpro/bf/ui/sciui/templates/scenario_test.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/bf/various.py` & `mlpro-1.4.0/src/mlpro/bf/various.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/gt/dynamicgames/basics.py` & `mlpro-1.4.0/src/mlpro/gt/dynamicgames/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/gt/dynamicgames/potential.py` & `mlpro-1.4.0/src/mlpro/gt/dynamicgames/potential.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/gt/dynamicgames/stackelberg.py` & `mlpro-1.4.0/src/mlpro/gt/dynamicgames/stackelberg.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/gt/native/basics.py` & `mlpro-1.4.0/src/mlpro/gt/native/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/gt/pool/boards/bglp.py` & `mlpro-1.4.0/src/mlpro/gt/pool/boards/bglp.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/gt/pool/native/games/prisonersdilemma_2p.py` & `mlpro-1.4.0/src/mlpro/gt/pool/native/games/prisonersdilemma_2p.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/gt/pool/native/games/prisonersdilemma_3p.py` & `mlpro-1.4.0/src/mlpro/gt/pool/native/games/prisonersdilemma_3p.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/gt/pool/native/games/rockpaperscissors.py` & `mlpro-1.4.0/src/mlpro/gt/pool/native/games/rockpaperscissors.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/gt/pool/native/games/routingproblems_3p.py` & `mlpro-1.4.0/src/mlpro/gt/pool/native/games/routingproblems_3p.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/gt/pool/native/games/supplydemand_3p.py` & `mlpro-1.4.0/src/mlpro/gt/pool/native/games/supplydemand_3p.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/gt/pool/native/solvers/greedypolicy.py` & `mlpro-1.4.0/src/mlpro/gt/pool/native/solvers/greedypolicy.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/gt/pool/native/solvers/randomsolver.py` & `mlpro-1.4.0/src/mlpro/gt/pool/native/solvers/randomsolver.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/oa/sciui/iis.py` & `mlpro-1.4.0/src/mlpro/oa/sciui/iis.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/oa/sciui/runme.py` & `mlpro-1.4.0/src/mlpro/oa/sciui/runme.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/oa/sciui/scenario_oa1.py` & `mlpro-1.4.0/src/mlpro/oa/sciui/scenario_oa1.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/oa/streams/basics.py` & `mlpro-1.4.0/src/mlpro/oa/streams/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/oa/streams/tasks/anomalydetectors.py` & `mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/basics.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,190 +1,212 @@
 ## -------------------------------------------------------------------------------------------------
-## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
-## -- Package : mlpro.oa.tasks.boundarydetectors
-## -- Module  : anomalydetectors.py
+## -- Project : MLPro - The integrative middleware framework for standardized machine learning
+## -- Package : mlpro.oa.tasks.anomalydetectors
+## -- Module  : basics.py
 ## -------------------------------------------------------------------------------------------------
 ## -- History :
 ## -- yyyy-mm-dd  Ver.      Auth.    Description
-## -- 2023-06-08  0.0.0     SP       Creation
-## -- 2023-                 SP       Release
+## -- 2023-06-08  0.0.0     SK       Creation
+## -- 2023-09-12  1.0.0     SK       Release
+## -- 2023-11-21  1.0.1     SK       Time Stamp update
+## -- 2024-02-25  1.1.0     SK       Visualisation update
+## -- 2024-04-10  1.2.0     DA/SK    Refactoring
+## -- 2024-04-11  1.3.0     DA       Methods AnomalyDetector.init/update_plot: determination and
+## --                                forwarding of changes on ax limits
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 1.0.0 (2023-06-23)
+Ver. 1.3.0 (2024-04-11)
+
 This module provides templates for anomaly detection to be used in the context of online adaptivity.
 """
 
-from mlpro.oa.streams.basics import *
-from mlpro.oa.streams.basics import Instance, List
-import numpy as np
+from typing import List
+from matplotlib.figure import Figure
+from mlpro.bf.plot import PlotSettings
+from mlpro.bf.various import Log
+from mlpro.bf.math.normalizers import Normalizer
+from mlpro.bf.streams import Instance
+from mlpro.oa.streams.tasks import OATask
+from mlpro.oa.streams.tasks.anomalydetectors.anomalies import Anomaly
+
 
 
 ## -------------------------------------------------------------------------------------------------
 ## -------------------------------------------------------------------------------------------------
 class AnomalyDetector(OATask):
     """
-    This is the base class for multivariate online anomaly detectors. It raises an event when an
+    This is the base class for online anomaly detectors. It raises an event when an
     anomaly is detected.
 
     """
 
-    C_NAME          = 'Anomaly Detector'
     C_TYPE          = 'Anomaly Detector'
-    C_EVENT_ANOMALY = 'ANOMALY'
 
-    ## -------------------------------------------------------------------------------------------------
+    C_PLOT_ACTIVE           = True
+    C_PLOT_STANDALONE       = False
+
+## -------------------------------------------------------------------------------------------------
     def __init__(self,
                  p_name:str = None,
-                 p_range_max = StreamTask.C_RANGE_THREAD,
+                 p_range_max = OATask.C_RANGE_THREAD,
                  p_ada : bool = True,
                  p_duplicate_data : bool = False,
                  p_visualize : bool = False,
                  p_logging=Log.C_LOG_ALL,
                  **p_kwargs):
 
         super().__init__(p_name = p_name,
                          p_range_max = p_range_max,
                          p_ada = p_ada,
                          p_duplicate_data = p_duplicate_data,
                          p_visualize = p_visualize,
                          p_logging = p_logging,
                          **p_kwargs)
         
-        self.data_points = []
-        self.counter = 0
-        self.anomaly_scores = []
+        self._ano_id = 0
+        self._anomalies = {}
+        self._ano_scores = []
 
 
-    ## ------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
     def _run(self, p_inst_new: list, p_inst_del: list):
         pass
 
 
+## -------------------------------------------------------------------------------------------------
+    def _get_next_anomaly_id(self):
+        self._ano_id +=1
+        return self._ano_id
 
-## -------------------------------------------------------------------------
-## -------------------------------------------------------------------------
-class AnomalyDetectorCB(AnomalyDetector):
-
-    C_TYPE = 'Cluster based Anomaly Detector'
-
-
-    ## ------------------------------------------------------------------------
-    def __init__(self,
-                 p_threshold = 5.0,
-                 p_centroid_threshold = 1.0,
-                 p_name:str = None,
-                 p_range_max = StreamTask.C_RANGE_THREAD,
-                 p_ada : bool = True,
-                 p_duplicate_data : bool = False,
-                 p_visualize : bool = False,
-                 p_logging=Log.C_LOG_ALL,
-                 **p_kwargs):
-
-        super().__init__(p_name = p_name,
-                         p_range_max = p_range_max,
-                         p_ada = p_ada,
-                         p_duplicate_data = p_duplicate_data,
-                         p_visualize = p_visualize,
-                         p_logging = p_logging,
-                         **p_kwargs)
-        
-        self.data_points = []
-        self.counter = 0
-        self.anomaly_scores = []
-        self.threshold = p_threshold
-        self.centroid_thre = p_centroid_threshold
-        self.centroids = []
-
-
-
-    ## -------------------------------------------------------------------------
-    def _run(self, p_inst_new: list, center: float, centroids: list):
-
-        anomaly = None
-        self.centroids.append(centroids)
-        
-        distance = np.linalg.norm(p_inst_new - center)
-        if distance > self.threshold:
-            anomaly = p_inst_new
 
-        if len(centroids) > 10:
-            self.centroids.pop(0)
-        
-        if len(self.centroids[-2]) != len(self.centroids[-1]):
-            anomaly = p_inst_new
+## -------------------------------------------------------------------------------------------------
+    def get_anomalies(self):
+        """
+        This method returns the current list of anomalies. 
+
+        Returns
+        -------
+        dict_of_anomalies : dict[Anomaly]
+            Current dictionary of anomalies.
+        """
 
-        differences = [abs(a - b) for a, b in zip(self.centroids[0], self.centroids[-1])]
-        if any(difference >= self.centroid_thre for difference in differences):
-            anomlay = p_inst_new
-
-        if anomaly != None:
-            self.counter += 1
-            event_obj = AnomalyEvent(p_raising_object=self, p_kwargs=self.data_points[-1]) 
-            handler = self.event_handler
-            self.register_event_handler(event_obj.C_NAME, handler)
-            self._raise_event(event_obj.C_NAME, event_obj)
+        return self._anomalies
     
 
+## -------------------------------------------------------------------------------------------------
+    def _buffer_anomaly(self, p_anomaly:Anomaly):
+        """
+        Method to be used to add a new anomaly. Please use as part of your algorithm.
+
+        Parameters
+        ----------
+        p_anomaly : Anomaly
+            Anomaly object to be added.
+        """
+
+        p_anomaly.set_id( p_id = self._get_next_anomaly_id() )
+        self._anomalies[p_anomaly.get_id()] = p_anomaly
+        return p_anomaly
 
-## -------------------------------------------------------------------------
-## -------------------------------------------------------------------------
-class AnomalyEvent (Event):
-
-    C_TYPE     = 'Event'
-
-    C_NAME     = 'Anomaly'
 
-    def __init__(self, p_raising_object, p_det_time : str, p_instance: str, **p_kwargs):
-        pass
+## -------------------------------------------------------------------------------------------------
+    def remove_anomaly(self, p_anomaly):
+        """
+        Method to remove an existing anomaly. Please use as part of your algorithm.
+
+        Parameters
+        ----------
+        p_anomaly : Anomaly
+            Anomaly object to be removed.
+        """
 
+        p_anomaly.remove_plot(p_refresh=True)
+        del self._anomalies[p_anomaly.get_id()]
 
 
-## -------------------------------------------------------------------------
-## -------------------------------------------------------------------------
-class PointAnomaly (AnomalyEvent):
+## -------------------------------------------------------------------------------------------------
+    def _raise_anomaly_event(self, p_anomaly : Anomaly ):
 
-    C_NAME      = 'Point Anomaly'
+        p_anomaly = self._buffer_anomaly(p_anomaly=p_anomaly)
 
-    def __init__(self, p_raising_object, p_det_time : str, p_instance : str, p_deviation : float, **p_kwargs):
-        pass
+        if self.get_visualization(): 
+            p_anomaly.init_plot( p_figure=self._figure, p_plot_settings=self.get_plot_settings() )
 
+        self._raise_event(p_anomaly.C_NAME, p_anomaly)
 
-## -------------------------------------------------------------------------
-## -------------------------------------------------------------------------
-class GroupAnomaly (AnomalyEvent):
+                 
+## -------------------------------------------------------------------------------------------------
+    def init_plot(self, p_figure: Figure = None, p_plot_settings: PlotSettings = None):
 
-    C_NAME      = 'Group Anomaly'
+        if not self.get_visualization(): return
 
-    def __init__(self, p_raising_object, p_det_time : str, p_instances : list, p_mean : float, p_mean_deviation : float, **p_kwargs):
-        pass
+        self._plot_ax_xlim = None
+        self._plot_ax_ylim = None
+        self._plot_ax_zlim = None
 
+        super().init_plot( p_figure=p_figure, p_plot_settings=p_plot_settings)
 
-## -------------------------------------------------------------------------
-## -------------------------------------------------------------------------
-class ContextualAnomaly (AnomalyEvent):
+        for anomaly in self._anomalies.values():
+            anomaly.init_plot(p_figure=p_figure, p_plot_settings = p_plot_settings)
+    
 
-    C_NAME      = 'Contextual Anomaly'
+## -------------------------------------------------------------------------------------------------
+    def update_plot(self, p_inst_new: List[Instance] = None, p_inst_del: List[Instance] = None, **p_kwargs):
+    
+        if not self.get_visualization(): return
 
-    def __init__(self, p_raising_object, p_det_time :str, p_instance: str,  **p_kwargs):
-        pass
+        super().update_plot(p_inst_new, p_inst_del, **p_kwargs)
 
+        axes = self._plot_settings.axes
 
-## -------------------------------------------------------------------------
-## -------------------------------------------------------------------------
-class DriftEvent (AnomalyEvent):
+        ax_xlim_new = axes.get_xlim()
+        if self._plot_settings.view != PlotSettings.C_VIEW_ND:
+            axlimits_changed = ( self._plot_ax_xlim is None ) or ( self._plot_ax_xlim != ax_xlim_new )
+        else:
+            axlimits_changed = False
+
+        ax_ylim_new = axes.get_ylim()
+        axlimits_changed = axlimits_changed or ( self._plot_ax_ylim is None ) or ( self._plot_ax_ylim != ax_ylim_new )
+        try:
+            ax_zlim_new = axes.get_zlim()
+            axlimits_changed = axlimits_changed or ( self._plot_ax_zlim is None ) or ( self._plot_ax_zlim != ax_zlim_new )
+        except:
+            ax_zlim_new = None
+        
+        self._plot_ax_xlim = ax_xlim_new
+        self._plot_ax_ylim = ax_ylim_new
+        self._plot_ax_zlim = ax_zlim_new
+
+        for anomaly in self._anomalies.values():
+            anomaly.update_plot( p_axlimits_changed = axlimits_changed,
+                                 p_xlim = ax_xlim_new,
+                                 p_ylim = ax_ylim_new,
+                                 p_zlim = ax_zlim_new,
+                                 **p_kwargs )
+    
 
-    C_NAME      = 'Drift'
+## -------------------------------------------------------------------------------------------------
+    def remove_plot(self, p_refresh: bool = True):
 
-    def __init__(self, p_raising_object, p_det_time : str, p_magnitude : float, p_rate : float, **p_kwargs):
-        pass
+        if not self.get_visualization(): return
 
+        super().remove_plot(p_refresh=p_refresh)
 
-## -------------------------------------------------------------------------
-## -------------------------------------------------------------------------
-class DriftEventCB (DriftEvent):
+        for anomaly in self._anomalies.values():
+            anomaly.remove_plot(p_refresh=p_refresh)
 
-    C_NAME      = 'Cluster based Drift'
 
-    def __init__(self, p_raising_object, p_det_time : str, **p_kwargs):
-        pass
+## -------------------------------------------------------------------------------------------------
+    def _renormalize(self, p_normalizer: Normalizer):
+        """
+        Internal renormalization of all anomaly instances. See method OATask.renormalize_on_event() for further
+        information.
+
+        Parameters
+        ----------
+        p_normalizer : Normalizer
+            Normalizer object to be applied on task-specific 
+        """
 
+        for anomaly in self._anomalies.values():
+            anomaly.get_instance().renormalize( p_normalizer=p_normalizer)
```

### Comparing `mlpro-1.3.1/src/mlpro/oa/streams/tasks/boundarydetectors.py` & `mlpro-1.4.0/src/mlpro/oa/streams/tasks/boundarydetectors.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/oa/streams/tasks/normalizers.py` & `mlpro-1.4.0/src/mlpro/oa/streams/tasks/normalizers.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/oa/systems/basics.py` & `mlpro-1.4.0/src/mlpro/oa/systems/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/oa/systems/pool/doublependulum.py` & `mlpro-1.4.0/src/mlpro/oa/systems/pool/doublependulum.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/rl/models.py` & `mlpro-1.4.0/src/mlpro/rl/models.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/rl/models_agents.py` & `mlpro-1.4.0/src/mlpro/rl/models_agents.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/rl/models_env.py` & `mlpro-1.4.0/src/mlpro/rl/models_env.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/rl/models_env_ada.py` & `mlpro-1.4.0/src/mlpro/rl/models_env_ada.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/rl/models_env_oa.py` & `mlpro-1.4.0/src/mlpro/rl/models_env_oa.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/rl/models_train.py` & `mlpro-1.4.0/src/mlpro/rl/models_train.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/rl/pool/actionplanner/mpc.py` & `mlpro-1.4.0/src/mlpro/rl/pool/actionplanner/mpc.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/rl/pool/envs/bglp.py` & `mlpro-1.4.0/src/mlpro/rl/pool/envs/bglp.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/rl/pool/envs/cartpole.py` & `mlpro-1.4.0/src/mlpro/rl/pool/envs/cartpole.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/rl/pool/envs/doublependulum.py` & `mlpro-1.4.0/src/mlpro/rl/pool/envs/doublependulum.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/rl/pool/envs/gridworld.py` & `mlpro-1.4.0/src/mlpro/rl/pool/envs/gridworld.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/rl/pool/envs/multicartpole.py` & `mlpro-1.4.0/src/mlpro/sl/basics.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,298 +1,369 @@
 ## -------------------------------------------------------------------------------------------------
 ## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
-## -- Package : mlpro.rl.pool.envs
-## -- Module  : multicartpole.py
+## -- Package : mlpro.sl
+## -- Module  : basics.py
 ## -------------------------------------------------------------------------------------------------
 ## -- History :
 ## -- yyyy-mm-dd  Ver.      Auth.    Description
-## -- 2021-06-05  0.0.0     DA       Creation
-## -- 2021-06-06  1.0.0     DA       Released first version
-## -- 2021-08-28  1.1.0     DA       Adjustments after changes on rl models
-## -- 2021-09-11  1.1.0     MRD      Change Header information to match our new library name
-## -- 2021-09-29  1.1.1     SY       Change name: WrEnvGym to WrEnvGYM2MLPro
-## -- 2021-10-05  1.1.2     SY       Update following new attributes done and broken in State
-## -- 2021-11-15  1.2.0     DA       Refactoring
-## -- 2021-12-03  1.2.1     DA       Refactoring
-## -- 2021-12-12  1.2.2     DA       Method MutliCartPole.get_cycle_limit() implemented
-## -- 2021-12-19  1.2.3     DA       Replaced 'done' by 'success'
-## -- 2021-12-21  1.2.4     DA       Class MultiCartPole: renamed method reset() to _reset()
-## -- 2022-02-25  1.2.5     SY       Refactoring due to auto generated ID in class Dimension
-## -- 2022-04-06  1.2.6     LSB      Freezing single environment after done returns true
-## -- 2022-07-20  1.2.7     SY       Update due to the latest introduction of Gym 0.25
-## -- 2022-11-07  1.3.0     DA       Class MultiCartPole: new parameter p_visualize
-## -- 2022-11-29  1.3.1     DA       Refactoring
-## -- 2023-01-14  1.3.2     MRD      Removing default parameter new_step_api and render_mode for gym
-## -- 2023-02-22  1.3.3     DA       Refactoring
-## -- 2023-04-19  1.3.4     MRD      Refactor module import gym to gymnasium
+## -- 2021-12-08  0.0.0     DA       Creation 
+## -- 2021-12-10  0.1.0     DA       Took over class AdaptiveFunction from bf.ml
+## -- 2022-08-15  0.1.1     SY       Renaming maturity to accuracy
+## -- 2022-11-02  0.2.0     DA       Refactoring: methods adapt(), _adapt()
+## -- 2022-11-15  0.3.0     DA       Class SLAdaptiveFunction: new parent class AdaptiveFunction
+## -- 2023-02-21  0.4.0     SY       - Introduce Class SLNetwork
+## --                                - Update Class SLAdaptiveFunction
+## -- 2023-02-22  0.4.1     SY       Update Class SLAdaptiveFunction
+## -- 2023-03-01  0.4.2     SY       - Renaming module
+## --                                - Remove SLNetwork
+## -- 2023-03-10  0.4.3     DA       Class SLAdaptiveFunction: refactoring of constructor parameters
+## -- 2023-06-20  0.4.4     LSB      Moved the quality check to the adapt online method
+## -- 2023-06-20  0.5.0     LSB      New methods: adapt_offline and adapt_online
+## -- 2023-07-24  0.5.1     LSB      Merged the new methods back to _adapt method
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 1.3.4 (2023-04-19)
+Ver. 0.5.1 (2023-06-24)
 
-This module provides an environment with multivariate state and action spaces based on the 
-OpenAI Gym environment 'CartPole-v1'. 
+This module provides model classes for supervised learning tasks. 
 """
 
 
-from mlpro.rl.models import *
-from mlpro.wrappers.gymnasium import WrEnvGYM2MLPro
-import numpy as np
-import gymnasium as gym
+
+from mlpro.bf.ml import *
+from mlpro.sl.models_eval import Metric
+from typing import List
 
 
 
 
 
 ## -------------------------------------------------------------------------------------------------
 ## -------------------------------------------------------------------------------------------------
-class MultiCartPole (Environment):
+class SLAdaptiveFunction (AdaptiveFunction):
     """
-    This environment multivariate space and action spaces by duplicating the
-    OpenAI Gym environment 'CartPole-v1'. The number of internal CartPole
-    sub-enironments can be parameterized.
+    Template class for an adaptive bi-multivariate mathematical function that adapts by supervised
+    learning.
+
+    Parameters
+    ----------
+    p_input_space : MSpace
+        Input space of function
+    p_output_space : MSpace
+        Output space of function
+    p_output_elem_cls 
+        Output element class (compatible to/inherited from class Element)
+    p_threshold : float
+        Threshold for the difference between a setpoint and a computed output. Computed outputs with 
+        a difference less than this threshold will be assessed as 'good' outputs. Default = 0.
+    p_ada : bool
+        Boolean switch for adaptivitiy. Default = True.
+    p_buffer_size : int
+        Initial size of internal data buffer. Defaut = 0 (no buffering).
+    p_name : str
+        Optional name of the model. Default is None.
+    p_range_max : int
+        Maximum range of asynchonicity. See class Range. Default is Range.C_RANGE_PROCESS.
+    p_autorun : int
+        On value C_AUTORUN_RUN method run() is called imediately during instantiation.
+        On vaule C_AUTORUN_LOOP method run_loop() is called.
+        Value C_AUTORUN_NONE (default) causes an object instantiation without starting further
+        actions.    
+    p_class_shared
+        Optional class for a shared object (class Shared or a child class of it)
+    p_visualize : bool
+        Boolean switch for visualisation. Default = False.
+    p_logging
+        Log level (see constants of class Log). Default: Log.C_LOG_ALL
+    p_par : Dict
+        Further model specific hyperparameters (to be defined in chhild class).
     """
 
-    C_NAME          = 'MultiCartPole'
-    C_LATENCY       = timedelta(0,1,0)
-    C_INFINITY      = np.finfo(np.float32).max     
+    C_TYPE = 'Adaptive Function (SL)'
+    C_NAME = '????'
 
-    C_PLOT_ACTIVE   = True 
 
 ## -------------------------------------------------------------------------------------------------
-    def __init__(self, 
-                 p_num_envs=2,                          # Number of internal sub-environments
-                 p_reward_type=Reward.C_TYPE_OVERALL,   # Reward type to be computed
-                 p_visualize:bool=True,
-                 p_logging=Log.C_LOG_ALL):              # Log level (see constants of class Log)
-
-        self._envs           = []
-        self._num_envs       = p_num_envs
-        self._reward_type    = p_reward_type
-        super().__init__(p_mode=Mode.C_MODE_SIM, p_visualize=p_visualize, p_logging=p_logging)
-        self._state_space, self._action_space = self._setup_spaces()
-
-        self._init_cartpoles()
+    def __init__( self,
+                  p_input_space : MSpace,
+                  p_output_space : MSpace,
+                  p_output_elem_cls=Element,
+                  p_threshold=0,
+                  p_ada : bool = True,
+                  p_buffer_size : int = 0,
+                  p_metrics : List[Metric] = [],
+                  p_score_metric = None,
+                  p_name: str = None,
+                  p_range_max: int = Async.C_RANGE_PROCESS,
+                  p_autorun = Task.C_AUTORUN_NONE,
+                  p_class_shared=None,
+                  p_visualize: bool = False, 
+                  p_logging=Log.C_LOG_ALL,
+                  **p_par ):
+
+        super().__init__( p_input_space = p_input_space,
+                          p_output_space = p_output_space,
+                          p_output_elem_cls = p_output_elem_cls,
+                          p_ada = p_ada,
+                          p_buffer_size = p_buffer_size,
+                          p_name = p_name,
+                          p_range_max = p_range_max,
+                          p_autorun = p_autorun,
+                          p_class_shared = p_class_shared,
+                          p_visualize = p_visualize,
+                          p_logging = p_logging,
+                          **p_par )                  
+
+        self._threshold      = p_threshold
+        self._mappings_total = 0  # Number of mappings since last adaptation
+        self._mappings_good  = 0  # Number of 'good' mappings since last adaptation
+        self._metrics        = p_metrics
+
+        self._score_metric   = p_score_metric or p_metrics[0] if len(p_metrics) != 0 else None
+        if (self._score_metric is not None) and (self._score_metric not in self._metrics):
+            self._metrics.insert(0, self._score_metric)
+
+        # self.metric_variables = []
+        self._metric_space = ESpace()
+
+        for metric in self._metrics:
+            dims = metric.get_output_space().get_dims()
+            for dim in dims:
+                self._metric_space.add_dim(dim.copy())
+
+        self._metric_values = Element(self._metric_space)
+
+        self._sl_model       = self._setup_model()
+        self._logging_set    = self._setup_logging_set()
 
 
 ## -------------------------------------------------------------------------------------------------
-    def _init_cartpoles(self):
-        for i in range(self._num_envs): 
-            state_space_id   = self._state_space.get_dim_ids()
-            action_space_id  = self._action_space.get_dim_ids()
-            state_space_env  = self._state_space.spawn([state_space_id[i*4], state_space_id[i*4+1], state_space_id[i*4+2], state_space_id[i*4+3]])
-            action_space_env = self._action_space.spawn([action_space_id[i]])
-            if self.get_visualization():
-                env_make     = gym.make('CartPole-v1', render_mode="human")
-            else:
-                env_make     = gym.make('CartPole-v1')
-            env              = WrEnvGYM2MLPro(env_make, state_space_env, action_space_env, p_visualize=self.get_visualization(), p_logging=self.get_log_level())
-            env.C_NAME = env.C_NAME + ' (' + str(i) + ')'
-            self._envs.append(env)
+    def _setup_model(self):
+        """
+        A method to set up a supervised learning network.
+        Please redefine this method according to the type of network, if not provided yet.
         
-        self.reset()
+        Returns
+        ----------
+            A set up supervised learning model
+        """
+
+        raise NotImplementedError
 
 
 ## -------------------------------------------------------------------------------------------------
-    @staticmethod
-    def load(p_path, p_filename):
-        mcp = Persistent.load(p_path, p_filename)
-        mcp._init_cartpoles()
-        return mcp
+    def get_input_space(self):
+        return self._input_space
 
 
 ## -------------------------------------------------------------------------------------------------
-    def _save(self, p_path, p_filename) -> bool:
-        self._envs.clear()
+    def get_output_space(self):
+        return self._output_space
 
-        pkl.dump( obj=self, 
-                  file=open(p_path + os.sep + p_filename, "wb"),
-                  protocol=pkl.HIGHEST_PROTOCOL )
 
-        self._init_cartpoles()
-        return True
+## -------------------------------------------------------------------------------------------------
+    def _setup_logging_set(self) -> Set :
+
+        return Set()
 
 
 ## -------------------------------------------------------------------------------------------------
-    def switch_logging(self, p_logging):
-        super().switch_logging(p_logging)
-        for env in self._envs: env.switch_logging(p_logging)
+    def get_logging_set(self) -> Set:
+
+        return self._logging_set
 
 
 ## -------------------------------------------------------------------------------------------------
-    @staticmethod
-    def setup_spaces():
-        return None, None
+    def get_logging_data(self) -> list :
+
+        return []
 
 
 ## -------------------------------------------------------------------------------------------------
-    def _setup_spaces(self):
-        state_space = ESpace()
-        action_space = ESpace()
+    def get_model(self):
+        """
+        A method to get the supervised learning network.
+        
+        Returns
+        ----------
+            A set up supervised learning model
+        """
 
-        for i in range(self._num_envs):
-            # Add a set of state dimensions for each sub-environment
-            env_str = str(i)
-            state_space.add_dim(Dimension( p_name_short='E-' + env_str + ' CPos', p_name_long='Env-' + env_str + ' Cart Position', p_unit='m', p_boundaries=[-4.8, 4.8]))
-            state_space.add_dim(Dimension( p_name_short='E-' + env_str + ' CVel', p_name_long='Env-' + env_str + ' Cart Velocity', p_unit='m/sec', p_unit_latex='\frac{m}{sec}', p_boundaries=[-self.C_INFINITY,self.C_INFINITY]))
-            state_space.add_dim(Dimension( p_name_short='E-' + env_str + ' PAng', p_name_long='Env-' + env_str + ' Pole Angle', p_unit='rad', p_boundaries=[-0.418, 0.418]))
-            state_space.add_dim(Dimension( p_name_short='E-' + env_str + ' PAVel', p_name_long='Env-' + env_str + ' Pole Angular Velocity', p_unit='rad/sec', p_unit_latex='\frac{rad}{sec}',p_boundaries=[-self.C_INFINITY,self.C_INFINITY]))
-            
-            # Add an action dimension for each sub-environment
-            action_space.add_dim(Dimension( p_name_short='E-' + env_str + ' Push', p_name_long='Env-' + env_str + ' Push Cart Left/Right', p_boundaries=[0,1]))
+        return self._sl_model
 
-        return state_space, action_space
 
-    
 ## -------------------------------------------------------------------------------------------------
-    def collect_substates(self) -> State:
-        state = State(self._state_space)
+    def adapt(self, p_input:Element=None, p_output:Element=None, p_dataset=None) -> bool:
+        """
+        Adaption by supervised learning.
+        
+        Parameters
+        ----------
+        p_input : Element
+            Abscissa/input element object (type Element)
+        p_output : Element
+            Setpoint ordinate/output element (type Element)
+        p_dataset
+            A set of data for offline learning
+        """
+
+        # if self._adaptivity:
+        #     self._set_adapted(self._adapt(p_input, p_output, p_dataset))
+        # else:
+        #     self._set_adapted(False)
+        adapted = Model.adapt(self, p_input=p_input, p_output = p_output, p_dataset=p_dataset)
+
+
+        return adapted
+
+
+## -------------------------------------------------------------------------------------------------
+    def _adapt(self, p_input:Element, p_output:Element, p_dataset:Buffer) -> bool:
+        """
+        Adaptation algorithm that is called by public adaptation method. This covers online and
+        offline supervised learning. Online learning means that the data set is dynamic according to
+        the input data, meanwhile offline learning means that the learning procedure is based on a
+        static data set.
+
+        Parameters
+        ----------
+        p_input : Element
+            Abscissa/input element object (type Element) for online learning
+        p_output : Element
+            Setpoint ordinate/output element (type Element) for online learning
+        p_dataset : Buffer
+            A set of data for offline learning
+
+        Returns
+        ----------
+            bool
+        """
+
+        if ( p_input is not None ) and ( p_output is not None ):
+            if not self._adaptivity:
+                return False
+
+            self.log(self.C_LOG_TYPE_I, 'Adaptation started')
+
+            adapted = False
+
+            if self._output_space.distance(p_output, self.map(p_input)) <= self._threshold:
+                # Quality of function ok. No need to adapt.
+                self._mappings_total += 1
+                self._mappings_good += 1
+
+            elif (p_input is not None) and (p_output is not None):
+                adapted = self._adapt_online(p_input, p_output)
+
+            if adapted:
+                self._mappings_total = 1
+
+                # Second quality check after adaptation
+                if self._output_space.distance(p_output, self.map(p_input)) <= self._threshold:
+                    self._mappings_good = 1
+                else:
+                    self._mappings_good = 0
 
-        success  = True
-        broken   = False
-        timeout  = False
-        terminal = True
+            else:
+                self._mappings_total += 1
+
+        else:
+            adapted = False
 
-        for env_id, env in enumerate(self._envs):
-            sub_state_val = env.get_state().get_values()
-            sub_state_dim = sub_state_val.shape[0]
-            for d in range(sub_state_dim):
-                state_ids = state.get_dim_ids()
-                state.set_value(state_ids[env_id*sub_state_dim + d], sub_state_val[d])
+            self.log(self.C_LOG_TYPE_I, 'Adaptation started')
 
-            success = success and env.get_state().get_success()
-            broken = broken or env.get_state().get_broken()
-            timeout = timeout or env.get_state().get_timeout()
-            terminal = terminal and env.get_state().get_terminal()
+            if self._adaptivity:
+                adapted = self._adapt_offline(p_dataset)
 
-        state.set_terminal(terminal)
-        state.set_success(success)
-        state.set_broken(broken)
-        state.set_timeout(timeout)
+            return adapted
 
-        return state
+        return adapted
 
 
 ## -------------------------------------------------------------------------------------------------
-    def get_cycle_limit(self):
-        return self._envs[0].get_cycle_limit()
+    def _adapt_online(self, p_input:Element, p_output:Element) -> bool:
+        """
+        Custom adaptation algorithm for online learning. Please redefine.
 
+        Parameters
+        ----------
+        p_input : Element
+            Abscissa/input element object (type Element)
+        p_output : Element
+            Setpoint ordinate/output element (type Element)
 
-## -------------------------------------------------------------------------------------------------
-    def _reset(self, p_seed=None):
-        seed = p_seed
+        Returns
+        ----------
+            bool
+        """
 
-        for env in self._envs: 
-            env.reset(seed)
-            if seed is not None:
-                seed += 1
+        raise NotImplementedError
 
-        self._set_state( self.collect_substates() )
-  
 
 ## -------------------------------------------------------------------------------------------------
-    def simulate_reaction(self, p_state:State, p_action:Action) -> State:
-        success = True
-        # frozen_envs = 0
+    def _adapt_offline(self, p_dataset:Buffer) -> bool:
+        """
+        Custom adaptation algorithm for offline learning. Please redefine.
 
-        for agent_id in p_action.get_agent_ids():
-            action_elem = p_action.get_elem(agent_id)
-            
-            try:
-                self.env_idx
-            except:
-                self.env_idx = 0    
-            
-            for action_id in action_elem.get_dim_ids():
-                env             = self._envs[self.env_idx]
+        Parameters
+        ----------
+        p_dataset : Buffer
+            A set of data for offline learning
 
-                # check for terminal state and skip the action simulation for this env
-                if env.get_state().get_terminal():
-                    # frozen_envs =+ 1
-                    if self.env_idx == len(self._envs) - 1:
-                        self.env_idx = 0
-                    else:
-                        self.env_idx += 1
-                    # if frozen_envs == len(self._envs): return self.collect_substates()
-                    continue
+        Returns
+        ----------
+            bool
+        """
 
+        raise NotImplementedError
 
-                action_elem_env = ActionElement(env.get_action_space())
-                action_elem_env.set_value(action_id, action_elem.get_value(action_id))
-                action_env      = Action()
-                action_env.add_elem(agent_id, action_elem_env)
-                env._set_state(env.simulate_reaction(None, action_env))
 
+## -------------------------------------------------------------------------------------------------
+    def get_accuracy(self):
+        """
+        Returns the accuracy of the adaptive function. The accuracy is defined as the relation 
+        between the number of successful mapped inputs and the total number of mappings since the 
+        last adaptation.
+        """
 
-                if env.get_state().get_terminal():
-                    self.log(self.C_LOG_TYPE_W, "Environment "+str(self.env_idx)+" is frozen after "+str(self._num_cycles)+" cycles")
+        if self._mappings_total == 0:
+            return 0
+        return self._mappings_good / self._mappings_total
 
 
-                if self.env_idx == len(self._envs)-1:
-                    self.env_idx = 0
-                else:
-                    self.env_idx += 1
+## -------------------------------------------------------------------------------------------------
+    def get_metrics(self) -> list:
 
-        return self.collect_substates()
+        return self._metrics
 
 
 ## -------------------------------------------------------------------------------------------------
-    def _compute_reward(self, p_state_old:State, p_state_new:State) -> Reward:
-        reward = Reward(self._reward_type)
+    def get_score_metric(self):
 
-        if self._reward_type == Reward.C_TYPE_OVERALL:
-            r_overall = 0
-            for env in self._envs: 
-                r_overall = r_overall + env.compute_reward().get_overall_reward()
-            r_overall = r_overall / len(self._envs)
-            reward.set_overall_reward(r_overall)
+        return self._score_metric
 
-        else:
-           for agent_id in self._last_action.get_agent_ids():
-                agent_action_elem = self._last_action.get_elem(agent_id)
-                agent_action_ids  = agent_action_elem.get_dim_ids()
-                r_agent = 0
-                
-                try:
-                    self.env_idx_reward
-                except:
-                    self.env_idx_reward = 0
-                    
-                for action_id in agent_action_ids:
-                    r_action = self._envs[self.env_idx_reward].compute_reward().get_overall_reward()
-                    if self._reward_type == Reward.C_TYPE_EVERY_ACTION:
-                        reward.add_action_reward(agent_id, action_id, r_action)
-                    elif self._reward_type == Reward.C_TYPE_EVERY_AGENT:
-                        r_agent = r_agent + r_action
-                
-                if self._reward_type == Reward.C_TYPE_EVERY_AGENT:
-                    r_agent = r_agent / len(agent_action_ids)
-                    reward.add_agent_reward(agent_id, r_agent)
-                
-                if self.env_idx_reward == len(self._envs)-1:
-                    self.env_idx_reward = 0
-                else:
-                    self.env_idx_reward += 1
 
-        return reward
+## -------------------------------------------------------------------------------------------------
+    def get_metric_space(self) -> ESpace:
+
+        return self._metric_space
 
 
 ## -------------------------------------------------------------------------------------------------
-    def compute_success(self, p_state:State) -> bool:
-        return self.get_success()
+    def calculate_metrics(self, p_data) -> Element:
 
+        val = []
+        for metric in self._metrics:
+            val.append(metric.compute(self, p_data))
 
-## -------------------------------------------------------------------------------------------------
-    def compute_broken(self, p_state:State) -> bool:
-        return self.get_broken()
+        self._metric_values = Element(self._metric_space)
+        self._metric_values.set_values(val)
+        return self._metric_values
 
 
 ## -------------------------------------------------------------------------------------------------
-    def init_plot(self, p_figure: Figure = None, p_plot_settings: list = ..., p_plot_depth: int = 0, p_detail_level: int = 0, p_step_rate: int = 0, **p_kwargs):
-        for env in self._envs: env.init_plot(p_figure=None)
+    def get_current_metrics(self):
+        return self._metric_values
 
 
-## -------------------------------------------------------------------------------------------------
-    def update_plot(self, **p_kwargs):
-        for env in self._envs: env.update_plot( **p_kwargs )
```

### Comparing `mlpro-1.3.1/src/mlpro/rl/pool/envs/robotinhtm.py` & `mlpro-1.4.0/src/mlpro/rl/pool/envs/robotinhtm.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/rl/pool/policies/dummy.py` & `mlpro-1.4.0/src/mlpro/rl/pool/policies/dummy.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/rl/pool/policies/randomgenerator.py` & `mlpro-1.4.0/src/mlpro/rl/pool/policies/randomgenerator.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/rl/pool/sarsbuffer/PrioritizedBuffer.py` & `mlpro-1.4.0/src/mlpro/rl/pool/sarsbuffer/PrioritizedBuffer.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/rl/pool/sarsbuffer/RandomSARSBuffer.py` & `mlpro-1.4.0/src/mlpro/rl/pool/sarsbuffer/RandomSARSBuffer.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/rl/sciui_rl.py` & `mlpro-1.4.0/src/mlpro/rl/sciui_rl.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/sl/examples/howto_sl_afct_100_train_and_reload_pytorch_mlp.py` & `mlpro-1.4.0/src/mlpro/sl/examples/howto_sl_afct_100_train_and_reload_pytorch_mlp.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/sl/fnn.py` & `mlpro-1.4.0/src/mlpro/sl/fnn.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/sl/models_eval.py` & `mlpro-1.4.0/src/mlpro/sl/models_eval.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/sl/models_train.py` & `mlpro-1.4.0/src/mlpro/sl/models_train.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/sl/pool/afct/fnn/pytorch/mlp.py` & `mlpro-1.4.0/src/mlpro/sl/pool/afct/fnn/pytorch/mlp.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/sl/pool/afct/pytorch.py` & `mlpro-1.4.0/src/mlpro/sl/pool/afct/pytorch.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.3.1/src/mlpro/wrappers/models.py` & `mlpro-1.4.0/src/mlpro/wrappers/basics.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ## -------------------------------------------------------------------------------------------------
-## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
+## -- Project : MLPro - The integrative middleware framework for standardized machine learning
 ## -- Package : mlpro.wrappers
-## -- Module  : models
+## -- Module  : basics.py
 ## -------------------------------------------------------------------------------------------------
 ## -- History :
 ## -- yyyy-mm-dd  Ver.      Auth.    Description
 ## -- 2021-04-16  0.0.0     DA       Creation
 ## -- 2021-05-29  1.0.0     DA       Release of first version
 ## -- 2021-06-16  1.1.0     SY       Adding the first version of data storing,
 ## --                                data plotting, and data saving classes
@@ -35,18 +35,15 @@
 
 """
 Ver. 1.8.1 (2023-01-14)
 
 This module provides model classes for wrappers in the MLPro project.
 """
 
-# from datetime import datetime, timedelta
-# from time import sleep
-# import dill as pkl
-# import os
+
 from mlpro.bf.exceptions import *
 from mlpro.bf.various import Log
 
 
 
 
 ## -------------------------------------------------------------------------------------------------
```

### Comparing `mlpro-1.3.1/src/mlpro/wrappers/mujoco.py` & `mlpro-1.4.0/src/mlpro/wrappers/mujoco.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ## -------------------------------------------------------------------------------------------------
-## -- Project : FH-SWF Automation Technology - Common Code Base (CCB)
-## -- Package : mlpro
+## -- Project : MLPro - The integrative middleware framework for standardized machine learning
+## -- Package : mlpro.wrappers
 ## -- Module  : mujoco.py
 ## -------------------------------------------------------------------------------------------------
 ## -- History :
 ## -- yyyy-mm-dd  Ver.      Auth.    Description
 ## -- 2022-09-17  0.0.0     MRD       Creation
 ## -- 2022-12-11  0.0.1     MRD       Refactor due to new bf.Systems
 ## -- 2022-12-11  1.0.0     MRD       First Release
@@ -26,33 +26,34 @@
 ## -- 2023-03-08  1.2.3     MRD       Add get_latency() function to get latency from xml
 ## -- 2023-04-09  1.2.4     MRD       Add Offscreen Render and Camera functionality for Image 
 ## --                                 Processing
 ## -- 2023-04-09  1.2.5     MRD       New ESpace for initial states of MuJoCo for easy access to the
 ## --                                 value by its dimnesion short name. Add docstring.
 ## -- 2023-04-14  1.2.6     MRD       Add camera fovy to the state
 ## -- 2023-04-14  1.2.7     MRD       Add depth data to the state, simplify _get_camera_data
+## -- 2024-04-10  1.2.8     DA        Refactoring
 ## -------------------------------------------------------------------------------------------------
 
 
 """
-Ver. 1.2.7  (2023-04-14)
+Ver. 1.2.8  (2024-04-10)
 
 This module wraps bf.Systems with MuJoCo Simulation functionality.
 """
 
 
 import time
 import glfw
 import mujoco
 import numpy as np
 from threading import Lock
 from lxml import etree
 
 from mlpro.rl.models import *
-from mlpro.wrappers.models import Wrapper
+from mlpro.wrappers.basics import Wrapper
 
 
 
 
 ## -------------------------------------------------------------------------------------------------
 ## -------------------------------------------------------------------------------------------------
 class CallbacksViewer():
```

### Comparing `mlpro-1.3.1/src/mlpro.egg-info/PKG-INFO` & `mlpro-1.4.0/src/mlpro.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpro
-Version: 1.3.1
+Version: 1.4.0
 Summary: MLPro - The Integrative Middleware Framework for Standardized Machine Learning
 Home-page: https://mlpro.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,28 +13,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: full
 Requires-Dist: dill>=0.3.6; extra == "full"
 Requires-Dist: numpy>=1.24.2; extra == "full"
 Requires-Dist: torch>=2.0.0; extra == "full"
 Requires-Dist: matplotlib>=3.7.1; extra == "full"
-Requires-Dist: stable_baselines3>=2.1.0; extra == "full"
 Requires-Dist: scipy>=1.10.1; extra == "full"
-Requires-Dist: pettingzoo>=1.22.3; extra == "full"
-Requires-Dist: pygame>=2.1.3; extra == "full"
-Requires-Dist: pymunk>=6.4.0; extra == "full"
 Requires-Dist: multiprocess>=0.70.14; extra == "full"
-Requires-Dist: river!=0.20.0,!=0.20.1,>=0.15.0; extra == "full"
-Requires-Dist: scikit-learn>=1.2.2; extra == "full"
 Requires-Dist: optuna>=3.1.1; extra == "full"
 Requires-Dist: hyperopt>=0.2.7; extra == "full"
-Requires-Dist: pyglet>=1.5.27; extra == "full"
-Requires-Dist: mujoco>=2.3.3; extra == "full"
+Requires-Dist: mujoco!=3.1.4,>=2.3.3; extra == "full"
 Requires-Dist: lxml>=4.9.2; extra == "full"
-Requires-Dist: gymnasium>=0.29; extra == "full"
+Requires-Dist: pandas>=2.1.3; extra == "full"
 
 [![CI](https://github.com/fhswf/MLPro/actions/workflows/ci.yml/badge.svg)](https://github.com/fhswf/MLPro/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/mlpro/badge/?version=latest)](https://mlpro.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/mlpro.svg)](https://badge.fury.io/py/mlpro)
 [![Anaconda-Version Badge](https://anaconda.org/mlpro/mlpro/badges/version.svg)](https://anaconda.org/mlpro/mlpro)
 [![Anaconda-Downloads Badge](https://img.shields.io/conda/dn/mlpro/mlpro?color=green&label=Anaconda.org%20Total%20downloads&style=flat-square)](https://anaconda.org/mlpro/mlpro)
 [![PyPI Total Downloads](https://static.pepy.tech/personalized-badge/mlpro?period=total&units=international_system&left_color=blue&right_color=orange&left_text=PyPI%20Total%20Downloads)](https://pepy.tech/project/mlpro)
```

### Comparing `mlpro-1.3.1/src/mlpro.egg-info/SOURCES.txt` & `mlpro-1.4.0/src/mlpro.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -36,20 +36,18 @@
 src/mlpro/bf/streams/samplers/__init__.py
 src/mlpro/bf/streams/samplers/min_wise.py
 src/mlpro/bf/streams/samplers/random.py
 src/mlpro/bf/streams/samplers/reservoir_sampling.py
 src/mlpro/bf/streams/samplers/weighted_random.py
 src/mlpro/bf/streams/streams/__init__.py
 src/mlpro/bf/streams/streams/clouds.py
-src/mlpro/bf/streams/streams/clouds2d_dynamic.py
-src/mlpro/bf/streams/streams/clouds2d_static.py
-src/mlpro/bf/streams/streams/clouds3d_dynamic.py
-src/mlpro/bf/streams/streams/clouds3d_static.py
+src/mlpro/bf/streams/streams/clouds_with_anomalies.py
 src/mlpro/bf/streams/streams/csv_file.py
 src/mlpro/bf/streams/streams/doublespiral2d.py
+src/mlpro/bf/streams/streams/point_outliers.py
 src/mlpro/bf/streams/streams/provider_mlpro.py
 src/mlpro/bf/streams/streams/rnd10d.py
 src/mlpro/bf/streams/tasks/__init__.py
 src/mlpro/bf/streams/tasks/deriver.py
 src/mlpro/bf/streams/tasks/rearranger.py
 src/mlpro/bf/streams/tasks/windows.py
 src/mlpro/bf/streams/workflows/__init__.py
@@ -92,15 +90,14 @@
 src/mlpro/gt/dynamicgames/potential.py
 src/mlpro/gt/dynamicgames/stackelberg.py
 src/mlpro/gt/native/__init__.py
 src/mlpro/gt/native/basics.py
 src/mlpro/gt/pool/__init__.py
 src/mlpro/gt/pool/boards/__init__.py
 src/mlpro/gt/pool/boards/bglp.py
-src/mlpro/gt/pool/boards/multicartpole.py
 src/mlpro/gt/pool/native/__init__.py
 src/mlpro/gt/pool/native/games/__init__.py
 src/mlpro/gt/pool/native/games/prisonersdilemma_2p.py
 src/mlpro/gt/pool/native/games/prisonersdilemma_3p.py
 src/mlpro/gt/pool/native/games/rockpaperscissors.py
 src/mlpro/gt/pool/native/games/routingproblems_3p.py
 src/mlpro/gt/pool/native/games/supplydemand_3p.py
@@ -112,18 +109,32 @@
 src/mlpro/oa/sciui/__init__.py
 src/mlpro/oa/sciui/iis.py
 src/mlpro/oa/sciui/runme.py
 src/mlpro/oa/sciui/scenario_oa1.py
 src/mlpro/oa/streams/__init__.py
 src/mlpro/oa/streams/basics.py
 src/mlpro/oa/streams/tasks/__init__.py
-src/mlpro/oa/streams/tasks/anomalydetectors.py
 src/mlpro/oa/streams/tasks/boundarydetectors.py
-src/mlpro/oa/streams/tasks/clusteranalyzers.py
 src/mlpro/oa/streams/tasks/normalizers.py
+src/mlpro/oa/streams/tasks/anomalydetectors/__init__.py
+src/mlpro/oa/streams/tasks/anomalydetectors/basics.py
+src/mlpro/oa/streams/tasks/anomalydetectors/cb_detectors.py
+src/mlpro/oa/streams/tasks/anomalydetectors/paga_detectors.py
+src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/__init__.py
+src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/basics.py
+src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/clusterbased.py
+src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/contextual.py
+src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/drift.py
+src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/group.py
+src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/point.py
+src/mlpro/oa/streams/tasks/clusteranalyzers/__init__.py
+src/mlpro/oa/streams/tasks/clusteranalyzers/basics.py
+src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/__init__.py
+src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/basics.py
+src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/centroid.py
 src/mlpro/oa/streams/workflows/__init__.py
 src/mlpro/oa/systems/__init__.py
 src/mlpro/oa/systems/basics.py
 src/mlpro/oa/systems/pool/__init__.py
 src/mlpro/oa/systems/pool/doublependulum.py
 src/mlpro/rl/__init__.py
 src/mlpro/rl/models.py
@@ -137,15 +148,14 @@
 src/mlpro/rl/pool/actionplanner/__init__.py
 src/mlpro/rl/pool/actionplanner/mpc.py
 src/mlpro/rl/pool/envs/__init__.py
 src/mlpro/rl/pool/envs/bglp.py
 src/mlpro/rl/pool/envs/cartpole.py
 src/mlpro/rl/pool/envs/doublependulum.py
 src/mlpro/rl/pool/envs/gridworld.py
-src/mlpro/rl/pool/envs/multicartpole.py
 src/mlpro/rl/pool/envs/robotinhtm.py
 src/mlpro/rl/pool/policies/__init__.py
 src/mlpro/rl/pool/policies/dummy.py
 src/mlpro/rl/pool/policies/randomgenerator.py
 src/mlpro/rl/pool/sarsbuffer/PrioritizedBuffer.py
 src/mlpro/rl/pool/sarsbuffer/RandomSARSBuffer.py
 src/mlpro/rl/pool/sarsbuffer/__init__.py
@@ -160,30 +170,15 @@
 src/mlpro/sl/pool/__init__.py
 src/mlpro/sl/pool/afct/__init__.py
 src/mlpro/sl/pool/afct/pytorch.py
 src/mlpro/sl/pool/afct/fnn/__init__.py
 src/mlpro/sl/pool/afct/fnn/pytorch/__init__.py
 src/mlpro/sl/pool/afct/fnn/pytorch/mlp.py
 src/mlpro/wrappers/__init__.py
-src/mlpro/wrappers/gymnasium.py
-src/mlpro/wrappers/hyperopt.py
-src/mlpro/wrappers/models.py
+src/mlpro/wrappers/basics.py
 src/mlpro/wrappers/mujoco.py
-src/mlpro/wrappers/openml.py
-src/mlpro/wrappers/optuna.py
-src/mlpro/wrappers/pettingzoo.py
-src/mlpro/wrappers/sb3.py
-src/mlpro/wrappers/river/__init__.py
-src/mlpro/wrappers/river/anomalydetectors.py
-src/mlpro/wrappers/river/basics.py
-src/mlpro/wrappers/river/clusteranalyzers.py
-src/mlpro/wrappers/river/streams.py
-src/mlpro/wrappers/sklearn/__init__.py
-src/mlpro/wrappers/sklearn/anomalydetectors.py
-src/mlpro/wrappers/sklearn/basics.py
 test/test_buffer.py
 test/test_environment.py
 test/test_examples.py
 test/test_math.py
 test/test_pool_policies.py
-test/test_sb3_policy_wrapper.py
 test/test_various.py
```

### Comparing `mlpro-1.3.1/test/test_buffer.py` & `mlpro-1.4.0/test/test_buffer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,50 @@
 ## -------------------------------------------------------------------------------------------------
 ## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
 ## -- Package : mlpro
-## -- Module  : test_buffer
+## -- Module  : test_buffer.py
 ## -------------------------------------------------------------------------------------------------
 ## -- History :
 ## -- yyyy-mm-dd  Ver.      Auth.    Description
 ## -- 2021-09-27  1.0.0     WB       Creation
 ## -- 2021-09-27  1.0.0     WB       Release First Version
 ## -- 2022-11-07  1.1.0     DA       Refactoring
 ## -- 2023-04-19  1.1.1     MRD      Refactor module import gym to gymnasium
+## -- 2024-02-16  1.1.2     SY       Replace gym environment to BGLP to remove dependency
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 1.1.1 (2023-04-19)
+Ver. 1.1.2 (2023-04-19)
 
 Unit test classes for SARBuffer.
 """
 
 
 import pytest
-import random
-import numpy as np
 from mlpro.bf.various import *
 from mlpro.bf.math import *
 from mlpro.bf.ml import *
 from mlpro.rl.models import *
-from mlpro.wrappers.gymnasium import WrEnvGYM2MLPro
+from mlpro.rl.pool.envs.bglp import BGLP
 from mlpro.rl.pool.sarsbuffer.PrioritizedBuffer import PrioritizedBuffer
 from mlpro.rl.pool.sarsbuffer.RandomSARSBuffer import RandomSARSBuffer
 from mlpro.rl.pool.policies.dummy import MyDummyPolicy
-import gymnasium as gym
-import random
-from pathlib import Path
 
 
 
             
 # -------------------------------------------------------------------------------------------------
 @pytest.mark.parametrize("buffer_cls", [PrioritizedBuffer, RandomSARSBuffer])
 def test_buffer(buffer_cls):    
     class MyScenario(RLScenario):
 
         C_NAME      = 'Matrix'
 
         def _setup(self, p_mode, p_ada: bool, p_visualize: bool, p_logging) -> Model:
-            if p_visualize:
-                gym_env     = gym.make('CartPole-v1', render_mode="human")
-            else:
-                gym_env     = gym.make('CartPole-v1')
-            self._env   = WrEnvGYM2MLPro(gym_env, p_visualize=p_visualize, p_logging=p_logging)
+            self._env = BGLP(p_logging=p_logging, cycle_limit=100)
 
             class MyDummyPol(MyDummyPolicy):
                 C_BUFFER_CLS = buffer_cls
                 
             # 2 Setup standard single-agent with own policy
             return Agent(
                 p_policy=MyDummyPol(
```

### Comparing `mlpro-1.3.1/test/test_environment.py` & `mlpro-1.4.0/test/test_environment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 ## -------------------------------------------------------------------------------------------------
 ## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
 ## -- Package : mlpro
-## -- Module  : test_environment
+## -- Module  : test_environment.py
 ## -------------------------------------------------------------------------------------------------
 ## -- History :
 ## -- yyyy-mm-dd  Ver.      Auth.    Description
 ## -- 2021-09-11  1.0.0     MRD      Creation
 ## -- 2021-09-11  1.0.0     MRD      Release First Version
 ## -- 2021-09-22  1.0.1     WB       Change Environment Instantiation Method
 ## -- 2021-09-26  1.0.2     MRD      Change the structure to work with GitHub Automated Test
 ## -- 2021-09-26  1.0.3     MRD      Change the import module due to the change of the pool
 ## --                                folder structer
 ## -- 2021-09-26  1.0.4     MRD      Change the import module due to the change of the pool
 ## --                                folder structer
 ## -- 2022-09-02  1.0.5     SY       Add DoublePendulumS7 and DoublePendulumS4
 ## -- 2022-09-13  1.0.5     SY       Add Sim_MPPS
 ## -- 2022-11-22  1.0.6     SY       Remove Sim_MPPS
+## -- 2024-02-16  1.0.7     SY       Remove Multi-Cartpole
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 1.0.6 (2022-11-22)
+Ver. 1.0.7 (2024-02-16)
 
 Unit test classes for environment.
 """
 
 
 import pytest
 import random
 import numpy as np
 from mlpro.rl.models import *
 from mlpro.rl.pool.envs.robotinhtm import RobotHTM
 from mlpro.rl.pool.envs.bglp import BGLP
 from mlpro.rl.pool.envs.gridworld import GridWorld
-from mlpro.rl.pool.envs.multicartpole import MultiCartPole
 from mlpro.rl.pool.envs.doublependulum import DoublePendulumS7
 from mlpro.rl.pool.envs.doublependulum import DoublePendulumS4
 
 
 ## -------------------------------------------------------------------------------------------------
-@pytest.mark.parametrize("env_cls", [RobotHTM, BGLP, GridWorld, MultiCartPole, DoublePendulumS7, DoublePendulumS4])
+@pytest.mark.parametrize("env_cls", [RobotHTM, BGLP, GridWorld, DoublePendulumS7, DoublePendulumS4])
 def test_environment(env_cls):
     env = env_cls(p_visualize=False)
     assert isinstance(env, Environment)
     
     assert isinstance(env.get_state_space(), ESpace)
     assert env.get_state_space().get_num_dim() != 0
```

### Comparing `mlpro-1.3.1/test/test_examples.py` & `mlpro-1.4.0/test/test_examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,15 @@
                             self.log(Log.C_LOG_TYPE_W, 'File ignored:', file)
 
             break
 
         return file_list
 
 
+sys.path.append('src')
 
 tester = HowtoTester()
 howtos = tester.get_howtos( sys.path[0] + os.sep + 'howtos' )
 
 
 if __name__ != '__main__':
     @pytest.mark.parametrize("p_path,p_file", howtos)
```

### Comparing `mlpro-1.3.1/test/test_math.py` & `mlpro-1.4.0/test/test_math.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ## -------------------------------------------------------------------------------------------------
 ## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
 ## -- Package : mlpro
-## -- Module  : test_math
+## -- Module  : test_math.py
 ## -------------------------------------------------------------------------------------------------
 ## -- History :
 ## -- yyyy-mm-dd  Ver.      Auth.    Description
 ## -- 2021-05-23  1.0.0     DA       Creation
 ## -- 2021-09-11  1.0.0     MRD      Change Header information to match our new library name
 ## -------------------------------------------------------------------------------------------------
```

### Comparing `mlpro-1.3.1/test/test_pool_policies.py` & `mlpro-1.4.0/test/test_pool_policies.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 ## -------------------------------------------------------------------------------------------------
 ## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
 ## -- Package : mlpro
-## -- Module  : test_pool_policies
+## -- Module  : test_pool_policies.py
 ## -------------------------------------------------------------------------------------------------
 ## -- History :
 ## -- yyyy-mm-dd  Ver.      Auth.    Description
 ## -- 2021-12-08  1.0.0     MRD      Creation
 ## -- 2022-05-19  1.0.1     SY       Add RandomGenerator policy
 ## -- 2022-11-07  1.1.0     DA       Refactoring
 ## -- 2023-04-19  1.1.1     MRD      Refactor module import gym to gymnasium
+## -- 2024-02-16  1.1.2     SY       Replace gym environment to BGLP to remove dependency
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 1.1.1 (2023-04-19)
+Ver. 1.1.2 (2023-04-19)
 
 Unit test classes for policies.
 """
 
 
 import pytest
-import gymnasium as gym
-import numpy as np
 from mlpro.rl import *
-from mlpro.wrappers.gymnasium import WrEnvGYM2MLPro
+from mlpro.rl.pool.envs.bglp import BGLP
 from mlpro.rl.pool.policies.dummy import MyDummyPolicy
 from mlpro.rl.pool.policies.randomgenerator import RandomGenerator
 
 ## Instructions
 # Please Include your own policy implementation class on the test list parameter
 
 
@@ -35,16 +34,15 @@
 def test_pool_policies(policy_cls):
     class MyScenario (RLScenario):
 
         C_NAME      = 'Matrix'
 
         def _setup(self, p_mode, p_ada: bool, p_visualize: bool, p_logging) -> Model:
             # 1 Setup environment
-            gym_env     = gym.make('CartPole-v1')
-            self._env   = WrEnvGYM2MLPro(gym_env, p_visualize=p_visualize, p_logging=p_logging) 
+            self._env = BGLP(p_logging=p_logging, cycle_limit=100)
 
             # 2 Setup and return standard single-agent with own policy
             return Agent(
                 p_policy=policy_cls(
                     p_observation_space=self._env.get_state_space(),
                     p_action_space=self._env.get_action_space(),
                     p_buffer_size=10,
```

### Comparing `mlpro-1.3.1/test/test_various.py` & `mlpro-1.4.0/test/test_various.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ## -------------------------------------------------------------------------------------------------
 ## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
 ## -- Package : mlpro
-## -- Module  : test_various
+## -- Module  : test_various.py
 ## -------------------------------------------------------------------------------------------------
 ## -- History :
 ## -- yyyy-mm-dd  Ver.      Auth.    Description
 ## -- 2021-04-16  1.0.0     DA       Creation
 ## -- 2021-09-11  1.0.0     MRD      Change Header information to match our new library name
 ## -------------------------------------------------------------------------------------------------
```

