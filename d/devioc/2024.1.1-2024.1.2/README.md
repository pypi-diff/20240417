# Comparing `tmp/devioc-2024.1.1.tar.gz` & `tmp/devioc-2024.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devioc-2024.1.1.tar", last modified: Thu Apr 11 17:08:01 2024, max compression
+gzip compressed data, was "devioc-2024.1.2.tar", last modified: Wed Apr 17 15:19:54 2024, max compression
```

## Comparing `devioc-2024.1.1.tar` & `devioc-2024.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-04-11 17:08:01.065239 devioc-2024.1.1/
--rw-rw-r--   0 michel   (70005) michel   (70005)     1066 2020-05-10 23:36:10.000000 devioc-2024.1.1/LICENSE
--rw-r--r--   0 michel   (70005) michel   (70005)     1234 2024-04-11 17:08:01.065239 devioc-2024.1.1/PKG-INFO
--rw-rw-r--   0 michel   (70005) michel   (70005)      568 2020-05-11 01:30:54.000000 devioc-2024.1.1/README.md
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-04-11 17:08:01.064239 devioc-2024.1.1/bin/
--rwxrwxr-x   0 michel   (70005) michel   (70005)     9465 2022-02-17 18:35:37.000000 devioc-2024.1.1/bin/devioc-startproject
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-04-11 17:08:01.065239 devioc-2024.1.1/devioc/
--rw-rw-r--   0 michel   (70005) michel   (70005)        0 2020-05-10 23:36:10.000000 devioc-2024.1.1/devioc/__init__.py
--rw-rw-r--   0 michel   (70005) michel   (70005)     2819 2020-05-10 23:36:10.000000 devioc-2024.1.1/devioc/log.py
--rw-rw-r--   0 michel   (70005) michel   (70005)    16674 2024-04-11 16:55:14.000000 devioc-2024.1.1/devioc/models.py
--rw-r--r--   0 michel   (70005) michel   (70005)     1366 2020-05-10 23:50:35.000000 devioc-2024.1.1/devioc/version.py
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-04-11 17:08:01.065239 devioc-2024.1.1/devioc.egg-info/
--rw-r--r--   0 michel   (70005) michel   (70005)     1234 2024-04-11 17:08:01.000000 devioc-2024.1.1/devioc.egg-info/PKG-INFO
--rw-rw-r--   0 michel   (70005) michel   (70005)      301 2024-04-11 17:08:01.000000 devioc-2024.1.1/devioc.egg-info/SOURCES.txt
--rw-rw-r--   0 michel   (70005) michel   (70005)        1 2024-04-11 17:08:01.000000 devioc-2024.1.1/devioc.egg-info/dependency_links.txt
--rw-rw-r--   0 michel   (70005) michel   (70005)       82 2024-04-11 17:08:01.000000 devioc-2024.1.1/devioc.egg-info/requires.txt
--rw-rw-r--   0 michel   (70005) michel   (70005)       12 2024-04-11 17:08:01.000000 devioc-2024.1.1/devioc.egg-info/top_level.txt
--rw-r--r--   0 michel   (70005) michel   (70005)       38 2024-04-11 17:08:01.065239 devioc-2024.1.1/setup.cfg
--rw-rw-r--   0 michel   (70005) michel   (70005)     1018 2022-02-17 18:35:37.000000 devioc-2024.1.1/setup.py
-drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-04-11 17:08:01.065239 devioc-2024.1.1/test/
--rw-rw-r--   0 michel   (70005) michel   (70005)        0 2022-02-17 18:35:37.000000 devioc-2024.1.1/test/__init__.py
--rw-rw-r--   0 michel   (70005) michel   (70005)     4462 2024-02-16 17:57:09.000000 devioc-2024.1.1/test/test_ioc.py
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-04-17 15:19:54.131868 devioc-2024.1.2/
+-rw-rw-r--   0 michel   (70005) michel   (70005)     1066 2020-05-10 23:36:10.000000 devioc-2024.1.2/LICENSE
+-rw-r--r--   0 michel   (70005) michel   (70005)     1234 2024-04-17 15:19:54.131868 devioc-2024.1.2/PKG-INFO
+-rw-rw-r--   0 michel   (70005) michel   (70005)      568 2020-05-11 01:30:54.000000 devioc-2024.1.2/README.md
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-04-17 15:19:54.130868 devioc-2024.1.2/bin/
+-rwxrwxr-x   0 michel   (70005) michel   (70005)     9465 2022-02-17 18:35:37.000000 devioc-2024.1.2/bin/devioc-startproject
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-04-17 15:19:54.130868 devioc-2024.1.2/devioc/
+-rw-rw-r--   0 michel   (70005) michel   (70005)        0 2020-05-10 23:36:10.000000 devioc-2024.1.2/devioc/__init__.py
+-rw-rw-r--   0 michel   (70005) michel   (70005)     2819 2020-05-10 23:36:10.000000 devioc-2024.1.2/devioc/log.py
+-rw-rw-r--   0 michel   (70005) michel   (70005)    16849 2024-04-17 15:18:22.000000 devioc-2024.1.2/devioc/models.py
+-rw-r--r--   0 michel   (70005) michel   (70005)     1366 2020-05-10 23:50:35.000000 devioc-2024.1.2/devioc/version.py
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-04-17 15:19:54.130868 devioc-2024.1.2/devioc.egg-info/
+-rw-r--r--   0 michel   (70005) michel   (70005)     1234 2024-04-17 15:19:54.000000 devioc-2024.1.2/devioc.egg-info/PKG-INFO
+-rw-rw-r--   0 michel   (70005) michel   (70005)      301 2024-04-17 15:19:54.000000 devioc-2024.1.2/devioc.egg-info/SOURCES.txt
+-rw-rw-r--   0 michel   (70005) michel   (70005)        1 2024-04-17 15:19:54.000000 devioc-2024.1.2/devioc.egg-info/dependency_links.txt
+-rw-rw-r--   0 michel   (70005) michel   (70005)       82 2024-04-17 15:19:54.000000 devioc-2024.1.2/devioc.egg-info/requires.txt
+-rw-rw-r--   0 michel   (70005) michel   (70005)       12 2024-04-17 15:19:54.000000 devioc-2024.1.2/devioc.egg-info/top_level.txt
+-rw-r--r--   0 michel   (70005) michel   (70005)       38 2024-04-17 15:19:54.131868 devioc-2024.1.2/setup.cfg
+-rw-rw-r--   0 michel   (70005) michel   (70005)     1018 2022-02-17 18:35:37.000000 devioc-2024.1.2/setup.py
+drwxr-xr-x   0 michel   (70005) michel   (70005)        0 2024-04-17 15:19:54.130868 devioc-2024.1.2/test/
+-rw-rw-r--   0 michel   (70005) michel   (70005)        0 2022-02-17 18:35:37.000000 devioc-2024.1.2/test/__init__.py
+-rw-rw-r--   0 michel   (70005) michel   (70005)     4462 2024-02-16 17:57:09.000000 devioc-2024.1.2/test/test_ioc.py
```

### Comparing `devioc-2024.1.1/LICENSE` & `devioc-2024.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `devioc-2024.1.1/PKG-INFO` & `devioc-2024.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devioc
-Version: 2024.1.1
+Version: 2024.1.2
 Summary: Simple Python based EPICS Device IOC Support
 Home-page: https://github.com/michel4j/devioc
 Author: Michel Fodje
 Author-email: michel4j@gmail.com
 License: MIT
 Keywords: epics device ioc development
 Classifier: Intended Audience :: Developers
```

