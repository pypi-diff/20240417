# Comparing `tmp/editdistpy-0.1.3rc3.tar.gz` & `tmp/editdistpy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "editdistpy-0.1.3rc3.tar", last modified: Sun Nov 28 03:00:26 2021, max compression
+gzip compressed data, was "editdistpy-0.1.4.tar", last modified: Wed Apr 17 14:01:02 2024, max compression
```

## Comparing `editdistpy-0.1.3rc3.tar` & `editdistpy-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-28 03:00:26.345276 editdistpy-0.1.3rc3/
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2021-11-28 03:00:25.000000 editdistpy-0.1.3rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-11-28 03:00:25.000000 editdistpy-0.1.3rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5556 2021-11-28 03:00:26.341276 editdistpy-0.1.3rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3359 2021-11-28 03:00:25.000000 editdistpy-0.1.3rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-28 03:00:26.341276 editdistpy-0.1.3rc3/editdistpy/
--rw-r--r--   0 runner    (1001) docker     (121)     4872 2021-11-28 03:00:25.000000 editdistpy-0.1.3rc3/editdistpy/_damerau_osa.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      654 2021-11-28 03:00:25.000000 editdistpy-0.1.3rc3/editdistpy/_damerau_osa.hpp
--rw-r--r--   0 runner    (1001) docker     (121)      535 2021-11-28 03:00:25.000000 editdistpy-0.1.3rc3/editdistpy/_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      311 2021-11-28 03:00:25.000000 editdistpy-0.1.3rc3/editdistpy/_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     2958 2021-11-28 03:00:25.000000 editdistpy-0.1.3rc3/editdistpy/_levenshtein.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      654 2021-11-28 03:00:25.000000 editdistpy-0.1.3rc3/editdistpy/_levenshtein.hpp
--rw-r--r--   0 runner    (1001) docker     (121)   139271 2021-11-28 03:00:25.000000 editdistpy-0.1.3rc3/editdistpy/damerau_osa.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      947 2021-11-28 03:00:25.000000 editdistpy-0.1.3rc3/editdistpy/damerau_osa.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      288 2021-11-28 03:00:25.000000 editdistpy-0.1.3rc3/editdistpy/def.hpp
--rw-r--r--   0 runner    (1001) docker     (121)   139271 2021-11-28 03:00:25.000000 editdistpy-0.1.3rc3/editdistpy/levenshtein.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      947 2021-11-28 03:00:25.000000 editdistpy-0.1.3rc3/editdistpy/levenshtein.pyx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-28 03:00:26.341276 editdistpy-0.1.3rc3/editdistpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5556 2021-11-28 03:00:26.000000 editdistpy-0.1.3rc3/editdistpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      509 2021-11-28 03:00:26.000000 editdistpy-0.1.3rc3/editdistpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-28 03:00:26.000000 editdistpy-0.1.3rc3/editdistpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-28 03:00:26.000000 editdistpy-0.1.3rc3/editdistpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-11-28 03:00:26.000000 editdistpy-0.1.3rc3/editdistpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      117 2021-11-28 03:00:25.000000 editdistpy-0.1.3rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-28 03:00:26.345276 editdistpy-0.1.3rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5245 2021-11-28 03:00:25.000000 editdistpy-0.1.3rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:01:02.398275 editdistpy-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-17 14:00:56.000000 editdistpy-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-17 14:00:56.000000 editdistpy-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-04-17 14:01:02.398275 editdistpy-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5346 2024-04-17 14:00:56.000000 editdistpy-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:01:02.394275 editdistpy-0.1.4/editdistpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-04-17 14:00:56.000000 editdistpy-0.1.4/editdistpy/_damerau_osa.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-17 14:00:56.000000 editdistpy-0.1.4/editdistpy/_damerau_osa.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-17 14:00:56.000000 editdistpy-0.1.4/editdistpy/_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-17 14:00:56.000000 editdistpy-0.1.4/editdistpy/_levenshtein.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-17 14:00:56.000000 editdistpy-0.1.4/editdistpy/_levenshtein.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)   272139 2024-04-17 14:01:01.000000 editdistpy-0.1.4/editdistpy/damerau_osa.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-17 14:00:56.000000 editdistpy-0.1.4/editdistpy/damerau_osa.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-17 14:00:56.000000 editdistpy-0.1.4/editdistpy/def.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)   272139 2024-04-17 14:01:01.000000 editdistpy-0.1.4/editdistpy/levenshtein.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-17 14:00:56.000000 editdistpy-0.1.4/editdistpy/levenshtein.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:01:02.398275 editdistpy-0.1.4/editdistpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-04-17 14:01:02.000000 editdistpy-0.1.4/editdistpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-17 14:01:02.000000 editdistpy-0.1.4/editdistpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 14:01:02.000000 editdistpy-0.1.4/editdistpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 14:01:01.000000 editdistpy-0.1.4/editdistpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-17 14:01:02.000000 editdistpy-0.1.4/editdistpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-17 14:00:56.000000 editdistpy-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 14:01:02.398275 editdistpy-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-17 14:00:56.000000 editdistpy-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:01:02.398275 editdistpy-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-17 14:00:56.000000 editdistpy-0.1.4/tests/test_damerau_osa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-17 14:00:56.000000 editdistpy-0.1.4/tests/test_levenshtein.py
```

### Comparing `editdistpy-0.1.3rc3/LICENSE` & `editdistpy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `editdistpy-0.1.3rc3/editdistpy/_damerau_osa.cpp` & `editdistpy-0.1.4/editdistpy/_damerau_osa.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,98 @@
 #include "_damerau_osa.hpp"
 
+#include <algorithm>
+#include <cstdlib>
+
 #include "_helpers.hpp"
 
 const int kSpace = 32;
 
 int Distance(
-    const int* string_1
-  , const int* string_2
-  , const int string_len_1
-  , const int string_len_2
-  , const int64_t max_distance)
+    const int* pString1
+  , const int* pString2
+  , int stringLen1
+  , int stringLen2
+  , const int64_t maxDistance)
 {
-  int len_1 = string_len_1;
-  int len_2 = string_len_2;
-  int start;
-  PrefixSuffixPrep(string_1, string_2, len_1, len_2, start);
-  if (len_1 == 0) {
-    return len_2 <= max_distance ? len_2 : -1;
-  }
-  if (max_distance < len_2) {
-    return InternalDistanceMax(
-        string_1,
-        string_2,
-        len_1,
-        len_2,
-        start,
-        max_distance);
+  if (pString1 == NULL || pString2 == NULL) {
+    return NullDistanceResults(pString1, pString2, stringLen1, stringLen2,
+        maxDistance);
+  }
+  if (maxDistance <= 0) {
+    return ZeroDistanceResults(pString1, pString2, stringLen1, stringLen2);
+  }
+  if (stringLen2 - stringLen1 > maxDistance
+      || stringLen2 - stringLen1 < -maxDistance) {
+    return -1;
+  }
+  if (stringLen1 > stringLen2) {
+    std::swap(pString1, pString2);
+    std::swap(stringLen1, stringLen2);
+  }
+  // Trim suffix
+  while (stringLen1 != 0
+      && pString1[~-stringLen1] == pString2[~-stringLen2]) {
+    --stringLen1;
+    --stringLen2;
+  }
+  if (stringLen1 == 0) {
+    return stringLen2 <= maxDistance ? stringLen2 : -1;
+  }
+  // Trim prefix
+  int start = 0;
+  while (start != stringLen1 && pString1[start] == pString2[start]) {
+    ++start;
+  }
+  if (start != 0) {
+    stringLen1 -= start;
+    stringLen2 -= start;
+  }
+  if (stringLen1 == 0) {
+    return stringLen2 <= maxDistance ? stringLen2 : -1;
+  }
+  if (maxDistance < stringLen2) {
+    return InternalDistanceMax(pString1, pString2, stringLen1, stringLen2,
+        start, maxDistance);
   }
-  return InternalDistance(string_1, string_2, len_1, len_2, start);
+  return InternalDistance(pString1, pString2, stringLen1, stringLen2, start);
 }
 
 int InternalDistance(
-    const int* string_1
-  , const int* string_2
-  , const int len_1
-  , const int len_2
+    const int* pString1
+  , const int* pString2
+  , const int len1
+  , const int len2
   , const int start)
 {
-  int* prev_char_1_costs = new int[len_2];
-  int* char_1_costs = new int[len_2];
-  for (int i = 0; i < len_2; ++i) {
-    prev_char_1_costs[i] = 0;
-    char_1_costs[i] = i + 1;
+  int* p_prev_char_1_costs = (int*)calloc(len2, sizeof(int));
+  int* p_char_1_costs = (int*)malloc(len2 * sizeof(int));
+  for (int i = 0; i < len2; ++i) {
+    p_char_1_costs[i] = i + 1;
   }
   int char_1 = kSpace;
   int current_cost = 0;
-  for (int i = 0; i < len_1; ++i) {
+  for (int i = 0; i < len1; ++i) {
     const int prev_char_1 = char_1;
-    char_1 = string_1[start + i];
+    char_1 = pString1[start + i];
     int char_2 = kSpace;
     int above_char_cost = i;
     int left_char_cost = i;
     int next_trans_cost = 0;
-    for (int j = 0; j < len_2; ++j) {
+    for (int j = 0; j < len2; ++j) {
       const int this_trans_cost = next_trans_cost;
-      next_trans_cost = prev_char_1_costs[j];
+      next_trans_cost = p_prev_char_1_costs[j];
       // cost of diagonal (substitution)
       current_cost = left_char_cost;
-      prev_char_1_costs[j] = left_char_cost;
+      p_prev_char_1_costs[j] = left_char_cost;
       // left now equals current cost (which will be diagonal at next
       // iteration)
-      left_char_cost = char_1_costs[j];
+      left_char_cost = p_char_1_costs[j];
       const int prev_char_2 = char_2;
-      char_2 = string_2[start + j];
+      char_2 = pString2[start + j];
       if (char_1 != char_2) {
         // substitution if neither of two conditions below
         if (above_char_cost < current_cost) {
           current_cost = above_char_cost;
         }
         if (left_char_cost < current_cost) {
           current_cost = left_char_cost;
@@ -78,69 +104,68 @@
             && prev_char_1 == char_2
             && this_trans_cost + 1 < current_cost) {
           // transposition
           current_cost = this_trans_cost + 1;
         }
       }
       above_char_cost = current_cost;
-      char_1_costs[j] = current_cost;
+      p_char_1_costs[j] = current_cost;
     }
   }
-  delete[] prev_char_1_costs;
-  delete[] char_1_costs;
+  free(p_prev_char_1_costs);
+  free(p_char_1_costs);
   return current_cost;
 }
 
 int InternalDistanceMax(
-    const int* string_1
-  , const int* string_2
-  , const int len_1
-  , const int len_2
+    const int* pString1
+  , const int* pString2
+  , const int len1
+  , const int len2
   , const int start
-  , const int64_t max_distance)
+  , const int64_t maxDistance)
 {
-  int* prev_char_1_costs = new int[len_2];
-  int* char_1_costs = new int[len_2];
-  for (int i = 0; i < len_2; ++i) {
-    prev_char_1_costs[i] = 0;
-    char_1_costs[i] = i + 1;
+  int* p_prev_char_1_costs = (int*)calloc(len2, sizeof(int));
+  int* p_char_1_costs = (int*)malloc(len2 * sizeof(int));
+  for (int i = 0; i < len2; ++i) {
+    p_char_1_costs[i] = i + 1;
   }
-  const int len_diff = len_2 - len_1;
-  const int64_t j_start_offset = max_distance - len_diff;
+  const int len_diff = len2 - len1;
+  const int64_t j_start_offset = maxDistance - len_diff;
   int j_start = 0;
-  int64_t j_end = max_distance;
+  int64_t j_end = maxDistance;
   int char_1 = kSpace;
   int current_cost = 0;
-  for (int i = 0; i < len_1; ++i) {
+  for (int i = 0; i < len1; ++i) {
     const int prev_char_1 = char_1;
-    char_1 = string_1[start + i];
+    char_1 = pString1[start + i];
     int char_2 = kSpace;
     int above_char_cost = i;
     int left_char_cost = i;
     int next_trans_cost = 0;
-    // no need to look beyond window of lower right diagonal - max_distance
+    // no need to look beyond window of lower right diagonal - maxDistance
     // cells (lower right diag is i - len_diff) and the upper left diagonal
-    // + max_distance cells (upper left is i)
+    // + maxDistance cells (upper left is i)
     if (i > j_start_offset) {
       ++j_start;
     }
-    if (j_end < len_2) {
+    if (j_end < len2) {
       ++j_end;
     }
     for (int j = j_start; j < j_end; ++j) {
       const int this_trans_cost = next_trans_cost;
-      next_trans_cost = prev_char_1_costs[j];
+      next_trans_cost = p_prev_char_1_costs[j];
       // cost of diagonal (substitution)
       current_cost = left_char_cost;
-      prev_char_1_costs[j] = left_char_cost;
+      p_prev_char_1_costs[j] = left_char_cost;
       // left not equals current cost (which will be diagonal at next
       // iteration)
-      left_char_cost = char_1_costs[j];
+      left_char_cost = p_char_1_costs[j];
       const int prev_char_2 = char_2;
-      char_2 = string_2[start + j];
+      char_2 = pString2[start + j];
       if (char_1 != char_2) {
         // substitution if neither of two conditions below
         if (above_char_cost < current_cost) {
           current_cost = above_char_cost;
         }
         if (left_char_cost < current_cost) {
           current_cost = left_char_cost;
@@ -152,19 +177,19 @@
             && prev_char_1 == char_2
             && this_trans_cost + 1 < current_cost) {
           // transposition
           current_cost = this_trans_cost + 1;
         }
       }
       above_char_cost = current_cost;
-      char_1_costs[j] = current_cost;
+      p_char_1_costs[j] = current_cost;
     }
-    if (char_1_costs[i + len_diff] > max_distance) {
-      delete[] prev_char_1_costs;
-      delete[] char_1_costs;
+    if (p_char_1_costs[i + len_diff] > maxDistance) {
+      free(p_prev_char_1_costs);
+      free(p_char_1_costs);
       return -1;
     }
   }
-  delete[] prev_char_1_costs;
-  delete[] char_1_costs;
-  return current_cost <= max_distance ? current_cost : -1;
+  free(p_prev_char_1_costs);
+  free(p_char_1_costs);
+  return current_cost <= maxDistance ? current_cost : -1;
 }
```

