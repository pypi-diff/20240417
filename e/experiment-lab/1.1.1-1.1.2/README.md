# Comparing `tmp/experiment_lab-1.1.1.tar.gz` & `tmp/experiment_lab-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experiment_lab-1.1.1.tar", last modified: Mon Apr 15 19:35:42 2024, max compression
+gzip compressed data, was "experiment_lab-1.1.2.tar", last modified: Wed Apr 17 00:44:07 2024, max compression
```

## Comparing `experiment_lab-1.1.1.tar` & `experiment_lab-1.1.2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.332099 experiment_lab-1.1.1/
--rw-r--r--   0 rbhagat    (501) staff       (20)     1066 2024-03-01 07:08:11.000000 experiment_lab-1.1.1/LICENCE
--rw-r--r--   0 rbhagat    (501) staff       (20)       42 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/MANIFEST.in
--rw-r--r--   0 rbhagat    (501) staff       (20)     3949 2024-04-15 19:35:42.331901 experiment_lab-1.1.1/PKG-INFO
--rw-r--r--   0 rbhagat    (501) staff       (20)     2763 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/README.md
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.325523 experiment_lab-1.1.1/experiment_lab/
--rw-r--r--   0 rbhagat    (501) staff       (20)       75 2024-04-15 19:33:48.000000 experiment_lab-1.1.1/experiment_lab/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.326288 experiment_lab-1.1.1/experiment_lab/common/
--rw-r--r--   0 rbhagat    (501) staff       (20)        0 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/common/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.326776 experiment_lab-1.1.1/experiment_lab/common/networks/
--rw-r--r--   0 rbhagat    (501) staff       (20)      240 2024-03-12 21:19:35.000000 experiment_lab-1.1.1/experiment_lab/common/networks/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1773 2024-03-11 20:50:57.000000 experiment_lab-1.1.1/experiment_lab/common/networks/blocks.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1820 2024-03-12 21:19:35.000000 experiment_lab-1.1.1/experiment_lab/common/networks/mlp.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     6764 2024-04-15 14:50:08.000000 experiment_lab-1.1.1/experiment_lab/common/networks/network.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.327126 experiment_lab-1.1.1/experiment_lab/common/resolvers/
--rw-r--r--   0 rbhagat    (501) staff       (20)      682 2024-03-11 14:00:07.000000 experiment_lab-1.1.1/experiment_lab/common/resolvers/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1708 2024-03-12 21:19:35.000000 experiment_lab-1.1.1/experiment_lab/common/resolvers/list_resolvers.py
--rw-r--r--   0 rbhagat    (501) staff       (20)      120 2024-03-11 14:00:07.000000 experiment_lab-1.1.1/experiment_lab/common/resolvers/object_resolvers.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.327267 experiment_lab-1.1.1/experiment_lab/common/utils/
--rw-r--r--   0 rbhagat    (501) staff       (20)     1548 2024-03-11 19:31:56.000000 experiment_lab-1.1.1/experiment_lab/common/utils/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.327387 experiment_lab-1.1.1/experiment_lab/configs/
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.327481 experiment_lab-1.1.1/experiment_lab/configs/__pycache__/
--rw-r--r--   0 rbhagat    (501) staff       (20)      181 2024-03-02 18:58:05.000000 experiment_lab-1.1.1/experiment_lab/configs/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 rbhagat    (501) staff       (20)       40 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/configs/config.yaml
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.327674 experiment_lab-1.1.1/experiment_lab/configs/mc/
--rw-r--r--   0 rbhagat    (501) staff       (20)       38 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/configs/mc/config.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)      750 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/configs/mc/estimate_pi.yaml
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.328167 experiment_lab-1.1.1/experiment_lab/configs/rl/
--rw-r--r--   0 rbhagat    (501) staff       (20)      423 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/configs/rl/atari.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)      543 2024-04-15 19:33:48.000000 experiment_lab-1.1.1/experiment_lab/configs/rl/cartpole.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)       39 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/configs/rl/config.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)      503 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/configs/rl/crossing.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)      534 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/configs/rl/walker.yaml
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.328405 experiment_lab-1.1.1/experiment_lab/configs/supervised/
--rw-r--r--   0 rbhagat    (501) staff       (20)       42 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/configs/supervised/config.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)     2478 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/configs/supervised/fashion_mnist.yaml
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.328988 experiment_lab-1.1.1/experiment_lab/core/
--rw-r--r--   0 rbhagat    (501) staff       (20)      265 2024-04-15 14:50:08.000000 experiment_lab-1.1.1/experiment_lab/core/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     5398 2024-04-15 14:50:08.000000 experiment_lab-1.1.1/experiment_lab/core/base_analysis.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1371 2024-04-15 14:50:08.000000 experiment_lab-1.1.1/experiment_lab/core/base_config.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     5645 2024-04-15 14:50:08.000000 experiment_lab-1.1.1/experiment_lab/core/base_experiment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     2299 2024-04-15 19:21:43.000000 experiment_lab-1.1.1/experiment_lab/core/runner.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.329074 experiment_lab-1.1.1/experiment_lab/experiments/
--rw-r--r--   0 rbhagat    (501) staff       (20)       44 2024-03-04 14:43:06.000000 experiment_lab-1.1.1/experiment_lab/experiments/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.329430 experiment_lab-1.1.1/experiment_lab/experiments/examples/
--rw-r--r--   0 rbhagat    (501) staff       (20)       36 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/experiments/examples/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1767 2024-03-11 14:00:07.000000 experiment_lab-1.1.1/experiment_lab/experiments/examples/mc_pi_estimate.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1371 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/experiments/examples/random_waits.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.329812 experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/
--rw-r--r--   0 rbhagat    (501) staff       (20)      120 2024-03-11 14:00:07.000000 experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.330294 experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/components/
--rw-r--r--   0 rbhagat    (501) staff       (20)      563 2024-03-11 14:00:07.000000 experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/components/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     2328 2024-03-11 14:00:07.000000 experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/components/aggregators.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1103 2024-03-11 14:00:07.000000 experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/components/post_processors.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1062 2024-03-11 14:00:07.000000 experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/components/sample_filters.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1902 2024-03-11 14:00:07.000000 experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/components/samplers.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1638 2024-04-03 18:52:52.000000 experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/config.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     3212 2024-04-03 18:52:52.000000 experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/experiment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)      575 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/main.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.330879 experiment_lab-1.1.1/experiment_lab/experiments/rl/
--rw-r--r--   0 rbhagat    (501) staff       (20)      255 2024-03-11 14:00:07.000000 experiment_lab-1.1.1/experiment_lab/experiments/rl/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1421 2024-04-15 14:50:08.000000 experiment_lab-1.1.1/experiment_lab/experiments/rl/analysis.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1852 2024-03-13 20:27:53.000000 experiment_lab-1.1.1/experiment_lab/experiments/rl/config.py
--rw-r--r--   0 rbhagat    (501) staff       (20)    10546 2024-04-15 14:50:08.000000 experiment_lab-1.1.1/experiment_lab/experiments/rl/environment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     6423 2024-04-15 19:33:48.000000 experiment_lab-1.1.1/experiment_lab/experiments/rl/experiment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)      656 2024-04-15 14:50:08.000000 experiment_lab-1.1.1/experiment_lab/experiments/rl/main.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.331279 experiment_lab-1.1.1/experiment_lab/experiments/supervised/
--rw-r--r--   0 rbhagat    (501) staff       (20)       63 2024-03-12 21:19:35.000000 experiment_lab-1.1.1/experiment_lab/experiments/supervised/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     3436 2024-03-12 21:19:35.000000 experiment_lab-1.1.1/experiment_lab/experiments/supervised/config.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     8526 2024-03-13 13:55:28.000000 experiment_lab-1.1.1/experiment_lab/experiments/supervised/experiment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)      641 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/experiment_lab/experiments/supervised/main.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-15 19:35:42.331395 experiment_lab-1.1.1/experiment_lab.egg-info/
--rw-r--r--   0 rbhagat    (501) staff       (20)     3949 2024-04-15 19:35:42.000000 experiment_lab-1.1.1/experiment_lab.egg-info/PKG-INFO
--rw-r--r--   0 rbhagat    (501) staff       (20)     2501 2024-04-15 19:35:42.000000 experiment_lab-1.1.1/experiment_lab.egg-info/SOURCES.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)        1 2024-04-15 19:35:42.000000 experiment_lab-1.1.1/experiment_lab.egg-info/dependency_links.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)      237 2024-04-15 19:35:42.000000 experiment_lab-1.1.1/experiment_lab.egg-info/entry_points.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)      223 2024-04-15 19:35:42.000000 experiment_lab-1.1.1/experiment_lab.egg-info/requires.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)       15 2024-04-15 19:35:42.000000 experiment_lab-1.1.1/experiment_lab.egg-info/top_level.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)     1200 2024-03-23 19:11:29.000000 experiment_lab-1.1.1/pyproject.toml
--rw-r--r--   0 rbhagat    (501) staff       (20)       38 2024-04-15 19:35:42.332129 experiment_lab-1.1.1/setup.cfg
--rw-r--r--   0 rbhagat    (501) staff       (20)     1030 2024-03-03 02:11:13.000000 experiment_lab-1.1.1/setup.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-17 00:44:07.354715 experiment_lab-1.1.2/
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1066 2024-03-01 07:08:11.000000 experiment_lab-1.1.2/LICENCE
+-rw-r--r--   0 rbhagat    (501) staff       (20)       42 2024-03-23 19:11:29.000000 experiment_lab-1.1.2/MANIFEST.in
+-rw-r--r--   0 rbhagat    (501) staff       (20)     3949 2024-04-17 00:44:07.354548 experiment_lab-1.1.2/PKG-INFO
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2763 2024-03-23 19:11:29.000000 experiment_lab-1.1.2/README.md
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-17 00:44:07.348080 experiment_lab-1.1.2/experiment_lab/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       75 2024-04-17 00:41:18.000000 experiment_lab-1.1.2/experiment_lab/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-17 00:44:07.348833 experiment_lab-1.1.2/experiment_lab/common/
+-rw-r--r--   0 rbhagat    (501) staff       (20)        0 2024-03-23 19:11:29.000000 experiment_lab-1.1.2/experiment_lab/common/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-17 00:44:07.349244 experiment_lab-1.1.2/experiment_lab/common/networks/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      240 2024-03-12 21:19:35.000000 experiment_lab-1.1.2/experiment_lab/common/networks/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1773 2024-03-11 20:50:57.000000 experiment_lab-1.1.2/experiment_lab/common/networks/blocks.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1820 2024-03-12 21:19:35.000000 experiment_lab-1.1.2/experiment_lab/common/networks/mlp.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     6764 2024-04-15 14:50:08.000000 experiment_lab-1.1.2/experiment_lab/common/networks/network.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-17 00:44:07.349581 experiment_lab-1.1.2/experiment_lab/common/resolvers/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      682 2024-03-11 14:00:07.000000 experiment_lab-1.1.2/experiment_lab/common/resolvers/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1708 2024-03-12 21:19:35.000000 experiment_lab-1.1.2/experiment_lab/common/resolvers/list_resolvers.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)      120 2024-03-11 14:00:07.000000 experiment_lab-1.1.2/experiment_lab/common/resolvers/object_resolvers.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-17 00:44:07.349710 experiment_lab-1.1.2/experiment_lab/common/utils/
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1548 2024-03-11 19:31:56.000000 experiment_lab-1.1.2/experiment_lab/common/utils/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-17 00:44:07.349837 experiment_lab-1.1.2/experiment_lab/configs/
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-17 00:44:07.349944 experiment_lab-1.1.2/experiment_lab/configs/__pycache__/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      181 2024-03-02 18:58:05.000000 experiment_lab-1.1.2/experiment_lab/configs/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 rbhagat    (501) staff       (20)       40 2024-03-23 19:11:29.000000 experiment_lab-1.1.2/experiment_lab/configs/config.yaml
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-17 00:44:07.350162 experiment_lab-1.1.2/experiment_lab/configs/mc/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       38 2024-03-23 19:11:29.000000 experiment_lab-1.1.2/experiment_lab/configs/mc/config.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)      750 2024-03-23 19:11:29.000000 experiment_lab-1.1.2/experiment_lab/configs/mc/estimate_pi.yaml
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-17 00:44:07.350697 experiment_lab-1.1.2/experiment_lab/configs/rl/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      423 2024-03-23 19:11:29.000000 experiment_lab-1.1.2/experiment_lab/configs/rl/atari.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)      543 2024-04-15 19:33:48.000000 experiment_lab-1.1.2/experiment_lab/configs/rl/cartpole.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)       39 2024-03-23 19:11:29.000000 experiment_lab-1.1.2/experiment_lab/configs/rl/config.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)      503 2024-03-23 19:11:29.000000 experiment_lab-1.1.2/experiment_lab/configs/rl/crossing.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)      534 2024-03-23 19:11:29.000000 experiment_lab-1.1.2/experiment_lab/configs/rl/walker.yaml
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-17 00:44:07.350932 experiment_lab-1.1.2/experiment_lab/configs/supervised/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       42 2024-03-23 19:11:29.000000 experiment_lab-1.1.2/experiment_lab/configs/supervised/config.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2478 2024-03-23 19:11:29.000000 experiment_lab-1.1.2/experiment_lab/configs/supervised/fashion_mnist.yaml
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-17 00:44:07.351472 experiment_lab-1.1.2/experiment_lab/core/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      265 2024-04-15 14:50:08.000000 experiment_lab-1.1.2/experiment_lab/core/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     5398 2024-04-15 14:50:08.000000 experiment_lab-1.1.2/experiment_lab/core/base_analysis.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1371 2024-04-15 14:50:08.000000 experiment_lab-1.1.2/experiment_lab/core/base_config.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     5645 2024-04-15 14:50:08.000000 experiment_lab-1.1.2/experiment_lab/core/base_experiment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2299 2024-04-15 19:21:43.000000 experiment_lab-1.1.2/experiment_lab/core/runner.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-17 00:44:07.351579 experiment_lab-1.1.2/experiment_lab/experiments/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       44 2024-03-04 14:43:06.000000 experiment_lab-1.1.2/experiment_lab/experiments/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-17 00:44:07.351888 experiment_lab-1.1.2/experiment_lab/experiments/examples/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       36 2024-03-23 19:11:29.000000 experiment_lab-1.1.2/experiment_lab/experiments/examples/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1767 2024-03-11 14:00:07.000000 experiment_lab-1.1.2/experiment_lab/experiments/examples/mc_pi_estimate.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1371 2024-03-23 19:11:29.000000 experiment_lab-1.1.2/experiment_lab/experiments/examples/random_waits.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-17 00:44:07.352275 experiment_lab-1.1.2/experiment_lab/experiments/monte_carlo/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      120 2024-03-11 14:00:07.000000 experiment_lab-1.1.2/experiment_lab/experiments/monte_carlo/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-17 00:44:07.352772 experiment_lab-1.1.2/experiment_lab/experiments/monte_carlo/components/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      563 2024-03-11 14:00:07.000000 experiment_lab-1.1.2/experiment_lab/experiments/monte_carlo/components/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2328 2024-03-11 14:00:07.000000 experiment_lab-1.1.2/experiment_lab/experiments/monte_carlo/components/aggregators.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1103 2024-03-11 14:00:07.000000 experiment_lab-1.1.2/experiment_lab/experiments/monte_carlo/components/post_processors.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1062 2024-03-11 14:00:07.000000 experiment_lab-1.1.2/experiment_lab/experiments/monte_carlo/components/sample_filters.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1902 2024-03-11 14:00:07.000000 experiment_lab-1.1.2/experiment_lab/experiments/monte_carlo/components/samplers.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1638 2024-04-03 18:52:52.000000 experiment_lab-1.1.2/experiment_lab/experiments/monte_carlo/config.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     3212 2024-04-03 18:52:52.000000 experiment_lab-1.1.2/experiment_lab/experiments/monte_carlo/experiment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)      575 2024-03-23 19:11:29.000000 experiment_lab-1.1.2/experiment_lab/experiments/monte_carlo/main.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-17 00:44:07.353435 experiment_lab-1.1.2/experiment_lab/experiments/rl/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      255 2024-03-11 14:00:07.000000 experiment_lab-1.1.2/experiment_lab/experiments/rl/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1421 2024-04-15 14:50:08.000000 experiment_lab-1.1.2/experiment_lab/experiments/rl/analysis.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1852 2024-03-13 20:27:53.000000 experiment_lab-1.1.2/experiment_lab/experiments/rl/config.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)    10546 2024-04-15 14:50:08.000000 experiment_lab-1.1.2/experiment_lab/experiments/rl/environment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     6423 2024-04-15 19:33:48.000000 experiment_lab-1.1.2/experiment_lab/experiments/rl/experiment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)      656 2024-04-15 14:50:08.000000 experiment_lab-1.1.2/experiment_lab/experiments/rl/main.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-17 00:44:07.353892 experiment_lab-1.1.2/experiment_lab/experiments/supervised/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       63 2024-03-12 21:19:35.000000 experiment_lab-1.1.2/experiment_lab/experiments/supervised/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     3436 2024-03-12 21:19:35.000000 experiment_lab-1.1.2/experiment_lab/experiments/supervised/config.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     8526 2024-03-13 13:55:28.000000 experiment_lab-1.1.2/experiment_lab/experiments/supervised/experiment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)      641 2024-03-23 19:11:29.000000 experiment_lab-1.1.2/experiment_lab/experiments/supervised/main.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-17 00:44:07.354031 experiment_lab-1.1.2/experiment_lab.egg-info/
+-rw-r--r--   0 rbhagat    (501) staff       (20)     3949 2024-04-17 00:44:07.000000 experiment_lab-1.1.2/experiment_lab.egg-info/PKG-INFO
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2501 2024-04-17 00:44:07.000000 experiment_lab-1.1.2/experiment_lab.egg-info/SOURCES.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)        1 2024-04-17 00:44:07.000000 experiment_lab-1.1.2/experiment_lab.egg-info/dependency_links.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)      237 2024-04-17 00:44:07.000000 experiment_lab-1.1.2/experiment_lab.egg-info/entry_points.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)      223 2024-04-17 00:44:07.000000 experiment_lab-1.1.2/experiment_lab.egg-info/requires.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)       15 2024-04-17 00:44:07.000000 experiment_lab-1.1.2/experiment_lab.egg-info/top_level.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1200 2024-03-23 19:11:29.000000 experiment_lab-1.1.2/pyproject.toml
+-rw-r--r--   0 rbhagat    (501) staff       (20)       38 2024-04-17 00:44:07.354750 experiment_lab-1.1.2/setup.cfg
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1030 2024-03-03 02:11:13.000000 experiment_lab-1.1.2/setup.py
```

### Comparing `experiment_lab-1.1.1/LICENCE` & `experiment_lab-1.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/PKG-INFO` & `experiment_lab-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experiment-lab
-Version: 1.1.1
+Version: 1.1.2
 Summary: A suite of flexible experiments of a variety of different tasks.
 Author-email: Rishav Bhagat <rishavbhagat.cs@gmail.com>
 Project-URL: Repository, https://github.com/rishavb123/ExperimentLab
 Keywords: experiment,suite,lab
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `experiment_lab-1.1.1/README.md` & `experiment_lab-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/common/networks/blocks.py` & `experiment_lab-1.1.2/experiment_lab/common/networks/blocks.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/common/networks/mlp.py` & `experiment_lab-1.1.2/experiment_lab/common/networks/mlp.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/common/networks/network.py` & `experiment_lab-1.1.2/experiment_lab/common/networks/network.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/common/resolvers/__init__.py` & `experiment_lab-1.1.2/experiment_lab/common/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/common/resolvers/list_resolvers.py` & `experiment_lab-1.1.2/experiment_lab/common/resolvers/list_resolvers.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/common/utils/__init__.py` & `experiment_lab-1.1.2/experiment_lab/common/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/configs/mc/estimate_pi.yaml` & `experiment_lab-1.1.2/experiment_lab/configs/mc/estimate_pi.yaml`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/configs/rl/cartpole.yaml` & `experiment_lab-1.1.2/experiment_lab/configs/rl/cartpole.yaml`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/configs/rl/walker.yaml` & `experiment_lab-1.1.2/experiment_lab/configs/rl/walker.yaml`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/configs/supervised/fashion_mnist.yaml` & `experiment_lab-1.1.2/experiment_lab/configs/supervised/fashion_mnist.yaml`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/core/base_analysis.py` & `experiment_lab-1.1.2/experiment_lab/core/base_analysis.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/core/base_config.py` & `experiment_lab-1.1.2/experiment_lab/core/base_config.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/core/base_experiment.py` & `experiment_lab-1.1.2/experiment_lab/core/base_experiment.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/core/runner.py` & `experiment_lab-1.1.2/experiment_lab/core/runner.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/experiments/examples/mc_pi_estimate.py` & `experiment_lab-1.1.2/experiment_lab/experiments/examples/mc_pi_estimate.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/experiments/examples/random_waits.py` & `experiment_lab-1.1.2/experiment_lab/experiments/examples/random_waits.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/components/__init__.py` & `experiment_lab-1.1.2/experiment_lab/experiments/monte_carlo/components/__init__.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/components/aggregators.py` & `experiment_lab-1.1.2/experiment_lab/experiments/monte_carlo/components/aggregators.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/components/post_processors.py` & `experiment_lab-1.1.2/experiment_lab/experiments/monte_carlo/components/post_processors.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/components/sample_filters.py` & `experiment_lab-1.1.2/experiment_lab/experiments/monte_carlo/components/sample_filters.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/components/samplers.py` & `experiment_lab-1.1.2/experiment_lab/experiments/monte_carlo/components/samplers.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/config.py` & `experiment_lab-1.1.2/experiment_lab/experiments/monte_carlo/config.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/experiment.py` & `experiment_lab-1.1.2/experiment_lab/experiments/monte_carlo/experiment.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/experiments/monte_carlo/main.py` & `experiment_lab-1.1.2/experiment_lab/experiments/monte_carlo/main.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/experiments/rl/analysis.py` & `experiment_lab-1.1.2/experiment_lab/experiments/rl/analysis.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/experiments/rl/config.py` & `experiment_lab-1.1.2/experiment_lab/experiments/rl/config.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/experiments/rl/environment.py` & `experiment_lab-1.1.2/experiment_lab/experiments/rl/environment.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/experiments/rl/experiment.py` & `experiment_lab-1.1.2/experiment_lab/experiments/rl/experiment.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/experiments/rl/main.py` & `experiment_lab-1.1.2/experiment_lab/experiments/rl/main.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/experiments/supervised/config.py` & `experiment_lab-1.1.2/experiment_lab/experiments/supervised/config.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/experiments/supervised/experiment.py` & `experiment_lab-1.1.2/experiment_lab/experiments/supervised/experiment.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab/experiments/supervised/main.py` & `experiment_lab-1.1.2/experiment_lab/experiments/supervised/main.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/experiment_lab.egg-info/PKG-INFO` & `experiment_lab-1.1.2/experiment_lab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experiment-lab
-Version: 1.1.1
+Version: 1.1.2
 Summary: A suite of flexible experiments of a variety of different tasks.
 Author-email: Rishav Bhagat <rishavbhagat.cs@gmail.com>
 Project-URL: Repository, https://github.com/rishavb123/ExperimentLab
 Keywords: experiment,suite,lab
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `experiment_lab-1.1.1/experiment_lab.egg-info/SOURCES.txt` & `experiment_lab-1.1.2/experiment_lab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/pyproject.toml` & `experiment_lab-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.1/setup.py` & `experiment_lab-1.1.2/setup.py`

 * *Files identical despite different names*

