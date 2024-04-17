# Comparing `tmp/pcgym-0.1.2.tar.gz` & `tmp/pcgym-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcgym-0.1.2.tar", last modified: Wed Apr 17 10:50:15 2024, max compression
+gzip compressed data, was "pcgym-0.1.3.tar", last modified: Wed Apr 17 11:03:39 2024, max compression
```

## Comparing `pcgym-0.1.2.tar` & `pcgym-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 10:50:15.073233 pcgym-0.1.2/
--rw-rw-rw-   0        0        0     1094 2024-03-06 13:10:13.000000 pcgym-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     6543 2024-04-17 10:50:15.071234 pcgym-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3803 2024-04-16 14:40:43.000000 pcgym-0.1.2/README.md
--rw-rw-rw-   0        0        0     1309 2024-04-17 10:50:03.000000 pcgym-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       95 2024-04-02 11:41:57.000000 pcgym-0.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 10:50:15.073233 pcgym-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-17 10:50:15.034232 pcgym-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-17 10:50:15.064233 pcgym-0.1.2/src/pcgym/
--rw-rw-rw-   0        0        0      129 2024-04-17 10:46:31.000000 pcgym-0.1.2/src/pcgym/__init__.py
--rw-rw-rw-   0        0        0     7662 2024-04-17 10:20:21.000000 pcgym-0.1.2/src/pcgym/evaluation_metrics.py
--rw-rw-rw-   0        0        0     5303 2024-04-16 13:47:20.000000 pcgym-0.1.2/src/pcgym/integrator.py
--rw-rw-rw-   0        0        0    10621 2024-04-16 13:47:20.000000 pcgym-0.1.2/src/pcgym/model_classes.py
--rw-rw-rw-   0        0        0    10748 2024-04-16 13:47:20.000000 pcgym-0.1.2/src/pcgym/oracle.py
--rw-rw-rw-   0        0        0    16946 2024-04-17 10:47:07.000000 pcgym-0.1.2/src/pcgym/pcgym.py
--rw-rw-rw-   0        0        0    12943 2024-04-17 10:29:22.000000 pcgym-0.1.2/src/pcgym/policy_evaluation.py
--rw-rw-rw-   0        0        0     1637 2024-04-17 10:47:08.000000 pcgym-0.1.2/src/pcgym/test.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:50:15.070234 pcgym-0.1.2/src/pcgym.egg-info/
--rw-rw-rw-   0        0        0     6543 2024-04-17 10:50:15.000000 pcgym-0.1.2/src/pcgym.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      492 2024-04-17 10:50:15.000000 pcgym-0.1.2/src/pcgym.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 10:50:15.000000 pcgym-0.1.2/src/pcgym.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-04-17 10:50:15.000000 pcgym-0.1.2/src/pcgym.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-17 10:50:15.000000 pcgym-0.1.2/src/pcgym.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 11:03:39.223842 pcgym-0.1.3/
+-rw-rw-rw-   0        0        0     1094 2024-03-06 13:10:13.000000 pcgym-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     6543 2024-04-17 11:03:39.222842 pcgym-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3803 2024-04-16 14:40:43.000000 pcgym-0.1.3/README.md
+-rw-rw-rw-   0        0        0     1309 2024-04-17 11:03:33.000000 pcgym-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       95 2024-04-02 11:41:57.000000 pcgym-0.1.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 11:03:39.224842 pcgym-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 11:03:39.174774 pcgym-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 11:03:39.215841 pcgym-0.1.3/src/pcgym/
+-rw-rw-rw-   0        0        0       85 2024-04-17 10:53:11.000000 pcgym-0.1.3/src/pcgym/__init__.py
+-rw-rw-rw-   0        0        0     7662 2024-04-17 10:20:21.000000 pcgym-0.1.3/src/pcgym/evaluation_metrics.py
+-rw-rw-rw-   0        0        0     5303 2024-04-16 13:47:20.000000 pcgym-0.1.3/src/pcgym/integrator.py
+-rw-rw-rw-   0        0        0    10621 2024-04-16 13:47:20.000000 pcgym-0.1.3/src/pcgym/model_classes.py
+-rw-rw-rw-   0        0        0    10748 2024-04-16 13:47:20.000000 pcgym-0.1.3/src/pcgym/oracle.py
+-rw-rw-rw-   0        0        0    16961 2024-04-17 11:01:06.000000 pcgym-0.1.3/src/pcgym/pcgym.py
+-rw-rw-rw-   0        0        0    12943 2024-04-17 10:53:34.000000 pcgym-0.1.3/src/pcgym/policy_evaluation.py
+-rw-rw-rw-   0        0        0     1784 2024-04-17 11:01:20.000000 pcgym-0.1.3/src/pcgym/test.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:03:39.221842 pcgym-0.1.3/src/pcgym.egg-info/
+-rw-rw-rw-   0        0        0     6543 2024-04-17 11:03:39.000000 pcgym-0.1.3/src/pcgym.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      492 2024-04-17 11:03:39.000000 pcgym-0.1.3/src/pcgym.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 11:03:39.000000 pcgym-0.1.3/src/pcgym.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-04-17 11:03:39.000000 pcgym-0.1.3/src/pcgym.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-17 11:03:39.000000 pcgym-0.1.3/src/pcgym.egg-info/top_level.txt
```

### Comparing `pcgym-0.1.2/LICENSE` & `pcgym-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.2/PKG-INFO` & `pcgym-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcgym
-Version: 0.1.2
+Version: 0.1.3
 Summary: Reinforcement learning suite of process control problems.
 Author-email: Max Bloor <max.bloor@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Maximilian Bloor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pcgym Version: 0.1.2 Summary: Reinforcement
