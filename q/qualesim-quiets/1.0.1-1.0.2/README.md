# Comparing `tmp/qualesim-quiets-1.0.1.tar.gz` & `tmp/qualesim-quiets-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qualesim-quiets-1.0.1.tar", last modified: Wed Apr 17 01:54:43 2024, max compression
+gzip compressed data, was "qualesim-quiets-1.0.2.tar", last modified: Wed Apr 17 07:31:55 2024, max compression
```

## Comparing `qualesim-quiets-1.0.1.tar` & `qualesim-quiets-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 01:54:43.348481 qualesim-quiets-1.0.1/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    35149 2023-09-28 06:57:55.000000 qualesim-quiets-1.0.1/LICENSE
--rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      852 2024-04-17 01:54:43.348481 qualesim-quiets-1.0.1/PKG-INFO
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      250 2024-01-02 01:13:56.000000 qualesim-quiets-1.0.1/README.md
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 01:54:43.344481 qualesim-quiets-1.0.1/data/
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 01:54:43.344481 qualesim-quiets-1.0.1/data/bin/
--rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)      192 2024-01-02 01:31:17.000000 qualesim-quiets-1.0.1/data/bin/dqcsfeqi
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 01:54:43.344481 qualesim-quiets-1.0.1/qualesim_quiets/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2023-09-28 06:57:55.000000 qualesim-quiets-1.0.1/qualesim_quiets/__init__.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      192 2024-01-02 01:17:17.000000 qualesim-quiets-1.0.1/qualesim_quiets/__main__.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    43747 2024-04-17 01:54:17.000000 qualesim-quiets-1.0.1/qualesim_quiets/frontend.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    11427 2024-04-17 01:47:13.000000 qualesim-quiets-1.0.1/qualesim_quiets/utils.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 01:54:43.348481 qualesim-quiets-1.0.1/qualesim_quiets.egg-info/
--rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      852 2024-04-17 01:54:43.000000 qualesim-quiets-1.0.1/qualesim_quiets.egg-info/PKG-INFO
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      405 2024-04-17 01:54:43.000000 qualesim-quiets-1.0.1/qualesim_quiets.egg-info/SOURCES.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        1 2024-04-17 01:54:43.000000 qualesim-quiets-1.0.1/qualesim_quiets.egg-info/dependency_links.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       18 2024-04-17 01:54:43.000000 qualesim-quiets-1.0.1/qualesim_quiets.egg-info/requires.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       16 2024-04-17 01:54:43.000000 qualesim-quiets-1.0.1/qualesim_quiets.egg-info/top_level.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       38 2024-04-17 01:54:43.348481 qualesim-quiets-1.0.1/setup.cfg
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1086 2024-04-17 01:36:48.000000 qualesim-quiets-1.0.1/setup.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 01:54:43.348481 qualesim-quiets-1.0.1/tests/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     9572 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.1/tests/test_cls.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     7477 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.1/tests/test_gate.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     6223 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.1/tests/test_qifile.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 07:31:55.215607 qualesim-quiets-1.0.2/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    35149 2023-09-28 06:57:55.000000 qualesim-quiets-1.0.2/LICENSE
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      789 2024-04-17 07:31:55.215607 qualesim-quiets-1.0.2/PKG-INFO
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      250 2024-01-02 01:13:56.000000 qualesim-quiets-1.0.2/README.md
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 07:31:55.207607 qualesim-quiets-1.0.2/data/
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 07:31:55.211607 qualesim-quiets-1.0.2/data/bin/
+-rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)      192 2024-01-02 01:31:17.000000 qualesim-quiets-1.0.2/data/bin/dqcsfeqi
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 07:31:55.211607 qualesim-quiets-1.0.2/qualesim_quiets/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2023-09-28 06:57:55.000000 qualesim-quiets-1.0.2/qualesim_quiets/__init__.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      192 2024-01-02 01:17:17.000000 qualesim-quiets-1.0.2/qualesim_quiets/__main__.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    43747 2024-04-17 02:46:48.000000 qualesim-quiets-1.0.2/qualesim_quiets/frontend.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    11426 2024-04-17 02:46:12.000000 qualesim-quiets-1.0.2/qualesim_quiets/utils.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 07:31:55.215607 qualesim-quiets-1.0.2/qualesim_quiets.egg-info/
+-rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      789 2024-04-17 07:31:55.000000 qualesim-quiets-1.0.2/qualesim_quiets.egg-info/PKG-INFO
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      405 2024-04-17 07:31:55.000000 qualesim-quiets-1.0.2/qualesim_quiets.egg-info/SOURCES.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        1 2024-04-17 07:31:55.000000 qualesim-quiets-1.0.2/qualesim_quiets.egg-info/dependency_links.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       18 2024-04-17 07:31:55.000000 qualesim-quiets-1.0.2/qualesim_quiets.egg-info/requires.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       16 2024-04-17 07:31:55.000000 qualesim-quiets-1.0.2/qualesim_quiets.egg-info/top_level.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       38 2024-04-17 07:31:55.215607 qualesim-quiets-1.0.2/setup.cfg
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1086 2024-04-17 02:46:12.000000 qualesim-quiets-1.0.2/setup.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 07:31:55.215607 qualesim-quiets-1.0.2/tests/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     9572 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.2/tests/test_cls.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     7477 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.2/tests/test_gate.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     6223 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.2/tests/test_qifile.py
```

### Comparing `qualesim-quiets-1.0.1/LICENSE` & `qualesim-quiets-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qualesim-quiets-1.0.1/PKG-INFO` & `qualesim-quiets-1.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: qualesim-quiets
-Version: 1.0.1
+Version: 1.0.2
 Summary: QuaLeSim frontend for QUIET-S.
 Home-page: https://gitee.com/hpcl_quanta/dqcsim-quiets.git
 Author: Dingdong Liu
 Author-email: dingdongliu@quanta.org.cn
 License: GPLv3
 Keywords: qualesim quiets
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: ply
-Requires-Dist: pyquiet
 
 # DQCSim-Quiets
 
 #### 介绍
 1. 本前端为QuaLeSim-QUIETS前端，为QuaLeSim框架提供了一个可以识别QUIET-S量子-经典混合指令集的前端插件。
 
 #### 安装教程
