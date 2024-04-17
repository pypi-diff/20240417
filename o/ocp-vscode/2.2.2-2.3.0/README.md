# Comparing `tmp/ocp_vscode-2.2.2.tar.gz` & `tmp/ocp_vscode-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp_vscode-2.2.2.tar", last modified: Sat Mar 23 16:35:33 2024, max compression
+gzip compressed data, was "ocp_vscode-2.3.0.tar", last modified: Wed Apr 17 18:24:07 2024, max compression
```

## Comparing `ocp_vscode-2.2.2.tar` & `ocp_vscode-2.3.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-03-23 16:35:33.132739 ocp_vscode-2.2.2/
--rw-r--r--   0 bernhard   (501) staff       (20)    10938 2022-10-05 06:47:11.000000 ocp_vscode-2.2.2/LICENSE
--rw-r--r--   0 bernhard   (501) staff       (20)      806 2024-03-23 16:35:33.132789 ocp_vscode-2.2.2/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)    12164 2024-03-23 16:34:30.000000 ocp_vscode-2.2.2/README.md
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-03-23 16:35:33.131584 ocp_vscode-2.2.2/ocp_vscode/
--rw-r--r--   0 bernhard   (501) staff       (20)      815 2024-03-23 16:29:12.000000 ocp_vscode-2.2.2/ocp_vscode/__init__.py
--rw-r--r--   0 bernhard   (501) staff       (20)     4972 2024-01-16 17:49:02.000000 ocp_vscode-2.2.2/ocp_vscode/animation.py
--rw-r--r--   0 bernhard   (501) staff       (20)    14216 2024-01-16 17:49:02.000000 ocp_vscode-2.2.2/ocp_vscode/backend.py
--rw-r--r--   0 bernhard   (501) staff       (20)    19453 2024-01-16 17:49:02.000000 ocp_vscode-2.2.2/ocp_vscode/build123d.py
--rw-r--r--   0 bernhard   (501) staff       (20)    19488 2024-01-16 17:49:02.000000 ocp_vscode-2.2.2/ocp_vscode/colors.py
--rw-r--r--   0 bernhard   (501) staff       (20)     8011 2024-01-16 17:49:02.000000 ocp_vscode-2.2.2/ocp_vscode/comms.py
--rw-r--r--   0 bernhard   (501) staff       (20)    16012 2024-03-21 18:51:04.000000 ocp_vscode-2.2.2/ocp_vscode/config.py
--rw-r--r--   0 bernhard   (501) staff       (20)    33451 2024-03-21 20:22:37.000000 ocp_vscode-2.2.2/ocp_vscode/show.py
--rw-r--r--   0 bernhard   (501) staff       (20)     5024 2024-01-16 17:49:02.000000 ocp_vscode-2.2.2/ocp_vscode/state.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-03-23 16:35:33.132255 ocp_vscode-2.2.2/ocp_vscode.egg-info/
--rw-r--r--   0 bernhard   (501) staff       (20)      806 2024-03-23 16:35:33.000000 ocp_vscode-2.2.2/ocp_vscode.egg-info/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)      506 2024-03-23 16:35:33.000000 ocp_vscode-2.2.2/ocp_vscode.egg-info/SOURCES.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2024-03-23 16:35:33.000000 ocp_vscode-2.2.2/ocp_vscode.egg-info/dependency_links.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2024-03-23 16:35:33.000000 ocp_vscode-2.2.2/ocp_vscode.egg-info/not-zip-safe
--rw-r--r--   0 bernhard   (501) staff       (20)       78 2024-03-23 16:35:33.000000 ocp_vscode-2.2.2/ocp_vscode.egg-info/requires.txt
--rw-r--r--   0 bernhard   (501) staff       (20)       11 2024-03-23 16:35:33.000000 ocp_vscode-2.2.2/ocp_vscode.egg-info/top_level.txt
--rw-r--r--   0 bernhard   (501) staff       (20)     1038 2024-03-23 16:35:33.133033 ocp_vscode-2.2.2/setup.cfg
--rw-r--r--   0 bernhard   (501) staff       (20)     1227 2024-03-23 16:29:12.000000 ocp_vscode-2.2.2/setup.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-03-23 16:35:33.132634 ocp_vscode-2.2.2/test/
--rw-r--r--   0 bernhard   (501) staff       (20)      401 2023-11-24 07:13:36.000000 ocp_vscode-2.2.2/test/test_for_backend.py
--rw-r--r--   0 bernhard   (501) staff       (20)    18719 2024-01-16 17:49:02.000000 ocp_vscode-2.2.2/test/test_serialisation.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1890 2023-11-24 07:13:36.000000 ocp_vscode-2.2.2/test/testextension.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-17 18:24:07.921338 ocp_vscode-2.3.0/
+-rw-r--r--   0 bernhard   (501) staff       (20)    10938 2022-10-05 06:47:11.000000 ocp_vscode-2.3.0/LICENSE
+-rw-r--r--   0 bernhard   (501) staff       (20)      959 2024-04-17 18:24:07.921165 ocp_vscode-2.3.0/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)    12859 2024-04-17 06:53:57.000000 ocp_vscode-2.3.0/README.md
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-17 18:24:07.919664 ocp_vscode-2.3.0/ocp_vscode/
+-rw-r--r--   0 bernhard   (501) staff       (20)     1281 2024-04-16 19:20:47.000000 ocp_vscode-2.3.0/ocp_vscode/__init__.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     4972 2024-01-16 17:49:02.000000 ocp_vscode-2.3.0/ocp_vscode/animation.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    14216 2024-01-16 17:49:02.000000 ocp_vscode-2.3.0/ocp_vscode/backend.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    19453 2024-01-16 17:49:02.000000 ocp_vscode-2.3.0/ocp_vscode/build123d.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    19488 2024-01-16 17:49:02.000000 ocp_vscode-2.3.0/ocp_vscode/colors.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     8166 2024-04-16 20:13:02.000000 ocp_vscode-2.3.0/ocp_vscode/comms.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    16326 2024-04-16 20:13:23.000000 ocp_vscode-2.3.0/ocp_vscode/config.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    33098 2024-04-17 06:24:29.000000 ocp_vscode-2.3.0/ocp_vscode/show.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     5024 2024-01-16 17:49:02.000000 ocp_vscode-2.3.0/ocp_vscode/state.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-17 18:24:07.920954 ocp_vscode-2.3.0/ocp_vscode.egg-info/
+-rw-r--r--   0 bernhard   (501) staff       (20)      959 2024-04-17 18:24:07.000000 ocp_vscode-2.3.0/ocp_vscode.egg-info/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)      479 2024-04-17 18:24:07.000000 ocp_vscode-2.3.0/ocp_vscode.egg-info/SOURCES.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2024-04-17 18:24:07.000000 ocp_vscode-2.3.0/ocp_vscode.egg-info/dependency_links.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2024-04-17 18:24:07.000000 ocp_vscode-2.3.0/ocp_vscode.egg-info/not-zip-safe
+-rw-r--r--   0 bernhard   (501) staff       (20)       78 2024-04-17 18:24:07.000000 ocp_vscode-2.3.0/ocp_vscode.egg-info/requires.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)       11 2024-04-17 18:24:07.000000 ocp_vscode-2.3.0/ocp_vscode.egg-info/top_level.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)     1038 2024-04-17 18:24:07.921631 ocp_vscode-2.3.0/setup.cfg
+-rw-r--r--   0 bernhard   (501) staff       (20)     1227 2024-04-14 16:40:03.000000 ocp_vscode-2.3.0/setup.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-17 18:24:07.920771 ocp_vscode-2.3.0/test/
+-rw-r--r--   0 bernhard   (501) staff       (20)      401 2023-11-24 07:13:36.000000 ocp_vscode-2.3.0/test/test_for_backend.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1890 2023-11-24 07:13:36.000000 ocp_vscode-2.3.0/test/testextension.py
```

### Comparing `ocp_vscode-2.2.2/LICENSE` & `ocp_vscode-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ocp_vscode-2.2.2/PKG-INFO` & `ocp_vscode-2.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp_vscode
-Version: 2.2.2
+Version: 2.3.0
 Summary: OCP CAD Viewer for VSCode
 Home-page: https://github.com/bernhard-42/vscode-ocp-cad-viewer
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: vscode,widgets,CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
@@ -13,9 +13,14 @@
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 License-File: LICENSE
+Requires-Dist: ocp-tessellate<2.4.0,>=2.3.0
+Requires-Dist: requests
+Requires-Dist: ipykernel
+Requires-Dist: orjson
+Requires-Dist: websockets<11.1,>=11.0
 
 An extension to show OCP cad CAD objects (CadQuery, build123d) in VS Code via threejs
