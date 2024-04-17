# Comparing `tmp/pcgym-0.1.0.tar.gz` & `tmp/pcgym-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcgym-0.1.0.tar", last modified: Wed Apr 17 10:20:59 2024, max compression
+gzip compressed data, was "pcgym-0.1.1.tar", last modified: Wed Apr 17 10:40:35 2024, max compression
```

## Comparing `pcgym-0.1.0.tar` & `pcgym-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 10:20:59.398195 pcgym-0.1.0/
--rw-rw-rw-   0        0        0     1094 2024-03-06 13:10:13.000000 pcgym-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     6543 2024-04-17 10:20:59.397195 pcgym-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3803 2024-04-16 14:40:43.000000 pcgym-0.1.0/README.md
--rw-rw-rw-   0        0        0     1309 2024-04-17 10:20:04.000000 pcgym-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       95 2024-04-02 11:41:57.000000 pcgym-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 10:20:59.398195 pcgym-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-17 10:20:59.355195 pcgym-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-17 10:20:59.388195 pcgym-0.1.0/src/pcgym/
--rw-rw-rw-   0        0        0       85 2024-04-16 13:47:20.000000 pcgym-0.1.0/src/pcgym/__init__.py
--rw-rw-rw-   0        0        0     7662 2024-04-17 10:20:21.000000 pcgym-0.1.0/src/pcgym/evaluation_metrics.py
--rw-rw-rw-   0        0        0     5303 2024-04-16 13:47:20.000000 pcgym-0.1.0/src/pcgym/integrator.py
--rw-rw-rw-   0        0        0    10621 2024-04-16 13:47:20.000000 pcgym-0.1.0/src/pcgym/model_classes.py
--rw-rw-rw-   0        0        0    10748 2024-04-16 13:47:20.000000 pcgym-0.1.0/src/pcgym/oracle.py
--rw-rw-rw-   0        0        0    17070 2024-04-17 10:20:21.000000 pcgym-0.1.0/src/pcgym/pcgym.py
--rw-rw-rw-   0        0        0    12959 2024-04-17 10:20:21.000000 pcgym-0.1.0/src/pcgym/policy_evaluation.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:20:59.396198 pcgym-0.1.0/src/pcgym.egg-info/
--rw-rw-rw-   0        0        0     6543 2024-04-17 10:20:59.000000 pcgym-0.1.0/src/pcgym.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      474 2024-04-17 10:20:59.000000 pcgym-0.1.0/src/pcgym.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 10:20:59.000000 pcgym-0.1.0/src/pcgym.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-04-17 10:20:59.000000 pcgym-0.1.0/src/pcgym.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-17 10:20:59.000000 pcgym-0.1.0/src/pcgym.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 10:40:35.742610 pcgym-0.1.1/
+-rw-rw-rw-   0        0        0     1094 2024-03-06 13:10:13.000000 pcgym-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     6543 2024-04-17 10:40:35.741610 pcgym-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3803 2024-04-16 14:40:43.000000 pcgym-0.1.1/README.md
+-rw-rw-rw-   0        0        0     1309 2024-04-17 10:40:27.000000 pcgym-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       95 2024-04-02 11:41:57.000000 pcgym-0.1.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 10:40:35.742610 pcgym-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 10:40:35.698610 pcgym-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 10:40:35.733648 pcgym-0.1.1/src/pcgym/
+-rw-rw-rw-   0        0        0       85 2024-04-17 10:29:24.000000 pcgym-0.1.1/src/pcgym/__init__.py
+-rw-rw-rw-   0        0        0     7662 2024-04-17 10:20:21.000000 pcgym-0.1.1/src/pcgym/evaluation_metrics.py
+-rw-rw-rw-   0        0        0     5303 2024-04-16 13:47:20.000000 pcgym-0.1.1/src/pcgym/integrator.py
+-rw-rw-rw-   0        0        0    10621 2024-04-16 13:47:20.000000 pcgym-0.1.1/src/pcgym/model_classes.py
+-rw-rw-rw-   0        0        0    10748 2024-04-16 13:47:20.000000 pcgym-0.1.1/src/pcgym/oracle.py
+-rw-rw-rw-   0        0        0    16946 2024-04-17 10:34:51.000000 pcgym-0.1.1/src/pcgym/pcgym.py
+-rw-rw-rw-   0        0        0    12943 2024-04-17 10:29:22.000000 pcgym-0.1.1/src/pcgym/policy_evaluation.py
+-rw-rw-rw-   0        0        0     1637 2024-04-17 10:31:44.000000 pcgym-0.1.1/src/pcgym/test.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:40:35.739611 pcgym-0.1.1/src/pcgym.egg-info/
+-rw-rw-rw-   0        0        0     6543 2024-04-17 10:40:35.000000 pcgym-0.1.1/src/pcgym.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      492 2024-04-17 10:40:35.000000 pcgym-0.1.1/src/pcgym.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 10:40:35.000000 pcgym-0.1.1/src/pcgym.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-04-17 10:40:35.000000 pcgym-0.1.1/src/pcgym.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-17 10:40:35.000000 pcgym-0.1.1/src/pcgym.egg-info/top_level.txt
```

### Comparing `pcgym-0.1.0/LICENSE` & `pcgym-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.0/PKG-INFO` & `pcgym-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcgym
-Version: 0.1.0
+Version: 0.1.1
 Summary: Reinforcement learning suite of process control problems.
 Author-email: Max Bloor <max.bloor@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Maximilian Bloor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pcgym Version: 0.1.0 Summary: Reinforcement
