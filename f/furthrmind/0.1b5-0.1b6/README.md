# Comparing `tmp/furthrmind-0.1b5.tar.gz` & `tmp/furthrmind-0.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furthrmind-0.1b5.tar", max compression
+gzip compressed data, was "furthrmind-0.1b6.tar", max compression
```

## Comparing `furthrmind-0.1b5.tar` & `furthrmind-0.1b6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rwxr-xr-x   0        0        0    35823 2024-03-07 10:34:57.137547 furthrmind-0.1b5/LICENSE
--rwxr-xr-x   0        0        0     3328 2024-04-16 07:36:20.348303 furthrmind-0.1b5/README.md
--rwxr-xr-x   0        0        0     2353 2024-04-15 18:16:46.911920 furthrmind-0.1b5/furthrmind/__init__.py
--rwxr-xr-x   0        0        0      471 2024-03-15 09:10:04.917117 furthrmind-0.1b5/furthrmind/collection/__init__.py
--rwxr-xr-x   0        0        0    19254 2024-04-15 16:12:36.344833 furthrmind-0.1b5/furthrmind/collection/baseclass.py
--rwxr-xr-x   0        0        0     2157 2024-04-15 16:12:36.211301 furthrmind-0.1b5/furthrmind/collection/category.py
--rwxr-xr-x   0        0        0     5824 2024-04-15 16:12:36.294403 furthrmind-0.1b5/furthrmind/collection/column.py
--rwxr-xr-x   0        0        0     5946 2024-04-15 16:12:36.330101 furthrmind-0.1b5/furthrmind/collection/comboboxentry.py
--rwxr-xr-x   0        0        0     6775 2024-04-15 16:12:36.362346 furthrmind-0.1b5/furthrmind/collection/datatable.py
--rwxr-xr-x   0        0        0     6085 2024-04-15 16:12:36.202385 furthrmind-0.1b5/furthrmind/collection/experiment.py
--rwxr-xr-x   0        0        0     4805 2024-04-15 16:12:36.283804 furthrmind-0.1b5/furthrmind/collection/field.py
--rwxr-xr-x   0        0        0    10119 2024-04-15 16:12:36.242521 furthrmind-0.1b5/furthrmind/collection/fielddata.py
--rwxr-xr-x   0        0        0     1553 2024-04-15 16:12:36.336627 furthrmind-0.1b5/furthrmind/collection/file.py
--rwxr-xr-x   0        0        0     4114 2024-04-15 16:12:36.310225 furthrmind-0.1b5/furthrmind/collection/group.py
--rwxr-xr-x   0        0        0        1 2024-03-13 11:54:06.300443 furthrmind-0.1b5/furthrmind/collection/import_collection.py
--rwxr-xr-x   0        0        0     2803 2024-04-15 16:12:36.192946 furthrmind-0.1b5/furthrmind/collection/project.py
--rwxr-xr-x   0        0        0     9392 2024-04-15 16:12:36.353089 furthrmind-0.1b5/furthrmind/collection/researchitem.py
--rwxr-xr-x   0        0        0     6138 2024-04-15 16:12:36.219089 furthrmind-0.1b5/furthrmind/collection/sample.py
--rwxr-xr-x   0        0        0     4226 2024-04-15 16:12:36.302470 furthrmind-0.1b5/furthrmind/collection/unit.py
--rwxr-xr-x   0        0        0     9478 2024-03-22 14:47:35.501823 furthrmind-0.1b5/furthrmind/file_loader.py
--rwxr-xr-x   0        0        0     1058 2024-03-15 14:50:00.492475 furthrmind-0.1b5/furthrmind/utils.py
--rwxr-xr-x   0        0        0      723 2024-04-16 07:36:27.863733 furthrmind-0.1b5/pyproject.toml
--rw-r--r--   0        0        0     4165 1970-01-01 00:00:00.000000 furthrmind-0.1b5/PKG-INFO
+-rwxr-xr-x   0        0        0    35823 2024-03-07 10:34:57.137547 furthrmind-0.1b6/LICENSE
+-rwxr-xr-x   0        0        0     3326 2024-04-16 07:37:32.310043 furthrmind-0.1b6/README.md
+-rwxr-xr-x   0        0        0     2353 2024-04-15 18:16:46.911920 furthrmind-0.1b6/furthrmind/__init__.py
+-rwxr-xr-x   0        0        0      471 2024-03-15 09:10:04.917117 furthrmind-0.1b6/furthrmind/collection/__init__.py
+-rwxr-xr-x   0        0        0    20463 2024-04-16 15:02:25.552646 furthrmind-0.1b6/furthrmind/collection/baseclass.py
+-rwxr-xr-x   0        0        0     2157 2024-04-15 16:12:36.211301 furthrmind-0.1b6/furthrmind/collection/category.py
+-rwxr-xr-x   0        0        0     5824 2024-04-15 16:12:36.294403 furthrmind-0.1b6/furthrmind/collection/column.py
+-rwxr-xr-x   0        0        0     5946 2024-04-15 16:12:36.330101 furthrmind-0.1b6/furthrmind/collection/comboboxentry.py
+-rwxr-xr-x   0        0        0     6775 2024-04-15 16:12:36.362346 furthrmind-0.1b6/furthrmind/collection/datatable.py
+-rwxr-xr-x   0        0        0     6085 2024-04-15 16:12:36.202385 furthrmind-0.1b6/furthrmind/collection/experiment.py
+-rwxr-xr-x   0        0        0     4805 2024-04-15 16:12:36.283804 furthrmind-0.1b6/furthrmind/collection/field.py
+-rwxr-xr-x   0        0        0    10486 2024-04-16 14:39:14.885540 furthrmind-0.1b6/furthrmind/collection/fielddata.py
+-rwxr-xr-x   0        0        0     1553 2024-04-15 16:12:36.336627 furthrmind-0.1b6/furthrmind/collection/file.py
+-rwxr-xr-x   0        0        0     4114 2024-04-15 16:12:36.310225 furthrmind-0.1b6/furthrmind/collection/group.py
+-rwxr-xr-x   0        0        0        1 2024-03-13 11:54:06.300443 furthrmind-0.1b6/furthrmind/collection/import_collection.py
+-rwxr-xr-x   0        0        0     2803 2024-04-15 16:12:36.192946 furthrmind-0.1b6/furthrmind/collection/project.py
+-rwxr-xr-x   0        0        0     9392 2024-04-15 16:12:36.353089 furthrmind-0.1b6/furthrmind/collection/researchitem.py
+-rwxr-xr-x   0        0        0     6138 2024-04-15 16:12:36.219089 furthrmind-0.1b6/furthrmind/collection/sample.py
+-rwxr-xr-x   0        0        0     4226 2024-04-15 16:12:36.302470 furthrmind-0.1b6/furthrmind/collection/unit.py
+-rwxr-xr-x   0        0        0     9478 2024-03-22 14:47:35.501823 furthrmind-0.1b6/furthrmind/file_loader.py
+-rwxr-xr-x   0        0        0     1058 2024-03-15 14:50:00.492475 furthrmind-0.1b6/furthrmind/utils.py
+-rwxr-xr-x   0        0        0      723 2024-04-16 15:02:34.083847 furthrmind-0.1b6/pyproject.toml
+-rw-r--r--   0        0        0     4163 1970-01-01 00:00:00.000000 furthrmind-0.1b6/PKG-INFO
```

### Comparing `furthrmind-0.1b5/LICENSE` & `furthrmind-0.1b6/LICENSE`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b5/README.md` & `furthrmind-0.1b6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# furthrmind-sdk
+# furthrmind
 
-This package allows to easily interact with your FURTHRmind application in order to retrieve data or to write new
-data.
+This package allows to easily interact with your FURTHRmind application in order to 
+retrieve data or to write new data.
 
 ## Install
 ```
 pip install furthrmind
 ```
 
 ## Basic usage
@@ -22,16 +22,16 @@
 get this class either from your furthrmind instance or by importing it. 
 
 ```
 Experiment = fm.Experiment
 from furthrmind.collection import Experiment
 ```
 
-In order to get one experiment you can call the get method of the Experiment class and pass the id of the experiment
-you would like to retrieve. 
+In order to get one experiment you can call the get method of the Experiment class and 
+pass the id of the experiment you would like to retrieve. 
 
 ```
 exp = fm.Experiment.get(exp_id)
 ```
  or 
 ```
 exp = Experiment.get(exp_id)
