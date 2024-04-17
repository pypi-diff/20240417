# Comparing `tmp/omegapy-3.0.3.tar.gz` & `tmp/omegapy-3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omegapy-3.0.3.tar", last modified: Wed Apr 17 14:54:57 2024, max compression
+gzip compressed data, was "omegapy-3.0b0.tar", last modified: Thu Oct 19 05:32:58 2023, max compression
```

## Comparing `omegapy-3.0.3.tar` & `omegapy-3.0b0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:54:57.571723 omegapy-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-17 14:54:48.000000 omegapy-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-17 14:54:57.571723 omegapy-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-17 14:54:48.000000 omegapy-3.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:54:57.555723 omegapy-3.0.3/omegapy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:54:57.567723 omegapy-3.0.3/omegapy/OMEGA_dataref/
--rw-r--r--   0 runner    (1001) docker     (127)   143760 2024-04-17 14:54:48.000000 omegapy-3.0.3/omegapy/OMEGA_dataref/OBC_OMEGA_OCT2017.sav
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-17 14:54:48.000000 omegapy-3.0.3/omegapy/OMEGA_dataref/boundcur.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-17 14:54:48.000000 omegapy-3.0.3/omegapy/OMEGA_dataref/corrupted_obs.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1495234 2024-04-17 14:54:48.000000 omegapy-3.0.3/omegapy/OMEGA_dataref/cubindex.ref
--rw-r--r--   0 runner    (1001) docker     (127)    49152 2024-04-17 14:54:48.000000 omegapy-3.0.3/omegapy/OMEGA_dataref/flatVIS050701.bin
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-17 14:54:48.000000 omegapy-3.0.3/omegapy/OMEGA_dataref/fond2.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-17 14:54:48.000000 omegapy-3.0.3/omegapy/OMEGA_dataref/lambda_0403.dat
--rw-r--r--   0 runner    (1001) docker     (127)    48007 2024-04-17 14:54:48.000000 omegapy-3.0.3/omegapy/OMEGA_dataref/linearC.dat
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-17 14:54:48.000000 omegapy-3.0.3/omegapy/OMEGA_dataref/mtf120315_25.dat
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-17 14:54:48.000000 omegapy-3.0.3/omegapy/OMEGA_dataref/mtf120315_50.dat
--rw-r--r--   0 runner    (1001) docker     (127)   108892 2024-04-17 14:54:48.000000 omegapy-3.0.3/omegapy/OMEGA_dataref/omega128_interpol.sav
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-17 14:54:48.000000 omegapy-3.0.3/omegapy/OMEGA_dataref/omega_atmorap_CL.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-17 14:54:48.000000 omegapy-3.0.3/omegapy/OMEGA_dataref/omega_wvl_CL.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-04-17 14:54:48.000000 omegapy-3.0.3/omegapy/OMEGA_dataref/rapcur_25.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-04-17 14:54:48.000000 omegapy-3.0.3/omegapy/OMEGA_dataref/rapcur_50.dat
--rw-r--r--   0 runner    (1001) docker     (127)  6723584 2024-04-17 14:54:48.000000 omegapy-3.0.3/omegapy/OMEGA_dataref/rapmtflcur.bin
--rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-04-17 14:54:48.000000 omegapy-3.0.3/omegapy/OMEGA_dataref/refclair_sombr_omega_CL.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-17 14:54:48.000000 omegapy-3.0.3/omegapy/OMEGA_dataref/specsol_0403.dat
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-17 14:54:48.000000 omegapy-3.0.3/omegapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   134170 2024-04-17 14:54:48.000000 omegapy-3.0.3/omegapy/omega_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    74612 2024-04-17 14:54:48.000000 omegapy-3.0.3/omegapy/omega_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:54:57.567723 omegapy-3.0.3/omegapy/res_findcube/
--rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-04-17 14:54:48.000000 omegapy-3.0.3/omegapy/res_findcube/cubelist
--rw-r--r--   0 runner    (1001) docker     (127)    15597 2024-04-17 14:54:48.000000 omegapy-3.0.3/omegapy/useful_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:54:57.571723 omegapy-3.0.3/omegapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-17 14:54:57.000000 omegapy-3.0.3/omegapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-17 14:54:57.000000 omegapy-3.0.3/omegapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 14:54:57.000000 omegapy-3.0.3/omegapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-17 14:54:57.000000 omegapy-3.0.3/omegapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 14:54:57.000000 omegapy-3.0.3/omegapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 14:54:57.571723 omegapy-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-17 14:54:48.000000 omegapy-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 05:32:58.501486 omegapy-3.0b0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2023-10-19 05:32:47.000000 omegapy-3.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2023-10-19 05:32:58.497486 omegapy-3.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2023-10-19 05:32:47.000000 omegapy-3.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 05:32:58.477486 omegapy-3.0b0/omegapy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 05:32:58.497486 omegapy-3.0b0/omegapy/OMEGA_dataref/
+-rw-r--r--   0 runner    (1001) docker     (127)   143760 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/OBC_OMEGA_OCT2017.sav
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/boundcur.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/corrupted_obs.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1495234 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/cubindex.ref
+-rw-r--r--   0 runner    (1001) docker     (127)    49152 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/flatVIS050701.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/fond2.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/lambda_0403.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    48007 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/linearC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/mtf120315_25.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/mtf120315_50.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   108892 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/omega128_interpol.sav
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/omega_atmorap_CL.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/omega_wvl_CL.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/rapcur_25.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/rapcur_50.dat
+-rw-r--r--   0 runner    (1001) docker     (127)  6723584 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/rapmtflcur.bin
+-rw-r--r--   0 runner    (1001) docker     (127)     5720 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/refclair_sombr_omega_CL.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/specsol_0403.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   134170 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/omega_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74027 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/omega_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 05:32:58.497486 omegapy-3.0b0/omegapy/res_findcube/
+-rw-r--r--   0 runner    (1001) docker     (127)     5510 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/res_findcube/cubelist
+-rw-r--r--   0 runner    (1001) docker     (127)    15597 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/useful_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 05:32:58.481486 omegapy-3.0b0/omegapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2023-10-19 05:32:58.000000 omegapy-3.0b0/omegapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2023-10-19 05:32:58.000000 omegapy-3.0b0/omegapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-19 05:32:58.000000 omegapy-3.0b0/omegapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2023-10-19 05:32:58.000000 omegapy-3.0b0/omegapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-19 05:32:58.000000 omegapy-3.0b0/omegapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-19 05:32:58.501486 omegapy-3.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-10-19 05:32:47.000000 omegapy-3.0b0/setup.py
```

### Comparing `omegapy-3.0.3/LICENSE` & `omegapy-3.0b0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Aurélien Stcherbinine
+Copyright (c) 2021 Aurélien Stcherbinine
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `omegapy-3.0.3/README.md` & `omegapy-3.0b0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,190 +1,174 @@
-00000000: 5b21 5b76 6572 7369 6f6e 2d6a 736f 6e5d  [![version-json]
-00000010: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000020: 656c 6473 2e69 6f2f 6261 6467 652f 6479  elds.io/badge/dy
-00000030: 6e61 6d69 632f 6a73 6f6e 3f75 726c 3d68  namic/json?url=h
-00000040: 7474 7073 2533 4125 3246 2532 4672 6177  ttps%3A%2F%2Fraw
-00000050: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00000060: 6e74 2e63 6f6d 2532 4641 5374 6368 6572  nt.com%2FAStcher
-00000070: 6269 6e69 6e65 2532 466f 6d65 6761 7079  binine%2Fomegapy
-00000080: 2532 466d 6173 7465 7225 3246 7061 636b  %2Fmaster%2Fpack
-00000090: 6167 652e 6a73 6f6e 2671 7565 7279 3d25  age.json&query=%
-000000a0: 3234 2e76 6572 7369 6f6e 266c 6162 656c  24.version&label
-000000b0: 3d76 6572 7369 6f6e 266c 6162 656c 436f  =version&labelCo
-000000c0: 6c6f 723d 6772 6579 2663 6f6c 6f72 3d62  lor=grey&color=b
-000000d0: 6c75 6529 5d28 6874 7470 733a 2f2f 7079  lue)](https://py
-000000e0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f6f  pi.org/project/o
-000000f0: 6d65 6761 7079 290a 215b 7079 7468 6f6e  megapy).![python
-00000100: 7665 7273 696f 6e5d 2868 7474 7073 3a2f  version](https:/
-00000110: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000120: 6261 6467 652f 6479 6e61 6d69 632f 6a73  badge/dynamic/js
-00000130: 6f6e 3f75 726c 3d68 7474 7073 2533 4125  on?url=https%3A%
-00000140: 3246 2532 4672 6177 2e67 6974 6875 6275  2F%2Fraw.githubu
-00000150: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2532  sercontent.com%2
-00000160: 4641 5374 6368 6572 6269 6e69 6e65 2532  FAStcherbinine%2
-00000170: 466f 6d65 6761 7079 2532 466d 6173 7465  Fomegapy%2Fmaste
-00000180: 7225 3246 7061 636b 6167 652e 6a73 6f6e  r%2Fpackage.json
-00000190: 2671 7565 7279 3d25 3234 2e70 7974 686f  &query=%24.pytho
-000001a0: 6e56 6572 7369 6f6e 4d69 6e26 7375 6666  nVersionMin&suff
-000001b0: 6978 3d25 3242 266c 6f67 6f3d 7079 7468  ix=%2B&logo=pyth
-000001c0: 6f6e 266c 6f67 6f43 6f6c 6f72 3d77 6869  on&logoColor=whi
-000001d0: 7465 266c 6162 656c 3d70 7974 686f 6e26  te&label=python&
-000001e0: 6c61 6265 6c43 6f6c 6f72 3d67 7265 7926  labelColor=grey&
-000001f0: 636f 6c6f 723d 626c 7565 290a 5b21 5b44  color=blue).[![D
-00000200: 4f49 5d28 6874 7470 733a 2f2f 7a65 6e6f  OI](https://zeno
-00000210: 646f 2e6f 7267 2f62 6164 6765 2f33 3439  do.org/badge/349
-00000220: 3736 3338 3439 2e73 7667 295d 2868 7474  763849.svg)](htt
-00000230: 7073 3a2f 2f7a 656e 6f64 6f2e 6f72 672f  ps://zenodo.org/
-00000240: 646f 692f 3130 2e35 3238 312f 7a65 6e6f  doi/10.5281/zeno
-00000250: 646f 2e37 3831 3838 3238 290a 5b21 5b73  do.7818828).[![s
-00000260: 7461 7475 735d 2868 7474 7073 3a2f 2f6a  tatus](https://j
-00000270: 6f73 732e 7468 656f 6a2e 6f72 672f 7061  oss.theoj.org/pa
-00000280: 7065 7273 2f31 3563 6633 3438 6132 3964  pers/15cf348a29d
-00000290: 3138 3665 3132 6634 3961 3131 3066 3966  186e12f49a110f9f
-000002a0: 3738 3766 382f 7374 6174 7573 2e73 7667  787f8/status.svg
-000002b0: 295d 2868 7474 7073 3a2f 2f6a 6f73 732e  )](https://joss.
-000002c0: 7468 656f 6a2e 6f72 672f 7061 7065 7273  theoj.org/papers
-000002d0: 2f31 3563 6633 3438 6132 3964 3138 3665  /15cf348a29d186e
-000002e0: 3132 6634 3961 3131 3066 3966 3738 3766  12f49a110f9f787f
-000002f0: 3829 0a0a 3c70 2061 6c69 676e 3d22 6365  8)..<p align="ce
-00000300: 6e74 6572 223e 0a3c 696d 6720 7769 6474  nter">.<img widt
-00000310: 683d 2232 3530 2220 6865 6967 6874 3d22  h="250" height="
-00000320: 3235 3022 2073 7263 3d22 6874 7470 733a  250" src="https:
-00000330: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
-00000340: 636f 6e74 656e 742e 636f 6d2f 4153 7463  content.com/AStc
-00000350: 6865 7262 696e 696e 652f 6f6d 6567 6170  herbinine/omegap
-00000360: 792f 6d61 7374 6572 2f64 6f63 732f 6c6f  y/master/docs/lo
-00000370: 676f 5f6f 6d65 6761 7079 5f73 6d61 6c6c  go_omegapy_small
-00000380: 322e 706e 6722 3e0a 3c2f 703e 0a0a 2320  2.png">.</p>..# 
-00000390: 4f4d 4547 412d 5079 203a 2050 7974 686f  OMEGA-Py : Pytho
-000003a0: 6e20 746f 6f6c 7320 666f 7220 4f4d 4547  n tools for OMEG
-000003b0: 4120 6461 7461 0a0a 496d 706f 7274 6174  A data..Importat
-000003c0: 696f 6e20 616e 6420 6469 7370 6c61 7920  ion and display 
-000003d0: 6f66 204f 4d45 4741 2f4d 4578 206f 6273  of OMEGA/MEx obs
-000003e0: 6572 7661 7469 6f6e 7320 696e 2050 7974  ervations in Pyt
-000003f0: 686f 6e20 332c 2062 6173 6564 206f 6e20  hon 3, based on 
-00000400: 7468 6520 4944 4c20 2a53 4f46 5431 302a  the IDL *SOFT10*
-00000410: 2072 6f75 7469 6e65 7320 6465 7665 6c6f   routines develo
-00000420: 7070 6564 2069 6e20 7468 6520 4941 5320  pped in the IAS 
-00000430: 706c 616e 6574 6172 7920 7465 616d 2e0a  planetary team..
-00000440: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
-00000450: 2026 2055 7064 6174 650a 2323 2320 4d65   & Update.### Me
-00000460: 7468 6f64 2031 3a20 6672 6f6d 2050 7950  thod 1: from PyP
-00000470: 4920 2872 6563 6f6d 6d65 6e64 6564 290a  I (recommended).
-00000480: 2a2a 496e 7374 616c 6c61 7469 6f6e 3a2a  **Installation:*
-00000490: 2a20 6070 6970 3320 696e 7374 616c 6c20  * `pip3 install 
-000004a0: 6f6d 6567 6170 7960 0a0a 2a2a 5570 6461  omegapy`..**Upda
-000004b0: 7465 3a2a 2a20 6070 6970 3320 696e 7374  te:** `pip3 inst
-000004c0: 616c 6c20 6f6d 6567 6170 7920 2d2d 7570  all omegapy --up
-000004d0: 6772 6164 6560 200a 0a0a 2323 2320 4d65  grade` ...### Me
-000004e0: 7468 6f64 2032 3a20 6672 6f6d 2074 6865  thod 2: from the
-000004f0: 2047 6974 4875 6220 7265 706f 7369 746f   GitHub reposito
-00000500: 7279 2028 6465 7665 6c6f 706d 656e 7420  ry (development 
-00000510: 7665 7273 696f 6e29 0a2a 2a49 6e73 7461  version).**Insta
-00000520: 6c6c 6174 696f 6e3a 2a2a 2043 6c6f 6e65  llation:** Clone
-00000530: 2074 6865 2072 6570 6f73 6974 6f72 7920   the repository 
-00000540: 616e 6420 696e 7374 616c 6c20 7769 7468  and install with
-00000550: 2070 6970 3a0a 0a7e 7e7e 6261 7368 0a67   pip:..~~~bash.g
-00000560: 6974 2063 6c6f 6e65 2068 7474 7073 3a2f  it clone https:/
-00000570: 2f67 6974 6875 622e 636f 6d2f 4153 7463  /github.com/AStc
-00000580: 6865 7262 696e 696e 652f 6f6d 6567 6170  herbinine/omegap
-00000590: 792e 6769 740a 6364 206f 6d65 6761 7079  y.git.cd omegapy
-000005a0: 0a70 6970 3320 696e 7374 616c 6c20 2e0a  .pip3 install ..
-000005b0: 7e7e 7e0a 0a2a 2a55 7064 6174 653a 2a2a  ~~~..**Update:**
-000005c0: 2047 6f20 746f 2074 6865 2070 7265 7669   Go to the previ
-000005d0: 6f75 736c 7920 636c 6f6e 6564 2072 6570  ously cloned rep
-000005e0: 6f73 6974 6f72 792c 2070 756c 6c20 7468  ository, pull th
-000005f0: 6520 6c61 7374 2075 7064 6174 6573 2c20  e last updates, 
-00000600: 616e 6420 696e 7374 616c 6c20 7468 656d  and install them
-00000610: 2077 6974 6820 7069 703a 0a7e 7e7e 6261   with pip:.~~~ba
-00000620: 7368 0a63 6420 6f6d 6567 6170 790a 6769  sh.cd omegapy.gi
-00000630: 7420 7075 6c6c 0a70 6970 3320 696e 7374  t pull.pip3 inst
-00000640: 616c 6c20 2e0a 7e7e 7e0a 0a23 2320 446f  all ..~~~..## Do
-00000650: 6375 6d65 6e74 6174 696f 6e0a 4675 6c6c  cumentation.Full
-00000660: 2064 6f63 756d 656e 7461 7469 6f6e 206f   documentation o
-00000670: 6620 7468 6520 4f4d 4547 412d 5079 206d  f the OMEGA-Py m
-00000680: 6f64 756c 6520 6973 2061 7661 696c 6162  odule is availab
-00000690: 6c65 2061 7420 5b61 7374 6368 6572 6269  le at [astcherbi
-000006a0: 6e69 6e65 2e67 6974 6875 622e 696f 2f6f  nine.github.io/o
-000006b0: 6d65 6761 7079 5d28 6874 7470 733a 2f2f  megapy](https://
-000006c0: 6173 7463 6865 7262 696e 696e 652e 6769  astcherbinine.gi
-000006d0: 7468 7562 2e69 6f2f 6f6d 6567 6170 792f  thub.io/omegapy/
-000006e0: 290a 0a50 6c61 6e65 7461 7279 2044 6174  )..Planetary Dat
-000006f0: 6120 576f 726b 7368 6f70 2032 3032 333a  a Workshop 2023:
-00000700: 205b 6162 7374 7261 6374 5d28 6874 7470   [abstract](http
-00000710: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
-00000720: 5374 6368 6572 6269 6e69 6e65 2f6f 6d65  Stcherbinine/ome
-00000730: 6761 7079 2f62 6c6f 622f 6d61 7374 6572  gapy/blob/master
-00000740: 2f64 6f63 732f 5374 6368 6572 6269 6e69  /docs/Stcherbini
-00000750: 6e65 5f50 4457 3230 3233 5f37 3030 375f  ne_PDW2023_7007_
-00000760: 6f6d 6567 6170 792e 7064 6629 2026 205b  omegapy.pdf) & [
-00000770: 736c 6964 6573 5d28 6874 7470 733a 2f2f  slides](https://
-00000780: 6769 7468 7562 2e63 6f6d 2f41 5374 6368  github.com/AStch
-00000790: 6572 6269 6e69 6e65 2f6f 6d65 6761 7079  erbinine/omegapy
-000007a0: 2f62 6c6f 622f 6d61 7374 6572 2f64 6f63  /blob/master/doc
-000007b0: 732f 5044 575f 466c 6167 7374 6166 665f  s/PDW_Flagstaff_
-000007c0: 5374 6368 6572 6269 6e69 6e65 5f6f 6d65  Stcherbinine_ome
-000007d0: 6761 7079 5f75 706c 6f61 642e 7064 6629  gapy_upload.pdf)
-000007e0: 0a0a 2323 2043 6f6d 6d75 6e69 7479 2067  ..## Community g
-000007f0: 7569 6465 6c69 6e65 730a 546f 2063 6f6e  uidelines.To con
-00000800: 7472 6962 7574 6520 746f 204f 4d45 4741  tribute to OMEGA
-00000810: 2d50 792c 2072 6570 6f72 7420 616e 2069  -Py, report an i
-00000820: 7373 7565 206f 7220 7365 656b 2073 7570  ssue or seek sup
-00000830: 706f 7274 2c20 706c 6561 7365 2072 6566  port, please ref
-00000840: 6572 2074 6f20 7468 6520 636f 6d6d 756e  er to the commun
-00000850: 6974 7920 6775 6964 656c 696e 6573 0a70  ity guidelines.p
-00000860: 6167 6520 6f66 2074 6865 2064 6f63 756d  age of the docum
-00000870: 656e 7461 7469 6f6e 2061 7661 696c 6162  entation availab
-00000880: 6c65 205b 6865 7265 5d28 6874 7470 733a  le [here](https:
-00000890: 2f2f 6173 7463 6865 7262 696e 696e 652e  //astcherbinine.
-000008a0: 6769 7468 7562 2e69 6f2f 6f6d 6567 6170  github.io/omegap
-000008b0: 792f 636f 6d6d 756e 6974 792f 292e 0a0a  y/community/)...
-000008c0: 2323 2043 6974 696e 6720 4f4d 4547 412d  ## Citing OMEGA-
-000008d0: 5079 0a49 6620 796f 7520 6172 6520 7573  Py.If you are us
-000008e0: 696e 6720 4f4d 4547 412d 5079 2069 6e20  ing OMEGA-Py in 
-000008f0: 796f 7572 2072 6573 6561 7263 682c 2070  your research, p
-00000900: 6c65 6173 6520 6369 7465 2069 7420 6163  lease cite it ac
-00000910: 636f 7264 696e 6720 746f 2074 6865 2067  cording to the g
-00000920: 7569 6465 6c69 6e65 7320 6176 6169 6c61  uidelines availa
-00000930: 626c 6520 5b68 6572 655d 2868 7474 7073  ble [here](https
-00000940: 3a2f 2f61 7374 6368 6572 6269 6e69 6e65  ://astcherbinine
-00000950: 2e67 6974 6875 622e 696f 2f6f 6d65 6761  .github.io/omega
-00000960: 7079 2f63 7265 6469 7473 2f29 2e0a 0a23  py/credits/)...#
-00000970: 2320 4372 6564 6974 730a 0ac2 a920 4175  # Credits.... Au
-00000980: 72c3 a96c 6965 6e20 5374 6368 6572 6269  r..lien Stcherbi
-00000990: 6e69 6e65 2028 3230 3230 e280 9332 3032  nine (2020...202
-000009a0: 3429 0a0a 496e 7374 6974 7574 2064 2741  4)..Institut d'A
-000009b0: 7374 726f 7068 7973 6971 7565 2053 7061  strophysique Spa
-000009c0: 7469 616c 6520 2849 4153 292c 2055 6e69  tiale (IAS), Uni
-000009d0: 7665 7273 6974 c3a9 2050 6172 6973 2d53  versit.. Paris-S
-000009e0: 6163 6c61 792c 2043 4e52 532c 204f 7273  aclay, CNRS, Ors
-000009f0: 6179 2c20 4672 616e 6365 0a0a 4c41 544d  ay, France..LATM
-00000a00: 4f53 2f49 5053 4c2c 2055 5653 5120 556e  OS/IPSL, UVSQ Un
-00000a10: 6976 6572 7369 74c3 a920 5061 7269 732d  iversit.. Paris-
-00000a20: 5361 636c 6179 2c20 536f 7262 6f6e 6e65  Saclay, Sorbonne
-00000a30: 2055 6e69 7665 7273 6974 c3a9 2c20 434e   Universit.., CN
-00000a40: 5253 2c20 4775 7961 6e63 6f75 7274 2c20  RS, Guyancourt, 
-00000a50: 4672 616e 6365 0a0a 4465 7061 7274 6d65  France..Departme
-00000a60: 6e74 206f 6620 4173 7472 6f6e 6f6d 7920  nt of Astronomy 
-00000a70: 616e 6420 506c 616e 6574 6172 7920 5363  and Planetary Sc
-00000a80: 6965 6e63 652c 204e 6f72 7468 6572 6e20  ience, Northern 
-00000a90: 4172 697a 6f6e 6120 556e 6976 6572 7369  Arizona Universi
-00000aa0: 7479 2c20 466c 6167 7374 6166 662c 2041  ty, Flagstaff, A
-00000ab0: 5a2c 2055 5341 0a0a 496e 7374 6974 7574  Z, USA..Institut
-00000ac0: 2064 6520 5265 6368 6572 6368 6520 656e   de Recherche en
-00000ad0: 2041 7374 726f 7068 7973 6971 7565 2065   Astrophysique e
-00000ae0: 7420 506c 616e c3a9 746f 6c6f 6769 6520  t Plan..tologie 
-00000af0: 2849 5241 5029 2c20 434e 4553 2c20 556e  (IRAP), CNES, Un
-00000b00: 6976 6572 7369 74c3 a920 546f 756c 6f75  iversit.. Toulou
-00000b10: 7365 2049 4949 2c0a 434e 5253 2c20 546f  se III,.CNRS, To
-00000b20: 756c 6f75 7365 2c20 4672 616e 6365 0a0a  ulouse, France..
-00000b30: 0a23 2320 4c69 6365 6e73 650a 5468 6973  .## License.This
-00000b40: 2070 6163 6b61 6765 2069 7320 7265 6c65   package is rele
-00000b50: 6173 6564 2075 6e64 6572 2061 204d 4954  ased under a MIT
-00000b60: 206f 7065 6e20 736f 7572 6365 206c 6963   open source lic
-00000b70: 656e 7365 2e20 5365 6520 5b60 4c49 4345  ense. See [`LICE
-00000b80: 4e53 4560 5d28 6874 7470 733a 2f2f 6769  NSE`](https://gi
-00000b90: 7468 7562 2e63 6f6d 2f41 5374 6368 6572  thub.com/AStcher
-00000ba0: 6269 6e69 6e65 2f6f 6d65 6761 7079 2f62  binine/omegapy/b
-00000bb0: 6c6f 622f 6d61 7374 6572 2f4c 4943 454e  lob/master/LICEN
-00000bc0: 5345 2920 666f 7220 6d6f 7265 2064 6574  SE) for more det
-00000bd0: 6169 6c73 2e0a                           ails..
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6f6d 6567  : 2.1.Name: omeg
+00000020: 6170 790a 5665 7273 696f 6e3a 2033 2e30  apy.Version: 3.0
+00000030: 6230 0a53 756d 6d61 7279 3a20 5079 7468  b0.Summary: Pyth
+00000040: 6f6e 2074 6f6f 6c73 2066 6f72 204f 4d45  on tools for OME
+00000050: 4741 2f4d 4578 206f 6273 6572 7661 7469  GA/MEx observati
+00000060: 6f6e 7320 616e 616c 7973 6973 0a48 6f6d  ons analysis.Hom
+00000070: 652d 7061 6765 3a20 6874 7470 733a 2f2f  e-page: https://
+00000080: 6173 7463 6865 7262 696e 696e 652e 6769  astcherbinine.gi
+00000090: 7468 7562 2e69 6f2f 6f6d 6567 6170 790a  thub.io/omegapy.
+000000a0: 4175 7468 6f72 3a20 4175 72c3 a96c 6965  Author: Aur..lie
+000000b0: 6e20 5374 6368 6572 6269 6e69 6e65 0a41  n Stcherbinine.A
+000000c0: 7574 686f 722d 656d 6169 6c3a 2061 7572  uthor-email: aur
+000000d0: 656c 6965 6e40 7374 6368 6572 6269 6e69  elien@stcherbini
+000000e0: 6e65 2e6e 6574 0a50 726f 6a65 6374 2d55  ne.net.Project-U
+000000f0: 524c 3a20 536f 7572 6365 2c20 6874 7470  RL: Source, http
+00000100: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
+00000110: 5374 6368 6572 6269 6e69 6e65 2f6f 6d65  Stcherbinine/ome
+00000120: 6761 7079 0a43 6c61 7373 6966 6965 723a  gapy.Classifier:
+00000130: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000140: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000150: 3a3a 2033 0a43 6c61 7373 6966 6965 723a  :: 3.Classifier:
+00000160: 204c 6963 656e 7365 203a 3a20 4f53 4920   License :: OSI 
+00000170: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
+00000180: 4c69 6365 6e73 650a 436c 6173 7369 6669  License.Classifi
+00000190: 6572 3a20 4f70 6572 6174 696e 6720 5379  er: Operating Sy
+000001a0: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
+000001b0: 656e 6465 6e74 0a43 6c61 7373 6966 6965  endent.Classifie
+000001c0: 723a 2049 6e74 656e 6465 6420 4175 6469  r: Intended Audi
+000001d0: 656e 6365 203a 3a20 5363 6965 6e63 652f  ence :: Science/
+000001e0: 5265 7365 6172 6368 0a43 6c61 7373 6966  Research.Classif
+000001f0: 6965 723a 2054 6f70 6963 203a 3a20 5363  ier: Topic :: Sc
+00000200: 6965 6e74 6966 6963 2f45 6e67 696e 6565  ientific/Enginee
+00000210: 7269 6e67 203a 3a20 4173 7472 6f6e 6f6d  ring :: Astronom
+00000220: 790a 5265 7175 6972 6573 2d50 7974 686f  y.Requires-Pytho
+00000230: 6e3a 203e 3d33 2e37 0a44 6573 6372 6970  n: >=3.7.Descrip
+00000240: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
+00000250: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
+00000260: 0a4c 6963 656e 7365 2d46 696c 653a 204c  .License-File: L
+00000270: 4943 454e 5345 0a0a 215b 7665 7273 696f  ICENSE..![versio
+00000280: 6e5d 2868 7474 7073 3a2f 2f69 6d67 2e73  n](https://img.s
+00000290: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+000002a0: 7665 7273 696f 6e2d 332e 3062 6574 612d  version-3.0beta-
+000002b0: 626c 7565 290a 215b 7079 7468 6f6e 7665  blue).![pythonve
+000002c0: 7273 696f 6e5d 2868 7474 7073 3a2f 2f69  rsion](https://i
+000002d0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+000002e0: 6467 652f 5079 7468 6f6e 2d33 2e37 2b2d  dge/Python-3.7+-
+000002f0: 626c 7565 290a 5b21 5b44 4f49 5d28 6874  blue).[![DOI](ht
+00000300: 7470 733a 2f2f 7a65 6e6f 646f 2e6f 7267  tps://zenodo.org
+00000310: 2f62 6164 6765 2f33 3439 3736 3338 3439  /badge/349763849
+00000320: 2e73 7667 295d 2868 7474 7073 3a2f 2f7a  .svg)](https://z
+00000330: 656e 6f64 6f2e 6f72 672f 6261 6467 652f  enodo.org/badge/
+00000340: 6c61 7465 7374 646f 692f 3334 3937 3633  latestdoi/349763
+00000350: 3834 3929 0a0a 0a3c 7020 616c 6967 6e3d  849)...<p align=
+00000360: 2263 656e 7465 7222 3e0a 3c69 6d67 2077  "center">.<img w
+00000370: 6964 7468 3d22 3235 3022 2068 6569 6768  idth="250" heigh
+00000380: 743d 2232 3530 2220 7372 633d 2268 7474  t="250" src="htt
+00000390: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000003a0: 4153 7463 6865 7262 696e 696e 652f 6f6d  AStcherbinine/om
+000003b0: 6567 6170 792f 626c 6f62 2f6d 6173 7465  egapy/blob/maste
+000003c0: 722f 646f 6373 2f6c 6f67 6f5f 6f6d 6567  r/docs/logo_omeg
+000003d0: 6170 795f 736d 616c 6c32 2e70 6e67 223e  apy_small2.png">
+000003e0: 0a3c 2f70 3e0a 0a23 204f 4d45 4741 2d50  .</p>..# OMEGA-P
+000003f0: 7920 3a20 5079 7468 6f6e 2074 6f6f 6c73  y : Python tools
+00000400: 2066 6f72 204f 4d45 4741 2064 6174 610a   for OMEGA data.
+00000410: 0a49 6d70 6f72 7461 7469 6f6e 2061 6e64  .Importation and
+00000420: 2064 6973 706c 6179 206f 6620 4f4d 4547   display of OMEG
+00000430: 412f 4d45 7820 6f62 7365 7276 6174 696f  A/MEx observatio
+00000440: 6e73 2069 6e20 5079 7468 6f6e 2033 2c20  ns in Python 3, 
+00000450: 6261 7365 6420 6f6e 2074 6865 2049 444c  based on the IDL
+00000460: 202a 534f 4654 3130 2a20 726f 7574 696e   *SOFT10* routin
+00000470: 6573 2064 6576 656c 6f70 7065 6420 696e  es developped in
+00000480: 2074 6865 2049 4153 2070 6c61 6e65 7461   the IAS planeta
+00000490: 7279 2074 6561 6d2e 0a0a 3e20 2a2a 4469  ry team...> **Di
+000004a0: 7363 6c61 696d 6572 3a2a 2a20 5468 6973  sclaimer:** This
+000004b0: 206d 6f64 756c 6520 6973 206e 6f74 2074   module is not t
+000004c0: 6865 206f 6666 6963 6961 6c20 736f 6674  he official soft
+000004d0: 7761 7265 2064 6973 7472 6962 7574 6564  ware distributed
+000004e0: 2062 7920 7468 6520 4f4d 4547 4120 7465   by the OMEGA te
+000004f0: 616d 2e0a 0a23 2320 496e 7374 616c 6c61  am...## Installa
+00000500: 7469 6f6e 2026 2055 7064 6174 650a 2323  tion & Update.##
+00000510: 2320 4d65 7468 6f64 2031 3a20 6672 6f6d  # Method 1: from
+00000520: 2050 7950 4920 2872 6563 6f6d 6d65 6e64   PyPI (recommend
+00000530: 6564 290a 2a2a 496e 7374 616c 6c61 7469  ed).**Installati
+00000540: 6f6e 3a2a 2a20 6070 6970 3320 696e 7374  on:** `pip3 inst
+00000550: 616c 6c20 6f6d 6567 6170 7960 0a0a 2a2a  all omegapy`..**
+00000560: 5570 6461 7465 3a2a 2a20 6070 6970 3320  Update:** `pip3 
+00000570: 696e 7374 616c 6c20 6f6d 6567 6170 7920  install omegapy 
+00000580: 2d2d 7570 6772 6164 6560 200a 0a0a 2323  --upgrade` ...##
+00000590: 2320 4d65 7468 6f64 2032 3a20 6672 6f6d  # Method 2: from
+000005a0: 2074 6865 2047 6974 4875 6220 7265 706f   the GitHub repo
+000005b0: 7369 746f 7279 2028 6465 7665 6c6f 706d  sitory (developm
+000005c0: 656e 7420 7665 7273 696f 6e29 0a2a 2a49  ent version).**I
+000005d0: 6e73 7461 6c6c 6174 696f 6e3a 2a2a 2043  nstallation:** C
+000005e0: 6c6f 6e65 2074 6865 2072 6570 6f73 6974  lone the reposit
+000005f0: 6f72 7920 616e 6420 696e 7374 616c 6c20  ory and install 
+00000600: 7769 7468 2070 6970 3a0a 0a7e 7e7e 6261  with pip:..~~~ba
+00000610: 7368 0a67 6974 2063 6c6f 6e65 2068 7474  sh.git clone htt
+00000620: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000630: 4153 7463 6865 7262 696e 696e 652f 6f6d  AStcherbinine/om
+00000640: 6567 6170 792e 6769 740a 6364 206f 6d65  egapy.git.cd ome
+00000650: 6761 7079 0a70 6970 3320 696e 7374 616c  gapy.pip3 instal
+00000660: 6c20 2e0a 7e7e 7e0a 0a2a 2a55 7064 6174  l ..~~~..**Updat
+00000670: 653a 2a2a 2047 6f20 746f 2074 6865 2070  e:** Go to the p
+00000680: 7265 7669 6f75 736c 7920 636c 6f6e 6564  reviously cloned
+00000690: 2072 6570 6f73 6974 6f72 792c 2070 756c   repository, pul
+000006a0: 6c20 7468 6520 6c61 7374 2075 7064 6174  l the last updat
+000006b0: 6573 2c20 616e 6420 696e 7374 616c 6c20  es, and install 
+000006c0: 7468 656d 2077 6974 6820 7069 703a 0a7e  them with pip:.~
+000006d0: 7e7e 6261 7368 0a63 6420 6f6d 6567 6170  ~~bash.cd omegap
+000006e0: 790a 6769 7420 7075 6c6c 0a70 6970 3320  y.git pull.pip3 
+000006f0: 696e 7374 616c 6c20 2e0a 7e7e 7e0a 0a23  install ..~~~..#
+00000700: 2320 446f 6375 6d65 6e74 6174 696f 6e0a  # Documentation.
+00000710: 4675 6c6c 2064 6f63 756d 656e 7461 7469  Full documentati
+00000720: 6f6e 206f 6620 7468 6520 4f4d 4547 412d  on of the OMEGA-
+00000730: 5079 206d 6f64 756c 6520 6973 2061 7661  Py module is ava
+00000740: 696c 6162 6c65 2061 7420 5b61 7374 6368  ilable at [astch
+00000750: 6572 6269 6e69 6e65 2e67 6974 6875 622e  erbinine.github.
+00000760: 696f 2f6f 6d65 6761 7079 5d28 6874 7470  io/omegapy](http
+00000770: 733a 2f2f 6173 7463 6865 7262 696e 696e  s://astcherbinin
+00000780: 652e 6769 7468 7562 2e69 6f2f 6f6d 6567  e.github.io/omeg
+00000790: 6170 792f 290a 0a50 6c61 6e65 7461 7279  apy/)..Planetary
+000007a0: 2044 6174 6120 576f 726b 7368 6f70 2032   Data Workshop 2
+000007b0: 3032 333a 205b 6162 7374 7261 6374 5d28  023: [abstract](
+000007c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000007d0: 6f6d 2f41 5374 6368 6572 6269 6e69 6e65  om/AStcherbinine
+000007e0: 2f6f 6d65 6761 7079 2f62 6c6f 622f 6d61  /omegapy/blob/ma
+000007f0: 7374 6572 2f64 6f63 732f 5374 6368 6572  ster/docs/Stcher
+00000800: 6269 6e69 6e65 5f50 4457 3230 3233 5f37  binine_PDW2023_7
+00000810: 3030 375f 6f6d 6567 6170 792e 7064 6629  007_omegapy.pdf)
+00000820: 2026 205b 736c 6964 6573 5d28 6874 7470   & [slides](http
+00000830: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
+00000840: 5374 6368 6572 6269 6e69 6e65 2f6f 6d65  Stcherbinine/ome
+00000850: 6761 7079 2f62 6c6f 622f 6d61 7374 6572  gapy/blob/master
+00000860: 2f64 6f63 732f 5044 575f 466c 6167 7374  /docs/PDW_Flagst
+00000870: 6166 665f 5374 6368 6572 6269 6e69 6e65  aff_Stcherbinine
+00000880: 5f6f 6d65 6761 7079 5f75 706c 6f61 642e  _omegapy_upload.
+00000890: 7064 6629 0a0a 2323 2043 6974 696e 6720  pdf)..## Citing 
+000008a0: 4f4d 4547 412d 5079 0a49 6620 796f 7520  OMEGA-Py.If you 
+000008b0: 6172 6520 7573 696e 6720 4f4d 4547 412d  are using OMEGA-
+000008c0: 5079 2069 6e20 796f 7572 2072 6573 6561  Py in your resea
+000008d0: 7263 682c 2070 6c65 6173 6520 6369 7465  rch, please cite
+000008e0: 2069 7420 6163 636f 7264 696e 6720 746f   it according to
+000008f0: 2074 6865 2067 7569 6465 6c69 6e65 7320   the guidelines 
+00000900: 6176 6169 6c61 626c 6520 5b68 6572 655d  available [here]
+00000910: 2868 7474 7073 3a2f 2f61 7374 6368 6572  (https://astcher
+00000920: 6269 6e69 6e65 2e67 6974 6875 622e 696f  binine.github.io
+00000930: 2f6f 6d65 6761 7079 2f63 7265 6469 7473  /omegapy/credits
+00000940: 2f29 2e0a 0a23 2320 4372 6564 6974 730a  /)...## Credits.
+00000950: 0ac2 a920 4175 72c3 a96c 6965 6e20 5374  ... Aur..lien St
+00000960: 6368 6572 6269 6e69 6e65 2028 3230 3230  cherbinine (2020
+00000970: e280 9332 3032 3329 0a0a 496e 7374 6974  ...2023)..Instit
+00000980: 7574 2064 2741 7374 726f 7068 7973 6971  ut d'Astrophysiq
+00000990: 7565 2053 7061 7469 616c 6520 2849 4153  ue Spatiale (IAS
+000009a0: 292c 2055 6e69 7665 7273 6974 c3a9 2050  ), Universit.. P
+000009b0: 6172 6973 2d53 6163 6c61 792c 2043 4e52  aris-Saclay, CNR
+000009c0: 532c 204f 7273 6179 2c20 4672 616e 6365  S, Orsay, France
+000009d0: 0a0a 4c41 544d 4f53 2f49 5053 4c2c 2055  ..LATMOS/IPSL, U
+000009e0: 5653 5120 556e 6976 6572 7369 74c3 a920  VSQ Universit.. 
+000009f0: 5061 7269 732d 5361 636c 6179 2c20 536f  Paris-Saclay, So
+00000a00: 7262 6f6e 6e65 2055 6e69 7665 7273 6974  rbonne Universit
+00000a10: c3a9 2c20 434e 5253 2c20 4775 7961 6e63  .., CNRS, Guyanc
+00000a20: 6f75 7274 2c20 4672 616e 6365 0a0a 0a23  ourt, France...#
+00000a30: 2320 4c69 6365 6e73 650a 5468 6973 2070  # License.This p
+00000a40: 6163 6b61 6765 2069 7320 7265 6c65 6173  ackage is releas
+00000a50: 6564 2075 6e64 6572 2061 204d 4954 206f  ed under a MIT o
+00000a60: 7065 6e20 736f 7572 6365 206c 6963 656e  pen source licen
+00000a70: 7365 2e20 5365 6520 5b60 4c49 4345 4e53  se. See [`LICENS
+00000a80: 4560 5d28 6874 7470 733a 2f2f 6769 7468  E`](https://gith
+00000a90: 7562 2e63 6f6d 2f41 5374 6368 6572 6269  ub.com/AStcherbi
+00000aa0: 6e69 6e65 2f6f 6d65 6761 7079 2f62 6c6f  nine/omegapy/blo
+00000ab0: 622f 6d61 7374 6572 2f4c 4943 454e 5345  b/master/LICENSE
+00000ac0: 2920 666f 7220 6d6f 7265 2064 6574 6169  ) for more detai
+00000ad0: 6c73 2e0a                                ls..
```

