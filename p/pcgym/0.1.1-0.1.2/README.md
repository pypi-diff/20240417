# Comparing `tmp/pcgym-0.1.1.tar.gz` & `tmp/pcgym-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcgym-0.1.1.tar", last modified: Wed Apr 17 10:40:35 2024, max compression
+gzip compressed data, was "pcgym-0.1.2.tar", last modified: Wed Apr 17 10:50:15 2024, max compression
```

## Comparing `pcgym-0.1.1.tar` & `pcgym-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 10:40:35.742610 pcgym-0.1.1/
--rw-rw-rw-   0        0        0     1094 2024-03-06 13:10:13.000000 pcgym-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     6543 2024-04-17 10:40:35.741610 pcgym-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3803 2024-04-16 14:40:43.000000 pcgym-0.1.1/README.md
--rw-rw-rw-   0        0        0     1309 2024-04-17 10:40:27.000000 pcgym-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       95 2024-04-02 11:41:57.000000 pcgym-0.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 10:40:35.742610 pcgym-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-17 10:40:35.698610 pcgym-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-17 10:40:35.733648 pcgym-0.1.1/src/pcgym/
--rw-rw-rw-   0        0        0       85 2024-04-17 10:29:24.000000 pcgym-0.1.1/src/pcgym/__init__.py
--rw-rw-rw-   0        0        0     7662 2024-04-17 10:20:21.000000 pcgym-0.1.1/src/pcgym/evaluation_metrics.py
--rw-rw-rw-   0        0        0     5303 2024-04-16 13:47:20.000000 pcgym-0.1.1/src/pcgym/integrator.py
--rw-rw-rw-   0        0        0    10621 2024-04-16 13:47:20.000000 pcgym-0.1.1/src/pcgym/model_classes.py
--rw-rw-rw-   0        0        0    10748 2024-04-16 13:47:20.000000 pcgym-0.1.1/src/pcgym/oracle.py
--rw-rw-rw-   0        0        0    16946 2024-04-17 10:34:51.000000 pcgym-0.1.1/src/pcgym/pcgym.py
--rw-rw-rw-   0        0        0    12943 2024-04-17 10:29:22.000000 pcgym-0.1.1/src/pcgym/policy_evaluation.py
--rw-rw-rw-   0        0        0     1637 2024-04-17 10:31:44.000000 pcgym-0.1.1/src/pcgym/test.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:40:35.739611 pcgym-0.1.1/src/pcgym.egg-info/
--rw-rw-rw-   0        0        0     6543 2024-04-17 10:40:35.000000 pcgym-0.1.1/src/pcgym.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      492 2024-04-17 10:40:35.000000 pcgym-0.1.1/src/pcgym.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 10:40:35.000000 pcgym-0.1.1/src/pcgym.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-04-17 10:40:35.000000 pcgym-0.1.1/src/pcgym.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-17 10:40:35.000000 pcgym-0.1.1/src/pcgym.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 10:50:15.073233 pcgym-0.1.2/
+-rw-rw-rw-   0        0        0     1094 2024-03-06 13:10:13.000000 pcgym-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     6543 2024-04-17 10:50:15.071234 pcgym-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3803 2024-04-16 14:40:43.000000 pcgym-0.1.2/README.md
+-rw-rw-rw-   0        0        0     1309 2024-04-17 10:50:03.000000 pcgym-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       95 2024-04-02 11:41:57.000000 pcgym-0.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 10:50:15.073233 pcgym-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 10:50:15.034232 pcgym-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 10:50:15.064233 pcgym-0.1.2/src/pcgym/
+-rw-rw-rw-   0        0        0      129 2024-04-17 10:46:31.000000 pcgym-0.1.2/src/pcgym/__init__.py
+-rw-rw-rw-   0        0        0     7662 2024-04-17 10:20:21.000000 pcgym-0.1.2/src/pcgym/evaluation_metrics.py
+-rw-rw-rw-   0        0        0     5303 2024-04-16 13:47:20.000000 pcgym-0.1.2/src/pcgym/integrator.py
+-rw-rw-rw-   0        0        0    10621 2024-04-16 13:47:20.000000 pcgym-0.1.2/src/pcgym/model_classes.py
+-rw-rw-rw-   0        0        0    10748 2024-04-16 13:47:20.000000 pcgym-0.1.2/src/pcgym/oracle.py
+-rw-rw-rw-   0        0        0    16946 2024-04-17 10:47:07.000000 pcgym-0.1.2/src/pcgym/pcgym.py
+-rw-rw-rw-   0        0        0    12943 2024-04-17 10:29:22.000000 pcgym-0.1.2/src/pcgym/policy_evaluation.py
+-rw-rw-rw-   0        0        0     1637 2024-04-17 10:47:08.000000 pcgym-0.1.2/src/pcgym/test.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:50:15.070234 pcgym-0.1.2/src/pcgym.egg-info/
+-rw-rw-rw-   0        0        0     6543 2024-04-17 10:50:15.000000 pcgym-0.1.2/src/pcgym.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      492 2024-04-17 10:50:15.000000 pcgym-0.1.2/src/pcgym.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 10:50:15.000000 pcgym-0.1.2/src/pcgym.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-04-17 10:50:15.000000 pcgym-0.1.2/src/pcgym.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-17 10:50:15.000000 pcgym-0.1.2/src/pcgym.egg-info/top_level.txt
```

### Comparing `pcgym-0.1.1/LICENSE` & `pcgym-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.1/PKG-INFO` & `pcgym-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcgym
-Version: 0.1.1
+Version: 0.1.2
 Summary: Reinforcement learning suite of process control problems.
 Author-email: Max Bloor <max.bloor@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Maximilian Bloor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pcgym Version: 0.1.1 Summary: Reinforcement
