# Comparing `tmp/qsharp-1.3.5.dev0-cp37-abi3-win_arm64.whl.zip` & `tmp/qsharp-1.3.6.dev0-cp37-abi3-win_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 1435713 bytes, number of entries: 14
--rw-r--r--  4.6 unx     2098 b- defN 24-Apr-01 20:07 qsharp-1.3.5.dev0.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 24-Apr-01 20:07 qsharp-1.3.5.dev0.dist-info/WHEEL
--rw-r--r--  4.6 unx     3090 b- defN 24-Apr-01 20:07 qsharp/.data/qsharp_codemirror.js
--rw-r--r--  4.6 unx    38836 b- defN 24-Apr-01 20:07 qsharp/estimator/_estimator.py
--rw-r--r--  4.6 unx      859 b- defN 24-Apr-01 20:07 qsharp/estimator/__init__.py
--rw-r--r--  4.6 unx     1706 b- defN 24-Apr-01 20:07 qsharp/utils/_utils.py
--rw-r--r--  4.6 unx      146 b- defN 24-Apr-01 20:07 qsharp/utils/__init__.py
--rw-r--r--  4.6 unx      864 b- defN 24-Apr-01 20:07 qsharp/_fs.py
--rw-r--r--  4.6 unx     1848 b- defN 24-Apr-01 20:07 qsharp/_ipython.py
--rw-r--r--  4.6 unx     6129 b- defN 24-Apr-01 20:07 qsharp/_native.pyi
--rw-r--r--  4.6 unx    11231 b- defN 24-Apr-01 20:07 qsharp/_qsharp.py
--rw-r--r--  4.6 unx      902 b- defN 24-Apr-01 20:07 qsharp/__init__.py
--rwxr-xr-x  4.6 unx  3515392 b- defN 24-Apr-01 20:07 qsharp/_native.pyd
--rw-r--r--  4.6 unx     1085 b- defN 24-Apr-01 20:07 qsharp-1.3.5.dev0.dist-info/RECORD
-14 files, 3584280 bytes uncompressed, 1433943 bytes compressed:  60.0%
+Zip file size: 1596621 bytes, number of entries: 14
+-rw-r--r--  4.6 unx     2098 b- defN 24-Apr-17 19:23 qsharp-1.3.6.dev0.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 24-Apr-17 19:23 qsharp-1.3.6.dev0.dist-info/WHEEL
+-rw-r--r--  4.6 unx     3090 b- defN 24-Apr-17 19:23 qsharp/.data/qsharp_codemirror.js
+-rw-r--r--  4.6 unx    38836 b- defN 24-Apr-17 19:23 qsharp/estimator/_estimator.py
+-rw-r--r--  4.6 unx      859 b- defN 24-Apr-17 19:23 qsharp/estimator/__init__.py
+-rw-r--r--  4.6 unx     1706 b- defN 24-Apr-17 19:23 qsharp/utils/_utils.py
+-rw-r--r--  4.6 unx      146 b- defN 24-Apr-17 19:23 qsharp/utils/__init__.py
+-rw-r--r--  4.6 unx      864 b- defN 24-Apr-17 19:23 qsharp/_fs.py
+-rw-r--r--  4.6 unx     1848 b- defN 24-Apr-17 19:23 qsharp/_ipython.py
+-rw-r--r--  4.6 unx     6375 b- defN 24-Apr-17 19:23 qsharp/_native.pyi
+-rw-r--r--  4.6 unx    11512 b- defN 24-Apr-17 19:23 qsharp/_qsharp.py
+-rw-r--r--  4.6 unx      902 b- defN 24-Apr-17 19:23 qsharp/__init__.py
+-rwxr-xr-x  4.6 unx  3882496 b- defN 24-Apr-17 19:23 qsharp/_native.pyd
+-rw-r--r--  4.6 unx     1085 b- defN 24-Apr-17 19:23 qsharp-1.3.6.dev0.dist-info/RECORD
+14 files, 3951911 bytes uncompressed, 1594851 bytes compressed:  59.7%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
-Filename: qsharp-1.3.5.dev0.dist-info/METADATA
+Filename: qsharp-1.3.6.dev0.dist-info/METADATA
 Comment: 
 
-Filename: qsharp-1.3.5.dev0.dist-info/WHEEL
+Filename: qsharp-1.3.6.dev0.dist-info/WHEEL
 Comment: 
 
 Filename: qsharp/.data/qsharp_codemirror.js
 Comment: 
 
 Filename: qsharp/estimator/_estimator.py
 Comment: 
@@ -33,11 +33,11 @@
 
 Filename: qsharp/__init__.py
 Comment: 
 
 Filename: qsharp/_native.pyd
 Comment: 
 
-Filename: qsharp-1.3.5.dev0.dist-info/RECORD
+Filename: qsharp-1.3.6.dev0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qsharp/_native.pyi

```diff
@@ -1,34 +1,43 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 
 from enum import Enum
-from typing import Any, Callable, ClassVar, Tuple, Optional, Dict, List
+from typing import Any, Callable, ClassVar, Optional, Dict, List
 
 class TargetProfile:
     """
     A Q# target profile.
 
-    The target is the hardware or simulator which will be used to run the Q# program.
-    The target profile is a description of a target's capabilities.
-    """
-
-    Unrestricted: ClassVar[Any]
-    """
-    Describes the unrestricted set of capabilities required to run any Q# program.
+    A target profile describes the capabilities of the hardware or simulator
+    which will be used to run the Q# program.
     """
 
     Base: ClassVar[Any]
     """
     Target supports the minimal set of capabilities required to run a quantum
     program.
 
     This option maps to the Base Profile as defined by the QIR specification.
     """
 
+    Quantinuum: ClassVar[Any]
+    """
+    Target supports Quantinuum profile.
+
+    This profile includes all of the required Adaptive Profile
+    capabilities, as well as the optional integer computation and qubit
+    reset capabilities, as defined by the QIR specification.
+    """
+
+    Unrestricted: ClassVar[Any]
+    """
+    Describes the unrestricted set of capabilities required to run any Q# program.
+    """
+
 class Interpreter:
     """A Q# interpreter."""
 
     def __init__(
         self,
         target_profile: TargetProfile,
         language_features: Optional[List[str]],
```