### Comparing `omegapy-3.0.3/omegapy/OMEGA_dataref/OBC_OMEGA_OCT2017.sav` & `omegapy-3.0b0/omegapy/OMEGA_dataref/OBC_OMEGA_OCT2017.sav`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.3/omegapy/OMEGA_dataref/boundcur.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/boundcur.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.3/omegapy/OMEGA_dataref/corrupted_obs.csv` & `omegapy-3.0b0/omegapy/OMEGA_dataref/corrupted_obs.csv`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.3/omegapy/OMEGA_dataref/cubindex.ref` & `omegapy-3.0b0/omegapy/OMEGA_dataref/cubindex.ref`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.3/omegapy/OMEGA_dataref/flatVIS050701.bin` & `omegapy-3.0b0/omegapy/OMEGA_dataref/flatVIS050701.bin`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.3/omegapy/OMEGA_dataref/fond2.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/fond2.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.3/omegapy/OMEGA_dataref/lambda_0403.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/lambda_0403.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.3/omegapy/OMEGA_dataref/linearC.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/linearC.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.3/omegapy/OMEGA_dataref/mtf120315_25.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/mtf120315_25.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.3/omegapy/OMEGA_dataref/mtf120315_50.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/mtf120315_50.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.3/omegapy/OMEGA_dataref/omega128_interpol.sav` & `omegapy-3.0b0/omegapy/OMEGA_dataref/omega128_interpol.sav`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.3/omegapy/OMEGA_dataref/omega_atmorap_CL.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/omega_atmorap_CL.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.3/omegapy/OMEGA_dataref/omega_wvl_CL.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/omega_wvl_CL.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.3/omegapy/OMEGA_dataref/rapcur_25.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/rapcur_25.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.3/omegapy/OMEGA_dataref/rapcur_50.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/rapcur_50.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.3/omegapy/OMEGA_dataref/rapmtflcur.bin` & `omegapy-3.0b0/omegapy/OMEGA_dataref/rapmtflcur.bin`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.3/omegapy/OMEGA_dataref/refclair_sombr_omega_CL.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/refclair_sombr_omega_CL.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.3/omegapy/OMEGA_dataref/specsol_0403.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/specsol_0403.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.3/omegapy/omega_data.py` & `omegapy-3.0b0/omegapy/omega_data.py`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.3/omegapy/omega_plots.py` & `omegapy-3.0b0/omegapy/omega_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 ## omega_plots.py
 ## Created by Aurélien STCHERBININE
