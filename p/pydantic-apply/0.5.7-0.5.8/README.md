# Comparing `tmp/pydantic_apply-0.5.7.tar.gz` & `tmp/pydantic_apply-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_apply-0.5.7.tar", max compression
+gzip compressed data, was "pydantic_apply-0.5.8.tar", max compression
```

## Comparing `pydantic_apply-0.5.7.tar` & `pydantic_apply-0.5.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1078 2024-01-04 21:01:46.829128 pydantic_apply-0.5.7/LICENSE
--rw-r--r--   0        0        0     2264 2024-01-04 21:01:46.829128 pydantic_apply-0.5.7/README.md
--rw-r--r--   0        0        0       35 2024-01-04 21:01:46.829128 pydantic_apply-0.5.7/pydantic_apply/__init__.py
--rw-r--r--   0        0        0     2439 2024-01-04 21:01:46.829128 pydantic_apply-0.5.7/pydantic_apply/_compat.py
--rw-r--r--   0        0        0     5179 2024-01-04 21:01:46.829128 pydantic_apply-0.5.7/pydantic_apply/apply.py
--rw-r--r--   0        0        0        0 2024-01-04 21:01:46.829128 pydantic_apply-0.5.7/pydantic_apply/py.typed
--rw-r--r--   0        0        0      821 2024-01-04 21:01:46.829128 pydantic_apply-0.5.7/pydantic_apply/utils.py
--rw-r--r--   0        0        0      969 2024-01-04 21:01:46.829128 pydantic_apply-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     3018 1970-01-01 00:00:00.000000 pydantic_apply-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-17 07:31:05.933096 pydantic_apply-0.5.8/LICENSE
+-rw-r--r--   0        0        0     2264 2024-04-17 07:31:05.933096 pydantic_apply-0.5.8/README.md
+-rw-r--r--   0        0        0       54 2024-04-17 07:31:05.933096 pydantic_apply-0.5.8/pydantic_apply/__init__.py
+-rw-r--r--   0        0        0     2558 2024-04-17 07:31:05.933096 pydantic_apply-0.5.8/pydantic_apply/_compat.py
+-rw-r--r--   0        0        0     5208 2024-04-17 07:31:05.933096 pydantic_apply-0.5.8/pydantic_apply/apply.py
+-rw-r--r--   0        0        0        0 2024-04-17 07:31:05.933096 pydantic_apply-0.5.8/pydantic_apply/py.typed
+-rw-r--r--   0        0        0      821 2024-04-17 07:31:05.933096 pydantic_apply-0.5.8/pydantic_apply/utils.py
+-rw-r--r--   0        0        0      995 2024-04-17 07:31:05.933096 pydantic_apply-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0     3018 1970-01-01 00:00:00.000000 pydantic_apply-0.5.8/PKG-INFO
```

### Comparing `pydantic_apply-0.5.7/LICENSE` & `pydantic_apply-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_apply-0.5.7/README.md` & `pydantic_apply-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_apply-0.5.7/pydantic_apply/_compat.py` & `pydantic_apply-0.5.8/pydantic_apply/_compat.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Any, Dict, Optional, Set, Type
+from typing import Any, Dict, Set, Type
 
 import pydantic
 from pydantic.fields import FieldInfo
 from pydantic.version import VERSION as PYDANTIC_VERSION
 
 PYDANTIC_V1 = PYDANTIC_VERSION.startswith("1.")
 PYDANTIC_V2 = PYDANTIC_VERSION.startswith("2.")
 
 
 if PYDANTIC_V1:  # pragma: no cover
-    class PydanticCompat:
+    class PydanticCompat:  # type: ignore
         obj: pydantic.BaseModel
 
         def __init__(
             self,
             obj: pydantic.BaseModel,
         ) -> None:
             self.obj = obj
@@ -56,15 +56,17 @@
         def model_fields(self) -> Dict[str, FieldInfo]:
             return self.obj.model_fields
 
         @property
         def __pydantic_fields_set__(self) -> Set[str]:
             return self.obj.__pydantic_fields_set__
 