+Metadata-Version: 2.1 Name: pcgym Version: 0.1.3 Summary: Reinforcement
 learning suite of process control problems. Author-email: Max Bloor
 gmail.com> License: MIT License Copyright (c) 2024 Maximilian Bloor Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `pcgym-0.1.2/README.md` & `pcgym-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.2/pyproject.toml` & `pcgym-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pcgym"
-version = "0.1.2"
+version = "0.1.3"
 description = "Reinforcement learning suite of process control problems."
 requires-python = "~=3.10"
 license = { file = "LICENSE" }
 readme = "README.md"
 authors = [{ name = "Max Bloor", email = "max.bloor@gmail.com" }]
 keywords = [
   "reinforcement-learning",
```

### Comparing `pcgym-0.1.2/src/pcgym/evaluation_metrics.py` & `pcgym-0.1.3/src/pcgym/evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.2/src/pcgym/integrator.py` & `pcgym-0.1.3/src/pcgym/integrator.py`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.2/src/pcgym/model_classes.py` & `pcgym-0.1.3/src/pcgym/model_classes.py`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.2/src/pcgym/oracle.py` & `pcgym-0.1.3/src/pcgym/oracle.py`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.2/src/pcgym/pcgym.py` & `pcgym-0.1.3/src/pcgym/pcgym.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import numpy as np
 import gymnasium as gym
 from gymnasium import spaces