```

### Comparing `furthrmind-0.1b5/furthrmind/__init__.py` & `furthrmind-0.1b6/furthrmind/__init__.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b5/furthrmind/collection/baseclass.py` & `furthrmind-0.1b6/furthrmind/collection/baseclass.py`

 * *Files 3% similar despite different names*

```diff
@@ -213,41 +213,41 @@
     id = None
     fielddata = []
 
 
     def __init__(self, id=None, data=None):
         super().__init__(id, data)
 
-    def update_field_value(self, value, fieldname=None, fieldid=None):
+    def update_field_value(self, value, field_name=None, field_id=None):
         """
         :param value:
             - Numeric: float or int, or a string convertable to a float
             - Date: datetime, or date object, or unix timestamp or string with iso format
             - SingleLine: string
             - ComboBoxEntry: dict with id or name as key, or string with name, or string with id
             - MultiLine: dict with content as key, or string
             - CheckBox: boolean
         :param field_name: Name of field that should be updated. Either field_name or field_id must be specified
         :param field_id: id of field that should be updated. Either field_name or field_id must be specified
         :return: id
         """
 
         fielddata = None
-        for fielddata in self.fielddata:
-            if fielddata:
+        for item in self.fielddata:
+            if item:
                 break
-            if fieldid:
-                if fielddata.fieldid == fieldid:
-                    fielddata = fielddata
-            elif fieldname:
-                if fielddata.fieldname == fieldname:
-                    fielddata = fielddata
+            if field_id:
+                if item.fieldid == field_id:
+                    fielddata = item
+            elif field_name:
+                if item.fieldname == field_name:
+                    fielddata = item
 
         if not fielddata:
