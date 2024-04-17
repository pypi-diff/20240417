# Comparing `tmp/pcgym-0.0.9.tar.gz` & `tmp/pcgym-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcgym-0.0.9.tar", last modified: Fri Apr 12 12:06:28 2024, max compression
+gzip compressed data, was "pcgym-0.1.0.tar", last modified: Wed Apr 17 10:20:59 2024, max compression
```

## Comparing `pcgym-0.0.9.tar` & `pcgym-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 12:06:28.375646 pcgym-0.0.9/
--rw-rw-rw-   0        0        0     1094 2024-03-06 13:10:13.000000 pcgym-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     6056 2024-04-12 12:06:28.374647 pcgym-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     3316 2024-04-02 11:41:27.000000 pcgym-0.0.9/README.md
--rw-rw-rw-   0        0        0     1309 2024-04-12 12:06:03.000000 pcgym-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       95 2024-04-02 11:41:57.000000 pcgym-0.0.9/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 12:06:28.375646 pcgym-0.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 12:06:28.317783 pcgym-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 12:06:28.344765 pcgym-0.0.9/src/pcgym/
--rw-rw-rw-   0        0        0       93 2024-04-12 12:03:39.000000 pcgym-0.0.9/src/pcgym/__init__.py
--rw-rw-rw-   0        0        0     7262 2024-04-12 11:15:27.000000 pcgym-0.0.9/src/pcgym/evaluation_metrics.py
--rw-rw-rw-   0        0        0     5142 2024-04-12 11:17:30.000000 pcgym-0.0.9/src/pcgym/integrator.py
--rw-rw-rw-   0        0        0     8666 2024-04-12 11:20:55.000000 pcgym-0.0.9/src/pcgym/model_classes.py
--rw-rw-rw-   0        0        0     8782 2024-04-12 11:18:31.000000 pcgym-0.0.9/src/pcgym/oracle.py
--rw-rw-rw-   0        0        0    15378 2024-04-12 11:27:09.000000 pcgym-0.0.9/src/pcgym/pcgym.py
--rw-rw-rw-   0        0        0    10657 2024-04-12 11:25:21.000000 pcgym-0.0.9/src/pcgym/policy_evaluation.py
-drwxrwxrwx   0        0        0        0 2024-04-12 12:06:28.373645 pcgym-0.0.9/src/pcgym.egg-info/
--rw-rw-rw-   0        0        0     6056 2024-04-12 12:06:28.000000 pcgym-0.0.9/src/pcgym.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      474 2024-04-12 12:06:28.000000 pcgym-0.0.9/src/pcgym.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 12:06:28.000000 pcgym-0.0.9/src/pcgym.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-04-12 12:06:28.000000 pcgym-0.0.9/src/pcgym.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-12 12:06:28.000000 pcgym-0.0.9/src/pcgym.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 10:20:59.398195 pcgym-0.1.0/
+-rw-rw-rw-   0        0        0     1094 2024-03-06 13:10:13.000000 pcgym-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     6543 2024-04-17 10:20:59.397195 pcgym-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3803 2024-04-16 14:40:43.000000 pcgym-0.1.0/README.md
+-rw-rw-rw-   0        0        0     1309 2024-04-17 10:20:04.000000 pcgym-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       95 2024-04-02 11:41:57.000000 pcgym-0.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 10:20:59.398195 pcgym-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 10:20:59.355195 pcgym-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 10:20:59.388195 pcgym-0.1.0/src/pcgym/
+-rw-rw-rw-   0        0        0       85 2024-04-16 13:47:20.000000 pcgym-0.1.0/src/pcgym/__init__.py
+-rw-rw-rw-   0        0        0     7662 2024-04-17 10:20:21.000000 pcgym-0.1.0/src/pcgym/evaluation_metrics.py
+-rw-rw-rw-   0        0        0     5303 2024-04-16 13:47:20.000000 pcgym-0.1.0/src/pcgym/integrator.py
+-rw-rw-rw-   0        0        0    10621 2024-04-16 13:47:20.000000 pcgym-0.1.0/src/pcgym/model_classes.py
+-rw-rw-rw-   0        0        0    10748 2024-04-16 13:47:20.000000 pcgym-0.1.0/src/pcgym/oracle.py
+-rw-rw-rw-   0        0        0    17070 2024-04-17 10:20:21.000000 pcgym-0.1.0/src/pcgym/pcgym.py
+-rw-rw-rw-   0        0        0    12959 2024-04-17 10:20:21.000000 pcgym-0.1.0/src/pcgym/policy_evaluation.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:20:59.396198 pcgym-0.1.0/src/pcgym.egg-info/
+-rw-rw-rw-   0        0        0     6543 2024-04-17 10:20:59.000000 pcgym-0.1.0/src/pcgym.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2024-04-17 10:20:59.000000 pcgym-0.1.0/src/pcgym.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 10:20:59.000000 pcgym-0.1.0/src/pcgym.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-04-17 10:20:59.000000 pcgym-0.1.0/src/pcgym.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-17 10:20:59.000000 pcgym-0.1.0/src/pcgym.egg-info/top_level.txt
```

### Comparing `pcgym-0.0.9/LICENSE` & `pcgym-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pcgym-0.0.9/PKG-INFO` & `pcgym-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcgym
-Version: 0.0.9
+Version: 0.1.0
 Summary: Reinforcement learning suite of process control problems.
 Author-email: Max Bloor <max.bloor@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Maximilian Bloor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -63,14 +63,16 @@
   <b>Reinforcement learning environments for process control </b><br>
 </h1>
 <p align="center">
       <a href="https://www.python.org/doc/versions/">
         <img src="https://img.shields.io/badge/python-3.10-blue.svg" /></a>  
       <a href="https://opensource.org/license/mit">
         <img src="https://img.shields.io/badge/license-MIT-orange" /></a>
+      <a href="https://github.com/astral-sh/ruff">
+        <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json" /></a>
 </p>
 
 
 ## Quick start ⚡
 Setup a CSTR environment with a setpoint change
 
 ```python 
@@ -129,22 +131,23 @@
 ## Implemented Process Control Environments 🎛️
 
 |          Environment          | Reference | Source | Documentation |
 |:-----------------------------:|:---------:|:------:|---------------|
 |              CSTR             | [Hedengren, 2022](https://github.com/APMonitor/pdc/blob/master/CSTR_Control.ipynb)     | [Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/model_classes.py)      |               |
 |       First Order Sytem       |      N/A  | [Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/model_classes.py)        |               |
 | Multistage Extraction Column  |  [Ingham et al, 2007 (pg 471)](https://onlinelibrary.wiley.com/doi/book/10.1002/9783527614219)         | [Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/model_classes.py)        |               |
+| Nonsmooth Control|[Lim,1969](https://pubs.acs.org/doi/epdf/10.1021/i260031a007)|[Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/model_classes.py) ||
 
 
  
 ## Citing `pc-gym`
 If you use `pc-gym` in your research, please cite using the following 
 ```
 @software{pcgym2024,
-  author = {Max Bloor and ...},
+  author = {Max Bloor and and Jose Neto and Ilya Sandoval and Max Mowbray and Akhil Ahmed and Mehmet Mercangoz and Calvin Tsay and Antonio Del Rio-Chanona},
   title = {{pc-gym}: Reinforcement Learning Envionments for Process Control},
   url = {https://github.com/MaximilianB2/pc-gym},
   version = {0.0.4},
   year = {2024},
 }
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pcgym Version: 0.0.9 Summary: Reinforcement
+Metadata-Version: 2.1 Name: pcgym Version: 0.1.0 Summary: Reinforcement
 learning suite of process control problems. Author-email: Max Bloor
 gmail.com> License: MIT License Copyright (c) 2024 Maximilian Bloor Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -33,15 +33,16 @@
 "optional" Requires-Dist: stable-baselines3; extra == "optional" Requires-Dist:
 mkdocs-material; extra == "optional"
 ************ _[[_hh_tt_tt_pp_ss_::_//_//_gg_ii_tt_hh_uu_bb_.._cc_oo_mm_//_MM_aa_xx_ii_mm_ii_ll_ii_aa_nn_BB_22_//_pp_cc_--_gg_yy_mm_//_bb_ll_oo_bb_//_mm_aa_ii_nn_//_dd_oo_cc_ss_//_ii_mm_gg_//_pp_cc_--_gg_yy_mm_--_bb_ll_uu_ee_--
                                     _AA_ii_.._pp_nn_gg_]]
             RReeiinnffoorrcceemmeenntt lleeaarrnniinngg eennvviirroonnmmeennttss ffoorr pprroocceessss ccoonnttrrooll
                                      ************
   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-_3_._1_0_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-                           _b_a_d_g_e_/_l_i_c_e_n_s_e_-_M_I_T_-_o_r_a_n_g_e_]
+    _b_a_d_g_e_/_l_i_c_e_n_s_e_-_M_I_T_-_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_e_n_d_p_o_i_n_t_?_u_r_l_=_h_t_t_p_s_:_/_/
+      _r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_a_s_t_r_a_l_-_s_h_/_r_u_f_f_/_m_a_i_n_/_a_s_s_e_t_s_/_b_a_d_g_e_/_v_2_._j_s_o_n_]
 ## Quick start â¡ Setup a CSTR environment with a setpoint change ```python
 import pcgym # Simulation variables nsteps = 100 T = 25 # Setpoint SP = {'Ca':
 [0.85 for i in range(int(nsteps/2))] + [0.9 for i in range(int(nsteps/2))]} #
 Action and observation Space action_space = {'low': np.array([295]), 'high':
 np.array([302])} observation_space = {'low': np.array([0.7,300,0.8]),'high':
 np.array([1,350,0.9])} # Construct the environment parameter dictionary
 env_params = { 'N': nsteps, # Number of time steps 'tsim':T, # Simulation Time
@@ -59,15 +60,19 @@
 |---------------| | CSTR | [Hedengren, 2022](https://github.com/APMonitor/pdc/
 blob/master/CSTR_Control.ipynb) | [Source](https://github.com/MaximilianB2/pc-
 gym/blob/main/src/pcgym/model_classes.py) | | | First Order Sytem | N/A |
 [Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/
 model_classes.py) | | | Multistage Extraction Column | [Ingham et al, 2007 (pg
 471)](https://onlinelibrary.wiley.com/doi/book/10.1002/9783527614219) |
 [Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/
-model_classes.py) | | ## Citing `pc-gym` If you use `pc-gym` in your research,
-please cite using the following ``` @software{pcgym2024, author = {Max Bloor
-and ...}, title = {{pc-gym}: Reinforcement Learning Envionments for Process
-Control}, url = {https://github.com/MaximilianB2/pc-gym}, version = {0.0.4},
-year = {2024}, } ``` ## Other Great Gyms ð - â¨[safe-control-gym](https://
-github.com/utiasDSL/safe-control-gym) - â¨[safety-gymnasium](https://
-github.com/PKU-Alignment/safety-gymnasium) - â¨[gymnax](https://github.com/
-RobertTLange/gymnax)
+model_classes.py) | | | Nonsmooth Control|[Lim,1969](https://pubs.acs.org/doi/
+epdf/10.1021/i260031a007)|[Source](https://github.com/MaximilianB2/pc-gym/blob/
+main/src/pcgym/model_classes.py) || ## Citing `pc-gym` If you use `pc-gym` in
+your research, please cite using the following ``` @software{pcgym2024, author
+= {Max Bloor and and Jose Neto and Ilya Sandoval and Max Mowbray and Akhil
+Ahmed and Mehmet Mercangoz and Calvin Tsay and Antonio Del Rio-Chanona}, title
+= {{pc-gym}: Reinforcement Learning Envionments for Process Control}, url =
+{https://github.com/MaximilianB2/pc-gym}, version = {0.0.4}, year = {2024}, }
+``` ## Other Great Gyms ð - â¨[safe-control-gym](https://github.com/
+utiasDSL/safe-control-gym) - â¨[safety-gymnasium](https://github.com/PKU-
+Alignment/safety-gymnasium) - â¨[gymnax](https://github.com/RobertTLange/
+gymnax)
```

### Comparing `pcgym-0.0.9/README.md` & `pcgym-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,16 @@
   <b>Reinforcement learning environments for process control </b><br>
 </h1>
 <p align="center">
       <a href="https://www.python.org/doc/versions/">
         <img src="https://img.shields.io/badge/python-3.10-blue.svg" /></a>  
       <a href="https://opensource.org/license/mit">
         <img src="https://img.shields.io/badge/license-MIT-orange" /></a>