### Comparing `devioc-2024.1.1/README.md` & `devioc-2024.1.2/README.md`

 * *Files identical despite different names*

### Comparing `devioc-2024.1.1/bin/devioc-startproject` & `devioc-2024.1.2/bin/devioc-startproject`

 * *Files identical despite different names*

### Comparing `devioc-2024.1.1/devioc/log.py` & `devioc-2024.1.2/devioc/log.py`

 * *Files identical despite different names*

### Comparing `devioc-2024.1.1/devioc/models.py` & `devioc-2024.1.2/devioc/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import multiprocessing
 import os
 import platform
 import shutil
 import subprocess
 import sys
 import time
@@ -57,15 +59,15 @@
         self.options['record'] = self.record
         self.instance_fields = {}
         self.instance_fields.update(self.fields)
 
     def __str__(self):
         template = '\n'.join(
             ['record({record}, "$(device):{name}") {{'] +
-            ['  field({}, "{}")'.format(k, v) for k, v in self.instance_fields.items()] +
+            [f'  field({k}, "{v}")' for k, v in self.instance_fields.items()] +
             ['}}', '']
         )
         return template.format(**self.options)
 
     def add_field(self, key, value):
         """
         Add a database record field
@@ -114,16 +116,16 @@
         elif isinstance(self.options['choices'], Iterable):
             choice_pairs = [(c, i) for i, c in enumerate(self.options['choices'])]
         else:
             choice_pairs = []
         for i in range(len(choice_pairs)):
             name, value = choice_pairs[i]
             key = ENUM_KEYS[i]
-            self.add_field('{}VL'.format(key), "{}".format(value))
-            self.add_field('{}ST'.format(key), name)
+            self.add_field(f'{key}VL', f"{value}")
+            self.add_field(f'{key}ST', name)
 
 
 class BinaryOutput(Record):
     """
     Binary record type for converting between integers and bits
 
     :param name: Record name (str)
