# Comparing `tmp/pytket_pysimplex-0.8.0-py3-none-any.whl.zip` & `tmp/pytket_pysimplex-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 11108 bytes, number of entries: 10
--rw-r--r--  2.0 unx      842 b- defN 23-Jun-20 16:56 pytket/extensions/pysimplex/__init__.py
--rw-r--r--  2.0 unx       72 b- defN 23-Jun-20 16:56 pytket/extensions/pysimplex/_metadata.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-20 16:56 pytket/extensions/pysimplex/py.typed
--rw-r--r--  2.0 unx      724 b- defN 23-Jun-20 16:56 pytket/extensions/pysimplex/backends/__init__.py
--rw-r--r--  2.0 unx     6225 b- defN 23-Jun-20 16:56 pytket/extensions/pysimplex/backends/simplex_backend.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-20 16:56 pytket_pysimplex-0.8.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3956 b- defN 23-Jun-20 16:56 pytket_pysimplex-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 16:56 pytket_pysimplex-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jun-20 16:56 pytket_pysimplex-0.8.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      927 b- defN 23-Jun-20 16:56 pytket_pysimplex-0.8.0.dist-info/RECORD
-10 files, 24202 bytes uncompressed, 9482 bytes compressed:  60.8%
+Zip file size: 11128 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      826 b- defN 23-Sep-11 09:37 pytket/extensions/pysimplex/__init__.py
+-rw-r--r--  2.0 unx       72 b- defN 23-Sep-11 09:37 pytket/extensions/pysimplex/_metadata.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Sep-11 09:37 pytket/extensions/pysimplex/py.typed
+-rw-r--r--  2.0 unx      724 b- defN 23-Sep-11 09:37 pytket/extensions/pysimplex/backends/__init__.py
+-rw-r--r--  2.0 unx     6320 b- defN 23-Sep-11 09:37 pytket/extensions/pysimplex/backends/simplex_backend.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Sep-11 09:37 pytket_pysimplex-0.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3952 b- defN 23-Sep-11 09:37 pytket_pysimplex-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Sep-11 09:37 pytket_pysimplex-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Sep-11 09:37 pytket_pysimplex-0.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      927 b- defN 23-Sep-11 09:37 pytket_pysimplex-0.9.0.dist-info/RECORD
+10 files, 24277 bytes uncompressed, 9502 bytes compressed:  60.9%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: pytket/extensions/pysimplex/backends/__init__.py
 Comment: 
 
 Filename: pytket/extensions/pysimplex/backends/simplex_backend.py
 Comment: 
 
-Filename: pytket_pysimplex-0.8.0.dist-info/LICENSE
+Filename: pytket_pysimplex-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: pytket_pysimplex-0.8.0.dist-info/METADATA
+Filename: pytket_pysimplex-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: pytket_pysimplex-0.8.0.dist-info/WHEEL
+Filename: pytket_pysimplex-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: pytket_pysimplex-0.8.0.dist-info/top_level.txt
+Filename: pytket_pysimplex-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pytket_pysimplex-0.8.0.dist-info/RECORD
+Filename: pytket_pysimplex-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytket/extensions/pysimplex/__init__.py

```diff
@@ -12,9 +12,9 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Pytket extension for using the pysimplex Clifford simulator
 """
 
 # _metadata.py is copied to the folder after installation.
-from ._metadata import __extension_version__, __extension_name__  # type: ignore
+from ._metadata import __extension_version__, __extension_name__
 from .backends import SimplexBackend
```

## pytket/extensions/pysimplex/_metadata.py

```diff
@@ -1,2 +1,2 @@
-__extension_version__ = "0.8.0"
+__extension_version__ = "0.9.0"
 __extension_name__ = "pytket-pysimplex"
```

## pytket/extensions/pysimplex/backends/simplex_backend.py

