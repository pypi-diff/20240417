# Comparing `tmp/qaoa-1.0.2.tar.gz` & `tmp/qaoa-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qaoa-1.0.2.tar", last modified: Fri Sep 29 18:42:28 2023, max compression
+gzip compressed data, was "qaoa-1.0.3.tar", last modified: Wed Apr 17 12:20:10 2024, max compression
```

## Comparing `qaoa-1.0.2.tar` & `qaoa-1.0.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 franzf    (1000) users      (985)        0 2023-09-29 18:42:28.495389 qaoa-1.0.2/
--rw-r--r--   0 franzf    (1000) users      (985)    35149 2023-09-12 07:03:36.000000 qaoa-1.0.2/LICENSE
--rw-r--r--   0 franzf    (1000) users      (985)     5925 2023-09-29 18:42:28.495389 qaoa-1.0.2/PKG-INFO
--rw-r--r--   0 franzf    (1000) users      (985)     5572 2023-09-24 18:41:42.000000 qaoa-1.0.2/README.md
-drwxr-xr-x   0 franzf    (1000) users      (985)        0 2023-09-29 18:42:28.492055 qaoa-1.0.2/qaoa/
--rw-r--r--   0 franzf    (1000) users      (985)       96 2023-09-24 18:43:31.000000 qaoa-1.0.2/qaoa/__init__.py
-drwxr-xr-x   0 franzf    (1000) users      (985)        0 2023-09-29 18:42:28.492055 qaoa-1.0.2/qaoa/initialstates/
--rw-r--r--   0 franzf    (1000) users      (985)      173 2023-09-25 07:50:47.000000 qaoa-1.0.2/qaoa/initialstates/__init__.py
--rw-r--r--   0 franzf    (1000) users      (985)     2112 2023-09-24 18:41:42.000000 qaoa-1.0.2/qaoa/initialstates/base_initialstate.py
--rw-r--r--   0 franzf    (1000) users      (985)      561 2023-09-28 17:27:40.000000 qaoa-1.0.2/qaoa/initialstates/dicke_initialstate.py
--rw-r--r--   0 franzf    (1000) users      (985)      361 2023-09-24 18:41:42.000000 qaoa-1.0.2/qaoa/initialstates/plus_initialstate.py
--rw-r--r--   0 franzf    (1000) users      (985)      447 2023-09-24 18:41:42.000000 qaoa-1.0.2/qaoa/initialstates/statevector_initialstate.py
-drwxr-xr-x   0 franzf    (1000) users      (985)        0 2023-09-29 18:42:28.492055 qaoa-1.0.2/qaoa/mixers/
--rw-r--r--   0 franzf    (1000) users      (985)      154 2023-09-24 18:43:31.000000 qaoa-1.0.2/qaoa/mixers/__init__.py
--rw-r--r--   0 franzf    (1000) users      (985)     2256 2023-09-24 18:41:42.000000 qaoa-1.0.2/qaoa/mixers/base_mixer.py
--rw-r--r--   0 franzf    (1000) users      (985)     1437 2023-09-24 18:41:42.000000 qaoa-1.0.2/qaoa/mixers/constrained_mixer.py
--rw-r--r--   0 franzf    (1000) users      (985)     2390 2023-09-29 18:41:19.000000 qaoa-1.0.2/qaoa/mixers/grover_mixer.py
--rw-r--r--   0 franzf    (1000) users      (985)    16227 2023-09-12 07:03:36.000000 qaoa-1.0.2/qaoa/mixers/mixer_utilities.py
--rw-r--r--   0 franzf    (1000) users      (985)      358 2023-09-24 18:41:42.000000 qaoa-1.0.2/qaoa/mixers/x_mixer.py
--rw-r--r--   0 franzf    (1000) users      (985)     2529 2023-09-28 17:27:40.000000 qaoa-1.0.2/qaoa/mixers/xy_mixer.py
-drwxr-xr-x   0 franzf    (1000) users      (985)        0 2023-09-29 18:42:28.495389 qaoa-1.0.2/qaoa/problems/
--rw-r--r--   0 franzf    (1000) users      (985)      196 2023-09-24 18:43:31.000000 qaoa-1.0.2/qaoa/problems/__init__.py
--rw-r--r--   0 franzf    (1000) users      (985)     3836 2023-09-29 18:41:19.000000 qaoa-1.0.2/qaoa/problems/base_problem.py
--rw-r--r--   0 franzf    (1000) users      (985)     1872 2023-09-24 18:41:42.000000 qaoa-1.0.2/qaoa/problems/exactcover_problem.py
--rw-r--r--   0 franzf    (1000) users      (985)     1196 2023-09-24 18:43:31.000000 qaoa-1.0.2/qaoa/problems/maxcut_problem.py
--rw-r--r--   0 franzf    (1000) users      (985)     1979 2023-09-24 18:43:31.000000 qaoa-1.0.2/qaoa/problems/portfolio_problem.py
--rw-r--r--   0 franzf    (1000) users      (985)     3107 2023-09-24 18:43:31.000000 qaoa-1.0.2/qaoa/problems/qubo_problem.py
--rw-r--r--   0 franzf    (1000) users      (985)    16563 2023-09-29 15:34:38.000000 qaoa-1.0.2/qaoa/qaoa.py
-drwxr-xr-x   0 franzf    (1000) users      (985)        0 2023-09-29 18:42:28.495389 qaoa-1.0.2/qaoa/util/
--rw-r--r--   0 franzf    (1000) users      (985)       73 2023-09-28 17:27:40.000000 qaoa-1.0.2/qaoa/util/__init__.py
--rw-r--r--   0 franzf    (1000) users      (985)     3669 2023-09-28 17:27:40.000000 qaoa-1.0.2/qaoa/util/dicke_circuit.py
--rw-r--r--   0 franzf    (1000) users      (985)     1356 2023-09-29 15:34:38.000000 qaoa-1.0.2/qaoa/util/statistic.py
-drwxr-xr-x   0 franzf    (1000) users      (985)        0 2023-09-29 18:42:28.492055 qaoa-1.0.2/qaoa.egg-info/
--rw-r--r--   0 franzf    (1000) users      (985)     5925 2023-09-29 18:42:28.000000 qaoa-1.0.2/qaoa.egg-info/PKG-INFO
--rw-r--r--   0 franzf    (1000) users      (985)      844 2023-09-29 18:42:28.000000 qaoa-1.0.2/qaoa.egg-info/SOURCES.txt
--rw-r--r--   0 franzf    (1000) users      (985)        1 2023-09-29 18:42:28.000000 qaoa-1.0.2/qaoa.egg-info/dependency_links.txt
--rw-r--r--   0 franzf    (1000) users      (985)      112 2023-09-29 18:42:28.000000 qaoa-1.0.2/qaoa.egg-info/requires.txt
--rw-r--r--   0 franzf    (1000) users      (985)        5 2023-09-29 18:42:28.000000 qaoa-1.0.2/qaoa.egg-info/top_level.txt
--rw-r--r--   0 franzf    (1000) users      (985)       38 2023-09-29 18:42:28.495389 qaoa-1.0.2/setup.cfg
--rw-r--r--   0 franzf    (1000) users      (985)      791 2023-09-29 15:34:38.000000 qaoa-1.0.2/setup.py
+drwxr-xr-x   0 franzf    (1000) users      (985)        0 2024-04-17 12:20:10.463823 qaoa-1.0.3/
+-rw-r--r--   0 franzf    (1000) users      (985)    35149 2023-09-12 07:03:36.000000 qaoa-1.0.3/LICENSE
+-rw-r--r--   0 franzf    (1000) users      (985)     5923 2024-04-17 12:20:10.463823 qaoa-1.0.3/PKG-INFO
+-rw-r--r--   0 franzf    (1000) users      (985)     5570 2024-04-17 12:14:19.000000 qaoa-1.0.3/README.md
+drwxr-xr-x   0 franzf    (1000) users      (985)        0 2024-04-17 12:20:10.460489 qaoa-1.0.3/qaoa/
+-rw-r--r--   0 franzf    (1000) users      (985)       96 2023-09-24 18:43:31.000000 qaoa-1.0.3/qaoa/__init__.py
+drwxr-xr-x   0 franzf    (1000) users      (985)        0 2024-04-17 12:20:10.463823 qaoa-1.0.3/qaoa/initialstates/
+-rw-r--r--   0 franzf    (1000) users      (985)      173 2023-09-25 07:50:47.000000 qaoa-1.0.3/qaoa/initialstates/__init__.py
+-rw-r--r--   0 franzf    (1000) users      (985)     2112 2023-09-24 18:41:42.000000 qaoa-1.0.3/qaoa/initialstates/base_initialstate.py
+-rw-r--r--   0 franzf    (1000) users      (985)      561 2023-09-28 17:27:40.000000 qaoa-1.0.3/qaoa/initialstates/dicke_initialstate.py
+-rw-r--r--   0 franzf    (1000) users      (985)      361 2023-09-24 18:41:42.000000 qaoa-1.0.3/qaoa/initialstates/plus_initialstate.py
+-rw-r--r--   0 franzf    (1000) users      (985)      447 2023-09-24 18:41:42.000000 qaoa-1.0.3/qaoa/initialstates/statevector_initialstate.py
+drwxr-xr-x   0 franzf    (1000) users      (985)        0 2024-04-17 12:20:10.463823 qaoa-1.0.3/qaoa/mixers/
+-rw-r--r--   0 franzf    (1000) users      (985)      154 2023-09-24 18:43:31.000000 qaoa-1.0.3/qaoa/mixers/__init__.py
+-rw-r--r--   0 franzf    (1000) users      (985)     2256 2023-09-24 18:41:42.000000 qaoa-1.0.3/qaoa/mixers/base_mixer.py
+-rw-r--r--   0 franzf    (1000) users      (985)     1437 2023-09-24 18:41:42.000000 qaoa-1.0.3/qaoa/mixers/constrained_mixer.py
+-rw-r--r--   0 franzf    (1000) users      (985)     2390 2024-04-17 12:14:19.000000 qaoa-1.0.3/qaoa/mixers/grover_mixer.py
+-rw-r--r--   0 franzf    (1000) users      (985)    16227 2023-09-12 07:03:36.000000 qaoa-1.0.3/qaoa/mixers/mixer_utilities.py
+-rw-r--r--   0 franzf    (1000) users      (985)      358 2023-09-24 18:41:42.000000 qaoa-1.0.3/qaoa/mixers/x_mixer.py
+-rw-r--r--   0 franzf    (1000) users      (985)     2529 2023-09-28 17:27:40.000000 qaoa-1.0.3/qaoa/mixers/xy_mixer.py
+drwxr-xr-x   0 franzf    (1000) users      (985)        0 2024-04-17 12:20:10.463823 qaoa-1.0.3/qaoa/problems/
+-rw-r--r--   0 franzf    (1000) users      (985)      196 2023-09-24 18:43:31.000000 qaoa-1.0.3/qaoa/problems/__init__.py
+-rw-r--r--   0 franzf    (1000) users      (985)     3836 2024-04-17 12:14:19.000000 qaoa-1.0.3/qaoa/problems/base_problem.py
+-rw-r--r--   0 franzf    (1000) users      (985)     2124 2024-04-17 12:14:19.000000 qaoa-1.0.3/qaoa/problems/exactcover_problem.py
+-rw-r--r--   0 franzf    (1000) users      (985)     1196 2023-09-24 18:43:31.000000 qaoa-1.0.3/qaoa/problems/maxcut_problem.py
+-rw-r--r--   0 franzf    (1000) users      (985)     1979 2023-09-24 18:43:31.000000 qaoa-1.0.3/qaoa/problems/portfolio_problem.py
+-rw-r--r--   0 franzf    (1000) users      (985)     3183 2024-04-17 12:14:19.000000 qaoa-1.0.3/qaoa/problems/qubo_problem.py
+-rw-r--r--   0 franzf    (1000) users      (985)    19142 2024-04-17 12:14:19.000000 qaoa-1.0.3/qaoa/qaoa.py
+drwxr-xr-x   0 franzf    (1000) users      (985)        0 2024-04-17 12:20:10.463823 qaoa-1.0.3/qaoa/util/
+-rw-r--r--   0 franzf    (1000) users      (985)       73 2023-09-28 17:27:40.000000 qaoa-1.0.3/qaoa/util/__init__.py
+-rw-r--r--   0 franzf    (1000) users      (985)     3669 2023-09-28 17:27:40.000000 qaoa-1.0.3/qaoa/util/dicke_circuit.py
+-rw-r--r--   0 franzf    (1000) users      (985)     1947 2024-04-17 12:14:19.000000 qaoa-1.0.3/qaoa/util/statistic.py
+drwxr-xr-x   0 franzf    (1000) users      (985)        0 2024-04-17 12:20:10.463823 qaoa-1.0.3/qaoa.egg-info/
+-rw-r--r--   0 franzf    (1000) users      (985)     5923 2024-04-17 12:20:10.000000 qaoa-1.0.3/qaoa.egg-info/PKG-INFO
+-rw-r--r--   0 franzf    (1000) users      (985)      844 2024-04-17 12:20:10.000000 qaoa-1.0.3/qaoa.egg-info/SOURCES.txt
+-rw-r--r--   0 franzf    (1000) users      (985)        1 2024-04-17 12:20:10.000000 qaoa-1.0.3/qaoa.egg-info/dependency_links.txt
+-rw-r--r--   0 franzf    (1000) users      (985)      112 2024-04-17 12:20:10.000000 qaoa-1.0.3/qaoa.egg-info/requires.txt
+-rw-r--r--   0 franzf    (1000) users      (985)        5 2024-04-17 12:20:10.000000 qaoa-1.0.3/qaoa.egg-info/top_level.txt
+-rw-r--r--   0 franzf    (1000) users      (985)       38 2024-04-17 12:20:10.463823 qaoa-1.0.3/setup.cfg
+-rw-r--r--   0 franzf    (1000) users      (985)      791 2024-04-17 12:20:04.000000 qaoa-1.0.3/setup.py
```

### Comparing `qaoa-1.0.2/LICENSE` & `qaoa-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qaoa-1.0.2/PKG-INFO` & `qaoa-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaoa
-Version: 1.0.2
+Version: 1.0.3
 Summary: Quantum Alternating Operator Ansatz/Quantum Approximate Optimization Algorithm (QAOA)
 Author: Franz Georg Fuchs
 Author-email: franzgeorgfuchs@gmail.com
 License: GNU General Public License v3.0
 Keywords: quantum computing,qaoa,qiskit
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -99,23 +99,23 @@
 
 	qaoa = QAOA( ...,
 		backend= ,
 		noisemodel= ,
 		optimizer= ,
 		precision= ,
 		shots= ,
-		alpha=
+		cvar=
 	)
 
 - `backend`: the backend to be used, defaults to `Aer.get_backend("qasm_simulator")`
 - `noisemodel`: the noise model to be used, default to `None`,
 - `optimizer`: a list of the optimizer to be used from qiskit-algorithms together with options, defaults to `[COBYLA, {}]`,
 - `precision`: sampel until a certain precision of the expectation value is reached based on $\text{error}=\frac{\text{variance}}{\sqrt{\text{shots}}}$, defaults to `None`,
 - `shots`: number of shots to be used, defaults to `1024`,
