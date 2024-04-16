# Comparing `tmp/vplanet-2.5.3.tar.gz` & `tmp/vplanet-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vplanet-2.5.3.tar", last modified: Sat Apr 13 04:19:15 2024, max compression
+gzip compressed data, was "vplanet-2.5.4.tar", last modified: Tue Apr 16 22:32:15 2024, max compression
```

## Comparing `vplanet-2.5.3.tar` & `vplanet-2.5.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:19:15.157432 vplanet-2.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-13 04:19:10.000000 vplanet-2.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-04-13 04:19:15.157432 vplanet-2.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-04-13 04:19:10.000000 vplanet-2.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 04:19:15.157432 vplanet-2.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-13 04:19:11.000000 vplanet-2.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:19:15.157432 vplanet-2.5.3/src/
--rw-r--r--   0 runner    (1001) docker     (127)   172320 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/atmesc.c
--rw-r--r--   0 runner    (1001) docker     (127)    90413 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/binary.c
--rw-r--r--   0 runner    (1001) docker     (127)    45057 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/body.c
--rw-r--r--   0 runner    (1001) docker     (127)    35872 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/control.c
--rw-r--r--   0 runner    (1001) docker     (127)   261673 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/distorb.c
--rw-r--r--   0 runner    (1001) docker     (127)    84678 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/distrot.c
--rw-r--r--   0 runner    (1001) docker     (127)   173282 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/eqtide.c
--rw-r--r--   0 runner    (1001) docker     (127)    28197 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/evolve.c
--rw-r--r--   0 runner    (1001) docker     (127)    71119 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/flare.c
--rw-r--r--   0 runner    (1001) docker     (127)   141475 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/galhabit.c
--rw-r--r--   0 runner    (1001) docker     (127)    12739 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/halt.c
--rw-r--r--   0 runner    (1001) docker     (127)   116650 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/magmoc.c
--rw-r--r--   0 runner    (1001) docker     (127)    93363 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/module.c
--rw-r--r--   0 runner    (1001) docker     (127)   160335 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/options.c
--rw-r--r--   0 runner    (1001) docker     (127)    83300 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/output.c
--rw-r--r--   0 runner    (1001) docker     (127)   284882 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/poise.c
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/python_interface.c
--rw-r--r--   0 runner    (1001) docker     (127)   245259 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/radheat.c
--rw-r--r--   0 runner    (1001) docker     (127)    48492 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/spinbody.c
--rw-r--r--   0 runner    (1001) docker     (127)    77727 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/stellar.c
--rw-r--r--   0 runner    (1001) docker     (127)    33849 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/system.c
--rw-r--r--   0 runner    (1001) docker     (127)   196096 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/thermint.c
--rw-r--r--   0 runner    (1001) docker     (127)   159057 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/update.c
--rw-r--r--   0 runner    (1001) docker     (127)    43834 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/verify.c
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/vplanet.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:19:15.157432 vplanet-2.5.3/vplanet/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-13 04:19:11.000000 vplanet-2.5.3/vplanet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-13 04:19:11.000000 vplanet-2.5.3/vplanet/custom_units.py
--rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-04-13 04:19:11.000000 vplanet-2.5.3/vplanet/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-13 04:19:11.000000 vplanet-2.5.3/vplanet/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-04-13 04:19:11.000000 vplanet-2.5.3/vplanet/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-04-13 04:19:11.000000 vplanet-2.5.3/vplanet/quantity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-13 04:19:11.000000 vplanet-2.5.3/vplanet/quantity_support.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-13 04:19:11.000000 vplanet-2.5.3/vplanet/vplanet_help.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-13 04:19:11.000000 vplanet-2.5.3/vplanet/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:19:15.157432 vplanet-2.5.3/vplanet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-04-13 04:19:15.000000 vplanet-2.5.3/vplanet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-13 04:19:15.000000 vplanet-2.5.3/vplanet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 04:19:15.000000 vplanet-2.5.3/vplanet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-13 04:19:15.000000 vplanet-2.5.3/vplanet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 04:19:15.000000 vplanet-2.5.3/vplanet.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-13 04:19:15.000000 vplanet-2.5.3/vplanet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-13 04:19:15.000000 vplanet-2.5.3/vplanet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:32:15.931968 vplanet-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-16 22:32:14.000000 vplanet-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-04-16 22:32:15.931968 vplanet-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-04-16 22:32:14.000000 vplanet-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 22:32:15.931968 vplanet-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-16 22:32:15.000000 vplanet-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:32:15.927968 vplanet-2.5.4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)   172506 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/atmesc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    90413 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/binary.c
+-rw-r--r--   0 runner    (1001) docker     (127)    45227 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/body.c
+-rw-r--r--   0 runner    (1001) docker     (127)    35908 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/control.c
+-rw-r--r--   0 runner    (1001) docker     (127)   261673 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/distorb.c
+-rw-r--r--   0 runner    (1001) docker     (127)    84904 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/distrot.c
+-rw-r--r--   0 runner    (1001) docker     (127)   173282 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/eqtide.c
+-rw-r--r--   0 runner    (1001) docker     (127)    28197 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/evolve.c
+-rw-r--r--   0 runner    (1001) docker     (127)    71119 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/flare.c
+-rw-r--r--   0 runner    (1001) docker     (127)   141475 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/galhabit.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12739 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/halt.c
+-rw-r--r--   0 runner    (1001) docker     (127)   116650 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/magmoc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    93363 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/module.c
+-rw-r--r--   0 runner    (1001) docker     (127)   160335 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/options.c
+-rw-r--r--   0 runner    (1001) docker     (127)    83338 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/output.c
+-rw-r--r--   0 runner    (1001) docker     (127)   284882 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/poise.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/python_interface.c
+-rw-r--r--   0 runner    (1001) docker     (127)   245259 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/radheat.c
+-rw-r--r--   0 runner    (1001) docker     (127)    48492 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/spinbody.c
+-rw-r--r--   0 runner    (1001) docker     (127)    77773 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/stellar.c
+-rw-r--r--   0 runner    (1001) docker     (127)    33849 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/system.c
+-rw-r--r--   0 runner    (1001) docker     (127)   196096 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/thermint.c
+-rw-r--r--   0 runner    (1001) docker     (127)   159057 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/update.c
+-rw-r--r--   0 runner    (1001) docker     (127)    43834 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/verify.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/vplanet.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:32:15.931968 vplanet-2.5.4/vplanet/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet/custom_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet/quantity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet/quantity_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet/vplanet_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:32:15.931968 vplanet-2.5.4/vplanet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet.egg-info/top_level.txt
```

### Comparing `vplanet-2.5.3/LICENSE` & `vplanet-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.3/PKG-INFO` & `vplanet-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vplanet
-Version: 2.5.3
+Version: 2.5.4
 Summary: The virtual planet simulator
 Home-page: https://github.com/VirtualPlanetaryLaboratory/vplanet
 Author: Rory Barnes
 Author-email: rkb9@uw.edu
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -31,15 +31,15 @@
   <a href="https://www.youtube.com/@VPLanetCode/playlists">
     <img src="https://img.shields.io/badge/You-Tube-darkred.svg">
   </a>
    <a href="https://github.com/VirtualPlanetaryLaboratory/vplanet/discussions">
      <img src="https://img.shields.io/badge/Discussions-darkgreen.svg">
   </a>
   <br>
