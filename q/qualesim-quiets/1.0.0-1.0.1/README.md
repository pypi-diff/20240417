# Comparing `tmp/qualesim-quiets-1.0.0.tar.gz` & `tmp/qualesim-quiets-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qualesim-quiets-1.0.0.tar", last modified: Fri Mar 29 08:21:07 2024, max compression
+gzip compressed data, was "qualesim-quiets-1.0.1.tar", last modified: Wed Apr 17 01:54:43 2024, max compression
```

## Comparing `qualesim-quiets-1.0.0.tar` & `qualesim-quiets-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-03-29 08:21:07.197492 qualesim-quiets-1.0.0/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    35149 2023-09-28 06:57:55.000000 qualesim-quiets-1.0.0/LICENSE
--rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      852 2024-03-29 08:21:07.197492 qualesim-quiets-1.0.0/PKG-INFO
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      250 2024-01-02 01:13:56.000000 qualesim-quiets-1.0.0/README.md
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-03-29 08:21:07.193492 qualesim-quiets-1.0.0/data/
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-03-29 08:21:07.197492 qualesim-quiets-1.0.0/data/bin/
--rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)      192 2024-01-02 01:31:17.000000 qualesim-quiets-1.0.0/data/bin/dqcsfeqi
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-03-29 08:21:07.197492 qualesim-quiets-1.0.0/qualesim_quiets/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2023-09-28 06:57:55.000000 qualesim-quiets-1.0.0/qualesim_quiets/__init__.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      192 2024-01-02 01:17:17.000000 qualesim-quiets-1.0.0/qualesim_quiets/__main__.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    43408 2024-03-29 08:01:27.000000 qualesim-quiets-1.0.0/qualesim_quiets/frontend.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    11207 2024-03-29 08:01:37.000000 qualesim-quiets-1.0.0/qualesim_quiets/utils.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-03-29 08:21:07.197492 qualesim-quiets-1.0.0/qualesim_quiets.egg-info/
--rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      852 2024-03-29 08:21:07.000000 qualesim-quiets-1.0.0/qualesim_quiets.egg-info/PKG-INFO
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      405 2024-03-29 08:21:07.000000 qualesim-quiets-1.0.0/qualesim_quiets.egg-info/SOURCES.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        1 2024-03-29 08:21:07.000000 qualesim-quiets-1.0.0/qualesim_quiets.egg-info/dependency_links.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       18 2024-03-29 08:21:07.000000 qualesim-quiets-1.0.0/qualesim_quiets.egg-info/requires.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       16 2024-03-29 08:21:07.000000 qualesim-quiets-1.0.0/qualesim_quiets.egg-info/top_level.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       38 2024-03-29 08:21:07.197492 qualesim-quiets-1.0.0/setup.cfg
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1086 2024-03-29 08:00:19.000000 qualesim-quiets-1.0.0/setup.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-03-29 08:21:07.197492 qualesim-quiets-1.0.0/tests/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     9572 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.0/tests/test_cls.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     7477 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.0/tests/test_gate.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     6223 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.0/tests/test_qifile.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 01:54:43.348481 qualesim-quiets-1.0.1/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    35149 2023-09-28 06:57:55.000000 qualesim-quiets-1.0.1/LICENSE
+-rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      852 2024-04-17 01:54:43.348481 qualesim-quiets-1.0.1/PKG-INFO
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      250 2024-01-02 01:13:56.000000 qualesim-quiets-1.0.1/README.md
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 01:54:43.344481 qualesim-quiets-1.0.1/data/
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 01:54:43.344481 qualesim-quiets-1.0.1/data/bin/
+-rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)      192 2024-01-02 01:31:17.000000 qualesim-quiets-1.0.1/data/bin/dqcsfeqi
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 01:54:43.344481 qualesim-quiets-1.0.1/qualesim_quiets/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2023-09-28 06:57:55.000000 qualesim-quiets-1.0.1/qualesim_quiets/__init__.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      192 2024-01-02 01:17:17.000000 qualesim-quiets-1.0.1/qualesim_quiets/__main__.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    43747 2024-04-17 01:54:17.000000 qualesim-quiets-1.0.1/qualesim_quiets/frontend.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    11427 2024-04-17 01:47:13.000000 qualesim-quiets-1.0.1/qualesim_quiets/utils.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 01:54:43.348481 qualesim-quiets-1.0.1/qualesim_quiets.egg-info/
+-rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      852 2024-04-17 01:54:43.000000 qualesim-quiets-1.0.1/qualesim_quiets.egg-info/PKG-INFO
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      405 2024-04-17 01:54:43.000000 qualesim-quiets-1.0.1/qualesim_quiets.egg-info/SOURCES.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        1 2024-04-17 01:54:43.000000 qualesim-quiets-1.0.1/qualesim_quiets.egg-info/dependency_links.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       18 2024-04-17 01:54:43.000000 qualesim-quiets-1.0.1/qualesim_quiets.egg-info/requires.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       16 2024-04-17 01:54:43.000000 qualesim-quiets-1.0.1/qualesim_quiets.egg-info/top_level.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       38 2024-04-17 01:54:43.348481 qualesim-quiets-1.0.1/setup.cfg
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1086 2024-04-17 01:36:48.000000 qualesim-quiets-1.0.1/setup.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 01:54:43.348481 qualesim-quiets-1.0.1/tests/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     9572 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.1/tests/test_cls.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     7477 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.1/tests/test_gate.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     6223 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.1/tests/test_qifile.py
```

### Comparing `qualesim-quiets-1.0.0/LICENSE` & `qualesim-quiets-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qualesim-quiets-1.0.0/PKG-INFO` & `qualesim-quiets-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualesim-quiets
-Version: 1.0.0
+Version: 1.0.1
 Summary: QuaLeSim frontend for QUIET-S.
 Home-page: https://gitee.com/hpcl_quanta/dqcsim-quiets.git
 Author: Dingdong Liu
 Author-email: dingdongliu@quanta.org.cn
 License: GPLv3
 Keywords: qualesim quiets
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `qualesim-quiets-1.0.0/qualesim_quiets/frontend.py` & `qualesim-quiets-1.0.1/qualesim_quiets/frontend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 from qualesim.plugin import *
 from qualesim.host import *
-from qir.QiProg import *
+from pyquiet.qir.QiProg import *
+from pyquiet.QiParser.QiParser import QiParser
+from pyquiet.qir.qModule.IntInstruction import QuietImInstruction
+from pyquiet.qir.qModule.FloatInstructions import QuietFmInstruction
+from pyquiet.qir.qbody.Function import QiLabelTable
+from pyquiet.qir import (
+    FunctionCall,
+    QiDefineGate,
+    QiVariable,
+    QiList,
+    DoubleType,
+    IntType,
+    QiProgram,
+)
 from typing import List
 from antlr4 import *
-from QiParser.QiParser import QiParser
 from .utils import *
 from pathlib import Path
 
 
 @plugin("QUIET-S", "DDL", "0.0.2")
 class QUIETs(Frontend):
     """QUIETs frontend plugin. Must be implemented with the input *.qi file"""
```

