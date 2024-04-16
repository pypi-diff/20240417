# Comparing `tmp/dynamic_chunks-0.0.2.tar.gz` & `tmp/dynamic_chunks-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic_chunks-0.0.2.tar", last modified: Wed Nov 15 18:27:30 2023, max compression
+gzip compressed data, was "dynamic_chunks-0.0.3.tar", last modified: Tue Apr 16 23:10:38 2024, max compression
```

## Comparing `dynamic_chunks-0.0.2.tar` & `dynamic_chunks-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 18:27:30.265991 dynamic_chunks-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 18:27:30.261991 dynamic_chunks-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 18:27:30.261991 dynamic_chunks-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2023-11-15 18:27:13.000000 dynamic_chunks-0.0.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2023-11-15 18:27:13.000000 dynamic_chunks-0.0.2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2023-11-15 18:27:13.000000 dynamic_chunks-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-15 18:27:13.000000 dynamic_chunks-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2023-11-15 18:27:30.265991 dynamic_chunks-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      854 2023-11-15 18:27:13.000000 dynamic_chunks-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 18:27:30.261991 dynamic_chunks-0.0.2/dynamic_chunks/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-11-15 18:27:13.000000 dynamic_chunks-0.0.2/dynamic_chunks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-15 18:27:30.000000 dynamic_chunks-0.0.2/dynamic_chunks/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14812 2023-11-15 18:27:13.000000 dynamic_chunks-0.0.2/dynamic_chunks/algorithms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 18:27:30.261991 dynamic_chunks-0.0.2/dynamic_chunks/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8457 2023-11-15 18:27:13.000000 dynamic_chunks-0.0.2/dynamic_chunks/tests/test_algorithms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 18:27:30.261991 dynamic_chunks-0.0.2/dynamic_chunks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2023-11-15 18:27:30.000000 dynamic_chunks-0.0.2/dynamic_chunks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      453 2023-11-15 18:27:30.000000 dynamic_chunks-0.0.2/dynamic_chunks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 18:27:30.000000 dynamic_chunks-0.0.2/dynamic_chunks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-11-15 18:27:30.000000 dynamic_chunks-0.0.2/dynamic_chunks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-15 18:27:30.000000 dynamic_chunks-0.0.2/dynamic_chunks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2023-11-15 18:27:13.000000 dynamic_chunks-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-11-15 18:27:13.000000 dynamic_chunks-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-15 18:27:30.265991 dynamic_chunks-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-11-15 18:27:13.000000 dynamic_chunks-0.0.2/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:10:38.007792 dynamic_chunks-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:10:38.003792 dynamic_chunks-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:10:38.003792 dynamic_chunks-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-16 23:10:26.000000 dynamic_chunks-0.0.3/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-16 23:10:26.000000 dynamic_chunks-0.0.3/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-16 23:10:26.000000 dynamic_chunks-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 23:10:26.000000 dynamic_chunks-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-16 23:10:38.007792 dynamic_chunks-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-16 23:10:26.000000 dynamic_chunks-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:10:38.007792 dynamic_chunks-0.0.3/dynamic_chunks/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-16 23:10:26.000000 dynamic_chunks-0.0.3/dynamic_chunks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-16 23:10:37.000000 dynamic_chunks-0.0.3/dynamic_chunks/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14815 2024-04-16 23:10:26.000000 dynamic_chunks-0.0.3/dynamic_chunks/algorithms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:10:38.007792 dynamic_chunks-0.0.3/dynamic_chunks/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-04-16 23:10:26.000000 dynamic_chunks-0.0.3/dynamic_chunks/tests/test_algorithms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:10:38.007792 dynamic_chunks-0.0.3/dynamic_chunks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-16 23:10:37.000000 dynamic_chunks-0.0.3/dynamic_chunks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-16 23:10:37.000000 dynamic_chunks-0.0.3/dynamic_chunks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 23:10:37.000000 dynamic_chunks-0.0.3/dynamic_chunks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-16 23:10:37.000000 dynamic_chunks-0.0.3/dynamic_chunks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 23:10:37.000000 dynamic_chunks-0.0.3/dynamic_chunks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-16 23:10:26.000000 dynamic_chunks-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-16 23:10:26.000000 dynamic_chunks-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 23:10:38.007792 dynamic_chunks-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-16 23:10:26.000000 dynamic_chunks-0.0.3/test-requirements.txt
```

### Comparing `dynamic_chunks-0.0.2/.github/workflows/release.yaml` & `dynamic_chunks-0.0.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `dynamic_chunks-0.0.2/.github/workflows/test.yaml` & `dynamic_chunks-0.0.3/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `dynamic_chunks-0.0.2/.gitignore` & `dynamic_chunks-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dynamic_chunks-0.0.2/LICENSE` & `dynamic_chunks-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamic_chunks-0.0.2/dynamic_chunks/algorithms.py` & `dynamic_chunks-0.0.3/dynamic_chunks/algorithms.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         dim
         for dim in target_chunks_aspect_ratio.keys()
         if dim not in target_chunks_aspect_ratio_chunked_only.keys()
     ]
     print(f"{unchunked_dims=}")
 
     possible_chunks = []
-    for dim, s in ds.dims.items():
+    for dim, s in ds.sizes.items():
         if dim in unchunked_dims:
             # Always keep this dimension unchunked
             possible_chunks.append([s])
         else:
             # Get a list of all the even divisors
             possible_chunks.append(even_divisor_chunks(s))
 
@@ -202,15 +202,15 @@
     ]
 
     # convert each combination into an array of resulting chunks per dimension, then normalize
     dims_chunked_only = list(
         target_chunks_aspect_ratio_chunked_only.keys()
     )  # the order of these does matter
 
-    shape_chunked_only = np.array([ds.dims[dim] for dim in dims_chunked_only])
+    shape_chunked_only = np.array([ds.sizes[dim] for dim in dims_chunked_only])
     ratio = [
         shape_chunked_only / np.array([c[dim] for dim in dims_chunked_only])
         for c in combinations_filtered_chunked_only
     ]
     ratio_normalized = [normalize(r) for r in ratio]
 
     # Find the 'closest' fit between normalized ratios
@@ -308,15 +308,15 @@
                 dim_length / ratio
             )  # determine the largest chunksize that would adhere to the given aspect ratio
             scaled_chunk = max(1, round(max_chunk / scale_factor))
             return scaled_chunk
 
     def scale_and_normalize_chunks(ds, target_chunks_aspect_ratio, scale_factor):
         scaled_normalized_chunks = {
-            dim: maybe_scale_chunk(ratio, scale_factor, ds.dims[dim])
+            dim: maybe_scale_chunk(ratio, scale_factor, ds.sizes[dim])
             for dim, ratio in target_chunks_aspect_ratio.items()
         }
         return scaled_normalized_chunks
 
     max_chunks = scale_and_normalize_chunks(
         ds, target_chunks_aspect_ratio, 1
     )  # largest possible chunk size for each dimension
```

### Comparing `dynamic_chunks-0.0.2/dynamic_chunks/tests/test_algorithms.py` & `dynamic_chunks-0.0.3/dynamic_chunks/tests/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `dynamic_chunks-0.0.2/pyproject.toml` & `dynamic_chunks-0.0.3/pyproject.toml`

 * *Files identical despite different names*

