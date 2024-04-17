# Comparing `tmp/drex-0.0.242.tar.gz` & `tmp/drex-0.0.243.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drex-0.0.242.tar", last modified: Tue Apr 16 13:44:01 2024, max compression
+gzip compressed data, was "drex-0.0.243.tar", last modified: Wed Apr 17 08:54:32 2024, max compression
```

## Comparing `drex-0.0.242.tar` & `drex-0.0.243.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-16 13:44:01.958234 drex-0.0.242/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)       98 2024-03-29 18:39:48.000000 drex-0.0.242/.gitignore
--rw-r--r--   0 domizzi   (1000) domizzi   (1000)      720 2024-04-16 13:44:01.958234 drex-0.0.242/PKG-INFO
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      335 2024-04-04 15:50:32.000000 drex-0.0.242/README.md
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-16 13:44:01.958234 drex-0.0.242/data/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2912 2024-03-26 20:01:38.000000 drex-0.0.242/data/10MB.csv
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     7032 2024-03-26 20:01:41.000000 drex-0.0.242/data/1MB.csv
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2903 2024-03-26 20:01:25.000000 drex-0.0.242/data/200MB.csv
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1303 2024-03-26 20:01:44.000000 drex-0.0.242/data/50MB.csv
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-16 13:44:01.958234 drex-0.0.242/drex/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-03-28 21:09:29.000000 drex-0.0.242/drex/__init__.py
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-16 13:44:01.958234 drex-0.0.242/drex/schedulers/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      570 2024-04-15 08:46:06.000000 drex-0.0.242/drex/schedulers/algorithm1.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1418 2024-04-15 08:46:26.000000 drex-0.0.242/drex/schedulers/algorithm2.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     3138 2024-04-15 08:46:34.000000 drex-0.0.242/drex/schedulers/algorithm3.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1647 2024-04-15 08:30:49.000000 drex-0.0.242/drex/schedulers/random.py
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-16 13:44:01.958234 drex-0.0.242/drex/utils/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-03-28 21:06:13.000000 drex-0.0.242/drex/utils/__init__.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      784 2024-03-26 21:04:00.000000 drex-0.0.242/drex/utils/load_data.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    10547 2024-03-26 19:02:20.000000 drex-0.0.242/drex/utils/poibin.py
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-16 13:44:01.958234 drex-0.0.242/drex/utils/reliability/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-03-28 21:06:19.000000 drex-0.0.242/drex/utils/reliability/__init__.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     5214 2024-03-28 16:17:33.000000 drex-0.0.242/drex/utils/reliability/fragment_handler.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     6772 2024-03-28 21:59:40.000000 drex-0.0.242/drex/utils/reliability/ida.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     4913 2024-03-28 16:17:33.000000 drex-0.0.242/drex/utils/reliability/utils.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     5350 2024-04-15 08:30:49.000000 drex-0.0.242/drex/utils/tool_functions.py
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-16 13:44:01.958234 drex-0.0.242/drex.egg-info/
--rw-r--r--   0 domizzi   (1000) domizzi   (1000)      720 2024-04-16 13:44:01.000000 drex-0.0.242/drex.egg-info/PKG-INFO
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      635 2024-04-16 13:44:01.000000 drex-0.0.242/drex.egg-info/SOURCES.txt
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        1 2024-04-16 13:44:01.000000 drex-0.0.242/drex.egg-info/dependency_links.txt
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)       12 2024-04-16 13:44:01.000000 drex-0.0.242/drex.egg-info/requires.txt
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        5 2024-04-16 13:44:01.000000 drex-0.0.242/drex.egg-info/top_level.txt
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      595 2024-04-16 13:38:39.000000 drex-0.0.242/pyproject.toml
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)       38 2024-04-16 13:44:01.958234 drex-0.0.242/setup.cfg
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-16 13:44:01.958234 drex-0.0.242/test/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-04-01 18:01:10.000000 drex-0.0.242/test/__init__.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2157 2024-04-15 08:38:51.000000 drex-0.0.242/test/drex-test.py
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-17 08:54:32.940893 drex-0.0.243/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)       98 2024-03-29 18:39:48.000000 drex-0.0.243/.gitignore
+-rw-r--r--   0 domizzi   (1000) domizzi   (1000)      720 2024-04-17 08:54:32.940893 drex-0.0.243/PKG-INFO
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      335 2024-04-04 15:50:32.000000 drex-0.0.243/README.md
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-17 08:54:32.936893 drex-0.0.243/data/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2912 2024-03-26 20:01:38.000000 drex-0.0.243/data/10MB.csv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     7032 2024-03-26 20:01:41.000000 drex-0.0.243/data/1MB.csv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2903 2024-03-26 20:01:25.000000 drex-0.0.243/data/200MB.csv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1303 2024-03-26 20:01:44.000000 drex-0.0.243/data/50MB.csv
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-17 08:54:32.936893 drex-0.0.243/drex/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-03-28 21:09:29.000000 drex-0.0.243/drex/__init__.py
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-17 08:54:32.940893 drex-0.0.243/drex/schedulers/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      576 2024-04-17 08:25:26.000000 drex-0.0.243/drex/schedulers/algorithm1.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1432 2024-04-17 08:33:42.000000 drex-0.0.243/drex/schedulers/algorithm2.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     3152 2024-04-17 08:33:49.000000 drex-0.0.243/drex/schedulers/algorithm3.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1647 2024-04-15 08:30:49.000000 drex-0.0.243/drex/schedulers/random.py
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-17 08:54:32.940893 drex-0.0.243/drex/utils/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-03-28 21:06:13.000000 drex-0.0.243/drex/utils/__init__.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      784 2024-03-26 21:04:00.000000 drex-0.0.243/drex/utils/load_data.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    10547 2024-03-26 19:02:20.000000 drex-0.0.243/drex/utils/poibin.py
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-17 08:54:32.940893 drex-0.0.243/drex/utils/reliability/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-03-28 21:06:19.000000 drex-0.0.243/drex/utils/reliability/__init__.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     5214 2024-03-28 16:17:33.000000 drex-0.0.243/drex/utils/reliability/fragment_handler.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     6772 2024-03-28 21:59:40.000000 drex-0.0.243/drex/utils/reliability/ida.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     4913 2024-03-28 16:17:33.000000 drex-0.0.243/drex/utils/reliability/utils.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     5350 2024-04-15 08:30:49.000000 drex-0.0.243/drex/utils/tool_functions.py
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-17 08:54:32.940893 drex-0.0.243/drex.egg-info/
+-rw-r--r--   0 domizzi   (1000) domizzi   (1000)      720 2024-04-17 08:54:32.000000 drex-0.0.243/drex.egg-info/PKG-INFO
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      635 2024-04-17 08:54:32.000000 drex-0.0.243/drex.egg-info/SOURCES.txt
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        1 2024-04-17 08:54:32.000000 drex-0.0.243/drex.egg-info/dependency_links.txt
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)       12 2024-04-17 08:54:32.000000 drex-0.0.243/drex.egg-info/requires.txt
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        5 2024-04-17 08:54:32.000000 drex-0.0.243/drex.egg-info/top_level.txt
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      595 2024-04-17 08:54:05.000000 drex-0.0.243/pyproject.toml
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)       38 2024-04-17 08:54:32.940893 drex-0.0.243/setup.cfg
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-17 08:54:32.940893 drex-0.0.243/test/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-04-01 18:01:10.000000 drex-0.0.243/test/__init__.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2150 2024-04-17 08:36:19.000000 drex-0.0.243/test/drex-test.py
```

### Comparing `drex-0.0.242/PKG-INFO` & `drex-0.0.243/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drex
-Version: 0.0.242
+Version: 0.0.243
 Summary: DRex package
 Author-email: "Maxime, Dante, Haochen" <dantsanc@pa.uc3m.es>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `drex-0.0.242/data/10MB.csv` & `drex-0.0.243/data/10MB.csv`

 * *Files identical despite different names*