```

### Comparing `ocp_vscode-2.2.2/README.md` & `ocp_vscode-2.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -181,16 +181,36 @@
 
     Sometimes it is helpful to keep the orientation of an object across code changes. This is what `reset_camera` does:
 
     -   `reset_camera=Camera.Center` will keep position and rotation, but ignore panning. This means the new object will be repositioned to the center (most robust approach)
     -   `reset_camera=Camera.KEEP` will keep position, rotation and panning. However, panning can be problematic. When the next object to be shown is much larger or smaller and the object before was panned, it can happen that nothing is visible (the new object at the pan location is outside of the viewer frustum). OCP CAD Viewer checks whether the bounding box of an object is 2x smaller or larger than the one of the last shown object. If so, it falls back to `Camera.CENTER`. A notification is written to the OCP CAD Viewer output panel.
     -   `reset_camera=Camera.RESET` will ensure that position, rotation and panning will be reset to the initial default
 
+## Development
+
+Testing:
+
+Native tessellator can be set via `NATIVE_TESSELLATOR=1`and Python tessellator via `NATIVE_TESSELLATOR=0`.
+
+When `OCP_VSCODE_PYTEST=1` is set, `show` will not send the tessellated results to the viewer, but return it to the caller for inspection.
+
+A full test cycle consist of:
+
+```bash
+NATIVE_TESSELLATOR=0 OCP_VSCODE_PYTEST=1 pytest -v -s pytests/
+NATIVE_TESSELLATOR=1 OCP_VSCODE_PYTEST=1 pytest -v -s pytests/
+```
+
 ## Changes
 