+      <a href="https://github.com/astral-sh/ruff">
+        <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json" /></a>
 </p>
 
 
 ## Quick start ⚡
 Setup a CSTR environment with a setpoint change
 
 ```python 
@@ -70,22 +72,23 @@
 ## Implemented Process Control Environments 🎛️
 
 |          Environment          | Reference | Source | Documentation |
 |:-----------------------------:|:---------:|:------:|---------------|
 |              CSTR             | [Hedengren, 2022](https://github.com/APMonitor/pdc/blob/master/CSTR_Control.ipynb)     | [Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/model_classes.py)      |               |
 |       First Order Sytem       |      N/A  | [Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/model_classes.py)        |               |
 | Multistage Extraction Column  |  [Ingham et al, 2007 (pg 471)](https://onlinelibrary.wiley.com/doi/book/10.1002/9783527614219)         | [Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/model_classes.py)        |               |
+| Nonsmooth Control|[Lim,1969](https://pubs.acs.org/doi/epdf/10.1021/i260031a007)|[Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/model_classes.py) ||
 
 
  
 ## Citing `pc-gym`
 If you use `pc-gym` in your research, please cite using the following 
 ```
 @software{pcgym2024,
-  author = {Max Bloor and ...},
+  author = {Max Bloor and and Jose Neto and Ilya Sandoval and Max Mowbray and Akhil Ahmed and Mehmet Mercangoz and Calvin Tsay and Antonio Del Rio-Chanona},
   title = {{pc-gym}: Reinforcement Learning Envionments for Process Control},
   url = {https://github.com/MaximilianB2/pc-gym},
   version = {0.0.4},
   year = {2024},
 }
 ```
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 ************ _[[_hh_tt_tt_pp_ss_::_//_//_gg_ii_tt_hh_uu_bb_.._cc_oo_mm_//_MM_aa_xx_ii_mm_ii_ll_ii_aa_nn_BB_22_//_pp_cc_--_gg_yy_mm_//_bb_ll_oo_bb_//_mm_aa_ii_nn_//_dd_oo_cc_ss_//_ii_mm_gg_//_pp_cc_--_gg_yy_mm_--_bb_ll_uu_ee_--
                                     _AA_ii_.._pp_nn_gg_]]
             RReeiinnffoorrcceemmeenntt lleeaarrnniinngg eennvviirroonnmmeennttss ffoorr pprroocceessss ccoonnttrrooll
                                      ************
   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-_3_._1_0_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-                           _b_a_d_g_e_/_l_i_c_e_n_s_e_-_M_I_T_-_o_r_a_n_g_e_]
+    _b_a_d_g_e_/_l_i_c_e_n_s_e_-_M_I_T_-_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_e_n_d_p_o_i_n_t_?_u_r_l_=_h_t_t_p_s_:_/_/
+      _r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_a_s_t_r_a_l_-_s_h_/_r_u_f_f_/_m_a_i_n_/_a_s_s_e_t_s_/_b_a_d_g_e_/_v_2_._j_s_o_n_]
 ## Quick start â¡ Setup a CSTR environment with a setpoint change ```python
 import pcgym # Simulation variables nsteps = 100 T = 25 # Setpoint SP = {'Ca':
 [0.85 for i in range(int(nsteps/2))] + [0.9 for i in range(int(nsteps/2))]} #
 Action and observation Space action_space = {'low': np.array([295]), 'high':
 np.array([302])} observation_space = {'low': np.array([0.7,300,0.8]),'high':
 np.array([1,350,0.9])} # Construct the environment parameter dictionary
 env_params = { 'N': nsteps, # Number of time steps 'tsim':T, # Simulation Time
@@ -25,15 +26,19 @@
 |---------------| | CSTR | [Hedengren, 2022](https://github.com/APMonitor/pdc/
 blob/master/CSTR_Control.ipynb) | [Source](https://github.com/MaximilianB2/pc-
 gym/blob/main/src/pcgym/model_classes.py) | | | First Order Sytem | N/A |
 [Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/
 model_classes.py) | | | Multistage Extraction Column | [Ingham et al, 2007 (pg
 471)](https://onlinelibrary.wiley.com/doi/book/10.1002/9783527614219) |
 [Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/
-model_classes.py) | | ## Citing `pc-gym` If you use `pc-gym` in your research,
-please cite using the following ``` @software{pcgym2024, author = {Max Bloor
-and ...}, title = {{pc-gym}: Reinforcement Learning Envionments for Process
-Control}, url = {https://github.com/MaximilianB2/pc-gym}, version = {0.0.4},
-year = {2024}, } ``` ## Other Great Gyms ð - â¨[safe-control-gym](https://
-github.com/utiasDSL/safe-control-gym) - â¨[safety-gymnasium](https://
-github.com/PKU-Alignment/safety-gymnasium) - â¨[gymnax](https://github.com/
-RobertTLange/gymnax)
+model_classes.py) | | | Nonsmooth Control|[Lim,1969](https://pubs.acs.org/doi/
+epdf/10.1021/i260031a007)|[Source](https://github.com/MaximilianB2/pc-gym/blob/
+main/src/pcgym/model_classes.py) || ## Citing `pc-gym` If you use `pc-gym` in
+your research, please cite using the following ``` @software{pcgym2024, author
+= {Max Bloor and and Jose Neto and Ilya Sandoval and Max Mowbray and Akhil
+Ahmed and Mehmet Mercangoz and Calvin Tsay and Antonio Del Rio-Chanona}, title
+= {{pc-gym}: Reinforcement Learning Envionments for Process Control}, url =
+{https://github.com/MaximilianB2/pc-gym}, version = {0.0.4}, year = {2024}, }
+``` ## Other Great Gyms ð - â¨[safe-control-gym](https://github.com/
+utiasDSL/safe-control-gym) - â¨[safety-gymnasium](https://github.com/PKU-
+Alignment/safety-gymnasium) - â¨[gymnax](https://github.com/RobertTLange/
+gymnax)
```

### Comparing `pcgym-0.0.9/pyproject.toml` & `pcgym-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pcgym"
-version = "0.0.9"
+version = "0.1.0"
 description = "Reinforcement learning suite of process control problems."
 requires-python = "~=3.10"
 license = { file = "LICENSE" }
 readme = "README.md"
 authors = [{ name = "Max Bloor", email = "max.bloor@gmail.com" }]
 keywords = [
   "reinforcement-learning",
```

### Comparing `pcgym-0.0.9/src/pcgym/evaluation_metrics.py` & `pcgym-0.1.0/src/pcgym/evaluation_metrics.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-""" policy evaluation metrics
+"""policy evaluation metrics
 - general flavour follows the paper by Manon Flageat et al (2024) - https://arxiv.org/pdf/2312.07178.pdf
 """
+
 import numpy as np
 from abc import ABC
 
+
 class metric_base(ABC):
     def __init__(self, scalarised_weight):
         pass
 
     def evaluate(self, policy_evaluator):
         """
         Evaluate the given policy using the specified environment.
@@ -24,34 +26,39 @@
         """
         Evaluate the dispersion of the policy.
 
         Returns:
         - The policy dispersion metric value.
         - data: nested dictionary
         """
-        raise NotImplementedError("Subclasses must implement the policy_dispersion_metric method.")
+        raise NotImplementedError(
+            "Subclasses must implement the policy_dispersion_metric method."
+        )
 
     def policy_performance_metric(self, data):
         """
         Evaluate the performance of the policy.
 
         Returns:
         - The policy performance metric value.
         """
-        raise NotImplementedError("Subclasses must implement the policy_performance_metric method.")
+        raise NotImplementedError(
+            "Subclasses must implement the policy_performance_metric method."
+        )
 
     def scalarised_performance(self, data):
         """
         Evaluate the scalarised performance of the policy.
 
         Returns:
         - The scalarised policy performance metric value.
         """
-        raise NotImplementedError("Subclasses must implement the scalarised_performance method.")
-
+        raise NotImplementedError(
+            "Subclasses must implement the scalarised_performance method."
+        )
 
 
 class standard_deviation:
     def __init__(self, data):
         self.data = data
 
     def get_value(self):
@@ -61,31 +68,33 @@
         Returns:
         - The policy dispersion metric value.
         - data: numpy array
         """
         return np.std(self.data, axis=-1)
 
 
-
 class median_absolute_deviation:
     def __init__(self, data):
-        if data.ndim <2: 
+        if data.ndim < 2:
             data = data.reshape((data.shape[0], 1))
         self.data = data
 
     def get_value(self):
         """
         Evaluate the dispersion of the policy.
 
         Returns:
         - The policy dispersion metric value.
         - data: numpy array
         """
-        
-        return np.median(np.abs(self.data - np.median(self.data,axis=-1)), axis=-1) # Currently only works for the reward component
+
+        return np.median(
+            np.abs(self.data - np.median(self.data, axis=-1)),
+            axis=-1,  # Currently only works for the reward component
+        )
 
 
 class mean_performance:
     def __init__(self, data):
         self.data = data
 
     def get_value(self):
@@ -109,113 +118,124 @@
         Returns:
         - The policy performance metric value.
         """
         return np.median(self.data, axis=-1)
 
 
 class reproducibility_metric(metric_base):
-    def __init__(self, dispersion:str, performance:str, scalarised_weight:float):
-
+    def __init__(self, dispersion: str, performance: str, scalarised_weight: float):
         # scalarised weight is defined in terms of the upper confidence bound
         # it should be negative for the lower confidence bound
         self.scalarised_weight = scalarised_weight
-        if dispersion == 'std':
+        if dispersion == "std":
             self.dispersion = standard_deviation
-        elif dispersion == 'mad':
+        elif dispersion == "mad":
             self.dispersion = median_absolute_deviation
         else:
             raise ValueError("Invalid dispersion metric")
-        
-        if performance == 'mean':
+
+        if performance == "mean":
             self.performance = mean_performance
-        elif performance == 'median':
+        elif performance == "median":
             self.performance = median_performance
         else:
             raise ValueError("Invalid performance metric")
 
-    def evaluate(self, policy_evaluator, component:str=None):
+    def evaluate(self, policy_evaluator, component: str = None):
         """
         Evaluate the given policy using the specified environment.
 
         Parameters
         ----------
         policy_evaluator : The policy evaluator to generate data for a number of policy rollouts.
                             must be constructed prior to passing to evaluate
         """
 
         try:
-            self.data = policy_evaluator.data # Try to get data from policy evaluator if this fails then call the get_rollouts method to generate the data
+            self.data = policy_evaluator.data  # Try to get data from policy evaluator if this fails then call the get_rollouts method to generate the data
         except Exception:
             self.data = policy_evaluator.get_rollouts()
 
         return self.scalarised_performance(self.data, component)
 
-
-    def policy_dispersion_metric(self, data:dict, component:str):
+    def policy_dispersion_metric(self, data: dict, component: str):
         """
         Evaluate the dispersion of the policy.
 
         Returns
         -------
         The policy dispersion metric value.
         """
         values = {k: {} for k in data.keys()}
-    
-        for policy in data.keys(): # has structure n_x x T x reps  - operation always applied along the reps row
 
+        for policy in data.keys():  # has structure n_x x T x reps  - operation always applied along the reps row
             if component is None:
                 for comp in data[policy].keys():
                     operation = self.determine_op(comp)
-                    values[policy][comp] = self.dispersion(operation(data[policy][comp])).get_value()
+                    values[policy][comp] = self.dispersion(
+                        operation(data[policy][comp])
+                    ).get_value()
             else:
                 operation = self.determine_op(component)
-                values[policy][component] = self.dispersion(operation(data[policy][component])).get_value()
-
-       
+                values[policy][component] = self.dispersion(
+                    operation(data[policy][component])
+                ).get_value()
 
         return values
 
-    def policy_performance_metric(self, data:dict, component:str):
+    def policy_performance_metric(self, data: dict, component: str):
         """
         Evaluate the performance of the policy.
 
         Returns
         -------
         The policy performance metric value.
         """
         values = {k: {} for k in data.keys()}
 
         for policy in data.keys():
             if component is None:
                 for comp in data[policy].keys():
                     operation = self.determine_op(comp)
-                    values[policy][comp] = self.performance(operation(data[policy][comp])).get_value()
+                    values[policy][comp] = self.performance(
+                        operation(data[policy][comp])
+                    ).get_value()
             else:
                 operation = self.determine_op(component)
-                values[policy][component] = self.performance(operation(data[policy][component])).get_value()
+                values[policy][component] = self.performance(
+                    operation(data[policy][component])
+                ).get_value()
 
         return values
 
-    def scalarised_performance(self, data:dict, component:str):
+    def scalarised_performance(self, data: dict, component: str):
         """
         Evaluate the scalarised performance of the policy.
 
         Returns
         -------
         The scalarised policy performance metric value.
         set component to None to scalarise over all components
         """
 
         performance = self.policy_performance_metric(data, component)
         dispersion = self.policy_dispersion_metric(data, component)
-        return {k: {comp: performance[k][comp] + self.scalarised_weight * dispersion[k][comp] for comp in performance[k].keys()} for k in performance.keys()}
+        return {
+            k: {
+                comp: performance[k][comp]
+                + self.scalarised_weight * dispersion[k][comp]
+                for comp in performance[k].keys()
+            }
+            for k in performance.keys()
+        }
 
     def determine_op(self, component):
-
-        if component == 'x': 
+        if component == "x":
             return lambda x: x
-        elif component == 'u':
+        elif component == "u":
             return lambda x: x
-        elif component == 'r':
-            return lambda x: x # sum over discrete time indices (undiscounted)
-        elif component == 'g':
-            return lambda x: np.max(x, axis=0) # return the greatest constraint violation of n_g defined
+        elif component == "r":
+            return lambda x: x  # sum over discrete time indices (undiscounted)
+        elif component == "g":
+            return lambda x: np.max(
+                x, axis=0
+            )  # return the greatest constraint violation of n_g defined
```

### Comparing `pcgym-0.0.9/src/pcgym/integrator.py` & `pcgym-0.1.0/src/pcgym/integrator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,147 +1,170 @@
 from casadi import SX, vertcat, Function, integrator
-from diffrax import diffeqsolve, ODETerm, Tsit5, PIDController 
+from diffrax import diffeqsolve, ODETerm, Tsit5, PIDController
 import jax.numpy as jnp
 
+
 class integration_engine:
-    '''
+    """
     Integration class
     Contains both the casadi and JAX integration wrappers.
 
     Inputs: Environment, x0, dt,u_t
 
-    Output: x+  
-    '''
+    Output: x+
+    """
 
-    def __init__(self,make_env,env_params):
+    def __init__(self, make_env, env_params):
         self.env = make_env(env_params)
         try:
-            integration_method = env_params['integration_method']
+            integration_method = env_params["integration_method"]
         except Exception:
-            integration_method = 'casadi'
-        assert integration_method in ['jax', 'casadi'], "integration_method must be either 'jax' or 'casadi'"
-        
-        # NOTE common ode model signature
-        # all self.env.model currently have the signature ODE(states, controls)
-        # diffrax expects the signature ode(t, states, params)
+            integration_method = "casadi"
+        assert integration_method in [
+            "jax",
+            "casadi",
+        ], "integration_method must be either 'jax' or 'casadi'"
+
+        # NOTE common ode model signature
+        # all self.env.model currently have the signature ODE(states, controls)
+        # diffrax expects the signature ode(t, states, params)
         # the parameters are fixed within the models so the controllers are the inputs instead
 
-        if integration_method == 'casadi':
+        if integration_method == "casadi":
             # Generate casadi model
             self.sym_x = self.gen_casadi_variable(self.env.Nx_oracle, "x")
-            self.sym_u = self.gen_casadi_variable(self.env.Nu, "u")    
-            self.casadi_sym_model = self.casadify(self.env.model, self.sym_x, self.sym_u)
-            self.casadi_model_func = self.gen_casadi_function([self.sym_x, self.sym_u],[self.casadi_sym_model],
-                                                            "model_func", ["x","u"], ["model_rhs"])
-        
-        if integration_method == 'jax':
-            def autonomous_model(t,x,u): # ignore time
-                return jnp.array(self.env.model(x, u)) # ignore time
+            self.sym_u = self.gen_casadi_variable(self.env.Nu, "u")
+            self.casadi_sym_model = self.casadify(
+                self.env.model, self.sym_x, self.sym_u
+            )
+            self.casadi_model_func = self.gen_casadi_function(
+                [self.sym_x, self.sym_u],
+                [self.casadi_sym_model],
+                "model_func",
+                ["x", "u"],
+                ["model_rhs"],
+            )
+
+        if integration_method == "jax":
+
+            def autonomous_model(t, x, u):  # ignore time
+                return jnp.array(self.env.model(x, u))  # ignore time
+
             self.jax_ode = ODETerm(autonomous_model)
-            self.jax_solver = Tsit5() 
+            self.jax_solver = Tsit5()
             self.t0 = 0.0
             self.tf = self.env.dt
-            self.dt0 = None # adaptive step size
-            self.step_controller = PIDController(rtol=1e-5, atol=1e-5)   
- 
+            self.dt0 = None  # adaptive step size
+            self.step_controller = PIDController(rtol=1e-5, atol=1e-5)
+
     def jax_step(self, state, uk):
-        '''
+        """
         Integrate one time step with JAX.
 
         input: x0, uk
         output: x+
-        '''
-        y0 = jnp.array(state[:self.env.Nx_oracle]) # Only pass the states of the model (exclude the setpoints)
+        """
+        y0 = jnp.array(
+            state[: self.env.Nx_oracle]
+        )  # Only pass the states of the model (exclude the setpoints)
         uk = jnp.array(uk)
-        solution = diffeqsolve(self.jax_ode, self.jax_solver, self.t0, self.tf, self.dt0, y0, args=uk,stepsize_controller=self.step_controller)
+        solution = diffeqsolve(
+            self.jax_ode,
+            self.jax_solver,
+            self.t0,
+            self.tf,
+            self.dt0,
+            y0,
+            args=uk,
+            stepsize_controller=self.step_controller,
+        )
         return solution.ys[-1, :]  # return only final state
 
-    def casadi_step(self,state,uk):
-
-        '''
+    def casadi_step(self, state, uk):
+        """
         Integrate one time step with casadi.
 
         input: x0, uk
         output: x+
-        '''
+        """
         plant_func = self.casadi_model_func
         discretised_plant = self.discretise_model(plant_func, self.env.dt)
-   
-        xk = state[:self.env.Nx_oracle]
+
+        xk = state[: self.env.Nx_oracle]
 
         Fk = discretised_plant(x0=xk, p=uk)
         return Fk
 
     def casadify(self, model, sym_x, sym_u):
         """
         Given a model with Nx states and Nu inputs and returns rhs of ode,
         return casadi symbolic model (Not function!)
-        
+
         Inputs:
             model - model to be casidified i.e. a list of ode rhs of size Nx
-            
+
         Outputs:
             dxdt - casadi symbolic model of size Nx of rhs of ode
         """
-    
+
         dxdt = model(sym_x, sym_u)
-        dxdt = vertcat(*dxdt) #Return casadi list of size Nx
+        dxdt = vertcat(*dxdt)  # Return casadi list of size Nx
 
         return dxdt
 
-
-    def gen_casadi_variable(self, n_dim, name = "x"):
+    def gen_casadi_variable(self, n_dim, name="x"):
         """
         Generates casadi symbolic variable given n_dim and name for variable
-        
+
         Inputs:
             n_dim - symbolic variable dimension
             name - name for symbolic variable
-            
+
         Outputs:
             var - symbolic version of variable
         """
 
         var = SX.sym(name, n_dim)
 
         return var
 
-    def gen_casadi_function(self, casadi_input, casadi_output, name, input_name=[], output_name=[]):
+    def gen_casadi_function(
+        self, casadi_input, casadi_output, name, input_name=[], output_name=[]
+    ):
         """
         Generates a casadi function which maps inputs (casadi symbolic inputs) to outputs (casadi symbolic outputs)
-        
+
         Inputs:
             casadi_input - list of casadi symbolics constituting inputs
             casadi_output - list of casadi symbolic output of function
             name - name of function
             input_name - list of names for each input
             output_name - list of names for each output
-        
+
         Outputs:
             casadi function mapping [inputs] -> [outputs]
-        
+
         """
 
         function = Function(name, casadi_input, casadi_output, input_name, output_name)
 
         return function
-    
+
     def discretise_model(self, casadi_func, delta_t):
         """
         Input:
             casadi_func to be discretised
-        
+
         Output:
             discretised casadi func
         """
         x = SX.sym("x", self.env.Nx_oracle)
-       
+
         u = SX.sym("u", self.env.Nu)
         xdot = casadi_func(x, u)
 
-        dae = {'x':x, 'p':u, 'ode':xdot} 
+        dae = {"x": x, "p": u, "ode": xdot}
         t0 = 0
         tf = delta_t
-        discrete_model = integrator('discrete_model', 'cvodes', dae,t0,tf)
+        discrete_model = integrator("discrete_model", "cvodes", dae, t0, tf)
 
         return discrete_model
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pcgym-0.0.9/src/pcgym/model_classes.py` & `pcgym-0.1.0/src/pcgym/model_classes.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,261 +10,301 @@
 # ValueError: Non-hashable static arguments are not supported.
 
 # kw_only: require the parameter names if they want
 # to be set when the object is created
 
 # ==== CSTR Model ====#
 
-#Temperature Control of an unstable CSTR reactor.
-# highly exothermic reaction. This is an example of a highly nonlinear process prone to 
+
+# Temperature Control of an unstable CSTR reactor.
+# highly exothermic reaction. This is an example of a highly nonlinear process prone to
 # exponential run-away when the temperature rises too quickly.
-#source: https://apmonitor.com/pdc/index.php/Main/StirredReactor
+# source: https://apmonitor.com/pdc/index.php/Main/StirredReactor
 @dataclass(frozen=False, kw_only=True)
 class cstr_ode:
-  # Parameters
-  q:float = 100 #m3/s
-  V:float = 100 #m3
-  rho:float = 1000 #kg/m3
-  C:float = 0.239 #Joules/kg K
-  deltaHr:float = -5e4 #Joules/kg K
-  EA_over_R:float = 8750 #K
-  k0:float = 7.2e10 #1/sec
-  UA:float = 5e4 # W/K
-  Ti:float = 350 #K
-  Caf:float = 1
-  int_method:str = 'jax'
-
-     
-  def __call__(self, x, u):
-    # JAX requires jnp functions and arrays hence two versions
-    if self.int_method == 'jax':
-      ca,T = x[0],x[1]
-      if u.shape == (1,):
-        Tc = u[0]
-      else:
-         Tc,self.Ti,self.Caf = u[0],u[1],u[2]
-      Tc = u[0]
-      rA = self.k0 * jnp.exp(-self.EA_over_R/T)*ca
-      dxdt = jnp.array([
-          self.q/self.V*(self.Caf-ca) - rA,
-          self.q/self.V*(self.Ti-T) + ((-self.deltaHr)*rA)*(1/(self.rho*self.C)) + self.UA*(Tc-T)*(1/(self.rho*self.C*self.V))])
-      return dxdt
-    else:
-      ca,T = x[0],x[1]
-      if u.shape == (1,1):
-          Tc = u[0]
-      else:
-          Tc,self.Ti,self.Caf = u[0],u[1],u[2]
-      rA = self.k0 * np.exp(-self.EA_over_R/T)*ca
-      dxdt = [
-          self.q/self.V*(self.Caf-ca) - rA,
-          self.q/self.V*(self.Ti-T) + ((-self.deltaHr)*rA)*(1/(self.rho*self.C)) + self.UA*(Tc-T)*(1/(self.rho*self.C*self.V))]
-      return dxdt
-    
-  def info(self):
-    # Return a dictionary with the model information
-    info = {
-        'parameters': self.__dict__.copy(), 
-        'states': ['Ca', 'T'],
-        'inputs': ['Tc'],
-        'disturbances': ['Ti', 'Caf'],
-    }
-    info['parameters'].pop('int_method', None)  # Remove 'int_method' from the dictionary since it is not a parameter of the model
-    return info
+    # Parameters
+    q: float = 100  # m3/s
+    V: float = 100  # m3
+    rho: float = 1000  # kg/m3
+    C: float = 0.239  # Joules/kg K
+    deltaHr: float = -5e4  # Joules/kg K
+    EA_over_R: float = 8750  # K
+    k0: float = 7.2e10  # 1/sec
+    UA: float = 5e4  # W/K
+    Ti: float = 350  # K
+    Caf: float = 1
+    int_method: str = "jax"
+
+    def __call__(self, x, u):
+        # JAX requires jnp functions and arrays hence two versions
+        if self.int_method == "jax":
+            ca, T = x[0], x[1]
+            if u.shape == (1,):
+                Tc = u[0]
+            else:
+                Tc, self.Ti, self.Caf = u[0], u[1], u[2]
+            Tc = u[0]
+            rA = self.k0 * jnp.exp(-self.EA_over_R / T) * ca
+            dxdt = jnp.array(
+                [
+                    self.q / self.V * (self.Caf - ca) - rA,
+                    self.q / self.V * (self.Ti - T)
+                    + ((-self.deltaHr) * rA) * (1 / (self.rho * self.C))
+                    + self.UA * (Tc - T) * (1 / (self.rho * self.C * self.V)),
+                ]
+            )
+            return dxdt
+        else:
+            ca, T = x[0], x[1]
+            if u.shape == (1, 1):
+                Tc = u[0]
+            else:
+                Tc, self.Ti, self.Caf = u[0], u[1], u[2]
+            rA = self.k0 * np.exp(-self.EA_over_R / T) * ca
+            dxdt = [
+                self.q / self.V * (self.Caf - ca) - rA,
+                self.q / self.V * (self.Ti - T)
+                + ((-self.deltaHr) * rA) * (1 / (self.rho * self.C))
+                + self.UA * (Tc - T) * (1 / (self.rho * self.C * self.V)),
+            ]
+            return dxdt
+
+    def info(self):
+        # Return a dictionary with the model information
+        info = {
+            "parameters": self.__dict__.copy(),
+            "states": ["Ca", "T"],
+            "inputs": ["Tc"],
+            "disturbances": ["Ti", "Caf"],
+        }
+        info["parameters"].pop(
+            "int_method", None
+        )  # Remove 'int_method' from the dictionary since it is not a parameter of the model
+        return info
+
 
 # ==== First Order System Model ====#
 @dataclass(frozen=False, kw_only=True)
 class first_order_system_ode:
-  # Parameters
-  K:float = 1
-  tau:float = 0.5
-  int_method:str = 'jax'
-
-  def __call__(self, x, u):
-    # JAX requires jnp functions and arrays hence two versions
-    if self.int_method == 'jax':
-      #Model Equations
-      x = x[0]
-      u = u[0]
-
-      dxdt = jnp.array([(self.K*u - x)*1/self.tau])
-        
-      return dxdt
-    else:
-      x = x[0]
-      u = u[0]
-
-      dxdt = [(self.K*u - x)*1/self.tau]
-        
-      return dxdt
-    
-  def info(self):
-    # Return a dictionary with the model information
-    info = {
-        'parameters': self.__dict__.copy(), 
-        'states': ['x'],
-        'inputs': ['u'],
-        'disturbances': ['None'],
-    }
-    info['parameters'].pop('int_method', None)  # Remove 'int_method' from the dictionary since it is not a parameter of the model
-    return info
-  
+    # Parameters
+    K: float = 1
+    tau: float = 0.5
+    int_method: str = "jax"
+
+    def __call__(self, x, u):
+        # JAX requires jnp functions and arrays hence two versions
+        if self.int_method == "jax":
+            # Model Equations
+            x = x[0]
+            u = u[0]
+
+            dxdt = jnp.array([(self.K * u - x) * 1 / self.tau])
+
+            return dxdt
+        else:
+            x = x[0]
+            u = u[0]
+
+            dxdt = [(self.K * u - x) * 1 / self.tau]
+
+            return dxdt
+
+    def info(self):
+        # Return a dictionary with the model information
+        info = {
+            "parameters": self.__dict__.copy(),
+            "states": ["x"],
+            "inputs": ["u"],
+            "disturbances": ["None"],
+        }
+        info["parameters"].pop(
+            "int_method", None
+        )  # Remove 'int_method' from the dictionary since it is not a parameter of the model
+        return info
+
+
 @dataclass(frozen=False, kw_only=True)
 class multistage_extraction_ode:
-  # Parameters
-  Vl:float = 5 #Liquid volume in each stage
-  Vg:float = 5 #Gas volume in each stage
-  m:float = 1 #Equilibrium constant [-]
-  Kla:float = 5 #Mass transfer capacity constant 1/hr
-  eq_exponent:float = 2 #Change the nonlinearity of the equilibrium relationship
-  X0:float = 0.6 #Feed concentration of liquid
-  Y6:float = 0.05 #Feed conc of gas
-  int_method:str = 'jax'
-
-    
-  def __call__(self, x, u):
-    # JAX requires jnp functions and arrays hence two versions
-    if self.int_method == 'jax':
-      if u.shape == (2,):
-        L, G = u[0], u[1]
-      else:
-          L, G, self.X0, self.Y6 = u[0], u[1], u[2], u[3]
-      ###Model Equations###
-
-      ##States##
-      #Xn - Concentration of solute in liquid pase of stage n [kg/m3]
-      #Yn - Concentration of solute in gas phase of stage n [kg/m3]
-      X1, Y1, X2, Y2, X3, Y3, X4, Y4, X5, Y5 = x[0], x[1], x[2], x[3], x[4], x[5], x[6], x[7], x[8], x[9]
-
-      ##Inputs##
-      #L - Liquid flowrate m3/hr
-      #G - Gas flowrate m3/hr
-      X1_eq = ((Y1**self.eq_exponent)/self.m)
-      X2_eq = ((Y2**self.eq_exponent)/self.m)
-      X3_eq = ((Y3**self.eq_exponent)/self.m)
-      X4_eq = ((Y4**self.eq_exponent)/self.m)
-      X5_eq = ((Y5**self.eq_exponent)/self.m)
-
-      Q1 = self.Kla*(X1 - X1_eq)*self.Vl
-      Q2 = self.Kla*(X2 - X2_eq)*self.Vl
-      Q3 = self.Kla*(X3 - X3_eq)*self.Vl
-      Q4 = self.Kla*(X4 - X4_eq)*self.Vl
-      Q5 = self.Kla*(X5 - X5_eq)*self.Vl
-
-      dxdt = jnp.array([
-          (1/self.Vl)*(L * (self.X0 - X1) - Q1),
-          (1/self.Vg)*(G * (Y2 - Y1) + Q1),
-          (1/self.Vl)*(L * (X1 - X2) - Q2),
-          (1/self.Vg)*(G * (Y3 - Y2) + Q2),
-          (1/self.Vl)*(L * (X2 - X3) - Q3),
-          (1/self.Vg)*(G * (Y4 - Y3) + Q3),
-          (1/self.Vl)*(L * (X3 - X4) - Q4),
-          (1/self.Vg)*(G * (Y5 - Y4) + Q4),
-          (1/self.Vl)*(L * (X4 - X5) - Q5),
-          (1/self.Vg)*(G * (self.Y6 - Y5) + Q5),
-          ])
-      return dxdt
-    else:
-      if u.shape == (2,1):
-        L, G = u[0], u[1]
-      else:
-          L, G, self.X0, self.Y6 = u[0], u[1], u[2], u[3]
-      ###Model Equations###
-
-      ##States##
-      #Xn - Concentration of solute in liquid pase of stage n [kg/m3]
-      #Yn - Concentration of solute in gas phase of stage n [kg/m3]
-
-      X1, Y1, X2, Y2, X3, Y3, X4, Y4, X5, Y5 = x[0], x[1], x[2], x[3], x[4], x[5], x[6], x[7], x[8], x[9]
-
-      ##Inputs##
-      #L - Liquid flowrate m3/hr
-      #G - Gas flowrate m3/hr
-
-
-
-      X1_eq = ((Y1**self.eq_exponent)/self.m)
-      X2_eq = ((Y2**self.eq_exponent)/self.m)
-      X3_eq = ((Y3**self.eq_exponent)/self.m)
-      X4_eq = ((Y4**self.eq_exponent)/self.m)
-      X5_eq = ((Y5**self.eq_exponent)/self.m)
-
-      Q1 = self.Kla*(X1 - X1_eq)*self.Vl
-      Q2 = self.Kla*(X2 - X2_eq)*self.Vl
-      Q3 = self.Kla*(X3 - X3_eq)*self.Vl
-      Q4 = self.Kla*(X4 - X4_eq)*self.Vl
-      Q5 = self.Kla*(X5 - X5_eq)*self.Vl
-
-      dxdt = [
-          (1/self.Vl)*(L * (self.X0 - X1) - Q1),
-          (1/self.Vg)*(G * (Y2 - Y1) + Q1),
-          (1/self.Vl)*(L * (X1 - X2) - Q2),
-          (1/self.Vg)*(G * (Y3 - Y2) + Q2),
-          (1/self.Vl)*(L * (X2 - X3) - Q3),
-          (1/self.Vg)*(G * (Y4 - Y3) + Q3),
-          (1/self.Vl)*(L * (X3 - X4) - Q4),
-          (1/self.Vg)*(G * (Y5 - Y4) + Q4),
-          (1/self.Vl)*(L * (X4 - X5) - Q5),
-          (1/self.Vg)*(G * (self.Y6 - Y5) + Q5),
-          ]
-
-      return dxdt
-
-    
-  def info(self):
-    # Return a dictionary with the model information
-    info = {
-        'parameters': self.__dict__.copy(), 
-        'states': ['X1', 'Y1', 'X2', 'Y2', 'X3', 'Y3', 'X4', 'Y4', 'X5', 'Y5'],
-        'inputs': ['L','G'],
-        'disturbances': ['X0', 'Y6'],
-    }
-    info['parameters'].pop('int_method', None)  # Remove 'int_method' from the dictionary since it is not a parameter of the model
-    return info
+    # Parameters
+    Vl: float = 5  # Liquid volume in each stage
+    Vg: float = 5  # Gas volume in each stage
+    m: float = 1  # Equilibrium constant [-]
+    Kla: float = 5  # Mass transfer capacity constant 1/hr
+    eq_exponent: float = 2  # Change the nonlinearity of the equilibrium relationship
+    X0: float = 0.6  # Feed concentration of liquid
+    Y6: float = 0.05  # Feed conc of gas
+    int_method: str = "jax"
+
+    def __call__(self, x, u):
+        # JAX requires jnp functions and arrays hence two versions
+        if self.int_method == "jax":
+            if u.shape == (2,):
+                L, G = u[0], u[1]
+            else:
+                L, G, self.X0, self.Y6 = u[0], u[1], u[2], u[3]
+            ###Model Equations###
+
+            ##States##
+            # Xn - Concentration of solute in liquid pase of stage n [kg/m3]
+            # Yn - Concentration of solute in gas phase of stage n [kg/m3]
+            X1, Y1, X2, Y2, X3, Y3, X4, Y4, X5, Y5 = (
+                x[0],
+                x[1],
+                x[2],
+                x[3],
+                x[4],
+                x[5],
+                x[6],
+                x[7],
+                x[8],
+                x[9],
+            )
+
+            ##Inputs##
+            # L - Liquid flowrate m3/hr
+            # G - Gas flowrate m3/hr
+            X1_eq = (Y1**self.eq_exponent) / self.m
+            X2_eq = (Y2**self.eq_exponent) / self.m
+            X3_eq = (Y3**self.eq_exponent) / self.m
+            X4_eq = (Y4**self.eq_exponent) / self.m
+            X5_eq = (Y5**self.eq_exponent) / self.m
+
+            Q1 = self.Kla * (X1 - X1_eq) * self.Vl
+            Q2 = self.Kla * (X2 - X2_eq) * self.Vl
+            Q3 = self.Kla * (X3 - X3_eq) * self.Vl
+            Q4 = self.Kla * (X4 - X4_eq) * self.Vl
+            Q5 = self.Kla * (X5 - X5_eq) * self.Vl
+
+            dxdt = jnp.array(
+                [
+                    (1 / self.Vl) * (L * (self.X0 - X1) - Q1),
+                    (1 / self.Vg) * (G * (Y2 - Y1) + Q1),
+                    (1 / self.Vl) * (L * (X1 - X2) - Q2),
+                    (1 / self.Vg) * (G * (Y3 - Y2) + Q2),
+                    (1 / self.Vl) * (L * (X2 - X3) - Q3),
+                    (1 / self.Vg) * (G * (Y4 - Y3) + Q3),
+                    (1 / self.Vl) * (L * (X3 - X4) - Q4),
+                    (1 / self.Vg) * (G * (Y5 - Y4) + Q4),
+                    (1 / self.Vl) * (L * (X4 - X5) - Q5),
+                    (1 / self.Vg) * (G * (self.Y6 - Y5) + Q5),
+                ]
+            )
+            return dxdt
+        else:
+            if u.shape == (2, 1):
+                L, G = u[0], u[1]
+            else:
+                L, G, self.X0, self.Y6 = u[0], u[1], u[2], u[3]
+            ###Model Equations###
+
+            ##States##
+            # Xn - Concentration of solute in liquid pase of stage n [kg/m3]
+            # Yn - Concentration of solute in gas phase of stage n [kg/m3]
+
+            X1, Y1, X2, Y2, X3, Y3, X4, Y4, X5, Y5 = (
+                x[0],
+                x[1],
+                x[2],
+                x[3],
+                x[4],
+                x[5],
+                x[6],
+                x[7],
+                x[8],
+                x[9],
+            )
+
+            ##Inputs##
+            # L - Liquid flowrate m3/hr
+            # G - Gas flowrate m3/hr
+
+            X1_eq = (Y1**self.eq_exponent) / self.m
+            X2_eq = (Y2**self.eq_exponent) / self.m
+            X3_eq = (Y3**self.eq_exponent) / self.m
+            X4_eq = (Y4**self.eq_exponent) / self.m
+            X5_eq = (Y5**self.eq_exponent) / self.m
+
+            Q1 = self.Kla * (X1 - X1_eq) * self.Vl
+            Q2 = self.Kla * (X2 - X2_eq) * self.Vl
+            Q3 = self.Kla * (X3 - X3_eq) * self.Vl
+            Q4 = self.Kla * (X4 - X4_eq) * self.Vl
+            Q5 = self.Kla * (X5 - X5_eq) * self.Vl
+
+            dxdt = [
+                (1 / self.Vl) * (L * (self.X0 - X1) - Q1),
+                (1 / self.Vg) * (G * (Y2 - Y1) + Q1),
+                (1 / self.Vl) * (L * (X1 - X2) - Q2),
+                (1 / self.Vg) * (G * (Y3 - Y2) + Q2),
+                (1 / self.Vl) * (L * (X2 - X3) - Q3),
+                (1 / self.Vg) * (G * (Y4 - Y3) + Q3),
+                (1 / self.Vl) * (L * (X3 - X4) - Q4),
+                (1 / self.Vg) * (G * (Y5 - Y4) + Q4),
+                (1 / self.Vl) * (L * (X4 - X5) - Q5),
+                (1 / self.Vg) * (G * (self.Y6 - Y5) + Q5),
+            ]
+
+            return dxdt
+
+    def info(self):
+        # Return a dictionary with the model information
+        info = {
+            "parameters": self.__dict__.copy(),
+            "states": ["X1", "Y1", "X2", "Y2", "X3", "Y3", "X4", "Y4", "X5", "Y5"],
+            "inputs": ["L", "G"],
+            "disturbances": ["X0", "Y6"],
+        }
+        info["parameters"].pop(
+            "int_method", None
+        )  # Remove 'int_method' from the dictionary since it is not a parameter of the model
+        return info
 
 
 # ==== Bang-Bang Control Model ====#
 @dataclass(frozen=False, kw_only=True)
 class nonsmooth_control_ode:
-  # Parameters
-  int_method:str = 'jax'
-  a_11:float = 0
-  a_12:float = 1
-  a_21:float = -2
-  a_22:float = -3
-  b_1:float = 0
-  b_2:float = 1
-
-  def __call__(self, x, u):
-    # JAX requires jnp functions and arrays hence two versions
-    if self.int_method == 'jax':
-      # states
-      x1, x2 = x[0], x[1]
-
-      # ode system
-      dxdt = jnp.array([
-          self.a_11*x1 + self.a_12*x2 + self.b_1*u,
-          self.a_21*x1 + self.a_22*x2 + self.b_2*u
-      ])
-        
-      return dxdt
-    else:
-      # states
-      x1, x2 = x[0], x[1]
-
-      dxdt = [
-          self.a_11*x1 + self.a_12*x2 + self.b_1*u,
-          self.a_21*x1 + self.a_22*x2 + self.b_2*u
-      ]
-        
-      return dxdt
-    
-  def info(self):
-    # Return a dictionary with the model information
-    info = {
-        'parameters': self.__dict__.copy(), 
-        'states': ['X1', 'X2'],
-        'inputs': ['U'],
-        'disturbances': ['None'],
-    }
-    info['parameters'].pop('int_method', None)  # Remove 'int_method' from the dictionary since it is not a parameter of the model
-    return info
+    # Parameters
+    int_method: str = "jax"
+    a_11: float = 0
+    a_12: float = 1
+    a_21: float = -2
+    a_22: float = -3
+    b_1: float = 0
+    b_2: float = 1
+
+    def __call__(self, x, u):
+        # JAX requires jnp functions and arrays hence two versions
+        if self.int_method == "jax":
+            # states
+            x1, x2 = x[0], x[1]
+
+            # ode system
+            dxdt = jnp.array(
+                [
+                    self.a_11 * x1 + self.a_12 * x2 + self.b_1 * u,
+                    self.a_21 * x1 + self.a_22 * x2 + self.b_2 * u,
+                ]
+            )
+
+            return dxdt
+        else:
+            # states
+            x1, x2 = x[0], x[1]
+
+            dxdt = [
+                self.a_11 * x1 + self.a_12 * x2 + self.b_1 * u,
+                self.a_21 * x1 + self.a_22 * x2 + self.b_2 * u,
+            ]
+
+            return dxdt
+
+    def info(self):
+        # Return a dictionary with the model information
+        info = {
+            "parameters": self.__dict__.copy(),
+            "states": ["X1", "X2"],
+            "inputs": ["U"],
+            "disturbances": ["None"],
+        }
+        info["parameters"].pop(
+            "int_method", None
+        )  # Remove 'int_method' from the dictionary since it is not a parameter of the model
+        return info
```

### Comparing `pcgym-0.0.9/src/pcgym/oracle.py` & `pcgym-0.1.0/src/pcgym/oracle.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,230 +1,292 @@
 from casadi import MX, Function, integrator, Opti, vertcat, sum1, sum2
 import numpy as np
 
-class oracle():
-    '''
-    Oracle Class - Class to solve the optimal control problem with perfect 
+
+class oracle:
+    """
+    Oracle Class - Class to solve the optimal control problem with perfect
     knowledge of the environment.
-    Oracle is a nonlinear model predictive controller (nMPC), 
+    Oracle is a nonlinear model predictive controller (nMPC),
     using the multiple shooting method.
 
     Inputs: Env
 
     Outputs: Optimal control and state trajectories
-    '''
+    """
+
+    def __init__(self, env, env_params, MPC_params=False):
+        self.env_params = env_params
+        self.env_params["integration_method"] = "casadi"
+        self.env = env(env_params)
+
+        self.x0 = env_params["x0"]
+        self.T = self.env.tsim
+        if not MPC_params:
+            self.N = 5
+            self.R = 0.05
+        else:
+            self.N = MPC_params["N"]  # Horizon length
+            self.R = MPC_params["R"]  # Control penalty scaling factors
+        self.model_info = self.env.model.info()
 
-    def __init__(self,env,env_params,MPC_params = False):  
-      self.env_params = env_params
-      self.env_params['integration_method'] = 'casadi'
-      self.env = env(env_params)
-   
-      self.x0 = env_params['x0']
-      self.T = self.env.tsim
-      if not MPC_params:
-        self.N = 5
-        self.R = 0.05
-      else:
-        self.N = MPC_params['N'] #Horizon length 
-        self.R = MPC_params['R'] #Control penalty scaling factors
-      self.model_info = self.env.model.info()
     def model_gen(self):
-      '''
-      Generates a model for the given environment.
+        """
+        Generates a model for the given environment.
+
+        Returns:
+        f: A casadi function that can be used to solve the differential equations defined by the model.
+        """
+
+        self.u = MX.sym("u", self.env.Nu)
+        self.x = MX.sym("x", self.env.Nx_oracle)
+        dxdt = self.env.model(self.x, self.u)
+        dxdt = vertcat(*dxdt)
+        f = Function("f", [self.x, self.u], [dxdt], ["x", "u"], ["dxdt"])
+        return f
 
-      Returns:
-      f: A casadi function that can be used to solve the differential equations defined by the model.
-      '''
-
-      self.u  = MX.sym('u',self.env.Nu)
-      self.x = MX.sym('x',self.env.Nx_oracle)
-      dxdt = self.env.model(self.x,self.u)
-      dxdt = vertcat(*dxdt)
-      f = Function('f',[self.x,self.u],[dxdt],['x','u'],['dxdt'])
-      return f
-    
     def integrator_gen(self):
-      '''
-      Generates an integrator object for the given model.
+        """
+        Generates an integrator object for the given model.
+
+        Returns:
+        F: A casadi function that can be used to integrate the model over a given time horizon.
+        """
+
+        f = self.model_gen()
+        tf = self.env.dt
+        t0 = 0
+        dae = {"x": self.x, "p": self.u, "ode": f(self.x, self.u)}
+        opts = {"simplify": True, "number_of_finite_elements": 4}
+        intg = integrator("intg", "rk", dae, t0, tf, opts)
+        res = intg(x0=self.x, p=self.u)
+        x_next = res["xf"]
+        F = Function("F", [self.x, self.u], [x_next], ["x", "u"], ["x_next"])
+        return F
 
-      Returns:
-      F: A casadi function that can be used to integrate the model over a given time horizon.
-      '''
-
-      f = self.model_gen()
-      tf = self.env.dt
-      t0 = 0
-      dae = {'x': self.x, 'p': self.u, 'ode': f(self.x, self.u)}
-      opts = {'simplify': True, 'number_of_finite_elements': 4}
-      intg = integrator('intg', 'rk', dae, t0,tf,opts)
-      res = intg(x0=self.x, p=self.u)
-      x_next = res['xf']
-      F = Function('F',[self.x,self.u],[x_next],['x','u'],['x_next'])
-      return F
-    
     def disturbance_index(self):
-      
-      '''
-      Generates the indices of when the disturbance or setpoint value changes.
-      
-      Inputs: self
-
-      Returns: index of when either the disturbance or setpoint value changes.
-      
-      '''
-
-      index = []
-      if self.env_params.get('disturbances') is not None:
-        for key in self.env_params['disturbances']:
-          disturbance = self.env_params['disturbances'][key]
-          for i in range(disturbance.shape[0]-1):
-            if disturbance[i] != disturbance[i+1]:
-              index.append(i+1)
-      for key in self.env_params['SP']:
-        SP = self.env_params['SP'][key]
-        for i in range(len(SP)-1):
-          if SP[i] != SP[i+1]:
-            index.append(i+1)
-      
-      index = list(set(index))
-      return index
-       
-    def ocp(self,t_step):
-      """
-      Solves an optimal control problem (OCP) using the IPOPT solver.
-
-      Returns:
-      - M: A function that takes current state x_0 (p) and returns the optimal control input u.
-
-      """
-
-      opti = Opti()
-      F = self.integrator_gen()
-      x = opti.variable(self.env.Nx_oracle, self.N+1)
-      u = opti.variable(self.env.Nu, self.N)       
-      p = opti.parameter(self.env.Nx_oracle, 1)
-      setpoint = opti.parameter(len(self.env_params['SP']), self.N+1)
-    
-      # Cost function sum of squared error plus control penalty. 
-      # Both states and controls are normalised to errors equally
-      cost = 0
-      Sp_i = 0
-      for k in self.env_params['SP']:
-        
-        i  = self.model_info['states'].index(k)
-
-        o_space_low = self.env_params['o_space']['low'][i]*np.ones((1,self.N+1))
-        o_space_high = self.env_params['o_space']['high'][i]*np.ones((1,self.N+1))
-        x_normalized = (x[i,:] - o_space_low) / (o_space_high- o_space_low)
-        setpoint_normalized = (setpoint[Sp_i,:] - o_space_low ) / (o_space_high- o_space_low)
-       
-        r_scale = self.env_params.get('r_scale', {}) # if no r_scale: set r_scale to 1
-        cost += sum1(sum2((x_normalized - setpoint_normalized)**2))*r_scale.get(k, 1)
-        Sp_i += 1
-      u_normalized = (u - self.env_params['a_space']['low']) / (self.env_params['a_space']['high'] - self.env_params['a_space']['low'])
-
-      # Add the control cost
-      cost += self.R*sum1(sum2(u_normalized**2))
-
-      opti.minimize(cost)
-
-      # Dynamics
-      for k in range(self.N):
-        opti.subject_to(x[:, k+1] == F(x[:, k], u[:, k]))
-      
-      # Control constraints
-     
-      for i in range(self.env.Nu - self.env.Nd_model):
-        opti.subject_to(u[i,:] >= self.env_params['a_space']['low'][i])
-        opti.subject_to(u[i,:] <= self.env_params['a_space']['high'][i])
-      
-      # Define disturbance as a control input equality constraint
-      # TODO: Add an option to foresee any disturbance.
-      if self.env_params.get('disturbances') is not None:
-        for i, k in enumerate(self.env.model.info()['disturbances'], start=0):
-          if k in self.env.disturbances.keys():
-            opti.subject_to(u[self.env.Nu-len(self.env.model.info()['disturbances'])+i,:] == self.env.disturbances[k][t_step]) # Add disturbance to control vector
-            opti.set_initial(u[self.env.Nu-len(self.env.model.info()['disturbances'])+i,:], self.env.disturbances[k][t_step])
-          else:
-            opti.subject_to(u[self.env.Nu-len(self.env.model.info()['disturbances'])+i,:] == self.model_info['parameters'][str(k)]) # if there is no disturbance at this timestep, use the default value
-            opti.set_initial(u[self.env.Nu-len(self.env.model.info()['disturbances'])+i,:], self.model_info['parameters'][str(k)])
-      
-      # Initial condition
-      opti.subject_to(x[:, 0] == p )
-      
-      # Add user-defined constraint
-      if self.env_params.get('constraints') is not None:
-        for k in self.env_params['constraints']:
-          for j in range(len(k)):
-            if self.env_params['cons_type'][k][j] == '<=':
-              opti.subject_to(x[self.model_info['states'].index(k),:] <= self.env_params['constraints'][k][j])
-            elif self.env_params['cons_type'][k][j] == '>=':
-              opti.subject_to(x[self.model_info['states'].index(k),:] >= self.env_params['constraints'][k][j])
-            else:
-              raise ValueError('Invalid constraint type')
-      
-      # Define the setpoint for the cost function
-      SP_i = np.fromiter({k: v[t_step] for k, v in self.env_params['SP'].items()}.values(),dtype=float)
-      setpoint_value = SP_i*np.ones((self.N+1,1))  
-      opti.set_value(setpoint, setpoint_value.T)
-      
-      # Initial values
-      opti.set_value(p, self.x0[:self.env.Nx_oracle])
-      initial_x_values = np.zeros((self.env.Nx_oracle, self.N+1))
-      initial_x_values = (self.x0[:self.env.Nx_oracle]*np.ones((self.N+1,self.env.Nx_oracle))).T  
-      opti.set_initial(x, initial_x_values)
-      for i in range(self.env.Nu - self.env.Nd_model):     
-        opti.set_initial(u[i,:], self.env_params['a_space']['low'][i]*np.ones((1,self.N))) 
-     
-      # Silence the solver
-      opts = {
-      'ipopt.print_level': 0,
-      'ipopt.sb': 'no',
-      'print_time': 0,
-      'ipopt.print_user_options': 'no',
-
-      }
-
-      opti.solver('ipopt', opts)
-
-      # Make the opti object a function 
-      M = opti.to_function('M', [p], [u[:,1]], ['p'], ['u'])
-      return M
-    
-    def mpc(self):
-      '''
-      Solves a model predictive control problem (MPC) using the optimal control problem (OCP) solver.
+        """
+        Generates the indices of when the disturbance or setpoint value changes.
 
-      Returns:
-      - x_opt: Optimal state trajectory
-      - u_opt: Optimal control trajectory
-      '''
-      
-      regen_index = self.disturbance_index()
-      
-      M = self.ocp(t_step=0)
-      F = self.integrator_gen()
-      
-      u_log = np.zeros((self.env.Nu, self.env.N))
-      x_log = np.zeros((self.env.Nx_oracle, self.env.N))
-      x = np.array(self.x0[:self.env.Nx_oracle])
-      for i in range(self.env.N):
-          if i-1 in regen_index:
-            M = self.ocp(t_step=i)          
-          try:
-              x_log[:,i] = x
-          except Exception:
-              x_log[:,i] = x.reshape(-1)
-
-          if self.env_params.get('noise', False):
-              noise_percentage = self.env_params.get('noise_percentage', 0)
-              try:
-                x += np.random.normal(0,1,(self.env.Nx_oracle)) * x * noise_percentage
-
-              except Exception:
-
-                x += np.random.normal(0,1,(self.env.Nx_oracle,1)) * x * noise_percentage
-          u = M(x).full()
-          u_log[:,i] = u[0]
-          x = F(x,u).full() 
-      return x_log, u_log
+        Inputs: self
+
+        Returns: index of when either the disturbance or setpoint value changes.
+
+        """
+
+        index = []
+        if self.env_params.get("disturbances") is not None:
+            for key in self.env_params["disturbances"]:
+                disturbance = self.env_params["disturbances"][key]
+                for i in range(disturbance.shape[0] - 1):
+                    if disturbance[i] != disturbance[i + 1]:
+                        index.append(i + 1)
+        for key in self.env_params["SP"]:
+            SP = self.env_params["SP"][key]
+            for i in range(len(SP) - 1):
+                if SP[i] != SP[i + 1]:
+                    index.append(i + 1)
+
+        index = list(set(index))
+        return index
+
+    def ocp(self, t_step):
+        """
+        Solves an optimal control problem (OCP) using the IPOPT solver.
+
+        Returns:
+        - M: A function that takes current state x_0 (p) and returns the optimal control input u.
+
+        """
+
+        opti = Opti()
+        F = self.integrator_gen()
+        x = opti.variable(self.env.Nx_oracle, self.N + 1)
+        u = opti.variable(self.env.Nu, self.N)
+        p = opti.parameter(self.env.Nx_oracle, 1)
+        setpoint = opti.parameter(len(self.env_params["SP"]), self.N + 1)
+
+        # Cost function sum of squared error plus control penalty.
+        # Both states and controls are normalised to errors equally
+        cost = 0
+        Sp_i = 0
+        for k in self.env_params["SP"]:
+            i = self.model_info["states"].index(k)
+
+            o_space_low = self.env_params["o_space"]["low"][i] * np.ones(
+                (1, self.N + 1)
+            )
+            o_space_high = self.env_params["o_space"]["high"][i] * np.ones(
+                (1, self.N + 1)
+            )
+            x_normalized = (x[i, :] - o_space_low) / (o_space_high - o_space_low)
+            setpoint_normalized = (setpoint[Sp_i, :] - o_space_low) / (
+                o_space_high - o_space_low
+            )
+
+            r_scale = self.env_params.get(
+                "r_scale", {}
+            )  # if no r_scale: set r_scale to 1
+            cost += sum1(sum2((x_normalized - setpoint_normalized) ** 2)) * r_scale.get(
+                k, 1
+            )
+            Sp_i += 1
+        u_normalized = (u - self.env_params["a_space"]["low"]) / (
+            self.env_params["a_space"]["high"] - self.env_params["a_space"]["low"]
+        )
+
+        # Add the control cost
+        cost += self.R * sum1(sum2(u_normalized**2))
+
+        opti.minimize(cost)
+
+        # Dynamics
+        for k in range(self.N):
+            opti.subject_to(x[:, k + 1] == F(x[:, k], u[:, k]))
+
+        # Control constraints
+
+        for i in range(self.env.Nu - self.env.Nd_model):
+            opti.subject_to(u[i, :] >= self.env_params["a_space"]["low"][i])
+            opti.subject_to(u[i, :] <= self.env_params["a_space"]["high"][i])
+
+        # Define disturbance as a control input equality constraint
+        # TODO: Add an option to foresee any disturbance.
+        if self.env_params.get("disturbances") is not None:
+            for i, k in enumerate(self.env.model.info()["disturbances"], start=0):
+                if k in self.env.disturbances.keys():
+                    opti.subject_to(
+                        u[
+                            self.env.Nu
+                            - len(self.env.model.info()["disturbances"])
+                            + i,
+                            :,
+                        ]
+                        == self.env.disturbances[k][t_step]
+                    )  # Add disturbance to control vector
+                    opti.set_initial(
+                        u[
+                            self.env.Nu
+                            - len(self.env.model.info()["disturbances"])
+                            + i,
+                            :,
+                        ],
+                        self.env.disturbances[k][t_step],
+                    )
+                else:
+                    opti.subject_to(
+                        u[
+                            self.env.Nu
+                            - len(self.env.model.info()["disturbances"])
+                            + i,
+                            :,
+                        ]
+                        == self.model_info["parameters"][str(k)]
+                    )  # if there is no disturbance at this timestep, use the default value
+                    opti.set_initial(
+                        u[
+                            self.env.Nu
+                            - len(self.env.model.info()["disturbances"])
+                            + i,
+                            :,
+                        ],
+                        self.model_info["parameters"][str(k)],
+                    )
+
+        # Initial condition
+        opti.subject_to(x[:, 0] == p)
+
+        # Add user-defined constraint
+        if self.env_params.get("constraints") is not None:
+            for k in self.env_params["constraints"]:
+                for j in range(len(k)):
+                    if self.env_params["cons_type"][k][j] == "<=":
+                        opti.subject_to(
+                            x[self.model_info["states"].index(k), :]
+                            <= self.env_params["constraints"][k][j]
+                        )
+                    elif self.env_params["cons_type"][k][j] == ">=":
+                        opti.subject_to(
+                            x[self.model_info["states"].index(k), :]
+                            >= self.env_params["constraints"][k][j]
+                        )
+                    else:
+                        raise ValueError("Invalid constraint type")
+
+        # Define the setpoint for the cost function
+        SP_i = np.fromiter(
+            {k: v[t_step] for k, v in self.env_params["SP"].items()}.values(),
+            dtype=float,
+        )
+        setpoint_value = SP_i * np.ones((self.N + 1, 1))
+        opti.set_value(setpoint, setpoint_value.T)
+
+        # Initial values
+        opti.set_value(p, self.x0[: self.env.Nx_oracle])
+        initial_x_values = np.zeros((self.env.Nx_oracle, self.N + 1))
+        initial_x_values = (
+            self.x0[: self.env.Nx_oracle] * np.ones((self.N + 1, self.env.Nx_oracle))
+        ).T
+        opti.set_initial(x, initial_x_values)
+        for i in range(self.env.Nu - self.env.Nd_model):
+            opti.set_initial(
+                u[i, :], self.env_params["a_space"]["low"][i] * np.ones((1, self.N))
+            )
+
+        # Silence the solver
+        opts = {
+            "ipopt.print_level": 0,
+            "ipopt.sb": "no",
+            "print_time": 0,
+            "ipopt.print_user_options": "no",
+        }
+
+        opti.solver("ipopt", opts)
+
+        # Make the opti object a function
+        M = opti.to_function("M", [p], [u[:, 1]], ["p"], ["u"])
+        return M
+
+    def mpc(self):
+        """
+        Solves a model predictive control problem (MPC) using the optimal control problem (OCP) solver.
 
+        Returns:
+        - x_opt: Optimal state trajectory
+        - u_opt: Optimal control trajectory
+        """
+
+        regen_index = self.disturbance_index()
+
+        M = self.ocp(t_step=0)
+        F = self.integrator_gen()
+
+        u_log = np.zeros((self.env.Nu, self.env.N))
+        x_log = np.zeros((self.env.Nx_oracle, self.env.N))
+        x = np.array(self.x0[: self.env.Nx_oracle])
+        for i in range(self.env.N):
+            if i - 1 in regen_index:
+                M = self.ocp(t_step=i)
+            try:
+                x_log[:, i] = x
+            except Exception:
+                x_log[:, i] = x.reshape(-1)
+
+            if self.env_params.get("noise", False):
+                noise_percentage = self.env_params.get("noise_percentage", 0)
+                try:
+                    x += (
+                        np.random.normal(0, 1, (self.env.Nx_oracle))
+                        * x
+                        * noise_percentage
+                    )
+
+                except Exception:
+                    x += (
+                        np.random.normal(0, 1, (self.env.Nx_oracle, 1))
+                        * x
+                        * noise_percentage
+                    )
+            u = M(x).full()
+            u_log[:, i] = u[0]
+            x = F(x, u).full()
+        return x_log, u_log
```

### Comparing `pcgym-0.0.9/src/pcgym/pcgym.py` & `pcgym-0.1.0/src/pcgym/pcgym.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,165 +1,197 @@
 import numpy as np
 import gymnasium as gym
 from gymnasium import spaces
-from pcgym.model_classes import cstr_ode, first_order_system_ode, multistage_extraction_ode, nonsmooth_control_ode
-from pcgym.policy_evaluation import policy_eval
-from pcgym.integrator import integration_engine
-import copy 
-    
+from pcgym.model_classes import (
+    cstr_ode,
+    first_order_system_ode,
+    multistage_extraction_ode,
+    nonsmooth_control_ode,
+)
+from pcgym.Policy_Evaluation import policy_eval
+from pcgym.Integrator import integration_engine
+import copy
+
+
 class make_env(gym.Env):
-    '''
+    """
     Class for RL-Gym Environment
-    '''
-    def __init__(self,env_params):
-        '''
+    """
+
+    def __init__(self, env_params):
+        """
         Constructor for the class
-        '''
-        
+        """
+
         self.env_params = copy.deepcopy(env_params)
         try:
-            self.normalise_a = env_params['normalise_a']
-            self.normalise_o = env_params['normalise_o']
+            self.normalise_a = env_params["normalise_a"]
+            self.normalise_o = env_params["normalise_o"]
         except Exception:
             self.normalise_a = True
             self.normalise_o = True
-        
+
         # Define action and observation space
         if self.normalise_a is True:
-            self.action_space = spaces.Box(low = np.array([-1]*env_params['a_space']['low'].shape[0]), high = np.array([1]*env_params['a_space']['high'].shape[0]))
+            self.action_space = spaces.Box(
+                low=np.array([-1] * env_params["a_space"]["low"].shape[0]),
+                high=np.array([1] * env_params["a_space"]["high"].shape[0]),
+            )
         else:
-            self.action_space = spaces.Box(low=env_params['a_space']['low'],high = env_params['a_space']['high'])
-            
-        self.SP = env_params['SP']
-        self.N = env_params['N']
-        self.tsim = env_params['tsim']
-        self.x0 = env_params['x0']
+            self.action_space = spaces.Box(
+                low=env_params["a_space"]["low"], high=env_params["a_space"]["high"]
+            )
+
+        self.SP = env_params["SP"]
+        self.N = env_params["N"]
+        self.tsim = env_params["tsim"]
+        self.x0 = env_params["x0"]
         # Initial setup for observation space based on user-defined bounds
-        base_obs_low = env_params['o_space']['low']
-        base_obs_high = env_params['o_space']['high']
-        self.observation_space = spaces.Box(low=base_obs_low, high=base_obs_high)
+        base_obs_low = env_params["o_space"]["low"]
+        base_obs_high = env_params["o_space"]["high"]
+        self.observation_space_base = spaces.Box(low=base_obs_low, high=base_obs_high)
+
+        if self.normalise_o:
+            self.observation_space = spaces.Box(
+                low=np.array([-1] * base_obs_low.shape[0]),
+                high=np.array([1] * base_obs_high.shape[0]),
+            )
+        else:
+            self.observation_space = spaces.Box(low=base_obs_low, high=base_obs_high)
 
-        try :
-            self.integration_method = env_params['integration_method']
+        try:
+            self.integration_method = env_params["integration_method"]
         except Exception:
-            self.integration_method = 'casadi'
+            self.integration_method = "casadi"
 
-        self.dt =  self.tsim/self.N
+        self.dt = self.tsim / self.N
         self.done = False
 
-        
-
         # Constraints
         self.constraint_active = False
         self.r_penalty = False
         self.info = {}
 
         self.custom_constraint_active = False  # Initialize to False by default
-        
-        if env_params.get('constraints') is not None:
-            self.constraints = env_params['constraints']
-            self.done_on_constraint = env_params['done_on_cons_vio']
-            self.r_penalty = env_params['r_penalty']
-            self.cons_type = env_params['cons_type']
+
+        if env_params.get("constraints") is not None:
+            self.constraints = env_params["constraints"]
+            self.done_on_constraint = env_params["done_on_cons_vio"]
+            self.r_penalty = env_params["r_penalty"]
+            self.cons_type = env_params["cons_type"]
             self.constraint_active = True
             self.n_con = 0
             for _, con_list in self.constraints.items():
                 self.n_con += len(con_list)
-            self.info['cons_info'] = np.zeros((self.n_con,self.N,1))
+            self.info["cons_info"] = np.zeros((self.n_con, self.N, 1))
 
-        if env_params.get('custom_con') is not None:
-            self.done_on_constraint = env_params['done_on_cons_vio']
-            self.r_penalty = env_params['r_penalty']
+        if env_params.get("custom_con") is not None:
+            self.done_on_constraint = env_params["done_on_cons_vio"]
+            self.r_penalty = env_params["r_penalty"]
             self.custom_constraint_active = True
 
-    
-
-        #Select model 
+        # Select model
         model_mapping = {
-        'cstr_ode': cstr_ode,
-        'first_order_system_ode': first_order_system_ode,
-        'nonsmooth_control_ode': nonsmooth_control_ode,
-        'multistage_extraction_ode': multistage_extraction_ode,
-        }   
+            "cstr_ode": cstr_ode,
+            "first_order_system_ode": first_order_system_ode,
+            "nonsmooth_control_ode": nonsmooth_control_ode,
+            "multistage_extraction_ode": multistage_extraction_ode,
+        }
 
         # Load custom model if it is provide else load the selected standard model.