### Comparing `drex-0.0.242/data/1MB.csv` & `drex-0.0.243/data/1MB.csv`

 * *Files identical despite different names*

### Comparing `drex-0.0.242/data/200MB.csv` & `drex-0.0.243/data/200MB.csv`

 * *Files identical despite different names*

### Comparing `drex-0.0.242/data/50MB.csv` & `drex-0.0.243/data/50MB.csv`

 * *Files identical despite different names*

### Comparing `drex-0.0.242/drex/schedulers/algorithm1.py` & `drex-0.0.243/drex/schedulers/algorithm1.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 	K = get_max_K_from_reliability_threshold_and_nodes_chosen(N, reliability_threshold, reliability_of_nodes)
 	if (N == -1):
 		print("ERROR: No N was found for Algorithm 1.")
 		exit(1)
 	set_of_nodes = list(range(0, number_of_nodes))
 	end = time.time()
 	print("\nAlgorithm 1 chose N =", N, "and K =", K, "with the set of nodes:", set_of_nodes, "It took", end - start, "seconds.")
-	return set_of_nodes
+	return set_of_nodes, N, K
```

### Comparing `drex-0.0.242/drex/schedulers/algorithm2.py` & `drex-0.0.243/drex/schedulers/algorithm2.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 				if (replication_and_write_time < min_time):
 					min_time = replication_and_write_time
 					min_N = i
 					min_K = K
 					min_set_of_nodes_chosen = set_of_nodes_chosen
 	end = time.time()
 	print("\nAlgorithm 2 chose N =", min_N, "and K =", min_K, "with the set of nodes:", min_set_of_nodes_chosen, "It took", end - start, "seconds.")