@@ -185,15 +187,15 @@
     :keyword oname: string value when high. Sets the ONAM field
     :keyword *: Extra keyword arguments
     """
     record = 'bo'
     fields = {
         'ZNAM': '{zname}',
         'ONAM': '{oname}',
-        'HIGH': '{high:0.2g}'
+        'HIGH': '{high}'
     }
 
     def __init__(self, name, **kwargs):
         kwargs.update(
             high=kwargs.get("high", 0.1),
             zname=kwargs.get("zname", name),
             oname=kwargs.get("oname", "")
@@ -232,103 +234,127 @@
 
 
 class Integer(Record):
     """
     Integer Record.
 
     :param name: Record Name.
-    :keyword max_val: Maximum value permitted (float), default (no limit). Sets the DRVH and HOPR fields
-    :keyword min_val: Minimum value permitted (float), default (no limit). Sets the DRVL and LOPR fields
-    :keyword default: default value, default (0.0). Sets the VAL field
-    :keyword units:  engineering units (str), default empty string. Sets the EGU field
-    :keyword *: Extra keyword arguments
+    :param max_val: Maximum value permitted (float), default (no limit). Sets the DRVH and HOPR fields
+    :param min_val: Minimum value permitted (float), default (no limit). Sets the DRVL and LOPR fields
+    :param default: default value, default (0.0). Sets the VAL field
+    :param units:  engineering units (str), default empty string. Sets the EGU field
+    :param kwargs: Extra keyword arguments
     """
     record = 'longout'
     fields = {
         'HOPR': '{max_val}',
         'LOPR': '{min_val}',
         'DRVH': '{max_val}',
         'DRVL': '{min_val}',
         'VAL': '{default}',
         'EGU': '{units}',
     }
 
-    def __init__(self, name, **kwargs):
+    def __init__(
+            self,
+            name,
+            max_val: int | str = 0.,
+            min_val: int | str = 0.,
+            default: int | str = 0.,
+            units: str = '',
+            **kwargs
+    ):
         kwargs.update(
-            max_val=kwargs.get("max_val", 0),
-            min_val=kwargs.get("min_val", 0),
-            default=kwargs.get("default", 0),
-            units=kwargs.get("units", ""),
+            max_val=max_val,
+            min_val=min_val,
+            default=default,
+            units=units,
         )
         super(Integer, self).__init__(name, **kwargs)
 
 
 class Float(Record):
     """
     Float Record.
 
     :param name: Record Name.