-            raise ValueError("No field found with the given fieldid or fieldname")
+            raise ValueError("No field found with the given field_id or field_name")
 
         return fielddata.update_value(value)
 
     def update_field_unit(self, unit, field_name=None, field_id=None):
         """
         :param value:
             - Numeric: float or int, or a string convertable to a float
@@ -258,27 +258,57 @@
             - CheckBox: boolean
         :param field_name: Name of field that should be updated. Either field_name or field_id must be specified
         :param field_id: id of field that should be updated. Either field_name or field_id must be specified
         :return: id
         """
 
         fielddata = None
-        for fielddata in self.fielddata:
+        for item in self.fielddata:
+            if fielddata is not None:
+                break
             if field_id:
-                if fielddata.fieldid == field_id:
-                    fielddata = fielddata
+                if item.fieldid == field_id:
+                    fielddata = item
             elif field_name:
-                if fielddata.fieldname == field_name:
-                    fielddata = fielddata
+                if item.fieldname == field_name:
+                    fielddata = item
 
         if not fielddata:
-            raise ValueError("No field found with the given fieldid or fieldname")
+            raise ValueError("No field found with the given field_id or field_name")
 
         return fielddata.update_unit(unit)
 
+    def set_calculation_result(self, value: dict, field_name=None, field_id=None, fielddata_id=None):
+        """
+        :param value
+        :param field_name: Name of field that should be updated. Either field_name, field_id, fielddata_id must be specified
+        :param field_id: id of field that should be updated. Either field_name, field_id, or fielddata_id must be specified
+        :param field_data_id: id of the fielddata that should be updated. Either field_name, field_id, or fielddata_id must be specified
+        :return: id
+        """
+
+        fielddata = None
+        for item in self.fielddata:
+            if fielddata:
+                break
+            if fielddata_id:
+                if item.id == fielddata_id:
+                    fielddata = item
+            if field_id:
+                if item.fieldid == field_id:
+                    fielddata = item
+            elif field_name:
+                if item.fieldname == field_name:
+                    fielddata = item
+
+        if not fielddata:
+            raise ValueError("No field found with the given field_id or field_name")
+
+        return fielddata.set_calculation_result(value)
+
     def add_field(self, field_name=None, field_type=None, field_id=None,
                   value=None, unit=None) -> "FieldData":
         """
         :param field_name: Name of field that should be added. If fieldname provided,
                             also fieldtype must be specified. Either fieldname and fieldtype or field_id must be specified
         :param field_type: Type of field: Must be out of: Numeric, Date, SingleLine
                                                         ComboBoxEntry, MultiLine, CheckBox
```

### Comparing `furthrmind-0.1b5/furthrmind/collection/category.py` & `furthrmind-0.1b6/furthrmind/collection/category.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b5/furthrmind/collection/column.py` & `furthrmind-0.1b6/furthrmind/collection/column.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b5/furthrmind/collection/comboboxentry.py` & `furthrmind-0.1b6/furthrmind/collection/comboboxentry.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b5/furthrmind/collection/datatable.py` & `furthrmind-0.1b6/furthrmind/collection/datatable.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b5/furthrmind/collection/experiment.py` & `furthrmind-0.1b6/furthrmind/collection/experiment.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b5/furthrmind/collection/field.py` & `furthrmind-0.1b6/furthrmind/collection/field.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b5/furthrmind/collection/fielddata.py` & `furthrmind-0.1b6/furthrmind/collection/fielddata.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from ..utils import furthr_wrap
-from functools import wraps
-from furthrmind.collection.baseclass import BaseClass
 from datetime import datetime, date
+
 from bson import ObjectId
-from furthrmind.utils import instance_overload
 from typing_extensions import List, TYPE_CHECKING
+
+from furthrmind.collection.baseclass import BaseClass
+from furthrmind.utils import instance_overload
+
 if TYPE_CHECKING:
     from furthrmind.collection.unit import Unit
 
 
 class FieldData(BaseClass):
     id = ""
     field_name = ""
     field_id = ""
     field_type = ""
     si_value = None
     unit: List["Unit"] = None
     author = None
     value = None
 
-
     _attr_definition = {
         "unit": {"class": "Unit"},
         "field_name": {"data_key": "fieldname"},
         "field_type": {"data_key": "fieldtype"},
         "field_id": {"data_key": "fieldid"},
     }
 
@@ -57,21 +57,34 @@
             - Date: datetime, or date object, or unix timestamp or string with iso format
             - SingleLine: string
             - ComboBoxEntry: dict with id or name as key, or string with name, or string with id
             - MultiLine: dict with content as key, or string
             - CheckBox: boolean
         :return: id
         """