+v2.3.0
+- Add newest ocp-tessellate to allow using native tessellator from ocp_addons
+- Fine tune communication to ensure the memory view of buffers will be passed through to javascript for performance
+- Use of the new protocol v3 of three-cad-viewer
+
 v2.2.2
 - Fix regression in measure tools
 
 v2.2.1
 -   Fix: Wrong back material color for faces
 -   Improve parameters of Imageface
 -   Improve clipping when faces are deselected
```

### Comparing `ocp_vscode-2.2.2/ocp_vscode/animation.py` & `ocp_vscode-2.3.0/ocp_vscode/animation.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-2.2.2/ocp_vscode/backend.py` & `ocp_vscode-2.3.0/ocp_vscode/backend.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-2.2.2/ocp_vscode/build123d.py` & `ocp_vscode-2.3.0/ocp_vscode/build123d.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-2.2.2/ocp_vscode/colors.py` & `ocp_vscode-2.3.0/ocp_vscode/colors.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-2.2.2/ocp_vscode/comms.py` & `ocp_vscode-2.3.0/ocp_vscode/comms.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,28 +16,30 @@
     is_topods_shape,
     is_toploc_location,
     serialize,
     loc_to_tq,
 )
 from .state import get_state, update_state, get_config_file
 
+
 # pylint: disable=unused-import
 try:
     from IPython import get_ipython
     import jupyter_console
 
     JCONSOLE = True
 except:  # pylint: disable=bare-except
     JCONSOLE = False
 
 CMD_URL = "ws://127.0.0.1"
 CMD_PORT = 3939
 
 INIT_DONE = False
 
+
 #
 # Send data to the viewer
 #
 
 
 class MessageType(enum.IntEnum):
     """Message types"""
@@ -54,17 +56,22 @@
 __all__ = [
     "send_data",
     "send_command",
     "send_response",
     "set_port",
     "get_port",
     "listener",
+    "is_pytest",
 ]
 
 
+def is_pytest():
+    return os.environ.get("OCP_VSCODE_PYTEST") == "1"
+
+
 def port_check(port):
     """Check whether the port is listening"""
     s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     s.settimeout(1)
     result = s.connect_ex(("127.0.0.1", port)) == 0
     if result:
         s.close()
@@ -81,14 +88,17 @@
         return obj.value
     else:
         raise TypeError(f"Object of type {type(obj)} is not JSON serializable")
 
 
 def get_port():
     """Get the port"""
+    if is_pytest():
+        return 3939
+
     if not INIT_DONE:
         find_and_set_port()
         set_connection_file()
     return CMD_PORT
 
 
 def set_port(port):
