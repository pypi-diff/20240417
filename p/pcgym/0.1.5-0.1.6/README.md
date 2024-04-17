# Comparing `tmp/pcgym-0.1.5.tar.gz` & `tmp/pcgym-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcgym-0.1.5.tar", last modified: Wed Apr 17 11:09:30 2024, max compression
+gzip compressed data, was "pcgym-0.1.6.tar", last modified: Wed Apr 17 11:29:36 2024, max compression
```

## Comparing `pcgym-0.1.5.tar` & `pcgym-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 11:09:30.026832 pcgym-0.1.5/
--rw-rw-rw-   0        0        0     1094 2024-03-06 13:10:13.000000 pcgym-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     6543 2024-04-17 11:09:30.025832 pcgym-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     3803 2024-04-16 14:40:43.000000 pcgym-0.1.5/README.md
--rw-rw-rw-   0        0        0     1309 2024-04-17 11:09:06.000000 pcgym-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       95 2024-04-02 11:41:57.000000 pcgym-0.1.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 11:09:30.026832 pcgym-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-17 11:09:29.986833 pcgym-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-17 11:09:30.017832 pcgym-0.1.5/src/pcgym/
--rw-rw-rw-   0        0        0       85 2024-04-17 11:08:47.000000 pcgym-0.1.5/src/pcgym/__init__.py
--rw-rw-rw-   0        0        0     7662 2024-04-17 10:20:21.000000 pcgym-0.1.5/src/pcgym/evaluation_metrics.py
--rw-rw-rw-   0        0        0     5303 2024-04-17 11:06:59.000000 pcgym-0.1.5/src/pcgym/integrator.py
--rw-rw-rw-   0        0        0    10621 2024-04-16 13:47:20.000000 pcgym-0.1.5/src/pcgym/model_classes.py
--rw-rw-rw-   0        0        0    10748 2024-04-16 13:47:20.000000 pcgym-0.1.5/src/pcgym/oracle.py
--rw-rw-rw-   0        0        0    16946 2024-04-17 11:08:42.000000 pcgym-0.1.5/src/pcgym/pcgym.py
--rw-rw-rw-   0        0        0    12943 2024-04-17 11:06:05.000000 pcgym-0.1.5/src/pcgym/policy_evaluation.py
--rw-rw-rw-   0        0        0     1784 2024-04-17 11:01:20.000000 pcgym-0.1.5/src/pcgym/test.py
-drwxrwxrwx   0        0        0        0 2024-04-17 11:09:30.024832 pcgym-0.1.5/src/pcgym.egg-info/
--rw-rw-rw-   0        0        0     6543 2024-04-17 11:09:29.000000 pcgym-0.1.5/src/pcgym.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      492 2024-04-17 11:09:29.000000 pcgym-0.1.5/src/pcgym.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 11:09:29.000000 pcgym-0.1.5/src/pcgym.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-04-17 11:09:29.000000 pcgym-0.1.5/src/pcgym.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-17 11:09:29.000000 pcgym-0.1.5/src/pcgym.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 11:29:36.463689 pcgym-0.1.6/
+-rw-rw-rw-   0        0        0     1094 2024-03-06 13:10:13.000000 pcgym-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     6543 2024-04-17 11:29:36.463689 pcgym-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3803 2024-04-16 14:40:43.000000 pcgym-0.1.6/README.md
+-rw-rw-rw-   0        0        0     1309 2024-04-17 11:29:01.000000 pcgym-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       95 2024-04-02 11:41:57.000000 pcgym-0.1.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 11:29:36.464688 pcgym-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 11:29:36.422689 pcgym-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 11:29:36.454725 pcgym-0.1.6/src/pcgym/
+-rw-rw-rw-   0        0        0       85 2024-04-17 11:08:47.000000 pcgym-0.1.6/src/pcgym/__init__.py
+-rw-rw-rw-   0        0        0     7662 2024-04-17 10:20:21.000000 pcgym-0.1.6/src/pcgym/evaluation_metrics.py
+-rw-rw-rw-   0        0        0     5303 2024-04-17 11:06:59.000000 pcgym-0.1.6/src/pcgym/integrator.py
+-rw-rw-rw-   0        0        0    10621 2024-04-16 13:47:20.000000 pcgym-0.1.6/src/pcgym/model_classes.py
+-rw-rw-rw-   0        0        0    10748 2024-04-16 13:47:20.000000 pcgym-0.1.6/src/pcgym/oracle.py
+-rw-rw-rw-   0        0        0    16972 2024-04-17 11:29:18.000000 pcgym-0.1.6/src/pcgym/pcgym.py
+-rw-rw-rw-   0        0        0    12943 2024-04-17 11:28:56.000000 pcgym-0.1.6/src/pcgym/policy_evaluation.py
+-rw-rw-rw-   0        0        0     1551 2024-04-17 11:25:45.000000 pcgym-0.1.6/src/pcgym/test.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:29:36.461689 pcgym-0.1.6/src/pcgym.egg-info/
+-rw-rw-rw-   0        0        0     6543 2024-04-17 11:29:36.000000 pcgym-0.1.6/src/pcgym.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      492 2024-04-17 11:29:36.000000 pcgym-0.1.6/src/pcgym.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 11:29:36.000000 pcgym-0.1.6/src/pcgym.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-04-17 11:29:36.000000 pcgym-0.1.6/src/pcgym.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-17 11:29:36.000000 pcgym-0.1.6/src/pcgym.egg-info/top_level.txt
```

### Comparing `pcgym-0.1.5/LICENSE` & `pcgym-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.5/PKG-INFO` & `pcgym-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcgym
-Version: 0.1.5
+Version: 0.1.6
 Summary: Reinforcement learning suite of process control problems.
 Author-email: Max Bloor <max.bloor@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Maximilian Bloor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pcgym Version: 0.1.5 Summary: Reinforcement