-        value = self.__class__._check_value_type(value, self.fieldtype)
+        value = self.__class__._check_value_type(value, self.field_type)
         data = {"id": self.id,
                 "value": value}
         id = self.post(data)
         self.value = value
         return id
 
+    def set_calculation_result(self, value: dict):
+        """
+        Method to set a calculation result
+        :param value: dict
+        :return: id
+        """
+        if not self.field_type in ["Calculation", "RawDataCalc"]:
+            raise TypeError("Only applicable for calculation field")
+
+        url = f"{self.fm.base_url}/set-result/{self.id}"
+        self.fm.session.post(url, value)
+        return self.id
+
     @classmethod
     def _check_value_type(cls, value, fieldtype=None):
         if value is None:
             return value
         if issubclass(cls, BaseClass):
             # classmethod
             if fieldtype is None:
@@ -274,22 +287,21 @@
                 field = Field(id=field_id)
                 field.get()
                 field_type = field.type
             else:
                 if not field_name or not field_type:
                     raise ValueError("field_name and field_type must be specified")
                 _data = {"fieldname": field_name,
-                        "fieldtype": field_type}
+                         "fieldtype": field_type}
 
             value = FieldData._check_value_type(value, field_type)
             _data["value"] = value
 
             if unit:
                 unit = FieldData._check_unit(unit)
                 _data["unit"] = unit
             post_data_list.append(_data)
 