@@ -127,20 +137,21 @@
 
             result = None
             if message_type == MessageType.COMMAND:
                 try:
                     result = json.loads(ws.recv())
                 except Exception as ex:  # pylint: disable=broad-except
                     print(ex)
-            try:
-                ws.close()
-            except:  # pylint: disable=bare-except
-                pass
 
-            return result
+            # try:
+            #     ws.close()
+            # except Exception as ex:  # pylint: disable=bare-except
+            #     pass
+
+        return result
 
     except Exception as ex:  # pylint: disable=broad-except
         print(
             f"Cannot connect to viewer on port {port}, is it running and the right port provided?"
         )
         print(ex)
         return None
@@ -274,8 +285,8 @@
             update_state(CMD_PORT, "connection_file", cf)
             print(f"Jupyter connection file path written to {get_config_file()}")
         else:
             print("Jupyter kernel not responding")
     elif not JCONSOLE:
         print("Jupyter console not installed")
     else:
-        print("Jupyter kernel not running")
+        print("Jupyter kernel not running")
```

### Comparing `ocp_vscode-2.2.2/ocp_vscode/config.py` & `ocp_vscode-2.3.0/ocp_vscode/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from enum import Enum
 
-from .comms import send_command, send_config, get_port
+from .comms import send_command, send_config, get_port, is_pytest
 
 __all__ = [
     "workspace_config",
     "combined_config",
     "set_viewer_config",
     "set_defaults",
     "reset_defaults",
@@ -397,14 +397,18 @@
 def ui_filter(conf):
     """Filter out all non-UI keys from the config dict"""
     return {k: v for k, v in conf.items() if k in CONFIG_UI_KEYS}
 
 
 def status(port=None, debug=False):
     """Get viewer status"""
+
+    if is_pytest():
+        return {}
+
     if port is None:
         port = get_port()
     try:
         response = send_command("status", port=port)
         if debug:
             return response.get("_debugStarted", False)
         else:
@@ -414,14 +418,24 @@
         raise RuntimeError(
             "Cannot access viewer status. Is the viewer running?\n" + str(ex.args)
         ) from ex
 
 
 def workspace_config(port=None):
     """Get viewer workspace config"""
+
+    if is_pytest():
+        return {
+            "measure_tools": False,
+            "_splash": False,
+            "default_facecolor": (1, 234, 56),
+            "default_thickedgecolor": (123, 45, 6),
+            "default_vertexcolor": (123, 45, 6),
+        }
+
     if port is None:
         port = get_port()
     try:
         conf = send_command("config", port=port)
         mapping = {
             "none": Collapse.NONE,
             "leaves": Collapse.LEAVES,
```

### Comparing `ocp_vscode-2.2.2/ocp_vscode/show.py` & `ocp_vscode-2.3.0/ocp_vscode/show.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+import os
 import re
+import types
 
 from ocp_tessellate import PartGroup
 from ocp_tessellate.convert import (
     tessellate_group,
     get_normal_len,
     combined_bb,
     to_assembly,
@@ -46,27 +48,27 @@
     OCP_Edges,
     OCP_Faces,
     OCP_Part,
     OCP_Vertices,
 )
 import ocp_tessellate.convert as oc
 
-from .config import (
+from ocp_vscode.config import (
     preset,
     get_changed_config,
     workspace_config,
     combined_config,
     get_default,
     get_defaults,
     Camera,
     Collapse,
     check_deprecated,
 )
-from .comms import send_backend, send_data
-from .colors import get_colormap, web_to_rgb, BaseColorMap
+from ocp_vscode.comms import send_backend, send_data, is_pytest
+from ocp_vscode.colors import get_colormap, web_to_rgb, BaseColorMap
 
 __all__ = ["show", "show_object", "reset_show", "show_all", "show_clear"]
 
 OBJECTS = {"objs": [], "names": [], "colors": [], "alphas": []}
 
 LAST_CALL = "other"
 
@@ -136,15 +138,15 @@
         timeit = False
 
     if progress is None:
         progress = Progress([c for c in "-+c"])
 
     with Timer(timeit, "", "to_assembly", 1):
         changed_config = get_changed_config()
-        part_group = to_assembly(
+        part_group, instances = to_assembly(
             *cad_objs,
             names=names,
             colors=colors,
             alphas=alphas,
             render_mates=kwargs.get("render_mates", changed_config.get("render_mates")),
             render_joints=kwargs.get(
                 "render_joints", changed_config.get("render_joints")
@@ -212,29 +214,35 @@
 
     with Timer(timeit, "", "tessellate", 1):
         if parallel:
             init_pool()
             keymap.reset()
 
         instances, shapes, states, mapping = tessellate_group(
-            part_group, params, progress, params.get("timeit")
+            part_group, instances, params, progress, params.get("timeit")
         )
 
         if parallel:
             instances, shapes = mp_get_results(instances, shapes, progress)
             close_pool()
 
     params["normal_len"] = get_normal_len(
         preset("render_normals", params.get("render_normals")),
         shapes,
         preset("deviation", params.get("deviation")),
     )
 
     with Timer(timeit, "", "bb", 1):
-        bb = combined_bb(shapes).to_dict()
+        bb = combined_bb(shapes)
+        if bb is None:
+            bb = dict(
+                xmin=-1e-6, ymin=-1e-6, zmin=-1e-6, xmax=1e-6, ymax=1e-6, zmax=1e-6
+            )
+        else:
+            bb = bb.to_dict()
 
     # add global bounding box
     shapes["bb"] = bb
 
     return instances, shapes, states, params, part_group.count_shapes(), mapping
 
 
@@ -268,30 +276,34 @@
     if config.get("debug") is not None and config["debug"]:
         print("\nconfig:\n", config)
 
     if kwargs.get("explode") is not None:
         config["explode"] = kwargs["explode"]
 
     with Timer(timeit, "", "create data obj", 1):
+        if is_pytest():
+            return (instances, shapes, states, config, count_shapes), mapping
+
         return {
             "data": numpy_to_buffer_json(
-                dict(instances=instances, shapes=shapes, states=states)
+                dict(instances=instances, shapes=shapes, states=states),
             ),
             "type": "data",
             "config": config,
             "count": count_shapes,
         }, mapping
+    return result
 
 
 class Progress:
     """Progress indicator for tessellation"""
 
     def __init__(self, levels=None):
         if levels is None:
-            self.levels = ["+", "c", "-"]
+            self.levels = ["+c-*"]
         else:
             self.levels = levels
 
     def update(self, mark="+"):
         """Update progress indicator"""
         if mark in self.levels:
             print(mark, end="", flush=True)
@@ -314,15 +326,15 @@
 # pylint: disable=unused-argument
 def show(
     *cad_objs,
     names=None,
     colors=None,
     alphas=None,
     port=None,
-    progress="-+c",
+    progress="-+*c",
     glass=None,
     tools=None,
     measure_tools=None,
     tree_width=None,
     axes=None,
     axes0=None,
     grid=None,
@@ -384,16 +396,19 @@
         cad_objs:                All cad objects that should be shown as positional parameters
 
     Keywords for show:
         names:                   List of names for the cad_objs. Needs to have the same length as cad_objs
         colors:                  List of colors for the cad_objs. Needs to have the same length as cad_objs
         alphas:                  List of alpha values for the cad_objs. Needs to have the same length as cad_objs
         port:                    The port the viewer listens to. Typically use 'set_port(port)' instead
-        progress:                Show progress of tessellation with None is no progress indicator. (default="-+c")
-                                 for object: "-": is reference, "+": gets tessellated, "c": from cache
+        progress:                Show progress of tessellation with None is no progress indicator. (default="-+*c")
+                                 for object: "-": is reference,
+                                             "+": gets tessellated with Python code,
+                                             "*": gets tessellated with native code,
+                                             "c": from cache
 
     Valid keywords to configure the viewer (**kwargs):
     - UI
         glass:                   Use glass mode where tree is an overlay over the cad object (default=False)
         measure_tools:           Show measure tools (default=False)
         tools:                   Show tools (default=True)
         tree_width:              Width of the object tree (default=240)
@@ -548,14 +563,17 @@
         )
 
         if not _force_in_debug:
             LAST_CALL = "show"
         else:
             LAST_CALL = "other"
 
+    if is_pytest():
+        return t, mapping
+
     with Timer(timeit, "", "send"):
         send_data(t, port=port, timeit=timeit)
 
     if measure_tools:
         send_backend({"model": mapping}, port=port, timeit=timeit)
 
 
@@ -570,15 +588,15 @@
 def show_object(
     obj,
     name=None,
     options=None,
     parent=None,
     clear=False,
     port=None,
-    progress="-+c",
+    progress="-+*c",
     glass=None,
     tools=None,
     measure_tools=None,
     tree_width=None,
     axes=None,
     axes0=None,
     grid=None,
@@ -642,16 +660,20 @@
         name:                    The name of the CAD object
         options:                 A dict of color and alpha value: {"alpha":0.5, "color": (64, 164, 223)}
                                  0 <= alpha <= 1.0 and color is a 3-tuple of values between 0 and 255
         parent:                  Add another object, usually the parent of e.g. edges or vertices with alpha=0.25
         clear:                   In interactice mode, clear the stack of objects to be shown
                                  (typically used for the first object)
         port:                    The port the viewer listens to. Typically use 'set_port(port)' instead
-        progress:                Show progress of tessellation with None is no progress indicator. (default="-+c")
-                                 for object: "-": is reference, "+": gets tessellated, "c": from cache
+        progress:                Show progress of tessellation with None is no progress indicator. (default="-+*c")
+                                 for object: "-": is reference,
+                                             "+": gets tessellated with Python code,
+                                             "*": gets tessellated with native code,
+                                             "c": from cache
+
 
     Valid keywords to configure the viewer (**kwargs):
     - UI
         glass:                   Use glass mode where tree is an overlay over the cad object (default=False)
         measure_tools:           Show measure tools (default=False)
         tools:                   Show tools (default=True)
         tree_width:              Width of the object tree (default=240)
@@ -774,52 +796,21 @@
     """Clear the viewer"""
     data = {
         "type": "clear",
     }
     send_data(data)
 
 
-def ocp_group(obj, name):
-
-    def to_group(obj, name, group):
-        if isinstance(obj, list):
-            sub_group = OCP_PartGroup([], name=name)
-            for i, el in enumerate(obj):
-                new_obj = to_group(el, f"{name}[{i}]", sub_group)
-                if new_obj is not None:
-                    sub_group.add(new_obj)
-            group.add(sub_group)
-        elif isinstance(obj, dict):
-            sub_group = OCP_PartGroup([], name=name)
-            for name, el in obj.items():
-                new_obj = to_group(el, name, sub_group)
-                if new_obj is not None:
-                    sub_group.add(new_obj)
-            group.add(sub_group)
-        else:
-            if (
-                (is_wrapped(obj) and not obj.__class__.__name__ == "Color")
-                or is_build123d(obj)
-                or is_cadquery(obj)
-            ):
-                new_obj = conv(obj)
-                new_obj.name = name
-                group.add(new_obj)
-            else:
-                ...
-                # print(
-                #     f"show_all: Type {type(obj)} for name {name} cannot be visualized"
-                # )
-
-    group = OCP_PartGroup([], name=name)
-    to_group(obj, name, group)
-    return group.objects[0]
-
-
-def show_all(variables=None, exclude=None, classes=None, _visual_debug=False, **kwargs):
+def show_all(
+    variables=None,
+    exclude=None,
+    classes=None,
+    _visual_debug=False,
+    **kwargs,
+):
     """Show all variables in the current scope"""
     import inspect  # pylint: disable=import-outside-toplevel
 
     global LAST_CALL  # pylint: disable=global-statement
 
     if not _visual_debug:
         LAST_CALL = "other"
@@ -836,30 +827,31 @@
     if exclude is None:
         exclude = []
 
     objects = []
     names = []
     for name, obj in variables.items():
         if (
+            # ignore classes and ipython and jupyter variables
             isinstance(obj, type)
-            or name in ["_", "__", "___"]
+            or name in exclude + ["_", "__", "___", "_ih", "_oh", "_dh", "Out", "In"]
             or name.startswith("__")
             or re.search("_\\d+", name) is not None
+            # pylint: disable=protected-access
+            or (hasattr(obj, "_obj") and obj._obj is None)
+            or callable(obj)
+            or isinstance(obj, (int, float, str, bool, types.ModuleType))
         ):
-            continue  # ignore classes and jupyter variables
+            continue
+
         if hasattr(obj, "area") and obj.area > 1e99:  # inifinite face
             print(f"infinite face {name} skipped")
             continue
 
-        if name not in exclude and (classes is None or isinstance(obj, tuple(classes))):
-            if (
-                hasattr(obj, "_obj")
-                and obj._obj is None  # pylint: disable=protected-access
-            ):
-                continue
+        if classes is None or isinstance(obj, tuple(classes)):
 
             if hasattr(obj, "locations") and hasattr(obj, "local_locations"):
                 obj = obj.locations
 
             if hasattr(obj, "local_coord_system"):
                 obj = obj.location
 
@@ -877,14 +869,15 @@
                 or is_build123d(obj)
                 or is_cadquery_assembly(obj)
                 or (
                     hasattr(obj, "wrapped")
                     and hasattr(obj, "position")
                     and hasattr(obj, "direction")
                 )
+                or isinstance(obj, (list, tuple, dict))
             ):
                 objects.append(obj)
                 names.append(name)
 
             elif isinstance(
                 obj, (OCP_PartGroup, OCP_Edges, OCP_Faces, OCP_Part, OCP_Vertices)
             ):
@@ -894,31 +887,29 @@
 
             elif is_cadquery_sketch(obj):
                 pg = to_assembly([obj], names=[name])
                 pg.name = name
                 objects.append(pg)
                 names.append(name)
 
-            elif isinstance(obj, (list, tuple, dict)):
-                if not name in [
-                    "_ih",
-                    "_oh",
-                    "_dh",
-                    "Out",
-                    "In",
-                ]:  # no IPython dicts and lists
-                    obj = ocp_group(obj, name)
-                    if len(obj.objects) > 0:
-                        objects.append(obj)
-                        obj.name = name
-                        names.append(name)
+            else:
+                print(
+                    f"show_all: Type {type(obj)} for name {name} cannot be visualized"
+                )
 
     if len(objects) > 0:
-        show(
-            *objects,
-            names=names,
-            collapse=Collapse.ROOT,
-            _force_in_debug=_visual_debug,
-            **kwargs,
-        )
+        try:
+            result = show(
+                *objects,
+                names=names,
+                collapse=Collapse.ROOT,
+                _force_in_debug=_visual_debug,
+                **kwargs,
+            )
+            if is_pytest():
+                return result
+        except Exception as ex:  # pylint: disable=broad-exception-caught
+            print("show_all:", ex)
     else:
+        if is_pytest():
+            return None
         show_clear()
```

### Comparing `ocp_vscode-2.2.2/ocp_vscode/state.py` & `ocp_vscode-2.3.0/ocp_vscode/state.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-2.2.2/ocp_vscode.egg-info/PKG-INFO` & `ocp_vscode-2.3.0/ocp_vscode.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ocp-vscode
-Version: 2.2.2
+Name: ocp_vscode
+Version: 2.3.0
 Summary: OCP CAD Viewer for VSCode
 Home-page: https://github.com/bernhard-42/vscode-ocp-cad-viewer
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: vscode,widgets,CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
@@ -13,9 +13,14 @@
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 License-File: LICENSE
+Requires-Dist: ocp-tessellate<2.4.0,>=2.3.0
+Requires-Dist: requests
+Requires-Dist: ipykernel
+Requires-Dist: orjson
+Requires-Dist: websockets<11.1,>=11.0
 
 An extension to show OCP cad CAD objects (CadQuery, build123d) in VS Code via threejs
```

### Comparing `ocp_vscode-2.2.2/setup.cfg` & `ocp_vscode-2.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.2.2
+current_version = 2.3.0
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>\D*)(?P<build>\d*)
 serialize = 
 	{major}.{minor}.{patch}{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `ocp_vscode-2.2.2/setup.py` & `ocp_vscode-2.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup_args = {
     "name": "ocp_vscode",
-    "version": "2.2.2",
+    "version": "2.3.0",
     "description": "OCP CAD Viewer for VSCode",
     "long_description": "An extension to show OCP cad CAD objects (CadQuery, build123d) in VS Code via threejs",
     "include_package_data": True,
     "python_requires": ">=3.9",
     "install_requires": [
-        "ocp-tessellate>=2.2.2,<2.3.0",
+        "ocp-tessellate>=2.3.0,<2.4.0",
         "requests",
         "ipykernel",
         "orjson",
         "websockets>=11.0,<11.1",
     ],
     "packages": find_packages(),
     "zip_safe": False,
```

### Comparing `ocp_vscode-2.2.2/test/testextension.py` & `ocp_vscode-2.3.0/test/testextension.py`

 * *Files identical despite different names*