-from .model_classes import (
+from pcgym.model_classes import (
     cstr_ode,
     first_order_system_ode,
     multistage_extraction_ode,
     nonsmooth_control_ode,
 )
-from .Policy_Evaluation import policy_eval
-from .Integrator import integration_engine
+from pcgym.Policy_Evaluation import policy_eval
+from pcgym.Integrator import integration_engine
 import copy
 
 
 class make_env(gym.Env):
     """
     Class for RL-Gym Environment
     """
```

### Comparing `pcgym-0.1.2/src/pcgym/policy_evaluation.py` & `pcgym-0.1.3/src/pcgym/policy_evaluation.py`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.2/src/pcgym/test.py` & `pcgym-0.1.3/src/pcgym/test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,54 @@
-from pcgym import make_env
-import numpy as np
-from stable_baselines3 import PPO
 
-T = 26
-nsteps = 120
-SP = {
-    'Ca': [0.85 for i in range(int(nsteps/2))] + [0.9 for i in range(int(nsteps/2))],
-}
+from pcgym.policy_evaluation import policy_eval
+# from pcgym import make_env
+# import numpy as np
+# from stable_baselines3 import PPO
 
-disturbance = {'Caf': np.repeat([1, 1.05, 1], [nsteps//3, nsteps//3, nsteps//3])}
+# T = 26
+# nsteps = 120
+# SP = {
+#     'Ca': [0.85 for i in range(int(nsteps/2))] + [0.9 for i in range(int(nsteps/2))],
+# }
 
-#Continuous box action space
-action_space = {
-    'low': np.array([295]),
-    'high':np.array([302]) 
-}
-#Continuous box observation space
-observation_space = {
-    'low' : np.array([0.7,300,0.8]),
-    'high' : np.array([1,350,0.9])  
-}
-disturbance_space ={
-  'low': np.array([1]),
-  'high': np.array([1.05])
-}
-env_params = {
-    'N': nsteps, # Number of time steps
-    'tsim':T, # Simulation Time
-    'SP':SP, #Setpoint
-    'o_space' : observation_space, #Observation space
-    'a_space' : action_space, # Action space
-    'x0': np.array([0.8,330,0.8]), # Initial conditions (torch.tensor)
-    'model': 'cstr_ode', #Select the model
-    'normalise_a': True, #Normalise the actions
-    'normalise_o':True, #Normalise the states,
-    'r_scale': {'Ca':100},
-    'noise':True, #Add noise to the states
-    'integration_method': 'casadi', #Select the integration method
-    'noise_percentage':0, #Noise percentage
-    # 'disturbance_bounds':disturbance_space,
-    # 'disturbances': disturbance
-}
+# disturbance = {'Caf': np.repeat([1, 1.05, 1], [nsteps//3, nsteps//3, nsteps//3])}
 
-env = make_env(env_params)
-env.reset()
-env.step(0.1)
-model = PPO('MlpPolicy', env, verbose=1,learning_rate=1e-3)
-model.learn(total_timesteps=3e4)
-model.save('pse_track_ppo.zip')
-model.load('pse_track_ppo.zip')
-env.plot_rollout({'Random policy':model},1,oracle = True,dist_reward=True,MPC_params={'N':10,'R':0.001})
+# #Continuous box action space
+# action_space = {
+#     'low': np.array([295]),
+#     'high':np.array([302]) 
+# }
+# #Continuous box observation space
+# observation_space = {
+#     'low' : np.array([0.7,300,0.8]),
+#     'high' : np.array([1,350,0.9])  
+# }
+# disturbance_space ={
+#   'low': np.array([1]),
+#   'high': np.array([1.05])
+# }
+# env_params = {
+#     'N': nsteps, # Number of time steps
+#     'tsim':T, # Simulation Time
+#     'SP':SP, #Setpoint
+#     'o_space' : observation_space, #Observation space
+#     'a_space' : action_space, # Action space
+#     'x0': np.array([0.8,330,0.8]), # Initial conditions (torch.tensor)
+#     'model': 'cstr_ode', #Select the model
+#     'normalise_a': True, #Normalise the actions
+#     'normalise_o':True, #Normalise the states,
+#     'r_scale': {'Ca':100},
+#     'noise':True, #Add noise to the states
+#     'integration_method': 'casadi', #Select the integration method
+#     'noise_percentage':0, #Noise percentage
+#     # 'disturbance_bounds':disturbance_space,
+#     # 'disturbances': disturbance
+# }
+
+# env = make_env(env_params)
+# env.reset()
+# env.step(0.1)
+# model = PPO('MlpPolicy', env, verbose=1,learning_rate=1e-3)
+# model.learn(total_timesteps=3e4)
+# model.save('pse_track_ppo.zip')
+# model.load('pse_track_ppo.zip')
+# env.plot_rollout({'Random policy':model},1,oracle = True,dist_reward=True,MPC_params={'N':10,'R':0.001})
```

### Comparing `pcgym-0.1.2/src/pcgym.egg-info/PKG-INFO` & `pcgym-0.1.3/src/pcgym.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcgym
-Version: 0.1.2
+Version: 0.1.3
 Summary: Reinforcement learning suite of process control problems.
 Author-email: Max Bloor <max.bloor@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Maximilian Bloor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pcgym Version: 0.1.2 Summary: Reinforcement
+Metadata-Version: 2.1 Name: pcgym Version: 0.1.3 Summary: Reinforcement
 learning suite of process control problems. Author-email: Max Bloor
 gmail.com> License: MIT License Copyright (c) 2024 Maximilian Bloor Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

