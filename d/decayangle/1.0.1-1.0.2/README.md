# Comparing `tmp/decayangle-1.0.1.tar.gz` & `tmp/decayangle-1.0.2.tar.gz`

## Comparing `decayangle-1.0.1.tar` & `decayangle-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0    21702 2020-02-02 00:00:00.000000 decayangle-1.0.1/.pylintrc
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 decayangle-1.0.1/docs/Makefile
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 decayangle-1.0.1/docs/conf.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 decayangle-1.0.1/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 decayangle-1.0.1/docs/make.bat
--rw-r--r--   0        0        0    17345 2020-02-02 00:00:00.000000 decayangle-1.0.1/notebooks/decay_example.ipynb
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 decayangle-1.0.1/src/decayangle/__about__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 decayangle-1.0.1/src/decayangle/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 decayangle-1.0.1/src/decayangle/backend.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 decayangle-1.0.1/src/decayangle/config.py
--rw-r--r--   0        0        0    31233 2020-02-02 00:00:00.000000 decayangle-1.0.1/src/decayangle/decay_topology.py
--rw-r--r--   0        0        0    17593 2020-02-02 00:00:00.000000 decayangle-1.0.1/src/decayangle/kinematics.py
--rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 decayangle-1.0.1/src/decayangle/lorentz.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 decayangle-1.0.1/src/decayangle/numerics_helpers.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 decayangle-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 decayangle-1.0.1/tests/test_Nbody.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 decayangle-1.0.1/tests/test_decay.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 decayangle-1.0.1/tests/test_kinematics.py
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 decayangle-1.0.1/tests/test_lorentz.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 decayangle-1.0.1/tests/test_sorting.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 decayangle-1.0.1/tests/test_topology.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 decayangle-1.0.1/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 decayangle-1.0.1/LICENSE.md
--rw-r--r--   0        0        0    10948 2020-02-02 00:00:00.000000 decayangle-1.0.1/README.md
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 decayangle-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    12069 2020-02-02 00:00:00.000000 decayangle-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    21702 2020-02-02 00:00:00.000000 decayangle-1.0.2/.pylintrc
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 decayangle-1.0.2/docs/Makefile
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 decayangle-1.0.2/docs/conf.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 decayangle-1.0.2/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 decayangle-1.0.2/docs/make.bat
+-rw-r--r--   0        0        0    18517 2020-02-02 00:00:00.000000 decayangle-1.0.2/notebooks/decay_example.ipynb
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 decayangle-1.0.2/src/decayangle/__about__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 decayangle-1.0.2/src/decayangle/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 decayangle-1.0.2/src/decayangle/backend.py
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 decayangle-1.0.2/src/decayangle/config.py
+-rw-r--r--   0        0        0    31347 2020-02-02 00:00:00.000000 decayangle-1.0.2/src/decayangle/decay_topology.py
+-rw-r--r--   0        0        0    17707 2020-02-02 00:00:00.000000 decayangle-1.0.2/src/decayangle/kinematics.py
+-rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 decayangle-1.0.2/src/decayangle/lorentz.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 decayangle-1.0.2/src/decayangle/numerics_helpers.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 decayangle-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 decayangle-1.0.2/tests/test_Nbody.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 decayangle-1.0.2/tests/test_config.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 decayangle-1.0.2/tests/test_decay.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 decayangle-1.0.2/tests/test_kinematics.py
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 decayangle-1.0.2/tests/test_lorentz.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 decayangle-1.0.2/tests/test_sorting.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 decayangle-1.0.2/tests/test_topology.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 decayangle-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 decayangle-1.0.2/LICENSE.md
+-rw-r--r--   0        0        0    11392 2020-02-02 00:00:00.000000 decayangle-1.0.2/README.md
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 decayangle-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    12513 2020-02-02 00:00:00.000000 decayangle-1.0.2/PKG-INFO
```

### Comparing `decayangle-1.0.1/.pylintrc` & `decayangle-1.0.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.1/docs/Makefile` & `decayangle-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.1/docs/conf.py` & `decayangle-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.1/docs/index.rst` & `decayangle-1.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.1/docs/make.bat` & `decayangle-1.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.1/notebooks/decay_example.ipynb` & `decayangle-1.0.2/notebooks/decay_example.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9925656288156288%*

 * *Differences: {"'cells'": "{0: {'execution_count': 1, 'outputs': {0: {'text': {insert: [(0, 'Requirement already "*

 * *            'satisfied: particle in '*

 * *            "/home/kai/anaconda3/envs/decayangle/lib/python3.12/site-packages (0.23.1)\\n'), (1, "*

 * *            "'Requirement already satisfied: attrs>=19.2 in "*

 * *            '/home/kai/anaconda3/envs/decayangle/lib/python3.12/site-packages (from particle) '*

 * *            "(23.2.0)\\n'), (2, 'Requirement already satisfied: hepunits>=2.0.0 in "*

 * *            '/home/kai/anaconda […]*

```diff
@@ -1,25 +1,25 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 244,
+            "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Requirement already satisfied: particle in /home/kai/anaconda3/envs/decayangle_dev/lib/python3.11/site-packages (0.23.1)\n",
-                        "Requirement already satisfied: attrs>=19.2 in /home/kai/anaconda3/envs/decayangle_dev/lib/python3.11/site-packages (from particle) (23.2.0)\n",
-                        "Requirement already satisfied: hepunits>=2.0.0 in /home/kai/anaconda3/envs/decayangle_dev/lib/python3.11/site-packages (from particle) (2.3.3)\n",
-                        "Requirement already satisfied: typing-extensions>=4.5 in /home/kai/anaconda3/envs/decayangle_dev/lib/python3.11/site-packages (from particle) (4.10.0)\n",
+                        "Requirement already satisfied: particle in /home/kai/anaconda3/envs/decayangle/lib/python3.12/site-packages (0.23.1)\n",
+                        "Requirement already satisfied: attrs>=19.2 in /home/kai/anaconda3/envs/decayangle/lib/python3.12/site-packages (from particle) (23.2.0)\n",
+                        "Requirement already satisfied: hepunits>=2.0.0 in /home/kai/anaconda3/envs/decayangle/lib/python3.12/site-packages (from particle) (2.3.3)\n",
+                        "Requirement already satisfied: typing-extensions>=4.5 in /home/kai/anaconda3/envs/decayangle/lib/python3.12/site-packages (from particle) (4.10.0)\n",
                         "Note: you may need to restart the kernel to use updated packages.\n",
-                        "Requirement already satisfied: sympy in /home/kai/anaconda3/envs/decayangle_dev/lib/python3.11/site-packages (1.12)\n",
-                        "Requirement already satisfied: mpmath>=0.19 in /home/kai/anaconda3/envs/decayangle_dev/lib/python3.11/site-packages (from sympy) (1.3.0)\n",
+                        "Requirement already satisfied: sympy in /home/kai/anaconda3/envs/decayangle/lib/python3.12/site-packages (1.12)\n",
+                        "Requirement already satisfied: mpmath>=0.19 in /home/kai/anaconda3/envs/decayangle/lib/python3.12/site-packages (from sympy) (1.3.0)\n",
                         "Note: you may need to restart the kernel to use updated packages.\n"
                     ]
                 }
             ],
             "source": [
                 "%pip install particle\n",
                 "%pip install sympy"
@@ -33,24 +33,24 @@
                 "\n",
                 "For simplicity we will choose a simple\n",
                 "As you see, the isobars are allways isolated, meaning no isobar is the predecessor of another isobar. This makes the the full amplitude straightforward to calculate."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 245,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "( 0 -> ( (2, 3) -> 2, 3 ), 1 )\n",
-                        "( 0 -> ( (1, 3) -> 1, 3 ), 2 )\n",
-                        "( 0 -> ( (1, 2) -> 1, 2 ), 3 )\n"
+                        "Topology: ( 0 -> ( (2, 3) -> 2, 3 ), 1 )\n",
+                        "Topology: ( 0 -> ( (1, 3) -> 1, 3 ), 2 )\n",
+                        "Topology: ( 0 -> ( (1, 2) -> 1, 2 ), 3 )\n"
                     ]
                 }
             ],
             "source": [
                 "from decayangle.decay_topology import TopologyCollection, Node\n",
                 "import numpy as np\n",
                 "\n",
@@ -66,15 +66,15 @@
             "source": [
                 "First lets define some basic utility functions. This is not something you need to understand 100% on the first try.\n",
                 "What we do is set up the basic functional setup to be able to perform a three body analysis, which is the simplest case. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 246,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from typing import NamedTuple, Callable\n",
                 "from math import prod\n",
                 "from particle import Particle\n",
                 "\n",
@@ -209,15 +209,15 @@
                 "The particle porperites can be fetched directly from the PDG, with the help of the particles project.\n",
                 "\n",
                 "We go for a decay of $\\Lambda_b \\rightarrow \\Lambda_c^+ D^0 K^-$"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 247,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Particle 0: Lambda(b)0 spin: 1 helicities: [-1, 1]\n",
@@ -278,15 +278,15 @@
                 "\n",
                 "The $R(m,\\{\\lambda^{'}\\})$ is the lineshape of the resonance together with the couplings $H_{0 \\rightarrow (ij)\\, k}^{\\lambda_0, \\lambda_{(ij) - \\lambda_k}} \\cdot X(m,L) \\cdot H_{(ij) \\rightarrow i\\, j}^{\\lambda_{(ij)}, \\lambda_i^{'} - \\lambda_j^{'}}$. \n",
                 "The couplings $H$ are alled helicity couplings "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 248,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "{'D2800:resonanceDecay:L0.S2': LSCoupling(L=0, S=2, coupling=(1+0j)), 'D2800:resonanceDecay:L2.S0': LSCoupling(L=2, S=0, coupling=(1+0j)), 'D2800:resonanceDecay:L2.S2': LSCoupling(L=2, S=2, coupling=(1+0j)), 'D2800:resonanceDecay:L2.S4': LSCoupling(L=2, S=4, coupling=(1+0j))}\n"
@@ -318,32 +318,58 @@
             "metadata": {},
             "source": [
                 "Now we need to get the values for our rotations. For this we can simply iterate through all the possible decay topologys, the ```TopologyCollection``` Object generates for us."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 249,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "( 0 -> ( (2, 3) -> 2, 3 ), 1 ) {((2, 3), 1): (3.141592653589793, -1.1917396523105919)}\n",
-                        "( 0 -> ( (1, 3) -> 1, 3 ), 2 ) {((1, 3), 2): (5.951828758370096e-17, -0.23908244819164334)}\n",
-                        "( 0 -> ( (1, 2) -> 1, 2 ), 3 ) {((1, 2), 3): (5.041182631349134e-17, -0.26891484091188184)}\n"
+                        "Topology: ( 0 -> ( (2, 3) -> 2, 3 ), 1 ) {((2, 3), 1): HelicityAngles(theta_rf=-0.17491891382569247, psi_rf=-1.5707963267948966), (2, 3): HelicityAngles(theta_rf=-1.1917396523105919, psi_rf=3.141592653589793)}\n",
+                        "Topology: ( 0 -> ( (1, 3) -> 1, 3 ), 2 ) {((1, 3), 2): HelicityAngles(theta_rf=-3.136500881413798, psi_rf=-1.5707963267948966), (1, 3): HelicityAngles(theta_rf=-0.23908244819164334, psi_rf=5.951828758370096e-17)}\n",
+                        "Topology: ( 0 -> ( (1, 2) -> 1, 2 ), 3 ) {((1, 2), 3): HelicityAngles(theta_rf=-2.753684909312669, psi_rf=1.5707963267948966), (1, 2): HelicityAngles(theta_rf=-0.26891484091188184, psi_rf=5.041182631349134e-17)}\n"
                     ]
+                },
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "/home/kai/LHCb/decayangle/src/decayangle/kinematics.py:315: RuntimeWarning: invalid value encountered in divide\n",
+                        "  cosine_input = cb.where(abs(abs_mom) <= tol, 0, z_component(v) / abs_mom)\n"
+                    ]
+                },
+                {
+                    "data": {
+                        "text/plain": [
+                            "{((2, 3),\n",
+                            "  1): HelicityAngles(theta_rf=-0.17491891382569247, psi_rf=-1.5707963267948966),\n",
+                            " (2,\n",
+                            "  3): HelicityAngles(theta_rf=-1.1917396523105919, psi_rf=3.141592653589793)}"
+                        ]
+                    },
+                    "execution_count": 6,
+                    "metadata": {},
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
                 "for topology in tg.topologies:\n",
                 "        final_state_rotations = reference_topology.relative_wigner_angles(topology, momenta)\n",
                 "        isobars = topology.helicity_angles(momenta)\n",
-                "        print(topology, isobars)"
+                "        print(topology, isobars)\n",
+                "\n",
+                "topo = tg.topologies[0]\n",
+                "hel = topo.helicity_angles(momenta)\n",
+                "for k, v in hel.items():\n",
+                "    print(k, v)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "For each topology, we see, that we get exactly one isobar constellation. We also see, that of the two angles we compute, only one is non 0 (or $\\pi$).\n",
```

### Comparing `decayangle-1.0.1/src/decayangle/config.py` & `decayangle-1.0.2/src/decayangle/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from decayangle.backend import jax_backend, numpy_backend
 
 
 class _cfg:
     __state = {
         "backend": "numpy",
         "sorting": "value",
+        "numerical_safety_checks": True,
     }
     backend_map = {
         "jax": jax_backend,
         "numpy": numpy_backend,
     }
 
     @property
@@ -36,14 +37,24 @@
     def sorting(self, value):
         if value not in ["off", "value"]:
             raise ValueError(
                 f"Node sorting {value} not found"
                 "Only 'value' and 'off' are allowed for the time being"
             )
         self.__state["sorting"] = value
+    
+    @property
+    def numerical_safety_checks(self) -> bool:
+        return self.__state["numerical_safety_checks"]
+    
+    @numerical_safety_checks.setter
+    def numerical_safety_checks(self, value:bool):
+        if not isinstance(value, bool):
+            raise ValueError(f"Value {value} or type {type(value)} not understood for numerical_safety_checks")
+        self.__state["numerical_safety_checks"] = value
 
     def __value_sorting_fun(self, value):
         """Sort the value by lenght of the tuple first and then by absolute value of the integers
         Two tuples of the same length are sorted by the first element
 
         Returns:
             the sorted value
@@ -75,10 +86,14 @@
     def ordering_function(self, value):
         if self.sorting == "value":
             return self.__value_sorting_fun(value)
         if self.sorting == "off":
             return value
 
         raise ValueError(f"Node sorting {self.sorting} not found")
+    
+    def raise_if_safety_on(self, exception: Exception):
+        if self.numerical_safety_checks:
+            raise exception
 
 
 config = _cfg()
```

### Comparing `decayangle-1.0.1/src/decayangle/decay_topology.py` & `decayangle-1.0.2/src/decayangle/decay_topology.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,16 +278,18 @@
         It is expected, that the momenta are jax or numpy compatible and that the momenta are given in the rest frame of this node.
         """
         if not cb.allclose(
             akm.gamma(self.momentum(momenta)),
             cb.ones_like(akm.gamma(self.momentum(momenta))),
         ):
             gamma = akm.gamma(self.momentum(momenta))
-            raise ValueError(
-                f"gamma = {gamma} For the time being only particles at rest are supported as start nodes for a boost. This will be fixed in the future."
+            cfg.raise_if_safety_on( 
+                ValueError(
+                    f"gamma = {gamma} For the time being only particles at rest are supported as start nodes for a boost. This will be fixed in the future."
+                )
             )
         target = Node.get_node(target)
         zero = cb.zeros_like(akm.time_component(self.momentum(momenta)))
         one = cb.ones_like(zero)
         if self.value == target.value:
             return LorentzTrafo(zero, zero, zero, zero, zero, zero)
 
@@ -358,17 +360,19 @@
             theta_rf: The angle of the target momentum in the rest frame of this node
         """
         if not cb.allclose(
             akm.gamma(self.momentum(momenta)),
             cb.ones_like(akm.gamma(self.momentum(momenta))),
         ):
             gamma = akm.gamma(self.momentum(momenta))
-            raise ValueError(
-                f"gamma = {gamma} For the time being only particles at rest are supported as start nodes for a boost. This will be fixed in the future."
-            )
+            cfg.raise_if_safety_on(
+                ValueError(
+                    f"gamma = {gamma} For the time being only particles at rest are supported as start nodes for a boost. This will be fixed in the future."
+                )
+            ) 
         zero = cb.zeros_like(akm.time_component(self.momentum(momenta)))
         if self.value == target.value:
             return LorentzTrafo(zero, zero, zero, zero, zero, zero)
 
         if not target in self.daughters:
             raise ValueError(
                 f"Target node {target} is not a direct daughter of this node {self}"
```

### Comparing `decayangle-1.0.1/src/decayangle/kinematics.py` & `decayangle-1.0.2/src/decayangle/kinematics.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,16 +301,18 @@
     abs_mom = p(v)
     gma = w / m
 
     # gamma can be smaller than 1 due to numerical errors
     # for large deviations we will raise an exception
     gma = cb.where((abs(gma) < 1) & (abs(gma - 1) < 1e-14), 1, gma)
     if cb.any(gma < 1):
-        raise ValueError(
-            f"gamma is {gma}, which is less than 1. This is not a valid Lorentz transformation"
+        cfg.raise_if_safety_on(
+             ValueError(
+                f"gamma is {gma}, which is less than 1. This is not a valid Lorentz transformation"
+            )
         )
 
     xi = cb.arccosh(gma)
     phi = cb.arctan2(y_component(v), x_component(v))
 
     cosine_input = cb.where(abs(abs_mom) <= tol, 0, z_component(v) / abs_mom)
     theta = cb.arccos(cosine_input)
@@ -370,20 +372,22 @@
         cb.all(cb.isclose(m_original_2x2, -new_2x2, atol=3e-2), axis=-1), axis=-1
     )
 
     not_two_pi_shifted = cb.all(
         cb.all(cb.isclose(m_original_2x2, new_2x2, atol=3e-2), axis=-1), axis=-1
     )
     if cb.any(not_two_pi_shifted & two_pi_shifted):
-        raise ValueError(
-            f"The 2x2 matrix does not match the reconstruced parameters!"
-            f"This can happen due to numerical errors."
-            f"The original matrix is {m_original_2x2} and the reconstructed matrix is {new_2x2}"
-            f"Difference is {m_original_2x2 - new_2x2}"
-            f"Parameters are {phi}, {theta}, {xi}, {theta_rf}, {phi_rf}, {psi_rf}"
+        cfg.raise_if_safety_on(
+             ValueError(
+                f"The 2x2 matrix does not match the reconstruced parameters!"
+                f"This can happen due to numerical errors."
+                f"The original matrix is {m_original_2x2} and the reconstructed matrix is {new_2x2}"
+                f"Difference is {m_original_2x2 - new_2x2}"
+                f"Parameters are {phi}, {theta}, {xi}, {theta_rf}, {phi_rf}, {psi_rf}"
+            )
         )
 
     psi_rf = cb.where(two_pi_shifted, psi_rf + 2 * cb.pi, psi_rf)
     return phi, theta, xi, phi_rf, theta_rf, psi_rf
 
 
 def spatial_components(vector):
```

### Comparing `decayangle-1.0.1/src/decayangle/lorentz.py` & `decayangle-1.0.2/src/decayangle/lorentz.py`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.1/src/decayangle/numerics_helpers.py` & `decayangle-1.0.2/src/decayangle/numerics_helpers.py`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.1/tests/test_Nbody.py` & `decayangle-1.0.2/tests/test_Nbody.py`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.1/tests/test_decay.py` & `decayangle-1.0.2/tests/test_decay.py`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.1/tests/test_kinematics.py` & `decayangle-1.0.2/tests/test_kinematics.py`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.1/tests/test_lorentz.py` & `decayangle-1.0.2/tests/test_lorentz.py`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.1/tests/test_sorting.py` & `decayangle-1.0.2/tests/test_sorting.py`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.1/tests/test_topology.py` & `decayangle-1.0.2/tests/test_topology.py`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.1/LICENSE.md` & `decayangle-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.1/README.md` & `decayangle-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 # Welcome to the decayangle software Project
 
-<!-- [![PyPI - Version](https://img.shields.io/pypi/v/decayangle.svg)](https://pypi.org/project/decayangle)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/decayangle.svg)](https://pypi.org/project/decayangle) -->
-
-
-[![PyPI - Version](https://img.shields.io/pypi/v/decayangle.svg)](https://test.pypi.org/project/decayangle/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/decayangle.svg)](https://test.pypi.org/project/decayangle/)
+[![PyPI - Version](https://img.shields.io/pypi/v/decayangle.svg)](https://pypi.org/project/decayangle/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/decayangle.svg)](https://pypi.org/project/decayangle/)
+[![codecov](https://codecov.io/gh/KaiHabermann/decayangle/graph/badge.svg?token=KXBO8KEQ3V)](https://codecov.io/gh/KaiHabermann/decayangle)
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [Goal](#goal)
 - [Usage](#usage)
 - [On Topologies](#topologies)
 - [On Ordering](#ordering)
+- [Dealing with imperfect Data](#dealing-with-imperfect-data)
 - [Related projects](#related-projects)
 - [License](#license)
 
 ## Installation
 
 ```console
 pip install decayangle
@@ -204,14 +202,26 @@
 ```python
 from decayangle.config import config as cfg
 cfg.sorting = "off" # turns sorting off
 cfg.sorting = "value" # default sorting
 
 ```
 At this time only `"off"` and `"value"` are supported. For more sophisticated sorting algorithms the user has to write custom functions.
+
+## Dealing with imperfect Data
+
+When dealing with data, that has measurement uncertainty or other issues like backgrounds, it is sometimes easier to just process the data and remove all `inf` or `nan` values. 
+These values will usually trigger `ValueError` in `decayangle`. This behaviour can be disabled via the config as
+
+```python
+from decayangle.config import config as cfg
+cfg.numerical_safety_checks = False
+```
+Now `nan` and `inf` will be handeled only by `numpy` internally.
+
 ## Related projects
 
 Amplitude analyses dealing with non-zero spin of final-state particles have to implement wigner rotations in some way.
 However, there are a few projects addressing these rotations explicitly using analytic expressions in [DPD paper](https://inspirehep.net/literature/1758460), derived for three-body decays:
 - [ThreeBodyDecays.jl](https://github.com/mmikhasenko/ThreeBodyDecays.jl), 
 - [SymbolicThreeBodyDecays.jl](https://github.com/mmikhasenko/SymbolicThreeBodyDecays.jl),
 - [ComPWA/ampform-dpd](https://github.com/ComPWA/ampform-dpd).
```

### Comparing `decayangle-1.0.1/pyproject.toml` & `decayangle-1.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/decayangle"]
 
 [project]
 name = "decayangle"
 description = 'A tool for wigner rotations in n-body decays'
-version = '1.0.1'
+version = '1.0.2'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Kai Habermann", email = "kai.habermann@gmx.net" },
   { name = "Mikhail Mikhasenko", email = "mikhail.mikhasenko@cern.ch"},
@@ -57,12 +57,12 @@
 dependencies = [
   "coverage[toml]",
   "pytest",
   "pytest-cov",
 ]
 
 [tool.hatch.envs.test.scripts]
-cov = 'pytest --cov-report=term-missing --cov-config=pyproject.toml --cov --cov=tests'
+cov = 'pytest --cov-report=term-missing --cov-report=xml --cov-config=pyproject.toml --cov --cov=tests'
 
 [[tool.hatch.envs.test.matrix]]
-python = ["312", "38", "39", "311", "310"]
-version = ["1.0.1"]
+python = ["312", "311", "310", "39", "38"] 
+version = ["1.0.2"]
```

### Comparing `decayangle-1.0.1/PKG-INFO` & `decayangle-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: decayangle
-Version: 1.0.1
+Version: 1.0.2
 Summary: A tool for wigner rotations in n-body decays
 Project-URL: Documentation, https://kaihabermann.github.io/decayangle/
 Project-URL: Issues, https://github.com/KaiHabermann/decayangle/issues
 Project-URL: Source, https://github.com/KaiHabermann/decayangle
 Author-email: Kai Habermann <kai.habermann@gmx.net>, Mikhail Mikhasenko <mikhail.mikhasenko@cern.ch>
 License-Expression: MIT
 License-File: LICENSE.md
@@ -23,29 +23,27 @@
 Requires-Dist: networkx==3.0.0
 Requires-Dist: numpy
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
 # Welcome to the decayangle software Project
 
-<!-- [![PyPI - Version](https://img.shields.io/pypi/v/decayangle.svg)](https://pypi.org/project/decayangle)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/decayangle.svg)](https://pypi.org/project/decayangle) -->
-
-
-[![PyPI - Version](https://img.shields.io/pypi/v/decayangle.svg)](https://test.pypi.org/project/decayangle/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/decayangle.svg)](https://test.pypi.org/project/decayangle/)
+[![PyPI - Version](https://img.shields.io/pypi/v/decayangle.svg)](https://pypi.org/project/decayangle/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/decayangle.svg)](https://pypi.org/project/decayangle/)
+[![codecov](https://codecov.io/gh/KaiHabermann/decayangle/graph/badge.svg?token=KXBO8KEQ3V)](https://codecov.io/gh/KaiHabermann/decayangle)
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [Goal](#goal)
 - [Usage](#usage)
 - [On Topologies](#topologies)
 - [On Ordering](#ordering)
+- [Dealing with imperfect Data](#dealing-with-imperfect-data)
 - [Related projects](#related-projects)
 - [License](#license)
 
 ## Installation
 
 ```console
 pip install decayangle
@@ -231,14 +229,26 @@
 ```python
 from decayangle.config import config as cfg
 cfg.sorting = "off" # turns sorting off
 cfg.sorting = "value" # default sorting
 
 ```
 At this time only `"off"` and `"value"` are supported. For more sophisticated sorting algorithms the user has to write custom functions.
+
+## Dealing with imperfect Data
+
+When dealing with data, that has measurement uncertainty or other issues like backgrounds, it is sometimes easier to just process the data and remove all `inf` or `nan` values. 
+These values will usually trigger `ValueError` in `decayangle`. This behaviour can be disabled via the config as
+
+```python
+from decayangle.config import config as cfg
+cfg.numerical_safety_checks = False
+```
+Now `nan` and `inf` will be handeled only by `numpy` internally.
+
 ## Related projects
 
 Amplitude analyses dealing with non-zero spin of final-state particles have to implement wigner rotations in some way.
 However, there are a few projects addressing these rotations explicitly using analytic expressions in [DPD paper](https://inspirehep.net/literature/1758460), derived for three-body decays:
 - [ThreeBodyDecays.jl](https://github.com/mmikhasenko/ThreeBodyDecays.jl), 
 - [SymbolicThreeBodyDecays.jl](https://github.com/mmikhasenko/SymbolicThreeBodyDecays.jl),
 - [ComPWA/ampform-dpd](https://github.com/ComPWA/ampform-dpd).
```