-        def get_model_field_info_annotation(self, model_field: FieldInfo) -> Optional[Type[Any]]:
+        def get_model_field_info_annotation(self, model_field: FieldInfo) -> Type[Any]:
+            if model_field.annotation is None:
+                raise RuntimeError("model field has not typing annotation")
             return model_field.annotation
 
         def get_model_config_value(self, key: str) -> Any:
             return self.obj.model_config.get(key, None)
 
         def set_model_config_value(self, key: str, value: Any) -> None:
             self.obj.model_config[key] = value  # type: ignore
```

### Comparing `pydantic_apply-0.5.7/pydantic_apply/apply.py` & `pydantic_apply-0.5.8/pydantic_apply/apply.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import warnings
-from typing import Any, Dict, Union
+from typing import Any, Dict, Union, cast
 
 import pydantic
 
 from pydantic_apply._compat import PydanticCompat
 from pydantic_apply.utils import is_pydantic_apply_annotation
 
 
@@ -60,15 +60,15 @@
                     # When validation on assignment is enabled we need to
                     # copy the current value first. Otherwise, the validation
                     # might have issues, see below.
                     if self_compat.get_model_config_value("validate_assignment"):
                         current_value = PydanticCompat(current_value).model_copy()
 
                     # ...then use `.apply(...)` on the current value to prepare changes
-                    current_value.model_apply(changed_field_value)
+                    cast(ApplyModelMixin, current_value).model_apply(changed_field_value)
                     prepared_changes[field_name] = current_value
                     continue
 
             # Default apply: Just set new value
             prepared_changes[field_name] = changed_field_value
 
         # Apply changes
```

### Comparing `pydantic_apply-0.5.7/pydantic_apply/utils.py` & `pydantic_apply-0.5.8/pydantic_apply/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_apply-0.5.7/pyproject.toml` & `pydantic_apply-0.5.8/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 [tool.poetry]
 name = "pydantic-apply"
-version = "0.5.7"
+version = "0.5.8"
 description = "Apply changes as patches to pydanic models."
 authors = ["TEAM23 GmbH <info@team23.de>"]
 license = "MIT"
 repository = "https://github.com/team23/pydantic-apply"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = ">=1.9.0,<3.0.0"
 
 [tool.poetry.group.dev.dependencies]
-pytest = ">=7.1.2,<8.0.0"
-pytest-cov = ">=3,<5"
-mypy = ">=0.971,<2.0"
+pytest = ">=7.1.2,<9.0.0"
+pytest-cov = ">=3,<6"
 tox = ">=3.26,<5.0"
-ruff = ">=0.0.284,<0.2.0"
+ruff = ">=0.2.0,<0.4.0"
+pyright = ">=1.1.350,<1.2"
 
 [tool.ruff]
-select = ["F","E","W","C","I","N","UP","ANN","S","B","A","COM","C4","T20","PT","ARG","TD","RUF"]
 line-length = 115
 target-version = "py38"
-ignore = ["A001","A002","A003","ANN101","ANN102","ANN401","C901","N8","B008","F405","F821"]
 output-format = "grouped"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint]
+select = ["F","E","W","C","I","N","UP","ANN","S","B","A","COM","C4","T20","PT","ARG","TD","RUF"]
+ignore = ["A001","A002","A003","ANN101","ANN102","ANN401","C901","N8","B008","F405","F821"]
+
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
 "conftest.py" = ["S101","ANN","F401"]
 "test_*.py" = ["S101","ANN","F401"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pydantic_apply-0.5.7/PKG-INFO` & `pydantic_apply-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-apply
-Version: 0.5.7
+Version: 0.5.8
 Summary: Apply changes as patches to pydanic models.
 Home-page: https://github.com/team23/pydantic-apply
 License: MIT
 Author: TEAM23 GmbH
 Author-email: info@team23.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

