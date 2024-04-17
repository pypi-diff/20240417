# Comparing `tmp/pylogg-0.3.0.tar.gz` & `tmp/pylogg-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylogg-0.3.0.tar", last modified: Wed Apr 17 16:56:43 2024, max compression
+gzip compressed data, was "pylogg-0.3.1.tar", last modified: Wed Apr 17 17:35:16 2024, max compression
```

## Comparing `pylogg-0.3.0.tar` & `pylogg-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:43.312105 pylogg-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-17 16:56:36.000000 pylogg-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-17 16:56:43.312105 pylogg-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-17 16:56:36.000000 pylogg-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:43.308105 pylogg-0.3.0/pylogg/
--rw-r--r--   0 runner    (1001) docker     (127)    17574 2024-04-17 16:56:36.000000 pylogg-0.3.0/pylogg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-17 16:56:36.000000 pylogg-0.3.0/pylogg/jsonfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-04-17 16:56:36.000000 pylogg-0.3.0/pylogg/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)    10002 2024-04-17 16:56:36.000000 pylogg-0.3.0/pylogg/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:43.312105 pylogg-0.3.0/pylogg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-17 16:56:43.000000 pylogg-0.3.0/pylogg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-17 16:56:43.000000 pylogg-0.3.0/pylogg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:56:43.000000 pylogg-0.3.0/pylogg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-17 16:56:43.000000 pylogg-0.3.0/pylogg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 16:56:43.000000 pylogg-0.3.0/pylogg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-17 16:56:36.000000 pylogg-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 16:56:43.312105 pylogg-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:56:43.312105 pylogg-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-17 16:56:36.000000 pylogg-0.3.0/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:35:16.726394 pylogg-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-17 17:35:11.000000 pylogg-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-17 17:35:16.726394 pylogg-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-17 17:35:11.000000 pylogg-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:35:16.722394 pylogg-0.3.1/pylogg/
+-rw-r--r--   0 runner    (1001) docker     (127)    17574 2024-04-17 17:35:11.000000 pylogg-0.3.1/pylogg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-17 17:35:11.000000 pylogg-0.3.1/pylogg/jsonfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-04-17 17:35:11.000000 pylogg-0.3.1/pylogg/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-04-17 17:35:11.000000 pylogg-0.3.1/pylogg/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:35:16.722394 pylogg-0.3.1/pylogg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-17 17:35:16.000000 pylogg-0.3.1/pylogg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-17 17:35:16.000000 pylogg-0.3.1/pylogg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 17:35:16.000000 pylogg-0.3.1/pylogg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-17 17:35:16.000000 pylogg-0.3.1/pylogg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 17:35:16.000000 pylogg-0.3.1/pylogg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-17 17:35:11.000000 pylogg-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 17:35:16.726394 pylogg-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:35:16.722394 pylogg-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-17 17:35:11.000000 pylogg-0.3.1/tests/test_settings.py
```

### Comparing `pylogg-0.3.0/LICENSE` & `pylogg-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylogg-0.3.0/PKG-INFO` & `pylogg-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: pylogg
-Version: 0.3.0
+Version: 0.3.1
 Summary: Logging and YAML-based configuration modules in Python.
 Author-email: Akhlak Mahmood <akhlakm@gatech.edu>
 Project-URL: Homepage, https://github.com/akhlakm/python-logg
 Project-URL: Bug Tracker, https://github.com/akhlakm/python-logg/issues
 Keywords: logging,development
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml
-Requires-Dist: pydantic>=2.7
 Provides-Extra: postgres
 Requires-Dist: pandas; extra == "postgres"
 Requires-Dist: sshtunnel; extra == "postgres"
 Requires-Dist: psycopg[binary]; extra == "postgres"
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
```

### Comparing `pylogg-0.3.0/README.md` & `pylogg-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pylogg-0.3.0/pylogg/__init__.py` & `pylogg-0.3.1/pylogg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 A personally opinionated logging package.
 LICENSE MIT Copyright 2024 Akhlak Mahmood
 
 """
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 __author__ = "Akhlak Mahmood"
 
 import os
 import sys
 import textwrap
 import time
 from datetime import datetime, timezone
```

### Comparing `pylogg-0.3.0/pylogg/jsonfs.py` & `pylogg-0.3.1/pylogg/jsonfs.py`

 * *Files identical despite different names*

### Comparing `pylogg-0.3.0/pylogg/postgres.py` & `pylogg-0.3.1/pylogg/postgres.py`

 * *Files identical despite different names*

### Comparing `pylogg-0.3.0/pylogg/settings.py` & `pylogg-0.3.1/pylogg/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """
     A module to load configurations from environment varibles or
     YAML file(s).
 
 """
+
 import os
 import string
 import sys
+from typing import NamedTuple
 
 import yaml
-from pydantic import BaseModel
-from pydantic.fields import FieldInfo
-from pydantic_core import PydanticUndefined
 
+# For access to the __annotations__ attribute.
 assert sys.version_info >= (3, 10), "Minimum Python 3.10 required"
 
-class SettingsParser:
+
+class PLSettings:
     """
     Load all settings from environment variables and/or a YAML file.
 
     name:
         Name of the settings. Used as the prefix for environment variables.
 
     yaml_file:
@@ -34,40 +35,37 @@
         Override YAML vars with environment variables or vice versa.
         Default order: cmdline > YAML > Env.
         Prefer_env order: cmdline > Env. > YAML.
 
 
     Example:
 
-    Subclass the pydantic.BaseModel, and define a classmethod to load the
+    Subclass the typing.NamedTuple, and define a classmethod to load the
     settings.
 
     ```python
-    from typing import ClassVar
-    from pydantic import BaseModel
-
-    class TestSettings(BaseModel):
+    class _Test(NamedTuple):
         name: str   = 'hello'
 
-    class Settings(BaseModel):
-        YAML : ClassVar = None
+    class Settings(NamedTuple):
+        YAML = None
 
         # Define the sections ...
-        Test : TestSettings
+        TestSettings : _Test
 
         @classmethod
         def load(c, yaml_file = None, first_arg = False) -> 'Settings':
             c.YAML = PLSettings('pytest', yaml_file, first_arg=first_arg)
             return c.YAML.populate(c)
 
         def save(self, yaml_file = None):
             self.YAML.save(self, yaml_file=yaml_file)
 
     settings = Settings.load('settings.yaml')
-    test = settings.Test
+    test = settings.TestSettings
     print(test.name)
     ```
     """
 
     def __init__(self, name : str, yaml_file : str = None,
             first_arg : bool = True, load_env : bool = True,
             prefer_env : bool = False):
@@ -98,20 +96,17 @@
     def __repr__(self) -> str:
         s = self.__class__.__name__ + ": "
         for k, v in self._yamlvars.items():
             s += f"{k} {v._asdict()}"
         return s
 
 
-    def _populate_field(self, section : str, field : str, info : FieldInfo):
-        if info.is_required() and info.default is PydanticUndefined:
-            raise AssertionError(f"{section}.{field} is required")
-
+    def _populate_field(self, section : str, field : str, data_type, def_value):
         # Start with the default value.
-        value = info.default
+        value = def_value
 
         # If _name is given, prefix it for the env var.
         # Format: NAME_SECTION_FIELD=value
         env_var_name = f"{section.upper()}_{field.upper()}"
         if self._name:
             env_var_name = f"{self._name.upper()}_{env_var_name}"
 
@@ -128,52 +123,55 @@
 
         # Check if there is any $ arg template in env vars / yaml.
         value = self._get_arg(field, value)
 
         # Convert to expected type.
         if value is not None:
             try:
-                value = info.annotation(value)
+                value = data_type(value)
             except:
                 raise ValueError(f"Invalid type for {field}: {value}")
         return value
 
 
-    def _populate_section(self, section_name : str, section_cls : BaseModel):
+    def _populate_section(self, section_name : str, section_cls : NamedTuple):
         """ Populate settings to the current class/section. """
 
-        assert hasattr(section_cls, 'model_fields'), "Section must be a BaseModel."
+        assert hasattr(section_cls, '_fields'), "Section must be a NamedTuple."
 
         fields = {}
 
-        # for each BaseModel fields ...
-        for field in section_cls.model_fields:
-            section_cls.__annotations__[field]
+        # for each namedtuple fields ...
+        for field in section_cls._fields:
+            data_type = section_cls.__annotations__[field]
+
+            # Default value.
+            value = section_cls._field_defaults.get(field, None)
 
-        for field, field_info in section_cls.model_fields.items():
+            # Populate field
             fields[field] = \
-                self._populate_field(section_name, field, field_info)
+                self._populate_field(section_name, field, data_type, value)
 
         # Return initialized class.
         return section_cls(**fields)
 
 
-    def populate(self, settings : BaseModel):
-        """ Populate settings to all sections defined by BaseModel fields. """
+    def populate(self, settings : NamedTuple):
+        """ Populate settings to all sections defined by NamedTuple fields. """
 
-        assert hasattr(settings, 'model_fields'), "Settings must be a BaseModel."
+        assert hasattr(settings, '_fields'), "Settings must be a NamedTuple."
 
         sections = {}
 
         # for each settings sections ...
-        for section_name, section_info in settings.model_fields.items():
-            section_cls = section_info.annotation
+        for section_name in settings._fields:
+            section_definition = settings.__annotations__[section_name]
 
             # populate individual section
-            value = self._populate_section(section_name, section_cls)
+            value = self._populate_section(section_name, section_definition)
 
             # Add to class sections
             sections[section_name] = value
 
         # Return initialized class.
         return settings(**sections)
 
@@ -274,15 +272,15 @@
 
 
     def is_loaded(self) -> bool:
         """ Returns True if at least one section from YAML file was loaded. """
         return len(self._yamlvars) > 0
 
 
-    def save(self, settings : BaseModel, yaml_file : str = None,
+    def save(self, settings : NamedTuple, yaml_file : str = None,
                 keep_existing : bool = True):
         """ Save all sections of the settings to a YAML file.
             If no yaml_file is given, the initial file is used.
 
             keep_existing:
                 Keep the already existing sections in the YAML file.
         """
@@ -292,22 +290,22 @@
         existing = yaml.safe_load(open(outfile)) \
             if os.path.isfile(outfile) else {}
 
         configs = existing if keep_existing else {}
 
         assert type(configs) == dict, f"Existing YAML is not a dict: {outfile}"
 
-        assert hasattr(settings, 'model_fields'), "Settings must be a BaseModel."
+        assert hasattr(settings, '_fields'), "Settings must be a NamedTuple."
 
         # for each settings sections ...
-        for section_name in settings.model_fields:
+        for section_name in settings._fields:
             section = getattr(settings, section_name)
 
-            if hasattr(section, 'model_dump'):
-                configs[section_name] = section.model_dump()
+            if hasattr(section, '_asdict'):
+                configs[section_name] = section._asdict()
 
         yaml.safe_dump(configs, open(outfile, 'w'), indent=4)
         print("Save OK:", outfile)
 
 
     def copy_sample(self, sample_file : str):
         """ Copy a sample YAML file to the current settings file. """
```

### Comparing `pylogg-0.3.0/pylogg.egg-info/PKG-INFO` & `pylogg-0.3.1/pylogg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: pylogg
-Version: 0.3.0
+Version: 0.3.1
 Summary: Logging and YAML-based configuration modules in Python.
 Author-email: Akhlak Mahmood <akhlakm@gatech.edu>
 Project-URL: Homepage, https://github.com/akhlakm/python-logg
 Project-URL: Bug Tracker, https://github.com/akhlakm/python-logg/issues
 Keywords: logging,development
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml
-Requires-Dist: pydantic>=2.7
 Provides-Extra: postgres
 Requires-Dist: pandas; extra == "postgres"
 Requires-Dist: sshtunnel; extra == "postgres"
 Requires-Dist: psycopg[binary]; extra == "postgres"
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
```

### Comparing `pylogg-0.3.0/pyproject.toml` & `pylogg-0.3.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
 ]
 
 dependencies = [
     "pyyaml",
-    "pydantic >= 2.7",
 ]
 
 [project.optional-dependencies]
 postgres = [
     "pandas",
     "sshtunnel",
     "psycopg[binary]",
```

### Comparing `pylogg-0.3.0/tests/test_settings.py` & `pylogg-0.3.1/tests/test_settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,47 @@
-from typing import ClassVar
-
-from pydantic import BaseModel
-
-from pylogg.settings import SettingsParser
+from pylogg.settings import NamedTuple, PLSettings
 
 
 def test_load_settings(assets, tmp_path):
     asset_file = assets / "settings.yaml"
     test_output = tmp_path / "settings.yaml"
 
-    class Test(BaseModel):
+    class Test(NamedTuple):
         row1: float = 100.0
         row2: str   = 'Package'
         row3: str   = 'Settings'
         row4: str   = 'Default'
 
-    class Person(BaseModel):
+    class Person(NamedTuple):
         name : str = 'John'
         age : int = 3
 
-    class Settings(BaseModel):
-        YAML : ClassVar = None
+    class Settings(NamedTuple):
+        YAML = None
         TestSettings : Test
         PersonSettings : Person
 
         @classmethod
         def load(c, yaml_file = None, first_arg = False) -> 'Settings':
-            c.YAML = SettingsParser('pytest', yaml_file, first_arg=first_arg)
+            c.YAML = PLSettings('pytest', yaml_file, first_arg=first_arg)
             return c.YAML.populate(c)
 
         def create(self, newfile = None):
             self.YAML.save(self, yaml_file=newfile)
 
 
     sett = Settings.load(asset_file)
     test = sett.TestSettings
     assert test.row1 == 23.6
     assert test.row2 == "Hello"
     assert test.row3 == "World"
     assert test.row4 == "Default"
 
-    sett.TestSettings.row1 = 90.0
+    sett = sett._replace(TestSettings = sett.TestSettings._replace(row1 = 90.0))
+    test = sett.TestSettings
     assert test.row1 == 90.0
     assert test.row4 == "Default"
 
     person = sett.PersonSettings
     assert person.name == "Mike"
     assert person.age == 29
 
@@ -54,26 +51,26 @@
     assert 'row4: Default' in test_output.read_text()
 
 
 def test_yaml_write(assets, tmp_path):
     asset_file = assets / "settings.yaml"
     test_output = tmp_path / "settings.yaml"
 
-    class Test(BaseModel):
+    class Test(NamedTuple):
         row1: float = 23.6
         row2: str   = 'Hello'
         row3: str   = 'World'
 
-    class Settings(BaseModel):
-        YAML : ClassVar = None
+    class Settings(NamedTuple):
+        YAML = None
         TestSettings : Test
 
         @classmethod
         def load(c, yaml_file = None, first_arg = False) -> 'Settings':
-            c.YAML = SettingsParser('pytest', yaml_file, first_arg=first_arg)
+            c.YAML = PLSettings('pytest', yaml_file, first_arg=first_arg)
             return c.YAML.populate(c)
 
         def save(self, newfile = None):
             self.YAML.save(self, yaml_file=newfile)
 
     settings = Settings.load(asset_file)
     test = settings.TestSettings
@@ -88,26 +85,26 @@
     assert test.row3 in test_output.read_text()
 
 
 def test_args_subs():
     import sys
     sys.argv += ['--name', 'world', '--debug', '--num', '22']
 
-    class Test(BaseModel):
+    class Test(NamedTuple):
         greeting: str   = 'Hello $name'
         number : int    = '$num'
         debug : bool    = '$debug'
 
-    class Settings(BaseModel):
-        YAML : ClassVar = None
+    class Settings(NamedTuple):
+        YAML = None
         TestSettings : Test
 
         @classmethod
         def load(c, yaml_file = None, first_arg = False) -> 'Settings':
-            c.YAML = SettingsParser('pytest', yaml_file, first_arg=first_arg)
+            c.YAML = PLSettings('pytest', yaml_file, first_arg=first_arg)
             return c.YAML.populate(c)
 
         def save(self, newfile = None):
             self.YAML.save(self, yamlfile=newfile)
 
     settings = Settings.load(None)
     test = settings.TestSettings
@@ -118,18 +115,18 @@
 
     print(test)
 
 
 def test_postitional_args():
     import sys
 
-    yaml = SettingsParser('pytest')
+    yaml = PLSettings('pytest')
     print(yaml._pos_args)
 
     sys.argv += ['--name', 'world', 'settings2.yaml', '--debug', '--num', '22']
-    yaml = SettingsParser('pytest')
+    yaml = PLSettings('pytest')
     print(yaml._pos_args)
 
     sys.argv += ['settings2.yaml']
-    yaml = SettingsParser('pytest')
+    yaml = PLSettings('pytest')
     assert yaml._pos_args == ['settings2.yaml', 'settings2.yaml']
     print(yaml._pos_args)
```