+Metadata-Version: 2.1 Name: pcgym Version: 0.1.6 Summary: Reinforcement
 learning suite of process control problems. Author-email: Max Bloor
 gmail.com> License: MIT License Copyright (c) 2024 Maximilian Bloor Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `pcgym-0.1.5/README.md` & `pcgym-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.5/pyproject.toml` & `pcgym-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pcgym"
-version = "0.1.5"
+version = "0.1.6"
 description = "Reinforcement learning suite of process control problems."
 requires-python = "~=3.10"
 license = { file = "LICENSE" }
 readme = "README.md"
 authors = [{ name = "Max Bloor", email = "max.bloor@gmail.com" }]
 keywords = [
   "reinforcement-learning",
```

### Comparing `pcgym-0.1.5/src/pcgym/evaluation_metrics.py` & `pcgym-0.1.6/src/pcgym/evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.5/src/pcgym/integrator.py` & `pcgym-0.1.6/src/pcgym/integrator.py`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.5/src/pcgym/model_classes.py` & `pcgym-0.1.6/src/pcgym/model_classes.py`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.5/src/pcgym/oracle.py` & `pcgym-0.1.6/src/pcgym/oracle.py`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.5/src/pcgym/pcgym.py` & `pcgym-0.1.6/src/pcgym/pcgym.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,15 @@
         rew = self.reward_fn(self.state, constraint_violated)
 
         # For each set point, if it exists, append its value at the current time step to the list
         SP_t = []
         for k in self.SP.keys():
             if k in self.SP:
                 SP_t.append(self.SP[k][self.t])
-        self.state[self.Nx_oracle :] = np.array(SP_t)
+        self.state[self.Nx_oracle:self.Nx_oracle+len(self.SP)] = np.array(SP_t)
         # Update timestep
         self.t += 1
 
         if self.t == self.N:
             self.done = True
 
         # add noise to state
```

### Comparing `pcgym-0.1.5/src/pcgym/policy_evaluation.py` & `pcgym-0.1.6/src/pcgym/policy_evaluation.py`

 * *Files identical despite different names*

### Comparing `pcgym-0.1.5/src/pcgym/test.py` & `pcgym-0.1.6/src/pcgym/test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,50 @@
 
-from pcgym.policy_evaluation import policy_eval
-# from pcgym import make_env
-# import numpy as np
-# from stable_baselines3 import PPO
+from pcgym import make_env
+import numpy as np
+from stable_baselines3 import PPO
 
-# T = 26
-# nsteps = 120
-# SP = {
-#     'Ca': [0.85 for i in range(int(nsteps/2))] + [0.9 for i in range(int(nsteps/2))],
-# }
+nsteps = 150
+T = 3
+SP = {
+    'X1': [0 for i in range(int(nsteps))],
+    #'X2': [0 for i in range(int(nsteps))] 
+}
 