```

### Comparing `qualesim-quiets-1.0.1/qualesim_quiets/frontend.py` & `qualesim-quiets-1.0.2/qualesim_quiets/frontend.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,15 +304,15 @@
                     if (
                         func_data.func_qubit[ii][jj]
                         not in func_data.qubit_measure.keys()
                     ):
                         if len(func_data.func_qubit[ii]) == 1:
                             func_data.res_qubit.append(ii)
                         else:
-                            func_data.res_qubit.append(str(ii) + "[" + str(ik) + "]")
+                            func_data.res_qubit.append(str(ii) + "[" + str(jj) + "]")
             res_state_vector["classical"] = res_cls
             if measure_mod == "state_vector":
                 if measure_flag == 1:
                     res_state_vector["quantum"] = (
                         func_data.res_qubit,
                         eval(func_data.state_vector)[1],
                     )
```

### Comparing `qualesim-quiets-1.0.1/qualesim_quiets/utils.py` & `qualesim-quiets-1.0.2/qualesim_quiets/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from qualesim.plugin import *
 from qualesim.host import *
 from pyquiet.qir.QiProg import *
 from pyquiet.qir.qModule.StdInstructions import QuietStdInstruction
 from pyquiet.qir import QiVariable, VariableDecl, QiList
 from pyquiet.qir.Variable import QuietVariable
 from pyquiet.qir.Type import QuietType
-
 from typing import List
 from antlr4 import *
 import numpy as np
 
 
 class QiDataStack:
     def __init__(self) -> None:
```

### Comparing `qualesim-quiets-1.0.1/qualesim_quiets.egg-info/PKG-INFO` & `qualesim-quiets-1.0.2/qualesim_quiets.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: qualesim-quiets
-Version: 1.0.1
+Version: 1.0.2
 Summary: QuaLeSim frontend for QUIET-S.
 Home-page: https://gitee.com/hpcl_quanta/dqcsim-quiets.git
 Author: Dingdong Liu
 Author-email: dingdongliu@quanta.org.cn
 License: GPLv3
 Keywords: qualesim quiets
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: ply
-Requires-Dist: pyquiet
 
 # DQCSim-Quiets
 
 #### 介绍
 1. 本前端为QuaLeSim-QUIETS前端，为QuaLeSim框架提供了一个可以识别QUIET-S量子-经典混合指令集的前端插件。
 
 #### 安装教程
```

### Comparing `qualesim-quiets-1.0.1/setup.py` & `qualesim-quiets-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname)) as f:
         return f.read()
 
 
 setup(
     name="qualesim-quiets",
-    version="1.0.1",
+    version="1.0.2",
     author="Dingdong Liu",
     author_email="dingdongliu@quanta.org.cn",
     description="QuaLeSim frontend for QUIET-S.",
     license="GPLv3",
     keywords="qualesim quiets",
     url="https://gitee.com/hpcl_quanta/dqcsim-quiets.git",
     long_description=read("README.md"),
```

### Comparing `qualesim-quiets-1.0.1/tests/test_cls.py` & `qualesim-quiets-1.0.2/tests/test_cls.py`

 * *Files identical despite different names*

### Comparing `qualesim-quiets-1.0.1/tests/test_gate.py` & `qualesim-quiets-1.0.2/tests/test_gate.py`

 * *Files identical despite different names*

### Comparing `qualesim-quiets-1.0.1/tests/test_qifile.py` & `qualesim-quiets-1.0.2/tests/test_qifile.py`

 * *Files identical despite different names*