-## Last modified by Aurélien STCHERBININE : 16/04/2024
+## Last modified by Aurélien STCHERBININE : 18/10/2023
 
 ##----------------------------------------------------------------------------------------
 """Display of `OMEGAdata` cubes.
 """
 ##----------------------------------------------------------------------------------------
 ##----------------------------------------------------------------------------------------
 ## Packages
@@ -178,15 +178,15 @@
     cmap : str, default 'Greys_r'
         The matplotlib colormap.
     vmin : float or None, default None
         The lower bound of the colorscale.
     vmax : float or None, default None
         The upper bound of the colorscale.
     alpha : float or None, default None
-        Opacity of the plot, from 0 (transparent) to 1 (opaque).
+        Opacity of the plot.
     title : str, default 'auto'
         The title of the figure.
     lonlim : tuple of int or None, default (None, None)
         The longitude bounds of the figure.
     latlim : tuple of int or None, default (None, None)
         The latitude bounds of the y-axis of the figure.
     Nfig : int or str or None, default None
@@ -619,15 +619,15 @@
     autoyscale : bool, default True
         | `True` --> Enable the auto-scaling of the spectra y-axis.</br>
         | `False` --> Force use of the (vmin, vmax) bounds for the spectra plots.
     ylim_sp : tuple of float or None, default (None, None)
         If autoyscale is False, can specify the bound values for the spectrum y-axis,
         other that `(vmin, vmax)`.
     alpha : float or None, default None