-# disturbance = {'Caf': np.repeat([1, 1.05, 1], [nsteps//3, nsteps//3, nsteps//3])}
+#Continuous box action space
+action_space = {
+    'low': np.array([-1]),
+    'high':np.array([1]) 
+}
+#Continuous box observation space
+observation_space = {
+    'low' : np.array([-1,-1,-1]),
+    'high' : np.array([1,1,1])  
+}
 
-# #Continuous box action space
-# action_space = {
-#     'low': np.array([295]),
-#     'high':np.array([302]) 
-# }
-# #Continuous box observation space
-# observation_space = {
-#     'low' : np.array([0.7,300,0.8]),
-#     'high' : np.array([1,350,0.9])  
-# }
-# disturbance_space ={
-#   'low': np.array([1]),
-#   'high': np.array([1.05])
-# }
-# env_params = {
-#     'N': nsteps, # Number of time steps
-#     'tsim':T, # Simulation Time
-#     'SP':SP, #Setpoint
-#     'o_space' : observation_space, #Observation space
-#     'a_space' : action_space, # Action space
-#     'x0': np.array([0.8,330,0.8]), # Initial conditions (torch.tensor)
-#     'model': 'cstr_ode', #Select the model
-#     'normalise_a': True, #Normalise the actions
-#     'normalise_o':True, #Normalise the states,
-#     'r_scale': {'Ca':100},
-#     'noise':True, #Add noise to the states
-#     'integration_method': 'casadi', #Select the integration method
-#     'noise_percentage':0, #Noise percentage
-#     # 'disturbance_bounds':disturbance_space,
-#     # 'disturbances': disturbance
-# }
+r_scale ={
+    'X1': 100,
+}
+env_params = {
+    'N': nsteps, # Number of time steps
+    'tsim':T, # Simulation Time
+    'SP':SP, #Setpoint
+    'o_space' : observation_space, #Observation space
+    'a_space' : action_space, # Action space
+    'x0': np.array([1,-1,0.]), # Initial conditions (torch.tensor)
+    'model': 'nonsmooth_control_ode', #Select the model
+    'r_scale': r_scale, #Scale the L1 norm used for reward (|x-x_sp|*r_scale)
+    'normalise_a': False, #Normalise the actions
+    'normalise_o':False, #Normalise the states,
+    'noise':False, #Add noise to the states
+    'integration_method': 'casadi', #Select the integration method
+    'noise_percentage':0 #Noise percentage
+}
+env = make_env(env_params)
+# Load the saved policy
+bang_pol = PPO('MlpPolicy', env, verbose=1,learning_rate=1e-3)
+bang_pol.learn(total_timesteps=1e4)
+bang_pol.save('pse_track_ppo.zip')
+bang_pol.load('pse_track_ppo.zip')
 
-# env = make_env(env_params)
-# env.reset()
-# env.step(0.1)
-# model = PPO('MlpPolicy', env, verbose=1,learning_rate=1e-3)
-# model.learn(total_timesteps=3e4)
-# model.save('pse_track_ppo.zip')
-# model.load('pse_track_ppo.zip')
-# env.plot_rollout({'Random policy':model},1,oracle = True,dist_reward=True,MPC_params={'N':10,'R':0.001})
+# Evaluate the policy and plot the rollout
+evaluator, data = env.plot_rollout({'SAC': bang_pol}, reps=1, oracle=True, dist_reward=True, MPC_params={'N': 10, 'R': 0})
```

### Comparing `pcgym-0.1.5/src/pcgym.egg-info/PKG-INFO` & `pcgym-0.1.6/src/pcgym.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcgym
-Version: 0.1.5
+Version: 0.1.6
 Summary: Reinforcement learning suite of process control problems.
 Author-email: Max Bloor <max.bloor@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Maximilian Bloor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pcgym Version: 0.1.5 Summary: Reinforcement
+Metadata-Version: 2.1 Name: pcgym Version: 0.1.6 Summary: Reinforcement
 learning suite of process control problems. Author-email: Max Bloor
 gmail.com> License: MIT License Copyright (c) 2024 Maximilian Bloor Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