-        if self.env_params.get('custom_model') is not None:
-            m = self.env_params.get('custom_model')
+        if self.env_params.get("custom_model") is not None:
+            m = self.env_params.get("custom_model")
         else:
-            m = model_mapping.get(env_params['model'], None)
-        self.model = m(int_method=self.integration_method) # Initialise the model with the selected integration method
-
+            m = model_mapping.get(env_params["model"], None)
+        self.model = m(
+            int_method=self.integration_method
+        )  # Initialise the model with the selected integration method
 
         # Handle the case where the model is not found (do this for all)
         if self.model is None:
-            raise ValueError(f"Model '{env_params['model']}' not found in model_mapping.")
-        
+            raise ValueError(
+                f"Model '{env_params['model']}' not found in model_mapping."
+            )
+
         # Import states and controls from model info
-        self.Nx = len(self.model.info()['states']) + len(self.SP)
-        self.Nx_oracle = len(self.model.info()['states'])
-        self.Nu = len(self.model.info()['inputs'])
+        self.Nx = len(self.model.info()["states"]) + len(self.SP)
+        self.Nx_oracle = len(self.model.info()["states"])
+        self.Nu = len(self.model.info()["inputs"])
 
         # Disturbances
         self.disturbance_active = False
         self.Nd = 0
         self.Nd_model = 0
