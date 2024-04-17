# Comparing `tmp/pydantic_partial-0.5.4.tar.gz` & `tmp/pydantic_partial-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_partial-0.5.4.tar", max compression
+gzip compressed data, was "pydantic_partial-0.5.5.tar", max compression
```

## Comparing `pydantic_partial-0.5.4.tar` & `pydantic_partial-0.5.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2024-01-04 20:56:47.161029 pydantic_partial-0.5.4/LICENSE
--rw-r--r--   0        0        0     5597 2024-01-04 20:56:47.161029 pydantic_partial-0.5.4/README.md
--rw-r--r--   0        0        0       61 2024-01-04 20:56:47.161029 pydantic_partial-0.5.4/pydantic_partial/__init__.py
--rw-r--r--   0        0        0     2409 2024-01-04 20:56:47.161029 pydantic_partial-0.5.4/pydantic_partial/_compat.py
--rw-r--r--   0        0        0     5661 2024-01-04 20:56:47.161029 pydantic_partial-0.5.4/pydantic_partial/partial.py
--rw-r--r--   0        0        0        0 2024-01-04 20:56:47.161029 pydantic_partial-0.5.4/pydantic_partial/py.typed
--rw-r--r--   0        0        0     1034 2024-01-04 20:56:47.161029 pydantic_partial-0.5.4/pydantic_partial/utils.py
--rw-r--r--   0        0        0     1035 2024-01-04 20:56:47.161029 pydantic_partial-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     6369 1970-01-01 00:00:00.000000 pydantic_partial-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-17 07:41:12.379245 pydantic_partial-0.5.5/LICENSE
+-rw-r--r--   0        0        0     5605 2024-04-17 07:41:12.379245 pydantic_partial-0.5.5/README.md
+-rw-r--r--   0        0        0      126 2024-04-17 07:41:12.379245 pydantic_partial-0.5.5/pydantic_partial/__init__.py
+-rw-r--r--   0        0        0     2435 2024-04-17 07:41:12.379245 pydantic_partial-0.5.5/pydantic_partial/_compat.py
+-rw-r--r--   0        0        0     5742 2024-04-17 07:41:12.379245 pydantic_partial-0.5.5/pydantic_partial/partial.py
+-rw-r--r--   0        0        0        0 2024-04-17 07:41:12.379245 pydantic_partial-0.5.5/pydantic_partial/py.typed
+-rw-r--r--   0        0        0     1034 2024-04-17 07:41:12.379245 pydantic_partial-0.5.5/pydantic_partial/utils.py
+-rw-r--r--   0        0        0     1061 2024-04-17 07:41:12.379245 pydantic_partial-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     6377 1970-01-01 00:00:00.000000 pydantic_partial-0.5.5/PKG-INFO
```

### Comparing `pydantic_partial-0.5.4/LICENSE` & `pydantic_partial-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_partial-0.5.4/README.md` & `pydantic_partial-0.5.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pydantic-partial
 
 ## Installation
 
 Just use `pip install pydantic-partial` to install the library.
 
 **Note:** `pydantic-partial` is compatible with `pydantic` versions `1.9`, `1.10` and even `2.x` (🥳) on
-Python `3.9`, `3.10` and `3.11`. This is also ensured running all tests on all those versions
+Python `3.9`, `3.10`, `3.11` and `3.12`. This is also ensured running all tests on all those versions
 using `tox`.
 
 ## About
 
 Create partial models from your normal pydantic models. Partial models will allow
 some or all fields to be optional and thus not be required when creating the model
 instance.
```

### Comparing `pydantic_partial-0.5.4/pydantic_partial/_compat.py` & `pydantic_partial-0.5.5/pydantic_partial/_compat.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 NULLABLE_KWARGS: dict[str, Any]
 
 if PYDANTIC_V1:  # pragma: no cover
     from pydantic.fields import ModelField  # type: ignore
 
     NULLABLE_KWARGS = {"nullable": True}
 
-    class PydanticCompat:
+    class PydanticCompat:  # type: ignore
         model_class: type[pydantic.BaseModel]
 
         def __init__(
             self,
             model_class: type[pydantic.BaseModel],
         ) -> None:
             self.model_class = model_class
@@ -38,15 +38,15 @@
 
         def is_model_field_info_required(self, model_field: ModelField) -> bool:
             return (
                 model_field.required
                 or model_field.default is not None
             )
 
