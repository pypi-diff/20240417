# Comparing `tmp/how_is_the_weather-0.2.0.tar.gz` & `tmp/how_is_the_weather-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "how_is_the_weather-0.2.0.tar", max compression
+gzip compressed data, was "how_is_the_weather-0.3.0.tar", max compression
```

## Comparing `how_is_the_weather-0.2.0.tar` & `how_is_the_weather-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2024-04-16 18:26:28.954656 how_is_the_weather-0.2.0/LICENSE
--rw-r--r--   0        0        0      910 2024-04-16 18:26:28.954656 how_is_the_weather-0.2.0/README.md
--rw-r--r--   0        0        0      897 2024-04-16 18:26:28.954656 how_is_the_weather-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 18:26:28.954656 how_is_the_weather-0.2.0/src/how_is_the_weather/__init__.py
--rw-r--r--   0        0        0     1016 2024-04-16 18:26:28.954656 how_is_the_weather-0.2.0/src/how_is_the_weather/weather.py
--rw-r--r--   0        0        0     1555 1970-01-01 00:00:00.000000 how_is_the_weather-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-16 18:31:37.280422 how_is_the_weather-0.3.0/LICENSE
+-rw-r--r--   0        0        0      910 2024-04-16 18:31:37.280422 how_is_the_weather-0.3.0/README.md
+-rw-r--r--   0        0        0      955 2024-04-16 18:31:37.280422 how_is_the_weather-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 18:31:37.280422 how_is_the_weather-0.3.0/src/how_is_the_weather/__init__.py
+-rw-r--r--   0        0        0     1016 2024-04-16 18:31:37.280422 how_is_the_weather-0.3.0/src/how_is_the_weather/weather.py
+-rw-r--r--   0        0        0     1611 1970-01-01 00:00:00.000000 how_is_the_weather-0.3.0/PKG-INFO
```

### Comparing `how_is_the_weather-0.2.0/LICENSE` & `how_is_the_weather-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `how_is_the_weather-0.2.0/README.md` & `how_is_the_weather-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `how_is_the_weather-0.2.0/pyproject.toml` & `how_is_the_weather-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "how_is_the_weather"
-version = "0.2.0"
+version = "0.3.0"
 authors = [{ name = "Jim Jimbo", email = "jim377893@gmail.com" }]
 description = "A simple tool to describe weather conditions."
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -13,19 +13,20 @@
 dependencies = ["requests"]
 
 [project.scripts]
 how-is-the-weather = "how_is_the_weather.weather:main"
 
 [tool.poetry]
 name = "how-is-the-weather"
-version = "0.2.0"
+version = "0.3.0"
 description = "A simple tool to describe weather conditions"
 authors = ["Jim Jimbo <jim377893@gmail.com>"]
 license = "MIT"
 readme = "README.md"
+homepage = "https://github.com/jimbosimbo/howstheweather"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.31.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2"
```

### Comparing `how_is_the_weather-0.2.0/src/how_is_the_weather/weather.py` & `how_is_the_weather-0.3.0/src/how_is_the_weather/weather.py`

 * *Files identical despite different names*

### Comparing `how_is_the_weather-0.2.0/PKG-INFO` & `how_is_the_weather-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: how-is-the-weather
-Version: 0.2.0
+Version: 0.3.0
 Summary: A simple tool to describe weather conditions
+Home-page: https://github.com/jimbosimbo/howstheweather
 License: MIT
 Author: Jim Jimbo
 Author-email: jim377893@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