-        if env_params.get('disturbances') is not None:
+        if env_params.get("disturbances") is not None:
             self.disturbance_active = True
-            self.disturbances = env_params['disturbances']
+            self.disturbances = env_params["disturbances"]
             self.Nd = len(self.disturbances)
-            self.Nd_model = len(self.model.info()['disturbances'])
-            self.Nu += len(self.model.info()['disturbances'])
-        
+            self.Nd_model = len(self.model.info()["disturbances"])
+            self.Nu += len(self.model.info()["disturbances"])
+
             # Extend the state size by the number of disturbances
             self.Nx += self.Nd
             # user has defined disturbance_bounds within env_params
-            disturbance_low = env_params['disturbance_bounds']['low']
-            disturbance_high = env_params['disturbance_bounds']['high']
+            disturbance_low = env_params["disturbance_bounds"]["low"]
+            disturbance_high = env_params["disturbance_bounds"]["high"]
             # Extend the observation space bounds to include disturbances
             extended_obs_low = np.concatenate((base_obs_low, disturbance_low))
             extended_obs_high = np.concatenate((base_obs_high, disturbance_high))
             # Define the extended observation space
-            self.observation_space = spaces.Box(low=extended_obs_low, high=extended_obs_high, dtype=np.float32)
-          
-        
-        
+            self.observation_space_base = spaces.Box(
+                low=extended_obs_low, high=extended_obs_high, dtype=np.float32
+            )
+            if self.normalise_o:
+                self.observation_space = spaces.Box(
+                    low=np.array([-1] * extended_obs_low.shape[0]),
+                    high=np.array([1] * extended_obs_high.shape[0]),
+                )
+            else:
+                self.observation_space = spaces.Box(
+                    low=extended_obs_low, high=extended_obs_high, dtype=np.float32
+                )
+
     def reset(self, seed=None, **kwargs):  # Accept arbitrary keyword arguments
         """
-        Resets the state of the system 
+        Resets the state of the system
 
         Returns the state of the system
         """
         self.t = 0
