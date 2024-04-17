# Comparing `tmp/django-readers-2.2.0.tar.gz` & `tmp/django-readers-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-readers-2.2.0.tar", last modified: Fri Jan 12 16:52:42 2024, max compression
+gzip compressed data, was "django-readers-2.3.0.tar", last modified: Wed Apr 17 11:30:01 2024, max compression
```

## Comparing `django-readers-2.2.0.tar` & `django-readers-2.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 16:52:42.690910 django-readers-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-01-12 16:52:34.000000 django-readers-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-01-12 16:52:42.690910 django-readers-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-01-12 16:52:34.000000 django-readers-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 16:52:42.690910 django-readers-2.2.0/django_readers/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-12 16:52:34.000000 django-readers-2.2.0/django_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-01-12 16:52:34.000000 django-readers-2.2.0/django_readers/pairs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-01-12 16:52:34.000000 django-readers-2.2.0/django_readers/producers.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-01-12 16:52:34.000000 django-readers-2.2.0/django_readers/projectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10245 2024-01-12 16:52:34.000000 django-readers-2.2.0/django_readers/qs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9140 2024-01-12 16:52:34.000000 django-readers-2.2.0/django_readers/rest_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-01-12 16:52:34.000000 django-readers-2.2.0/django_readers/specs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-01-12 16:52:34.000000 django-readers-2.2.0/django_readers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 16:52:42.690910 django-readers-2.2.0/django_readers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-01-12 16:52:42.000000 django-readers-2.2.0/django_readers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-01-12 16:52:42.000000 django-readers-2.2.0/django_readers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 16:52:42.000000 django-readers-2.2.0/django_readers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-12 16:52:42.000000 django-readers-2.2.0/django_readers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-12 16:52:42.000000 django-readers-2.2.0/django_readers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-12 16:52:42.690910 django-readers-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-01-12 16:52:34.000000 django-readers-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:30:01.041576 django-readers-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-17 11:29:46.000000 django-readers-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-17 11:30:01.041576 django-readers-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-17 11:29:46.000000 django-readers-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:30:01.037576 django-readers-2.3.0/django_readers/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 11:29:46.000000 django-readers-2.3.0/django_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-17 11:29:46.000000 django-readers-2.3.0/django_readers/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-17 11:29:46.000000 django-readers-2.3.0/django_readers/producers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-17 11:29:46.000000 django-readers-2.3.0/django_readers/projectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10245 2024-04-17 11:29:46.000000 django-readers-2.3.0/django_readers/qs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-04-17 11:29:46.000000 django-readers-2.3.0/django_readers/rest_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-17 11:29:46.000000 django-readers-2.3.0/django_readers/specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-17 11:29:46.000000 django-readers-2.3.0/django_readers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:30:01.041576 django-readers-2.3.0/django_readers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-17 11:30:00.000000 django-readers-2.3.0/django_readers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-17 11:30:00.000000 django-readers-2.3.0/django_readers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 11:30:00.000000 django-readers-2.3.0/django_readers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 11:30:00.000000 django-readers-2.3.0/django_readers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 11:30:00.000000 django-readers-2.3.0/django_readers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-17 11:30:01.041576 django-readers-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-17 11:29:46.000000 django-readers-2.3.0/setup.py
```

### Comparing `django-readers-2.2.0/LICENSE` & `django-readers-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-readers-2.2.0/PKG-INFO` & `django-readers-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-readers
-Version: 2.2.0
+Version: 2.3.0
 Summary: A lightweight function-oriented toolkit for better organisation of business logic and efficient selection and projection of data in Django projects.
 Home-page: https://www.django-readers.org
 Author: DabApps
 Author-email: hello@dabapps.com
 License: BSD
 Project-URL: Changelog, https://github.com/dabapps/django-readers/releases
 Project-URL: Issues, https://github.com/dabapps/django-readers/issues
```

### Comparing `django-readers-2.2.0/README.md` & `django-readers-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `django-readers-2.2.0/django_readers/pairs.py` & `django-readers-2.3.0/django_readers/pairs.py`

 * *Files identical despite different names*

### Comparing `django-readers-2.2.0/django_readers/producers.py` & `django-readers-2.3.0/django_readers/producers.py`

 * *Files identical despite different names*

### Comparing `django-readers-2.2.0/django_readers/projectors.py` & `django-readers-2.3.0/django_readers/projectors.py`

 * *Files identical despite different names*