+Metadata-Version: 2.1 Name: pcgym Version: 0.1.2 Summary: Reinforcement
 learning suite of process control problems. Author-email: Max Bloor
 gmail.com> License: MIT License Copyright (c) 2024 Maximilian Bloor Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `pcgym-0.1.1/README.md` & `pcgym-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.1/pyproject.toml` & `pcgym-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pcgym"
-version = "0.1.1"
+version = "0.1.2"
 description = "Reinforcement learning suite of process control problems."
 requires-python = "~=3.10"
 license = { file = "LICENSE" }
 readme = "README.md"
 authors = [{ name = "Max Bloor", email = "max.bloor@gmail.com" }]
 keywords = [
   "reinforcement-learning",
```

### Comparing `pcgym-0.1.1/src/pcgym/evaluation_metrics.py` & `pcgym-0.1.2/src/pcgym/evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.1/src/pcgym/integrator.py` & `pcgym-0.1.2/src/pcgym/integrator.py`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.1/src/pcgym/model_classes.py` & `pcgym-0.1.2/src/pcgym/model_classes.py`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.1/src/pcgym/oracle.py` & `pcgym-0.1.2/src/pcgym/oracle.py`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.1/src/pcgym/pcgym.py` & `pcgym-0.1.2/src/pcgym/pcgym.py`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.1/src/pcgym/policy_evaluation.py` & `pcgym-0.1.2/src/pcgym/policy_evaluation.py`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.1/src/pcgym/test.py` & `pcgym-0.1.2/src/pcgym/test.py`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.1/src/pcgym.egg-info/PKG-INFO` & `pcgym-0.1.2/src/pcgym.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcgym
-Version: 0.1.1
+Version: 0.1.2
 Summary: Reinforcement learning suite of process control problems.
 Author-email: Max Bloor <max.bloor@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Maximilian Bloor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pcgym Version: 0.1.1 Summary: Reinforcement
+Metadata-Version: 2.1 Name: pcgym Version: 0.1.2 Summary: Reinforcement
 learning suite of process control problems. Author-email: Max Bloor
 gmail.com> License: MIT License Copyright (c) 2024 Maximilian Bloor Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

