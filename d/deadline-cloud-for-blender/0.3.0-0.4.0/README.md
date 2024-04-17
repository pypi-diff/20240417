# Comparing `tmp/deadline_cloud_for_blender-0.3.0.tar.gz` & `tmp/deadline_cloud_for_blender-0.4.0.tar.gz`

## Comparing `deadline_cloud_for_blender-0.3.0.tar` & `deadline_cloud_for_blender-0.4.0.tar`

### file list

```diff
@@ -1,38 +1,37 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/_version.py
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/hatch_custom_hook.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_adaptor/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_adaptor/_version.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_adaptor/BlenderAdaptor/BlenderAdaptor.json
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_adaptor/BlenderAdaptor/__init__.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_adaptor/BlenderAdaptor/__main__.py
--rw-r--r--   0        0        0    18486 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_adaptor/BlenderAdaptor/adaptor.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_adaptor/BlenderAdaptor/py.typed
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_adaptor/BlenderAdaptor/schemas/init_data.schema.json
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_adaptor/BlenderAdaptor/schemas/run_data.schema.json
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_adaptor/BlenderClient/__init__.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_adaptor/BlenderClient/blender_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_adaptor/BlenderClient/py.typed
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_adaptor/BlenderClient/render_handlers/__init__.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_adaptor/BlenderClient/render_handlers/cycles_blender_handler.py
--rw-r--r--   0        0        0     7928 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_adaptor/BlenderClient/render_handlers/default_blender_handler.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_adaptor/BlenderClient/render_handlers/workbench_blender_handler.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_submitter/_version.py
--rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/_version.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/adaptor_override_environment.yaml
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/addonpreferences.py
--rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/blender_utils.py
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/default_blender_template.yaml
--rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/job_settings.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/logutil.py
--rw-r--r--   0        0        0     7649 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/open_deadline_cloud_dialog.py
--rw-r--r--   0        0        0     6519 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/sanity_checks.py
--rw-r--r--   0        0        0    10897 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/scene_settings_widget.py
--rw-r--r--   0        0        0    16433 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/template_filling.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/NOTICE
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/README.md
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/hatch.toml
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/_version.py
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/hatch_custom_hook.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/_version.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderAdaptor/BlenderAdaptor.json
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderAdaptor/__init__.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderAdaptor/__main__.py
+-rw-r--r--   0        0        0    18486 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderAdaptor/adaptor.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderAdaptor/py.typed
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderAdaptor/schemas/init_data.schema.json
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderAdaptor/schemas/run_data.schema.json
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderClient/__init__.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderClient/blender_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderClient/py.typed
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderClient/render_handlers/__init__.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderClient/render_handlers/cycles_blender_handler.py
+-rw-r--r--   0        0        0     7928 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderClient/render_handlers/default_blender_handler.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderClient/render_handlers/workbench_blender_handler.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/_version.py
+-rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/_version.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/adaptor_override_environment.yaml
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/addonpreferences.py
+-rw-r--r--   0        0        0     4530 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/blender_utils.py
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/default_blender_template.yaml
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/logutil.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/open_deadline_cloud_dialog.py
+-rw-r--r--   0        0        0     6530 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/sanity_checks.py
+-rw-r--r--   0        0        0    10922 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/scene_settings_widget.py
+-rw-r--r--   0        0        0    16431 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/template_filling.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/NOTICE
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/README.md
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/hatch.toml
+-rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 deadline_cloud_for_blender-0.4.0/PKG-INFO
```

### Comparing `deadline_cloud_for_blender-0.3.0/hatch_custom_hook.py` & `deadline_cloud_for_blender-0.4.0/hatch_custom_hook.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.3.0/src/deadline/blender_adaptor/BlenderAdaptor/__main__.py` & `deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderAdaptor/__main__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.3.0/src/deadline/blender_adaptor/BlenderAdaptor/adaptor.py` & `deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderAdaptor/adaptor.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.3.0/src/deadline/blender_adaptor/BlenderAdaptor/schemas/init_data.schema.json` & `deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderAdaptor/schemas/init_data.schema.json`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.3.0/src/deadline/blender_adaptor/BlenderClient/blender_client.py` & `deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderClient/blender_client.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.3.0/src/deadline/blender_adaptor/BlenderClient/render_handlers/__init__.py` & `deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderClient/render_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.3.0/src/deadline/blender_adaptor/BlenderClient/render_handlers/default_blender_handler.py` & `deadline_cloud_for_blender-0.4.0/src/deadline/blender_adaptor/BlenderClient/render_handlers/default_blender_handler.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.3.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/__init__.py` & `deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.3.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/adaptor_override_environment.yaml` & `deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/adaptor_override_environment.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.3.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/addonpreferences.py` & `deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/addonpreferences.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.3.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/blender_utils.py` & `deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/blender_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,23 @@
 from pathlib import Path
 
 import bpy
 
 _logger = logging.getLogger(__name__)
 
 