-    :keyword max_val: Maximum value permitted (float), default (no limit). Sets the DRVH and HOPR fields
-    :keyword min_val: Minimum value permitted (float), default (no limit). Sets the DRVL and LOPR fields
-    :keyword default: default value, default (0.0). Sets the VAL field
-    :keyword prec: number of decimal places, default (4). Sets the PREC field
-    :keyword units:  engineering units (str), default empty string. Sets the EGU field
-    :keyword *: Extra keyword arguments
+    :param max_val: Maximum value permitted (float), default (no limit). Sets the DRVH and HOPR fields
+    :param min_val: Minimum value permitted (float), default (no limit). Sets the DRVL and LOPR fields
+    :param prec: number of decimal places, default (4). Sets the PREC field
+    :param default: default value, default (0.0). Sets the VAL field
+    :param units:  engineering units (str), default empty string. Sets the EGU field
+    :param kwargs: Extra keyword arguments
     """
 
     record = 'ao'
     fields = {
-        'DRVH': '{max_val:0.4e}',
-        'DRVL': '{min_val:0.4e}',
-        'HOPR': '{max_val:0.4e}',
-        'LOPR': '{min_val:0.4e}',
+        'DRVH': '{max_val}',
+        'DRVL': '{min_val}',
+        'HOPR': '{max_val}',
+        'LOPR': '{min_val}',
         'PREC': '{prec}',
         'EGU': '{units}',
         'VAL': '{default}'
     }
 
-    def __init__(self, name, max_val=0, min_val=0, default=0.0, prec=4, units='', **kwargs):
+    def __init__(
+            self,
+            name,
+            max_val: float | str = 0.,
+            min_val: float | str = 0.,
+            default: float | str = 0.,
+            prec: int | str = 4,
+            units: str = '',
+            **kwargs
+    ):
         kwargs.update(
-            max_val=kwargs.get("max_val", 0),
-            min_val=kwargs.get("min_val", 0),
-            default=kwargs.get("default", 0),
-            prec=kwargs.get("prec", 4),
-            units=kwargs.get("units", ""),
+            max_val=max_val,
+            min_val=min_val,
+            default=default,
+            prec=prec,
+            units=units,
         )
         super(Float, self).__init__(name, **kwargs)
 
 
 class Calc(Record):
     """
     Calc Record
 
     :param name: Record name
-    :keyword scan: scan parameter, default (0 ie passive). Sets the SCAN field
-    :keyword prec: number of decimal places, default (4). Sets the PREC field
-    :keyword calc: Calculation. Sets CALC field
-    :keyword inpa: Input A specification. Sets the INPA field
-    :keyword *: Extra keyword arguments. Any additional database fields required should be specified as lower-case kwargs.
+    :param scan: scan parameter, default (0 ie passive). Sets the SCAN field
+    :param prec: number of decimal places, default (4). Sets the PREC field
+    :param calc: Calculation. Sets CALC field
+    :param inpa: Input A specification. Sets the INPA field
+    :param kwargs: Extra keyword arguments. Any additional database fields required should be specified as lower-case kwargs.
     """
 
     record = 'calc'
     fields = {
         'CALC': '{calc}',
         'SCAN': '{scan}',
         'PREC': '{prec}',
     }
 
-    def __init__(self, name, **kwargs):
+    def __init__(
+            self,
+            name: str,
+            scan: int | str = 0,
+            prec: int | str = 0,
+            calc: str = '',
+            **kwargs
+    ):
         kwargs.update(
-            scan=kwargs.get("scan", 0),
-            prec=kwargs.get("prec", 0),
-            calc=kwargs.get("calc", "")
+            scan=scan,
+            prec=prec,
+            calc=calc
         )
         super(Calc, self).__init__(name, **kwargs)
         for c in 'ABCDEFGHIJKL':
-            key = 'INP{}'.format(c)
+            key = f'INP{c}'
             if key.lower() in self.options:
                 self.add_field(key, self.options[key.lower()])
 
 
 class CalcOut(Calc):
     """
     CalcOutput Record
@@ -343,20 +369,16 @@
     record = 'calcout'
     fields = {
         'OOPT': '{oopt}',
         'DOPT': '{dopt}',
         'OUT': '{out}',
     }
 
