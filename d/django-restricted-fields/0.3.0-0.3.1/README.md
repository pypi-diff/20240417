# Comparing `tmp/django_restricted_fields-0.3.0.tar.gz` & `tmp/django_restricted_fields-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_restricted_fields-0.3.0.tar", last modified: Tue Apr 16 19:01:37 2024, max compression
+gzip compressed data, was "django_restricted_fields-0.3.1.tar", last modified: Tue Apr 16 22:24:06 2024, max compression
```

## Comparing `django_restricted_fields-0.3.0.tar` & `django_restricted_fields-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 lannert   (4779) lannert   (4779)        0 2024-04-16 19:01:37.326855 django_restricted_fields-0.3.0/
--rw-r--r--   0 lannert   (4779) lannert   (4779)     1065 2024-04-16 17:11:06.000000 django_restricted_fields-0.3.0/LICENSE
--rw-r--r--   0 lannert   (4779) lannert   (4779)     4883 2024-04-16 19:01:37.322855 django_restricted_fields-0.3.0/PKG-INFO
--rw-r--r--   0 lannert   (4779) lannert   (4779)      909 2024-04-16 18:53:25.000000 django_restricted_fields-0.3.0/README.md
--rw-r--r--   0 lannert   (4779) lannert   (4779)      923 2024-04-16 18:10:11.000000 django_restricted_fields-0.3.0/README.rst
--rw-r--r--   0 lannert   (4779) lannert   (4779)     1544 2024-04-16 19:01:07.000000 django_restricted_fields-0.3.0/pyproject.toml
--rw-r--r--   0 lannert   (4779) lannert   (4779)     2509 2024-04-16 18:40:14.000000 django_restricted_fields-0.3.0/requirements-dev.txt
--rw-r--r--   0 lannert   (4779) lannert   (4779)       14 2024-04-16 16:44:11.000000 django_restricted_fields-0.3.0/requirements.in
--rw-r--r--   0 lannert   (4779) lannert   (4779)       38 2024-04-16 19:01:37.326855 django_restricted_fields-0.3.0/setup.cfg
-drwxr-xr-x   0 lannert   (4779) lannert   (4779)        0 2024-04-16 19:01:37.318854 django_restricted_fields-0.3.0/src/
-drwxr-xr-x   0 lannert   (4779) lannert   (4779)        0 2024-04-16 19:01:37.318854 django_restricted_fields-0.3.0/src/django_restricted_fields/
--rw-r--r--   0 lannert   (4779) lannert   (4779)        6 2024-04-16 19:01:22.000000 django_restricted_fields-0.3.0/src/django_restricted_fields/VERSION
--rw-r--r--   0 lannert   (4779) lannert   (4779)        8 2024-04-16 16:58:10.000000 django_restricted_fields-0.3.0/src/django_restricted_fields/__init__.py
--rw-r--r--   0 lannert   (4779) lannert   (4779)     6902 2024-04-16 16:48:38.000000 django_restricted_fields-0.3.0/src/django_restricted_fields/forms.py
-drwxr-xr-x   0 lannert   (4779) lannert   (4779)        0 2024-04-16 19:01:37.318854 django_restricted_fields-0.3.0/src/django_restricted_fields.egg-info/
--rw-r--r--   0 lannert   (4779) lannert   (4779)     4883 2024-04-16 19:01:37.000000 django_restricted_fields-0.3.0/src/django_restricted_fields.egg-info/PKG-INFO
--rw-r--r--   0 lannert   (4779) lannert   (4779)      455 2024-04-16 19:01:37.000000 django_restricted_fields-0.3.0/src/django_restricted_fields.egg-info/SOURCES.txt
--rw-r--r--   0 lannert   (4779) lannert   (4779)        1 2024-04-16 19:01:37.000000 django_restricted_fields-0.3.0/src/django_restricted_fields.egg-info/dependency_links.txt
--rw-r--r--   0 lannert   (4779) lannert   (4779)     1076 2024-04-16 19:01:37.000000 django_restricted_fields-0.3.0/src/django_restricted_fields.egg-info/requires.txt
--rw-r--r--   0 lannert   (4779) lannert   (4779)       25 2024-04-16 19:01:37.000000 django_restricted_fields-0.3.0/src/django_restricted_fields.egg-info/top_level.txt
+drwxr-xr-x   0 lannert   (4779) lannert   (4779)        0 2024-04-16 22:24:06.868534 django_restricted_fields-0.3.1/
+-rw-r--r--   0 lannert   (4779) lannert   (4779)     1065 2024-04-16 17:11:06.000000 django_restricted_fields-0.3.1/LICENSE
+-rw-r--r--   0 lannert   (4779) lannert   (4779)     4883 2024-04-16 22:24:06.868534 django_restricted_fields-0.3.1/PKG-INFO
+-rw-r--r--   0 lannert   (4779) lannert   (4779)      909 2024-04-16 18:53:25.000000 django_restricted_fields-0.3.1/README.md
+-rw-r--r--   0 lannert   (4779) lannert   (4779)      923 2024-04-16 18:10:11.000000 django_restricted_fields-0.3.1/README.rst
+-rw-r--r--   0 lannert   (4779) lannert   (4779)     1544 2024-04-16 19:01:07.000000 django_restricted_fields-0.3.1/pyproject.toml
+-rw-r--r--   0 lannert   (4779) lannert   (4779)     2509 2024-04-16 18:40:14.000000 django_restricted_fields-0.3.1/requirements-dev.txt
+-rw-r--r--   0 lannert   (4779) lannert   (4779)       14 2024-04-16 16:44:11.000000 django_restricted_fields-0.3.1/requirements.in
+-rw-r--r--   0 lannert   (4779) lannert   (4779)       38 2024-04-16 22:24:06.868534 django_restricted_fields-0.3.1/setup.cfg
+drwxr-xr-x   0 lannert   (4779) lannert   (4779)        0 2024-04-16 22:24:06.860535 django_restricted_fields-0.3.1/src/
+drwxr-xr-x   0 lannert   (4779) lannert   (4779)        0 2024-04-16 22:24:06.864534 django_restricted_fields-0.3.1/src/django_restricted_fields/
+-rw-r--r--   0 lannert   (4779) lannert   (4779)        6 2024-04-16 21:54:42.000000 django_restricted_fields-0.3.1/src/django_restricted_fields/VERSION
+-rw-r--r--   0 lannert   (4779) lannert   (4779)        8 2024-04-16 16:58:10.000000 django_restricted_fields-0.3.1/src/django_restricted_fields/__init__.py
+-rw-r--r--   0 lannert   (4779) lannert   (4779)     6989 2024-04-16 22:18:44.000000 django_restricted_fields-0.3.1/src/django_restricted_fields/forms.py
+drwxr-xr-x   0 lannert   (4779) lannert   (4779)        0 2024-04-16 22:24:06.864534 django_restricted_fields-0.3.1/src/django_restricted_fields.egg-info/
+-rw-r--r--   0 lannert   (4779) lannert   (4779)     4883 2024-04-16 22:24:06.000000 django_restricted_fields-0.3.1/src/django_restricted_fields.egg-info/PKG-INFO
+-rw-r--r--   0 lannert   (4779) lannert   (4779)      455 2024-04-16 22:24:06.000000 django_restricted_fields-0.3.1/src/django_restricted_fields.egg-info/SOURCES.txt
+-rw-r--r--   0 lannert   (4779) lannert   (4779)        1 2024-04-16 22:24:06.000000 django_restricted_fields-0.3.1/src/django_restricted_fields.egg-info/dependency_links.txt
+-rw-r--r--   0 lannert   (4779) lannert   (4779)     1076 2024-04-16 22:24:06.000000 django_restricted_fields-0.3.1/src/django_restricted_fields.egg-info/requires.txt
+-rw-r--r--   0 lannert   (4779) lannert   (4779)       25 2024-04-16 22:24:06.000000 django_restricted_fields-0.3.1/src/django_restricted_fields.egg-info/top_level.txt
```

### Comparing `django_restricted_fields-0.3.0/LICENSE` & `django_restricted_fields-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_restricted_fields-0.3.0/PKG-INFO` & `django_restricted_fields-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-restricted-fields
-Version: 0.3.0
+Version: 0.3.1
 Summary: Provides date and date/time fields with restrictions for Django forms.
 Author-email: Detlef Lannert <detlef@lannert.de>
 Maintainer-email: Detlef Lannert <detlef@lannert.de>
 Project-URL: Homepage, https://github.com/detlefla/django-restricted-fields
 Project-URL: Repository, https://github.com/detlefla/django-restricted-fields
 Project-URL: Issues, https://github.com/detlefla/django-restricted-fields/issues
 Keywords: web,django,forms
