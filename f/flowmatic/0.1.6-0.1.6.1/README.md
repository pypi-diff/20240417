# Comparing `tmp/flowmatic-0.1.6.tar.gz` & `tmp/flowmatic-0.1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowmatic-0.1.6.tar", max compression
+gzip compressed data, was "flowmatic-0.1.6.1.tar", max compression
```

## Comparing `flowmatic-0.1.6.tar` & `flowmatic-0.1.6.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1532 2024-04-17 06:42:47.608678 flowmatic-0.1.6/assets/icons/Code.png
--rw-r--r--   0        0        0      838 2024-04-17 06:42:47.610179 flowmatic-0.1.6/assets/icons/File.png
--rw-r--r--   0        0        0     1346 2024-04-17 06:42:47.610679 flowmatic-0.1.6/assets/icons/Image.png
--rw-r--r--   0        0        0     2210 2024-04-17 06:42:47.611680 flowmatic-0.1.6/assets/icons/PDF.png
--rw-r--r--   0        0        0     1048 2024-04-17 06:42:47.612680 flowmatic-0.1.6/assets/icons/Table.png
--rw-r--r--   0        0        0      965 2024-04-17 06:42:47.613684 flowmatic-0.1.6/assets/icons/Text.png
--rw-r--r--   0        0        0     1207 2024-04-17 06:42:47.615180 flowmatic-0.1.6/assets/icons/Zip.png
--rw-r--r--   0        0        0     1919 2024-04-17 06:42:47.619682 flowmatic-0.1.6/flowmatic/__init__.py
--rw-r--r--   0        0        0     2317 2024-04-17 06:42:47.620181 flowmatic-0.1.6/flowmatic/flowmatic.py
--rw-r--r--   0        0        0       24 2024-04-17 06:42:47.622179 flowmatic-0.1.6/flowmatic/flows/__init__.py
--rw-r--r--   0        0        0      951 2024-04-17 06:42:47.623181 flowmatic-0.1.6/flowmatic/flows/flow.py
--rw-r--r--   0        0        0       63 2024-04-17 06:42:47.625681 flowmatic-0.1.6/flowmatic/forms/__init__.py
--rw-r--r--   0        0        0      233 2024-04-17 06:42:47.627182 flowmatic-0.1.6/flowmatic/forms/fields/__init__.py
--rw-r--r--   0        0        0     1255 2024-04-17 06:42:47.628179 flowmatic-0.1.6/flowmatic/forms/fields/check_box.py
--rw-r--r--   0        0        0     1527 2024-04-17 06:42:47.629180 flowmatic-0.1.6/flowmatic/forms/fields/date_select.py
--rw-r--r--   0        0        0     1266 2024-04-17 06:42:47.630179 flowmatic-0.1.6/flowmatic/forms/fields/display.py
--rw-r--r--   0        0        0      688 2024-04-17 06:42:47.631690 flowmatic-0.1.6/flowmatic/forms/fields/field.py
--rw-r--r--   0        0        0     6014 2024-04-17 06:42:47.632679 flowmatic-0.1.6/flowmatic/forms/fields/file_field.py
--rw-r--r--   0        0        0     1433 2024-04-17 06:42:47.633680 flowmatic-0.1.6/flowmatic/forms/fields/radio_group.py
--rw-r--r--   0        0        0     1755 2024-04-17 06:42:47.634679 flowmatic-0.1.6/flowmatic/forms/fields/text_field.py
--rw-r--r--   0        0        0      685 2024-04-17 06:42:47.635679 flowmatic-0.1.6/flowmatic/forms/validation.py
--rw-r--r--   0        0        0      182 2024-04-17 06:42:47.637679 flowmatic-0.1.6/flowmatic/gui/__init__.py
--rw-r--r--   0        0        0      105 2024-04-17 06:42:47.638688 flowmatic-0.1.6/flowmatic/gui/constants.py
--rw-r--r--   0        0        0       64 2024-04-17 06:42:47.640679 flowmatic-0.1.6/flowmatic/gui/elements/__init__.py
--rw-r--r--   0        0        0      276 2024-04-17 06:42:47.641680 flowmatic-0.1.6/flowmatic/gui/elements/element_infos.py
--rw-r--r--   0        0        0      906 2024-04-17 06:42:47.643181 flowmatic-0.1.6/flowmatic/gui/gui.py
--rw-r--r--   0        0        0      284 2024-04-17 06:42:47.644680 flowmatic-0.1.6/flowmatic/gui/screens/__init__.py
--rw-r--r--   0        0        0     1611 2024-04-17 06:42:47.645680 flowmatic-0.1.6/flowmatic/gui/screens/element_screen.py
--rw-r--r--   0        0        0     5186 2024-04-17 06:42:47.647180 flowmatic-0.1.6/flowmatic/gui/screens/form_screen.py
--rw-r--r--   0        0        0      799 2024-04-17 06:42:47.648681 flowmatic-0.1.6/flowmatic/gui/screens/menu_screen.py
--rw-r--r--   0        0        0     5449 2024-04-17 06:42:47.649681 flowmatic-0.1.6/flowmatic/gui/screens/result_screen.py
--rw-r--r--   0        0        0     2230 2024-04-17 06:42:47.650680 flowmatic-0.1.6/flowmatic/gui/screens/screen.py
--rw-r--r--   0        0        0      716 2024-04-17 06:42:47.651680 flowmatic-0.1.6/flowmatic/gui/screens/title_screen.py
--rw-r--r--   0        0        0       29 2024-04-17 06:42:47.654180 flowmatic-0.1.6/flowmatic/gui/style/__init__.py
--rw-r--r--   0        0        0      103 2024-04-17 06:42:47.655182 flowmatic-0.1.6/flowmatic/gui/style/style.py
--rw-r--r--   0        0        0     3204 2024-04-17 06:42:47.656182 flowmatic-0.1.6/flowmatic/gui/tkgui.py
--rw-r--r--   0        0        0       54 2024-04-17 06:42:47.618679 flowmatic-0.1.6/flowmatic/README.md
--rw-r--r--   0        0        0       61 2024-04-17 06:42:47.657183 flowmatic-0.1.6/flowmatic/server.py
--rw-r--r--   0        0        0      247 2024-04-17 06:42:47.658679 flowmatic-0.1.6/flowmatic/util/__init__.py
--rw-r--r--   0        0        0      792 2024-04-17 06:42:47.659681 flowmatic-0.1.6/flowmatic/util/exceptions.py
--rw-r--r--   0        0        0     1171 2024-04-17 06:42:47.660679 flowmatic-0.1.6/flowmatic/util/icons.py
--rw-r--r--   0        0        0     1752 2024-04-17 06:42:47.661681 flowmatic-0.1.6/flowmatic/util/saved_class.py
--rw-r--r--   0        0        0       82 2024-04-17 06:42:47.663182 flowmatic-0.1.6/flowmatic/util/settings.py
--rw-r--r--   0        0        0      232 2024-04-17 06:42:47.664182 flowmatic-0.1.6/flowmatic/util/singleton.py
--rw-r--r--   0        0        0       78 2024-04-17 06:42:47.665182 flowmatic-0.1.6/flowmatic/util/user.py
--rw-r--r--   0        0        0      451 2024-04-17 07:46:43.010183 flowmatic-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       49 2024-04-17 06:42:47.604181 flowmatic-0.1.6/README.md
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 flowmatic-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1532 2024-04-17 06:42:47.608678 flowmatic-0.1.6.1/assets/icons/Code.png
+-rw-r--r--   0        0        0      838 2024-04-17 06:42:47.610179 flowmatic-0.1.6.1/assets/icons/File.png
+-rw-r--r--   0        0        0     1346 2024-04-17 06:42:47.610679 flowmatic-0.1.6.1/assets/icons/Image.png
+-rw-r--r--   0        0        0     2210 2024-04-17 06:42:47.611680 flowmatic-0.1.6.1/assets/icons/PDF.png
+-rw-r--r--   0        0        0     1048 2024-04-17 06:42:47.612680 flowmatic-0.1.6.1/assets/icons/Table.png
+-rw-r--r--   0        0        0      965 2024-04-17 06:42:47.613684 flowmatic-0.1.6.1/assets/icons/Text.png
+-rw-r--r--   0        0        0     1207 2024-04-17 06:42:47.615180 flowmatic-0.1.6.1/assets/icons/Zip.png
+-rw-r--r--   0        0        0     1919 2024-04-17 06:42:47.619682 flowmatic-0.1.6.1/flowmatic/__init__.py
+-rw-r--r--   0        0        0     2317 2024-04-17 06:42:47.620181 flowmatic-0.1.6.1/flowmatic/flowmatic.py
+-rw-r--r--   0        0        0       24 2024-04-17 06:42:47.622179 flowmatic-0.1.6.1/flowmatic/flows/__init__.py
+-rw-r--r--   0        0        0      951 2024-04-17 06:42:47.623181 flowmatic-0.1.6.1/flowmatic/flows/flow.py
+-rw-r--r--   0        0        0       63 2024-04-17 06:42:47.625681 flowmatic-0.1.6.1/flowmatic/forms/__init__.py
+-rw-r--r--   0        0        0      233 2024-04-17 06:42:47.627182 flowmatic-0.1.6.1/flowmatic/forms/fields/__init__.py
+-rw-r--r--   0        0        0     1255 2024-04-17 06:42:47.628179 flowmatic-0.1.6.1/flowmatic/forms/fields/check_box.py
+-rw-r--r--   0        0        0     1527 2024-04-17 06:42:47.629180 flowmatic-0.1.6.1/flowmatic/forms/fields/date_select.py
+-rw-r--r--   0        0        0     1266 2024-04-17 06:42:47.630179 flowmatic-0.1.6.1/flowmatic/forms/fields/display.py
+-rw-r--r--   0        0        0      688 2024-04-17 06:42:47.631690 flowmatic-0.1.6.1/flowmatic/forms/fields/field.py
+-rw-r--r--   0        0        0     6014 2024-04-17 06:42:47.632679 flowmatic-0.1.6.1/flowmatic/forms/fields/file_field.py
+-rw-r--r--   0        0        0     1433 2024-04-17 06:42:47.633680 flowmatic-0.1.6.1/flowmatic/forms/fields/radio_group.py
+-rw-r--r--   0        0        0     1755 2024-04-17 06:42:47.634679 flowmatic-0.1.6.1/flowmatic/forms/fields/text_field.py
+-rw-r--r--   0        0        0      685 2024-04-17 06:42:47.635679 flowmatic-0.1.6.1/flowmatic/forms/validation.py
+-rw-r--r--   0        0        0      182 2024-04-17 06:42:47.637679 flowmatic-0.1.6.1/flowmatic/gui/__init__.py
+-rw-r--r--   0        0        0      105 2024-04-17 06:42:47.638688 flowmatic-0.1.6.1/flowmatic/gui/constants.py
+-rw-r--r--   0        0        0       64 2024-04-17 06:42:47.640679 flowmatic-0.1.6.1/flowmatic/gui/elements/__init__.py
+-rw-r--r--   0        0        0      276 2024-04-17 06:42:47.641680 flowmatic-0.1.6.1/flowmatic/gui/elements/element_infos.py
+-rw-r--r--   0        0        0      906 2024-04-17 06:42:47.643181 flowmatic-0.1.6.1/flowmatic/gui/gui.py
+-rw-r--r--   0        0        0      284 2024-04-17 06:42:47.644680 flowmatic-0.1.6.1/flowmatic/gui/screens/__init__.py
+-rw-r--r--   0        0        0     1611 2024-04-17 06:42:47.645680 flowmatic-0.1.6.1/flowmatic/gui/screens/element_screen.py
+-rw-r--r--   0        0        0     5186 2024-04-17 06:42:47.647180 flowmatic-0.1.6.1/flowmatic/gui/screens/form_screen.py
+-rw-r--r--   0        0        0      799 2024-04-17 06:42:47.648681 flowmatic-0.1.6.1/flowmatic/gui/screens/menu_screen.py
+-rw-r--r--   0        0        0     5449 2024-04-17 06:42:47.649681 flowmatic-0.1.6.1/flowmatic/gui/screens/result_screen.py
+-rw-r--r--   0        0        0     2230 2024-04-17 06:42:47.650680 flowmatic-0.1.6.1/flowmatic/gui/screens/screen.py
+-rw-r--r--   0        0        0      716 2024-04-17 06:42:47.651680 flowmatic-0.1.6.1/flowmatic/gui/screens/title_screen.py
+-rw-r--r--   0        0        0       29 2024-04-17 06:42:47.654180 flowmatic-0.1.6.1/flowmatic/gui/style/__init__.py
+-rw-r--r--   0        0        0      103 2024-04-17 06:42:47.655182 flowmatic-0.1.6.1/flowmatic/gui/style/style.py
+-rw-r--r--   0        0        0     3204 2024-04-17 06:42:47.656182 flowmatic-0.1.6.1/flowmatic/gui/tkgui.py
+-rw-r--r--   0        0        0       54 2024-04-17 06:42:47.618679 flowmatic-0.1.6.1/flowmatic/README.md
+-rw-r--r--   0        0        0       61 2024-04-17 06:42:47.657183 flowmatic-0.1.6.1/flowmatic/server.py
+-rw-r--r--   0        0        0      247 2024-04-17 06:42:47.658679 flowmatic-0.1.6.1/flowmatic/util/__init__.py
+-rw-r--r--   0        0        0      792 2024-04-17 06:42:47.659681 flowmatic-0.1.6.1/flowmatic/util/exceptions.py
+-rw-r--r--   0        0        0     1171 2024-04-17 06:42:47.660679 flowmatic-0.1.6.1/flowmatic/util/icons.py
+-rw-r--r--   0        0        0     1752 2024-04-17 06:42:47.661681 flowmatic-0.1.6.1/flowmatic/util/saved_class.py
+-rw-r--r--   0        0        0       82 2024-04-17 06:42:47.663182 flowmatic-0.1.6.1/flowmatic/util/settings.py
+-rw-r--r--   0        0        0      232 2024-04-17 06:42:47.664182 flowmatic-0.1.6.1/flowmatic/util/singleton.py
+-rw-r--r--   0        0        0       78 2024-04-17 06:42:47.665182 flowmatic-0.1.6.1/flowmatic/util/user.py
+-rw-r--r--   0        0        0      453 2024-04-17 08:01:03.066678 flowmatic-0.1.6.1/pyproject.toml
+-rw-r--r--   0        0        0       49 2024-04-17 06:42:47.604181 flowmatic-0.1.6.1/README.md
+-rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 flowmatic-0.1.6.1/PKG-INFO
```

### Comparing `flowmatic-0.1.6/assets/icons/Code.png` & `flowmatic-0.1.6.1/assets/icons/Code.png`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/assets/icons/File.png` & `flowmatic-0.1.6.1/assets/icons/File.png`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/assets/icons/Image.png` & `flowmatic-0.1.6.1/assets/icons/Image.png`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/assets/icons/PDF.png` & `flowmatic-0.1.6.1/assets/icons/PDF.png`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/assets/icons/Table.png` & `flowmatic-0.1.6.1/assets/icons/Table.png`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/assets/icons/Text.png` & `flowmatic-0.1.6.1/assets/icons/Text.png`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/assets/icons/Zip.png` & `flowmatic-0.1.6.1/assets/icons/Zip.png`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/flowmatic/__init__.py` & `flowmatic-0.1.6.1/flowmatic/__init__.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/flowmatic/flowmatic.py` & `flowmatic-0.1.6.1/flowmatic/flowmatic.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/flowmatic/flows/flow.py` & `flowmatic-0.1.6.1/flowmatic/flows/flow.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/flowmatic/forms/fields/check_box.py` & `flowmatic-0.1.6.1/flowmatic/forms/fields/check_box.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/flowmatic/forms/fields/date_select.py` & `flowmatic-0.1.6.1/flowmatic/forms/fields/date_select.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/flowmatic/forms/fields/display.py` & `flowmatic-0.1.6.1/flowmatic/forms/fields/display.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/flowmatic/forms/fields/field.py` & `flowmatic-0.1.6.1/flowmatic/forms/fields/field.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/flowmatic/forms/fields/file_field.py` & `flowmatic-0.1.6.1/flowmatic/forms/fields/file_field.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/flowmatic/forms/fields/radio_group.py` & `flowmatic-0.1.6.1/flowmatic/forms/fields/radio_group.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/flowmatic/forms/fields/text_field.py` & `flowmatic-0.1.6.1/flowmatic/forms/fields/text_field.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/flowmatic/forms/validation.py` & `flowmatic-0.1.6.1/flowmatic/forms/validation.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/flowmatic/gui/gui.py` & `flowmatic-0.1.6.1/flowmatic/gui/gui.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/flowmatic/gui/screens/element_screen.py` & `flowmatic-0.1.6.1/flowmatic/gui/screens/element_screen.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/flowmatic/gui/screens/form_screen.py` & `flowmatic-0.1.6.1/flowmatic/gui/screens/form_screen.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/flowmatic/gui/screens/menu_screen.py` & `flowmatic-0.1.6.1/flowmatic/gui/screens/menu_screen.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/flowmatic/gui/screens/result_screen.py` & `flowmatic-0.1.6.1/flowmatic/gui/screens/result_screen.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/flowmatic/gui/screens/screen.py` & `flowmatic-0.1.6.1/flowmatic/gui/screens/screen.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/flowmatic/gui/screens/title_screen.py` & `flowmatic-0.1.6.1/flowmatic/gui/screens/title_screen.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/flowmatic/gui/tkgui.py` & `flowmatic-0.1.6.1/flowmatic/gui/tkgui.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/flowmatic/util/exceptions.py` & `flowmatic-0.1.6.1/flowmatic/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/flowmatic/util/icons.py` & `flowmatic-0.1.6.1/flowmatic/util/icons.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/flowmatic/util/saved_class.py` & `flowmatic-0.1.6.1/flowmatic/util/saved_class.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.6/PKG-INFO` & `flowmatic-0.1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowmatic
-Version: 0.1.6
+Version: 0.1.6.1
 Summary: 
 Author: aeteseb
 Author-email: 113799213+aeteseb@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