+Metadata-Version: 2.1 Name: pcgym Version: 0.1.1 Summary: Reinforcement
 learning suite of process control problems. Author-email: Max Bloor
 gmail.com> License: MIT License Copyright (c) 2024 Maximilian Bloor Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `pcgym-0.1.0/README.md` & `pcgym-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.0/pyproject.toml` & `pcgym-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pcgym"
-version = "0.1.0"
+version = "0.1.1"
 description = "Reinforcement learning suite of process control problems."
 requires-python = "~=3.10"
 license = { file = "LICENSE" }
 readme = "README.md"
 authors = [{ name = "Max Bloor", email = "max.bloor@gmail.com" }]
 keywords = [
   "reinforcement-learning",
```

### Comparing `pcgym-0.1.0/src/pcgym/evaluation_metrics.py` & `pcgym-0.1.1/src/pcgym/evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.0/src/pcgym/integrator.py` & `pcgym-0.1.1/src/pcgym/integrator.py`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.0/src/pcgym/model_classes.py` & `pcgym-0.1.1/src/pcgym/model_classes.py`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.0/src/pcgym/oracle.py` & `pcgym-0.1.1/src/pcgym/oracle.py`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.0/src/pcgym/pcgym.py` & `pcgym-0.1.1/src/pcgym/pcgym.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import numpy as np
 import gymnasium as gym
 from gymnasium import spaces
-from pcgym.model_classes import (
+from .model_classes import (
     cstr_ode,
     first_order_system_ode,
     multistage_extraction_ode,
     nonsmooth_control_ode,
 )
-from pcgym.Policy_Evaluation import policy_eval
-from pcgym.Integrator import integration_engine
+from .Policy_Evaluation import policy_eval
+from .Integrator import integration_engine
 import copy
 
 
 class make_env(gym.Env):
     """
     Class for RL-Gym Environment
     """
@@ -46,22 +46,19 @@
         self.tsim = env_params["tsim"]
         self.x0 = env_params["x0"]
         # Initial setup for observation space based on user-defined bounds
         base_obs_low = env_params["o_space"]["low"]
         base_obs_high = env_params["o_space"]["high"]
         self.observation_space_base = spaces.Box(low=base_obs_low, high=base_obs_high)
 
-        if self.normalise_o:
-            self.observation_space = spaces.Box(
-                low=np.array([-1] * base_obs_low.shape[0]),
-                high=np.array([1] * base_obs_high.shape[0]),
-            )
+        if self.normalise_o: 
+            self.observation_space = spaces.Box(low=np.array([-1]*base_obs_low.shape[0]), high=np.array([1]*base_obs_high.shape[0]))
         else:
             self.observation_space = spaces.Box(low=base_obs_low, high=base_obs_high)
-
+        
         try:
             self.integration_method = env_params["integration_method"]
         except Exception:
             self.integration_method = "casadi"
 
         self.dt = self.tsim / self.N
         self.done = False
@@ -137,22 +134,19 @@
             extended_obs_low = np.concatenate((base_obs_low, disturbance_low))
             extended_obs_high = np.concatenate((base_obs_high, disturbance_high))
             # Define the extended observation space
             self.observation_space_base = spaces.Box(
                 low=extended_obs_low, high=extended_obs_high, dtype=np.float32
             )
             if self.normalise_o:
-                self.observation_space = spaces.Box(
-                    low=np.array([-1] * extended_obs_low.shape[0]),
-                    high=np.array([1] * extended_obs_high.shape[0]),
-                )
+                self.observation_space = spaces.Box(low=np.array([-1]*extended_obs_low.shape[0]), high=np.array([1]*extended_obs_high.shape[0]))
             else:
                 self.observation_space = spaces.Box(
-                    low=extended_obs_low, high=extended_obs_high, dtype=np.float32
-                )
+                low=extended_obs_low, high=extended_obs_high, dtype=np.float32
+            )
 
     def reset(self, seed=None, **kwargs):  # Accept arbitrary keyword arguments
         """
         Resets the state of the system
 
         Returns the state of the system
         """