-- `alpha`: the value for [conditional value at risk (CVAR)](https://arxiv.org/pdf/1907.04769.pdf), defaults to `1`, which are the standard moments.
+- `cvar`: the value for [conditional value at risk (CVAR)](https://arxiv.org/pdf/1907.04769.pdf), defaults to `1`, which are the standard moments.
 
 ***
 ### Extract results
 
 Once `qaoa.optimize(depth=p)` is run, one can extract, the expectation value, variance, and parametres for each depth $1\leq i \leq p$ by respectively calling:
 
 	qaoa.get_Exp(depth=i)
```

### Comparing `qaoa-1.0.2/README.md` & `qaoa-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -88,23 +88,23 @@
 
 	qaoa = QAOA( ...,
 		backend= ,
 		noisemodel= ,
 		optimizer= ,
 		precision= ,
 		shots= ,
-		alpha=
+		cvar=
 	)
 
 - `backend`: the backend to be used, defaults to `Aer.get_backend("qasm_simulator")`
 - `noisemodel`: the noise model to be used, default to `None`,
 - `optimizer`: a list of the optimizer to be used from qiskit-algorithms together with options, defaults to `[COBYLA, {}]`,
 - `precision`: sampel until a certain precision of the expectation value is reached based on $\text{error}=\frac{\text{variance}}{\sqrt{\text{shots}}}$, defaults to `None`,
 - `shots`: number of shots to be used, defaults to `1024`,
-- `alpha`: the value for [conditional value at risk (CVAR)](https://arxiv.org/pdf/1907.04769.pdf), defaults to `1`, which are the standard moments.
+- `cvar`: the value for [conditional value at risk (CVAR)](https://arxiv.org/pdf/1907.04769.pdf), defaults to `1`, which are the standard moments.
 
 ***
 ### Extract results
 
 Once `qaoa.optimize(depth=p)` is run, one can extract, the expectation value, variance, and parametres for each depth $1\leq i \leq p$ by respectively calling:
 
 	qaoa.get_Exp(depth=i)
```

### Comparing `qaoa-1.0.2/qaoa/initialstates/base_initialstate.py` & `qaoa-1.0.3/qaoa/initialstates/base_initialstate.py`

 * *Files identical despite different names*

### Comparing `qaoa-1.0.2/qaoa/initialstates/dicke_initialstate.py` & `qaoa-1.0.3/qaoa/initialstates/dicke_initialstate.py`

 * *Files identical despite different names*

### Comparing `qaoa-1.0.2/qaoa/mixers/base_mixer.py` & `qaoa-1.0.3/qaoa/mixers/base_mixer.py`

 * *Files identical despite different names*

### Comparing `qaoa-1.0.2/qaoa/mixers/constrained_mixer.py` & `qaoa-1.0.3/qaoa/mixers/constrained_mixer.py`

 * *Files identical despite different names*

### Comparing `qaoa-1.0.2/qaoa/mixers/grover_mixer.py` & `qaoa-1.0.3/qaoa/mixers/grover_mixer.py`

 * *Files identical despite different names*

### Comparing `qaoa-1.0.2/qaoa/mixers/mixer_utilities.py` & `qaoa-1.0.3/qaoa/mixers/mixer_utilities.py`

 * *Files identical despite different names*

### Comparing `qaoa-1.0.2/qaoa/mixers/xy_mixer.py` & `qaoa-1.0.3/qaoa/mixers/xy_mixer.py`

 * *Files identical despite different names*

### Comparing `qaoa-1.0.2/qaoa/problems/base_problem.py` & `qaoa-1.0.3/qaoa/problems/base_problem.py`

 * *Files identical despite different names*

### Comparing `qaoa-1.0.2/qaoa/problems/exactcover_problem.py` & `qaoa-1.0.3/qaoa/problems/exactcover_problem.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,63 +7,63 @@
 
 from qiskit.circuit import Parameter
 
 
 class ExactCover(Problem):
     def __init__(
         self,
-        FR,
-        CR=None,
-        mu=1,
+        columns,
+        weights=None,
+        penalty_factor=1,
     ) -> None:
-        self.FR = FR
-        self.CR = CR
-        self.mu = 1
+        self.columns = columns 
+        self.weights = weights 
+        self.penalty_factor = penalty_factor
 
-        fN = FR.shape[0]  ### number of flights
-        rN = FR.shape[1]  ### number of routes
+        colSize = columns.shape[0]  ### Size per column
+        numColumns = columns.shape[1]  ### number of columns/qubits
 
-        self.N_qubits = rN
+        self.N_qubits = numColumns
 
     def cost(self, string):
         x = np.array(list(map(int, string)))
         c_e = self.__exactCover(x)
 
-        if self.CR is None:
+        if self.weights is None:
             return -c_e
         else:
-            return -(self.CR @ x + self.mu * c_e)
+            return -(self.weights @ x + self.penalty_factor * c_e)
 
     def create_circuit(self):
         """
         Creates parameterized circuit corresponding to the cost function
         """
         q = QuantumRegister(self.N_qubits)
         self.circuit = QuantumCircuit(q)
         cost_param = Parameter("x_gamma")
 
-        F, R = np.shape(self.FR)
+        colSize, numColumns = np.shape(self.columns) 
 
         ### cost Hamiltonian
-        for r in range(R):
-            hr = self.mu * 0.5 * self.FR[:, r] @ (np.sum(self.FR, axis=1) - 2)
-            if not self.CR is None:
-                hr += 0.5 * self.CR[r]
+        for col in range(numColumns):
+            hr = self.penalty_factor * 0.5 * self.columns[:, col] @ (np.sum(self.columns, axis=1) - 2)
+            if not self.weights is None:
+                hr += 0.5 * self.weights[col]
 
             if not math.isclose(hr, 0, abs_tol=1e-7):
-                self.circuit.rz(cost_param * hr, q[r])
+                self.circuit.rz(cost_param * hr, q[col])
 
-            for r_ in range(r + 1, R):
-                Jrr_ = self.mu * 0.5 * self.FR[:, r] @ self.FR[:, r_]
+            for col_ in range(col + 1, numColumns):
+                Jrr_ = self.penalty_factor * 0.5 * self.columns[:, col] @ self.columns[:, col_]
 
                 if not math.isclose(Jrr_, 0, abs_tol=1e-7):
-                    self.circuit.cx(q[r], q[r_])
-                    self.circuit.rz(cost_param * Jrr_, q[r_])
-                    self.circuit.cx(q[r], q[r_])
+                    self.circuit.cx(q[col], q[col_])
+                    self.circuit.rz(cost_param * Jrr_, q[col_])
+                    self.circuit.cx(q[col], q[col_])
 
     def isFeasible(self, string):
         x = np.array(list(map(int, string)))
         c_e = self.__exactCover(x)
         return math.isclose(c_e, 0, abs_tol=1e-7)
 
     def __exactCover(self, x):
-        return np.sum((1 - (self.FR @ x)) ** 2)
+        return np.sum((1 - (self.columns @ x)) ** 2)
```

### Comparing `qaoa-1.0.2/qaoa/problems/maxcut_problem.py` & `qaoa-1.0.3/qaoa/problems/maxcut_problem.py`

 * *Files identical despite different names*

### Comparing `qaoa-1.0.2/qaoa/problems/portfolio_problem.py` & `qaoa-1.0.3/qaoa/problems/portfolio_problem.py`

 * *Files identical despite different names*

### Comparing `qaoa-1.0.2/qaoa/problems/qubo_problem.py` & `qaoa-1.0.3/qaoa/problems/qubo_problem.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 
 class QUBO(Problem):
     def __init__(self, Q=None, c=None, b=None) -> None:
         """
         Implements the mapping from the parameters in params to the QUBO problem.
         Is expected to be called by the child class.
+
+        # The QUBO will be on this form:
+        # min x^T Q x + c^T x + b
         """
         assert type(Q) is np.ndarray, "Q needs to be a numpy ndarray, but is " + str(
             type(Q)
         )
         assert (
             Q.ndim == 2
         ), "Q needs to be a 2-dimensional numpy ndarray, but has dim " + str(Q.ndim)
```

### Comparing `qaoa-1.0.2/qaoa/qaoa.py` & `qaoa-1.0.3/qaoa/qaoa.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,26 +22,28 @@
 
     def __init__(self, depth):
         self.depth = depth
 
         self.angles = []
         self.Exp = []
         self.Var = []
-        self.MaxCost = []
-        self.MinCost = []
+        self.WorstCost = []
+        self.BestCost = []
+        self.BestSols = []
         self.shots = []
 
         self.index_Exp_min = -1
 
     def add_iteration(self, angles, stat, shots):
         self.angles.append(angles)
         self.Exp.append(-stat.get_CVaR())
         self.Var.append(stat.get_Variance())
-        self.MaxCost.append(-stat.get_max())
-        self.MinCost.append(-stat.get_min())
+        self.BestCost.append(-stat.get_max())
+        self.WorstCost.append(-stat.get_min())
+        self.BestSols.append(stat.get_max_sols())
         self.shots.append(shots)
 
     def compute_best_index(self):
         self.index_Exp_min = self.Exp.index(min(self.Exp))
 
     def get_best_Exp(self):
         return self.Exp[self.index_Exp_min]
@@ -54,14 +56,26 @@
 
     def num_fval(self):
         return len(self.Exp)
 
     def num_shots(self):
         return sum(self.shots)
 
+    def get_best_solution(self):
+        best_cost = np.min(self.BestCost)
+        iterations_with_best_cost = np.where(self.BestCost == best_cost)[0]
+
+        all_best_sols = []
+        for i in iterations_with_best_cost:
+            all_best_sols.append(self.BestSols[i])
+        # flatten the list:
+        all_best_sols = [item for sublist in all_best_sols for item in sublist]
+        best_sols = np.unique(all_best_sols)
+        return best_sols, best_cost
+
 
 class QAOA:
     """Main class"""
 
     def __init__(
         self,
         problem,
@@ -69,14 +83,15 @@
         initialstate,
         backend=Aer.get_backend("qasm_simulator"),
         noisemodel=None,
         optimizer=[COBYLA, {}],  # optimizer, options
         precision=None,
         shots=1024,
         cvar=1,
+        memorysize=-1,
     ) -> None:
         """
         A QAO-Ansatz consist of these parts:
 
         :problem of Basetype Problem,
         implementing the phase circuit and the cost.
 
@@ -84,15 +99,15 @@
         specifying the mixer circuit.
 
         :initialstate of Basetype InitialState,
         specifying the initial state.
 
         :backend: backend
         :noisemodel: noisemodel
-        :optmizer: optimizer
+        :optmizer: optimizer as a list containing [optimizer object, options dict]
         :precision: precision to reach for expectation value based on error=variance/sqrt(shots)
         :shots: if precision=None, the number of samples taken
                       if precision!=None, the minimum number of samples taken
         :cvar: used for CVar
         """
 
         assert issubclass(type(problem), Problem)
@@ -111,14 +126,16 @@
         self.backend = backend
         self.optimizer = optimizer
         self.noisemodel = noisemodel
         self.shots = shots
         self.precision = precision
         self.stat = Statistic(cvar=cvar)
         self.cvar = cvar
+        self.memorysize = memorysize
+        self.memory = self.memorysize > 0
 
         self.usebarrier = False
         self.isQNSPSA = False
 
         self.current_depth = 0  # depth at which local optimization has been done
 
         self.gamma_params = None
@@ -127,14 +144,15 @@
         self.Exp_sampled_p1 = None
         self.landscape_p1_angles = {}
         self.Var_sampled_p1 = None
         self.MaxCost_sampled_p1 = None
         self.MinCost_sampled_p1 = None
 
         self.optimization_results = {}
+        self.memory_lists = []
 
     def exp_landscape(self):
         ### at depth p = 1
         return self.Exp_sampled_p1
 
     def var_landscape(self):
         ### at depth p = 1
@@ -161,14 +179,22 @@
         return self.optimization_results[depth].get_best_angles()[1::2]
 
     def get_gamma(self, depth):
         if depth > self.current_depth + 1:
             raise ValueError
         return self.optimization_results[depth].get_best_angles()[::2]
 
+    def get_angles(self, depth):
+        if depth > self.current_depth + 1:
+            raise ValueError
+        return self.optimization_results[depth].get_best_angles()
+
+    def get_memory_lists(self):
+        return self.memory_lists
+
     def createParameterizedCircuit(self, depth):
         if self.parameterized_circuit_depth == depth:
             LOG.info(
                 "Circuit is already of depth " + str(self.parameterized_circuit_depth)
             )
             return
 
@@ -247,14 +273,15 @@
             logger.info(f"parameters: {len(parameters)}")
             job = execute(
                 self.parameterized_circuit,
                 self.backend,
                 shots=self.shots,
                 parameter_binds=[parameters],
                 optimization_level=0,
+                memory=self.memory,
             )
             logger.info("Done execute")
             self.measurementStatistics(job)
             logger.info("Done measurement")
 
         else:
             raise NotImplementedError
@@ -266,25 +293,38 @@
         implements a function for expectation value and variance
 
         :param job: job instance derived from BaseJob
         :return: expectation and variance, if the job is a list
         """
         jres = job.result()
         counts_list = jres.get_counts()
+
+        if self.memorysize > 0:
+            for i, _ in enumerate(jres.results):
+                memory_list = jres.get_memory(experiment=i)
+                if self.memorysize > 0:
+                    for measurement in memory_list:
+                        self.memory_lists.append(
+                            [measurement, self.problem.cost(measurement[::-1])]
+                        )
+                        self.memorysize -= 1
+                        if self.memorysize < 1:
+                            break
+
         if isinstance(counts_list, list):
             expectations = []
             variances = []
             maxcosts = []
             mincosts = []
             for i, counts in enumerate(counts_list):
                 self.stat.reset()
                 for string in counts:
                     # qiskit binary strings use little endian encoding, but our cost function expects big endian encoding. Therefore, we reverse the order
                     cost = self.problem.cost(string[::-1])
-                    self.stat.add_sample(cost, counts[string])
+                    self.stat.add_sample(cost, counts[string], string[::-1])
                 expectations.append(self.stat.get_CVaR())
                 variances.append(self.stat.get_Variance())
                 maxcosts.append(self.stat.get_max())
                 mincosts.append(self.stat.get_min())
             angles = self.landscape_p1_angles
             self.Exp_sampled_p1 = -np.array(expectations).reshape(
                 angles["beta"][2], angles["gamma"][2]
@@ -298,35 +338,31 @@
             self.MinCost_sampled_p1 = -np.array(mincosts).reshape(
                 angles["beta"][2], angles["gamma"][2]
             )
         else:
             for string in counts_list:
                 # qiskit binary strings use little endian encoding, but our cost function expects big endian encoding. Therefore, we reverse the order
                 cost = self.problem.cost(string[::-1])
-                self.stat.add_sample(cost, counts_list[string])
+                self.stat.add_sample(cost, counts_list[string], string[::-1])
 
     def optimize(self, depth):
         ## run local optimization by iteratively increasing the depth until depth p is reached
         while self.current_depth < depth:
             if self.current_depth == 0:
                 if self.Exp_sampled_p1 is None:
                     self.sample_cost_landscape()
                 ind_Emin = np.unravel_index(
                     np.argmin(self.Exp_sampled_p1, axis=None), self.Exp_sampled_p1.shape
                 )
                 angles0 = np.array(
                     (self.gamma_grid[ind_Emin[1]], self.beta_grid[ind_Emin[0]])
                 )
             else:
-                gamma = self.optimization_results[self.current_depth].get_best_angles()[
-                    ::2
-                ]
-                beta = self.optimization_results[self.current_depth].get_best_angles()[
-                    1::2
-                ]
+                gamma = self.get_gamma(self.current_depth)
+                beta = self.get_beta(self.current_depth)
 
                 gamma_interp = self.interp(gamma)
                 beta_interp = self.interp(beta)
                 angles0 = np.zeros(2 * (self.current_depth + 1))
                 angles0[::2] = gamma_interp
                 angles0[1::2] = beta_interp
 
@@ -386,14 +422,15 @@
                 job = execute(
                     self.parameterized_circuit,
                     backend=self.backend,
                     noise_model=self.noisemodel,
                     shots=shots,
                     parameter_binds=[params],
                     optimization_level=0,
+                    memory=self.memory,
                 )
             else:
                 raise NotImplementedError
             shots_taken += shots
             self.measurementStatistics(job)
             if self.precision is None:
                 break
@@ -453,25 +490,53 @@
         if self.backend.configuration().local:
             job = execute(
                 self.parameterized_circuit,
                 self.backend,
                 shots=shots,
                 parameter_binds=[params],
                 optimization_level=0,
+                memory=self.memory,
             )
         else:
             raise NotImplementedError
-        return job.result().get_counts()
+
+        # Qiskit uses big endian encoding, cost function uses litle endian encoding.
+        # Therefore the string is reversed before passing it to the cost function.
+        hist = job.result().get_counts()
+        corrected_hist = {}
+        for string in hist:
+            corrected_hist[string[::-1]] = hist[string]
+        return corrected_hist
 
     def random_init(self, gamma_bounds, beta_bounds, depth):
         """
         Enforces the bounds of gamma and beta based on the graph type.
         :param gamma_bounds: Parameter bound tuple (min,max) for gamma
         :param beta_bounds: Parameter bound tuple (min,max) for beta
         :return: np.array on the form (gamma_1, beta_1, gamma_2, ...., gamma_d, beta_d)
         """
         gamma_list = np.random.uniform(gamma_bounds[0], gamma_bounds[1], size=depth)
         beta_list = np.random.uniform(beta_bounds[0], beta_bounds[1], size=depth)
         initial = np.empty((gamma_list.size + beta_list.size,), dtype=gamma_list.dtype)
         initial[0::2] = gamma_list
         initial[1::2] = beta_list
         return initial
+
+    def get_optimal_solutions(self):
+        """
+        Iterates through all optimization result objects looking for the bit-string(s)
+        that gave optimal cost value.
+        :return: list with the obtained best bit-strings
+        """
+        best_sols = []
+        best_costs = []
+        for i in self.optimization_results:
+            best_sols_i, best_cost_i = self.optimization_results[i].get_best_solution()
+            best_sols.append(best_sols_i)
+            best_costs.append(best_cost_i)
+
+        best_iterations = np.where(best_costs == np.min(best_costs))[0]
+        opt_sols = []
+        for i in best_iterations:
+            opt_sols.append(best_sols[i])
+        opt_sols = [item for sublist in opt_sols for item in sublist]
+        return np.unique(opt_sols)
```

### Comparing `qaoa-1.0.2/qaoa/util/dicke_circuit.py` & `qaoa-1.0.3/qaoa/util/dicke_circuit.py`

 * *Files identical despite different names*

### Comparing `qaoa-1.0.2/qaoa.egg-info/PKG-INFO` & `qaoa-1.0.3/qaoa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaoa
-Version: 1.0.2
+Version: 1.0.3
 Summary: Quantum Alternating Operator Ansatz/Quantum Approximate Optimization Algorithm (QAOA)
 Author: Franz Georg Fuchs
 Author-email: franzgeorgfuchs@gmail.com
 License: GNU General Public License v3.0
 Keywords: quantum computing,qaoa,qiskit
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -99,23 +99,23 @@
 
 	qaoa = QAOA( ...,
 		backend= ,
 		noisemodel= ,
 		optimizer= ,
 		precision= ,
 		shots= ,
-		alpha=
+		cvar=
 	)
 
 - `backend`: the backend to be used, defaults to `Aer.get_backend("qasm_simulator")`
 - `noisemodel`: the noise model to be used, default to `None`,
 - `optimizer`: a list of the optimizer to be used from qiskit-algorithms together with options, defaults to `[COBYLA, {}]`,
 - `precision`: sampel until a certain precision of the expectation value is reached based on $\text{error}=\frac{\text{variance}}{\sqrt{\text{shots}}}$, defaults to `None`,
 - `shots`: number of shots to be used, defaults to `1024`,
-- `alpha`: the value for [conditional value at risk (CVAR)](https://arxiv.org/pdf/1907.04769.pdf), defaults to `1`, which are the standard moments.
+- `cvar`: the value for [conditional value at risk (CVAR)](https://arxiv.org/pdf/1907.04769.pdf), defaults to `1`, which are the standard moments.
 
 ***
 ### Extract results
 
 Once `qaoa.optimize(depth=p)` is run, one can extract, the expectation value, variance, and parametres for each depth $1\leq i \leq p$ by respectively calling:
 
 	qaoa.get_Exp(depth=i)
```

### Comparing `qaoa-1.0.2/qaoa.egg-info/SOURCES.txt` & `qaoa-1.0.3/qaoa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qaoa-1.0.2/setup.py` & `qaoa-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="qaoa",
-    version="1.0.2",
+    version="1.0.3",
     license="GNU General Public License v3.0",
     author="Franz Georg Fuchs",
     author_email="franzgeorgfuchs@gmail.com",
     description="Quantum Alternating Operator Ansatz/Quantum Approximate Optimization Algorithm (QAOA)",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=["examples", "images"]),
```