### Comparing `django-readers-2.2.0/django_readers/qs.py` & `django-readers-2.3.0/django_readers/qs.py`

 * *Files identical despite different names*

### Comparing `django-readers-2.2.0/django_readers/rest_framework.py` & `django-readers-2.3.0/django_readers/rest_framework.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,28 @@
 from django_readers import specs
 from django_readers.utils import SpecVisitor
 from functools import wraps
 from rest_framework import serializers
 from rest_framework.utils import model_meta
 
 
+def add_annotation(obj, key, value):
+    obj._readers_annotation = getattr(obj, "_readers_annotation", None) or {}
+    obj._readers_annotation[key] = value
+
+
+def get_annotation(obj, key):
+    # Either the item itself or (if this is a pair) just the
+    # producer/projector function may have been decorated
+    if value := getattr(obj, "_readers_annotation", {}).get(key):
+        return value
+    if isinstance(obj, tuple):
+        return get_annotation(obj[1], key)
+
+
 class ProjectionSerializer:
     def __init__(self, data=None, many=False, context=None):
         self.many = many
         self._data = data
         self.context = context
 
     @property
@@ -73,54 +87,51 @@
         self.field_builder = serializers.ModelSerializer()
         self.info = model_meta.get_field_info(model)
         self.fields = {}
 
     def _lowercase_with_underscores_to_capitalized_words(self, string):
         return "".join(part.title() for part in string.split("_"))
 
-    def _prepare_field(self, field):
+    def _prepare_field(self, field, kwargs=None):
         # We copy the field so its _creation_counter is correct and
         # it appears in the right order in the resulting serializer.
         # We also force it to be read_only
         field = deepcopy(field)
+        if kwargs:
+            field._kwargs.update(kwargs)
         field._kwargs["read_only"] = True
         return field
 
-    def _get_out_value(self, item):
-        # Either the item itself or (if this is a pair) just the
-        # producer/projector function may have been decorated
-        if hasattr(item, "out"):
-            return item.out
-        if isinstance(item, tuple) and hasattr(item[1], "out"):
-            return item[1].out
-        return None
-
     def visit_str(self, item):
         return self.visit_dict_item_str(item, item)
 
     def visit_dict_item_str(self, key, value):
         # This is a model field name. First, check if the
         # field has been explicitly overridden
-        if hasattr(value, "out"):
-            field = self._prepare_field(value.out)
-            self.fields[str(key)] = field
-            return key, field
-
-        # No explicit override, so we can use ModelSerializer
-        # machinery to figure out which field type to use
-        field_class, field_kwargs = self.field_builder.build_field(
-            value,
-            self.info,
-            self.model,
-            0,
-        )
-        if key != value:
-            field_kwargs["source"] = value
-        field_kwargs.setdefault("read_only", True)
-        self.fields[key] = field_class(**field_kwargs)
+        if out := get_annotation(value, "field"):
+            field = self._prepare_field(out, kwargs=get_annotation(value, "kwargs"))
+
+        else:
+            # No explicit override, so we can use ModelSerializer
+            # machinery to figure out which field type to use
+            field_class, field_kwargs = self.field_builder.build_field(
+                value,
+                self.info,
+                self.model,
+                0,
+            )
+            if key != value:
+                field_kwargs["source"] = value
+            field_kwargs.setdefault("read_only", True)
+
+            if kwargs := get_annotation(value, "kwargs"):
+                field_kwargs.update(kwargs)
+            field = field_class(**field_kwargs)
+
+        self.fields[str(key)] = field
         return key, value
 
     def _get_child_serializer_kwargs(self, rel_info):
         kwargs = {"read_only": True, "many": rel_info.to_many}
         if rel_info.model_field and rel_info.model_field.null:
             kwargs["allow_null"] = True
         return kwargs
@@ -169,32 +180,34 @@
         serializer_kwargs = self._get_child_serializer_kwargs(rel_info)
         serializer_kwargs["source"] = relationship_name
         self.fields[key] = child_serializer_class(**serializer_kwargs)
         return key, value
 
     def visit_dict_item_tuple(self, key, value):
         # This is a producer pair.
-        out = self._get_out_value(value)
+        out = get_annotation(value, "field")
+        kwargs = get_annotation(value, "kwargs") or {}
         if out:
-            field = self._prepare_field(out)
+            field = self._prepare_field(out, kwargs)
             self.fields[key] = field
         else:
             # Fallback case: we don't know what field type to use