-	return min_set_of_nodes_chosen
+	return min_set_of_nodes_chosen, min_N, min_K
```

### Comparing `drex-0.0.242/drex/schedulers/algorithm3.py` & `drex-0.0.243/drex/schedulers/algorithm3.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,8 +59,8 @@
 	
 	min_N = set_of_possible_solutions[set_of_solution_on_pareto[min_index]][0]
 	min_K = set_of_possible_solutions[set_of_solution_on_pareto[min_index]][1]
 	min_set_of_nodes_chosen = set_of_possible_solutions[set_of_solution_on_pareto[min_index]][2]
 
 	end = time.time()
 	print("\nAlgorithm 3 chose N =", min_N, "and K =", min_K, "with the set of nodes:", min_set_of_nodes_chosen, "It took", end - start, "seconds.")
-	return min_set_of_nodes_chosen
+	return min_set_of_nodes_chosen, min_N, min_K
```

### Comparing `drex-0.0.242/drex/schedulers/random.py` & `drex-0.0.243/drex/schedulers/random.py`

 * *Files identical despite different names*

### Comparing `drex-0.0.242/drex/utils/load_data.py` & `drex-0.0.243/drex/utils/load_data.py`

 * *Files identical despite different names*

### Comparing `drex-0.0.242/drex/utils/poibin.py` & `drex-0.0.243/drex/utils/poibin.py`

 * *Files identical despite different names*

### Comparing `drex-0.0.242/drex/utils/reliability/fragment_handler.py` & `drex-0.0.243/drex/utils/reliability/fragment_handler.py`

 * *Files identical despite different names*

### Comparing `drex-0.0.242/drex/utils/reliability/ida.py` & `drex-0.0.243/drex/utils/reliability/ida.py`

 * *Files identical despite different names*

### Comparing `drex-0.0.242/drex/utils/reliability/utils.py` & `drex-0.0.243/drex/utils/reliability/utils.py`

 * *Files identical despite different names*

### Comparing `drex-0.0.242/drex/utils/tool_functions.py` & `drex-0.0.243/drex/utils/tool_functions.py`

 * *Files identical despite different names*

### Comparing `drex-0.0.242/drex.egg-info/PKG-INFO` & `drex-0.0.243/drex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drex
-Version: 0.0.242
+Version: 0.0.243
 Summary: DRex package
 Author-email: "Maxime, Dante, Haochen" <dantsanc@pa.uc3m.es>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `drex-0.0.242/drex.egg-info/SOURCES.txt` & `drex-0.0.243/drex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drex-0.0.242/pyproject.toml` & `drex-0.0.243/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=64.0", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "drex"
-version = "0.0.242"
+version = "0.0.243"
 authors = [
   { name="Maxime, Dante, Haochen", email="dantsanc@pa.uc3m.es" },
 ]
 description = "DRex package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `drex-0.0.242/test/drex-test.py` & `drex-0.0.243/test/drex-test.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 file_size = 300
 
 # Test for invalid values
 if (file_size <= 0 or number_of_nodes < 3):
 	print("ERROR: invalid value for file_size and/or number_of_nodes")
 	exit(1)
 
-#k = 2
 for i in range(3, number_of_nodes):
 	print(i,i-2,replication_and_chuncking_time(i, 2, file_size, bandwidths[:i], real_records))
 
 # Algorithm 1
 # Time for 10 nodes: 0 seconds
 # Time for 100 nodes: 0 seconds
 # Time for 1000 nodes: 11 seconds
```

