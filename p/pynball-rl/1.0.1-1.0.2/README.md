# Comparing `tmp/pynball_rl-1.0.1.tar.gz` & `tmp/pynball_rl-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynball_rl-1.0.1.tar", max compression
+gzip compressed data, was "pynball_rl-1.0.2.tar", max compression
```

## Comparing `pynball_rl-1.0.1.tar` & `pynball_rl-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1060 2024-03-13 16:31:36.208873 pynball_rl-1.0.1/LICENSE
--rw-r--r--   0        0        0     2558 2024-04-05 10:05:51.034931 pynball_rl-1.0.1/README.md
--rw-r--r--   0        0        0      185 2024-03-13 16:44:03.303221 pynball_rl-1.0.1/pynball_rl/__init__.py
--rw-r--r--   0        0        0     1595 2024-03-14 17:16:25.740448 pynball_rl-1.0.1/pynball_rl/__main__.py
--rw-r--r--   0        0        0     2826 2024-03-13 16:50:10.446528 pynball_rl-1.0.1/pynball_rl/ball.py
--rw-r--r--   0        0        0      580 2024-04-04 10:09:25.854283 pynball_rl-1.0.1/pynball_rl/configs/corridor_2d_config.toml
--rw-r--r--   0        0        0     1274 2024-04-05 10:42:13.719149 pynball_rl-1.0.1/pynball_rl/configs/easy_2d_config.toml
--rw-r--r--   0        0        0     1239 2024-04-05 09:17:56.678149 pynball_rl-1.0.1/pynball_rl/configs/easy_config.toml
--rw-r--r--   0        0        0     1036 2024-04-05 09:18:04.665429 pynball_rl-1.0.1/pynball_rl/configs/four_rooms_2d_config.toml
--rw-r--r--   0        0        0     2413 2024-04-05 09:18:12.333930 pynball_rl-1.0.1/pynball_rl/configs/hard_config.toml
--rw-r--r--   0        0        0      657 2024-04-05 09:18:18.029280 pynball_rl-1.0.1/pynball_rl/configs/very_easy_config.toml
--rw-r--r--   0        0        0     1015 2024-03-13 16:50:15.675372 pynball_rl-1.0.1/pynball_rl/obstacle.py
--rw-r--r--   0        0        0     3631 2024-03-13 16:31:36.210369 pynball_rl-1.0.1/pynball_rl/point.py
--rw-r--r--   0        0        0     8455 2024-04-08 11:46:01.738264 pynball_rl-1.0.1/pynball_rl/polygon_obstacle.py
--rw-r--r--   0        0        0     7274 2024-04-05 09:50:05.254739 pynball_rl-1.0.1/pynball_rl/pynball_env.py
--rw-r--r--   0        0        0     1420 2024-03-26 11:41:56.589854 pynball_rl-1.0.1/pynball_rl/rollout.py
--rw-r--r--   0        0        0     1672 2024-03-13 16:50:35.717816 pynball_rl-1.0.1/pynball_rl/target.py
--rw-r--r--   0        0        0     1104 2024-03-25 15:38:34.521815 pynball_rl-1.0.1/pynball_rl/utils.py
--rw-r--r--   0        0        0     2702 2024-03-13 16:50:41.622167 pynball_rl-1.0.1/pynball_rl/viewer.py
--rw-r--r--   0        0        0      737 2024-04-09 12:03:37.271618 pynball_rl-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3379 1970-01-01 00:00:00.000000 pynball_rl-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-03-13 16:31:36.208873 pynball_rl-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2558 2024-04-05 10:05:51.034931 pynball_rl-1.0.2/README.md
+-rw-r--r--   0        0        0      185 2024-03-13 16:44:03.303221 pynball_rl-1.0.2/pynball_rl/__init__.py
+-rw-r--r--   0        0        0     1595 2024-03-14 17:16:25.740448 pynball_rl-1.0.2/pynball_rl/__main__.py
+-rw-r--r--   0        0        0     2826 2024-03-13 16:50:10.446528 pynball_rl-1.0.2/pynball_rl/ball.py
+-rw-r--r--   0        0        0      580 2024-04-04 10:09:25.854283 pynball_rl-1.0.2/pynball_rl/configs/corridor_2d_config.toml
+-rw-r--r--   0        0        0     1274 2024-04-05 10:42:13.719149 pynball_rl-1.0.2/pynball_rl/configs/easy_2d_config.toml
+-rw-r--r--   0        0        0     1239 2024-04-05 09:17:56.678149 pynball_rl-1.0.2/pynball_rl/configs/easy_config.toml
+-rw-r--r--   0        0        0     1036 2024-04-05 09:18:04.665429 pynball_rl-1.0.2/pynball_rl/configs/four_rooms_2d_config.toml
+-rw-r--r--   0        0        0     2412 2024-04-17 09:10:36.486543 pynball_rl-1.0.2/pynball_rl/configs/hard_2d_config.toml
+-rw-r--r--   0        0        0     2413 2024-04-05 09:18:12.333930 pynball_rl-1.0.2/pynball_rl/configs/hard_config.toml
+-rw-r--r--   0        0        0      657 2024-04-05 09:18:18.029280 pynball_rl-1.0.2/pynball_rl/configs/very_easy_config.toml
+-rw-r--r--   0        0        0     1015 2024-03-13 16:50:15.675372 pynball_rl-1.0.2/pynball_rl/obstacle.py
+-rw-r--r--   0        0        0     3631 2024-03-13 16:31:36.210369 pynball_rl-1.0.2/pynball_rl/point.py
+-rw-r--r--   0        0        0     8455 2024-04-08 11:46:01.738264 pynball_rl-1.0.2/pynball_rl/polygon_obstacle.py
+-rw-r--r--   0        0        0     7274 2024-04-05 09:50:05.254739 pynball_rl-1.0.2/pynball_rl/pynball_env.py
+-rw-r--r--   0        0        0     1420 2024-03-26 11:41:56.589854 pynball_rl-1.0.2/pynball_rl/rollout.py
+-rw-r--r--   0        0        0     1672 2024-03-13 16:50:35.717816 pynball_rl-1.0.2/pynball_rl/target.py
+-rw-r--r--   0        0        0     1104 2024-03-25 15:38:34.521815 pynball_rl-1.0.2/pynball_rl/utils.py
+-rw-r--r--   0        0        0     2702 2024-03-13 16:50:41.622167 pynball_rl-1.0.2/pynball_rl/viewer.py
+-rw-r--r--   0        0        0      737 2024-04-17 09:21:27.010896 pynball_rl-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3379 1970-01-01 00:00:00.000000 pynball_rl-1.0.2/PKG-INFO
```

### Comparing `pynball_rl-1.0.1/LICENSE` & `pynball_rl-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pynball_rl-1.0.1/README.md` & `pynball_rl-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pynball_rl-1.0.1/pynball_rl/__main__.py` & `pynball_rl-1.0.2/pynball_rl/__main__.py`

 * *Files identical despite different names*

### Comparing `pynball_rl-1.0.1/pynball_rl/ball.py` & `pynball_rl-1.0.2/pynball_rl/ball.py`

 * *Files identical despite different names*

### Comparing `pynball_rl-1.0.1/pynball_rl/configs/corridor_2d_config.toml` & `pynball_rl-1.0.2/pynball_rl/configs/corridor_2d_config.toml`

 * *Files identical despite different names*

### Comparing `pynball_rl-1.0.1/pynball_rl/configs/easy_2d_config.toml` & `pynball_rl-1.0.2/pynball_rl/configs/easy_2d_config.toml`

 * *Files identical despite different names*

### Comparing `pynball_rl-1.0.1/pynball_rl/configs/easy_config.toml` & `pynball_rl-1.0.2/pynball_rl/configs/easy_config.toml`

 * *Files identical despite different names*

### Comparing `pynball_rl-1.0.1/pynball_rl/configs/four_rooms_2d_config.toml` & `pynball_rl-1.0.2/pynball_rl/configs/four_rooms_2d_config.toml`

 * *Files identical despite different names*

### Comparing `pynball_rl-1.0.1/pynball_rl/configs/hard_config.toml` & `pynball_rl-1.0.2/pynball_rl/configs/hard_config.toml`

 * *Files identical despite different names*

### Comparing `pynball_rl-1.0.1/pynball_rl/configs/very_easy_config.toml` & `pynball_rl-1.0.2/pynball_rl/configs/very_easy_config.toml`

 * *Files identical despite different names*

### Comparing `pynball_rl-1.0.1/pynball_rl/obstacle.py` & `pynball_rl-1.0.2/pynball_rl/obstacle.py`

 * *Files identical despite different names*

### Comparing `pynball_rl-1.0.1/pynball_rl/point.py` & `pynball_rl-1.0.2/pynball_rl/point.py`

 * *Files identical despite different names*

### Comparing `pynball_rl-1.0.1/pynball_rl/polygon_obstacle.py` & `pynball_rl-1.0.2/pynball_rl/polygon_obstacle.py`

 * *Files identical despite different names*

### Comparing `pynball_rl-1.0.1/pynball_rl/pynball_env.py` & `pynball_rl-1.0.2/pynball_rl/pynball_env.py`

 * *Files identical despite different names*

### Comparing `pynball_rl-1.0.1/pynball_rl/rollout.py` & `pynball_rl-1.0.2/pynball_rl/rollout.py`

 * *Files identical despite different names*

### Comparing `pynball_rl-1.0.1/pynball_rl/target.py` & `pynball_rl-1.0.2/pynball_rl/target.py`

 * *Files identical despite different names*

### Comparing `pynball_rl-1.0.1/pynball_rl/utils.py` & `pynball_rl-1.0.2/pynball_rl/utils.py`

 * *Files identical despite different names*

### Comparing `pynball_rl-1.0.1/pynball_rl/viewer.py` & `pynball_rl-1.0.2/pynball_rl/viewer.py`

 * *Files identical despite different names*

### Comparing `pynball_rl-1.0.1/pyproject.toml` & `pynball_rl-1.0.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pynball-rl"
-version = "1.0.1"
+version = "1.0.2"
 description = "A python implementation of the classic reinforcement learning domain pinball: http://irl.cs.brown.edu/pinball/"
 license = "MIT"
 authors = ["Tom Smith <tmssmith@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/tmssmith/pynball-rl"
 exclude = ["./tests/*"]
 include = ["./pynball_rl/configs/*"]
```

### Comparing `pynball_rl-1.0.1/PKG-INFO` & `pynball_rl-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynball-rl
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python implementation of the classic reinforcement learning domain pinball: http://irl.cs.brown.edu/pinball/
 Home-page: https://github.com/tmssmith/pynball-rl
 License: MIT
 Author: Tom Smith
 Author-email: tmssmith@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

