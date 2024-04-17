# Comparing `tmp/xmlable-2.0.1.tar.gz` & `tmp/xmlable-2.0.2.tar.gz`

## Comparing `xmlable-2.0.1.tar` & `xmlable-2.0.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 xmlable-2.0.1/.github/dependabot.yml
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 xmlable-2.0.1/.github/workflows/pr.yml
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 xmlable-2.0.1/.github/workflows/pypi.yml
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/README.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/basic_config/config.xsd
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/basic_config/config_xml_example.xml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/basic_config/config_xml_template.xml
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/basic_config/main.py
--rw-r--r--   0        0        0     3649 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/complex/config.xsd
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/complex/config_xml_example.xml
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/complex/config_xml_template.xml
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/complex/main.py
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/complex_application/config.xsd
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/complex_application/config_xml_example.xml
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/complex_application/config_xml_template.xml
--rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/complex_application/ipconn.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/complex_application/main.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/maps/config.xsd
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/maps/config_xml_example.xml
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/maps/config_xml_template.xml
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/maps/main.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/namespaces/config.xsd
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/namespaces/config_xml_example.xml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/namespaces/config_xml_template.xml
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/namespaces/main.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/userdefined/config.xsd
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/userdefined/config_xml_example.xml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/userdefined/config_xml_template.xml
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/userdefined/main.py
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 xmlable-2.0.1/examples/userdefined/pgconn.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 xmlable-2.0.1/src/xmlable/__init__.py
--rw-r--r--   0        0        0     8972 2020-02-02 00:00:00.000000 xmlable-2.0.1/src/xmlable/_errors.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 xmlable-2.0.1/src/xmlable/_io.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 xmlable-2.0.1/src/xmlable/_lxml_helpers.py
--rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 xmlable-2.0.1/src/xmlable/_manual.py
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 xmlable-2.0.1/src/xmlable/_user.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 xmlable-2.0.1/src/xmlable/_utils.py
--rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 xmlable-2.0.1/src/xmlable/_xmlify.py
--rw-r--r--   0        0        0    20921 2020-02-02 00:00:00.000000 xmlable-2.0.1/src/xmlable/_xobject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xmlable-2.0.1/src/xmlable/py.typed
--rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 xmlable-2.0.1/tests/test_basic.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 xmlable-2.0.1/tests/test_errors.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 xmlable-2.0.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 xmlable-2.0.1/LICENSE
--rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 xmlable-2.0.1/README.md
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 xmlable-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 xmlable-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 xmlable-2.0.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 xmlable-2.0.2/.github/workflows/pr.yml
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 xmlable-2.0.2/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/README.md
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/basic_config/config.xsd
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/basic_config/config_xml_example.xml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/basic_config/config_xml_template.xml
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/basic_config/main.py
+-rw-r--r--   0        0        0     3649 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/complex/config.xsd
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/complex/config_xml_example.xml
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/complex/config_xml_template.xml
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/complex/main.py
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/complex_application/config.xsd
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/complex_application/config_xml_example.xml
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/complex_application/config_xml_template.xml
+-rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/complex_application/ipconn.py
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/complex_application/main.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/maps/config.xsd
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/maps/config_xml_example.xml
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/maps/config_xml_template.xml
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/maps/main.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/namespaces/config.xsd
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/namespaces/config_xml_example.xml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/namespaces/config_xml_template.xml
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/namespaces/main.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/userdefined/config.xsd
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/userdefined/config_xml_example.xml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/userdefined/config_xml_template.xml
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/userdefined/main.py
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 xmlable-2.0.2/examples/userdefined/pgconn.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 xmlable-2.0.2/src/xmlable/__init__.py
+-rw-r--r--   0        0        0     8973 2020-02-02 00:00:00.000000 xmlable-2.0.2/src/xmlable/_errors.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 xmlable-2.0.2/src/xmlable/_io.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 xmlable-2.0.2/src/xmlable/_lxml_helpers.py
+-rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 xmlable-2.0.2/src/xmlable/_manual.py
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 xmlable-2.0.2/src/xmlable/_user.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 xmlable-2.0.2/src/xmlable/_utils.py
+-rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 xmlable-2.0.2/src/xmlable/_xmlify.py
+-rw-r--r--   0        0        0    20922 2020-02-02 00:00:00.000000 xmlable-2.0.2/src/xmlable/_xobject.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xmlable-2.0.2/src/xmlable/py.typed
+-rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 xmlable-2.0.2/tests/test_basic.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 xmlable-2.0.2/tests/test_errors.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 xmlable-2.0.2/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 xmlable-2.0.2/LICENSE
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 xmlable-2.0.2/README.md
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 xmlable-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 xmlable-2.0.2/PKG-INFO
```

### Comparing `xmlable-2.0.1/.github/workflows/pr.yml` & `xmlable-2.0.2/.github/workflows/pr.yml`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/examples/basic_config/config.xsd` & `xmlable-2.0.2/examples/basic_config/config.xsd`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/examples/basic_config/main.py` & `xmlable-2.0.2/examples/basic_config/main.py`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/examples/complex/config.xsd` & `xmlable-2.0.2/examples/complex/config.xsd`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/examples/complex/config_xml_example.xml` & `xmlable-2.0.2/examples/complex/config_xml_example.xml`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/examples/complex/config_xml_template.xml` & `xmlable-2.0.2/examples/complex/config_xml_template.xml`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/examples/complex/main.py` & `xmlable-2.0.2/examples/complex/main.py`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/examples/complex_application/config.xsd` & `xmlable-2.0.2/examples/complex_application/config.xsd`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/examples/complex_application/config_xml_example.xml` & `xmlable-2.0.2/examples/complex_application/config_xml_example.xml`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/examples/complex_application/config_xml_template.xml` & `xmlable-2.0.2/examples/complex_application/config_xml_template.xml`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/examples/complex_application/ipconn.py` & `xmlable-2.0.2/examples/complex_application/ipconn.py`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/examples/complex_application/main.py` & `xmlable-2.0.2/examples/complex_application/main.py`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/examples/maps/config.xsd` & `xmlable-2.0.2/examples/maps/config.xsd`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/examples/maps/config_xml_example.xml` & `xmlable-2.0.2/examples/maps/config_xml_example.xml`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/examples/maps/config_xml_template.xml` & `xmlable-2.0.2/examples/maps/config_xml_template.xml`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/examples/maps/main.py` & `xmlable-2.0.2/examples/maps/main.py`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/examples/namespaces/config.xsd` & `xmlable-2.0.2/examples/namespaces/config.xsd`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/examples/namespaces/main.py` & `xmlable-2.0.2/examples/namespaces/main.py`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/examples/userdefined/config.xsd` & `xmlable-2.0.2/examples/userdefined/config.xsd`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/examples/userdefined/main.py` & `xmlable-2.0.2/examples/userdefined/main.py`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/examples/userdefined/pgconn.py` & `xmlable-2.0.2/examples/userdefined/pgconn.py`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/src/xmlable/_errors.py` & `xmlable-2.0.2/src/xmlable/_errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Colourful & descriptive errors for xmlable 
 - Clear messages
 - Trace for parsing
 """
+
 from dataclasses import dataclass
 from typing import Any, Iterable
 from termcolor import colored
 from termcolor.termcolor import Color
 
 from xmlable._utils import typename
```