-        self.int_eng = integration_engine(make_env,self.env_params)
-        
-        state = copy.deepcopy(self.env_params['x0'])
-        
+        self.int_eng = integration_engine(make_env, self.env_params)
+
+        state = copy.deepcopy(self.env_params["x0"])
+
         # If disturbances are active, expand the initial state with disturbances
         if self.disturbance_active:
-            initial_disturbances = [] 
-            for k in self.model.info()['disturbances']:
+            initial_disturbances = []
+            for k in self.model.info()["disturbances"]:
                 if k in self.disturbances:
                     initial_disturbances.append(self.disturbances[k][0])
-              
-            
+
             # Append initial disturbances to the state
             state = np.concatenate((state, initial_disturbances))
 
         self.state = state
 
-        r_init = self.reward_fn(state,False)
+        r_init = self.reward_fn(state, False)
 
         self.done = False
 
         if self.normalise_o is True:
-            self.normstate = 2 * (self.state - self.observation_space.low) / (self.observation_space.high - self.observation_space.low) - 1
-            return self.normstate, {'r_init':r_init}
+            self.normstate = (
+                2
+                * (self.state - self.observation_space_base.low)
+                / (self.observation_space_base.high - self.observation_space_base.low)
+                - 1
+            )
+            return self.normstate, {"r_init": r_init}
         else:
-            return self.state,{'r_init':r_init}
-    
+            return self.state, {"r_init": r_init}
+
     def step(self, action):
         """
         Simulate one timestep of the environment
 
         Parameters
         ----------
         action : action taken by agent
@@ -172,200 +204,242 @@
         rew : float
             reward obtained
         done : {0,1}
             0 if target not reached. 1 if reached
         info :
 
         """
-        
-        # Create control vector 
+
+        # Create control vector
         uk = np.zeros(self.Nu)
         if self.normalise_a is True:
-            action = (action + 1)*(self.env_params['a_space']['high'] - self.env_params['a_space']['low'])/2 + self.env_params['a_space']['low']
-        
+            action = (action + 1) * (
+                self.env_params["a_space"]["high"] - self.env_params["a_space"]["low"]
+            ) / 2 + self.env_params["a_space"]["low"]
+
         # Add disturbance to control vector
         if self.disturbance_active:
-            uk[:self.Nu-len(self.model.info()['disturbances'])] = action # Add action to control vector
+            uk[: self.Nu - len(self.model.info()["disturbances"])] = (
+                action  # Add action to control vector
+            )
             disturbance_values = []
             disturbance_values_state = []
-            for i, k in enumerate(self.model.info()['disturbances'], start=0):     
+            for i, k in enumerate(self.model.info()["disturbances"], start=0):
                 if k in self.disturbances:
                     current_disturbance_value = self.disturbances[k][self.t]
-                    uk[self.Nu-self.Nd_model+i] = self.disturbances[k][self.t] # Add disturbance to control vector
+                    uk[self.Nu - self.Nd_model + i] = self.disturbances[k][
+                        self.t
+                    ]  # Add disturbance to control vector
                     disturbance_values_state.append(current_disturbance_value)
                     disturbance_values.append(current_disturbance_value)
                 else:
-                    default_value = self.model.info()['parameters'][str(k)]
-                    uk[self.Nu-self.Nd_model+i] = self.model.info()['parameters'][str(k)] # if there is no disturbance at this timestep, use the default value
+                    default_value = self.model.info()["parameters"][str(k)]
+                    uk[self.Nu - self.Nd_model + i] = self.model.info()["parameters"][
+                        str(k)
+                    ]  # if there is no disturbance at this timestep, use the default value
                     disturbance_values.append(default_value)
-      
+
             # Update the state vector with current disturbance values
-            self.state[self.Nx_oracle+len(self.SP):] = disturbance_values_state
+            self.state[self.Nx_oracle + len(self.SP) :] = disturbance_values_state
         else:
             uk = action  # Add action to control vector
-
         # Simulate one timestep
-        if self.integration_method == 'casadi':
-            Fk = self.int_eng.casadi_step(self.state,uk)
-            self.state[:self.Nx_oracle] = np.array(Fk['xf'].full()).reshape(self.Nx_oracle)
-        elif self.integration_method == 'jax':
-            self.state[:self.Nx_oracle] = self.int_eng.jax_step(self.state,uk)
+        if self.integration_method == "casadi":
+            Fk = self.int_eng.casadi_step(self.state, uk)
+            self.state[: self.Nx_oracle] = np.array(Fk["xf"].full()).reshape(
+                self.Nx_oracle
+            )
+        elif self.integration_method == "jax":
+            self.state[: self.Nx_oracle] = self.int_eng.jax_step(self.state, uk)
 
         # Check if constraints are violated
         constraint_violated = False
         if self.constraint_active or self.custom_constraint_active:
-            constraint_violated = self.constraint_check(self.state,uk)
-        
+            constraint_violated = self.constraint_check(self.state, uk)
+
         # Compute reward
         rew = self.reward_fn(self.state, constraint_violated)
-        
+
         # For each set point, if it exists, append its value at the current time step to the list
         SP_t = []
         for k in self.SP.keys():
             if k in self.SP:
-                SP_t.append(self.SP[k][self.t]) 
-        self.state[self.Nx:] = np.array(SP_t)   
-                
-       
+                SP_t.append(self.SP[k][self.t])
+        self.state[self.Nx_oracle :] = np.array(SP_t)
         # Update timestep
         self.t += 1
-    
+
         if self.t == self.N:
             self.done = True
-      
-        # add noise to state
-        if self.env_params.get('noise', False):
-            noise_percentage = self.env_params.get('noise_percentage', 0)
-            self.state[:self.Nx_oracle] += np.random.normal(0, 1, self.Nx_oracle) * self.state[:self.Nx_oracle] * noise_percentage
 
+        # add noise to state
+        if self.env_params.get("noise", False):
+            noise_percentage = self.env_params.get("noise_percentage", 0)
+            self.state[: self.Nx_oracle] += (
+                np.random.normal(0, 1, self.Nx_oracle)
+                * self.state[: self.Nx_oracle]
+                * noise_percentage
+            )
 
         if self.normalise_o is True:
-            self.normstate = 2 * (self.state - self.observation_space.low) / (self.observation_space.high - self.observation_space.low) - 1
+            self.normstate = (
+                2
+                * (self.state - self.observation_space_base.low)
+                / (self.observation_space_base.high - self.observation_space_base.low)
+                - 1
+            )
             return self.normstate, rew, self.done, False, self.info
         else:
             return self.state, rew, self.done, False, self.info
-    
-    def reward_fn(self, state,c_violated):
+
+    def reward_fn(self, state, c_violated):
         """
         Compute reward for one timestep and penalise constraint violation if requested by the user.
 
         Inputs:
             state - current state of the system
             c_violated - boolean indicating if constraint is violated
         Outputs:
             r - reward for current timestep
 
         """
 
-        r = 0.
+        r = 0.0
 
         for k in self.SP:
-            i = self.model.info()['states'].index(k)
-            r_scale = self.env_params.get('r_scale', {})
-            r +=  (-((state[i] - np.array(self.SP[k][self.t]))**2))*r_scale.get(k, 1)
+            i = self.model.info()["states"].index(k)
+            r_scale = self.env_params.get("r_scale", {})
+            r += (-((state[i] - np.array(self.SP[k][self.t])) ** 2)) * r_scale.get(k, 1)
             if self.r_penalty and c_violated:
                 r -= 1000
         return r
-    
+
     def con_checker(self, model_states, curr_state):
         """
         Check constraints for given model_states and their values.
 
         Parameters:
         model_states (list): A list of model_states (states or inputs).
         curr_state (list): A list of corresponding item values.
 
         Returns:
         bool: True if any constraint is violated, False otherwise.
         """
         for i, state in enumerate(model_states):
             if state in self.constraints:
-                constraint = self.constraints[state] # List of constraints
-                cons_type = self.cons_type[state] # List of cons type
+                constraint = self.constraints[state]  # List of constraints
+                cons_type = self.cons_type[state]  # List of cons type
                 for j in range(len(constraint)):
                     curr_state_i = curr_state[i]
-                    is_greater_violated = cons_type[j] == '>=' and curr_state_i <= constraint[j]
-                    is_less_violated = cons_type[j] == '<=' and curr_state_i >= constraint[j]
+                    is_greater_violated = (
+                        cons_type[j] == ">=" and curr_state_i <= constraint[j]
+                    )
+                    is_less_violated = (
+                        cons_type[j] == "<=" and curr_state_i >= constraint[j]
+                    )
 
                     if is_greater_violated or is_less_violated:
-                        self.info['cons_info'][self.con_i, self.t, :] = abs(curr_state_i - constraint[j])
+                        self.info["cons_info"][self.con_i, self.t, :] = abs(
+                            curr_state_i - constraint[j]
+                        )
                         return True
-                    self.con_i += 1 
+                    self.con_i += 1
         return False
-    
 
-    def constraint_check(self,state,input):
+    def constraint_check(self, state, input):
         """
         Check if constraints are violated and update info array accordingly.
 
         Inputs: state - current state of the system
 
         Outputs: constraint_violated - boolean indicating if constraint is violated
         """
         self.con_i = 0
         constraint_violated = False
-        states = self.model.info()['states']
-        inputs = self.model.info()['inputs']
-        if self.env_params.get('custom_con') is not None:
-            custom_con_vio_f = self.env_params['custom_con']
-            custom_con_vio = custom_con_vio_f(state,input) # User defined constraint return True if violated
-            assert isinstance(custom_con_vio, bool), "Custom constraint must return a boolean (True == Violated)"
+        states = self.model.info()["states"]
+        inputs = self.model.info()["inputs"]
+        if self.env_params.get("custom_con") is not None:
+            custom_con_vio_f = self.env_params["custom_con"]
+            custom_con_vio = custom_con_vio_f(
+                state, input
+            )  # User defined constraint return True if violated
+            assert isinstance(
+                custom_con_vio, bool
+            ), "Custom constraint must return a boolean (True == Violated)"
         else:
             custom_con_vio = False
 
         if self.constraint_active and self.custom_constraint_active:
-            constraint_violated = self.con_checker(states, state) or self.con_checker(inputs, input) or False # Check both inputs and states
+            constraint_violated = (
+                self.con_checker(states, state)
+                or self.con_checker(inputs, input)
+                or False
+            )  # Check both inputs and states
         elif self.constraint_active:
-            constraint_violated = self.con_checker(states, state) or self.con_checker(inputs, input) or False # Check both inputs and states
+            constraint_violated = (
+                self.con_checker(states, state)
+                or self.con_checker(inputs, input)
+                or False
+            )  # Check both inputs and states
         elif self.custom_constraint_active:
             constraint_violated = custom_con_vio
 
-        self.done = self.done_on_constraint 
+        self.done = self.done_on_constraint
         return constraint_violated
-            
-              
-    def get_rollouts(self, policies, reps, oracle = False, dist_reward = False, MPC_params = False, cons_viol = False):
-        '''
+
+    def get_rollouts(
+        self,
+        policies,
+        reps,
+        oracle=False,
+        dist_reward=False,
+        MPC_params=False,
+        cons_viol=False,
+    ):
+        """
         Plot the rollout of the given policy.
 
         Parameters:
         - policies: dictionary of policies to evaluate
         - reps: The number of rollouts to perform.
         - oracle: Whether to use an oracle model for evaluation. Default is False.
         - dist_reward: Whether to use reward distribution for plotting. Default is False.
         - MPC_params: Whether to use MPC parameters. Default is False.
-        '''
+        """
         # construct evaluator
-        evaluator = policy_eval(make_env, policies, reps, self.env_params, oracle, MPC_params)
-        # generate rollouts 
+        evaluator = policy_eval(
+            make_env, policies, reps, self.env_params, oracle, MPC_params
+        )
+        # generate rollouts
         data = evaluator.get_rollouts()
         # return evaluator and data
         return evaluator, data
 
-
-    def plot_rollout(self, policies, reps, oracle = False, dist_reward = False, MPC_params = False, cons_viol = False):
-        '''
+    def plot_rollout(
+        self,
+        policies,
+        reps,
+        oracle=False,
+        dist_reward=False,
+        MPC_params=False,
+        cons_viol=False,
+    ):
+        """
         Plot the rollout of the given policy.
 
         Parameters:
         - policies: dictionary of policies to evaluate
         - reps: The number of rollouts to perform.
         - oracle: Whether to use an oracle model for evaluation. Default is False.
         - dist_reward: Whether to use reward distribution for plotting. Default is False.
         - MPC_params: Whether to use MPC parameters. Default is False.
-        '''
+        """
         # construct evaluator
-        evaluator = policy_eval(make_env, policies, reps, self.env_params, oracle, MPC_params, cons_viol)
-        # generate rollouts 
+        evaluator = policy_eval(
+            make_env, policies, reps, self.env_params, oracle, MPC_params, cons_viol
+        )
+        # generate rollouts
         data = evaluator.get_rollouts()
         # plot data from rollouts via the evaluator method
         evaluator.plot_data(data, dist_reward)
         # return constructed evaluator and data
         return evaluator, data
-        
-
-    
-
-
-
-
-
```

### Comparing `pcgym-0.0.9/src/pcgym/policy_evaluation.py` & `pcgym-0.1.0/src/pcgym/policy_evaluation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,223 +1,332 @@
 # Policy Evaluation Class for pc-gym
 import numpy as np
 import matplotlib.pyplot as plt
-from .oracle import oracle
+from oracle import oracle
 
-class policy_eval():
-    '''
+
+class policy_eval:
+    """
     Policy Evaluation Class
 
     Inputs: Environment, policy and number of policy repitions
 
     Outputs: Plots of states/control/constraints/setpoints (complete),
              return distribution (incomplete), expected return (incomplete),
              oracle trajectories (incomplete) and lower confidence bounds (incomplete)
-    '''
-    def __init__(self,make_env,policies,reps,env_params, oracle = False, MPC_params = False, cons_viol = False):
+    """
+
+    def __init__(
+        self,
+        make_env,
+        policies,
+        reps,
+        env_params,
+        oracle=False,
+        MPC_params=False,
+        cons_viol=False,
+    ):
         self.make_env = make_env
         self.env_params = env_params
         self.env = make_env(env_params)
         self.policies = policies
         self.n_pi = len(policies)
         self.reps = reps
         self.oracle = oracle
         self.cons_viol = cons_viol
- 
-        self.MPC_params  = MPC_params  
-        
 
-    def rollout(self,policy_i):
-        '''
+        self.MPC_params = MPC_params
+
+    def rollout(self, policy_i):
+        """
         Rollout the policy for N steps and return the total reward, states and actions
 
         Input:
             policy - policy to be rolled out
 
         Outputs:
             total_reward - total reward obtained
             states - states obtained from rollout
             actions - actions obtained from rollout
 
-        '''
-        
+        """
+
         total_reward = 0
         s_rollout = np.zeros((self.env.Nx, self.env.N))
-        actions = np.zeros((self.env.env_params['a_space']['low'].shape[0], self.env.N))
-        
+        actions = np.zeros((self.env.env_params["a_space"]["low"].shape[0], self.env.N))
+
         o, r = self.env.reset()
-        total_reward = r['r_init']
-        s_rollout[:,0] = (o + 1)*(self.env.observation_space.high - self.env.observation_space.low)/2 + self.env.observation_space.low
-        for i in range(self.env.N-1):
-            a, _s = policy_i.predict(o, deterministic = True) # Rollout with a deterministic policy
+        total_reward = r["r_init"]
+        s_rollout[:, 0] = (o + 1) * (
+            self.env.observation_space_base.high - self.env.observation_space_base.low
+        ) / 2 + self.env.observation_space_base.low
+        for i in range(self.env.N - 1):
+            a, _s = policy_i.predict(
+                o, deterministic=True
+            )  # Rollout with a deterministic policy
             o, r, term, trunc, info = self.env.step(a)
-            
-            actions[:, i] = (a + 1)*(self.env.env_params['a_space']['high'] - self.env.env_params['a_space']['low'])/2 + self.env.env_params['a_space']['low']
-            s_rollout[:, i+1] = (o + 1)*(self.env.observation_space.high - self.env.observation_space.low)/2 + self.env.observation_space.low
-            
+
+            actions[:, i] = (a + 1) * (
+                self.env.env_params["a_space"]["high"]
+                - self.env.env_params["a_space"]["low"]
+            ) / 2 + self.env.env_params["a_space"]["low"]
+            s_rollout[:, i + 1] = (o + 1) * (
+                self.env.observation_space_base.high
+                - self.env.observation_space_base.low
+            ) / 2 + self.env.observation_space_base.low
+
             total_reward += r
 
         if self.env.constraint_active:
-            cons_info = info['cons_info']
+            cons_info = info["cons_info"]
         else:
-            cons_info = np.zeros((1,self.env.N,1))
-        a, _s = policy_i.predict(o, deterministic = True)
-        actions[:,self.env.N-1] = (a + 1)*(self.env.env_params['a_space']['high'] - self.env.env_params['a_space']['low'])/2 + self.env.env_params['a_space']['low']
-        
-        return total_reward, s_rollout, actions,cons_info
-    
+            cons_info = np.zeros((1, self.env.N, 1))
+        a, _s = policy_i.predict(o, deterministic=True)
+        actions[:, self.env.N - 1] = (a + 1) * (
+            self.env.env_params["a_space"]["high"]
+            - self.env.env_params["a_space"]["low"]
+        ) / 2 + self.env.env_params["a_space"]["low"]
+
+        return total_reward, s_rollout, actions, cons_info
+
     def get_rollouts(self):
-        '''
+        """
         Function to plot the rollout of the policy
 
         Inputs:
             policy - policy to be rolled out
             reps - number of rollouts to be performed
 
         Outputs:
             Plot of states and actions with setpoints and constraints if they exist]
 