-            self.fields[key] = serializers.ReadOnlyField()
+            self.fields[key] = serializers.ReadOnlyField(**kwargs)
         return key, value
 
     visit_dict_item_callable = visit_dict_item_tuple
 
     def visit_tuple(self, item):
         # This is a projector pair.
-        out = self._get_out_value(item)
+        out = get_annotation(item, "field")
+        kwargs = get_annotation(item, "kwargs") or {}
         if out:
             # `out` is a dictionary mapping field names to Fields
             for name, field in out.items():
-                field = self._prepare_field(field)
+                field = self._prepare_field(field, kwargs)
                 self.fields[name] = field
         # There is no fallback case because we have no way of knowing the shape
         # of the returned dictionary, so the schema will be unavoidably incorrect.
         return item
 
     visit_callable = visit_tuple
 
@@ -227,48 +240,57 @@
         raise ImproperlyConfigured(
             "View class must have either a 'queryset' or 'model' attribute"
         )
 
     return serializer_class_for_spec(name_prefix, model, view.spec)
 
 
-class PairWithOutAttribute(tuple):
-    out = None
+class PairWithAnnotation(tuple):
+    _readers_annotation = None
 
 
-class StringWithOutAttribute(str):
-    out = None
+class StringWithAnnotation(str):
+    _readers_annotation = None
 
 
-def out(field_or_dict):
-    if isinstance(field_or_dict, dict):
-        if not all(
-            isinstance(item, serializers.Field) for item in field_or_dict.values()
-        ):
-            raise TypeError("Each value must be an instance of Field")
-    elif not isinstance(field_or_dict, serializers.Field):
-        raise TypeError("Must be an instance of Field")
+def out(*args, **kwargs):
+    if args:
+        if len(args) != 1:
+            raise TypeError("Provide a single field or dictionary of fields")
+        field_or_dict = args[0]
+        if isinstance(field_or_dict, dict):
+            if not all(
+                isinstance(item, serializers.Field) for item in field_or_dict.values()
+            ):
+                raise TypeError("Each value must be an instance of Field")
+        elif not isinstance(field_or_dict, serializers.Field):
+            raise TypeError("Must be an instance of Field")
+    else:
+        field_or_dict = None
 
     class ShiftableDecorator:
         def __call__(self, item):
             if callable(item):
 
                 @wraps(item)
                 def wrapper(*args, **kwargs):
                     result = item(*args, **kwargs)
                     return self(result)
 
-                wrapper.out = field_or_dict
+                add_annotation(wrapper, "field", field_or_dict)
+                add_annotation(wrapper, "kwargs", kwargs)
                 return wrapper
             else:
                 if isinstance(item, str):
-                    item = StringWithOutAttribute(item)
-                    item.out = field_or_dict
+                    item = StringWithAnnotation(item)
+                    add_annotation(item, "field", field_or_dict)
+                    add_annotation(item, "kwargs", kwargs)
                 if isinstance(item, tuple):
-                    item = PairWithOutAttribute(item)
-                    item.out = field_or_dict
+                    item = PairWithAnnotation(item)
+                    add_annotation(item, "field", field_or_dict)
+                    add_annotation(item, "kwargs", kwargs)
                 return item
 
         def __rrshift__(self, other):
             return self(other)
 
     return ShiftableDecorator()
```

### Comparing `django-readers-2.2.0/django_readers/specs.py` & `django-readers-2.3.0/django_readers/specs.py`

 * *Files identical despite different names*

### Comparing `django-readers-2.2.0/django_readers/utils.py` & `django-readers-2.3.0/django_readers/utils.py`

 * *Files identical despite different names*

### Comparing `django-readers-2.2.0/django_readers.egg-info/PKG-INFO` & `django-readers-2.3.0/django_readers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-readers
-Version: 2.2.0
+Version: 2.3.0
 Summary: A lightweight function-oriented toolkit for better organisation of business logic and efficient selection and projection of data in Django projects.
 Home-page: https://www.django-readers.org
 Author: DabApps
 Author-email: hello@dabapps.com
 License: BSD
 Project-URL: Changelog, https://github.com/dabapps/django-readers/releases
 Project-URL: Issues, https://github.com/dabapps/django-readers/issues
```

### Comparing `django-readers-2.2.0/setup.py` & `django-readers-2.3.0/setup.py`

 * *Files identical despite different names*