-        Opacity of the plot, from 0 (transparent) to 1 (opaque).
+        Opacity of the plot.
     lonlim : tuple of int or None, default (None, None)
         The longitude bounds of the figure.
     latlim : tuple of int or None, default (None, None)
         The latitude bounds of the y-axis of the figure.
     polar : bool, default False
         If `True` --> Use a polar projection for the plot.
     cbar : bool, default True
@@ -813,15 +813,15 @@
     cmap : str, default 'Greys_r'
         The matplotlib colormap.
     vmin : float or None, default None
         The lower bound of the colorscale.
     vmax : float or None, default None
         The upper bound of the colorscale.
     alpha : float or None, default None
-        Opacity of the plot, from 0 (transparent) to 1 (opaque).
+        Opacity of the plot.
     title : str, default 'auto'
         The title of the figure.
     cb_title : str, default 'data'
         The title of the colorbar.
     lonlim : tuple of int or None, default (None, None)
         The longitude bounds of the figure.
     latlim : tuple of int or None, default (None, None)
@@ -857,24 +857,16 @@
             negatives_longitudes = True
     if title == 'auto':
         title = ('OMEGA/MEx observation {0}'.format(omega.name))
     fig = plt.figure(Nfig)
     Nfig = fig.number   # get the actual figure number if Nfig=None
     if not (mask is None):
         data = deepcopy(data) * mask     # apply mask to remove bad pixels (turned to NaN)