### Comparing `qualesim-quiets-1.0.0/qualesim_quiets/utils.py` & `qualesim-quiets-1.0.1/qualesim_quiets/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 from typing import Union
 from qualesim.plugin import *
 from qualesim.host import *
-from qir.QiProg import *
+from pyquiet.qir.QiProg import *
+from pyquiet.qir.qModule.StdInstructions import QuietStdInstruction
+from pyquiet.qir import QiVariable, VariableDecl, QiList
+from pyquiet.qir.Variable import QuietVariable
+from pyquiet.qir.Type import QuietType
+
 from typing import List
 from antlr4 import *
 import numpy as np
 
 
 class QiDataStack:
     def __init__(self) -> None:
```

### Comparing `qualesim-quiets-1.0.0/qualesim_quiets.egg-info/PKG-INFO` & `qualesim-quiets-1.0.1/qualesim_quiets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualesim-quiets
-Version: 1.0.0
+Version: 1.0.1
 Summary: QuaLeSim frontend for QUIET-S.
 Home-page: https://gitee.com/hpcl_quanta/dqcsim-quiets.git
 Author: Dingdong Liu
 Author-email: dingdongliu@quanta.org.cn
 License: GPLv3
 Keywords: qualesim quiets
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `qualesim-quiets-1.0.0/setup.py` & `qualesim-quiets-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname)) as f:
         return f.read()
 
 
 setup(
     name="qualesim-quiets",
-    version="1.0.0",
+    version="1.0.1",
     author="Dingdong Liu",
     author_email="dingdongliu@quanta.org.cn",
     description="QuaLeSim frontend for QUIET-S.",
     license="GPLv3",
     keywords="qualesim quiets",
     url="https://gitee.com/hpcl_quanta/dqcsim-quiets.git",
     long_description=read("README.md"),
```

### Comparing `qualesim-quiets-1.0.0/tests/test_cls.py` & `qualesim-quiets-1.0.1/tests/test_cls.py`

 * *Files identical despite different names*

### Comparing `qualesim-quiets-1.0.0/tests/test_gate.py` & `qualesim-quiets-1.0.1/tests/test_gate.py`

 * *Files identical despite different names*

### Comparing `qualesim-quiets-1.0.0/tests/test_qifile.py` & `qualesim-quiets-1.0.1/tests/test_qifile.py`

 * *Files identical despite different names*