-  <img src="https://img.shields.io/badge/Unit%20Tests-18,062-darkblue.svg">
+  <img src="https://img.shields.io/badge/Unit%20Tests-19,130-darkblue.svg">
   <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-linux.yml/badge.svg">
   <img src="https://img.shields.io/badge/Ubuntu%2020-Python%203.6--3.11-7d93c7.svg">
   <img src="https://img.shields.io/badge/Ubuntu%2022-Python%203.7--3.11-7d93c7.svg">
   
   <br>
   <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-macos-intel.yml/badge.svg">
   <img src="https://img.shields.io/badge/MacOS%2011--13-Python%203.6--3.11-7d93c7.svg">
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: vplanet Version: 2.5.3 Summary: The virtual planet
+Metadata-Version: 2.1 Name: vplanet Version: 2.5.4 Summary: The virtual planet
 simulator Home-page: https://github.com/VirtualPlanetaryLaboratory/vplanet
 Author: Rory Barnes Author-email: rkb9@uw.edu License: MIT Platform: UNKNOWN
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE
                         [docs/VPLanetLogo.png?raw=true]
               ************ VVPPLLaanneett:: TThhee VViirrttuuaall PPllaanneett SSiimmuullaattoorr ************
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_a_d_-_t_h_e___d_o_c_s_-_b_l_u_e_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_][https://
    github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/docs.yml/
             badge.svg]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_a_d_-_t_h_e___p_a_p_e_r_-
    _d_a_r_k_g_r_e_e_n_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_d_e_%_2_0_o_f_-_C_o_n_d_u_c_t_-
     _7_d_9_3_c_7_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_Y_o_u_-_T_u_b_e_-_d_a_r_k_r_e_d_._s_v_g_]_[_h_t_t_p_s_:_/_/
                 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_D_i_s_c_u_s_s_i_o_n_s_-_d_a_r_k_g_r_e_e_n_._s_v_g_]
-   [https://img.shields.io/badge/Unit%20Tests-18,062-darkblue.svg][https://
+   [https://img.shields.io/badge/Unit%20Tests-19,130-darkblue.svg][https://
     github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-
  linux.yml/badge.svg][https://img.shields.io/badge/Ubuntu%2020-Python%203.6--
  3.11-7d93c7.svg][https://img.shields.io/badge/Ubuntu%2022-Python%203.7--3.11-
                                   7d93c7.svg]
 [https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-
     macos-intel.yml/badge.svg][https://img.shields.io/badge/MacOS%2011--13-
  Python%203.6--3.11-7d93c7.svg][https://github.com/VirtualPlanetaryLaboratory/
```

### Comparing `vplanet-2.5.3/README.md` & `vplanet-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   <a href="https://www.youtube.com/@VPLanetCode/playlists">
     <img src="https://img.shields.io/badge/You-Tube-darkred.svg">
   </a>
    <a href="https://github.com/VirtualPlanetaryLaboratory/vplanet/discussions">
      <img src="https://img.shields.io/badge/Discussions-darkgreen.svg">
   </a>
   <br>
-  <img src="https://img.shields.io/badge/Unit%20Tests-18,062-darkblue.svg">
+  <img src="https://img.shields.io/badge/Unit%20Tests-19,130-darkblue.svg">
   <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-linux.yml/badge.svg">
   <img src="https://img.shields.io/badge/Ubuntu%2020-Python%203.6--3.11-7d93c7.svg">
   <img src="https://img.shields.io/badge/Ubuntu%2022-Python%203.7--3.11-7d93c7.svg">
   
   <br>
   <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-macos-intel.yml/badge.svg">
   <img src="https://img.shields.io/badge/MacOS%2011--13-Python%203.6--3.11-7d93c7.svg">
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
               ************ VVPPLLaanneett:: TThhee VViirrttuuaall PPllaanneett SSiimmuullaattoorr ************
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_a_d_-_t_h_e___d_o_c_s_-_b_l_u_e_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_][https://
    github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/docs.yml/
             badge.svg]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_a_d_-_t_h_e___p_a_p_e_r_-
    _d_a_r_k_g_r_e_e_n_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_d_e_%_2_0_o_f_-_C_o_n_d_u_c_t_-
     _7_d_9_3_c_7_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_Y_o_u_-_T_u_b_e_-_d_a_r_k_r_e_d_._s_v_g_]_[_h_t_t_p_s_:_/_/
                 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_D_i_s_c_u_s_s_i_o_n_s_-_d_a_r_k_g_r_e_e_n_._s_v_g_]