-    if len(fig.get_axes()) != 0:    # If presence of axes
-        ax0 = fig.get_axes()[0]
-        is_ax0_polar = hasattr(ax0, 'set_theta_offset') # Test if ax has polar projection
-        if not polar == is_ax0_polar:
-            raise ValueError("Can not mix polar and non-polar projections in the same plot")
     if polar:
-        if len(fig.get_axes()) == 0:    # Test presence of axes in the figure
-            ax = plt.axes(polar=True)
-        else:
-            ax = fig.get_axes()[0]  # Do not create new axes instance
+        ax = plt.axes(polar=True)
         plt.pcolormesh(omega.lon_grid*np.pi/180, omega.lat_grid, data, cmap=cmap, 
                        alpha=alpha, vmin=vmin, vmax=vmax, **kwargs)
         ax.set_yticklabels([])  # remove the latitude values in the plot
         if latlim[0] is None:
             if np.max(omega.lat) > 0:
                 latlim = (90, np.min(omega.lat_grid)-1)
             else:
```

### Comparing `omegapy-3.0.3/omegapy/res_findcube/cubelist` & `omegapy-3.0b0/omegapy/res_findcube/cubelist`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.3/omegapy/useful_functions.py` & `omegapy-3.0b0/omegapy/useful_functions.py`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.3/omegapy.egg-info/SOURCES.txt` & `omegapy-3.0b0/omegapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.3/setup.py` & `omegapy-3.0b0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 import setuptools
-import json
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 with open('requirements.txt', 'r') as f:
     requirements = f.read().strip('\n').split('\n')
-with open('omegapy/package.json', 'r') as f:
-    data_json = json.load(f)
 
 package_data = {
     '': ['OMEGA_dataref/*', 'res_findcube/*'],
     }
 
 setuptools.setup(
     name='omegapy',
-    version=data_json['version'],
+    version='3.0beta',
     author='Aurélien Stcherbinine',
     author_email='aurelien@stcherbinine.net',
     description='Python tools for OMEGA/MEx observations analysis',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://astcherbinine.github.io/omegapy',
     project_urls={
         'Source' : 'https://github.com/AStcherbinine/omegapy',
     },
     packages=setuptools.find_packages(),
     package_data=package_data,
-    python_requires='>='+data_json['pythonVersionMin'],
+    python_requires='>=3.7',
     setup_requires=['wheel'],
     install_requires=requirements,
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Intended Audience :: Science/Research',
```