## qsharp/_qsharp.py

```diff
@@ -5,32 +5,38 @@
     Interpreter,
     TargetProfile,
     StateDumpData,
     QSharpError,
     Output,
     Circuit,
 )
+from warnings import warn
 from typing import Any, Callable, Dict, Optional, TypedDict, Union, List
 from .estimator._estimator import EstimatorResult, EstimatorParams
 import json
 
 _interpreter = None
 
 
 class Config:
     _config: Dict[str, str]
     """
     Configuration hints for the language service.
     """
 
     def __init__(self, target_profile: TargetProfile, language_features: List[str]):
-        if target_profile == TargetProfile.Unrestricted:
-            self._config = {"targetProfile": "unrestricted"}
+        if target_profile == TargetProfile.Quantinuum:
+            self._config = {"targetProfile": "quantinuum"}
+            warn("The Quantinuum target profile is a preview feature.")
+            warn("Functionality may be incomplete or incorrect.")
         elif target_profile == TargetProfile.Base:
             self._config = {"targetProfile": "base"}
+        elif target_profile == TargetProfile.Unrestricted:
+            self._config = {"targetProfile": "unrestricted"}
+
         self._config["languageFeatures"] = language_features
 
     def __repr__(self) -> str:
         return "Q# initialized with configuration: " + str(self._config)
 
     # See https://ipython.readthedocs.io/en/stable/config/integrating.html#rich-display
     # See https://ipython.org/ipython-doc/3/notebook/nbformat.html#display-data
```

## Comparing `qsharp-1.3.5.dev0.dist-info/METADATA` & `qsharp-1.3.6.dev0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsharp
-Version: 1.3.5.dev0
+Version: 1.3.6.dev0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

## Comparing `qsharp-1.3.5.dev0.dist-info/RECORD` & `qsharp-1.3.6.dev0.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-qsharp-1.3.5.dev0.dist-info/METADATA,sha256=lDlZ_JIIBK-ITlIrKZE_ToIBpooRIBIbYmqF7BCgnQY,2098
-qsharp-1.3.5.dev0.dist-info/WHEEL,sha256=xsrEGIMmQ1avWDJ2-RvHLDam8haXzwGnBhrUlFUsLAc,94
+qsharp-1.3.6.dev0.dist-info/METADATA,sha256=ds9Xe3pp7phe62a97KpEmjT4P_DItAxuDbA0BBo5Cj8,2098
+qsharp-1.3.6.dev0.dist-info/WHEEL,sha256=xsrEGIMmQ1avWDJ2-RvHLDam8haXzwGnBhrUlFUsLAc,94
 qsharp/.data/qsharp_codemirror.js,sha256=72E3fTxGxfBe_bBhPD5-8ul_S61MLVA_JmMJwOXgmhc,3090
 qsharp/estimator/_estimator.py,sha256=LMTJg2xPwhvswlc0ts0zsjRPd82mF5KzYgmHyFFl2PE,38836
 qsharp/estimator/__init__.py,sha256=JK6oDnNX_rgsPnfyFsK0yxMBRinmW8jlc8183BydxXA,859
 qsharp/utils/_utils.py,sha256=s3ausLf4wp08rgRDrcdzSXOYPRQ63isX0umCA9MIq7M,1706
 qsharp/utils/__init__.py,sha256=ejBPCXRttEGKCDehjldx8SryqQfNHXsgsRFK5O-zRU8,146
 qsharp/_fs.py,sha256=RGhwMRUwfxGoPVEPaP39FxyRcPeZoyhB0kb4MwzxE54,864
 qsharp/_ipython.py,sha256=x8J7HatTw15xTg9Ppd-yRmhNz9eY8cBAhruRiHo46bQ,1848
-qsharp/_native.pyi,sha256=6ga5-snfFILNktO__JUjYxpZNrx9Te_xIQJOiPcvsik,6129
-qsharp/_qsharp.py,sha256=tGrOLgZh89KiL2JE-QzRgVbzFkNY03v-VImRhZ4cB2M,11231
+qsharp/_native.pyi,sha256=w0bBah7mtOnoLcchXMfMoH6PJaf1Bm0lmSJe8574s4U,6375
+qsharp/_qsharp.py,sha256=h3zPZ91r85sTvJJU7y-L9HNJeQZTzO3MVI4uzfrCWb0,11512
 qsharp/__init__.py,sha256=-KmJgZV8ZRqWSIOENAhyE39vYF5eZ_p4W04XZ29YKfs,902
-qsharp/_native.pyd,sha256=IJPh6CLPZz6joSV7JV1s_PUCvhLK_1YeqvZyO27zH2E,3515392
-qsharp-1.3.5.dev0.dist-info/RECORD,,
+qsharp/_native.pyd,sha256=0GpYp8Ct26jaz7sv40allwuwe_FpeD9M5e5g8BJtM5s,3882496
+qsharp-1.3.6.dev0.dist-info/RECORD,,
```