```

### Comparing `django_restricted_fields-0.3.0/README.md` & `django_restricted_fields-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `django_restricted_fields-0.3.0/README.rst` & `django_restricted_fields-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `django_restricted_fields-0.3.0/pyproject.toml` & `django_restricted_fields-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_restricted_fields-0.3.0/requirements-dev.txt` & `django_restricted_fields-0.3.1/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `django_restricted_fields-0.3.0/src/django_restricted_fields/forms.py` & `django_restricted_fields-0.3.1/src/django_restricted_fields/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     input_type = "datetime-local"
     
     def render(self, name, value, attrs=None, renderer=None):
         """Render the widget as an HTML string."""
         new_value = value
         if value and not isinstance(value, str):
                 new_value = value.isoformat()
+        new_value = new_value[:-2] + "00"  # value comparisons don't work on seconds?!
         return super().render(name, new_value, attrs=attrs, renderer=renderer)
 
 
 class NativeDateInput(DateInput):
     input_type = "date-local"
     
     def render(self, name, value, attrs=None, renderer=None):
@@ -69,24 +70,24 @@
             # is there a min restriction?
             _min = None
             if not self.past_allowed:
                 _min = now
             if self.min_value is not None and (_min is None or self.min_value > _min):
                 _min = self.min_value
             if _min is not None:
-                attrs["min"] = f"{_min:%Y-%m-%dT%H:%M:%S}"
+                attrs["min"] = f"{_min:%Y-%m-%dT00:00:00}"
             
             # is there a max restriction?
             _max = None
             if not self.future_allowed:
                 _max = now
             if self.max_value is not None and (_max is None or self.max_value < _max):
                 _max = self.max_value
             if _max is not None:
-                attrs["max"] = f"{_max:%Y-%m-%dT%H:%M:%S}"
+                attrs["max"] = f"{_max:%Y-%m-%dT23:59:59}"
         
         return attrs
     
     def validate(self, value: Any) -> None:
         """Validates the form input for this field."""
         super().validate(value)
         now = datetime.now(timezone.utc)
```

### Comparing `django_restricted_fields-0.3.0/src/django_restricted_fields.egg-info/PKG-INFO` & `django_restricted_fields-0.3.1/src/django_restricted_fields.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-restricted-fields
-Version: 0.3.0
+Version: 0.3.1
 Summary: Provides date and date/time fields with restrictions for Django forms.
 Author-email: Detlef Lannert <detlef@lannert.de>
 Maintainer-email: Detlef Lannert <detlef@lannert.de>
 Project-URL: Homepage, https://github.com/detlefla/django-restricted-fields
 Project-URL: Repository, https://github.com/detlefla/django-restricted-fields
 Project-URL: Issues, https://github.com/detlefla/django-restricted-fields/issues
 Keywords: web,django,forms
```

### Comparing `django_restricted_fields-0.3.0/src/django_restricted_fields.egg-info/requires.txt` & `django_restricted_fields-0.3.1/src/django_restricted_fields.egg-info/requires.txt`

 * *Files identical despite different names*

