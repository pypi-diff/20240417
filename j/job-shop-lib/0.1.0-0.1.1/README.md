# Comparing `tmp/job_shop_lib-0.1.0.tar.gz` & `tmp/job_shop_lib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "job_shop_lib-0.1.0.tar", max compression
+gzip compressed data, was "job_shop_lib-0.1.1.tar", max compression
```

## Comparing `job_shop_lib-0.1.0.tar` & `job_shop_lib-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1069 2024-02-06 16:50:21.344036 job_shop_lib-0.1.0/LICENSE
--rw-r--r--   0        0        0    12660 2024-04-17 16:40:03.167184 job_shop_lib-0.1.0/README.md
--rw-r--r--   0        0        0      581 2024-04-17 18:49:25.563004 job_shop_lib-0.1.0/job_shop_lib/__init__.py
--rw-r--r--   0        0        0     1368 2024-04-17 18:49:22.658989 job_shop_lib-0.1.0/job_shop_lib/base_solver.py
--rw-r--r--   0        0        0     3354 2024-04-17 18:29:10.381234 job_shop_lib-0.1.0/job_shop_lib/benchmarking/__init__.py
--rw-r--r--   0        0        0   464841 2024-03-01 17:52:19.596032 job_shop_lib-0.1.0/job_shop_lib/benchmarking/benchmark_instances.json
--rw-r--r--   0        0        0     5625 2024-04-13 15:45:21.680914 job_shop_lib-0.1.0/job_shop_lib/benchmarking/load_benchmark.py
--rw-r--r--   0        0        0       97 2024-04-13 17:42:22.701917 job_shop_lib-0.1.0/job_shop_lib/cp_sat/__init__.py
--rw-r--r--   0        0        0     8130 2024-04-17 18:26:23.704578 job_shop_lib-0.1.0/job_shop_lib/cp_sat/ortools_solver.py
--rw-r--r--   0        0        0     1432 2024-04-17 18:51:16.107562 job_shop_lib-0.1.0/job_shop_lib/dispatching/__init__.py
--rw-r--r--   0        0        0    10135 2024-04-17 18:40:15.600273 job_shop_lib-0.1.0/job_shop_lib/dispatching/dispatcher.py
--rw-r--r--   0        0        0     4392 2024-04-17 18:50:15.491255 job_shop_lib-0.1.0/job_shop_lib/dispatching/dispatching_rule_solver.py
--rw-r--r--   0        0        0     5557 2024-04-17 14:11:05.549956 job_shop_lib-0.1.0/job_shop_lib/dispatching/dispatching_rules.py
--rw-r--r--   0        0        0     7267 2024-04-17 18:36:42.623252 job_shop_lib-0.1.0/job_shop_lib/dispatching/factories.py
--rw-r--r--   0        0        0     4378 2024-04-17 14:09:16.084490 job_shop_lib-0.1.0/job_shop_lib/dispatching/pruning_functions.py
--rw-r--r--   0        0        0      899 2024-04-16 16:26:15.416010 job_shop_lib-0.1.0/job_shop_lib/exceptions.py
--rw-r--r--   0        0        0      154 2024-04-17 18:37:08.259373 job_shop_lib-0.1.0/job_shop_lib/generators/__init__.py
--rw-r--r--   0        0        0     7533 2024-04-17 18:37:26.163458 job_shop_lib-0.1.0/job_shop_lib/generators/basic_generator.py
--rw-r--r--   0        0        0     1454 2024-04-17 18:38:06.339650 job_shop_lib-0.1.0/job_shop_lib/graphs/__init__.py
--rw-r--r--   0        0        0     7128 2024-04-02 19:34:54.999808 job_shop_lib-0.1.0/job_shop_lib/graphs/build_agent_task_graph.py
--rw-r--r--   0        0        0     2877 2024-04-17 18:51:04.799505 job_shop_lib-0.1.0/job_shop_lib/graphs/build_disjunctive_graph.py
--rw-r--r--   0        0        0      374 2024-03-27 15:56:38.467324 job_shop_lib-0.1.0/job_shop_lib/graphs/constants.py
--rw-r--r--   0        0        0     5972 2024-04-02 19:26:46.141395 job_shop_lib-0.1.0/job_shop_lib/graphs/job_shop_graph.py
--rw-r--r--   0        0        0     4880 2024-03-28 10:18:53.973376 job_shop_lib-0.1.0/job_shop_lib/graphs/node.py
--rw-r--r--   0        0        0    12801 2024-04-03 10:47:39.697352 job_shop_lib-0.1.0/job_shop_lib/job_shop_instance.py
--rw-r--r--   0        0        0     3862 2024-04-06 19:26:36.742129 job_shop_lib-0.1.0/job_shop_lib/operation.py
--rw-r--r--   0        0        0     6509 2024-04-11 17:06:21.882095 job_shop_lib-0.1.0/job_shop_lib/schedule.py
--rw-r--r--   0        0        0     3127 2024-04-11 17:12:11.243224 job_shop_lib-0.1.0/job_shop_lib/scheduled_operation.py
--rw-r--r--   0        0        0      693 2024-04-17 18:46:13.614040 job_shop_lib-0.1.0/job_shop_lib/visualization/__init__.py
--rw-r--r--   0        0        0     8284 2024-04-03 10:47:25.781302 job_shop_lib-0.1.0/job_shop_lib/visualization/agent_task_graph.py
--rw-r--r--   0        0        0     6382 2024-04-17 18:51:20.995586 job_shop_lib-0.1.0/job_shop_lib/visualization/create_gif.py
--rw-r--r--   0        0        0     5803 2024-04-17 18:49:29.543024 job_shop_lib-0.1.0/job_shop_lib/visualization/disjunctive_graph.py
--rw-r--r--   0        0        0     4415 2024-04-17 18:52:22.519817 job_shop_lib-0.1.0/job_shop_lib/visualization/gantt_chart.py
--rw-r--r--   0        0        0     1372 2024-04-16 16:03:01.998600 job_shop_lib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    13503 1970-01-01 00:00:00.000000 job_shop_lib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-02-06 16:50:21.344036 job_shop_lib-0.1.1/LICENSE
+-rw-r--r--   0        0        0    12660 2024-04-17 16:40:03.167184 job_shop_lib-0.1.1/README.md
+-rw-r--r--   0        0        0      581 2024-04-17 18:49:25.563004 job_shop_lib-0.1.1/job_shop_lib/__init__.py
+-rw-r--r--   0        0        0     1368 2024-04-17 18:49:22.658989 job_shop_lib-0.1.1/job_shop_lib/base_solver.py
+-rw-r--r--   0        0        0     3354 2024-04-17 18:29:10.381234 job_shop_lib-0.1.1/job_shop_lib/benchmarking/__init__.py
+-rw-r--r--   0        0        0   464841 2024-03-01 17:52:19.596032 job_shop_lib-0.1.1/job_shop_lib/benchmarking/benchmark_instances.json
+-rw-r--r--   0        0        0     5625 2024-04-13 15:45:21.680914 job_shop_lib-0.1.1/job_shop_lib/benchmarking/load_benchmark.py
+-rw-r--r--   0        0        0       97 2024-04-13 17:42:22.701917 job_shop_lib-0.1.1/job_shop_lib/cp_sat/__init__.py
+-rw-r--r--   0        0        0     8130 2024-04-17 18:26:23.704578 job_shop_lib-0.1.1/job_shop_lib/cp_sat/ortools_solver.py
+-rw-r--r--   0        0        0     1432 2024-04-17 18:51:16.107562 job_shop_lib-0.1.1/job_shop_lib/dispatching/__init__.py
+-rw-r--r--   0        0        0    10135 2024-04-17 18:40:15.600273 job_shop_lib-0.1.1/job_shop_lib/dispatching/dispatcher.py
+-rw-r--r--   0        0        0     4392 2024-04-17 18:50:15.491255 job_shop_lib-0.1.1/job_shop_lib/dispatching/dispatching_rule_solver.py
+-rw-r--r--   0        0        0     5557 2024-04-17 14:11:05.549956 job_shop_lib-0.1.1/job_shop_lib/dispatching/dispatching_rules.py
+-rw-r--r--   0        0        0     7267 2024-04-17 18:36:42.623252 job_shop_lib-0.1.1/job_shop_lib/dispatching/factories.py
+-rw-r--r--   0        0        0     4378 2024-04-17 14:09:16.084490 job_shop_lib-0.1.1/job_shop_lib/dispatching/pruning_functions.py
+-rw-r--r--   0        0        0      899 2024-04-16 16:26:15.416010 job_shop_lib-0.1.1/job_shop_lib/exceptions.py
+-rw-r--r--   0        0        0      154 2024-04-17 18:37:08.259373 job_shop_lib-0.1.1/job_shop_lib/generators/__init__.py
+-rw-r--r--   0        0        0     7533 2024-04-17 18:37:26.163458 job_shop_lib-0.1.1/job_shop_lib/generators/basic_generator.py
+-rw-r--r--   0        0        0     1454 2024-04-17 18:38:06.339650 job_shop_lib-0.1.1/job_shop_lib/graphs/__init__.py
+-rw-r--r--   0        0        0     7128 2024-04-02 19:34:54.999808 job_shop_lib-0.1.1/job_shop_lib/graphs/build_agent_task_graph.py
+-rw-r--r--   0        0        0     2877 2024-04-17 18:51:04.799505 job_shop_lib-0.1.1/job_shop_lib/graphs/build_disjunctive_graph.py
+-rw-r--r--   0        0        0      374 2024-03-27 15:56:38.467324 job_shop_lib-0.1.1/job_shop_lib/graphs/constants.py
+-rw-r--r--   0        0        0     5972 2024-04-02 19:26:46.141395 job_shop_lib-0.1.1/job_shop_lib/graphs/job_shop_graph.py
+-rw-r--r--   0        0        0     4880 2024-03-28 10:18:53.973376 job_shop_lib-0.1.1/job_shop_lib/graphs/node.py
+-rw-r--r--   0        0        0    12801 2024-04-03 10:47:39.697352 job_shop_lib-0.1.1/job_shop_lib/job_shop_instance.py
+-rw-r--r--   0        0        0     3862 2024-04-06 19:26:36.742129 job_shop_lib-0.1.1/job_shop_lib/operation.py
+-rw-r--r--   0        0        0     6509 2024-04-11 17:06:21.882095 job_shop_lib-0.1.1/job_shop_lib/schedule.py
+-rw-r--r--   0        0        0     3127 2024-04-11 17:12:11.243224 job_shop_lib-0.1.1/job_shop_lib/scheduled_operation.py
+-rw-r--r--   0        0        0      693 2024-04-17 18:46:13.614040 job_shop_lib-0.1.1/job_shop_lib/visualization/__init__.py
+-rw-r--r--   0        0        0     8284 2024-04-03 10:47:25.781302 job_shop_lib-0.1.1/job_shop_lib/visualization/agent_task_graph.py
+-rw-r--r--   0        0        0     6382 2024-04-17 18:51:20.995586 job_shop_lib-0.1.1/job_shop_lib/visualization/create_gif.py
+-rw-r--r--   0        0        0     5803 2024-04-17 18:49:29.543024 job_shop_lib-0.1.1/job_shop_lib/visualization/disjunctive_graph.py
+-rw-r--r--   0        0        0     4415 2024-04-17 18:52:22.519817 job_shop_lib-0.1.1/job_shop_lib/visualization/gantt_chart.py
+-rw-r--r--   0        0        0     1352 2024-04-17 19:19:30.434622 job_shop_lib-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    13467 1970-01-01 00:00:00.000000 job_shop_lib-0.1.1/PKG-INFO
```

### Comparing `job_shop_lib-0.1.0/LICENSE` & `job_shop_lib-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/README.md` & `job_shop_lib-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/__init__.py` & `job_shop_lib-0.1.1/job_shop_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/base_solver.py` & `job_shop_lib-0.1.1/job_shop_lib/base_solver.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/benchmarking/__init__.py` & `job_shop_lib-0.1.1/job_shop_lib/benchmarking/__init__.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/benchmarking/benchmark_instances.json` & `job_shop_lib-0.1.1/job_shop_lib/benchmarking/benchmark_instances.json`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/benchmarking/load_benchmark.py` & `job_shop_lib-0.1.1/job_shop_lib/benchmarking/load_benchmark.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/cp_sat/ortools_solver.py` & `job_shop_lib-0.1.1/job_shop_lib/cp_sat/ortools_solver.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/dispatching/__init__.py` & `job_shop_lib-0.1.1/job_shop_lib/dispatching/__init__.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/dispatching/dispatcher.py` & `job_shop_lib-0.1.1/job_shop_lib/dispatching/dispatcher.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/dispatching/dispatching_rule_solver.py` & `job_shop_lib-0.1.1/job_shop_lib/dispatching/dispatching_rule_solver.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/dispatching/dispatching_rules.py` & `job_shop_lib-0.1.1/job_shop_lib/dispatching/dispatching_rules.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/dispatching/factories.py` & `job_shop_lib-0.1.1/job_shop_lib/dispatching/factories.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/dispatching/pruning_functions.py` & `job_shop_lib-0.1.1/job_shop_lib/dispatching/pruning_functions.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/exceptions.py` & `job_shop_lib-0.1.1/job_shop_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/generators/basic_generator.py` & `job_shop_lib-0.1.1/job_shop_lib/generators/basic_generator.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/graphs/__init__.py` & `job_shop_lib-0.1.1/job_shop_lib/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/graphs/build_agent_task_graph.py` & `job_shop_lib-0.1.1/job_shop_lib/graphs/build_agent_task_graph.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/graphs/build_disjunctive_graph.py` & `job_shop_lib-0.1.1/job_shop_lib/graphs/build_disjunctive_graph.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/graphs/job_shop_graph.py` & `job_shop_lib-0.1.1/job_shop_lib/graphs/job_shop_graph.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/graphs/node.py` & `job_shop_lib-0.1.1/job_shop_lib/graphs/node.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/job_shop_instance.py` & `job_shop_lib-0.1.1/job_shop_lib/job_shop_instance.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/operation.py` & `job_shop_lib-0.1.1/job_shop_lib/operation.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/schedule.py` & `job_shop_lib-0.1.1/job_shop_lib/schedule.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/scheduled_operation.py` & `job_shop_lib-0.1.1/job_shop_lib/scheduled_operation.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/visualization/__init__.py` & `job_shop_lib-0.1.1/job_shop_lib/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/visualization/agent_task_graph.py` & `job_shop_lib-0.1.1/job_shop_lib/visualization/agent_task_graph.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/visualization/create_gif.py` & `job_shop_lib-0.1.1/job_shop_lib/visualization/create_gif.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/visualization/disjunctive_graph.py` & `job_shop_lib-0.1.1/job_shop_lib/visualization/disjunctive_graph.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/job_shop_lib/visualization/gantt_chart.py` & `job_shop_lib-0.1.1/job_shop_lib/visualization/gantt_chart.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.0/pyproject.toml` & `job_shop_lib-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "job-shop-lib"
-version = "0.1.0"
+version = "0.1.1"
 description = "An easy-to-use and modular Python library for the Job Shop Scheduling Problem (JSSP)"
 authors = ["Pabloo22 <pablete.arino@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "job_shop_lib"}]
 include = ["benchmarks/benchmark_instances.json"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-ortools = "^9.8.3296"
-matplotlib = "^3.8.3"
+ortools = "^9"
+matplotlib = "^3"
 pyarrow = "^15.0.0"  # An optional pandas' dependency that will be required in the future
-networkx = "^3.2.1"
-imageio = "^2.34.0"
+networkx = "^3"
+imageio = "^2"
 pygraphviz = {version = "^1.12", optional = true}
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.0"
```

### Comparing `job_shop_lib-0.1.0/PKG-INFO` & `job_shop_lib-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: job-shop-lib
-Version: 0.1.0
+Version: 0.1.1
 Summary: An easy-to-use and modular Python library for the Job Shop Scheduling Problem (JSSP)
 License: MIT
 Author: Pabloo22
 Author-email: pablete.arino@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: pygraphviz
-Requires-Dist: imageio (>=2.34.0,<3.0.0)
-Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
-Requires-Dist: networkx (>=3.2.1,<4.0.0)
-Requires-Dist: ortools (>=9.8.3296,<10.0.0)
+Requires-Dist: imageio (>=2,<3)
+Requires-Dist: matplotlib (>=3,<4)
+Requires-Dist: networkx (>=3,<4)
+Requires-Dist: ortools (>=9,<10)
 Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
 Requires-Dist: pygraphviz (>=1.12,<2.0) ; extra == "pygraphviz"
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 <img src="images/logo_with_transparent_background.png" height="150px">
```