-   [https://img.shields.io/badge/Unit%20Tests-18,062-darkblue.svg][https://
+   [https://img.shields.io/badge/Unit%20Tests-19,130-darkblue.svg][https://
     github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-
  linux.yml/badge.svg][https://img.shields.io/badge/Ubuntu%2020-Python%203.6--
  3.11-7d93c7.svg][https://img.shields.io/badge/Ubuntu%2022-Python%203.7--3.11-
                                   7d93c7.svg]
 [https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-
     macos-intel.yml/badge.svg][https://img.shields.io/badge/MacOS%2011--13-
  Python%203.6--3.11-7d93c7.svg][https://github.com/VirtualPlanetaryLaboratory/
```

### Comparing `vplanet-2.5.3/setup.py` & `vplanet-2.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.3/src/atmesc.c` & `vplanet-2.5.4/src/atmesc.c`

 * *Files 1% similar despite different names*

```diff
@@ -2104,51 +2104,45 @@
   if (options[OPT_FXUV].iLine[iBody + 1] > -1) {
     body[iBody].bCalcFXUV = 0;
   } else {
     body[iBody].bCalcFXUV = 1;
   }
 
   if (body[iBody].iPlanetRadiusModel == ATMESC_LEHMER17) {
-    if (body[iBody].dEnvelopeMass >= 0.5 * body[iBody].dMass) {
-      fprintf(stderr,
-              "ERROR: %s's Envelope mass is greater than 50%% of its total "
-              "mass, which ",
+    if (body[0].bStellar) {
+      if (body[iBody].dEnvelopeMass > 0.5 * body[iBody].dMass) {
+        fprintf(stderr,
+                "ERROR: %s's Envelope mass is greater than 50%% of its total "
+                "mass, which ",
+                body[iBody].cName);
+        fprintf(
+              stderr,
+              "is not allowed  for the Lehmer-Catling (2017) envelope model.\n");
+        DoubleLineExit(files->Infile[iBody + 1].cIn, files->Infile[iBody + 1].cIn,
+                      options[OPT_ENVELOPEMASS].iLine[iBody + 1],
+                      options[OPT_MASS].iLine[iBody + 1]);
+      }
+      if (body[iBody].dEnvelopeMass >= 0.1 * body[iBody].dMass) {
+        fprintf(
+              stderr,
+              "WARNING: Envelope masses more than 10%% of the total mass are not "
+              "recommended for the Lehmer-Catling (2017) envelope model. %s's "
+              "envelope ",
               body[iBody].cName);
-      fprintf(
-            stderr,
-            "is not allowed  for the Lehmer-Catling (2017) envelope model.\n");
-      DoubleLineExit(files->Infile[iBody + 1].cIn, files->Infile[iBody + 1].cIn,
-                     options[OPT_ENVELOPEMASS].iLine[iBody + 1],
-                     options[OPT_ENVELOPEMASS].iLine[iBody + 1]);
-    }
-    if (body[iBody].dEnvelopeMass >= 0.1 * body[iBody].dMass) {
-      fprintf(
-            stderr,
-            "WARNING: Envelope masses more than 10%% of the total mass are not "
-            "recommended for the Lehmer-Catling (2017) envelope model. %s's "
-            "envelope ",
-            body[iBody].cName);
-      fprintf(stderr, "mass exceeds this threshold.\n");
-    }
+        fprintf(stderr, "mass exceeds this threshold.\n");
+      }
 
-    // Get thermal temperature
-    if (body[iBody].bAutoThermTemp) {
-      body[iBody].dThermTemp = fdThermalTemp(body, iBody);
-    }
-    body[iBody].dRadSolid = fdMassToRad_LehmerCatling17(
-          body[iBody].dMass - body[iBody].dEnvelopeMass);
-    body[iBody].dGravAccel = BIGG *
-                             (body[iBody].dMass - body[iBody].dEnvelopeMass) /
-                             (body[iBody].dRadSolid * body[iBody].dRadSolid);
-    body[iBody].dScaleHeight = body[iBody].dAtmGasConst *
-                               body[iBody].dThermTemp / body[iBody].dGravAccel;
-    body[iBody].dPresSurf =
-          fdLehmerPres(body[iBody].dEnvelopeMass, body[iBody].dGravAccel,
-                       body[iBody].dRadSolid);
-    body[iBody].dRadXUV = fdLehmerRadius(body, iBody);
+      // Calculate auxiliary properties
+      body[iBody].dRadSolid = fdMassToRad_LehmerCatling17(body[iBody].dMass - body[iBody].dEnvelopeMass);
+      AuxPropsLehmer17(body,iBody);      
+    } else {
+      fprintf(stderr,
+              "ERROR: The Lehmer & Catling (2017) model requires a star.\n");
+      exit(EXIT_INPUT);
+    }
   } else {
     int iCol, bError = 0;
     for (iCol = 0; iCol < files->Outfile[iBody].iNumCols; iCol++) {
       if (memcmp(files->Outfile[iBody].caCol[iCol],
                  output[OUT_PLANETRADXUV].cName,
                  strlen(output[OUT_PLANETRADXUV].cName)) == 0) {
         /* Match! */
@@ -2826,18 +2820,22 @@
                   UNITS *units, UPDATE *update, int iBody, double *dTmp,
                   char cUnit[]) {
 
   // Get the RG flux
   double flux = fdHZRG14(body, iBody);
 
   // Convert to semi-major axis *at current eccentricity!*
-  *dTmp = pow(4 * PI * flux /
-                    (body[0].dLuminosity *
-                     pow((1 - body[iBody].dEcc * body[iBody].dEcc), 0.5)),
-              -0.5);
+  if (body[0].dLuminosity == 0) {
+    *dTmp = -1;
+  } else {
+    *dTmp = pow(4 * PI * flux /
+                (body[0].dLuminosity *
+                pow((1 - body[iBody].dEcc * body[iBody].dEcc), 0.5)),
+                -0.5);
+  }
 
   if (output->bDoNeg[iBody]) {
     *dTmp *= output->dNeg;
     strcpy(cUnit, output->cNeg);
   } else {
     *dTmp /= fdUnitsLength(units->iLength);
     fsUnitsLength(units->iLength, cUnit);
@@ -3354,18 +3352,22 @@
                        double *dTmp, char cUnit[]) {
   double BDIFF = 4.8e19 * pow(body[iBody].dFlowTemp, 0.75);
   double XO    = fdAtomicOxygenMixingRatio(body[iBody].dSurfaceWaterMass,
                                            body[iBody].dOxygenMass);
   double GPotential =
         (BIGG * body[iBody].dMass * PROTONMASS) / (body[iBody].dRadius);
 
-  *dTmp = ((4 * BDIFF * pow(GPotential, 2)) /
-           (body[iBody].dAtmXAbsEffH2O * KBOLTZ * body[iBody].dFlowTemp *
-            body[iBody].dRadius)) *
-          (QOH - 1) * (1 - XO);
+  if (body[iBody].dAtmXAbsEffH2O > 0 && body[iBody].dFlowTemp > 0 && body[iBody].dRadius > 0) {
+    *dTmp = ((4 * BDIFF * pow(GPotential, 2)) /
+            (body[iBody].dAtmXAbsEffH2O * KBOLTZ * body[iBody].dFlowTemp *
+              body[iBody].dRadius)) *
+            (QOH - 1) * (1 - XO);
+  } else {
+    *dTmp = -1;
+  }
   if (output->bDoNeg[iBody]) {
     *dTmp *= output->dNeg;
     strcpy(cUnit, output->cNeg);
   } else {
     strcpy(cUnit, "W/m^2");
   }
 }
@@ -4301,32 +4303,37 @@
   double b3 = -0.8988;
   double c0 = -0.00441536;
   double c1 = -0.03068399;
   double c2 = 0.04946948;
   double c3 = -0.89880083;
 
   // Convert to erg/cm^2/s and take the log
-  double x = log10(dFXUV * 1.e3);
-  double y;
+  double dWaterEscapeEfficiency;
 
-  // Piecewise polynomial fit and handle edge cases
-  if ((x >= -2) && (x < -1)) {
-    y = pow(10, a0 * x * x + a1 * x + a2);
-  } else if ((x >= -1) && (x < 0)) {
-    y = pow(10, b0 * x * x * x + b1 * x * x + b2 * x + b3);
-  } else if ((x >= 0) && (x <= 5)) {
-    y = pow(10, c0 * x * x * x + c1 * x * x + c2 * x + c3);
-  } else if (x < -2) { // Lower flux bound
-    y = 0.001;
-  } else if (x > 5) { // Upper flux bound
-    y = 0.01;
-  } else { // Base case that never happens but DPF likes code symmetry
-    y = 0.1;
+  if (dFXUV > 0) {
+    double x = log10(dFXUV * 1.e3);
+
+    // Piecewise polynomial fit and handle edge cases
+    if ((x >= -2) && (x < -1)) {
+      dWaterEscapeEfficiency = pow(10, a0 * x * x + a1 * x + a2);
+    } else if ((x >= -1) && (x < 0)) {
+      dWaterEscapeEfficiency = pow(10, b0 * x * x * x + b1 * x * x + b2 * x + b3);
+    } else if ((x >= 0) && (x <= 5)) {
+      dWaterEscapeEfficiency = pow(10, c0 * x * x * x + c1 * x * x + c2 * x + c3);
+    } else if (x < -2) { // Lower flux bound
+      dWaterEscapeEfficiency = 0.001;
+    } else if (x > 5) { // Upper flux bound
+      dWaterEscapeEfficiency = 0.01;
+    } else { // Base case that never happens but DPF likes code symmetry
+      dWaterEscapeEfficiency = 0.1;
+    }
+  } else {
+    dWaterEscapeEfficiency = 0; // No escape if F_XUV = 0
   }
-  return y;
+  return dWaterEscapeEfficiency;
 }
 
 /**
 Performs a really simple linear least-squares fit on data.
 
 @param x The independent coordinates
 @param y The dependent coordinates
@@ -4396,22 +4403,25 @@
 
  @param body BODY struct
  @param iBody int body indentifier
 
  @return Body's Bondi radius
 */
 double fdBondiRadius(BODY *body, int iBody) {
-
+  double dBondiRadius;
   // Compute sound speed in planet's atmosphere assuming a diatomic H atmosphere
-  // assuming body 0 is the star as it should be when using atmesc
-  double cs = fdEqH2AtmosphereSoundSpeed(body[0].dTemperature, body[0].dRadius,
+  // assuming body 0 is the star
+  if (body[0].bStellar) {
+    double dSoundSpeed = fdEqH2AtmosphereSoundSpeed(body[0].dTemperature, body[0].dRadius,
                                          body[iBody].dSemi);
-  double rb = BIGG * body[iBody].dMass / (2.0 * cs * cs);
-
-  return rb;
+    dBondiRadius = BIGG * body[iBody].dMass / (2.0 * dSoundSpeed * dSoundSpeed);
+  } else {
+    dBondiRadius = -1;
+  }
+  return dBondiRadius;
 }
 
 /**
  Calculate the whether or not incident XUV flux exceeds critical flux between
  the radiation/recombination-limited and energy-limited H envelope escape
  regimes following Luger+2015 Eqn. 13
```

### Comparing `vplanet-2.5.3/src/binary.c` & `vplanet-2.5.4/src/binary.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.3/src/body.c` & `vplanet-2.5.4/src/body.c`

 * *Files 0% similar despite different names*

```diff
@@ -57,18 +57,18 @@
   Caclulate the characteristic timescale for a variable to change that is
   controlled by only 1 module.
 
   @param dVar The value of the variable
   @param dDeriv The value of the variable's time derivative
 
   @return The timescale of the variable's change: |x/(dx/dt)|. If the
-  derivative is 0, return 0.
+  derivative is <1e-100, return 0.
 */
 double fdTimescale(double dVar, double dDeriv) {
-  if (dDeriv != 0) {
+  if (dDeriv > 1e-100) {
     return fabs(dVar / dDeriv);
   } else {
     return 0;
   }
 }
 
 /**
@@ -80,24 +80,24 @@
 @param iNum The number of derivatives
 @param dTime Dummy variable to keep track of the sum of the derivative
 @param iPert Index of the perturbing process
 
 @return The timescale of the variable's change: |x/Sum(dx/dt)|
 */
 double fdTimescaleMulti(double dVar, double *dDeriv, int iNum) {
-  double dTime;
+  double dTime,dTotalDerivative;
   int iPert;
 
-  dTime = 0;
+  dTotalDerivative = 0;
   for (iPert = 0; iPert < iNum; iPert++) {
     if (dDeriv[iPert] != 0) {
-      dTime += dDeriv[iPert]; // Note that here dTime is actullay the rate
+      dTotalDerivative += dDeriv[iPert]; 
     }
-    dTime = fabs(dVar / dTime);
   }
+  dTime = fabs(dVar / dTotalDerivative);
   return dTime;
 }
 
 /**
  Convert an angular frequency to a period
 
  @param dFreq The frequency
@@ -576,18 +576,23 @@
    @param dPresSurf pressure at surface due to envelope
    @param dRadXUV radius from center of planet where optical depth of XUV is
   unity
    */
 double fdLehmerRadius(BODY *body, int iBody) {
   double dRadXUV, dRoche;
 
-  dRadXUV = body[iBody].dRadSolid * body[iBody].dRadSolid /
+  // Set floor for surface pressure to prevent overflow error
+  if (body[iBody].dPresSurf > 1e-100) {
+    dRadXUV = body[iBody].dRadSolid * body[iBody].dRadSolid /
             (body[iBody].dScaleHeight *
                    log(body[iBody].dPresXUV / body[iBody].dPresSurf) +
              body[iBody].dRadSolid);
+  } else {
+    dRadXUV = body[iBody].dRadSolid;
+  }
   dRoche = fdRocheRadius(body, iBody);
   // printf("%lf %lf %lf %lf
   // %lf\n",body[iBody].dPresXUV,body[iBody].dPresSurf,body[iBody].dGravAccel,body[iBody].dEnvelopeMass,dRadXUV);
   if (dRadXUV <= 0) {
     dRadXUV = dRoche;
   }
   if (dRadXUV > dRoche) {
```

### Comparing `vplanet-2.5.3/src/control.c` & `vplanet-2.5.4/src/control.c`

 * *Files 1% similar despite different names*

```diff
@@ -1082,16 +1082,17 @@
   strcat(cUnit, "^2/");
   fsUnitsTime(units->iTime, cTmp);
   strcat(cUnit, cTmp);
   strcat(cUnit, "^2");
 }
 
 double fdUnitsEnergy(int iTime, int iMass, int iLength) {
-  return fdUnitsMass(iMass) * fdUnitsLength(iLength) * fdUnitsLength(iLength) /
+  double dConversion = fdUnitsMass(iMass) * fdUnitsLength(iLength) * fdUnitsLength(iLength) /
          (fdUnitsTime(iTime) * fdUnitsTime(iTime));
+  return dConversion;
 }
 
 void fsUnitsPower(UNITS *units, char cUnit[]) {
   char cTmp[OPTLEN];
 
   fsUnitsMass(units->iMass, cUnit);
   strcat(cUnit, "*");
```

### Comparing `vplanet-2.5.3/src/distorb.c` & `vplanet-2.5.4/src/distorb.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.3/src/distrot.c` & `vplanet-2.5.4/src/distrot.c`

 * *Files 1% similar despite different names*

```diff
@@ -1024,15 +1024,19 @@
   dDeriv = 0;
   for (iPert = 0; iPert < body[iBody].iGravPerts; iPert++) {
     dDeriv += dObldx * (*(update[iBody].padDXoblDtDistRot[iPert])) +
               dObldy * (*(update[iBody].padDYoblDtDistRot[iPert])) +
               dObldz * (*(update[iBody].padDZoblDtDistRot[iPert]));
   }
 
+  if (dDeriv == 0) {
+    *dTmp = -1;
+  } else {
   *dTmp = fabs(PI / dDeriv);
+  }
 
   if (output->bDoNeg[iBody]) {
     *dTmp *= output->dNeg;
     strcpy(cUnit, output->cNeg);
   } else {
     *dTmp *= fdUnitsTime(units->iTime);
     fsUnitsRate(units->iTime, cUnit);
@@ -1061,15 +1065,19 @@
   /* Ensure that we don't overwrite derivative */
   dDeriv = 0;
   for (iPert = 0; iPert <= body[iBody].iGravPerts; iPert++) {
     dDeriv += dpAdx * (*(update[iBody].padDXoblDtDistRot[iPert])) +
               dpAdy * (*(update[iBody].padDYoblDtDistRot[iPert]));
   }
 
-  *dTmp = fabs(2 * PI / dDeriv);
+  if (dDeriv == 0) {
+    dDeriv = -1;
+  } else {
+    *dTmp = fabs(2 * PI / dDeriv);
+  }
 
   if (output->bDoNeg[iBody]) {
     *dTmp *= output->dNeg;
     strcpy(cUnit, output->cNeg);
   } else {
     *dTmp /= fdUnitsTime(units->iTime);
     fsUnitsTime(units->iTime, cUnit);
@@ -1142,16 +1150,14 @@
                              SYSTEM *system, UNITS *units, UPDATE *update,
                              int iBody, double *dTmp, char cUnit[]) {
   double dDeriv;
   int iPert;
 
   /* Ensure that we don't overwrite derivative */
   dDeriv = 0;
-  dDeriv = pow(10, 300);
-  dDeriv *= dDeriv;
   for (iPert = 0; iPert <= body[iBody].iGravPerts; iPert++) {
     dDeriv += *(update[iBody].padDYoblDtDistRot[iPert]);
   }
 
   *dTmp = dDeriv;
 
   if (output->bDoNeg[iBody]) {
@@ -1194,15 +1200,19 @@
 
   /* Ensure that we don't overwrite derivative */
   dDeriv = 0;
   for (iPert = 0; iPert <= body[iBody].iGravPerts; iPert++) {
     dDeriv += *(update[iBody].padDXoblDtDistRot[iPert]);
   }
 
-  *dTmp = fabs(1. / dDeriv);
+  if (dDeriv == 0) {
+    *dTmp = -1;
+  } else {
+    *dTmp = fabs(1. / dDeriv);
+  }
 
   if (output->bDoNeg[iBody]) {
     *dTmp *= output->dNeg;
     strcpy(cUnit, output->cNeg);
   } else {
     *dTmp *= fdUnitsTime(units->iTime);
     fsUnitsRate(units->iTime, cUnit);
@@ -1217,15 +1227,19 @@
 
   /* Ensure that we don't overwrite derivative */
   dDeriv = 0;
   for (iPert = 0; iPert <= body[iBody].iGravPerts; iPert++) {
     dDeriv += *(update[iBody].padDYoblDtDistRot[iPert]);
   }
 
-  *dTmp = fabs(1. / dDeriv);
+  if (dDeriv == 0) {
+    *dTmp = -1;
+  } else {
+    *dTmp = fabs(1. / dDeriv);
+  }
 
   if (output->bDoNeg[iBody]) {
     *dTmp *= output->dNeg;
     strcpy(cUnit, output->cNeg);
   } else {
     *dTmp *= fdUnitsTime(units->iTime);
     fsUnitsRate(units->iTime, cUnit);
@@ -1240,16 +1254,20 @@
 
   /* Ensure that we don't overwrite derivative */
   dDeriv = 0;
   for (iPert = 0; iPert < body[iBody].iGravPerts; iPert++) {
     dDeriv += *(update[iBody].padDZoblDtDistRot[iPert]);
   }
 
-  *dTmp = fabs(1. / dDeriv);
-
+  if (dDeriv == 0) {
+    *dTmp = -1;
+  } else {
+    *dTmp = fabs(1. / dDeriv);
+  }
+  
   if (output->bDoNeg[iBody]) {
     *dTmp *= output->dNeg;
     strcpy(cUnit, output->cNeg);
   } else {
     *dTmp *= fdUnitsTime(units->iTime);
     fsUnitsRate(units->iTime, cUnit);
   }
```

### Comparing `vplanet-2.5.3/src/eqtide.c` & `vplanet-2.5.4/src/eqtide.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.3/src/evolve.c` & `vplanet-2.5.4/src/evolve.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.3/src/flare.c` & `vplanet-2.5.4/src/flare.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.3/src/galhabit.c` & `vplanet-2.5.4/src/galhabit.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.3/src/halt.c` & `vplanet-2.5.4/src/halt.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.3/src/magmoc.c` & `vplanet-2.5.4/src/magmoc.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.3/src/module.c` & `vplanet-2.5.4/src/module.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.3/src/options.c` & `vplanet-2.5.4/src/options.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.3/src/output.c` & `vplanet-2.5.4/src/output.c`

 * *Files 0% similar despite different names*

```diff
@@ -672,15 +672,16 @@
   *dTmp = body[iBody].dLostEng;
 
 
   if (output->bDoNeg[iBody]) {
     *dTmp *= output->dNeg;
     strcpy(cUnit, output->cNeg);
   } else {
-    *dTmp /= fdUnitsEnergy(units->iTime, units->iMass, units->iLength);
+    double dConversion = fdUnitsEnergy(units->iTime, units->iMass, units->iLength);
+    *dTmp /= dConversion;
     fsUnitsEnergy(units, cUnit);
   }
 }
 
 void WriteOrbEnergy(BODY *body, CONTROL *control, OUTPUT *output,
                     SYSTEM *system, UNITS *units, UPDATE *update, int iBody,
                     double *dTmp, char cUnit[]) {
```

### Comparing `vplanet-2.5.3/src/poise.c` & `vplanet-2.5.4/src/poise.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.3/src/python_interface.c` & `vplanet-2.5.4/src/python_interface.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.3/src/radheat.c` & `vplanet-2.5.4/src/radheat.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.3/src/spinbody.c` & `vplanet-2.5.4/src/spinbody.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.3/src/stellar.c` & `vplanet-2.5.4/src/stellar.c`

 * *Files 0% similar despite different names*

```diff
@@ -459,15 +459,15 @@
   sprintf(options[OPT_XUVBETA].cLongDescr,
           "After the \"saturation\" phase, the ratio of the XUV to total "
           "luminosity\n"
           "will follow a power law followinfg this exponent. Units are "
           "gigayears.");
 
   sprintf(options[OPT_STELLARMODEL].cName, "sStellarModel");
-  sprintf(options[OPT_STELLARMODEL].cDescr, "Luminosity evolution model");
+  sprintf(options[OPT_STELLARMODEL].cDescr, "Stellar evolution model");
   sprintf(options[OPT_STELLARMODEL].cDefault, "BARAFFE");
   sprintf(options[OPT_STELLARMODEL].cValues, "BARAFFE PROXIMA SINEWAVE NONE");
   options[OPT_STELLARMODEL].iType      = 3;
   options[OPT_STELLARMODEL].bMultiFile = 1;
   fnRead[OPT_STELLARMODEL]             = &ReadStellarModel;
   sprintf(
         options[OPT_STELLARMODEL].cLongDescr,
@@ -1520,14 +1520,15 @@
     if (!isnan(foo)) {
       return foo;
     } else {
       body[iaBody[0]].iStellarModel = STELLAR_MODEL_CONST;
     }
   }
   if (body[iaBody[0]].iStellarModel == STELLAR_MODEL_SINEWAVE) {
+    printf("%lf\n",body[iaBody[0]].dLuminosity);
     foo = fdEffectiveTemperature(body,iaBody[0]);
     return foo;
   }
   if (body[iaBody[0]].iStellarModel == STELLAR_MODEL_NONE ||
       body[iaBody[0]].iStellarModel == STELLAR_MODEL_CONST) {
     return body[iaBody[0]].dTemperature;
   } else {
```

### Comparing `vplanet-2.5.3/src/system.c` & `vplanet-2.5.4/src/system.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.3/src/thermint.c` & `vplanet-2.5.4/src/thermint.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.3/src/update.c` & `vplanet-2.5.4/src/update.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.3/src/verify.c` & `vplanet-2.5.4/src/verify.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.3/src/vplanet.c` & `vplanet-2.5.4/src/vplanet.c`

 * *Files 4% similar despite different names*

```diff
@@ -24,24 +24,26 @@
 /*!
 Actual implementation of the main function; called from in `int main()` below.
 We need this wrapper so we can call `main_impl` from Python.
 
  */
 int main_impl(int argc, char *argv[]) {
 #ifdef DEBUG
-#ifdef __x86_64__
-  //  feenableexcept(FE_INVALID | FE_OVERFLOW);
-  _MM_SET_EXCEPTION_MASK(_MM_GET_EXCEPTION_MASK() & ~_MM_MASK_INVALID);
-  _MM_SET_EXCEPTION_MASK(_MM_GET_EXCEPTION_MASK() & ~_MM_MASK_OVERFLOW);
-  fprintf(stderr, "INFO: Floating point trapping enabled.\n");
-#else
-  fprintf(stderr,
-          "WARNING: Floating point trapping only enabled for x86 "
-          "architectures.\n");
-#endif
+  #ifdef __x86_64__
+    //  feenableexcept(FE_INVALID | FE_OVERFLOW);
+    _MM_SET_EXCEPTION_MASK(_MM_GET_EXCEPTION_MASK() & ~_MM_MASK_INVALID);
+    _MM_SET_EXCEPTION_MASK(_MM_GET_EXCEPTION_MASK() & ~_MM_MASK_OVERFLOW);
+    _MM_SET_EXCEPTION_MASK(_MM_GET_EXCEPTION_MASK() & ~_MM_MASK_DIV_ZERO);
+    //_MM_SET_EXCEPTION_MASK(_MM_GET_EXCEPTION_MASK() & ~_MM_MASK_UNDERFLOW);
+    fprintf(stderr, "INFO: Floating point trapping enabled.\n");
+  #else
+    fprintf(stderr,
+            "WARNING: Floating point trapping only enabled for x86 "
+            "architectures.\n");
+  #endif
 #endif
 
   // struct timeval start, end;
 
   /* Fix CPU time calculation someday
   gettimeofday(&start, NULL);
```

### Comparing `vplanet-2.5.3/vplanet/custom_units.py` & `vplanet-2.5.4/vplanet/custom_units.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.3/vplanet/log.py` & `vplanet-2.5.4/vplanet/log.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.3/vplanet/output.py` & `vplanet-2.5.4/vplanet/output.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.3/vplanet/quantity.py` & `vplanet-2.5.4/vplanet/quantity.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.3/vplanet/quantity_support.py` & `vplanet-2.5.4/vplanet/quantity_support.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.3/vplanet/wrapper.py` & `vplanet-2.5.4/vplanet/wrapper.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.3/vplanet.egg-info/PKG-INFO` & `vplanet-2.5.4/vplanet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vplanet
-Version: 2.5.3
+Version: 2.5.4
 Summary: The virtual planet simulator
 Home-page: https://github.com/VirtualPlanetaryLaboratory/vplanet
 Author: Rory Barnes
 Author-email: rkb9@uw.edu
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -31,15 +31,15 @@
   <a href="https://www.youtube.com/@VPLanetCode/playlists">
     <img src="https://img.shields.io/badge/You-Tube-darkred.svg">
   </a>
    <a href="https://github.com/VirtualPlanetaryLaboratory/vplanet/discussions">
      <img src="https://img.shields.io/badge/Discussions-darkgreen.svg">
   </a>
   <br>
-  <img src="https://img.shields.io/badge/Unit%20Tests-18,062-darkblue.svg">
+  <img src="https://img.shields.io/badge/Unit%20Tests-19,130-darkblue.svg">
   <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-linux.yml/badge.svg">
   <img src="https://img.shields.io/badge/Ubuntu%2020-Python%203.6--3.11-7d93c7.svg">
   <img src="https://img.shields.io/badge/Ubuntu%2022-Python%203.7--3.11-7d93c7.svg">
   
   <br>
   <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-macos-intel.yml/badge.svg">
   <img src="https://img.shields.io/badge/MacOS%2011--13-Python%203.6--3.11-7d93c7.svg">
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: vplanet Version: 2.5.3 Summary: The virtual planet
+Metadata-Version: 2.1 Name: vplanet Version: 2.5.4 Summary: The virtual planet
 simulator Home-page: https://github.com/VirtualPlanetaryLaboratory/vplanet
 Author: Rory Barnes Author-email: rkb9@uw.edu License: MIT Platform: UNKNOWN
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE
                         [docs/VPLanetLogo.png?raw=true]
               ************ VVPPLLaanneett:: TThhee VViirrttuuaall PPllaanneett SSiimmuullaattoorr ************
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_a_d_-_t_h_e___d_o_c_s_-_b_l_u_e_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_][https://
    github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/docs.yml/
             badge.svg]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_a_d_-_t_h_e___p_a_p_e_r_-
    _d_a_r_k_g_r_e_e_n_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_d_e_%_2_0_o_f_-_C_o_n_d_u_c_t_-
     _7_d_9_3_c_7_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_Y_o_u_-_T_u_b_e_-_d_a_r_k_r_e_d_._s_v_g_]_[_h_t_t_p_s_:_/_/
                 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_D_i_s_c_u_s_s_i_o_n_s_-_d_a_r_k_g_r_e_e_n_._s_v_g_]
-   [https://img.shields.io/badge/Unit%20Tests-18,062-darkblue.svg][https://
+   [https://img.shields.io/badge/Unit%20Tests-19,130-darkblue.svg][https://
     github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-
  linux.yml/badge.svg][https://img.shields.io/badge/Ubuntu%2020-Python%203.6--
  3.11-7d93c7.svg][https://img.shields.io/badge/Ubuntu%2022-Python%203.7--3.11-
                                   7d93c7.svg]
 [https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-
     macos-intel.yml/badge.svg][https://img.shields.io/badge/MacOS%2011--13-
  Python%203.6--3.11-7d93c7.svg][https://github.com/VirtualPlanetaryLaboratory/
```

### Comparing `vplanet-2.5.3/vplanet.egg-info/SOURCES.txt` & `vplanet-2.5.4/vplanet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

