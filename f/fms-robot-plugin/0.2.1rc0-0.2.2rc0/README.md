# Comparing `tmp/fms_robot_plugin-0.2.1rc0.tar.gz` & `tmp/fms_robot_plugin-0.2.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fms_robot_plugin-0.2.1rc0.tar", max compression
+gzip compressed data, was "fms_robot_plugin-0.2.2rc0.tar", max compression
```

## Comparing `fms_robot_plugin-0.2.1rc0.tar` & `fms_robot_plugin-0.2.2rc0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       26 2024-04-17 02:39:21.572440 fms_robot_plugin-0.2.1rc0/README.md
--rw-r--r--   0        0        0       49 2024-04-17 02:39:21.576440 fms_robot_plugin-0.2.1rc0/fms_robot_plugin/__init__.py
--rw-r--r--   0        0        0     1824 2024-04-17 02:39:21.576440 fms_robot_plugin-0.2.1rc0/fms_robot_plugin/mqtt.py
--rw-r--r--   0        0        0     8771 2024-04-17 02:39:21.576440 fms_robot_plugin-0.2.1rc0/fms_robot_plugin/robot.py
--rw-r--r--   0        0        0     3168 2024-04-17 02:39:21.576440 fms_robot_plugin-0.2.1rc0/fms_robot_plugin/typings.py
--rw-r--r--   0        0        0      657 2024-04-17 02:39:21.576440 fms_robot_plugin-0.2.1rc0/pyproject.toml
--rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 fms_robot_plugin-0.2.1rc0/setup.py
--rw-r--r--   0        0        0      502 1970-01-01 00:00:00.000000 fms_robot_plugin-0.2.1rc0/PKG-INFO
+-rw-r--r--   0        0        0       26 2024-04-12 08:08:58.136799 fms_robot_plugin-0.2.2rc0/README.md
+-rw-r--r--   0        0        0       49 2024-04-12 08:08:58.140799 fms_robot_plugin-0.2.2rc0/fms_robot_plugin/__init__.py
+-rw-r--r--   0        0        0     1824 2024-04-12 08:08:58.140799 fms_robot_plugin-0.2.2rc0/fms_robot_plugin/mqtt.py
+-rw-r--r--   0        0        0     8727 2024-04-12 08:08:58.140799 fms_robot_plugin-0.2.2rc0/fms_robot_plugin/robot.py
+-rw-r--r--   0        0        0     3168 2024-04-12 08:08:58.140799 fms_robot_plugin-0.2.2rc0/fms_robot_plugin/typings.py
+-rw-r--r--   0        0        0      657 2024-04-12 08:08:58.140799 fms_robot_plugin-0.2.2rc0/pyproject.toml
+-rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 fms_robot_plugin-0.2.2rc0/setup.py
+-rw-r--r--   0        0        0      502 1970-01-01 00:00:00.000000 fms_robot_plugin-0.2.2rc0/PKG-INFO
```

### Comparing `fms_robot_plugin-0.2.1rc0/fms_robot_plugin/mqtt.py` & `fms_robot_plugin-0.2.2rc0/fms_robot_plugin/mqtt.py`

 * *Files identical despite different names*

### Comparing `fms_robot_plugin-0.2.1rc0/fms_robot_plugin/robot.py` & `fms_robot_plugin-0.2.2rc0/fms_robot_plugin/robot.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,28 +68,28 @@
         topic = f"robots/{self.robot_key}/mapping/save"
         self.consumer(topic).consume(lambda _: cb(), serialize=False)
 
     def on_localize(self, cb: Callable[[str, Pose], None]):
         topic = f"robots/{self.robot_key}/localize"
         self.consumer(topic).consume(lambda data: cb(data["map_id"], Pose(**data["initial_pose"])))
 
-    def on_load_navigation_map_pgm(self, cb: Callable[[bytes, str], None]):
-        topic = f"robots/{self.robot_key}/maps/:map_id/load/navigation_pgm"
+    def on_load_map_pgm(self, cb: Callable[[bytes, str], None]):
+        topic = f"robots/{self.robot_key}/maps/:map_id/load/pgm"
         self.consumer(topic).consume(lambda pgm, url_params: cb(pgm, url_params["map_id"]), serialize=False)
 
-    def on_load_navigation_map_yaml(self, cb: Callable[[bytes, str], None]):
-        topic = f"robots/{self.robot_key}/maps/:map_id/load/navigation_yaml"
+    def on_load_map_yaml(self, cb: Callable[[bytes, str], None]):
+        topic = f"robots/{self.robot_key}/maps/:map_id/load/yaml"
         self.consumer(topic).consume(lambda yaml, url_params: cb(yaml, url_params["map_id"]), serialize=False)
 
-    def on_load_localization_map_pgm(self, cb: Callable[[bytes, str], None]):
-        topic = f"robots/{self.robot_key}/maps/:map_id/load/localization_pgm"
+    def on_load_map_localization_pgm(self, cb: Callable[[bytes, str], None]):
+        topic = f"robots/{self.robot_key}/maps/:map_id/load/localization/pgm"
         self.consumer(topic).consume(lambda pgm, url_params: cb(pgm, url_params["map_id"]), serialize=False)
 
-    def on_load_localization_map_yaml(self, cb: Callable[[bytes, str], None]):
-        topic = f"robots/{self.robot_key}/maps/:map_id/load/localization_yaml"
+    def on_load_map_localization_yaml(self, cb: Callable[[bytes, str], None]):
+        topic = f"robots/{self.robot_key}/maps/:map_id/load/localization/yaml"
         self.consumer(topic).consume(lambda yaml, url_params: cb(yaml, url_params["map_id"]), serialize=False)
 
     def on_unload_map(self, cb: Callable[[], None]):
         topic = f"robots/{self.robot_key}/maps/unload"
         self.consumer(topic).consume(lambda _: cb(), serialize=False)
 
     def on_execute_task(self, cb: Callable[[Task], None]):
```

### Comparing `fms_robot_plugin-0.2.1rc0/fms_robot_plugin/typings.py` & `fms_robot_plugin-0.2.2rc0/fms_robot_plugin/typings.py`

 * *Files identical despite different names*

### Comparing `fms_robot_plugin-0.2.1rc0/pyproject.toml` & `fms_robot_plugin-0.2.2rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fms-robot-plugin"
-version = "0.2.1rc0"
+version = "0.2.2rc0"
 description = ""
 authors = [
   "Dionesius Agung <dionesius@movel.ai>",
   "Steven Hansel <steven@movel.ai>"
 ]
 readme = "README.md"
 packages = [{include = "fms_robot_plugin"}]
```

### Comparing `fms_robot_plugin-0.2.1rc0/setup.py` & `fms_robot_plugin-0.2.2rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['paho-mqtt>=1.6.1,<2.0.0', 'pydantic>=2.3.0,<3.0.0', 'requests>=2.31.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'fms-robot-plugin',
-    'version': '0.2.1rc0',
+    'version': '0.2.2rc0',
     'description': '',
     'long_description': '# FMS Robot Plugin Library',
     'author': 'Dionesius Agung',
     'author_email': 'dionesius@movel.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