### Comparing `editdistpy-0.1.3rc3/editdistpy/_damerau_osa.hpp` & `editdistpy-0.1.4/editdistpy/_damerau_osa.hpp`

 * *Files 25% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 #include "def.hpp"
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 int Distance(
-    const int* string_1
-  , const int* string_2
-  , const int string_len_1
-  , const int string_len_2
-  , const int64_t max_distance);
+    const int* pString1
+  , const int* pString2
+  , int stringLen1
+  , int stringLen2
+  , const int64_t maxDistance);
 
 int InternalDistance(
-    const int* string_1
-  , const int* string_2
-  , const int len_1
-  , const int len_2
+    const int* pString1
+  , const int* pString2
+  , const int len1
+  , const int len2
   , const int start);
 
 int InternalDistanceMax(
-    const int* string_1
-  , const int* string_2
-  , const int len_1
-  , const int len_2
+    const int* pString1
+  , const int* pString2
+  , const int len1
+  , const int len2
   , const int start
-  , const int64_t max_distance);
+  , const int64_t maxDistance);
 
 #ifdef __cplusplus
 }
 #endif
 
 #endif  // EDITDISTPY__DAMERAU_OSA_HPP_
```

### Comparing `editdistpy-0.1.3rc3/editdistpy/_levenshtein.cpp` & `editdistpy-0.1.4/editdistpy/_levenshtein.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,116 +1,143 @@
 #include "_levenshtein.hpp"
 