@@ -212,14 +206,15 @@
         # Create control vector
         uk = np.zeros(self.Nu)
         if self.normalise_a is True:
             action = (action + 1) * (
                 self.env_params["a_space"]["high"] - self.env_params["a_space"]["low"]
             ) / 2 + self.env_params["a_space"]["low"]
 
+
         # Add disturbance to control vector
         if self.disturbance_active:
             uk[: self.Nu - len(self.model.info()["disturbances"])] = (
                 action  # Add action to control vector
             )
             disturbance_values = []
             disturbance_values_state = []
@@ -298,15 +293,15 @@
         Inputs:
             state - current state of the system
             c_violated - boolean indicating if constraint is violated
         Outputs:
             r - reward for current timestep
 
         """
-
+        
         r = 0.0
 
         for k in self.SP:
             i = self.model.info()["states"].index(k)
             r_scale = self.env_params.get("r_scale", {})
             r += (-((state[i] - np.array(self.SP[k][self.t])) ** 2)) * r_scale.get(k, 1)
             if self.r_penalty and c_violated:
```

### Comparing `pcgym-0.1.0/src/pcgym/policy_evaluation.py` & `pcgym-0.1.1/src/pcgym/policy_evaluation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Policy Evaluation Class for pc-gym
 import numpy as np
 import matplotlib.pyplot as plt
-from oracle import oracle
+from .oracle import oracle
 
 
 class policy_eval:
     """
     Policy Evaluation Class
 
     Inputs: Environment, policy and number of policy repitions
@@ -66,16 +66,15 @@
             o, r, term, trunc, info = self.env.step(a)
 
             actions[:, i] = (a + 1) * (
                 self.env.env_params["a_space"]["high"]
                 - self.env.env_params["a_space"]["low"]
             ) / 2 + self.env.env_params["a_space"]["low"]
             s_rollout[:, i + 1] = (o + 1) * (
-                self.env.observation_space_base.high
-                - self.env.observation_space_base.low
+                self.env.observation_space_base.high - self.env.observation_space_base.low
             ) / 2 + self.env.observation_space_base.low
 
             total_reward += r
 
         if self.env.constraint_active:
             cons_info = info["cons_info"]
         else:
```

### Comparing `pcgym-0.1.0/src/pcgym.egg-info/PKG-INFO` & `pcgym-0.1.1/src/pcgym.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcgym
-Version: 0.1.0
+Version: 0.1.1
 Summary: Reinforcement learning suite of process control problems.
 Author-email: Max Bloor <max.bloor@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Maximilian Bloor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pcgym Version: 0.1.0 Summary: Reinforcement
+Metadata-Version: 2.1 Name: pcgym Version: 0.1.1 Summary: Reinforcement
 learning suite of process control problems. Author-email: Max Bloor
 gmail.com> License: MIT License Copyright (c) 2024 Maximilian Bloor Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