-    def __init__(self, name, **kwargs):
-        kwargs.update(
-            out=kwargs.get("out", ""),
-            oopt=kwargs.get("oopt", 0),
-            dopt=kwargs.get("dopt", 0)
-        )
+    def __init__(self, name, out: str = "", oopt: int | str = 0, dopt: int | str = 0, **kwargs):
+        kwargs.update(out=out, oopt=oopt, dopt=dopt)
         super(CalcOut, self).__init__(name, **kwargs)
 
 
 class Array(Record):
     """
     Array Record.
 
@@ -367,19 +389,16 @@
     """
     record = 'waveform'
     fields = {
         'NELM': '{length}',
         'FTVL': '{type}',
     }
 
-    def __init__(self, name, **kwargs):
-        kwargs.update(
-            type=kwargs.get("type", int),
-            length=kwargs.get("length", 256),
-        )
+    def __init__(self, name, type: str | type = int, length: int | str = 256, **kwargs):
+        kwargs.update(type=type, length=length)
         super(Array, self).__init__(name, **kwargs)
         element_type = self.options['type']
         self.options['type'] = {
             str: 'STRING',
             int: 'LONG',
             float: 'FLOAT',
         }.get(element_type, element_type)
@@ -442,14 +461,16 @@
             ...
 
     which accepts the active record (pv), the changed value (value) and the ioc instance (ioc). If the Model
     is also the callbacks provider, self, and ioc are identical, otherwise ioc is a reference to the database
     model on which the record resides.
     """
 
+    _fields: dict[str, Record]
+
     def __init__(self, device_name, callbacks=None, command='softIoc', macros=None):
         self.device_name = device_name
         self.db_name = self.__class__.__name__
         self.callbacks = callbacks or self
         self.ioc_process = None
         self.macros = {'device': self.device_name}
         if isinstance(macros, dict):
@@ -474,15 +495,15 @@
         db_filename = self.db_cache_dir / f'{self.db_name}.db'
         cmd_filename = self.db_cache_dir / f'{self.db_name}.cmd'
         with open(db_filename, 'w') as db_file:
             for k, v in self._fields.items():
                 db_file.write(str(v))
 
         with open(cmd_filename, 'w') as cmd_file:
-            macro_text = ','.join(['{}={}'.format(k, v) for k, v in self.macros.items()])
+            macro_text = ','.join([f'{k}={v}' for k, v in self.macros.items()])
             cmd_file.write(CMD_TEMPLATE.format(macros=macro_text, db_name=self.db_name))
 
         return db_filename, cmd_filename
 
     def _startup(self):
         """
         Generate the database and start the IOC application in a separate process
@@ -519,16 +540,16 @@
 
     def _setup(self):
         """
         Set up the ioc records and connect all callbacks
         """
         pending = set()
         for k, f in self._fields.items():
-            pv_name = '{}:{}'.format(self.device_name, f.options['name'])
-            callback_name = 'do_{}'.format(k).lower()
+            pv_name = f'{self.device_name}:{f.options["name"]}'
+            callback_name = f'do_{k}'.lower()
             pv = gepics.PV(pv_name)
             setattr(self, k, pv)
             callback = getattr(self.callbacks, callback_name, None)
             if callback:
                 pv.connect('changed', callback, self)
             pending.add(pv)
```

### Comparing `devioc-2024.1.1/devioc/version.py` & `devioc-2024.1.2/devioc/version.py`

 * *Files identical despite different names*

### Comparing `devioc-2024.1.1/devioc.egg-info/PKG-INFO` & `devioc-2024.1.2/devioc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devioc
-Version: 2024.1.1
+Version: 2024.1.2
 Summary: Simple Python based EPICS Device IOC Support
 Home-page: https://github.com/michel4j/devioc
 Author: Michel Fodje
 Author-email: michel4j@gmail.com
 License: MIT
 Keywords: epics device ioc development
 Classifier: Intended Audience :: Developers
```

### Comparing `devioc-2024.1.1/setup.py` & `devioc-2024.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `devioc-2024.1.1/test/test_ioc.py` & `devioc-2024.1.2/test/test_ioc.py`

 * *Files identical despite different names*