-        '''
+        """
         data = {}
-        action_space_shape = self.env.env_params['a_space']['low'].shape[0]
+        action_space_shape = self.env.env_params["a_space"]["low"].shape[0]
         num_states = self.env.Nx
-        
-
 
         # Collect Oracle data
         if self.oracle:
-            r_opt = np.zeros((1,self.reps))
+            r_opt = np.zeros((1, self.reps))
             x_opt = np.zeros((self.env.Nx_oracle, self.env.N, self.reps))
             u_opt = np.zeros((self.env.Nu, self.env.N, self.reps))
-            oracle_instance = oracle(self.make_env, self.env_params,self.MPC_params)
+            oracle_instance = oracle(self.make_env, self.env_params, self.MPC_params)
             for i in range(self.reps):
                 x_opt[:, :, i], u_opt[:, :, i] = oracle_instance.mpc()
                 for k in self.env.SP:
-                    state_i = self.env.model.info()['states'].index(k)
-                    r_scale = self.env_params.get('r_scale', {})
-                    r_opt[:,i] += np.sum((x_opt[state_i,:,i] - self.env.SP[k])**2)*-1*r_scale.get(k, 1)
-            data.update({'oracle': {'r':r_opt,'x':x_opt,'u':u_opt}})   
-           
-      
+                    state_i = self.env.model.info()["states"].index(k)
+                    r_scale = self.env_params.get("r_scale", {})
+                    r_opt[:, i] += (
+                        np.sum((x_opt[state_i, :, i] - self.env.SP[k]) ** 2)
+                        * -1
+                        * r_scale.get(k, 1)
+                    )
+            data.update({"oracle": {"r": r_opt, "x": x_opt, "u": u_opt}})
 
         # Collect RL rollouts for all policies
         for pi_name, pi_i in self.policies.items():
             states = np.zeros((num_states, self.env.N, self.reps))
             actions = np.zeros((action_space_shape, self.env.N, self.reps))
             rew = np.zeros((1, self.reps))
             try:
-                cons_info = np.zeros((self.env.n_con,self.env.N,1,self.reps))
+                cons_info = np.zeros((self.env.n_con, self.env.N, 1, self.reps))
             except Exception:
-                cons_info = np.zeros((1,self.env.N,1,self.reps))
+                cons_info = np.zeros((1, self.env.N, 1, self.reps))
             for r_i in range(self.reps):
-                rew[:, r_i], states[:, :, r_i], actions[:, :, r_i], cons_info[:,:,:,r_i] = self.rollout(pi_i)
-            data.update({pi_name:{'r' :rew,
-                         'x' : states,
-                         'u' : actions}})
+                (
+                    rew[:, r_i],
+                    states[:, :, r_i],
+                    actions[:, :, r_i],
+                    cons_info[:, :, :, r_i],
+                ) = self.rollout(pi_i)
+            data.update({pi_name: {"r": rew, "x": states, "u": actions}})
             if self.env.constraint_active:
-                data[pi_name].update({'g' : cons_info})
+                data[pi_name].update({"g": cons_info})
         self.data = data
         return data
 
-    def plot_data(self, data, reward_dist = False):
+    def plot_data(self, data, reward_dist=False):
         t = np.linspace(0, self.env.tsim, self.env.N)
         len_d = 0
 
         if self.env.disturbance_active:
-            len_d = len(self.env.model.info()['disturbances'])
+            len_d = len(self.env.model.info()["disturbances"])
 
-        col = ['tab:red','tab:purple','tab:olive','tab:gray','tab:cyan']
+        col = ["tab:red", "tab:purple", "tab:olive", "tab:gray", "tab:cyan"]
         if self.n_pi > len(col):
-            raise ValueError(f"Number of policies ({self.n_pi}) is greater than the number of available colors ({len(col)})")
-
+            raise ValueError(
+                f"Number of policies ({self.n_pi}) is greater than the number of available colors ({len(col)})"
+            )
 
-        plt.figure(figsize=(10, 2*(self.env.Nx_oracle+self.env.Nu-self.env.Nd)))
+        plt.figure(figsize=(10, 2 * (self.env.Nx_oracle + self.env.Nu - self.env.Nd)))
         for i in range(self.env.Nx_oracle):
-            plt.subplot(self.env.Nx_oracle + self.env.Nu-self.env.Nd,1,i+1)
+            plt.subplot(self.env.Nx_oracle + self.env.Nu - self.env.Nd, 1, i + 1)
             for ind, (pi_name, pi_i) in enumerate(self.policies.items()):
-                plt.plot(t, np.median(data[pi_name]['x'][i,:,:], axis=1), color=col[ind], lw=3, label = self.env.model.info()['states'][i] + ' (' + pi_name + ')' )
-                plt.gca().fill_between(t, np.min(data[pi_name]['x'][i,:,:], axis=1), np.max(data[pi_name]['x'][i,:,:], axis=1), color=col[ind], alpha=0.2, edgecolor = 'none')
+                plt.plot(
+                    t,
+                    np.median(data[pi_name]["x"][i, :, :], axis=1),
+                    color=col[ind],
+                    lw=3,
+                    label=self.env.model.info()["states"][i] + " (" + pi_name + ")",
+                )
+                plt.gca().fill_between(
+                    t,
+                    np.min(data[pi_name]["x"][i, :, :], axis=1),
+                    np.max(data[pi_name]["x"][i, :, :], axis=1),
+                    color=col[ind],
+                    alpha=0.2,
+                    edgecolor="none",
+                )
             if self.oracle:
-                plt.plot(t, np.median(data['oracle']['x'][i,:,:],axis=1), color='tab:blue', lw=3,label = 'Oracle '+ self.env.model.info()['states'][i])
-                plt.gca().fill_between(t, np.min(data['oracle']['x'][i,:,:],axis=1), np.max(data['oracle']['x'][i,:,:],axis=1), color='tab:blue', alpha=0.2,edgecolor = 'none' )
-            if self.env.model.info()['states'][i] in self.env.SP:
-                plt.step(t, self.env.SP[self.env.model.info()['states'][i]],where = 'post', color = 'black', linestyle = '--', label='Set Point')
+                plt.plot(
+                    t,
+                    np.median(data["oracle"]["x"][i, :, :], axis=1),
+                    color="tab:blue",
+                    lw=3,
+                    label="Oracle " + self.env.model.info()["states"][i],
+                )
+                plt.gca().fill_between(
+                    t,
+                    np.min(data["oracle"]["x"][i, :, :], axis=1),
+                    np.max(data["oracle"]["x"][i, :, :], axis=1),
+                    color="tab:blue",
+                    alpha=0.2,
+                    edgecolor="none",
+                )
+            if self.env.model.info()["states"][i] in self.env.SP:
+                plt.step(
+                    t,
+                    self.env.SP[self.env.model.info()["states"][i]],
+                    where="post",
+                    color="black",
+                    linestyle="--",
+                    label="Set Point",
+                )
             if self.env.constraint_active:
-                if self.env.model.info()['states'][i] in self.env.constraints:
-                    plt.hlines(self.env.constraints[self.env.model.info()['states'][i]], 0, self.env.tsim, color = 'black',label='Constraint')
-            plt.ylabel(self.env.model.info()['states'][i])
-            plt.xlabel('Time (min)')
-            plt.legend(loc='best')
-            plt.grid('True')
+                if self.env.model.info()["states"][i] in self.env.constraints:
+                    plt.hlines(
+                        self.env.constraints[self.env.model.info()["states"][i]],
+                        0,
+                        self.env.tsim,
+                        color="black",
+                        label="Constraint",
+                    )
+            plt.ylabel(self.env.model.info()["states"][i])
+            plt.xlabel("Time (min)")
+            plt.legend(loc="best")
+            plt.grid("True")
             plt.xlim(min(t), max(t))
 
-        for j in range(self.env.Nu-len_d):
-            plt.subplot(self.env.Nx_oracle + self.env.Nu - self.env.Nd, 1, j+self.env.Nx_oracle+1)
+        for j in range(self.env.Nu - len_d):
+            plt.subplot(
+                self.env.Nx_oracle + self.env.Nu - self.env.Nd,
+                1,
+                j + self.env.Nx_oracle + 1,
+            )
             for ind, (pi_name, pi_i) in enumerate(self.policies.items()):
-                plt.step(t, np.median(data[pi_name]['u'][j,:,:], axis=1), color=col[ind], lw=3, label=self.env.model.info()['inputs'][j] + ' (' + pi_name + ')')
+                plt.step(
+                    t,
+                    np.median(data[pi_name]["u"][j, :, :], axis=1),
+                    color=col[ind],
+                    lw=3,
+                    label=self.env.model.info()["inputs"][j] + " (" + pi_name + ")",
+                )
             if self.oracle:
-                plt.step(t, np.median(data['oracle']['u'][j,:,:],axis=1), color='tab:blue', lw=3, label='Oracle '+ str(self.env.model.info()['inputs'][j]))
+                plt.step(
+                    t,
+                    np.median(data["oracle"]["u"][j, :, :], axis=1),
+                    color="tab:blue",
+                    lw=3,
+                    label="Oracle " + str(self.env.model.info()["inputs"][j]),
+                )
             if self.env.constraint_active:
                 for con_i in self.env.constraints:
-                    if self.env.model.info()['inputs'][j] == con_i:
-                        plt.hlines(self.env.constraints[self.env.model.info()['inputs'][j]], 0,self.env.tsim,'black',label='Constraint')
-            plt.ylabel(self.env.model.info()['inputs'][j])
-            plt.xlabel('Time (min)')
-            plt.legend(loc='best')
-            plt.grid('True')
+                    if self.env.model.info()["inputs"][j] == con_i:
+                        plt.hlines(
+                            self.env.constraints[self.env.model.info()["inputs"][j]],
+                            0,
+                            self.env.tsim,
+                            "black",
+                            label="Constraint",
+                        )
+            plt.ylabel(self.env.model.info()["inputs"][j])
+            plt.xlabel("Time (min)")
+            plt.legend(loc="best")
+            plt.grid("True")
             plt.xlim(min(t), max(t))
 
         if self.env.disturbance_active:
             for k in self.env.disturbances.keys():
                 i = 1
                 if self.env.disturbances[k].any() is not None:
-                    plt.subplot(self.env.Nx_oracle+self.env.Nu-self.env.Nd,1,i+j+self.env.Nx_oracle+1)
-                    plt.step(t, self.env.disturbances[k], color = 'tab:orange',label=k)
-                    plt.xlabel('Time (min)')
+                    plt.subplot(
+                        self.env.Nx_oracle + self.env.Nu - self.env.Nd,
+                        1,
+                        i + j + self.env.Nx_oracle + 1,
+                    )
+                    plt.step(t, self.env.disturbances[k], color="tab:orange", label=k)
+                    plt.xlabel("Time (min)")
                     plt.ylabel(k)
                     plt.xlim(min(t), max(t))
-                    i += 1 
+                    i += 1
         plt.tight_layout()
         plt.show()
-        
+
         if self.cons_viol:
             plt.figure(figsize=(12, 3 * self.env.n_con))
             con_i = 0
             for i, con in enumerate(self.env.constraints):
                 for j in range(len(self.env.constraints[str(con)])):
-                    plt.subplot(self.env.n_con,1,con_i+1)
-                    plt.title(f'{con} Constraint')
+                    plt.subplot(self.env.n_con, 1, con_i + 1)
+                    plt.title(f"{con} Constraint")
                     for ind, (pi_name, pi_i) in enumerate(self.policies.items()):
-                        plt.step(t, np.sum(data[pi_name]['g'][con_i,:,:,:],axis=2), color = col[ind], label = f'{con} ({pi_name}) Violation (Sum over Repetitions)')
-                    plt.grid('True')
-                    plt.xlabel('Time (min)')
+                        plt.step(
+                            t,
+                            np.sum(data[pi_name]["g"][con_i, :, :, :], axis=2),
+                            color=col[ind],
+                            label=f"{con} ({pi_name}) Violation (Sum over Repetitions)",
+                        )
+                    plt.grid("True")
+                    plt.xlabel("Time (min)")
                     plt.ylabel(con)
                     plt.xlim(min(t), max(t))
-                    plt.legend(loc = 'best')
+                    plt.legend(loc="best")
                     con_i += 1
             plt.tight_layout()
             plt.show()
 
         if reward_dist:
-            plt.figure(figsize=(12, 8))  
-            plt.grid(True, linestyle='--', alpha=0.6)  
-            all_data = np.concatenate([data[key]['r'].flatten() for key in data.keys()])
+            plt.figure(figsize=(12, 8))
+            plt.grid(True, linestyle="--", alpha=0.6)
+            all_data = np.concatenate([data[key]["r"].flatten() for key in data.keys()])
 
             min_value = np.min(all_data)
             max_value = np.max(all_data)
 
             bins = np.linspace(min_value, max_value, self.reps)
             if self.oracle:
-                plt.hist(data['oracle']['r'].flatten(), bins=bins, color='tab:blue', alpha=0.5, label='Oracle', edgecolor='black')  
+                plt.hist(
+                    data["oracle"]["r"].flatten(),
+                    bins=bins,
+                    color="tab:blue",
+                    alpha=0.5,
+                    label="Oracle",
+                    edgecolor="black",
+                )
             for ind, (pi_name, pi_i) in enumerate(self.policies.items()):
-                plt.hist(data[pi_name]['r'].flatten(), bins=bins, color=col[ind], alpha=0.5, label=pi_name, edgecolor='black')  
-
-            plt.xlabel('Return', fontsize=14)  
-            plt.ylabel('Frequency', fontsize=14)  
-            plt.title('Distribution of Expected Return', fontsize=16)  
-            plt.legend(fontsize=12)  
+                plt.hist(
+                    data[pi_name]["r"].flatten(),
+                    bins=bins,
+                    color=col[ind],
+                    alpha=0.5,
+                    label=pi_name,
+                    edgecolor="black",
+                )
+
+            plt.xlabel("Return", fontsize=14)
+            plt.ylabel("Frequency", fontsize=14)
+            plt.title("Distribution of Expected Return", fontsize=16)
+            plt.legend(fontsize=12)
 
             plt.show()
 
-        return 
-
-    
+        return
```

### Comparing `pcgym-0.0.9/src/pcgym.egg-info/PKG-INFO` & `pcgym-0.1.0/src/pcgym.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcgym
-Version: 0.0.9
+Version: 0.1.0
 Summary: Reinforcement learning suite of process control problems.
 Author-email: Max Bloor <max.bloor@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Maximilian Bloor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -63,14 +63,16 @@
   <b>Reinforcement learning environments for process control </b><br>
 </h1>
 <p align="center">
       <a href="https://www.python.org/doc/versions/">
         <img src="https://img.shields.io/badge/python-3.10-blue.svg" /></a>  
       <a href="https://opensource.org/license/mit">
         <img src="https://img.shields.io/badge/license-MIT-orange" /></a>
+      <a href="https://github.com/astral-sh/ruff">
+        <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json" /></a>
 </p>
 
 
 ## Quick start ⚡
 Setup a CSTR environment with a setpoint change
 
 ```python 
@@ -129,22 +131,23 @@
 ## Implemented Process Control Environments 🎛️
 
 |          Environment          | Reference | Source | Documentation |
 |:-----------------------------:|:---------:|:------:|---------------|
 |              CSTR             | [Hedengren, 2022](https://github.com/APMonitor/pdc/blob/master/CSTR_Control.ipynb)     | [Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/model_classes.py)      |               |
 |       First Order Sytem       |      N/A  | [Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/model_classes.py)        |               |
 | Multistage Extraction Column  |  [Ingham et al, 2007 (pg 471)](https://onlinelibrary.wiley.com/doi/book/10.1002/9783527614219)         | [Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/model_classes.py)        |               |
+| Nonsmooth Control|[Lim,1969](https://pubs.acs.org/doi/epdf/10.1021/i260031a007)|[Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/model_classes.py) ||
 
 
  
 ## Citing `pc-gym`
 If you use `pc-gym` in your research, please cite using the following 
 ```
 @software{pcgym2024,
-  author = {Max Bloor and ...},
+  author = {Max Bloor and and Jose Neto and Ilya Sandoval and Max Mowbray and Akhil Ahmed and Mehmet Mercangoz and Calvin Tsay and Antonio Del Rio-Chanona},
   title = {{pc-gym}: Reinforcement Learning Envionments for Process Control},
   url = {https://github.com/MaximilianB2/pc-gym},
   version = {0.0.4},
   year = {2024},
 }
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pcgym Version: 0.0.9 Summary: Reinforcement
+Metadata-Version: 2.1 Name: pcgym Version: 0.1.0 Summary: Reinforcement
 learning suite of process control problems. Author-email: Max Bloor
 gmail.com> License: MIT License Copyright (c) 2024 Maximilian Bloor Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -33,15 +33,16 @@
 "optional" Requires-Dist: stable-baselines3; extra == "optional" Requires-Dist:
 mkdocs-material; extra == "optional"
 ************ _[[_hh_tt_tt_pp_ss_::_//_//_gg_ii_tt_hh_uu_bb_.._cc_oo_mm_//_MM_aa_xx_ii_mm_ii_ll_ii_aa_nn_BB_22_//_pp_cc_--_gg_yy_mm_//_bb_ll_oo_bb_//_mm_aa_ii_nn_//_dd_oo_cc_ss_//_ii_mm_gg_//_pp_cc_--_gg_yy_mm_--_bb_ll_uu_ee_--
                                     _AA_ii_.._pp_nn_gg_]]
             RReeiinnffoorrcceemmeenntt lleeaarrnniinngg eennvviirroonnmmeennttss ffoorr pprroocceessss ccoonnttrrooll
                                      ************
   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-_3_._1_0_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-                           _b_a_d_g_e_/_l_i_c_e_n_s_e_-_M_I_T_-_o_r_a_n_g_e_]
+    _b_a_d_g_e_/_l_i_c_e_n_s_e_-_M_I_T_-_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_e_n_d_p_o_i_n_t_?_u_r_l_=_h_t_t_p_s_:_/_/
+      _r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_a_s_t_r_a_l_-_s_h_/_r_u_f_f_/_m_a_i_n_/_a_s_s_e_t_s_/_b_a_d_g_e_/_v_2_._j_s_o_n_]
 ## Quick start â¡ Setup a CSTR environment with a setpoint change ```python
 import pcgym # Simulation variables nsteps = 100 T = 25 # Setpoint SP = {'Ca':
 [0.85 for i in range(int(nsteps/2))] + [0.9 for i in range(int(nsteps/2))]} #
 Action and observation Space action_space = {'low': np.array([295]), 'high':
 np.array([302])} observation_space = {'low': np.array([0.7,300,0.8]),'high':
 np.array([1,350,0.9])} # Construct the environment parameter dictionary
 env_params = { 'N': nsteps, # Number of time steps 'tsim':T, # Simulation Time
@@ -59,15 +60,19 @@
 |---------------| | CSTR | [Hedengren, 2022](https://github.com/APMonitor/pdc/
 blob/master/CSTR_Control.ipynb) | [Source](https://github.com/MaximilianB2/pc-
 gym/blob/main/src/pcgym/model_classes.py) | | | First Order Sytem | N/A |
 [Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/
 model_classes.py) | | | Multistage Extraction Column | [Ingham et al, 2007 (pg
 471)](https://onlinelibrary.wiley.com/doi/book/10.1002/9783527614219) |
 [Source](https://github.com/MaximilianB2/pc-gym/blob/main/src/pcgym/
-model_classes.py) | | ## Citing `pc-gym` If you use `pc-gym` in your research,
-please cite using the following ``` @software{pcgym2024, author = {Max Bloor
-and ...}, title = {{pc-gym}: Reinforcement Learning Envionments for Process
-Control}, url = {https://github.com/MaximilianB2/pc-gym}, version = {0.0.4},
-year = {2024}, } ``` ## Other Great Gyms ð - â¨[safe-control-gym](https://
-github.com/utiasDSL/safe-control-gym) - â¨[safety-gymnasium](https://
-github.com/PKU-Alignment/safety-gymnasium) - â¨[gymnax](https://github.com/
-RobertTLange/gymnax)
+model_classes.py) | | | Nonsmooth Control|[Lim,1969](https://pubs.acs.org/doi/
+epdf/10.1021/i260031a007)|[Source](https://github.com/MaximilianB2/pc-gym/blob/
+main/src/pcgym/model_classes.py) || ## Citing `pc-gym` If you use `pc-gym` in
+your research, please cite using the following ``` @software{pcgym2024, author
+= {Max Bloor and and Jose Neto and Ilya Sandoval and Max Mowbray and Akhil
+Ahmed and Mehmet Mercangoz and Calvin Tsay and Antonio Del Rio-Chanona}, title
+= {{pc-gym}: Reinforcement Learning Envionments for Process Control}, url =
+{https://github.com/MaximilianB2/pc-gym}, version = {0.0.4}, year = {2024}, }
+``` ## Other Great Gyms ð - â¨[safe-control-gym](https://github.com/
+utiasDSL/safe-control-gym) - â¨[safety-gymnasium](https://github.com/PKU-
+Alignment/safety-gymnasium) - â¨[gymnax](https://github.com/RobertTLange/
+gymnax)
```