-
         id_list = FieldData.post(post_data_list, project_id)
         for data, id in zip(data_list, id_list):
             data["id"] = id
-        return data_list
+        return data_list
```

### Comparing `furthrmind-0.1b5/furthrmind/collection/file.py` & `furthrmind-0.1b6/furthrmind/collection/file.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b5/furthrmind/collection/group.py` & `furthrmind-0.1b6/furthrmind/collection/group.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b5/furthrmind/collection/project.py` & `furthrmind-0.1b6/furthrmind/collection/project.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b5/furthrmind/collection/researchitem.py` & `furthrmind-0.1b6/furthrmind/collection/researchitem.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b5/furthrmind/collection/sample.py` & `furthrmind-0.1b6/furthrmind/collection/sample.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b5/furthrmind/collection/unit.py` & `furthrmind-0.1b6/furthrmind/collection/unit.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b5/furthrmind/file_loader.py` & `furthrmind-0.1b6/furthrmind/file_loader.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b5/furthrmind/utils.py` & `furthrmind-0.1b6/furthrmind/utils.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b5/pyproject.toml` & `furthrmind-0.1b6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "furthrmind"
-version = "0.1b5"
+version = "0.1b6"
 description = "Official python wrapper for the FURTHRmind rest api."
 authors = ["Daniel Menne"]
 license = "GNU GENERAL PUBLIC LICENSE Version 3"
 readme = "README.md"
 repository = "https://github.com/FURTHRresearch/furthrmind-sdk"
 
 [tool.poetry.dependencies]
```

### Comparing `furthrmind-0.1b5/PKG-INFO` & `furthrmind-0.1b6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: furthrmind
-Version: 0.1b5
+Version: 0.1b6
 Summary: Official python wrapper for the FURTHRmind rest api.
 Home-page: https://github.com/FURTHRresearch/furthrmind-sdk
 License: GNU GENERAL PUBLIC LICENSE Version 3
 Author: Daniel Menne
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -15,18 +15,18 @@
 Requires-Dist: pathvalidate (>=3.2.0,<4.0.0)
 Requires-Dist: pymongo (>=4.6.2,<5.0.0)
 Requires-Dist: requests
 Requires-Dist: typing-extensions (>=4.10.0,<5.0.0)
 Project-URL: Repository, https://github.com/FURTHRresearch/furthrmind-sdk
 Description-Content-Type: text/markdown
 
-# furthrmind-sdk
+# furthrmind
 
-This package allows to easily interact with your FURTHRmind application in order to retrieve data or to write new
-data.
+This package allows to easily interact with your FURTHRmind application in order to 
+retrieve data or to write new data.
 
 ## Install
 ```
 pip install furthrmind
 ```
 
 ## Basic usage
@@ -43,16 +43,16 @@
 get this class either from your furthrmind instance or by importing it. 
 
 ```
 Experiment = fm.Experiment
 from furthrmind.collection import Experiment
 ```
 
-In order to get one experiment you can call the get method of the Experiment class and pass the id of the experiment
-you would like to retrieve. 
+In order to get one experiment you can call the get method of the Experiment class and 
+pass the id of the experiment you would like to retrieve. 
 
 ```
 exp = fm.Experiment.get(exp_id)
 ```
  or 
 ```
 exp = Experiment.get(exp_id)
```