### Comparing `xmlable-2.0.1/src/xmlable/_io.py` & `xmlable-2.0.2/src/xmlable/_io.py`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/src/xmlable/_lxml_helpers.py` & `xmlable-2.0.2/src/xmlable/_lxml_helpers.py`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/src/xmlable/_manual.py` & `xmlable-2.0.2/src/xmlable/_manual.py`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/src/xmlable/_user.py` & `xmlable-2.0.2/src/xmlable/_user.py`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/src/xmlable/_utils.py` & `xmlable-2.0.2/src/xmlable/_utils.py`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/src/xmlable/_xmlify.py` & `xmlable-2.0.2/src/xmlable/_xmlify.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Given a dataclass:
 - Produce an xsd schema based on the class
 - Produce an xml template based on the class
 - Given any instance of the class, make a best-effort attempt at turning it into
   a filled xml
 - Create a parser for parsing the xml
 """
+
 from humps import pascalize
 from dataclasses import fields, is_dataclass
 from typing import Any, dataclass_transform
 from lxml.objectify import ObjectifiedElement
 from lxml.etree import Element, _Element
 
 from xmlable._utils import get, typename
```

### Comparing `xmlable-2.0.1/src/xmlable/_xobject.py` & `xmlable-2.0.2/src/xmlable/_xobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ XObjects
 XObjects are an intermediate representation for python types -> xsd/xml
 - Produced by @xmlify decorated classes, and by gen_xobject
 - Associated xsd, xml and parsing 
 """