+#include <algorithm>
+#include <cstdlib>
+
 #include "_helpers.hpp"
 
 int Distance(
-    const int* string_1
-  , const int* string_2
-  , const int string_len_1
-  , const int string_len_2
-  , const int64_t max_distance)
+    const int* pString1
+  , const int* pString2
+  , int stringLen1
+  , int stringLen2
+  , const int64_t maxDistance)
 {
-  int len_1 = string_len_1;
-  int len_2 = string_len_2;
-  int start;
-  PrefixSuffixPrep(string_1, string_2, len_1, len_2, start);
-  if (len_1 == 0) {
-    return len_2 <= max_distance ? len_2 : -1;
-  }
-  if (max_distance < len_2) {
-    return InternalDistanceMax(
-        string_1,
-        string_2,
-        len_1,
-        len_2,
-        start,
-        max_distance);
+  if (pString1 == NULL || pString2 == NULL) {
+    return NullDistanceResults(pString1, pString2, stringLen1, stringLen2,
+        maxDistance);
+  }
+  if (maxDistance <= 0) {
+    return ZeroDistanceResults(pString1, pString2, stringLen1, stringLen2);
+  }
+  if (stringLen2 - stringLen1 > maxDistance
+      || stringLen2 - stringLen1 < -maxDistance) {
+    return -1;
+  }
+  if (stringLen1 > stringLen2) {
+    std::swap(pString1, pString2);
+    std::swap(stringLen1, stringLen2);
+  }
+  // Trim suffix
+  while (stringLen1 != 0
+      && pString1[~-stringLen1] == pString2[~-stringLen2]) {
+    --stringLen1;
+    --stringLen2;
+  }
+  if (stringLen1 == 0) {
+    return stringLen2 <= maxDistance ? stringLen2 : -1;
+  }
+  // Trim prefix
+  int start = 0;
+  while (start != stringLen1 && pString1[start] == pString2[start]) {
+    ++start;
+  }
+  if (start != 0) {
+    stringLen1 -= start;
+    stringLen2 -= start;
+  }
+  if (stringLen1 == 0) {
+    return stringLen2 <= maxDistance ? stringLen2 : -1;
+  }
+  if (maxDistance < stringLen2) {
+    return InternalDistanceMax(pString1, pString2, stringLen1, stringLen2,
+        start, maxDistance);
   }
-  return InternalDistance(string_1, string_2, len_1, len_2, start);
+  return InternalDistance(pString1, pString2, stringLen1, stringLen2, start);
 }
 
 int InternalDistance(
-    const int* string_1
-  , const int* string_2
-  , const int len_1
-  , const int len_2
+    const int* pString1
+  , const int* pString2
+  , const int len1
+  , const int len2
   , const int start)
 {
-  int* char_1_costs = new int[len_2];
-  for (int i = 0; i < len_2; ++i) {
-    char_1_costs[i] = i + 1;
+  int* p_char_1_costs = (int*)malloc(len2 * sizeof(int));
+  for (int i = 0; i < len2; ++i) {
+    p_char_1_costs[i] = i + 1;
   }
   int current_cost = 0;
-  for (int i = 0; i < len_1; ++i) {
+  for (int i = 0; i < len1; ++i) {
     int above_char_cost = i;
     int left_char_cost = i;
-    const int char_1 = string_1[start + i];
-    for (int j = 0; j < len_2; ++j) {
+    const int char_1 = pString1[start + i];
+    for (int j = 0; j < len2; ++j) {
       current_cost = left_char_cost;
-      left_char_cost = char_1_costs[j];
-      if (char_1 != string_2[start + j]) {
+      left_char_cost = p_char_1_costs[j];
+      if (char_1 != pString2[start + j]) {
         if (above_char_cost < current_cost) {
           current_cost = above_char_cost;
         }
         if (left_char_cost < current_cost) {
           current_cost = left_char_cost;
         }
         ++current_cost;
       }
       above_char_cost = current_cost;
-      char_1_costs[j] = current_cost;
+      p_char_1_costs[j] = current_cost;
     }
   }
-  delete[] char_1_costs;
+  free(p_char_1_costs);
   return current_cost;
 }
 
 int InternalDistanceMax(
-    const int* string_1
-  , const int* string_2
-  , const int len_1
-  , const int len_2
+    const int* pString1
+  , const int* pString2
+  , const int len1
+  , const int len2
   , const int start
-  , const int64_t max_distance)
+  , const int64_t maxDistance)
 {
-  int* char_1_costs = new int[len_2];
-  for (int i = 0; i < len_2; ++i) {
-    char_1_costs[i] = i < max_distance ? i + 1 : max_distance + 1;
+  int* p_char_1_costs = (int*)malloc(len2 * sizeof(int));
+  for (int i = 0; i < len2; ++i) {
+    p_char_1_costs[i] = i < maxDistance ? i + 1 : maxDistance + 1;
   }
-  const int len_diff = len_2 - len_1;
-  const int64_t j_start_offset = max_distance - len_diff;
+  const int len_diff = len2 - len1;
+  const int64_t j_start_offset = maxDistance - len_diff;
   int j_start = 0;
-  int64_t j_end = max_distance;
+  int64_t j_end = maxDistance;
   int current_cost = 0;
-  for (int i = 0; i < len_1; ++i) {
-    int char_1 = string_1[start + i];
+  for (int i = 0; i < len1; ++i) {
+    int char_1 = pString1[start + i];
     int above_char_cost = i;
     int prev_char_1_cost = i;
     if (i > j_start_offset) {
       ++j_start;
     }
-    if (j_end < len_2) {
+    if (j_end < len2) {
       ++j_end;
     }
     for (int j = j_start; j < j_end; ++j) {
       current_cost = prev_char_1_cost;
-      prev_char_1_cost = char_1_costs[j];
-      if (char_1 != string_2[start + j]) {
+      prev_char_1_cost = p_char_1_costs[j];
+      if (char_1 != pString2[start + j]) {
         if (above_char_cost < current_cost) {
           current_cost = above_char_cost;
         }
         if (prev_char_1_cost < current_cost) {
           current_cost = prev_char_1_cost;
         }
         ++current_cost;
       }
       above_char_cost = current_cost;
-      char_1_costs[j] = current_cost;
+      p_char_1_costs[j] = current_cost;
     }
-    if (char_1_costs[i + len_diff] > max_distance) {
-      delete[] char_1_costs;
+    if (p_char_1_costs[i + len_diff] > maxDistance) {
+      free(p_char_1_costs);
       return -1;
     }
   }
-  delete[] char_1_costs;
-  return current_cost <= max_distance ? current_cost : -1;
+  free(p_char_1_costs);
+  return current_cost <= maxDistance ? current_cost : -1;
 }
```

### Comparing `editdistpy-0.1.3rc3/editdistpy/damerau_osa.pyx` & `editdistpy-0.1.4/editdistpy/levenshtein.pyx`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 # distutils: language = c++
-# distutils: sources = editdistpy/_damerau_osa.cpp
+# distutils: sources = editdistpy/_levenshtein.cpp
 # cython: language_level=3
 
 from libc.stdlib cimport malloc, free
 
-cdef extern from "_damerau_osa.hpp":
+cdef extern from "_levenshtein.hpp":
     ctypedef int int64_t
     int Distance(
-        const int* string_1,
-        const int* string_2,
-        const int string_len_1,
-        const int string_len_2,
-        const int64_t max_distance,
+        const int* pString1,
+        const int* pString2,
+        int stringLen1,
+        int stringLen2,
+        const int64_t maxDistance,
     )
 
 cpdef int distance(
     object string_1,
     object string_2,
-    object max_distance
+    object max_distance,
 ) except +:
-    cdef int len_1 = len(string_1)
-    cdef int len_2 = len(string_2)
-    cdef int* c_string_1 = <int*>malloc(len_1 * sizeof(int))
-    cdef int* c_string_2 = <int*>malloc(len_2 * sizeof(int))
-    for i in range(len_1):
-        c_string_1[i] = ord(string_1[i])
-    for i in range(len_2):
-        c_string_2[i] = ord(string_2[i])
+    cdef int len_1 = 0
+    cdef int* c_string_1 = NULL
+    cdef int len_2 = 0
+    cdef int* c_string_2 = NULL
+
+    if string_1 is not None:
+        len_1 = len(string_1)
+        c_string_1 = <int*>malloc(len_1 * sizeof(int))
+        for i in range(len_1):
+            c_string_1[i] = ord(string_1[i])
+    if string_2 is not None:
+        len_2 = len(string_2)
+        c_string_2 = <int*>malloc(len_2 * sizeof(int))
+        for i in range(len_2):
+            c_string_2[i] = ord(string_2[i])
+
     dist = Distance(c_string_1, c_string_2, len_1, len_2, max_distance)
     free(c_string_1)
     free(c_string_2)
     return dist
```

### Comparing `editdistpy-0.1.3rc3/editdistpy/levenshtein.pyx` & `editdistpy-0.1.4/editdistpy/damerau_osa.pyx`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 # distutils: language = c++
-# distutils: sources = editdistpy/_levenshtein.cpp
+# distutils: sources = editdistpy/_damerau_osa.cpp
 # cython: language_level=3
 
 from libc.stdlib cimport malloc, free
 
-cdef extern from "_levenshtein.hpp":
+cdef extern from "_damerau_osa.hpp":
     ctypedef int int64_t
     int Distance(
-        const int* string_1,
-        const int* string_2,
-        const int string_len_1,
-        const int string_len_2,
-        const int64_t max_distance,
+        const int* pString1,
+        const int* pString2,
+        int stringLen1,
+        int stringLen2,
+        const int64_t maxDistance,
     )
 
 cpdef int distance(
     object string_1,
     object string_2,
-    object max_distance
+    object max_distance,
 ) except +:
-    cdef int len_1 = len(string_1)
-    cdef int len_2 = len(string_2)
-    cdef int* c_string_1 = <int*>malloc(len_1 * sizeof(int))
-    cdef int* c_string_2 = <int*>malloc(len_2 * sizeof(int))
-    for i in range(len_1):
-        c_string_1[i] = ord(string_1[i])
-    for i in range(len_2):
-        c_string_2[i] = ord(string_2[i])
+    cdef int len_1 = 0
+    cdef int* c_string_1 = NULL
+    cdef int len_2 = 0
+    cdef int* c_string_2 = NULL
+
+    if string_1 is not None:
+        len_1 = len(string_1)
+        c_string_1 = <int*>malloc(len_1 * sizeof(int))
+        for i in range(len_1):
+            c_string_1[i] = ord(string_1[i])
+    if string_2 is not None:
+        len_2 = len(string_2)
+        c_string_2 = <int*>malloc(len_2 * sizeof(int))
+        for i in range(len_2):
+            c_string_2[i] = ord(string_2[i])
+
     dist = Distance(c_string_1, c_string_2, len_1, len_2, max_distance)
     free(c_string_1)
     free(c_string_2)
     return dist
```

### Comparing `editdistpy-0.1.3rc3/setup.py` & `editdistpy-0.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 try:
     from Cython.Build import cythonize
 except ImportError:
     cythonize = None
 
 PROJ_DIR = Path(__file__).resolve().parent
 NAME = "editdistpy"
-VERSION = "0.1.3rc3"
+VERSION = "0.1.4"
 DESCRIPTION = "Fast Levenshtein and Damerau optimal string alignment algorithms."
 with open(PROJ_DIR / "README.md", "r", encoding="utf-8") as infile:
     LONG_DESCRIPTION = infile.read()
 LONG_DESCRIPTION_CONTENT_TYPE = "text/markdown"
 AUTHOR = "mmb L"
 URL = "https://github.com/mammothb/editdistpy"
 LICENSE = "MIT"
@@ -84,27 +84,25 @@
     extra_link_args = ["-stdlib=libc++"]
 
 ext_modules = [
     Extension(
         "editdistpy.levenshtein",
         [
             "editdistpy/_levenshtein.cpp",
-            "editdistpy/_helpers.cpp",
             "editdistpy/levenshtein.pyx",
         ],
         include_dirs=["./editdistpy"],
         language="c++",
         extra_compile_args=extra_compile_args,
         extra_link_args=extra_link_args,
     ),
     Extension(
         "editdistpy.damerau_osa",
         [
             "editdistpy/_damerau_osa.cpp",
-            "editdistpy/_helpers.cpp",
             "editdistpy/damerau_osa.pyx",
         ],
         include_dirs=["./editdistpy"],
         language="c++",
         extra_compile_args=extra_compile_args,
         extra_link_args=extra_link_args,
     ),
@@ -139,18 +137,20 @@
         "Operating System :: POSIX",
         "Operating System :: Unix",
         "Operating System :: MacOS",
         "Programming Language :: C++",
         "Programming Language :: Cython",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
     ],
     zip_safe=False,
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     include_package_data=True,
     package_dir={"editdistpy": "editdistpy"},
     ext_modules=ext_modules,
 )
```