-def get_view_layers(saved_scene_name) -> list[str]:
-    """Get the view layers associated with a scene.
+def get_renderable_view_layers(saved_scene_name) -> list[str]:
+    """Get the view layers associated with a scene that are selected to use
+    during rendering.
 
     Args:
         saved_scene_name: The name of the scene.
     """
     scene_name = bpy.data.scenes[saved_scene_name].name
-    layers = [layer.name for layer in bpy.data.scenes[scene_name].view_layers]
+    layers = [layer.name for layer in bpy.data.scenes[scene_name].view_layers if layer.use]
     return layers
 
 
 def get_renderable_cameras(saved_scene_name) -> list[str]:
     """Returns a list of all camera objects in the scene that are marked as renderable.
 
     Args:
```

### Comparing `deadline_cloud_for_blender-0.3.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/default_blender_template.yaml` & `deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/default_blender_template.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.3.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/logutil.py` & `deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/logutil.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.3.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/open_deadline_cloud_dialog.py` & `deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/open_deadline_cloud_dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     # Initialize render settings with default values.
     settings = tf.BlenderSubmitterUISettings()
 
     # Set settings dependent on scene.
     settings.name = bu.get_scene_name()
     settings.project_path = bpy.context.blend_data.filepath
     settings.output_path = os.path.dirname(bpy.context.blend_data.filepath)
+    settings.frame_list = bu.get_frames()
 
     # Load and set sticky settings, if any.
     settings.load_sticky_settings(settings.project_path)
 
     settings.current_layer_selectable_cameras = settings.camera_selection
     settings.all_layer_selectable_cameras = settings.camera_selection
 
@@ -143,15 +144,15 @@
         image_height_parameter_name=settings.image_height_parameter_name,
         scene_name=settings.scene_name,
     )
 
     # Add selected layers to the list of layers to render.
     layers: list[tf.Layer] = []
     if settings.view_layer_selection == ssw.COMBO_DEFAULT_ALL_RENDERABLE_LAYERS:
-        for layer in bu.get_view_layers(settings.scene_name):
+        for layer in bu.get_renderable_view_layers(settings.scene_name):
             layers.append(tf.Layer(layer, common_layer_settings))
     else:
         layers.append(tf.Layer(settings.view_layer_selection, common_layer_settings))
 
     if settings.override_frame_range:
         common_layer_settings.frame_range = settings.frame_list
```

### Comparing `deadline_cloud_for_blender-0.3.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/sanity_checks.py` & `deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/sanity_checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     if settings.scene_name not in blender_utils.get_all_scenes():
         raise RuntimeError(
             "The selected scene ({}) no longer exists! \n"
             "Please select a different scene.".format(settings.scene_name)
         )
 
     renderable_cameras = blender_utils.get_renderable_cameras(settings.scene_name)
-    renderable_layers = blender_utils.get_view_layers(settings.scene_name)
+    renderable_layers = blender_utils.get_renderable_view_layers(settings.scene_name)
 
     # Ensure there is at least one renderable camera.
     if len(renderable_cameras) == 0:
         raise RuntimeError(
             "There are no renderable cameras in the scene. Please enable at least one before submitting."
         )
```

### Comparing `deadline_cloud_for_blender-0.3.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/scene_settings_widget.py` & `deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/scene_settings_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,14 @@
         self.current_layer_selectable_cameras = initial_settings.current_layer_selectable_cameras
 
         self._build_ui()
         self._load(initial_settings)
 
     def _build_ui(self):
         """Set up the UI."""
-
         layout = QGridLayout(self)
 
         qt_pos_index = 0
         self.proj_path_txt = QLineEdit(self)
         layout.addWidget(QLabel("Project Path"), qt_pos_index, 0)
         layout.addWidget(self.proj_path_txt, qt_pos_index, 1)
         self.proj_path_txt.setReadOnly(True)