+
 from humps import pascalize
 from dataclasses import dataclass
 from types import NoneType, UnionType
 from lxml.objectify import ObjectifiedElement
 from lxml.etree import Element, Comment, _Element
 from abc import ABC, abstractmethod
 from typing import Any, Callable, get_args
```

### Comparing `xmlable-2.0.1/tests/test_basic.py` & `xmlable-2.0.2/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/tests/test_errors.py` & `xmlable-2.0.2/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/LICENSE` & `xmlable-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/README.md` & `xmlable-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `xmlable-2.0.1/pyproject.toml` & `xmlable-2.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "xmlable"
-version = "2.0.1"
+version = "2.0.2"
 authors = [
     { name = "Oliver Killane", email = "oliverkillane.business@gmail.com" },
 ]
 description = "A decorator for generating xsd, xml and parsers from dataclasses"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["xml", "xmlschema", "xsd", "lxml"]
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "lxml==4.9.3",
-    "lxml-stubs==0.4.0",
+    "lxml==5.2.1",
+    "lxml-stubs==0.5.1",
     "termcolor==2.4.0",
     "pyhumps==3.8.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/OliverKillane/xmlable"
 "Bug Tracker" = "https://github.com/OliverKillane/xmlable/issues"
 "Source" = "https://github.com/OliverKillane/xmlable"
 
 [project.optional-dependencies]
-dev = ["black==23.11.0", "mypy==1.7.1", "pytest==7.4.3"]
+dev = ["black==24.4.0", "mypy==1.9.0", "pytest==8.1.1"]
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-ra -q"
 pythonpath = ["src"]
 testpaths = ["tests"]
```

### Comparing `xmlable-2.0.1/PKG-INFO` & `xmlable-2.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: xmlable
-Version: 2.0.1
+Version: 2.0.2
 Summary: A decorator for generating xsd, xml and parsers from dataclasses
 Project-URL: Homepage, https://github.com/OliverKillane/xmlable
 Project-URL: Bug Tracker, https://github.com/OliverKillane/xmlable/issues
 Project-URL: Source, https://github.com/OliverKillane/xmlable
 Author-email: Oliver Killane <oliverkillane.business@gmail.com>
 License: MIT License
         
@@ -29,22 +29,22 @@
         SOFTWARE.
 License-File: LICENSE
 Keywords: lxml,xml,xmlschema,xsd
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
-Requires-Dist: lxml-stubs==0.4.0
-Requires-Dist: lxml==4.9.3
+Requires-Dist: lxml-stubs==0.5.1
+Requires-Dist: lxml==5.2.1
 Requires-Dist: pyhumps==3.8.0
 Requires-Dist: termcolor==2.4.0
 Provides-Extra: dev
-Requires-Dist: black==23.11.0; extra == 'dev'
-Requires-Dist: mypy==1.7.1; extra == 'dev'
-Requires-Dist: pytest==7.4.3; extra == 'dev'
+Requires-Dist: black==24.4.0; extra == 'dev'
+Requires-Dist: mypy==1.9.0; extra == 'dev'
+Requires-Dist: pytest==8.1.1; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # XMLable
 
 ## An easy xml/xsd generator and parser for python dataclasses!
 
 ```python
```