-        def copy_model_field_info(self, model_field: ModelField, **kwargs: Any) -> bool:
+        def copy_model_field_info(self, model_field: ModelField, **kwargs: Any) -> FieldInfo:
             return copy_field_info(model_field.field_info, **kwargs)
 
 elif PYDANTIC_V2:  # pragma: no cover
     NULLABLE_KWARGS = {"json_schema_extra": {"nullable": True}}
 
     class PydanticCompat:  # type: ignore
         model_class: type[pydantic.BaseModel]
@@ -63,9 +63,9 @@
 
         def get_model_field_info_annotation(self, field_info: FieldInfo) -> Optional[type[Any]]:
             return field_info.annotation
 
         def is_model_field_info_required(self, field_info: FieldInfo) -> bool:
             return field_info.is_required()  # type: ignore
 
-        def copy_model_field_info(self, field_info: FieldInfo, **kwargs: Any) -> bool:
+        def copy_model_field_info(self, field_info: FieldInfo, **kwargs: Any) -> FieldInfo:
             return copy_field_info(field_info, **kwargs)
```

### Comparing `pydantic_partial-0.5.4/pydantic_partial/partial.py` & `pydantic_partial-0.5.5/pydantic_partial/partial.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # You could also create a "partial Partial":
 #AgeSomethingPartial = Something.as_partial("age")
 ```
 """
 
 import functools
 import warnings
-from typing import Any, Optional, TypeVar, Union, get_args, get_origin
+from typing import Any, Optional, TypeVar, Union, cast, get_args, get_origin
 
 import pydantic
 
 from ._compat import NULLABLE_KWARGS, PydanticCompat
 
 SelfT = TypeVar("SelfT", bound=pydantic.BaseModel)
 ModelSelfT = TypeVar("ModelSelfT", bound="PartialModelMixin")
@@ -87,15 +87,15 @@
         if field_name not in fields_ and not sub_fields_requested:
             continue
 
         # Change type for sub models, if requested
         if recursive or sub_fields_requested:
             field_annotation_origin = get_origin(field_annotation)
             if field_annotation_origin in (Union, list, tuple, tuple, list, dict, dict):
-                field_annotation = field_annotation_origin[
+                field_annotation = field_annotation_origin[  # type: ignore
                     tuple(
                         _partial_annotation_arg(field_name, field_annotation_arg)
                         for field_annotation_arg
                         in get_args(field_annotation)
                     )
                 ]
             else:
@@ -139,15 +139,18 @@
 
     @classmethod
     def model_as_partial(
         cls: type[ModelSelfT],
         *fields: str,
         recursive: bool = False,
     ) -> type[ModelSelfT]:
-        return create_partial_model(cls, *fields, recursive=recursive)
+        return cast(
+            type[ModelSelfT],
+            create_partial_model(cls, *fields, recursive=recursive),
+        )
 
     @classmethod
     def as_partial(
         cls: type[ModelSelfT],
         *fields: str,
         recursive: bool = False,
     ) -> type[ModelSelfT]:
```

### Comparing `pydantic_partial-0.5.4/pydantic_partial/utils.py` & `pydantic_partial-0.5.5/pydantic_partial/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_partial-0.5.4/pyproject.toml` & `pydantic_partial-0.5.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 [tool.poetry]
 name = "pydantic-partial"
-version = "0.5.4"
+version = "0.5.5"
 description = "Create partial models from your pydantic models. Partial models may allow None for certain or all fields."
 authors = ["TEAM23 GmbH <info@team23.de>"]
 license = "MIT"
 repository = "https://github.com/team23/pydantic-partial"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
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
 target-version = "py39"
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

### Comparing `pydantic_partial-0.5.4/PKG-INFO` & `pydantic_partial-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-partial
-Version: 0.5.4
+Version: 0.5.5
 Summary: Create partial models from your pydantic models. Partial models may allow None for certain or all fields.
 Home-page: https://github.com/team23/pydantic-partial
 License: MIT
 Author: TEAM23 GmbH
 Author-email: info@team23.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,15 @@
 # pydantic-partial
 
 ## Installation
 
 Just use `pip install pydantic-partial` to install the library.
 
 **Note:** `pydantic-partial` is compatible with `pydantic` versions `1.9`, `1.10` and even `2.x` (🥳) on
-Python `3.9`, `3.10` and `3.11`. This is also ensured running all tests on all those versions
+Python `3.9`, `3.10`, `3.11` and `3.12`. This is also ensured running all tests on all those versions
 using `tox`.
 
 ## About
 
 Create partial models from your normal pydantic models. Partial models will allow
 some or all fields to be optional and thus not be required when creating the model
 instance.
```