@@ -172,15 +171,15 @@
             saved_view_layer_name = self.layers_box.currentData()
             self.layers_box.clear()
 
             # Collect layer data to display.
             self.layers_box.addItem(
                 COMBO_DEFAULT_ALL_RENDERABLE_LAYERS, COMBO_DEFAULT_ALL_RENDERABLE_LAYERS
             )
-            for layer in blender_utils.get_view_layers(scene):
+            for layer in blender_utils.get_renderable_view_layers(scene):
                 self.layers_box.addItem(layer, layer)
 
             # Re-select the layer if possible
             index = self.layers_box.findData(saved_view_layer_name)
             if index >= 0:
                 self.layers_box.setCurrentIndex(index)
 
@@ -224,15 +223,15 @@
         settings.frame_list = self.frame_override_txt.text()
         settings.include_adaptor_wheels = (
             self.include_adaptor_wheels.isChecked() if self.dev_options else False
         )
 
     def activate_frame_override_changed(self, state):
         """Set the activated/deactivated status of the Frame override text box."""
-        self.frame_override_txt.setEnabled(state == Qt.Checked)
+        self.frame_override_txt.setEnabled(Qt.CheckState(state) == Qt.Checked)
 
 
 class FileSearchLineEdit(QWidget):
     """Widget used to contain a line edit and a button which opens a file search box."""
 
     def __init__(self, directory_only=False, parent=None):
         super().__init__(parent=parent)
```

### Comparing `deadline_cloud_for_blender-0.3.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/template_filling.py` & `deadline_cloud_for_blender-0.4.0/src/deadline/blender_submitter/addons/deadline_cloud_blender_submitter/template_filling.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     ui_group_label: str = field(default="Blender Settings")
 
     # Frame settings.
     # Whether to override the frame range.
     override_frame_range: bool = field(default=False, metadata={"sticky": True})
     # The frame range to use if override_frame_range_check is True.
-    frame_list: str = field(default="1-3", metadata={"sticky": True})
+    frame_list: str = field(default="1", metadata={"sticky": True})
 
     # Paths and files.
     project_path: str = field(default="")
     output_path: str = field(default="")
     input_filenames: list[str] = field(default_factory=list, metadata={"sticky": True})
     input_directories: list[str] = field(default_factory=list, metadata={"sticky": True})
     output_directories: list[str] = field(default_factory=list, metadata={"sticky": True})
```

### Comparing `deadline_cloud_for_blender-0.3.0/LICENSE` & `deadline_cloud_for_blender-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.3.0/README.md` & `deadline_cloud_for_blender-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.3.0/hatch.toml` & `deadline_cloud_for_blender-0.4.0/hatch.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_blender-0.3.0/pyproject.toml` & `deadline_cloud_for_blender-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,36 +3,37 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "deadline-cloud-for-blender"
 dynamic = ["version"]
 readme = "README.md"
 license = "Apache-2.0"
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 description = "AWS Deadline Cloud for Blender"
 authors = [
   {name = "Amazon Web Services"},
 ]
 # https://pypi.org/classifiers/
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Operating System :: POSIX :: Linux",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: MacOS",
   "License :: OSI Approved :: Apache Software License",
   "Intended Audience :: Developers",
   "Intended Audience :: End Users/Desktop",
 ]
-# Blender 3.1+ uses Python version 3.10+ (https://vfxplatform.com/ 2023)
-
+# Blender 3.1-4.0 uses Python version 3.10
+# Blender 4.1+ uses Python version 3.11
 
 dependencies = [
     "deadline == 0.47.*", 
     "openjd-adaptor-runtime == 0.7.*",
 ]
 
 [project.urls]
```

### Comparing `deadline_cloud_for_blender-0.3.0/PKG-INFO` & `deadline_cloud_for_blender-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline-cloud-for-blender
-Version: 0.3.0
+Version: 0.4.0
 Summary: AWS Deadline Cloud for Blender
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud-for-blender
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud-for-blender
 Author: Amazon Web Services
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
@@ -13,18 +13,19 @@
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Requires-Dist: deadline==0.47.*
 Requires-Dist: openjd-adaptor-runtime==0.7.*
 Description-Content-Type: text/markdown
 
 # AWS Deadline Cloud for Blender
 
 [![pypi](https://img.shields.io/pypi/v/deadline-cloud-for-blender.svg?style=flat)](https://pypi.python.org/pypi/deadline-cloud-for-blender)
```