```diff
@@ -21,29 +21,30 @@
     CircuitNotRunError,
     CircuitStatus,
     ResultHandle,
     StatusEnum,
 )
 from pytket.backends.backendresult import BackendResult
 from pytket.backends.resulthandle import _ResultIdTuple
-from pytket.circuit import Circuit, OpType  # type: ignore
-from pytket.passes import (  # type: ignore
+from pytket.circuit import Circuit, OpType
+from pytket.passes import (
     BasePass,
     DecomposeBoxes,
     FlattenRegisters,
     RebaseCustom,
     RemoveRedundancies,
     SequencePass,
 )
-from pytket.predicates import (  # type: ignore
+from pytket.predicates import (
     DefaultRegisterPredicate,
     GateSetPredicate,
     NoClassicalControlPredicate,
     Predicate,
 )
+from pytket.unit_id import Bit, Qubit
 from pytket.utils.outcomearray import OutcomeArray
 from pytket.utils.results import KwargTypes
 
 _gateset = {
     OpType.X,
     OpType.Y,
     OpType.Z,
@@ -56,15 +57,15 @@
     OpType.Measure,
 }
 
 
 def _int_double(x: float) -> int:
     # return (2x) mod 8 if x is close to a half-integer, otherwise error
     y = 2 * x
-    n = int(np.round(y))  # type: ignore
+    n = int(np.round(y))
     if np.isclose(y, n):
         return n % 8
     else:
         raise ValueError("Non-Clifford angle encountered")
 
 
 def _tk1_to_cliff(a: float, b: float, c: float) -> Circuit:
@@ -104,19 +105,21 @@
         S = Simplex(n_qubits)
         measurements = [0] * n_bits
         for cmd in cmds:
             optype = cmd.op.type
             args = cmd.args
             if optype == OpType.Measure:
                 qarg, carg = args
+                assert isinstance(qarg, Qubit)
+                assert isinstance(carg, Bit)
                 qb = qubits.index(qarg)
                 cb = bits.index(carg)
                 measurements[cb] = S.MeasZ(qb)
             else:
-                qbs = [qubits.index(arg) for arg in args]
+                qbs = [qubits.index(cast(Qubit, arg)) for arg in args]
                 if optype == OpType.X:
                     S.X(*qbs)
                 elif optype == OpType.Y:
                     S.Y(*qbs)
                 elif optype == OpType.Z:
                     S.Z(*qbs)
                 elif optype == OpType.H:
@@ -150,15 +153,15 @@
         return [
             DefaultRegisterPredicate(),
             GateSetPredicate(_gateset),
             NoClassicalControlPredicate(),
         ]
 
     def rebase_pass(self) -> BasePass:
-        return RebaseCustom(_gateset, Circuit(), _tk1_to_cliff)
+        return RebaseCustom(_gateset, Circuit(), _tk1_to_cliff)  # type: ignore
 
     def default_compilation_pass(self, optimisation_level: int = 1) -> BasePass:
         # No optimization.
         return SequencePass(
             [
                 DecomposeBoxes(),
                 FlattenRegisters(),
```

## Comparing `pytket_pysimplex-0.8.0.dist-info/LICENSE` & `pytket_pysimplex-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pytket_pysimplex-0.8.0.dist-info/METADATA` & `pytket_pysimplex-0.9.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-pysimplex
-Version: 0.8.0
+Version: 0.9.0
 Summary: Extension for pytket, providing access to the pysimplex Clifford simulator
 Author: TKET development team
 Author-email: tket-support@cambridgequantum.com
 License: Apache 2
 Project-URL: Documentation, https://cqcl.github.io/pytket-pysimplex/api/index.html
 Project-URL: Source, https://github.com/CQCL/pytket-pysimplex
 Project-URL: Tracker, https://github.com/CQCL/pytket-pysimplex/issues
@@ -17,16 +17,16 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pytket (~=1.16)
-Requires-Dist: pysimplex (~=1.4)
+Requires-Dist: pytket ~=1.19
+Requires-Dist: pysimplex ~=1.4
 
 # Pytket Extensions
 
 This repository contains the pytket-pysimplex extension, using Quantinuum's
 [pytket](https://cqcl.github.io/tket/pytket/api/index.html) quantum SDK.
 
 # pytket-pysimplex
```

