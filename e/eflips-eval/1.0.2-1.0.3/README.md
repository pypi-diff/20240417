# Comparing `tmp/eflips_eval-1.0.2.tar.gz` & `tmp/eflips_eval-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eflips_eval-1.0.2.tar", max compression
+gzip compressed data, was "eflips_eval-1.0.3.tar", max compression
```

## Comparing `eflips_eval-1.0.2.tar` & `eflips_eval-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    34260 2024-03-26 16:50:21.863844 eflips_eval-1.0.2/LICENSE.md
--rw-r--r--   0        0        0     4658 2024-03-26 16:50:21.863844 eflips_eval-1.0.2/README.md
--rw-r--r--   0        0        0        0 2024-03-26 16:50:21.863844 eflips_eval-1.0.2/eflips/eval/input/__init__.py
--rw-r--r--   0        0        0     3291 2024-03-26 16:50:21.867844 eflips_eval-1.0.2/eflips/eval/input/prepare.py
--rw-r--r--   0        0        0     1321 2024-03-26 16:50:21.867844 eflips_eval-1.0.2/eflips/eval/input/visualize.py
--rw-r--r--   0        0        0        0 2024-03-26 16:50:21.867844 eflips_eval-1.0.2/eflips/eval/output/__init__.py
--rw-r--r--   0        0        0    15846 2024-03-26 16:50:21.867844 eflips_eval-1.0.2/eflips/eval/output/prepare.py
--rw-r--r--   0        0        0    10443 2024-03-26 16:50:21.867844 eflips_eval-1.0.2/eflips/eval/output/visualize.py
--rw-r--r--   0        0        0      781 2024-03-26 16:50:21.887844 eflips_eval-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     5134 1970-01-01 00:00:00.000000 eflips_eval-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    34260 2024-04-17 13:29:32.016875 eflips_eval-1.0.3/LICENSE.md
+-rw-r--r--   0        0        0     4658 2024-04-17 13:29:32.016875 eflips_eval-1.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 13:29:32.016875 eflips_eval-1.0.3/eflips/eval/input/__init__.py
+-rw-r--r--   0        0        0     3291 2024-04-17 13:29:32.016875 eflips_eval-1.0.3/eflips/eval/input/prepare.py
+-rw-r--r--   0        0        0     1321 2024-04-17 13:29:32.016875 eflips_eval-1.0.3/eflips/eval/input/visualize.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:29:32.016875 eflips_eval-1.0.3/eflips/eval/output/__init__.py
+-rw-r--r--   0        0        0    15760 2024-04-17 13:29:32.016875 eflips_eval-1.0.3/eflips/eval/output/prepare.py
+-rw-r--r--   0        0        0    10443 2024-04-17 13:29:32.016875 eflips_eval-1.0.3/eflips/eval/output/visualize.py
+-rw-r--r--   0        0        0      781 2024-04-17 13:29:32.036875 eflips_eval-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5134 1970-01-01 00:00:00.000000 eflips_eval-1.0.3/PKG-INFO
```

### Comparing `eflips_eval-1.0.2/LICENSE.md` & `eflips_eval-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eflips_eval-1.0.2/README.md` & `eflips_eval-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `eflips_eval-1.0.2/eflips/eval/input/prepare.py` & `eflips_eval-1.0.3/eflips/eval/input/prepare.py`

 * *Files identical despite different names*

### Comparing `eflips_eval-1.0.2/eflips/eval/input/visualize.py` & `eflips_eval-1.0.3/eflips/eval/input/visualize.py`

 * *Files identical despite different names*

### Comparing `eflips_eval-1.0.2/eflips/eval/output/prepare.py` & `eflips_eval-1.0.3/eflips/eval/output/prepare.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,14 @@
         this_event_unix_times = np.array([t.timestamp() for t in this_event_times])
 
         # Validation: the timeseries should be sorted and the socs should be in the range [0, 1] and monotonically increasing
         assert all(
             this_event_times[i] <= this_event_times[i + 1]
             for i in range(len(this_event_times) - 1)
         )
-        assert all(0 <= this_event_socs[i] <= 1 for i in range(len(this_event_socs)))
         assert all(
             this_event_socs[i] <= this_event_socs[i + 1]
             for i in range(len(this_event_socs) - 1)
         )
 
         # Convert from SoC to enerhgy using the vehicle types battery capacity
         this_event_energy = (
```

### Comparing `eflips_eval-1.0.2/eflips/eval/output/visualize.py` & `eflips_eval-1.0.3/eflips/eval/output/visualize.py`

 * *Files identical despite different names*

### Comparing `eflips_eval-1.0.2/pyproject.toml` & `eflips_eval-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eflips-eval"
-version = "1.0.2"
+version = "1.0.3"
 description = ""
 authors = [
     "Ludger Heide <ludger.heide@lhtechnologies.de>",
 	"Shuyao Guo <shuyao.guo@tu-berlin.de>"
 ]
 readme = "README.md"
 packages = [{ include = "eflips/eval" }]
```

### Comparing `eflips_eval-1.0.2/PKG-INFO` & `eflips_eval-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eflips-eval
-Version: 1.0.2
+Version: 1.0.3
 Summary: 
 Author: Ludger Heide
 Author-email: ludger.heide@lhtechnologies.de
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

