# Comparing `tmp/dimlpfidex-0.0.0.tar.gz` & `tmp/dimlpfidex-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dimlpfidex-0.0.0.tar", max compression
+gzip compressed data, was "dimlpfidex-0.0.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `dimlpfidex-0.0.0.tar` & `dimlpfidex-0.0.1.tar`

### file list

```diff
@@ -1,136 +1,1374 @@
--rw-r--r--   0        0        0     1497 2023-04-19 08:20:49.680102 dimlpfidex-0.0.0/LICENSE
--rw-r--r--   0        0        0     2055 2023-09-26 08:51:57.599279 dimlpfidex-0.0.0/README.md
--rw-r--r--   0        0        0     2703 2023-08-25 14:36:27.212537 dimlpfidex-0.0.0/build.py
--rw-r--r--   0        0        0     2805 2023-05-10 13:50:30.097943 dimlpfidex-0.0.0/dimlp/CMakeLists.txt
--rw-r--r--   0        0        0        0 2023-05-08 12:26:01.289246 dimlpfidex-0.0.0/dimlp/__init__.py
--rw-r--r--   0        0        0    17039 2023-09-26 08:51:57.599279 dimlpfidex-0.0.0/dimlp/convKeras.py
--rw-r--r--   0        0        0     3902 2023-09-13 14:13:35.009351 dimlpfidex-0.0.0/dimlp/convKerasV1.py
--rw-r--r--   0        0        0     8586 2023-06-20 06:07:51.722437 dimlpfidex-0.0.0/dimlp/cpp/CMakeLists.txt
--rw-r--r--   0        0        0    57391 2023-07-06 07:51:52.044009 dimlpfidex-0.0.0/dimlp/cpp/src/CrossValid.cpp
--rw-r--r--   0        0        0      304 2023-05-30 05:36:57.520650 dimlpfidex-0.0.0/dimlp/cpp/src/DensCls.cpp
--rw-r--r--   0        0        0    16375 2023-09-11 09:37:18.878636 dimlpfidex-0.0.0/dimlp/cpp/src/DensClsFct.cpp
--rw-r--r--   0        0        0      305 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/DensClsFct.h
--rw-r--r--   0        0        0      304 2023-05-30 05:36:57.530650 dimlpfidex-0.0.0/dimlp/cpp/src/DimlpBT.cpp
--rw-r--r--   0        0        0    19898 2023-07-12 08:41:26.246594 dimlpfidex-0.0.0/dimlp/cpp/src/DimlpBTFct.cpp
--rw-r--r--   0        0        0      305 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/DimlpBTFct.h
--rw-r--r--   0        0        0      307 2023-05-30 05:36:57.530650 dimlpfidex-0.0.0/dimlp/cpp/src/DimlpCls.cpp
--rw-r--r--   0        0        0    11621 2023-09-11 09:37:18.878636 dimlpfidex-0.0.0/dimlp/cpp/src/DimlpClsFct.cpp
--rw-r--r--   0        0        0      388 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/DimlpClsFct.h
--rw-r--r--   0        0        0      310 2023-05-30 05:36:57.530650 dimlpfidex-0.0.0/dimlp/cpp/src/DimlpPred.cpp
--rw-r--r--   0        0        0     8835 2023-09-11 09:37:18.878636 dimlpfidex-0.0.0/dimlp/cpp/src/DimlpPredFct.cpp
--rw-r--r--   0        0        0      387 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/DimlpPredFct.h
--rw-r--r--   0        0        0      306 2023-05-30 05:36:57.530650 dimlpfidex-0.0.0/dimlp/cpp/src/DimlpRul.cpp
--rw-r--r--   0        0        0    14752 2023-09-11 09:37:18.878636 dimlpfidex-0.0.0/dimlp/cpp/src/DimlpRulFct.cpp
--rw-r--r--   0        0        0      306 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/DimlpRulFct.h
--rw-r--r--   0        0        0      307 2023-05-30 05:36:57.530650 dimlpfidex-0.0.0/dimlp/cpp/src/DimlpTrn.cpp
--rw-r--r--   0        0        0    20726 2023-09-11 09:37:18.878636 dimlpfidex-0.0.0/dimlp/cpp/src/DimlpTrnFct.cpp
--rw-r--r--   0        0        0      463 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/DimlpTrnFct.h
--rw-r--r--   0        0        0      262 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/ante.cpp
--rw-r--r--   0        0        0      493 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/ante.h
--rw-r--r--   0        0        0     1636 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/attrName.cpp
--rw-r--r--   0        0        0      664 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/attrName.h
--rw-r--r--   0        0        0     8373 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/bagDimlp.cpp
--rw-r--r--   0        0        0     2018 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/bagDimlp.h
--rw-r--r--   0        0        0    23513 2023-07-06 07:51:52.054009 dimlpfidex-0.0.0/dimlp/cpp/src/bpNN.cpp
--rw-r--r--   0        0        0     4712 2023-07-06 07:51:52.054009 dimlpfidex-0.0.0/dimlp/cpp/src/bpNN.h
--rw-r--r--   0        0        0     1182 2023-05-30 05:36:57.530650 dimlpfidex-0.0.0/dimlp/cpp/src/checkFun.cpp
--rw-r--r--   0        0        0      111 2023-07-06 07:51:52.054009 dimlpfidex-0.0.0/dimlp/cpp/src/checkFun.h
--rw-r--r--   0        0        0    43712 2023-09-11 09:37:18.878636 dimlpfidex-0.0.0/dimlp/cpp/src/cleanRS.cpp
--rw-r--r--   0        0        0     3958 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/cleanRS.h
--rw-r--r--   0        0        0     6572 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/dataSet.cpp
--rw-r--r--   0        0        0     1430 2023-07-06 07:51:52.054009 dimlpfidex-0.0.0/dimlp/cpp/src/dataSet.h
--rw-r--r--   0        0        0     2033 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/dimlp.cpp
--rw-r--r--   0        0        0     1554 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/dimlp.h
--rw-r--r--   0        0        0      384 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/errFunct.cpp
--rw-r--r--   0        0        0      143 2023-07-06 07:51:52.054009 dimlpfidex-0.0.0/dimlp/cpp/src/errFunct.h
--rw-r--r--   0        0        0     9672 2023-07-06 07:51:52.054009 dimlpfidex-0.0.0/dimlp/cpp/src/layer.cpp
--rw-r--r--   0        0        0     3169 2023-07-06 07:51:52.054009 dimlpfidex-0.0.0/dimlp/cpp/src/layer.h
--rw-r--r--   0        0        0      490 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/layerD2.cpp
--rw-r--r--   0        0        0      894 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/layerD2.h
--rw-r--r--   0        0        0      490 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/layerD3.cpp
--rw-r--r--   0        0        0      884 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/layerD3.h
--rw-r--r--   0        0        0      490 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/layerD4.cpp
--rw-r--r--   0        0        0      868 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/layerD4.h
--rw-r--r--   0        0        0      489 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/layerDmp.cpp
--rw-r--r--   0        0        0      835 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/layerDmp.h
--rw-r--r--   0        0        0      407 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/layerFdp.cpp
--rw-r--r--   0        0        0      838 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/layerFdp.h
--rw-r--r--   0        0        0      763 2023-07-06 07:51:52.054009 dimlpfidex-0.0.0/dimlp/cpp/src/layerRad.h
--rw-r--r--   0        0        0      664 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/layerSD.h
--rw-r--r--   0        0        0      666 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/layerSP3.h
--rw-r--r--   0        0        0      666 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/layerSP4.h
--rw-r--r--   0        0        0      666 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/layerSP5.h
--rw-r--r--   0        0        0      839 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/misc.cpp
--rw-r--r--   0        0        0      205 2023-07-06 07:51:52.054009 dimlpfidex-0.0.0/dimlp/cpp/src/misc.h
--rw-r--r--   0        0        0     1551 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/oneVarTD.cpp
--rw-r--r--   0        0        0     1263 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/oneVarTD.h
--rw-r--r--   0        0        0     2471 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/randFun.cpp
--rw-r--r--   0        0        0      814 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/randFun.h
--rw-r--r--   0        0        0    21715 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/realHyp.cpp
--rw-r--r--   0        0        0     3719 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/realHyp.h
--rw-r--r--   0        0        0      954 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/realHyp2.cpp
--rw-r--r--   0        0        0     1012 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/realHyp2.h
--rw-r--r--   0        0        0     1413 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/rule.cpp
--rw-r--r--   0        0        0     1283 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/rule.h
--rw-r--r--   0        0        0    14851 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/rulePro.cpp
--rw-r--r--   0        0        0     2030 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/rulePro.h
--rw-r--r--   0        0        0     1220 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/stairObj.cpp
--rw-r--r--   0        0        0      904 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/stairObj.h
--rw-r--r--   0        0        0     1092 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/standAct.cpp
--rw-r--r--   0        0        0      216 2023-07-06 07:51:52.054009 dimlpfidex-0.0.0/dimlp/cpp/src/standAct.h
--rw-r--r--   0        0        0     1629 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/stringI.cpp
--rw-r--r--   0        0        0      890 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/stringI.h
--rw-r--r--   0        0        0      673 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/thresD.cpp
--rw-r--r--   0        0        0      650 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/thresD.h
--rw-r--r--   0        0        0     1370 2023-07-06 07:51:52.054009 dimlpfidex-0.0.0/dimlp/cpp/src/vectWRV.cpp
--rw-r--r--   0        0        0      402 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/vectWRV.h
--rw-r--r--   0        0        0     4689 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/virtHyp.cpp
--rw-r--r--   0        0        0     1252 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/cpp/src/virtHyp.h
--rw-r--r--   0        0        0      299 2023-05-30 05:36:57.530650 dimlpfidex-0.0.0/dimlp/cpp/src/writeErr.cpp
--rw-r--r--   0        0        0      164 2023-05-30 05:36:57.530650 dimlpfidex-0.0.0/dimlp/cpp/src/writeErr.h
--rw-r--r--   0        0        0   152823 2023-09-11 09:37:18.878636 dimlpfidex-0.0.0/dimlp/crossValid.py
--rw-r--r--   0        0        0    26918 2023-09-11 09:37:18.878636 dimlpfidex-0.0.0/dimlp/crossValidDimlpRul.py
--rw-r--r--   0        0        0    15226 2023-09-13 14:13:35.009351 dimlpfidex-0.0.0/dimlp/gradBoostTrn.py
--rw-r--r--   0        0        0    18977 2023-09-13 14:13:35.009351 dimlpfidex-0.0.0/dimlp/mlpTrn.py
--rw-r--r--   0        0        0     1454 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/dimlp/pybind/bindings.cpp
--rw-r--r--   0        0        0    14051 2023-09-13 14:13:35.009351 dimlpfidex-0.0.0/dimlp/randForestsTrn.py
--rw-r--r--   0        0        0     1576 2023-06-21 09:38:17.727787 dimlpfidex-0.0.0/dimlp/stairObj.py
--rw-r--r--   0        0        0    13269 2023-09-13 14:13:35.009351 dimlpfidex-0.0.0/dimlp/svmTrn.py
--rw-r--r--   0        0        0    13225 2023-09-13 14:13:35.009351 dimlpfidex-0.0.0/dimlp/trnFun.py
--rw-r--r--   0        0        0     2729 2023-05-10 13:50:30.097943 dimlpfidex-0.0.0/example/CMakeLists.txt
--rw-r--r--   0        0        0        0 2023-04-26 12:26:01.495054 dimlpfidex-0.0.0/example/__init__.py
--rw-r--r--   0        0        0      584 2023-05-10 13:50:30.097943 dimlpfidex-0.0.0/example/cpp/CMakeLists.txt
--rw-r--r--   0        0        0       81 2023-04-21 15:37:02.998085 dimlpfidex-0.0.0/example/cpp/include/examples.hpp
--rw-r--r--   0        0        0      240 2023-05-08 12:26:01.299246 dimlpfidex-0.0.0/example/cpp/src/examples.cpp
--rw-r--r--   0        0        0      356 2023-04-21 15:37:02.998085 dimlpfidex-0.0.0/example/pybind/bindings.cpp
--rw-r--r--   0        0        0     2673 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/fidex/CMakeLists.txt
--rw-r--r--   0        0        0        0 2023-05-08 12:26:01.299246 dimlpfidex-0.0.0/fidex/__init__.py
--rw-r--r--   0        0        0      682 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/fidex/cpp/CMakeLists.txt
--rw-r--r--   0        0        0      298 2023-05-30 05:36:57.540650 dimlpfidex-0.0.0/fidex/cpp/src/fidex.cpp
--rw-r--r--   0        0        0    40066 2023-09-11 09:37:18.878636 dimlpfidex-0.0.0/fidex/cpp/src/fidexFct.cpp
--rw-r--r--   0        0        0      566 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/fidex/cpp/src/fidexFct.h
--rw-r--r--   0        0        0     3530 2023-06-21 09:38:17.727787 dimlpfidex-0.0.0/fidex/cpp/src/hyperspace.cpp
--rw-r--r--   0        0        0     1268 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/fidex/cpp/src/hyperspace.h
--rw-r--r--   0        0        0      287 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/fidex/pybind/bindings.cpp
--rw-r--r--   0        0        0     2739 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/fidexGlo/CMakeLists.txt
--rw-r--r--   0        0        0        0 2023-05-08 12:26:01.299246 dimlpfidex-0.0.0/fidexGlo/__init__.py
--rw-r--r--   0        0        0     2014 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/fidexGlo/cpp/CMakeLists.txt
--rw-r--r--   0        0        0     5989 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/fidexGlo/cpp/src/checkCovSize.cpp
--rw-r--r--   0        0        0     7164 2023-09-11 09:37:18.878636 dimlpfidex-0.0.0/fidexGlo/cpp/src/fidexAlgo.cpp
--rw-r--r--   0        0        0      921 2023-09-11 09:37:18.878636 dimlpfidex-0.0.0/fidexGlo/cpp/src/fidexAlgo.h
--rw-r--r--   0        0        0      307 2023-05-30 05:36:57.540650 dimlpfidex-0.0.0/fidexGlo/cpp/src/fidexGlo.cpp
--rw-r--r--   0        0        0    17011 2023-07-06 07:51:52.054009 dimlpfidex-0.0.0/fidexGlo/cpp/src/fidexGloFct.cpp
--rw-r--r--   0        0        0      415 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/fidexGlo/cpp/src/fidexGloFct.h
--rw-r--r--   0        0        0      322 2023-05-30 05:36:57.540650 dimlpfidex-0.0.0/fidexGlo/cpp/src/fidexGloRules.cpp
--rw-r--r--   0        0        0    34697 2023-09-26 08:51:57.599279 dimlpfidex-0.0.0/fidexGlo/cpp/src/fidexGloRulesFct.cpp
--rw-r--r--   0        0        0      518 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/fidexGlo/cpp/src/fidexGloRulesFct.h
--rw-r--r--   0        0        0      322 2023-05-30 05:36:57.540650 dimlpfidex-0.0.0/fidexGlo/cpp/src/fidexGloStats.cpp
--rw-r--r--   0        0        0    16018 2023-09-11 09:37:18.878636 dimlpfidex-0.0.0/fidexGlo/cpp/src/fidexGloStatsFct.cpp
--rw-r--r--   0        0        0      394 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/fidexGlo/cpp/src/fidexGloStatsFct.h
--rw-r--r--   0        0        0     7703 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/fidexGlo/cpp/src/getRulesFun.cpp
--rw-r--r--   0        0        0      759 2023-07-06 07:51:52.054009 dimlpfidex-0.0.0/fidexGlo/cpp/src/getRulesFun.h
--rw-r--r--   0        0        0     2813 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/fidexGlo/cpp/src/hyperspace.cpp
--rw-r--r--   0        0        0     1152 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/fidexGlo/cpp/src/hyperspace.h
--rw-r--r--   0        0        0      595 2023-06-20 06:07:51.732437 dimlpfidex-0.0.0/fidexGlo/pybind/bindings.cpp
--rw-r--r--   0        0        0     3053 2023-09-13 14:13:35.009351 dimlpfidex-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     3655 1970-01-01 00:00:00.000000 dimlpfidex-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0       56 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/.clang-format
+-rw-r--r--   0        0        0      287 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/.editorconfig
+-rw-r--r--   0        0        0     1353 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0     3404 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/.github/workflows/package.yml
+-rw-r--r--   0        0        0     1621 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/.github/workflows/sonar.yml
+-rw-r--r--   0        0        0     2321 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/.gitignore
+-rw-r--r--   0        0        0      127 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/.gitmodules
+-rw-r--r--   0        0        0      425 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/.python-version
+-rw-r--r--   0        0        0      554 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/CMakeLists.txt
+-rw-r--r--   0        0        0     2680 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/LICENSE
+-rw-r--r--   0        0        0     3296 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/README.md
+-rw-r--r--   0        0        0     1105 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/RELEASE.md
+-rw-r--r--   0        0        0      618 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/Untitled.ipynb
+-rw-r--r--   0        0        0     1452 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/common/CMakeLists.txt
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/common/__init__.py
+-rw-r--r--   0        0        0      604 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/common/cpp/CMakeLists.txt
+-rw-r--r--   0        0        0      865 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/common/cpp/src/antecedant.cpp
+-rw-r--r--   0        0        0     2200 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/common/cpp/src/antecedant.h
+-rw-r--r--   0        0        0    16778 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/common/cpp/src/checkFun.cpp
+-rw-r--r--   0        0        0     1359 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/common/cpp/src/checkFun.h
+-rw-r--r--   0        0        0    38380 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/common/cpp/src/dataSet.cpp
+-rw-r--r--   0        0        0     3229 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/common/cpp/src/dataSet.h
+-rw-r--r--   0        0        0     2636 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/common/cpp/src/errorHandler.h
+-rw-r--r--   0        0        0    30420 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/common/cpp/src/parameters.cpp
+-rw-r--r--   0        0        0    12232 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/common/cpp/src/parameters.h
+-rw-r--r--   0        0        0    23269 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/common/cpp/src/rule.cpp
+-rw-r--r--   0        0        0     4694 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/common/cpp/src/rule.h
+-rw-r--r--   0        0        0     1629 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/common/cpp/src/stringI.cpp
+-rw-r--r--   0        0        0      890 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/common/cpp/src/stringI.h
+-rw-r--r--   0        0        0      776 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/config.json
+-rw-r--r--   0        0        0     2878 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/CMakeLists.txt
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/__init__.py
+-rw-r--r--   0        0        0     5637 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/CMakeLists.txt
+-rw-r--r--   0        0        0      277 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/ante.cpp
+-rw-r--r--   0        0        0      523 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/ante.h
+-rw-r--r--   0        0        0     2587 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/attrName.cpp
+-rw-r--r--   0        0        0      745 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/attrName.h
+-rw-r--r--   0        0        0     8584 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/bagDimlp.cpp
+-rw-r--r--   0        0        0     2063 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/bagDimlp.h
+-rw-r--r--   0        0        0    26422 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/bpNN.cpp
+-rw-r--r--   0        0        0     4817 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/bpNN.h
+-rw-r--r--   0        0        0    46223 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/cleanRS.cpp
+-rw-r--r--   0        0        0     4176 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/cleanRS.h
+-rw-r--r--   0        0        0    12071 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/dataSet.cpp
+-rw-r--r--   0        0        0     1702 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/dataSet.h
+-rw-r--r--   0        0        0      297 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/densCls.cpp
+-rw-r--r--   0        0        0    18642 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/densClsFct.cpp
+-rw-r--r--   0        0        0      392 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/densClsFct.h
+-rw-r--r--   0        0        0     2097 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/dimlp.cpp
+-rw-r--r--   0        0        0     1600 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/dimlp.h
+-rw-r--r--   0        0        0      297 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/dimlpBT.cpp
+-rw-r--r--   0        0        0    22373 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/dimlpBTFct.cpp
+-rw-r--r--   0        0        0      392 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/dimlpBTFct.h
+-rw-r--r--   0        0        0      299 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/dimlpCls.cpp
+-rw-r--r--   0        0        0    12804 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/dimlpClsFct.cpp
+-rw-r--r--   0        0        0      483 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/dimlpClsFct.h
+-rw-r--r--   0        0        0      301 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/dimlpPred.cpp
+-rw-r--r--   0        0        0    10161 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/dimlpPredFct.cpp
+-rw-r--r--   0        0        0      488 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/dimlpPredFct.h
+-rw-r--r--   0        0        0      298 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/dimlpRul.cpp
+-rw-r--r--   0        0        0    17732 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/dimlpRulFct.cpp
+-rw-r--r--   0        0        0      394 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/dimlpRulFct.h
+-rw-r--r--   0        0        0     1448 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/dimlpRule.cpp
+-rw-r--r--   0        0        0     1292 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/dimlpRule.h
+-rw-r--r--   0        0        0      299 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/dimlpTrn.cpp
+-rw-r--r--   0        0        0    23955 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/dimlpTrnFct.cpp
+-rw-r--r--   0        0        0      558 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/dimlpTrnFct.h
+-rw-r--r--   0        0        0      384 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/errFunct.cpp
+-rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/errFunct.h
+-rw-r--r--   0        0        0     9682 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/layer.cpp
+-rw-r--r--   0        0        0     3169 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/layer.h
+-rw-r--r--   0        0        0      490 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/layerD2.cpp
+-rw-r--r--   0        0        0      894 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/layerD2.h
+-rw-r--r--   0        0        0      490 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/layerD3.cpp
+-rw-r--r--   0        0        0      884 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/layerD3.h
+-rw-r--r--   0        0        0      490 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/layerD4.cpp
+-rw-r--r--   0        0        0      868 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/layerD4.h
+-rw-r--r--   0        0        0      489 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/layerDmp.cpp
+-rw-r--r--   0        0        0      835 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/layerDmp.h
+-rw-r--r--   0        0        0      407 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/layerFdp.cpp
+-rw-r--r--   0        0        0      838 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/layerFdp.h
+-rw-r--r--   0        0        0      763 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/layerRad.h
+-rw-r--r--   0        0        0      664 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/layerSD.h
+-rw-r--r--   0        0        0      666 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/layerSP3.h
+-rw-r--r--   0        0        0      666 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/layerSP4.h
+-rw-r--r--   0        0        0      666 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/layerSP5.h
+-rw-r--r--   0        0        0      863 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/misc.cpp
+-rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/misc.h
+-rw-r--r--   0        0        0     1551 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/oneVarTD.cpp
+-rw-r--r--   0        0        0     1287 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/oneVarTD.h
+-rw-r--r--   0        0        0     2467 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/randFun.cpp
+-rw-r--r--   0        0        0      832 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/randFun.h
+-rw-r--r--   0        0        0    22857 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/realHyp.cpp
+-rw-r--r--   0        0        0     3944 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/realHyp.h
+-rw-r--r--   0        0        0      954 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/realHyp2.cpp
+-rw-r--r--   0        0        0     1012 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/realHyp2.h
+-rw-r--r--   0        0        0    14951 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/rulePro.cpp
+-rw-r--r--   0        0        0     2055 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/rulePro.h
+-rw-r--r--   0        0        0     1220 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/stairObj.cpp
+-rw-r--r--   0        0        0      904 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/stairObj.h
+-rw-r--r--   0        0        0     1092 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/standAct.cpp
+-rw-r--r--   0        0        0      216 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/standAct.h
+-rw-r--r--   0        0        0      673 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/thresD.cpp
+-rw-r--r--   0        0        0      650 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/thresD.h
+-rw-r--r--   0        0        0     1370 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/vectWRV.cpp
+-rw-r--r--   0        0        0      426 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/vectWRV.h
+-rw-r--r--   0        0        0     4689 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/virtHyp.cpp
+-rw-r--r--   0        0        0     1252 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/cpp/src/virtHyp.h
+-rw-r--r--   0        0        0     2062 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/docs/formats.txt
+-rw-r--r--   0        0        0    10250 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/imageAnalyser.py
+-rw-r--r--   0        0        0     1640 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/pybind/bindings.cpp
+-rw-r--r--   0        0        0     1756 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/rgbToHSL.py
+-rw-r--r--   0        0        0     1759 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlp/rulesConversion.py
+-rw-r--r--   0        0        0     1832 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/.gitignore
+-rw-r--r--   0        0        0       52 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/README.md
+-rw-r--r--   0        0        0     1420 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/analysis_options.yaml
+-rw-r--r--   0        0        0     3373 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/lib/data/common_fields_data.dart
+-rw-r--r--   0        0        0     2600 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/lib/data/field.dart
+-rw-r--r--   0        0        0    63761 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/lib/data/fields_data.dart
+-rw-r--r--   0        0        0    31703 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/lib/data/params_by_program.md
+-rw-r--r--   0        0        0      109 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/lib/main.dart
+-rw-r--r--   0        0        0     3668 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/lib/ui/glossary_card.dart
+-rw-r--r--   0        0        0    16345 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/lib/ui/input_field.dart
+-rw-r--r--   0        0        0     1332 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/lib/ui/nested_tab_bar.dart
+-rw-r--r--   0        0        0     1032 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/lib/ui/simple_button.dart
+-rw-r--r--   0        0        0     4588 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/lib/views/app_view.dart
+-rw-r--r--   0        0        0     5948 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/lib/views/form_view.dart
+-rw-r--r--   0        0        0     1590 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/lib/views/glossary_view.dart
+-rw-r--r--   0        0        0     3497 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/lib/views/home_view.dart
+-rw-r--r--   0        0        0       18 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/linux/.gitignore
+-rw-r--r--   0        0        0     5441 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/linux/CMakeLists.txt
+-rw-r--r--   0        0        0     2815 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/linux/flutter/CMakeLists.txt
+-rw-r--r--   0        0        0      440 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/linux/flutter/generated_plugin_registrant.cc
+-rw-r--r--   0        0        0      303 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/linux/flutter/generated_plugin_registrant.h
+-rw-r--r--   0        0        0      761 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/linux/flutter/generated_plugins.cmake
+-rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/linux/main.cc
+-rw-r--r--   0        0        0     3726 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/linux/my_application.cc
+-rw-r--r--   0        0        0      388 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/linux/my_application.h
+-rw-r--r--   0        0        0       89 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/.gitignore
+-rw-r--r--   0        0        0       48 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/Flutter/Flutter-Debug.xcconfig
+-rw-r--r--   0        0        0       48 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/Flutter/Flutter-Release.xcconfig
+-rw-r--r--   0        0        0      384 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/Flutter/GeneratedPluginRegistrant.swift
+-rw-r--r--   0        0        0      214 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/Runner/AppDelegate.swift
+-rw-r--r--   0        0        0     1291 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/Runner/Assets.xcassets/AppIcon.appiconset/Contents.json
+-rw-r--r--   0        0        0   102994 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/Runner/Assets.xcassets/AppIcon.appiconset/app_icon_1024.png
+-rw-r--r--   0        0        0     5680 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/Runner/Assets.xcassets/AppIcon.appiconset/app_icon_128.png
+-rw-r--r--   0        0        0      520 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/Runner/Assets.xcassets/AppIcon.appiconset/app_icon_16.png
+-rw-r--r--   0        0        0    14142 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/Runner/Assets.xcassets/AppIcon.appiconset/app_icon_256.png
+-rw-r--r--   0        0        0     1066 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/Runner/Assets.xcassets/AppIcon.appiconset/app_icon_32.png
+-rw-r--r--   0        0        0    36406 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/Runner/Assets.xcassets/AppIcon.appiconset/app_icon_512.png
+-rw-r--r--   0        0        0     2218 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/Runner/Assets.xcassets/AppIcon.appiconset/app_icon_64.png
+-rw-r--r--   0        0        0    23729 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/Runner/Base.lproj/MainMenu.xib
+-rw-r--r--   0        0        0      614 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/Runner/Configs/AppInfo.xcconfig
+-rw-r--r--   0        0        0       77 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/Runner/Configs/Debug.xcconfig
+-rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/Runner/Configs/Release.xcconfig
+-rw-r--r--   0        0        0      580 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/Runner/Configs/Warnings.xcconfig
+-rw-r--r--   0        0        0      348 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/Runner/DebugProfile.entitlements
+-rw-r--r--   0        0        0     1060 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/Runner/Info.plist
+-rw-r--r--   0        0        0      388 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/Runner/MainFlutterWindow.swift
+-rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/Runner/Release.entitlements
+-rw-r--r--   0        0        0    25960 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/Runner.xcodeproj/project.pbxproj
+-rw-r--r--   0        0        0      238 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/Runner.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+-rw-r--r--   0        0        0     3679 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/Runner.xcodeproj/xcshareddata/xcschemes/Runner.xcscheme
+-rw-r--r--   0        0        0      152 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/Runner.xcworkspace/contents.xcworkspacedata
+-rw-r--r--   0        0        0      238 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/Runner.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+-rw-r--r--   0        0        0      290 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/macos/RunnerTests/RunnerTests.swift
+-rw-r--r--   0        0        0    12877 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/pubspec.lock
+-rw-r--r--   0        0        0     4010 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/pubspec.yaml
+-rw-r--r--   0        0        0     1073 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/test/widget_test.dart
+-rw-r--r--   0        0        0      917 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/web/favicon.png
+-rw-r--r--   0        0        0     5292 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/web/icons/Icon-192.png
+-rw-r--r--   0        0        0     8252 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/web/icons/Icon-512.png
+-rw-r--r--   0        0        0     5594 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/web/icons/Icon-maskable-192.png
+-rw-r--r--   0        0        0    20998 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/web/icons/Icon-maskable-512.png
+-rw-r--r--   0        0        0     1855 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/web/index.html
+-rw-r--r--   0        0        0      924 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/web/manifest.json
+-rw-r--r--   0        0        0      291 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/windows/.gitignore
+-rw-r--r--   0        0        0     4164 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/windows/CMakeLists.txt
+-rw-r--r--   0        0        0     3742 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/windows/flutter/CMakeLists.txt
+-rw-r--r--   0        0        0      328 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/windows/flutter/generated_plugin_registrant.cc
+-rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/windows/flutter/generated_plugin_registrant.h
+-rw-r--r--   0        0        0      767 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/windows/flutter/generated_plugins.cmake
+-rw-r--r--   0        0        0     1796 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/windows/runner/CMakeLists.txt
+-rw-r--r--   0        0        0     3053 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/windows/runner/Runner.rc
+-rw-r--r--   0        0        0     2122 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/windows/runner/flutter_window.cpp
+-rw-r--r--   0        0        0      928 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/windows/runner/flutter_window.h
+-rw-r--r--   0        0        0     1267 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/windows/runner/main.cpp
+-rw-r--r--   0        0        0      432 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/windows/runner/resource.h
+-rw-r--r--   0        0        0    33772 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/windows/runner/resources/app_icon.ico
+-rw-r--r--   0        0        0     1788 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/windows/runner/utils.cpp
+-rw-r--r--   0        0        0      672 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/windows/runner/utils.h
+-rw-r--r--   0        0        0     8534 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/windows/runner/win32_window.cpp
+-rw-r--r--   0        0        0     3522 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/dimlpfidex_gui/windows/runner/win32_window.h
+-rw-r--r--   0        0        0     1804 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/doc.md
+-rw-r--r--   0        0        0     2729 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/example/CMakeLists.txt
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/example/__init__.py
+-rw-r--r--   0        0        0      584 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/example/cpp/CMakeLists.txt
+-rw-r--r--   0        0        0       81 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/example/cpp/include/examples.hpp
+-rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/example/cpp/src/examples.cpp
+-rw-r--r--   0        0        0      356 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/example/pybind/bindings.cpp
+-rw-r--r--   0        0        0      368 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/example.py
+-rw-r--r--   0        0        0     2844 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/fidex/CMakeLists.txt
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/fidex/__init__.py
+-rw-r--r--   0        0        0     2843 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/fidex/cpp/CMakeLists.txt
+-rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/fidex/cpp/src/fidex.cpp
+-rw-r--r--   0        0        0    18209 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/fidex/cpp/src/fidexAlgo.cpp
+-rw-r--r--   0        0        0     2281 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/fidex/cpp/src/fidexAlgo.h
+-rw-r--r--   0        0        0    24651 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/fidex/cpp/src/fidexFct.cpp
+-rw-r--r--   0        0        0      866 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/fidex/cpp/src/fidexFct.h
+-rw-r--r--   0        0        0      299 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/fidex/cpp/src/fidexGlo.cpp
+-rw-r--r--   0        0        0    31260 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/fidex/cpp/src/fidexGloFct.cpp
+-rw-r--r--   0        0        0      907 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/fidex/cpp/src/fidexGloFct.h
+-rw-r--r--   0        0        0      309 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/fidex/cpp/src/fidexGloRules.cpp
+-rw-r--r--   0        0        0    32680 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/fidex/cpp/src/fidexGloRulesFct.cpp
+-rw-r--r--   0        0        0      639 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/fidex/cpp/src/fidexGloRulesFct.h
+-rw-r--r--   0        0        0      309 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/fidex/cpp/src/fidexGloStats.cpp
+-rw-r--r--   0        0        0    29548 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/fidex/cpp/src/fidexGloStatsFct.cpp
+-rw-r--r--   0        0        0      532 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/fidex/cpp/src/fidexGloStatsFct.h
+-rw-r--r--   0        0        0     4276 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/fidex/cpp/src/hyperLocus.cpp
+-rw-r--r--   0        0        0      565 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/fidex/cpp/src/hyperLocus.h
+-rw-r--r--   0        0        0     2190 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/fidex/cpp/src/hyperbox.cpp
+-rw-r--r--   0        0        0     1080 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/fidex/cpp/src/hyperbox.h
+-rw-r--r--   0        0        0     4428 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/fidex/cpp/src/hyperspace.cpp
+-rw-r--r--   0        0        0     1277 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/fidex/cpp/src/hyperspace.h
+-rw-r--r--   0        0        0      846 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/fidex/pybind/bindings.cpp
+-rw-r--r--   0        0        0      400 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.cirrus.yml
+-rw-r--r--   0        0        0     2442 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.clang-format
+-rw-r--r--   0        0        0     2478 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.clang-tidy
+-rw-r--r--   0        0        0       29 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.git
+-rw-r--r--   0        0        0      267 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.github/CODEOWNERS
+-rw-r--r--   0        0        0     3213 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     8210 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0       51 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.github/FUNDING.yml
+-rw-r--r--   0        0        0     3331 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.github/ISSUE_TEMPLATE/bug.yaml
+-rw-r--r--   0        0        0      188 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     2507 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      446 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.github/SECURITY.md
+-rw-r--r--   0        0        0     1123 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.github/config.yml
+-rw-r--r--   0        0        0     2985 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.github/external_ci/appveyor.yml
+-rw-r--r--   0        0        0      478 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.github/labeler.yml
+-rw-r--r--   0        0        0      691 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.github/stale.yml
+-rw-r--r--   0        0        0     2375 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.github/workflows/check_amalgamation.yml
+-rw-r--r--   0        0        0      725 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.github/workflows/cifuzz.yml
+-rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     2791 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.github/workflows/comment_check_amalgamation.yml
+-rw-r--r--   0        0        0      332 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.github/workflows/labeler.yml
+-rw-r--r--   0        0        0     1783 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.github/workflows/macos.yml
+-rw-r--r--   0        0        0     1029 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.github/workflows/publish_documentation.yml
+-rw-r--r--   0        0        0     7866 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.github/workflows/ubuntu.yml
+-rw-r--r--   0        0        0     4615 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.github/workflows/windows.yml
+-rw-r--r--   0        0        0      656 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.gitignore
+-rw-r--r--   0        0        0       77 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.lgtm.yml
+-rw-r--r--   0        0        0      275 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.reuse/README.md
+-rw-r--r--   0        0        0      830 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.reuse/dep5
+-rw-r--r--   0        0        0      349 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.reuse/templates/json.jinja2
+-rw-r--r--   0        0        0      367 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/.reuse/templates/json_support.jinja2
+-rw-r--r--   0        0        0     2634 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/BUILD.bazel
+-rw-r--r--   0        0        0      410 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/CITATION.cff
+-rw-r--r--   0        0        0     7180 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/CMakeLists.txt
+-rw-r--r--   0        0        0   304881 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/ChangeLog.md
+-rw-r--r--   0        0        0     1076 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/LICENSE.MIT
+-rw-r--r--   0        0        0    10280 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0     1460 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0        0        0    34670 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0        0        0     1078 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/LICENSES/MIT.txt
+-rw-r--r--   0        0        0      554 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/Package.swift
+-rw-r--r--   0        0        0   113396 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/README.md
+-rw-r--r--   0        0        0       34 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/WORKSPACE.bazel
+-rw-r--r--   0        0        0    45381 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/cmake/ci.cmake
+-rw-r--r--   0        0        0      710 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/cmake/config.cmake.in
+-rw-r--r--   0        0        0     3185 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/cmake/download_test_data.cmake
+-rw-r--r--   0        0        0      709 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/cmake/nlohmann_jsonConfigVersion.cmake.in
+-rw-r--r--   0        0        0      126 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/cmake/pkg-config.pc.in
+-rw-r--r--   0        0        0      543 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/cmake/scripts/gen_bazel_build_file.cmake
+-rw-r--r--   0        0        0    10468 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/cmake/test.cmake
+-rw-r--r--   0        0        0      796 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/README.md
+-rw-r--r--   0        0        0  1703752 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/avatars.png
+-rw-r--r--   0        0        0      607 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/docset/Info.plist
+-rw-r--r--   0        0        0      699 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/docset/README.md
+-rw-r--r--   0        0        0    28934 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/docset/docSet.sql
+-rw-r--r--   0        0        0      222 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/docset/docset.json
+-rw-r--r--   0        0        0      700 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/docset/icon.png
+-rw-r--r--   0        0        0     1362 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/docset/icon@2x.png
+-rw-r--r--   0        0        0      753 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/README.cpp
+-rw-r--r--   0        0        0      404 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/README.output
+-rw-r--r--   0        0        0      466 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/accept__string.cpp
+-rw-r--r--   0        0        0       11 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/accept__string.output
+-rw-r--r--   0        0        0      543 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/array.cpp
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/array.output
+-rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/array_t.cpp
+-rw-r--r--   0        0        0        5 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/array_t.output
+-rw-r--r--   0        0        0     2506 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/at__json_pointer.cpp
+-rw-r--r--   0        0        0      451 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/at__json_pointer.output
+-rw-r--r--   0        0        0     1982 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/at__json_pointer_const.cpp
+-rw-r--r--   0        0        0      351 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/at__json_pointer_const.output
+-rw-r--r--   0        0        0     1138 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/at__keytype.c++17.cpp
+-rw-r--r--   0        0        0      201 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/at__keytype.c++17.output
+-rw-r--r--   0        0        0      998 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/at__keytype_const.c++17.cpp
+-rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/at__keytype_const.c++17.output
+-rw-r--r--   0        0        0      993 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/at__object_t_key_type.cpp
+-rw-r--r--   0        0        0      201 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/at__object_t_key_type.output
+-rw-r--r--   0        0        0      873 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/at__object_t_key_type_const.cpp
+-rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/at__object_t_key_type_const.output
+-rw-r--r--   0        0        0      894 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/at__size_type.cpp
+-rw-r--r--   0        0        0      168 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/at__size_type.output
+-rw-r--r--   0        0        0      766 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/at__size_type_const.cpp
+-rw-r--r--   0        0        0      132 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/at__size_type_const.output
+-rw-r--r--   0        0        0     1055 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/back.cpp
+-rw-r--r--   0        0        0       89 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/back.output
+-rw-r--r--   0        0        0     6448 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/basic_json__CompatibleType.cpp
+-rw-r--r--   0        0        0      669 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/basic_json__CompatibleType.output
+-rw-r--r--   0        0        0      854 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/basic_json__InputIt_InputIt.cpp
+-rw-r--r--   0        0        0       98 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/basic_json__InputIt_InputIt.output
+-rw-r--r--   0        0        0      338 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/basic_json__basic_json.cpp
+-rw-r--r--   0        0        0       59 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/basic_json__basic_json.output
+-rw-r--r--   0        0        0      283 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/basic_json__copyassignment.cpp
+-rw-r--r--   0        0        0        6 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/basic_json__copyassignment.output
+-rw-r--r--   0        0        0      593 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/basic_json__list_init_t.cpp
+-rw-r--r--   0        0        0       83 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/basic_json__list_init_t.output
+-rw-r--r--   0        0        0      287 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/basic_json__moveconstructor.cpp
+-rw-r--r--   0        0        0        8 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/basic_json__moveconstructor.output
+-rw-r--r--   0        0        0      298 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/basic_json__nullptr_t.cpp
+-rw-r--r--   0        0        0       10 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/basic_json__nullptr_t.output
+-rw-r--r--   0        0        0      420 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/basic_json__size_type_basic_json.cpp
+-rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/basic_json__size_type_basic_json.output
+-rw-r--r--   0        0        0      764 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/basic_json__value_t.cpp
+-rw-r--r--   0        0        0       26 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/basic_json__value_t.output
+-rw-r--r--   0        0        0      330 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/begin.cpp
+-rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/begin.output
+-rw-r--r--   0        0        0      408 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/binary.cpp
+-rw-r--r--   0        0        0       26 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/binary.output
+-rw-r--r--   0        0        0      265 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/binary_t.cpp
+-rw-r--r--   0        0        0        5 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/binary_t.output
+-rw-r--r--   0        0        0      206 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/boolean_t.cpp
+-rw-r--r--   0        0        0        5 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/boolean_t.output
+-rw-r--r--   0        0        0      648 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/byte_container_with_subtype__byte_container_with_subtype.cpp
+-rw-r--r--   0        0        0      112 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/byte_container_with_subtype__byte_container_with_subtype.output
+-rw-r--r--   0        0        0      576 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/byte_container_with_subtype__clear_subtype.cpp
+-rw-r--r--   0        0        0      147 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/byte_container_with_subtype__clear_subtype.output
+-rw-r--r--   0        0        0      602 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/byte_container_with_subtype__has_subtype.cpp
+-rw-r--r--   0        0        0       49 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/byte_container_with_subtype__has_subtype.output
+-rw-r--r--   0        0        0      594 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/byte_container_with_subtype__set_subtype.cpp
+-rw-r--r--   0        0        0      147 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/byte_container_with_subtype__set_subtype.output
+-rw-r--r--   0        0        0      712 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/byte_container_with_subtype__subtype.cpp
+-rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/byte_container_with_subtype__subtype.output
+-rw-r--r--   0        0        0      343 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/cbegin.cpp
+-rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/cbegin.output
+-rw-r--r--   0        0        0      843 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/cbor_tag_handler_t.cpp
+-rw-r--r--   0        0        0      198 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/cbor_tag_handler_t.output
+-rw-r--r--   0        0        0      413 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/cend.cpp
+-rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/cend.output
+-rw-r--r--   0        0        0      832 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/clear.cpp
+-rw-r--r--   0        0        0       26 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/clear.output
+-rw-r--r--   0        0        0     1129 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/contains__json_pointer.cpp
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/contains__json_pointer.output
+-rw-r--r--   0        0        0      635 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/contains__keytype.c++17.cpp
+-rw-r--r--   0        0        0       95 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/contains__keytype.c++17.output
+-rw-r--r--   0        0        0      563 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/contains__object_t_key_type.cpp
+-rw-r--r--   0        0        0       95 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/contains__object_t_key_type.output
+-rw-r--r--   0        0        0      535 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/count__keytype.c++17.cpp
+-rw-r--r--   0        0        0       76 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/count__keytype.c++17.output
+-rw-r--r--   0        0        0      465 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/count__object_t_key_type.cpp
+-rw-r--r--   0        0        0       76 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/count__object_t_key_type.output
+-rw-r--r--   0        0        0      350 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/crbegin.cpp
+-rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/crbegin.output
+-rw-r--r--   0        0        0      413 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/crend.cpp
+-rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/crend.output
+-rw-r--r--   0        0        0      325 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/default_object_comparator_t.cpp
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/default_object_comparator_t.output
+-rw-r--r--   0        0        0      384 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/diagnostics_extended.cpp
+-rw-r--r--   0        0        0       90 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/diagnostics_extended.output
+-rw-r--r--   0        0        0      355 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/diagnostics_standard.cpp
+-rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/diagnostics_standard.output
+-rw-r--r--   0        0        0      741 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/diff.cpp
+-rw-r--r--   0        0        0      317 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/diff.output
+-rw-r--r--   0        0        0     1478 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/dump.cpp
+-rw-r--r--   0        0        0      467 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/dump.output
+-rw-r--r--   0        0        0      775 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/emplace.cpp
+-rw-r--r--   0        0        0       86 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/emplace.output
+-rw-r--r--   0        0        0      452 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/emplace_back.cpp
+-rw-r--r--   0        0        0       70 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/emplace_back.output
+-rw-r--r--   0        0        0      907 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/empty.cpp
+-rw-r--r--   0        0        0       51 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/empty.output
+-rw-r--r--   0        0        0      406 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/end.cpp
+-rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/end.output
+-rw-r--r--   0        0        0      862 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/erase__IteratorType.cpp
+-rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/erase__IteratorType.output
+-rw-r--r--   0        0        0      978 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/erase__IteratorType_IteratorType.cpp
+-rw-r--r--   0        0        0       39 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/erase__IteratorType_IteratorType.output
+-rw-r--r--   0        0        0      466 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/erase__keytype.c++17.cpp
+-rw-r--r--   0        0        0       14 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/erase__keytype.c++17.output
+-rw-r--r--   0        0        0      396 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/erase__object_t_key_type.cpp
+-rw-r--r--   0        0        0       14 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/erase__object_t_key_type.output
+-rw-r--r--   0        0        0      259 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/erase__size_type.cpp
+-rw-r--r--   0        0        0       12 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/erase__size_type.output
+-rw-r--r--   0        0        0      658 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/error_handler_t.cpp
+-rw-r--r--   0        0        0      166 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/error_handler_t.output
+-rw-r--r--   0        0        0      438 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/exception.cpp
+-rw-r--r--   0        0        0       90 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/exception.output
+-rw-r--r--   0        0        0      617 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/find__keytype.c++17.cpp
+-rw-r--r--   0        0        0       69 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/find__keytype.c++17.output
+-rw-r--r--   0        0        0      547 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/find__object_t_key_type.cpp
+-rw-r--r--   0        0        0       69 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/find__object_t_key_type.output
+-rw-r--r--   0        0        0      598 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/flatten.cpp
+-rw-r--r--   0        0        0      228 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/flatten.output
+-rw-r--r--   0        0        0      574 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/from_bjdata.cpp
+-rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/from_bjdata.output
+-rw-r--r--   0        0        0      635 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/from_bson.cpp
+-rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/from_bson.output
+-rw-r--r--   0        0        0      546 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/from_cbor.cpp
+-rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/from_cbor.output
+-rw-r--r--   0        0        0      664 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/from_json__default_constructible.cpp
+-rw-r--r--   0        0        0       49 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/from_json__default_constructible.output
+-rw-r--r--   0        0        0     1182 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/from_json__non_default_constructible.cpp
+-rw-r--r--   0        0        0       49 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/from_json__non_default_constructible.output
+-rw-r--r--   0        0        0      556 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/from_msgpack.cpp
+-rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/from_msgpack.output
+-rw-r--r--   0        0        0      574 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/from_ubjson.cpp
+-rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/from_ubjson.output
+-rw-r--r--   0        0        0      951 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/front.cpp
+-rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/front.output
+-rw-r--r--   0        0        0      666 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/get__PointerType.cpp
+-rw-r--r--   0        0        0       17 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/get__PointerType.output
+-rw-r--r--   0        0        0     1417 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/get__ValueType_const.cpp
+-rw-r--r--   0        0        0      157 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/get__ValueType_const.output
+-rw-r--r--   0        0        0      401 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/get_allocator.cpp
+-rw-r--r--   0        0        0       16 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/get_allocator.output
+-rw-r--r--   0        0        0      408 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/get_binary.cpp
+-rw-r--r--   0        0        0       26 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/get_binary.output
+-rw-r--r--   0        0        0      641 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/get_ptr.cpp
+-rw-r--r--   0        0        0       17 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/get_ptr.output
+-rw-r--r--   0        0        0      579 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/get_ref.cpp
+-rw-r--r--   0        0        0      100 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/get_ref.output
+-rw-r--r--   0        0        0     1362 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/get_to.cpp
+-rw-r--r--   0        0        0      157 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/get_to.output
+-rw-r--r--   0        0        0      352 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/insert.cpp
+-rw-r--r--   0        0        0       16 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/insert.output
+-rw-r--r--   0        0        0      372 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/insert__count.cpp
+-rw-r--r--   0        0        0       26 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/insert__count.output
+-rw-r--r--   0        0        0      367 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/insert__ilist.cpp
+-rw-r--r--   0        0        0       18 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/insert__ilist.output
+-rw-r--r--   0        0        0      473 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/insert__range.cpp
+-rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/insert__range.output
+-rw-r--r--   0        0        0      457 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/insert__range_object.cpp
+-rw-r--r--   0        0        0      134 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/insert__range_object.output
+-rw-r--r--   0        0        0      475 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/invalid_iterator.cpp
+-rw-r--r--   0        0        0      107 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/invalid_iterator.output
+-rw-r--r--   0        0        0      951 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/is_array.cpp
+-rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/is_array.output
+-rw-r--r--   0        0        0      961 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/is_binary.cpp
+-rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/is_binary.output
+-rw-r--r--   0        0        0      971 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/is_boolean.cpp
+-rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/is_boolean.output
+-rw-r--r--   0        0        0      991 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/is_discarded.cpp
+-rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/is_discarded.output
+-rw-r--r--   0        0        0      941 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/is_null.cpp
+-rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/is_null.output
+-rw-r--r--   0        0        0      961 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/is_number.cpp
+-rw-r--r--   0        0        0       51 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/is_number.output
+-rw-r--r--   0        0        0     1021 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/is_number_float.cpp
+-rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/is_number_float.output
+-rw-r--r--   0        0        0     1041 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/is_number_integer.cpp
+-rw-r--r--   0        0        0       52 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/is_number_integer.output
+-rw-r--r--   0        0        0     1051 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/is_number_unsigned.cpp
+-rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/is_number_unsigned.output
+-rw-r--r--   0        0        0      961 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/is_object.cpp
+-rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/is_object.output
+-rw-r--r--   0        0        0      991 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/is_primitive.cpp
+-rw-r--r--   0        0        0       47 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/is_primitive.output
+-rw-r--r--   0        0        0      961 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/is_string.cpp
+-rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/is_string.output
+-rw-r--r--   0        0        0     1001 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/is_structured.cpp
+-rw-r--r--   0        0        0       52 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/is_structured.output
+-rw-r--r--   0        0        0      514 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/items.cpp
+-rw-r--r--   0        0        0      124 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/items.output
+-rw-r--r--   0        0        0     2235 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_base_class_t.cpp
+-rw-r--r--   0        0        0      157 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_base_class_t.output
+-rw-r--r--   0        0        0      569 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_lines.cpp
+-rw-r--r--   0        0        0      215 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_lines.output
+-rw-r--r--   0        0        0     1056 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer.cpp
+-rw-r--r--   0        0        0      314 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer.output
+-rw-r--r--   0        0        0      421 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__back.cpp
+-rw-r--r--   0        0        0       80 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__back.output
+-rw-r--r--   0        0        0      579 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__empty.cpp
+-rw-r--r--   0        0        0       48 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__empty.output
+-rw-r--r--   0        0        0      645 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__operator__equal.cpp
+-rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__operator__equal.output
+-rw-r--r--   0        0        0      917 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__operator__equal_stringtype.cpp
+-rw-r--r--   0        0        0      184 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__operator__equal_stringtype.output
+-rw-r--r--   0        0        0      645 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__operator__notequal.cpp
+-rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__operator__notequal.output
+-rw-r--r--   0        0        0      896 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__operator__notequal_stringtype.cpp
+-rw-r--r--   0        0        0      187 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__operator__notequal_stringtype.output
+-rw-r--r--   0        0        0      491 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__operator_add.cpp
+-rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__operator_add.output
+-rw-r--r--   0        0        0      421 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__operator_add_binary.cpp
+-rw-r--r--   0        0        0       36 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__operator_add_binary.output
+-rw-r--r--   0        0        0      339 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__operator_string_t.cpp
+-rw-r--r--   0        0        0       13 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__operator_string_t.output
+-rw-r--r--   0        0        0      576 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__parent_pointer.cpp
+-rw-r--r--   0        0        0       71 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__parent_pointer.output
+-rw-r--r--   0        0        0      418 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__pop_back.cpp
+-rw-r--r--   0        0        0       36 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__pop_back.output
+-rw-r--r--   0        0        0      419 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__push_back.cpp
+-rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__push_back.output
+-rw-r--r--   0        0        0      303 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__string_t.cpp
+-rw-r--r--   0        0        0       23 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__string_t.output
+-rw-r--r--   0        0        0     1210 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__to_string.cpp
+-rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/json_pointer__to_string.output
+-rw-r--r--   0        0        0      707 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/max_size.cpp
+-rw-r--r--   0        0        0       48 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/max_size.output
+-rw-r--r--   0        0        0     1031 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/merge_patch.cpp
+-rw-r--r--   0        0        0      196 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/merge_patch.output
+-rw-r--r--   0        0        0      188 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/meta.cpp
+-rw-r--r--   0        0        0      373 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/meta.output
+-rw-r--r--   0        0        0     1696 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_define_type_intrusive_explicit.cpp
+-rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_define_type_intrusive_explicit.output
+-rw-r--r--   0        0        0     1203 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_define_type_intrusive_macro.cpp
+-rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_define_type_intrusive_macro.output
+-rw-r--r--   0        0        0      919 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_define_type_intrusive_only_serialize_explicit.cpp
+-rw-r--r--   0        0        0       82 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_define_type_intrusive_only_serialize_explicit.output
+-rw-r--r--   0        0        0      710 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_define_type_intrusive_only_serialize_macro.cpp
+-rw-r--r--   0        0        0       82 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_define_type_intrusive_only_serialize_macro.output
+-rw-r--r--   0        0        0     1755 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_define_type_intrusive_with_default_explicit.cpp
+-rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_define_type_intrusive_with_default_explicit.output
+-rw-r--r--   0        0        0     1126 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_define_type_intrusive_with_default_macro.cpp
+-rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_define_type_intrusive_with_default_macro.output
+-rw-r--r--   0        0        0     1412 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_define_type_non_intrusive_explicit.cpp
+-rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_define_type_non_intrusive_explicit.output
+-rw-r--r--   0        0        0      981 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_define_type_non_intrusive_macro.cpp
+-rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_define_type_non_intrusive_macro.output
+-rw-r--r--   0        0        0      660 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_define_type_non_intrusive_only_serialize_explicit.cpp
+-rw-r--r--   0        0        0       82 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_define_type_non_intrusive_only_serialize_explicit.output
+-rw-r--r--   0        0        0      497 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_define_type_non_intrusive_only_serialize_macro.cpp
+-rw-r--r--   0        0        0       82 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_define_type_non_intrusive_only_serialize_macro.output
+-rw-r--r--   0        0        0     1669 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_define_type_non_intrusive_with_default_explicit.cpp
+-rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_define_type_non_intrusive_with_default_explicit.output
+-rw-r--r--   0        0        0     1106 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_define_type_non_intrusive_with_default_macro.cpp
+-rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_define_type_non_intrusive_with_default_macro.output
+-rw-r--r--   0        0        0      353 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_json_namespace.cpp
+-rw-r--r--   0        0        0       27 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_json_namespace.output
+-rw-r--r--   0        0        0      687 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_json_namespace_begin.c++17.cpp
+-rw-r--r--   0        0        0        9 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_json_namespace_begin.c++17.output
+-rw-r--r--   0        0        0      284 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_json_namespace_no_version.cpp
+-rw-r--r--   0        0        0       19 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_json_namespace_no_version.output
+-rw-r--r--   0        0        0     1486 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_json_serialize_enum.cpp
+-rw-r--r--   0        0        0      103 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_json_serialize_enum.output
+-rw-r--r--   0        0        0      810 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_json_serialize_enum_2.cpp
+-rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_json_serialize_enum_2.output
+-rw-r--r--   0        0        0      306 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_json_version.cpp
+-rw-r--r--   0        0        0       35 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/nlohmann_json_version.output
+-rw-r--r--   0        0        0      213 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/number_float_t.cpp
+-rw-r--r--   0        0        0        5 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/number_float_t.output
+-rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/number_integer_t.cpp
+-rw-r--r--   0        0        0        5 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/number_integer_t.output
+-rw-r--r--   0        0        0      223 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/number_unsigned_t.cpp
+-rw-r--r--   0        0        0        5 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/number_unsigned_t.output
+-rw-r--r--   0        0        0      707 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/object.cpp
+-rw-r--r--   0        0        0       99 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/object.output
+-rw-r--r--   0        0        0      377 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/object_comparator_t.cpp
+-rw-r--r--   0        0        0       98 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/object_comparator_t.output
+-rw-r--r--   0        0        0      231 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/object_t.cpp
+-rw-r--r--   0        0        0        5 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/object_t.output
+-rw-r--r--   0        0        0     1431 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator__ValueType.cpp
+-rw-r--r--   0        0        0      225 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator__ValueType.output
+-rw-r--r--   0        0        0      827 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator__equal.cpp
+-rw-r--r--   0        0        0      106 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator__equal.output
+-rw-r--r--   0        0        0      698 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator__equal__nullptr_t.cpp
+-rw-r--r--   0        0        0      124 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator__equal__nullptr_t.output
+-rw-r--r--   0        0        0      474 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator__equal__specializations.cpp
+-rw-r--r--   0        0        0       11 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator__equal__specializations.output
+-rw-r--r--   0        0        0      817 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator__greater.cpp
+-rw-r--r--   0        0        0      115 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator__greater.output
+-rw-r--r--   0        0        0      825 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator__greaterequal.cpp
+-rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator__greaterequal.output
+-rw-r--r--   0        0        0      821 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator__less.cpp
+-rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator__less.output
+-rw-r--r--   0        0        0      825 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator__lessequal.cpp
+-rw-r--r--   0        0        0      117 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator__lessequal.output
+-rw-r--r--   0        0        0      827 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator__notequal.cpp
+-rw-r--r--   0        0        0      106 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator__notequal.output
+-rw-r--r--   0        0        0      698 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator__notequal__nullptr_t.cpp
+-rw-r--r--   0        0        0      121 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator__notequal__nullptr_t.output
+-rw-r--r--   0        0        0     1361 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator__value_t.cpp
+-rw-r--r--   0        0        0       40 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator__value_t.output
+-rw-r--r--   0        0        0     1366 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_array__json_pointer.cpp
+-rw-r--r--   0        0        0      122 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_array__json_pointer.output
+-rw-r--r--   0        0        0      684 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_array__json_pointer_const.cpp
+-rw-r--r--   0        0        0       16 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_array__json_pointer_const.output
+-rw-r--r--   0        0        0      734 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_array__keytype.c++17.cpp
+-rw-r--r--   0        0        0      194 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_array__keytype.c++17.output
+-rw-r--r--   0        0        0      353 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_array__keytype_const.c++17.cpp
+-rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_array__keytype_const.c++17.output
+-rw-r--r--   0        0        0      656 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_array__object_t_key_type.cpp
+-rw-r--r--   0        0        0      194 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_array__object_t_key_type.output
+-rw-r--r--   0        0        0      285 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_array__object_t_key_type_const.cpp
+-rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_array__object_t_key_type_const.output
+-rw-r--r--   0        0        0      483 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_array__size_type.cpp
+-rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_array__size_type.output
+-rw-r--r--   0        0        0      268 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_array__size_type_const.cpp
+-rw-r--r--   0        0        0        8 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_array__size_type_const.output
+-rw-r--r--   0        0        0      524 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_deserialize.cpp
+-rw-r--r--   0        0        0      136 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_deserialize.output
+-rw-r--r--   0        0        0      254 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_literal_json.cpp
+-rw-r--r--   0        0        0       39 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_literal_json.output
+-rw-r--r--   0        0        0      297 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_literal_json_pointer.cpp
+-rw-r--r--   0        0        0        8 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_literal_json_pointer.output
+-rw-r--r--   0        0        0      549 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_ltlt__basic_json.cpp
+-rw-r--r--   0        0        0      121 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_ltlt__basic_json.output
+-rw-r--r--   0        0        0      246 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_ltlt__json_pointer.cpp
+-rw-r--r--   0        0        0       13 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_ltlt__json_pointer.output
+-rw-r--r--   0        0        0     1164 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_spaceship__const_reference.c++20.cpp
+-rw-r--r--   0        0        0      141 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_spaceship__const_reference.c++20.output
+-rw-r--r--   0        0        0     1114 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_spaceship__scalartype.c++20.cpp
+-rw-r--r--   0        0        0      101 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/operator_spaceship__scalartype.c++20.output
+-rw-r--r--   0        0        0      224 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/ordered_json.cpp
+-rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/ordered_json.output
+-rw-r--r--   0        0        0     1109 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/ordered_map.cpp
+-rw-r--r--   0        0        0      172 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/ordered_map.output
+-rw-r--r--   0        0        0      705 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/other_error.cpp
+-rw-r--r--   0        0        0      140 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/other_error.output
+-rw-r--r--   0        0        0      418 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/out_of_range.cpp
+-rw-r--r--   0        0        0       91 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/out_of_range.output
+-rw-r--r--   0        0        0      668 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/parse__allow_exceptions.cpp
+-rw-r--r--   0        0        0      257 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/parse__allow_exceptions.output
+-rw-r--r--   0        0        0      678 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/parse__array__parser_callback_t.cpp
+-rw-r--r--   0        0        0      382 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/parse__array__parser_callback_t.output
+-rw-r--r--   0        0        0      363 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/parse__contiguouscontainer__parser_callback_t.cpp
+-rw-r--r--   0        0        0       25 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/parse__contiguouscontainer__parser_callback_t.output
+-rw-r--r--   0        0        0     1354 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/parse__istream__parser_callback_t.cpp
+-rw-r--r--   0        0        0      616 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/parse__istream__parser_callback_t.output
+-rw-r--r--   0        0        0      423 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/parse__iterator_pair.cpp
+-rw-r--r--   0        0        0       89 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/parse__iterator_pair.link
+-rw-r--r--   0        0        0       25 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/parse__iterator_pair.output
+-rw-r--r--   0        0        0      360 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/parse__pointers.cpp
+-rw-r--r--   0        0        0       89 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/parse__pointers.link
+-rw-r--r--   0        0        0       25 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/parse__pointers.output
+-rw-r--r--   0        0        0     1192 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/parse__string__parser_callback_t.cpp
+-rw-r--r--   0        0        0      616 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/parse__string__parser_callback_t.output
+-rw-r--r--   0        0        0      463 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/parse_error.cpp
+-rw-r--r--   0        0        0      202 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/parse_error.output
+-rw-r--r--   0        0        0      738 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/patch.cpp
+-rw-r--r--   0        0        0       99 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/patch.output
+-rw-r--r--   0        0        0      772 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/patch_inplace.cpp
+-rw-r--r--   0        0        0      112 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/patch_inplace.output
+-rw-r--r--   0        0        0      440 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/push_back.cpp
+-rw-r--r--   0        0        0       52 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/push_back.output
+-rw-r--r--   0        0        0      611 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/push_back__initializer_list.cpp
+-rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/push_back__initializer_list.output
+-rw-r--r--   0        0        0      584 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/push_back__object_t__value.cpp
+-rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/push_back__object_t__value.output
+-rw-r--r--   0        0        0      343 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/rbegin.cpp
+-rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/rbegin.output
+-rw-r--r--   0        0        0      406 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/rend.cpp
+-rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/rend.output
+-rw-r--r--   0        0        0     3319 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/sax_parse.cpp
+-rw-r--r--   0        0        0     1030 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/sax_parse.output
+-rw-r--r--   0        0        0     2933 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/sax_parse__binary.cpp
+-rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/sax_parse__binary.output
+-rw-r--r--   0        0        0      864 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/size.cpp
+-rw-r--r--   0        0        0       18 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/size.output
+-rw-r--r--   0        0        0      803 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/std_hash.cpp
+-rw-r--r--   0        0        0      214 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/std_hash.output
+-rw-r--r--   0        0        0      382 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/std_swap.cpp
+-rw-r--r--   0        0        0       86 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/std_swap.output
+-rw-r--r--   0        0        0      212 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/string_t.cpp
+-rw-r--r--   0        0        0        5 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/string_t.output
+-rw-r--r--   0        0        0      444 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/swap__array_t.cpp
+-rw-r--r--   0        0        0       61 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/swap__array_t.output
+-rw-r--r--   0        0        0      432 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/swap__binary_t.cpp
+-rw-r--r--   0        0        0       83 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/swap__binary_t.output
+-rw-r--r--   0        0        0      494 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/swap__object_t.cpp
+-rw-r--r--   0        0        0       88 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/swap__object_t.output
+-rw-r--r--   0        0        0      372 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/swap__reference.cpp
+-rw-r--r--   0        0        0       69 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/swap__reference.output
+-rw-r--r--   0        0        0      438 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/swap__string_t.cpp
+-rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/swap__string_t.output
+-rw-r--r--   0        0        0     1481 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/to_bjdata.cpp
+-rw-r--r--   0        0        0       77 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/to_bjdata.output
+-rw-r--r--   0        0        0      507 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/to_bson.cpp
+-rw-r--r--   0        0        0      136 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/to_bson.output
+-rw-r--r--   0        0        0      507 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/to_cbor.cpp
+-rw-r--r--   0        0        0       91 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/to_cbor.output
+-rw-r--r--   0        0        0      513 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/to_json.cpp
+-rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/to_json.output
+-rw-r--r--   0        0        0      517 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/to_msgpack.cpp
+-rw-r--r--   0        0        0       91 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/to_msgpack.output
+-rw-r--r--   0        0        0      472 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/to_string.cpp
+-rw-r--r--   0        0        0       22 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/to_string.output
+-rw-r--r--   0        0        0     1481 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/to_ubjson.cpp
+-rw-r--r--   0        0        0       77 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/to_ubjson.output
+-rw-r--r--   0        0        0     1031 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/type.cpp
+-rw-r--r--   0        0        0       40 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/type.output
+-rw-r--r--   0        0        0      433 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/type_error.cpp
+-rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/type_error.output
+-rw-r--r--   0        0        0     1021 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/type_name.cpp
+-rw-r--r--   0        0        0      165 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/type_name.output
+-rw-r--r--   0        0        0      553 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/unflatten.cpp
+-rw-r--r--   0        0        0      255 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/unflatten.output
+-rw-r--r--   0        0        0      691 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/update.cpp
+-rw-r--r--   0        0        0      206 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/update.output
+-rw-r--r--   0        0        0      727 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/update__range.cpp
+-rw-r--r--   0        0        0      206 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/update__range.output
+-rw-r--r--   0        0        0      907 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/value__json_ptr.cpp
+-rw-r--r--   0        0        0       19 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/value__json_ptr.output
+-rw-r--r--   0        0        0      889 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/value__keytype.c++17.cpp
+-rw-r--r--   0        0        0       19 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/value__keytype.c++17.output
+-rw-r--r--   0        0        0      815 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/value__object_t_key_type.cpp
+-rw-r--r--   0        0        0       19 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/examples/value__object_t_key_type.output
+-rw-r--r--   0        0        0  1652796 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/json.gif
+-rw-r--r--   0        0        0     2159 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/adl_serializer/from_json.md
+-rw-r--r--   0        0        0      908 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/adl_serializer/index.md
+-rw-r--r--   0        0        0      995 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/adl_serializer/to_json.md
+-rw-r--r--   0        0        0     3174 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/accept.md
+-rw-r--r--   0        0        0     1614 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/array.md
+-rw-r--r--   0        0        0     1744 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/array_t.md
+-rw-r--r--   0        0        0     7555 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/at.md
+-rw-r--r--   0        0        0     1324 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/back.md
+-rw-r--r--   0        0        0    15491 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/basic_json.md
+-rw-r--r--   0        0        0      663 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/begin.md
+-rw-r--r--   0        0        0     1899 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/binary.md
+-rw-r--r--   0        0        0     3559 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/binary_t.md
+-rw-r--r--   0        0        0      930 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/boolean_t.md
+-rw-r--r--   0        0        0      641 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/cbegin.md
+-rw-r--r--   0        0        0      842 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/cbor_tag_handler_t.md
+-rw-r--r--   0        0        0      644 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/cend.md
+-rw-r--r--   0        0        0     1256 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/clear.md
+-rw-r--r--   0        0        0     3270 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/contains.md
+-rw-r--r--   0        0        0     1993 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/count.md
+-rw-r--r--   0        0        0      695 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/crbegin.md
+-rw-r--r--   0        0        0      802 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/crend.md
+-rw-r--r--   0        0        0      863 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/default_object_comparator_t.md
+-rw-r--r--   0        0        0     1265 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/diff.md
+-rw-r--r--   0        0        0     2609 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/dump.md
+-rw-r--r--   0        0        0     1518 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/emplace.md
+-rw-r--r--   0        0        0     1226 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/emplace_back.md
+-rw-r--r--   0        0        0     1749 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/empty.md
+-rw-r--r--   0        0        0      664 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/end.md
+-rw-r--r--   0        0        0     7465 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/erase.md
+-rw-r--r--   0        0        0      950 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/error_handler_t.md
+-rw-r--r--   0        0        0     2091 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/exception.md
+-rw-r--r--   0        0        0     2220 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/find.md
+-rw-r--r--   0        0        0     1164 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/flatten.md
+-rw-r--r--   0        0        0     2686 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/from_bjdata.md
+-rw-r--r--   0        0        0     3479 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/from_bson.md
+-rw-r--r--   0        0        0     4172 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/from_cbor.md
+-rw-r--r--   0        0        0     3824 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/from_msgpack.md
+-rw-r--r--   0        0        0     3556 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/from_ubjson.md
+-rw-r--r--   0        0        0     1310 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/front.md
+-rw-r--r--   0        0        0     4371 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/get.md
+-rw-r--r--   0        0        0      502 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/get_allocator.md
+-rw-r--r--   0        0        0      745 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/get_binary.md
+-rw-r--r--   0        0        0     1531 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/get_ptr.md
+-rw-r--r--   0        0        0     1678 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/get_ref.md
+-rw-r--r--   0        0        0     1518 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/get_to.md
+-rw-r--r--   0        0        0    16886 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/index.md
+-rw-r--r--   0        0        0      847 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/input_format_t.md
+-rw-r--r--   0        0        0     6528 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/insert.md
+-rw-r--r--   0        0        0     1719 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/invalid_iterator.md
+-rw-r--r--   0        0        0      657 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/is_array.md
+-rw-r--r--   0        0        0      664 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/is_binary.md
+-rw-r--r--   0        0        0      689 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/is_boolean.md
+-rw-r--r--   0        0        0     2004 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/is_discarded.md
+-rw-r--r--   0        0        0      662 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/is_null.md
+-rw-r--r--   0        0        0     1303 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/is_number.md
+-rw-r--r--   0        0        0     1038 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/is_number_float.md
+-rw-r--r--   0        0        0     1114 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/is_number_integer.md
+-rw-r--r--   0        0        0     1056 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/is_number_unsigned.md
+-rw-r--r--   0        0        0      664 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/is_object.md
+-rw-r--r--   0        0        0     1860 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/is_primitive.md
+-rw-r--r--   0        0        0      662 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/is_string.md
+-rw-r--r--   0        0        0     1384 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/is_structured.md
+-rw-r--r--   0        0        0     2696 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/items.md
+-rw-r--r--   0        0        0     1165 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/json_base_class_t.md
+-rw-r--r--   0        0        0      875 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/json_serializer.md
+-rw-r--r--   0        0        0     1806 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/max_size.md
+-rw-r--r--   0        0        0     1537 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/merge_patch.md
+-rw-r--r--   0        0        0     3249 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/meta.md
+-rw-r--r--   0        0        0     2931 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/number_float_t.md
+-rw-r--r--   0        0        0     3198 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/number_integer_t.md
+-rw-r--r--   0        0        0     3250 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/number_unsigned_t.md
+-rw-r--r--   0        0        0     1799 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/object.md
+-rw-r--r--   0        0        0      816 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/object_comparator_t.md
+-rw-r--r--   0        0        0     4225 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/object_t.md
+-rw-r--r--   0        0        0     3058 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/operator+=.md
+-rw-r--r--   0        0        0     1056 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/operator=.md
+-rw-r--r--   0        0        0     8075 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/operator[].md
+-rw-r--r--   0        0        0     2404 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/operator_ValueType.md
+-rw-r--r--   0        0        0     4589 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/operator_eq.md
+-rw-r--r--   0        0        0     2349 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/operator_ge.md
+-rw-r--r--   0        0        0     2290 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/operator_gt.md
+-rw-r--r--   0        0        0     2336 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/operator_le.md
+-rw-r--r--   0        0        0     2599 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/operator_lt.md
+-rw-r--r--   0        0        0     2545 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/operator_ne.md
+-rw-r--r--   0        0        0     3045 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/operator_spaceship.md
+-rw-r--r--   0        0        0     1470 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/operator_value_t.md
+-rw-r--r--   0        0        0     1697 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/other_error.md
+-rw-r--r--   0        0        0     1774 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/out_of_range.md
+-rw-r--r--   0        0        0     6308 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/parse.md
+-rw-r--r--   0        0        0     2115 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/parse_error.md
+-rw-r--r--   0        0        0      800 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/parse_event_t.md
+-rw-r--r--   0        0        0     3648 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/parser_callback_t.md
+-rw-r--r--   0        0        0     2545 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/patch.md
+-rw-r--r--   0        0        0     2575 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/patch_inplace.md
+-rw-r--r--   0        0        0     3005 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/push_back.md
+-rw-r--r--   0        0        0      726 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/rbegin.md
+-rw-r--r--   0        0        0      832 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/rend.md
+-rw-r--r--   0        0        0     3195 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/sax_parse.md
+-rw-r--r--   0        0        0     1544 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/size.md
+-rw-r--r--   0        0        0      777 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/std_hash.md
+-rw-r--r--   0        0        0      782 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/std_swap.md
+-rw-r--r--   0        0        0     2187 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/string_t.md
+-rw-r--r--   0        0        0     4902 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/swap.md
+-rw-r--r--   0        0        0     1939 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/to_bjdata.md
+-rw-r--r--   0        0        0     1301 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/to_bson.md
+-rw-r--r--   0        0        0     1480 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/to_cbor.md
+-rw-r--r--   0        0        0     1433 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/to_msgpack.md
+-rw-r--r--   0        0        0     1161 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/to_string.md
+-rw-r--r--   0        0        0     1951 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/to_ubjson.md
+-rw-r--r--   0        0        0     1412 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/type.md
+-rw-r--r--   0        0        0     1707 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/type_error.md
+-rw-r--r--   0        0        0     1604 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/type_name.md
+-rw-r--r--   0        0        0     1606 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/unflatten.md
+-rw-r--r--   0        0        0     3853 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/update.md
+-rw-r--r--   0        0        0     5167 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/value.md
+-rw-r--r--   0        0        0     2632 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/value_t.md
+-rw-r--r--   0        0        0      329 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/basic_json/~basic_json.md
+-rw-r--r--   0        0        0     1021 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/byte_container_with_subtype/byte_container_with_subtype.md
+-rw-r--r--   0        0        0      755 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/byte_container_with_subtype/clear_subtype.md
+-rw-r--r--   0        0        0      682 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/byte_container_with_subtype/has_subtype.md
+-rw-r--r--   0        0        0     1244 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/byte_container_with_subtype/index.md
+-rw-r--r--   0        0        0      767 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/byte_container_with_subtype/set_subtype.md
+-rw-r--r--   0        0        0     1002 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/byte_container_with_subtype/subtype.md
+-rw-r--r--   0        0        0      472 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json.md
+-rw-r--r--   0        0        0      644 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_pointer/back.md
+-rw-r--r--   0        0        0      636 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_pointer/empty.md
+-rw-r--r--   0        0        0     2104 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_pointer/index.md
+-rw-r--r--   0        0        0     1189 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_pointer/json_pointer.md
+-rw-r--r--   0        0        0     3365 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_pointer/operator_eq.md
+-rw-r--r--   0        0        0     3224 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_pointer/operator_ne.md
+-rw-r--r--   0        0        0     1503 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_pointer/operator_slash.md
+-rw-r--r--   0        0        0     1231 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_pointer/operator_slasheq.md
+-rw-r--r--   0        0        0      875 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_pointer/operator_string_t.md
+-rw-r--r--   0        0        0      654 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_pointer/parent_pointer.md
+-rw-r--r--   0        0        0      550 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_pointer/pop_back.md
+-rw-r--r--   0        0        0      663 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_pointer/push_back.md
+-rw-r--r--   0        0        0      576 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_pointer/string_t.md
+-rw-r--r--   0        0        0      651 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_pointer/to_string.md
+-rw-r--r--   0        0        0      557 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_sax/binary.md
+-rw-r--r--   0        0        0      485 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_sax/boolean.md
+-rw-r--r--   0        0        0      440 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_sax/end_array.md
+-rw-r--r--   0        0        0      443 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_sax/end_object.md
+-rw-r--r--   0        0        0     2081 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_sax/index.md
+-rw-r--r--   0        0        0      536 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_sax/key.md
+-rw-r--r--   0        0        0      423 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_sax/null.md
+-rw-r--r--   0        0        0      597 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_sax/number_float.md
+-rw-r--r--   0        0        0      513 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_sax/number_integer.md
+-rw-r--r--   0        0        0      534 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_sax/number_unsigned.md
+-rw-r--r--   0        0        0      784 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_sax/parse_error.md
+-rw-r--r--   0        0        0      618 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_sax/start_array.md
+-rw-r--r--   0        0        0      621 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_sax/start_object.md
+-rw-r--r--   0        0        0      541 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/json_sax/string.md
+-rw-r--r--   0        0        0     3420 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/macros/index.md
+-rw-r--r--   0        0        0     2003 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/macros/json_assert.md
+-rw-r--r--   0        0        0     2297 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/macros/json_diagnostics.md
+-rw-r--r--   0        0        0     3948 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/macros/json_disable_enum_serialization.md
+-rw-r--r--   0        0        0     1145 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/macros/json_has_cpp_11.md
+-rw-r--r--   0        0        0     1514 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/macros/json_has_filesystem.md
+-rw-r--r--   0        0        0      667 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/macros/json_has_ranges.md
+-rw-r--r--   0        0        0      701 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/macros/json_has_static_rtti.md
+-rw-r--r--   0        0        0      744 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/macros/json_has_three_way_comparison.md
+-rw-r--r--   0        0        0      739 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/macros/json_no_io.md
+-rw-r--r--   0        0        0     1085 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/macros/json_noexception.md
+-rw-r--r--   0        0        0      747 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/macros/json_skip_library_version_check.md
+-rw-r--r--   0        0        0      716 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/macros/json_skip_unsupported_compiler_check.md
+-rw-r--r--   0        0        0     2612 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/macros/json_throw_user.md
+-rw-r--r--   0        0        0     2250 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/macros/json_use_global_udls.md
+-rw-r--r--   0        0        0     1611 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/macros/json_use_implicit_conversions.md
+-rw-r--r--   0        0        0     2501 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/macros/json_use_legacy_discarded_value_comparison.md
+-rw-r--r--   0        0        0     6431 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/macros/nlohmann_define_type_intrusive.md
+-rw-r--r--   0        0        0     6534 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/macros/nlohmann_define_type_non_intrusive.md
+-rw-r--r--   0        0        0     1115 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/macros/nlohmann_json_namespace.md
+-rw-r--r--   0        0        0     1732 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/macros/nlohmann_json_namespace_begin.md
+-rw-r--r--   0        0        0     1074 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/macros/nlohmann_json_namespace_no_version.md
+-rw-r--r--   0        0        0     2730 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/macros/nlohmann_json_serialize_enum.md
+-rw-r--r--   0        0        0     1072 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/macros/nlohmann_json_version_major.md
+-rw-r--r--   0        0        0     1651 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/operator_gtgt.md
+-rw-r--r--   0        0        0     1447 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/operator_literal_json.md
+-rw-r--r--   0        0        0     1653 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/operator_literal_json_pointer.md
+-rw-r--r--   0        0        0     2868 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/operator_ltlt.md
+-rw-r--r--   0        0        0      559 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/ordered_json.md
+-rw-r--r--   0        0        0     1607 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/api/ordered_map.md
+-rw-r--r--   0        0        0      104 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/css/custom.css
+-rw-r--r--   0        0        0    11424 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/arbitrary_types.md
+-rw-r--r--   0        0        0     3766 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/assertions.md
+-rw-r--r--   0        0        0    10300 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/binary_formats/bjdata.md
+-rw-r--r--   0        0        0     4127 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/binary_formats/bson.md
+-rw-r--r--   0        0        0    10325 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/binary_formats/cbor.md
+-rw-r--r--   0        0        0     2733 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/binary_formats/index.md
+-rw-r--r--   0        0        0     7194 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/binary_formats/messagepack.md
+-rw-r--r--   0        0        0     5745 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/binary_formats/ubjson.md
+-rw-r--r--   0        0        0    11778 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/binary_values.md
+-rw-r--r--   0        0        0     2955 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/comments.md
+-rw-r--r--   0        0        0     3934 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/element_access/checked_access.md
+-rw-r--r--   0        0        0      978 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/element_access/default_value.md
+-rw-r--r--   0        0        0      275 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/element_access/index.md
+-rw-r--r--   0        0        0     5649 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/element_access/unchecked_access.md
+-rw-r--r--   0        0        0     2341 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/enum_conversion.md
+-rw-r--r--   0        0        0     4109 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/iterators.md
+-rw-r--r--   0        0        0     1033 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/json_patch.md
+-rw-r--r--   0        0        0     4288 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/json_pointer.md
+-rw-r--r--   0        0        0     9088 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/macros.md
+-rw-r--r--   0        0        0      760 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/merge_patch.md
+-rw-r--r--   0        0        0     4265 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/namespace.md
+-rw-r--r--   0        0        0     2678 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/object_order.md
+-rw-r--r--   0        0        0      159 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/parsing/index.md
+-rw-r--r--   0        0        0     1537 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/parsing/json_lines.md
+-rw-r--r--   0        0        0     3470 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/parsing/parse_exceptions.md
+-rw-r--r--   0        0        0     3778 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/parsing/parser_callbacks.md
+-rw-r--r--   0        0        0     3290 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/parsing/sax_interface.md
+-rw-r--r--   0        0        0    12701 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/types/index.md
+-rw-r--r--   0        0        0    15100 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/features/types/number_handling.md
+-rw-r--r--   0        0        0     3213 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/home/code_of_conduct.md
+-rw-r--r--   0        0        0     2485 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/home/design_goals.md
+-rw-r--r--   0        0        0    28081 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/home/exceptions.md
+-rw-r--r--   0        0        0     6853 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/home/faq.md
+-rw-r--r--   0        0        0     1984 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/home/license.md
+-rw-r--r--   0        0        0   101382 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/home/releases.md
+-rw-r--r--   0        0        0      396 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/home/sponsors.md
+-rw-r--r--   0        0        0    46039 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/images/callback_events.png
+-rw-r--r--   0        0        0    37014 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/images/json_syntax_number.png
+-rw-r--r--   0        0        0    14240 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/images/range-begin-end.svg
+-rw-r--r--   0        0        0    41277 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/images/range-rbegin-rend.svg
+-rw-r--r--   0        0        0       44 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/index.md
+-rw-r--r--   0        0        0     6497 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/integration/cmake.md
+-rw-r--r--   0        0        0      254 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/integration/conan/CMakeLists.txt
+-rw-r--r--   0        0        0       51 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/integration/conan/Conanfile.txt
+-rw-r--r--   0        0        0      139 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/integration/conan/example.cpp
+-rw-r--r--   0        0        0      174 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/integration/example.cpp
+-rw-r--r--   0        0        0      637 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/integration/index.md
+-rw-r--r--   0        0        0     8377 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/integration/migration_guide.md
+-rw-r--r--   0        0        0     9829 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/integration/package_managers.md
+-rw-r--r--   0        0        0      405 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/integration/pkg-config.md
+-rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/integration/vcpkg/CMakeLists.txt
+-rw-r--r--   0        0        0      139 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/docs/integration/vcpkg/example.cpp
+-rw-r--r--   0        0        0    15765 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/mkdocs.yml
+-rw-r--r--   0        0        0      911 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/requirements.txt
+-rwxr-xr-x   0        0        0     8453 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/mkdocs/scripts/check_structure.py
+-rwxr-xr-x   0        0        0   208669 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/usages/ios.png
+-rw-r--r--   0        0        0  1305068 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/docs/usages/macos.png
+-rw-r--r--   0        0        0     2279 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/adl_serializer.hpp
+-rw-r--r--   0        0        0     3533 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/byte_container_with_subtype.hpp
+-rw-r--r--   0        0        0     3807 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/abi_macros.hpp
+-rw-r--r--   0        0        0    18880 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/conversions/from_json.hpp
+-rw-r--r--   0        0        0    38562 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/conversions/to_chars.hpp
+-rw-r--r--   0        0        0    16274 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/conversions/to_json.hpp
+-rw-r--r--   0        0        0     9267 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/exceptions.hpp
+-rw-r--r--   0        0        0     4016 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/hash.hpp
+-rw-r--r--   0        0        0   103146 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/input/binary_reader.hpp
+-rw-r--r--   0        0        0    17402 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/input/input_adapters.hpp
+-rw-r--r--   0        0        0    21420 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/input/json_sax.hpp
+-rw-r--r--   0        0        0    54569 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/input/lexer.hpp
+-rw-r--r--   0        0        0    19661 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/input/parser.hpp
+-rw-r--r--   0        0        0      958 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/input/position_t.hpp
+-rw-r--r--   0        0        0     1071 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/iterators/internal_iterator.hpp
+-rw-r--r--   0        0        0    24046 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/iterators/iter_impl.hpp
+-rw-r--r--   0        0        0     8238 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/iterators/iteration_proxy.hpp
+-rw-r--r--   0        0        0     1757 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/iterators/iterator_traits.hpp
+-rw-r--r--   0        0        0     3861 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/iterators/json_reverse_iterator.hpp
+-rw-r--r--   0        0        0     3227 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/iterators/primitive_iterator.hpp
+-rw-r--r--   0        0        0     1178 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/json_custom_base_class.hpp
+-rw-r--r--   0        0        0    37143 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/json_pointer.hpp
+-rw-r--r--   0        0        0     1811 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/json_ref.hpp
+-rw-r--r--   0        0        0    43639 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/macro_scope.hpp
+-rw-r--r--   0        0        0     1252 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/macro_unscope.hpp
+-rw-r--r--   0        0        0      453 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/meta/call_std/begin.hpp
+-rw-r--r--   0        0        0      451 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/meta/call_std/end.hpp
+-rw-r--r--   0        0        0     5178 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/meta/cpp_future.hpp
+-rw-r--r--   0        0        0     2109 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/meta/detected.hpp
+-rw-r--r--   0        0        0      526 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/meta/identity_tag.hpp
+-rw-r--r--   0        0        0     6960 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/meta/is_sax.hpp
+-rw-r--r--   0        0        0      766 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/meta/std_fs.hpp
+-rw-r--r--   0        0        0    29454 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/meta/type_traits.hpp
+-rw-r--r--   0        0        0      597 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/meta/void_t.hpp
+-rw-r--r--   0        0        0    71152 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/output/binary_writer.hpp
+-rw-r--r--   0        0        0     4067 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/output/output_adapters.hpp
+-rw-r--r--   0        0        0    40163 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/output/serializer.hpp
+-rw-r--r--   0        0        0     5951 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/string_concat.hpp
+-rw-r--r--   0        0        0     2168 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/string_escape.hpp
+-rw-r--r--   0        0        0     4326 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/detail/value_t.hpp
+-rw-r--r--   0        0        0   198618 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/json.hpp
+-rw-r--r--   0        0        0     2541 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/json_fwd.hpp
+-rw-r--r--   0        0        0    11692 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/ordered_map.hpp
+-rw-r--r--   0        0        0    86068 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/thirdparty/hedley/hedley.hpp
+-rw-r--r--   0        0        0     5500 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/include/nlohmann/thirdparty/hedley/hedley_undef.hpp
+-rw-r--r--   0        0        0      629 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/meson.build
+-rw-r--r--   0        0        0    19578 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/nlohmann_json.natvis
+-rw-r--r--   0        0        0   919975 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/single_include/nlohmann/json.hpp
+-rw-r--r--   0        0        0     6340 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/single_include/nlohmann/json_fwd.hpp
+-rw-r--r--   0        0        0     7533 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/CMakeLists.txt
+-rw-r--r--   0        0        0     1132 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/abi/CMakeLists.txt
+-rw-r--r--   0        0        0      771 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/abi/config/CMakeLists.txt
+-rw-r--r--   0        0        0      941 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/abi/config/config.hpp
+-rw-r--r--   0        0        0     1027 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/abi/config/custom.cpp
+-rw-r--r--   0        0        0     1186 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/abi/config/default.cpp
+-rw-r--r--   0        0        0     1085 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/abi/config/noversion.cpp
+-rw-r--r--   0        0        0      695 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/abi/diag/CMakeLists.txt
+-rw-r--r--   0        0        0     1084 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/abi/diag/diag.cpp
+-rw-r--r--   0        0        0      558 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/abi/diag/diag.hpp
+-rw-r--r--   0        0        0      731 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/abi/diag/diag_off.cpp
+-rw-r--r--   0        0        0      728 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/abi/diag/diag_on.cpp
+-rw-r--r--   0        0        0   804148 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/abi/include/nlohmann/json_v3_10_5.hpp
+-rw-r--r--   0        0        0      430 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/abi/inline_ns/CMakeLists.txt
+-rw-r--r--   0        0        0     1055 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/abi/inline_ns/use_current.cpp
+-rw-r--r--   0        0        0      729 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/abi/inline_ns/use_v3_10_5.cpp
+-rw-r--r--   0        0        0      454 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/abi/main.cpp
+-rw-r--r--   0        0        0     1212 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/benchmarks/CMakeLists.txt
+-rw-r--r--   0        0        0     8179 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/benchmarks/src/benchmarks.cpp
+-rw-r--r--   0        0        0      587 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/cmake_add_subdirectory/CMakeLists.txt
+-rw-r--r--   0        0        0      727 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/cmake_add_subdirectory/project/CMakeLists.txt
+-rw-r--r--   0        0        0      416 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/cmake_add_subdirectory/project/main.cpp
+-rw-r--r--   0        0        0      682 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/cmake_fetch_content/CMakeLists.txt
+-rw-r--r--   0        0        0      677 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/cmake_fetch_content/project/CMakeLists.txt
+-rw-r--r--   0        0        0      416 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/cmake_fetch_content/project/main.cpp
+-rw-r--r--   0        0        0      688 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/cmake_fetch_content2/CMakeLists.txt
+-rw-r--r--   0        0        0      533 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/cmake_fetch_content2/project/CMakeLists.txt
+-rw-r--r--   0        0        0      416 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/cmake_fetch_content2/project/main.cpp
+-rw-r--r--   0        0        0      561 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/cmake_import/CMakeLists.txt
+-rw-r--r--   0        0        0      343 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/cmake_import/project/CMakeLists.txt
+-rw-r--r--   0        0        0      416 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/cmake_import/project/main.cpp
+-rw-r--r--   0        0        0      603 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/cmake_import_minver/CMakeLists.txt
+-rw-r--r--   0        0        0      241 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/cmake_import_minver/project/CMakeLists.txt
+-rw-r--r--   0        0        0      416 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/cmake_import_minver/project/main.cpp
+-rw-r--r--   0        0        0      657 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/cmake_target_include_directories/CMakeLists.txt
+-rw-r--r--   0        0        0      344 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/cmake_target_include_directories/project/Bar.cpp
+-rw-r--r--   0        0        0      389 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/cmake_target_include_directories/project/Bar.hpp
+-rw-r--r--   0        0        0      992 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/cmake_target_include_directories/project/CMakeLists.txt
+-rw-r--r--   0        0        0      344 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/cmake_target_include_directories/project/Foo.cpp
+-rw-r--r--   0        0        0      370 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/cmake_target_include_directories/project/Foo.hpp
+-rw-r--r--   0        0        0      416 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/cmake_target_include_directories/project/main.cpp
+-rw-r--r--   0        0        0      324 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/cuda_example/CMakeLists.txt
+-rw-r--r--   0        0        0      560 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/cuda_example/json_cuda.cu
+-rw-r--r--   0        0        0     3187 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/fuzzing.md
+-rw-r--r--   0        0        0    28144 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/reports/2016-08-29-fuzz/exec_speed.png
+-rw-r--r--   0        0        0   235588 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/reports/2016-08-29-fuzz/fuzz.tiff
+-rw-r--r--   0        0        0    26251 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/reports/2016-08-29-fuzz/high_freq.png
+-rw-r--r--   0        0        0      443 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/reports/2016-08-29-fuzz/index.html
+-rw-r--r--   0        0        0    11752 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/reports/2016-08-29-fuzz/low_freq.png
+-rw-r--r--   0        0        0      994 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/reports/2016-09-09-nativejson_benchmark/README.md
+-rw-r--r--   0        0        0    43054 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/reports/2016-09-09-nativejson_benchmark/conformance_Nlohmann (C++11).md
+-rw-r--r--   0        0        0   169617 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/reports/2016-09-09-nativejson_benchmark/conformance_overall_Result.png
+-rw-r--r--   0        0        0   196128 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/reports/2016-09-09-nativejson_benchmark/performance_Corei7-4980HQ@2.80GHz_mac64_clang7.0_1._Parse_Memory_(byte).png
+-rw-r--r--   0        0        0   149308 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/reports/2016-09-09-nativejson_benchmark/performance_Corei7-4980HQ@2.80GHz_mac64_clang7.0_1._Parse_Time_(ms).png
+-rw-r--r--   0        0        0   139615 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/reports/2016-09-09-nativejson_benchmark/performance_Corei7-4980HQ@2.80GHz_mac64_clang7.0_2._Stringify_Time_(ms).png
+-rw-r--r--   0        0        0   100027 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/reports/2016-09-09-nativejson_benchmark/performance_Corei7-4980HQ@2.80GHz_mac64_clang7.0_3._Prettify_Time_(ms).png
+-rw-r--r--   0        0        0   186055 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/reports/2016-09-09-nativejson_benchmark/performance_Corei7-4980HQ@2.80GHz_mac64_clang7.0_7._Code_size_FileSize_(byte).png
+-rw-r--r--   0        0        0    31420 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/reports/2016-10-02-fuzz/exec_speed.png
+-rw-r--r--   0        0        0   264782 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/reports/2016-10-02-fuzz/fuzz.tiff
+-rw-r--r--   0        0        0    23019 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/reports/2016-10-02-fuzz/high_freq.png
+-rw-r--r--   0        0        0      444 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/reports/2016-10-02-fuzz/index.html
+-rw-r--r--   0        0        0    14234 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/reports/2016-10-02-fuzz/low_freq.png
+-rw-r--r--   0        0        0     1060 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/fuzzer-driver_afl.cpp
+-rw-r--r--   0        0        0     2778 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/fuzzer-parse_bjdata.cpp
+-rw-r--r--   0        0        0     1929 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/fuzzer-parse_bson.cpp
+-rw-r--r--   0        0        0     1855 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/fuzzer-parse_cbor.cpp
+-rw-r--r--   0        0        0     1806 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/fuzzer-parse_json.cpp
+-rw-r--r--   0        0        0     1896 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/fuzzer-parse_msgpack.cpp
+-rw-r--r--   0        0        0     2778 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/fuzzer-parse_ubjson.cpp
+-rw-r--r--   0        0        0     1011 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/make_test_data_available.hpp
+-rw-r--r--   0        0        0     1011 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/test_utils.hpp
+-rw-r--r--   0        0        0     4744 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-32bit.cpp
+-rw-r--r--   0        0        0    12281 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-algorithms.cpp
+-rw-r--r--   0        0        0     7336 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-allocator.cpp
+-rw-r--r--   0        0        0     8149 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-alt-string.cpp
+-rw-r--r--   0        0        0     1476 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-assert_macro.cpp
+-rw-r--r--   0        0        0    10751 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-binary_formats.cpp
+-rw-r--r--   0        0        0   181011 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-bjdata.cpp
+-rw-r--r--   0        0        0    45437 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-bson.cpp
+-rw-r--r--   0        0        0     2763 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-byte_container_with_subtype.cpp
+-rw-r--r--   0        0        0    17325 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-capacity.cpp
+-rw-r--r--   0        0        0   130082 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-cbor.cpp
+-rw-r--r--   0        0        0    14545 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-class_const_iterator.cpp
+-rw-r--r--   0        0        0    17188 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-class_iterator.cpp
+-rw-r--r--   0        0        0    11097 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-class_lexer.cpp
+-rw-r--r--   0        0        0    84946 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-class_parser.cpp
+-rw-r--r--   0        0        0    30690 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-comparison.cpp
+-rw-r--r--   0        0        0     5293 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-concepts.cpp
+-rw-r--r--   0        0        0    54687 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-constructor1.cpp
+-rw-r--r--   0        0        0     4645 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-constructor2.cpp
+-rw-r--r--   0        0        0     5919 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-convenience.cpp
+-rw-r--r--   0        0        0    54637 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-conversions.cpp
+-rw-r--r--   0        0        0     9789 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-custom-base-class.cpp
+-rw-r--r--   0        0        0    44703 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-deserialization.cpp
+-rw-r--r--   0        0        0     8611 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-diagnostics.cpp
+-rw-r--r--   0        0        0     1838 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-disabled_exceptions.cpp
+-rw-r--r--   0        0        0    40061 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-element_access1.cpp
+-rw-r--r--   0        0        0    95999 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-element_access2.cpp
+-rw-r--r--   0        0        0     4134 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-hash.cpp
+-rw-r--r--   0        0        0    14131 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-inspection.cpp
+-rw-r--r--   0        0        0    36170 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-items.cpp
+-rw-r--r--   0        0        0    50621 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-iterators1.cpp
+-rw-r--r--   0        0        0    54923 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-iterators2.cpp
+-rw-r--r--   0        0        0    47997 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-json_patch.cpp
+-rw-r--r--   0        0        0    30712 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-json_pointer.cpp
+-rw-r--r--   0        0        0      795 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-large_json.cpp
+-rw-r--r--   0        0        0     7177 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-merge_patch.cpp
+-rw-r--r--   0        0        0     1120 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-meta.cpp
+-rw-r--r--   0        0        0    32426 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-modifiers.cpp
+-rw-r--r--   0        0        0    87159 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-msgpack.cpp
+-rw-r--r--   0        0        0     1740 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-no-mem-leak-on-adl-serialize.cpp
+-rw-r--r--   0        0        0     3554 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-noexcept.cpp
+-rw-r--r--   0        0        0     2338 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-ordered_json.cpp
+-rw-r--r--   0        0        0     9631 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-ordered_map.cpp
+-rw-r--r--   0        0        0    21115 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-pointer_access.cpp
+-rw-r--r--   0        0        0    10436 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-readme.cpp
+-rw-r--r--   0        0        0    14292 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-reference_access.cpp
+-rw-r--r--   0        0        0    55356 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-regression1.cpp
+-rw-r--r--   0        0        0    29577 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-regression2.cpp
+-rw-r--r--   0        0        0    11731 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-serialization.cpp
+-rw-r--r--   0        0        0   104439 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-testsuites.cpp
+-rw-r--r--   0        0        0    34466 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-to_chars.cpp
+-rw-r--r--   0        0        0     1989 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-type_traits.cpp
+-rw-r--r--   0        0        0   113692 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-ubjson.cpp
+-rw-r--r--   0        0        0     1875 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-udl.cpp
+-rw-r--r--   0        0        0    22700 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-udt.cpp
+-rw-r--r--   0        0        0    12964 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-udt_macro.cpp
+-rw-r--r--   0        0        0    26988 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-unicode1.cpp
+-rw-r--r--   0        0        0    20459 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-unicode2.cpp
+-rw-r--r--   0        0        0    10969 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-unicode3.cpp
+-rw-r--r--   0        0        0    10976 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-unicode4.cpp
+-rw-r--r--   0        0        0    10970 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-unicode5.cpp
+-rw-r--r--   0        0        0     3255 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-user_defined_input.cpp
+-rw-r--r--   0        0        0      543 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-windows_h.cpp
+-rw-r--r--   0        0        0     2469 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit-wstring.cpp
+-rw-r--r--   0        0        0      391 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/src/unit.cpp
+-rw-r--r--   0        0        0     1386 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/CMakeLists.txt
+-rw-r--r--   0        0        0     6788 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerCorpus.h
+-rw-r--r--   0        0        0     1870 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerCrossOver.cpp
+-rw-r--r--   0        0        0     2366 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerDefs.h
+-rw-r--r--   0        0        0     3499 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerDictionary.h
+-rw-r--r--   0        0        0    18124 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerDriver.cpp
+-rw-r--r--   0        0        0     2424 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerExtFunctions.def
+-rw-r--r--   0        0        0     1041 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerExtFunctions.h
+-rw-r--r--   0        0        0     1639 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerExtFunctionsDlsym.cpp
+-rw-r--r--   0        0        0     1717 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerExtFunctionsWeak.cpp
+-rw-r--r--   0        0        0     1805 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerExtFunctionsWeakAlias.cpp
+-rw-r--r--   0        0        0     6612 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerFlags.def
+-rw-r--r--   0        0        0     3230 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerIO.cpp
+-rw-r--r--   0        0        0     1777 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerIO.h
+-rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerIOPosix.cpp
+-rw-r--r--   0        0        0     7798 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerIOWindows.cpp
+-rw-r--r--   0        0        0     2685 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerInterface.h
+-rw-r--r--   0        0        0     5518 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerInternal.h
+-rw-r--r--   0        0        0    25459 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerLoop.cpp
+-rw-r--r--   0        0        0      715 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerMain.cpp
+-rw-r--r--   0        0        0     8793 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerMerge.cpp
+-rw-r--r--   0        0        0     2490 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerMerge.h
+-rw-r--r--   0        0        0    19209 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerMutate.cpp
+-rw-r--r--   0        0        0     6033 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerMutate.h
+-rw-r--r--   0        0        0     1893 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerOptions.h
+-rw-r--r--   0        0        0     1031 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerRandom.h
+-rw-r--r--   0        0        0     5553 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerSHA1.cpp
+-rw-r--r--   0        0        0      950 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerSHA1.h
+-rw-r--r--   0        0        0    12124 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerTracePC.cpp
+-rw-r--r--   0        0        0     4732 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerTracePC.h
+-rw-r--r--   0        0        0    11395 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerTraceState.cpp
+-rw-r--r--   0        0        0     6086 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerUtil.cpp
+-rw-r--r--   0        0        0     2145 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerUtil.h
+-rw-r--r--   0        0        0     5600 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerUtilDarwin.cpp
+-rw-r--r--   0        0        0      668 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerUtilLinux.cpp
+-rw-r--r--   0        0        0     3194 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerUtilPosix.cpp
+-rw-r--r--   0        0        0     5060 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerUtilWindows.cpp
+-rw-r--r--   0        0        0     2703 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/FuzzerValueBitMap.h
+-rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/README.txt
+-rw-r--r--   0        0        0    11188 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/afl/afl_driver.cpp
+-rwxr-xr-x   0        0        0      213 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/build.sh
+-rw-r--r--   0        0        0     1016 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/cxx.dict
+-rw-r--r--   0        0        0     1702 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/standalone/StandaloneFuzzTargetMain.c
+-rw-r--r--   0        0        0      607 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/AFLDriverTest.cpp
+-rw-r--r--   0        0        0      622 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/AbsNegAndConstant64Test.cpp
+-rw-r--r--   0        0        0      588 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/AbsNegAndConstantTest.cpp
+-rw-r--r--   0        0        0      527 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/AccumulateAllocationsTest.cpp
+-rw-r--r--   0        0        0      594 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/BufferOverflowOnInput.cpp
+-rw-r--r--   0        0        0     6093 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/CMakeLists.txt
+-rw-r--r--   0        0        0     2193 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/CallerCalleeTest.cpp
+-rw-r--r--   0        0        0      480 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/CounterTest.cpp
+-rw-r--r--   0        0        0     1745 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/CustomCrossOverTest.cpp
+-rw-r--r--   0        0        0      962 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/CustomMutatorTest.cpp
+-rw-r--r--   0        0        0      236 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/DSO1.cpp
+-rw-r--r--   0        0        0      236 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/DSO2.cpp
+-rw-r--r--   0        0        0      222 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/DSOTestExtra.cpp
+-rw-r--r--   0        0        0      809 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/DSOTestMain.cpp
+-rw-r--r--   0        0        0      489 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/DivTest.cpp
+-rw-r--r--   0        0        0      285 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/EmptyTest.cpp
+-rw-r--r--   0        0        0      614 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/FourIndependentBranchesTest.cpp
+-rw-r--r--   0        0        0      708 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/FullCoverageSetTest.cpp
+-rw-r--r--   0        0        0    28308 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/FuzzerUnittest.cpp
+-rw-r--r--   0        0        0      721 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/InitializeTest.cpp
+-rw-r--r--   0        0        0      371 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/LeakTest.cpp
+-rw-r--r--   0        0        0      396 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/LeakTimeoutTest.cpp
+-rw-r--r--   0        0        0      555 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/LoadTest.cpp
+-rw-r--r--   0        0        0     1008 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/MemcmpTest.cpp
+-rw-r--r--   0        0        0      415 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/NthRunCrashTest.cpp
+-rw-r--r--   0        0        0      479 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/NullDerefOnEmptyTest.cpp
+-rw-r--r--   0        0        0      652 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/NullDerefTest.cpp
+-rw-r--r--   0        0        0      694 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/OneHugeAllocTest.cpp
+-rw-r--r--   0        0        0      629 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/OutOfMemorySingleLargeMallocTest.cpp
+-rw-r--r--   0        0        0      748 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/OutOfMemoryTest.cpp
+-rw-r--r--   0        0        0      845 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/RepeatedBytesTest.cpp
+-rw-r--r--   0        0        0      517 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/RepeatedMemcmp.cpp
+-rw-r--r--   0        0        0      745 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/ShrinkControlFlowTest.cpp
+-rw-r--r--   0        0        0      610 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/ShrinkValueProfileTest.cpp
+-rw-r--r--   0        0        0      626 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/SignedIntOverflowTest.cpp
+-rw-r--r--   0        0        0     1329 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/SimpleCmpTest.cpp
+-rw-r--r--   0        0        0      751 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/SimpleDictionaryTest.cpp
+-rw-r--r--   0        0        0     1252 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/SimpleHashTest.cpp
+-rw-r--r--   0        0        0      651 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/SimpleTest.cpp
+-rw-r--r--   0        0        0      694 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/SimpleThreadedTest.cpp
+-rw-r--r--   0        0        0      470 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/SingleMemcmpTest.cpp
+-rw-r--r--   0        0        0      467 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/SingleStrcmpTest.cpp
+-rw-r--r--   0        0        0      471 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/SingleStrncmpTest.cpp
+-rw-r--r--   0        0        0      527 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/SpamyTest.cpp
+-rw-r--r--   0        0        0      850 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/StrcmpTest.cpp
+-rw-r--r--   0        0        0      566 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/StrncmpOOBTest.cpp
+-rw-r--r--   0        0        0      798 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/StrncmpTest.cpp
+-rw-r--r--   0        0        0      754 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/StrstrTest.cpp
+-rw-r--r--   0        0        0      844 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/SwapCmpTest.cpp
+-rw-r--r--   0        0        0      852 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/Switch2Test.cpp
+-rw-r--r--   0        0        0     1617 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/SwitchTest.cpp
+-rw-r--r--   0        0        0      457 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/ThreadedLeakTest.cpp
+-rw-r--r--   0        0        0      722 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/ThreadedTest.cpp
+-rw-r--r--   0        0        0      380 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/TimeoutEmptyTest.cpp
+-rw-r--r--   0        0        0      590 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/TimeoutTest.cpp
+-rw-r--r--   0        0        0      542 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/TraceMallocTest.cpp
+-rw-r--r--   0        0        0      284 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/UninstrumentedTest.cpp
+-rw-r--r--   0        0        0     1296 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/afl-driver-extra-stats.test
+-rw-r--r--   0        0        0      408 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/afl-driver-stderr.test
+-rw-r--r--   0        0        0      148 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/caller-callee.test
+-rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/coverage.test
+-rw-r--r--   0        0        0       61 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/dict1.txt
+-rw-r--r--   0        0        0      769 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/dump_coverage.test
+-rw-r--r--   0        0        0      442 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/fuzzer-customcrossover.test
+-rw-r--r--   0        0        0      181 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/fuzzer-custommutator.test
+-rw-r--r--   0        0        0      282 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/fuzzer-dict.test
+-rw-r--r--   0        0        0      680 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/fuzzer-dirs.test
+-rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/fuzzer-fdmask.test
+-rw-r--r--   0        0        0      524 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/fuzzer-finalstats.test
+-rw-r--r--   0        0        0      522 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/fuzzer-flags.test
+-rw-r--r--   0        0        0     1089 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/fuzzer-jobs.test
+-rw-r--r--   0        0        0     1949 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/fuzzer-leak.test
+-rw-r--r--   0        0        0      256 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/fuzzer-oom-with-profile.test
+-rw-r--r--   0        0        0      547 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/fuzzer-oom.test
+-rw-r--r--   0        0        0      189 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/fuzzer-printcovpcs.test
+-rw-r--r--   0        0        0      307 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/fuzzer-runs.test
+-rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/fuzzer-seed.test
+-rw-r--r--   0        0        0      307 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/fuzzer-segv.test
+-rw-r--r--   0        0        0      825 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/fuzzer-singleinputs.test
+-rw-r--r--   0        0        0      327 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/fuzzer-threaded.test
+-rw-r--r--   0        0        0      885 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/fuzzer-timeout.test
+-rw-r--r--   0        0        0     1320 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/fuzzer-traces-hooks.test
+-rw-r--r--   0        0        0      204 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/fuzzer-ubsan.test
+-rw-r--r--   0        0        0     3000 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/fuzzer.test
+-rw-r--r--   0        0        0        3 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/hi.txt
+-rw-r--r--   0        0        0     1066 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/lit.cfg
+-rw-r--r--   0        0        0      218 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/lit.site.cfg.in
+-rw-r--r--   0        0        0     1985 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/merge.test
+-rw-r--r--   0        0        0      564 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/minimize_crash.test
+-rw-r--r--   0        0        0      863 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/no-coverage/CMakeLists.txt
+-rw-r--r--   0        0        0       89 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/repeated-bytes.test
+-rw-r--r--   0        0        0      748 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/shrink.test
+-rw-r--r--   0        0        0       91 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/simple-cmp.test
+-rw-r--r--   0        0        0      218 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/standalone.test
+-rw-r--r--   0        0        0       88 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/swap-cmp.test
+-rw-r--r--   0        0        0      468 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/trace-malloc.test
+-rw-r--r--   0        0        0      394 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/ubsan/CMakeLists.txt
+-rw-r--r--   0        0        0       47 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/ulimit.test
+-rw-r--r--   0        0        0      500 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/uninstrumented/CMakeLists.txt
+-rw-r--r--   0        0        0      214 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/unit/lit.cfg
+-rw-r--r--   0        0        0      127 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/unit/lit.site.cfg.in
+-rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/value-profile-cmp.test
+-rw-r--r--   0        0        0      124 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/value-profile-cmp2.test
+-rw-r--r--   0        0        0      131 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/value-profile-cmp3.test
+-rw-r--r--   0        0        0      133 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/value-profile-cmp4.test
+-rw-r--r--   0        0        0      122 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/value-profile-div.test
+-rw-r--r--   0        0        0      153 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/value-profile-load.test
+-rw-r--r--   0        0        0      140 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/value-profile-mem.test
+-rw-r--r--   0        0        0      138 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/value-profile-set.test
+-rw-r--r--   0        0        0      140 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/value-profile-strcmp.test
+-rw-r--r--   0        0        0      140 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/value-profile-strncmp.test
+-rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/Fuzzer/test/value-profile-switch.test
+-rw-r--r--   0        0        0   321644 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/doctest/doctest.h
+-rw-r--r--   0        0        0     1789 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/doctest/doctest_compatibility.h
+-rw-r--r--   0        0        0    13352 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/fifo_map/fifo_map.hpp
+-rwxr-xr-x   0        0        0     2403 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tests/thirdparty/imapdl/filterbr.py
+-rw-r--r--   0        0        0      432 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tools/amalgamate/CHANGES.md
+-rw-r--r--   0        0        0     2373 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tools/amalgamate/README.md
+-rwxr-xr-x   0        0        0    11442 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tools/amalgamate/amalgamate.py
+-rw-r--r--   0        0        0      164 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tools/amalgamate/config_json.json
+-rw-r--r--   0        0        0      172 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tools/amalgamate/config_json_fwd.json
+-rw-r--r--   0        0        0     2759 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tools/gdb_pretty_printer/README.md
+-rw-r--r--   0        0        0     1238 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tools/gdb_pretty_printer/nlohmann-json.py
+-rw-r--r--   0        0        0      203 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tools/generate_natvis/README.md
+-rwxr-xr-x   0        0        0     1423 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tools/generate_natvis/generate_natvis.py
+-rw-r--r--   0        0        0     2258 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tools/generate_natvis/nlohmann_json.natvis.j2
+-rw-r--r--   0        0        0     1266 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tools/macro_builder/main.cpp
+-rw-r--r--   0        0        0     3930 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tools/serve_header/README.md
+-rw-r--r--   0        0        0   557446 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tools/serve_header/demo.png
+-rw-r--r--   0        0        0       28 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tools/serve_header/requirements.txt
+-rwxr-xr-x   0        0        0    14710 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tools/serve_header/serve_header.py
+-rw-r--r--   0        0        0      316 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/tools/serve_header/serve_header.yml.example
+-rw-r--r--   0        0        0      608 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/json/wsjcpp.yml
+-rw-r--r--   0        0        0     1803 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1473 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/requirements-dev.lock
+-rw-r--r--   0        0        0     1325 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/requirements.lock
+-rw-r--r--   0        0        0      495 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/sonar-project.properties
+-rw-r--r--   0        0        0     1608 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/CMakeLists.txt
+-rw-r--r--   0        0        0     1364 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/cpp/CMakeLists.txt
+-rw-r--r--   0        0        0      197 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/cpp/headers/commonTests.hpp
+-rw-r--r--   0        0        0      785 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/cpp/headers/dimlpTests.hpp
+-rw-r--r--   0        0        0      426 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/cpp/headers/fidexTests.hpp
+-rw-r--r--   0        0        0      586 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/cpp/headers/parametersTests.hpp
+-rw-r--r--   0        0        0      209 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/cpp/headers/tests.hpp
+-rw-r--r--   0        0        0     4170 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/cpp/headers/utils.hpp
+-rw-r--r--   0        0        0      343 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/cpp/src/commonTests.cpp
+-rw-r--r--   0        0        0     1333 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/cpp/src/dimlpTests.cpp
+-rw-r--r--   0        0        0     1681 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/cpp/src/fidexTests.cpp
+-rw-r--r--   0        0        0     6480 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/cpp/src/parametersTests.cpp
+-rw-r--r--   0        0        0     2223 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/cpp/src/utils.cpp
+-rw-r--r--   0        0        0      709 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/cpp/tests.cpp
+-rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/dataset/data/attributes.txt
+-rw-r--r--   0        0        0   373005 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/dataset/data/modified-data.csv
+-rw-r--r--   0        0        0      208 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/dataset/data/normalization_stats.txt
+-rw-r--r--   0        0        0   263639 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/dataset/data/original-data.csv
+-rw-r--r--   0        0        0    32448 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/dataset/data/test.txt
+-rw-r--r--   0        0        0     5908 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/dataset/data/test_true_classes.txt
+-rw-r--r--   0        0        0   280774 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/dataset/data/train.txt
+-rw-r--r--   0        0        0    53172 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/dataset/data/train_true_classes.txt
+-rw-r--r--   0        0        0      616 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/dataset/info.txt
+-rw-r--r--   0        0        0      683 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/templates/config_densCls.json
+-rw-r--r--   0        0        0      994 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/templates/config_dimlpBT.json
+-rw-r--r--   0        0        0      462 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/templates/config_dimlpCls.json
+-rw-r--r--   0        0        0      336 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/templates/config_dimlpPred.json
+-rw-r--r--   0        0        0      553 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/templates/config_dimlpRul.json
+-rw-r--r--   0        0        0      949 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/templates/config_dimlpTrn.json
+-rw-r--r--   0        0        0      834 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/templates/config_fidexGloRules_1.json
+-rw-r--r--   0        0        0      829 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/templates/config_fidexGloRules_2.json
+-rw-r--r--   0        0        0      515 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/templates/config_fidexGloStats.json
+-rw-r--r--   0        0        0      842 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/templates/config_fidexGlo_1.json
+-rw-r--r--   0        0        0      837 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/templates/config_fidexGlo_2.json
+-rw-r--r--   0        0        0      891 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/templates/config_fidex_1.json
+-rw-r--r--   0        0        0      887 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/templates/config_fidex_2.json
+-rw-r--r--   0        0        0      752 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/templates/default_config.json
+-rw-r--r--   0        0        0     2242 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/templates/rules.json
+-rwxr-xr-x   0        0        0    21298 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/tests/templates/tests.sh
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/trainings/__init__.py
+-rw-r--r--   0        0        0     7713 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/trainings/computeRocCurve.py
+-rw-r--r--   0        0        0    28816 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/trainings/convKeras.py
+-rw-r--r--   0        0        0   181426 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/trainings/crossValid.py
+-rw-r--r--   0        0        0    15603 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/trainings/gradBoostTrn.py
+-rw-r--r--   0        0        0    15729 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/trainings/mlpTrn.py
+-rw-r--r--   0        0        0    37185 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/trainings/normalization.py
+-rw-r--r--   0        0        0    26497 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/trainings/parameters.py
+-rw-r--r--   0        0        0    14819 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/trainings/randForestsTrn.py
+-rw-r--r--   0        0        0     4779 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/trainings/stairObj.py
+-rw-r--r--   0        0        0    13603 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/trainings/svmTrn.py
+-rw-r--r--   0        0        0      850 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/trainings/templates/config_gradBoost.json
+-rw-r--r--   0        0        0     1045 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/trainings/templates/config_mlp.json
+-rw-r--r--   0        0        0      376 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/trainings/templates/config_normalization.json
+-rw-r--r--   0        0        0      800 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/trainings/templates/config_randForests.json
+-rw-r--r--   0        0        0      304 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/trainings/templates/config_roc.json
+-rw-r--r--   0        0        0      878 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/trainings/templates/config_svm.json
+-rw-r--r--   0        0        0    25511 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/trainings/trnFun.py
+-rw-r--r--   0        0        0     4735 2022-11-09 12:37:21.000000 dimlpfidex-0.0.1/PKG-INFO
```

### Comparing `dimlpfidex-0.0.0/LICENSE` & `dimlpfidex-0.0.1/json/LICENSES/BSD-3-Clause.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,11 @@
-BSD 3-Clause License
+Copyright (c) <year> <owner>. 
 
-Copyright (c) 2023, HES-XPLAIN
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
+1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
+2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
+3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `dimlpfidex-0.0.0/README.md` & `dimlpfidex-0.0.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,27 @@
-# dimlpfidex
+# dimlpfidex ![build](https://github.com/HES-XPLAIN/dimlpfidex/actions/workflows/build.yml/badge.svg)
 Discretized Interpretable Multi Layer Perceptron (DIMLP) and related algorithms
 
 ## Contribution
 
+### Get the project code
+
+To get the latest source code, install [git](https://git-scm.com/) and [clone](https://docs.github.com/en/get-started/getting-started-with-git/about-remote-repositories) the repository:
+
+```sh
+$ git clone https://github.com/HES-XPLAIN/dimlpfidex.git
+```
+
+To download the required dependencies on your system, run:
+
+```sh
+$ git submodule init
+$ git submodule update
+```
+
 ### Install C++ toolchain
 
 #### Linux, macOS, Windows/WSL
 
 Install with your package manager:
 
 * a C++ compiler (gcc/g++)
@@ -23,81 +38,100 @@
 
 Ensure `cmake.exe` is accessible in the `$PATH` environment variable.
 
 ```shell
 cmake.exe --version
 ```
 
-### Install Python and Poetry
-
-#### Linux, macOS, Windows/WSL
+### Install Python
 
-Use your package manager to install:
+Install [Python](https://www.python.org/):
 
-* python
-* poetry
+#### Manually
 
-#### Windows
+* **Linux, macOS, Windows/WSL**: Use your package manager to install `python3` and `python3-dev`
+* **Windows**: `winget install Python.Python.3.11`
 
-* Install [Python](https://www.python.org/)
+> [!IMPORTANT]
+> On Windows, avoid installing Python through the Microsoft Store as the package has additional permission restrictions.
 
-```shell
-winget install Python.Python.3.10
-```
+#### Using Rye
 
-* Install [poetry](https://python-poetry.org/docs/#installation) and add it to your PATH.
+- Install [Rye](https://rye-up.com/) and [add shims](https://rye-up.com/guide/installation/) to your PATH.
 
-Ensure `python.exe` and `poetry.exe` are accessible in the `$PATH` environment variable.
+Ensure `rye` is accessible in the `$PATH` environment variable.
+Rye will automatically download the suitable Python toolchain as needed.
 
-To check the installation, check these commands return an output:
+To check the installation, check the following commands return an output:
 
 ```shell
-python.exe --version
-poetry.exe --version
+rye --version
 ```
 
-### Compile
+### Install Python dependencies
 
-Activate the virtual environment:
+#### Using pip
 
 ```shell
-poetry shell
+python -m venv .venv
+source .venv/bin/activate
+pip install .
 ```
 
-Install python dependencies and compile:
+> [!NOTE]
+> On Windows, use `.venv\Scripts\activate` instead.
+
+#### Using Rye
+
+Install python dependencies and create a virtualenv in `.venv`:
 
 ```shell
-poetry install
-poetry build
+rye sync
 ```
 
-If CMake complains about not finding pybind11, ensure to activate the shell first.
+#### Add dependencies
+
+To add new dependencies to the project, either add them to the `pyproject.toml` file or use `rye add <dependency>`.
+To add them to the virtualenv, use `pip install .` or `rye sync`.
+
+### Work with virtualenv
+
+To activate the virtualenv, use the standard methods:
+
+* Unix: `source .venv/bin/activate`
+* Windows: `.venv\Scripts\activate`
 
-**Note**: If you still have an issue on Windows, try the following commands to
-build manually:
+To leave the virtualenv, use `deactivate`.
+
+### Compile and Package
+
+Compile and create archives for distribution:
 
 ```shell
-mkdir build && cd build
-$path = (poetry env info | Select-String -Pattern 'Path:\s+(.*)').Matches.Groups[1].Value
-cmake.exe -G "MinGW Makefiles" -DCMAKE_PREFIX_PATH="$path" ..
-cmake.exe --build .
+python -m build
 ```
 
 ### Install Pre-commit hooks
 
 Git hooks are used to ensure quality checks are run by all developers every time
 before a commit.
 
+Install with `pip install pre-commit` or`rye sync`.
+
+To enable pre-commit:
+
 ```shell
-poetry shell
 pre-commit install
 ```
 
 Pre-commit hooks can be run manually with:
 
 ```shell
 pre-commit run --all-files
 ```
 
 ## Release
 
 To publish the package on [PyPI](https://pypi.org/project/dimlpfidex/), refer to [RELEASE](RELEASE.md).
+
+## Credits
+Our test suite is using [Obesity or CVD risk dataset](https://www.kaggle.com/datasets/aravindpcoder/obesity-or-cvd-risk-classifyregressorcluster) from [AravindPCoder](https://www.kaggle.com/aravindpcoder) (under CC BY-SA 4.0 license)
```

### Comparing `dimlpfidex-0.0.0/dimlp/CMakeLists.txt` & `dimlpfidex-0.0.1/dimlp/CMakeLists.txt`

 * *Files 5% similar despite different names*

```diff
@@ -54,24 +54,26 @@
     include_directories(
         ${pybind11_INCLUDE_DIRS}
     )
 endif()
 
 # Build binding lib
 pybind11_add_module(dimlp
+    ${DIMLP_COMMON_SRC}
     ${COMMON_SRC}
     ${DIMLP_TRN_SRC}
     ${DIMLP_PRED_SRC}
     ${DIMLP_CLS_SRC}
     ${DIMLP_BT_SRC}
     ${DENS_CLS_SRC}
     ${DIMLP_RUL_SRC}
     ${CROSS_VALID_SRC}
-    ${FCT_SRC}
     ${PYTHON_FILES}
 )
 
 set_target_properties(
     dimlp PROPERTIES LIBRARY_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/dimlpfidex
 )
 
-target_link_libraries(dimlp PUBLIC)
+target_link_libraries(dimlp PUBLIC common)
+
+install(TARGETS dimlp LIBRARY DESTINATION ./dimlpfidex)
```

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/DensClsFct.cpp` & `dimlpfidex-0.0.1/dimlp/cpp/src/dimlpRulFct.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,631 +1,476 @@
-#include "DensClsFct.h"
-using namespace std;
+#include "dimlpRulFct.h"
 
 const int BPNN = 1;
 
 ////////////////////////////////////////////////////////////
 
-void GiveAllParamDensCls()
+void showDimlpRulParams()
 
 {
-  cout << "\n-------------------------------------------------\n\n";
-
-  cout << "DensCls -L <training set file(path with respect to specified root folder)> ";
-  cout << "-W <Prefix of file of weights> (for instance give DimlpBT) ";
-  cout << "-I <number of input neurons> -O <number of output neurons> ";
-  cout << "-N <number of networks>";
-  cout << " <Options>\n\n";
-
-  cout << "Options are: \n\n";
-  cout << "-S <Folder based on main folder dimlpfidex(default folder) where generated files will be saved. If a file name is specified with another option, his path will be configured with respect to this root folder>\n";
-  cout << "-A <file of attributes>\n";
-  cout << "-T <testing set file>\n";
-  cout << "-1 <file of train classes>\n";
-  cout << "-2 <file of test classes>\n";
-  cout << "-r <file where you redirect console result>\n"; // If we want to redirect console result to file
-  cout << "-p <output train prediction file>\n";           // If we want to specify output train prediction file, not to be densCls.out
-  cout << "-t <output test prediction file>\n";            // If we want to specify output test prediction file, not to be densClsTest.out
-  cout << "-o <output file with global train and test accuracy>\n";
-  cout << "-H1 <number of neurons in the first hidden layer> ";
-  cout << "(if not specified this number will be equal to the ";
-  cout << "number of input neurons)\n";
-  cout << "-Hk <number of neurons in the kth hidden layer>\n";
-  cout << "-R (RULE EXTRACTION)\n";
-  cout << "-F <extraction ruleFile>\n"; // If we want to extract rules in a rulesFile instead of console
-  cout << "-q <number of stairs in staircase activation function>\n";
-
-  cout << "\n-------------------------------------------------\n\n";
+  std::cout << std::endl
+            << "---------------------------------------------------------------------" << std::endl
+            << std::endl;
+  std::cout << "Warning! The files are localised with respect to root folder dimlpfidex." << std::endl;
+  std::cout << "The arguments can be specified in the command or in a json configuration file with --json_config_file your_config_file.json." << std::endl
+            << std::endl;
+
+  std::cout << "----------------------------" << std::endl
+            << std::endl;
+  std::cout << "Required parameters:" << std::endl
+            << std::endl;
+
+  printOptionDescription("--train_data_file <str>", "Train data file");
+  printOptionDescription("--weights_file <str>", "Weights file");
+  printOptionDescription("--nb_attributes <int [1,inf[>", "Number of input neurons");
+  printOptionDescription("--nb_classes <int [2,inf[>", "Number of output neurons");
+  printOptionDescription("--hidden_layers_file <str>", "Hidden layers file name");
+
+  std::cout << std::endl
+            << "----------------------------" << std::endl
+            << std::endl;
+  std::cout << "Optional parameters: " << std::endl
+            << std::endl;
+
+  printOptionDescription("--json_config_file <str>", "JSON file to configure all parameters. If used, this must be the sole argument and must specify the file's relative path");
+  printOptionDescription("--root_folder <str>", "Folder based on main folder dimlpfidex(default folder) containg all used files and where generated files will be saved. If a file name is specified with another option, his path will be configured with respect to this root folder");
+  printOptionDescription("--attributes_file <str>", "File of attributes");
+  printOptionDescription("--valid_data_file <str>", "Validation data file");
+  printOptionDescription("--test_data_file <str>", "Test data file");
+  printOptionDescription("--train_class_file <str>", "Train true class file");
+  printOptionDescription("--test_class_file <str>", "Test true class file");
+  printOptionDescription("--valid_class_file <str>", "Validation true class file");
+  printOptionDescription("--global_rules_outfile <str>", "Rules output file (default: dimlp.rls)");
+  printOptionDescription("--console_file <str>", "File with console logs redirection");
+  printOptionDescription("--stats_file <str>", "Output file name with train, test and validation accuracy");
+  printOptionDescription("--nb_quant_levels <int [3,inf[>", "Number of stairs in staircase activation function (default: 50)");
+  printOptionDescription("--normalization_file <str>", "File containing the mean and std of some attributes. Used to denormalize the rules if specified");
+  printOptionDescription("--mus <list<float ]inf,inf[>>", "Mean or median of each attribute index to denormalize in the rules");
+  printOptionDescription("--sigmas <list<float ]inf,inf[>>", "Standard deviation of each attribute index to denormalize in the rules");
+  printOptionDescription("--normalization_indices <list<int [0,nb_attributes-1]>>", "Attribute indices to denormalize in the rules, only used when no normalization_file is given, index starts at 0 (default: [0,...,nb_attributes-1])");
+
+  std::cout << std::endl
+            << "----------------------------" << std::endl
+            << std::endl;
+  std::cout << "Execution example :" << std::endl
+            << std::endl;
+  std::cout << "dimlp.dimlpRul(\"--train_data_file datanormTrain.txt --train_class_file dataclass2Train.txt --weights_file dimlpDatanorm.wts --test_data_file datanormTest.txt --test_class_file dataclass2Test.txt --nb_attributes 16 --hidden_layers_file hidden_layers.out --nb_classes 2 --global_rules_outfile globalRules.rls --stats_file stats.txt --root_folder dimlp/datafiles\")" << std::endl
+            << std::endl;
+  std::cout << "---------------------------------------------------------------------" << std::endl
+            << std::endl;
 }
 
 ////////////////////////////////////////////////////////////
 
-int densCls(const string &command) {
+/**
+ * @brief Used to set default hyperparameters values and to check the sanity of all used values like boundaries and logic.
+ *
+ * @param p is the Parameter class containing all hyperparameters that rule the entire algorithm execution.
+ */
+void checkDimlpRulParametersLogicValues(Parameters &p) {
+  // setting default values
+  p.setDefaultNbQuantLevels();
+  p.setDefaultString(GLOBAL_RULES_OUTFILE, "dimlp.rls", true);
+
+  // this sections check if values comply with program logic
+
+  // asserting mandatory parameters
+  p.assertIntExists(NB_ATTRIBUTES);
+  p.assertIntExists(NB_CLASSES);
+  p.assertStringExists(TRAIN_DATA_FILE);
+  p.assertStringExists(WEIGHTS_FILE);
+  p.assertStringExists(HIDDEN_LAYERS_FILE);
+
+  // verifying logic between parameters, values range and so on...
+  p.checkParametersCommon();
+  p.checkParametersNormalization();
+}
 
-  // Parsing the command
-  vector<string> commandList;
-  const char delim = ' ';
-  string s;
-  stringstream ss(command);
-  while (std::getline(ss, s, delim)) {
-    commandList.push_back(s);
-  }
-  size_t nbParam = commandList.size();
+int dimlpRul(const std::string &command) {
 
-  DataSet Train;
-  DataSet Test;
-  DataSet TrainClass;
-  DataSet TestClass;
-  DataSet Valid;
-  DataSet ValidClass;
-  DataSet All;
-
-  AttrName Attr;
-
-  int nbDimlpNets = 0;
-
-  int ruleExtr = 0;
-
-  int nbIn = 0;
-  int nbOut = 0;
-  int quant = 50;
-
-  string learnFileTemp;
-  bool learnFileInit = false;
-  string testFileTemp;
-  bool testFileInit = false;
-  string validFileTemp;
-  bool validFileInit = false;
-  string weightFileTemp;
-  bool weightFileInit = false;
-  string weightFileSaveTemp = "dimlp.wts";
-  string predTrainFileTemp = "densCls.out";
-  string predTestFileTemp = "densClsTest.out";
-  string rulesFileTemp;
-  bool rulesFileInit = false;
-  string consoleFileTemp;
-  bool consoleFileInit = false;
-  string accuracyFileTemp;
-  bool accuracyFileInit = false;
-  string learnTarTemp;
-  bool learnTarInit = false;
-  string testTarTemp;
-  bool testTarInit = false;
-  string validTarTemp;
-  bool validTarInit = false;
-  string attrFileTemp;
-  bool attrFileInit = false;
-  string rootFolderTemp;
-  bool rootFolderInit = false;
-
-  int nbLayers;
-  int nbWeightLayers;
-  std::vector<int> vecNbNeurons;
-
-  StringInt arch;
-  StringInt archInd;
-
-  if (nbParam <= 1) {
-    GiveAllParamDensCls();
-    return 0;
-  }
+  // Save buffer where we output results
+  std::ofstream ofs;
+  std::streambuf *cout_buff = std::cout.rdbuf(); // Save old buf
+  try {
 
-  int k = 1; // We skip "DensCls"
-  while (k < nbParam) {
-    if (commandList[k][0] == '-') {
-      k++;
-
-      if (k >= nbParam && commandList[k - 1][1] != 'R') {
-        cout << "Missing something at the end of the command.\n";
-        return -1;
+    float temps;
+    clock_t t1;
+    clock_t t2;
+
+    t1 = clock();
+
+    // Parsing the command
+    std::vector<std::string> commandList = {"dimlpRul"};
+    std::string s;
+    std::stringstream ss(command);
+
+    while (ss >> s) {
+      commandList.push_back(s);
+    }
+
+    size_t nbParam = commandList.size();
+    if (nbParam < 2 || commandList[1] == "-h" || commandList[1] == "--help") {
+      showDimlpRulParams();
+      return 0;
+    }
+
+    // Import parameters
+    std::unique_ptr<Parameters> params;
+    std::vector<ParameterCode> validParams = {TRAIN_DATA_FILE, WEIGHTS_FILE, NB_ATTRIBUTES, NB_CLASSES, ROOT_FOLDER,
+                                              ATTRIBUTES_FILE, VALID_DATA_FILE, TEST_DATA_FILE, TRAIN_CLASS_FILE,
+                                              TEST_CLASS_FILE, VALID_CLASS_FILE, GLOBAL_RULES_OUTFILE, CONSOLE_FILE,
+                                              STATS_FILE, HIDDEN_LAYERS_FILE, NB_QUANT_LEVELS, NORMALIZATION_FILE, MUS, SIGMAS, NORMALIZATION_INDICES};
+    if (commandList[1].compare("--json_config_file") == 0) {
+      if (commandList.size() < 3) {
+        throw CommandArgumentException("JSON config file name/path is missing");
+      } else if (commandList.size() > 3) {
+        throw CommandArgumentException("Option " + commandList[1] + " has to be the only option in the command if specified.");
       }
-
-      char option = commandList[k - 1][1];
-      const char *arg = &(commandList[k])[0];
-      const char *lastArg = &(commandList[k - 1])[0];
-      switch (option) {
-
-      case 'W':
-        weightFileTemp = arg;
-        weightFileInit = true;
-        break;
-
-      case 'q':
-        if (CheckInt(arg))
-          quant = atoi(arg);
-        else
-          return -1;
-
-        break;
-
-      case 'N':
-        if (CheckInt(arg))
-          nbDimlpNets = atoi(arg);
-        else
-          return -1;
-
-        break;
-
-      case 'I':
-        if (CheckInt(arg))
-          nbIn = atoi(arg);
-        else
-          return -1;
-
-        break;
-
-      case 'H':
-        if (CheckInt(arg)) {
-          arch.Insert(atoi(arg));
-
-          const char *ptrParam = lastArg;
-
-          if (ptrParam[2] != '\0') {
-            std::string str(ptrParam + 2);
-            archInd.Insert(std::atoi(str.c_str()));
-          } else {
-            cout << "Which hidden layer (-H) ?\n";
-            return -1;
-          }
-        } else
-          return -1;
-
-        break;
-
-      case 'O':
-        if (CheckInt(arg))
-          nbOut = atoi(arg);
-        else
-          return -1;
-
-        break;
-
-      case 'S':
-        rootFolderTemp = arg;
-        rootFolderInit = true;
-        break;
-
-      case 'A':
-        attrFileTemp = arg;
-        attrFileInit = true;
-        break;
-
-      case 'L':
-        learnFileTemp = arg;
-        learnFileInit = true;
-        break;
-
-      case 'T':
-        testFileTemp = arg;
-        testFileInit = true;
-        break;
-
-      case 'r':
-        consoleFileTemp = arg;
-        consoleFileInit = true;
-        break;
-
-      case 'p':
-        predTrainFileTemp = arg;
-        break;
-
-      case 't':
-        predTestFileTemp = arg;
-        break;
-
-      case 'o':
-        accuracyFileTemp = arg;
-        accuracyFileInit = true;
-        break;
-
-      case '1':
-        learnTarTemp = arg;
-        learnTarInit = true;
-        break;
-
-      case '2':
-        testTarTemp = arg;
-        testTarInit = true;
-        break;
-
-      case 'R':
-        ruleExtr = 1;
-        k--;
-        break;
-
-      case 'F':
-        rulesFileTemp = arg;
-        rulesFileInit = true;
-        break;
-
-      default:
-        cout << "Illegal option: " << lastArg << "\n";
-        return -1;
+      try {
+        params = std::unique_ptr<Parameters>(new Parameters(commandList[2], validParams));
+      } catch (const std::out_of_range &e) {
+        throw CommandArgumentException("Some value inside your JSON config file '" + commandList[2] + "' is out of range.\n(Probably due to a too large or too tiny numeric value).");
+      } catch (const std::exception &e) {
+        std::string msg(e.what()) ;
+        throw CommandArgumentException("Unknown JSON config file error: " + msg);
       }
+    } else {
+      // Read parameters from CLI
+      params = std::unique_ptr<Parameters>(new Parameters(commandList, validParams));
     }
 
-    else {
-      cout << "Illegal option: " << &(commandList[k])[0] << "\n";
-      return -1;
-    }
-    k++;
-  }
-
-  // ----------------------------------------------------------------------
+    // getting all program arguments from CLI
+    checkDimlpRulParametersLogicValues(*params);
 
-  // create paths with root foler
+    // Get console results to file
+    if (params->isStringSet(CONSOLE_FILE)) {
+      ofs.open(params->getString(CONSOLE_FILE));
+      std::cout.rdbuf(ofs.rdbuf()); // redirect cout to file
+    }
 
-  const char *learnFile = nullptr;
-  const char *testFile = nullptr;
-  const char *validFile = nullptr;
-  const char *weightFile = nullptr;
-  const char *predTrainFile = nullptr;
-  const char *predTestFile = nullptr;
-  const char *rulesFile = nullptr;
-  const char *consoleFile = nullptr;
-  const char *accuracyFile = nullptr;
-  const char *learnTar = nullptr;
-  const char *testTar = nullptr;
-  const char *validTar = nullptr;
-  const char *attrFile = nullptr;
-  const char *weightFileSave = nullptr;
-
-  string root = "";
-  if (rootFolderInit) {
-#if defined(__unix__) || defined(__APPLE__)
-    root = rootFolderTemp + "/";
-#elif defined(_WIN32)
-    root = rootFolderTemp + "\\";
-#endif
-  }
-  if (learnFileInit) {
-    learnFileTemp = root + learnFileTemp;
-    learnFile = &learnFileTemp[0];
-  }
+    // Show chosen parameters
+    std::cout << *params;
 
-  if (testFileInit) {
-    testFileTemp = root + testFileTemp;
-    testFile = &testFileTemp[0];
-  }
+    // ----------------------------------------------------------------------
 
-  if (validFileInit) {
-    validFileTemp = root + validFileTemp;
-    validFile = &validFileTemp[0];
-  }
+    // Get parameters values
 
-  if (weightFileInit) {
-    weightFileTemp = root + weightFileTemp;
-    weightFile = &weightFileTemp[0];
-  }
+    int nbIn = params->getInt(NB_ATTRIBUTES);
+    int nbOut = params->getInt(NB_CLASSES);
+    std::string learnFile = params->getString(TRAIN_DATA_FILE);
+    std::string weightFile = params->getString(WEIGHTS_FILE);
+    std::string rulesFile = params->getString(GLOBAL_RULES_OUTFILE);
+    int quant = params->getInt(NB_QUANT_LEVELS);
 
-  predTrainFileTemp = root + predTrainFileTemp;
-  predTrainFile = &predTrainFileTemp[0];
+    int nbLayers;
+    int nbWeightLayers;
+    std::vector<int> vecNbNeurons;
+    StringInt arch;
+    StringInt archInd;
+    params->readHiddenLayersFile(arch, archInd);
 
-  predTestFileTemp = root + predTestFileTemp;
-  predTestFile = &predTestFileTemp[0];
+    DataSet Train;
+    DataSet Test;
+    DataSet TrainClass;
+    DataSet TestClass;
+    DataSet Valid;
+    DataSet ValidClass;
+    DataSet All;
 
-  if (rulesFileInit) {
-    rulesFileTemp = root + rulesFileTemp;
-    rulesFile = &rulesFileTemp[0];
-  }
+    AttrName Attr;
 
-  if (consoleFileInit) {
-    consoleFileTemp = root + consoleFileTemp;
-    consoleFile = &consoleFileTemp[0];
-  }
+    // ----------------------------------------------------------------------
 
-  if (accuracyFileInit) {
-    accuracyFileTemp = root + accuracyFileTemp;
-    accuracyFile = &accuracyFileTemp[0];
-  }
+    if (arch.GetNbEl() == 0) {
+      nbLayers = 3;
+      nbWeightLayers = nbLayers - 1;
 
-  if (learnTarInit) {
-    learnTarTemp = root + learnTarTemp;
-    learnTar = &learnTarTemp[0];
-  }
+      vecNbNeurons.assign(nbLayers, 0);
+      vecNbNeurons[0] = nbIn;
+      vecNbNeurons[1] = nbIn;
+      vecNbNeurons[2] = nbOut;
+    }
 
-  if (testTarInit) {
-    testTarTemp = root + testTarTemp;
-    testTar = &testTarTemp[0];
-  }
+    else {
+      archInd.GoToBeg();
 
-  if (validTarInit) {
-    validTarTemp = root + validTarTemp;
-    validTar = &validTarTemp[0];
-  }
+      if (archInd.GetVal() == 1) {
+        arch.GoToBeg();
 
-  if (attrFileInit) {
-    attrFileTemp = root + attrFileTemp;
-    attrFile = &attrFileTemp[0];
-  }
+        if (arch.GetVal() % nbIn != 0) {
+          throw InternalError("The number of neurons in the first hidden layer must be a multiple of the number of input neurons.");
+        }
 
-  weightFileSaveTemp = root + weightFileSaveTemp;
-  weightFileSave = &weightFileSaveTemp[0];
+        nbLayers = arch.GetNbEl() + 2;
+        nbWeightLayers = nbLayers - 1;
 
-  // ----------------------------------------------------------------------
+        vecNbNeurons.assign(nbLayers, 0);
+        vecNbNeurons[0] = nbIn;
+        vecNbNeurons[nbLayers - 1] = nbOut;
+
+        arch.GoToBeg();
+        for (int p = 1; p <= arch.GetNbEl(); p++, arch.GoToNext()) {
+          vecNbNeurons[p] = arch.GetVal();
 
-  // Get console results to file
-  std::ofstream ofs;
-  std::streambuf *cout_buff = std::cout.rdbuf(); // Save old buf
-  if (consoleFileInit != false) {
-    ofs.open(consoleFile);
-    std::cout.rdbuf(ofs.rdbuf()); // redirect std::cout to file
-  }
+          if (vecNbNeurons[p] == 0) {
+            throw InternalError("The number of neurons must be greater than 0.");
+          }
+        }
+      }
 
-  // ----------------------------------------------------------------------
+      else {
+        nbLayers = arch.GetNbEl() + 3;
+        nbWeightLayers = nbLayers - 1;
+
+        vecNbNeurons.assign(nbLayers, 0);
+        vecNbNeurons[0] = nbIn;
+        vecNbNeurons[1] = nbIn;
+        vecNbNeurons[nbLayers - 1] = nbOut;
+
+        arch.GoToBeg();
+        for (int p = 1; p <= arch.GetNbEl(); p++, arch.GoToNext()) {
+          vecNbNeurons[p + 1] = arch.GetVal();
 
-  if (quant == 0) {
-    cout << "The number of quantized levels must be greater than 0.\n";
-    return -1;
-  }
+          if (vecNbNeurons[p + 1] == 0) {
+            throw InternalError("The number of neurons must be greater than 0.");
+          }
+        }
+      }
+    }
 
-  if (nbIn == 0) {
-    cout << "The number of input neurons must be given with option -I.\n";
-    return -1;
-  }
+    // ----------------------------------------------------------------------
 
-  if (nbOut == 0) {
-    cout << "The number of output neurons must be given with option -O.\n";
-    return -1;
-  }
+    if (params->isStringSet(TRAIN_CLASS_FILE)) {
+      DataSet train(learnFile, nbIn, nbOut);
+      DataSet trainClass(params->getString(TRAIN_CLASS_FILE), nbIn, nbOut);
 
-  if (weightFileInit == false) {
-    cout << "Give a file of weights with -W selection please."
-         << "\n";
-    return -1;
-  }
+      Train = train;
+      TrainClass = trainClass;
+    } else {
+      DataSet data(learnFile, nbIn, nbOut);
 
-  if (nbDimlpNets == 0) {
-    cout << "Give the number of networks with -W selection please."
-         << "\n";
-    return -1;
-  }
+      DataSet train(data.GetNbEx());
+      DataSet trainClass(data.GetNbEx());
 
-  // ----------------------------------------------------------------------
+      data.ExtractDataAndTarget(train, nbIn, trainClass, nbOut);
 
-  if (arch.GetNbEl() == 0) {
-    nbLayers = 3;
-    nbWeightLayers = nbLayers - 1;
-
-    vecNbNeurons.assign(nbLayers, 0);
-    vecNbNeurons[0] = nbIn;
-    vecNbNeurons[1] = nbIn;
-    vecNbNeurons[2] = nbOut;
-  }
+      Train = train;
+      TrainClass = trainClass;
 
-  else {
-    archInd.GoToBeg();
+      data.Del();
+    }
 
-    if (archInd.GetVal() == 1) {
-      arch.GoToBeg();
+    if (params->isStringSet(VALID_DATA_FILE)) {
+      if (params->isStringSet(VALID_CLASS_FILE)) {
+        DataSet valid(params->getString(VALID_DATA_FILE), nbIn, nbOut);
+        DataSet validClass(params->getString(VALID_CLASS_FILE), nbIn, nbOut);
 
-      if (arch.GetVal() % nbIn != 0) {
-        cout << "The number of neurons in the first hidden layer must be";
-        cout << " a multiple of the number of input neurons.\n";
-        return -1;
+        Valid = valid;
+        ValidClass = validClass;
       }
 
-      nbLayers = arch.GetNbEl() + 2;
-      nbWeightLayers = nbLayers - 1;
+      else {
+        DataSet data(params->getString(VALID_DATA_FILE), nbIn, nbOut);
 
-      vecNbNeurons.assign(nbLayers, 0);
-      vecNbNeurons[0] = nbIn;
-      vecNbNeurons[nbLayers - 1] = nbOut;
+        DataSet valid(data.GetNbEx());
+        DataSet validClass(data.GetNbEx());
 
-      for (k = 1, arch.GoToBeg(); k <= arch.GetNbEl(); k++, arch.GoToNext()) {
-        vecNbNeurons[k] = arch.GetVal();
+        data.ExtractDataAndTarget(valid, nbIn, validClass, nbOut);
 
-        if (vecNbNeurons[k] == 0) {
-          cout << "The number of neurons must be greater than 0.\n";
-          return -1;
-        }
-      }
-    }
+        Valid = valid;
+        ValidClass = validClass;
 
-    else {
-      nbLayers = arch.GetNbEl() + 3;
-      nbWeightLayers = nbLayers - 1;
-
-      vecNbNeurons.assign(nbLayers, 0);
-      vecNbNeurons[0] = nbIn;
-      vecNbNeurons[1] = nbIn;
-      vecNbNeurons[nbLayers - 1] = nbOut;
-
-      for (k = 1, arch.GoToBeg(); k <= arch.GetNbEl(); k++, arch.GoToNext()) {
-        vecNbNeurons[k + 1] = arch.GetVal();
-
-        if (vecNbNeurons[k + 1] == 0) {
-          cout << "The number of neurons must be greater than 0.\n";
-          return -1;
-        }
+        data.Del();
       }
     }
-  }
 
-  // ----------------------------------------------------------------------
+    if (params->isStringSet(TEST_DATA_FILE)) {
+      if (params->isStringSet(TEST_CLASS_FILE)) {
+        DataSet test(params->getString(TEST_DATA_FILE), nbIn, nbOut);
+        DataSet testClass(params->getString(TEST_CLASS_FILE), nbIn, nbOut);
 
-  if (learnFileInit == false) {
-    cout << "Give the training file with -L selection please."
-         << "\n";
-    return -1;
-  }
+        Test = test;
+        TestClass = testClass;
+      }
 
-  if (learnTarInit != false) {
-    DataSet train(learnFile, nbIn);
-    DataSet trainClass(learnTar, nbOut);
+      else {
+        DataSet data(params->getString(TEST_DATA_FILE), nbIn, nbOut);
 
-    Train = train;
-    TrainClass = trainClass;
-  } else {
-    DataSet data(learnFile, nbIn + nbOut);
+        DataSet test(data.GetNbEx());
+        DataSet testClass(data.GetNbEx());
 
-    DataSet train(data.GetNbEx());
-    DataSet trainClass(data.GetNbEx());
+        data.ExtractDataAndTarget(test, nbIn, testClass, nbOut);
 
-    data.ExtractDataAndTarget(train, nbIn, trainClass, nbOut);
+        Test = test;
+        TestClass = testClass;
 
-    Train = train;
-    TrainClass = trainClass;
+        data.Del();
+      }
+    }
 
-    data.Del();
-  }
+    // ----------------------------------------------------------------------
 
-  if (validFileInit != false) {
-    if (validTarInit != false) {
-      DataSet valid(validFile, nbIn);
-      DataSet validClass(validTar, nbOut);
+    auto net = std::make_shared<Dimlp>(weightFile, nbLayers, vecNbNeurons, quant);
 
-      Valid = valid;
-      ValidClass = validClass;
-    }
+    float accTrain;
+    float errTrain;
+    float accValid;
+    float errValid;
+    float accTest;
+    float errTest;
 
-    else {
-      DataSet data(validFile, nbIn + nbOut);
+    errTrain = net->Error(Train, TrainClass, &accTrain);
 
-      DataSet valid(data.GetNbEx());
-      DataSet validClass(data.GetNbEx());
+    std::cout << "\n\n*** SUM SQUARED ERROR ON TRAINING SET = " << errTrain;
+    std::cout << "\n\n*** ACCURACY ON TRAINING SET = " << accTrain << "" << std::endl;
 
-      data.ExtractDataAndTarget(valid, nbIn, validClass, nbOut);
-
-      Valid = valid;
-      ValidClass = validClass;
+    if (Valid.GetNbEx() > 0) {
+      errValid = net->Error(Valid, ValidClass, &accValid);
 
-      data.Del();
+      std::cout << "\n\n*** SUM SQUARED ERROR ON VALIDATION SET = " << errValid;
+      std::cout << "\n\n*** ACCURACY ON VALIDATION SET = " << accValid << "" << std::endl;
     }
-  }
 
-  if (testFileInit != false) {
-    if (testTarInit != false) {
-      DataSet test(testFile, nbIn);
-      DataSet testClass(testTar, nbOut);
+    if (Test.GetNbEx() > 0) {
+      errTest = net->Error(Test, TestClass, &accTest);
 
-      Test = test;
-      TestClass = testClass;
+      std::cout << "\n\n*** SUM SQUARED ERROR ON TESTING SET = " << errTest;
+      std::cout << "\n\n*** ACCURACY ON TESTING SET = " << accTest << "" << std::endl;
+    }
+
+    // Output accuracy stats in file
+    if (params->isStringSet(STATS_FILE)) {
+      std::ofstream accFile(params->getString(STATS_FILE));
+      if (accFile.is_open()) {
+        accFile << "Sum squared error on training set = " << errTrain << "" << std::endl;
+        accFile << "Accuracy on training set = " << accTrain << "\n"
+                << std::endl;
+        if (Valid.GetNbEx() > 0) {
+          accFile << "Sum squared error on validation set = " << errValid << "" << std::endl;
+          accFile << "Accuracy on validation set = " << accValid << "\n"
+                  << std::endl;
+        }
+        if (Test.GetNbEx() > 0) {
+          accFile << "Sum squared error on testing set = " << errTest << "" << std::endl;
+          accFile << "Accuracy on testing set = " << accTest << "\n"
+                  << std::endl;
+        }
+        accFile.close();
+      } else {
+        throw CannotOpenFileError("Error : could not open accuracy file " + params->getString(STATS_FILE));
+      }
     }
 
-    else {
-      DataSet data(testFile, nbIn + nbOut);
+    std::cout << "\n-------------------------------------------------\n"
+              << std::endl;
 
-      DataSet test(data.GetNbEx());
-      DataSet testClass(data.GetNbEx());
+    // ----------------------------------------------------------------------
 
-      data.ExtractDataAndTarget(test, nbIn, testClass, nbOut);
+    All = Train;
 
-      Test = test;
-      TestClass = testClass;
+    std::cout << "Extraction Part :: " << std::endl;
 
-      data.Del();
+    if (Valid.GetNbEx() > 0) {
+      DataSet all2(All, Valid);
+      All = all2;
     }
-  }
-
-  auto net = std::make_shared<BagDimlp>(quant, nbLayers, vecNbNeurons, nbDimlpNets, weightFileSave);
-
-  net->DefNetsWithWeights(weightFile);
 
-  float acc;
-  float accTest;
+    std::cout << "\n\n****************************************************\n"
+              << std::endl;
+    std::cout << "*** RULE EXTRACTION" << std::endl;
 
-  net->ComputeAcc(Train, TrainClass, &acc, 1, predTrainFile);
-  cout << "\n\n*** GLOBAL ACCURACY ON TRAINING SET = " << acc << "\n\n";
+    std::vector<std::string> attributeNames;
 
-  if (Test.GetNbEx() != 0) {
-    net->ComputeAcc(Test, TestClass, &accTest, 1, predTestFile);
-    cout << "*** GLOBAL ACCURACY ON TESTING SET = " << accTest << "\n";
-  }
-
-  // Output accuracy stats in file
-  if (accuracyFileInit != false) {
-    ofstream accFile(accuracyFile);
-    if (accFile.is_open()) {
-      accFile << "Global accuracy on training set = " << acc << "\n";
-      if (Test.GetNbEx() != 0) {
-        accFile << "Global accuracy on testing set = " << accTest;
-      }
-      accFile.close();
-    } else {
-      cout << "Error : could not open accuracy file " << accuracyFile << " not found.\n";
-      return -1;
-    }
-  }
-
-  if (ruleExtr) {
-    if (attrFileInit != false) {
-      AttrName attr(attrFile, nbIn, nbOut);
+    if (params->isStringSet(ATTRIBUTES_FILE)) {
+      AttrName attr(params->getString(ATTRIBUTES_FILE), nbIn, nbOut);
 
       if (attr.ReadAttr())
-        cout << "\n\n"
-             << attrFile << ": Read file of attributes.\n\n";
+        std::cout << "\n\n"
+                  << params->getString(ATTRIBUTES_FILE) << ": Read file of attributes.\n"
+                  << std::endl;
 
       Attr = attr;
+      attributeNames = Attr.GetListAttr();
     }
 
-    All = Train;
+    std::vector<int> normalizationIndices;
+    std::vector<double> mus;
+    std::vector<double> sigmas;
 
-    if (Valid.GetNbEx() > 0) {
-      DataSet all2(All, Valid);
-      All = all2;
+    // Get mus, sigmas and normalizationIndices from normalizationFile for denormalization :
+    if (params->isStringSet(NORMALIZATION_FILE)) {
+      auto results = parseNormalizationStats(params->getString(NORMALIZATION_FILE), params->getInt(NB_ATTRIBUTES), attributeNames);
+      normalizationIndices = std::get<0>(results);
+      mus = std::get<2>(results);
+      sigmas = std::get<3>(results);
+      params->setIntVector(NORMALIZATION_INDICES, normalizationIndices);
+      params->setDoubleVector(MUS, mus);
+      params->setDoubleVector(SIGMAS, sigmas);
     }
 
-    cout << "\n\n****************************************************\n\n";
-    cout << "*** RULE EXTRACTION\n";
+    RealHyp ryp(All, net, quant, nbIn,
+                vecNbNeurons[1] / nbIn, nbWeightLayers);
 
-    std::shared_ptr<VirtualHyp> globVirt = net->MakeGlobalVirt(quant, nbIn,
-                                                               vecNbNeurons[1] / nbIn);
+    std::filebuf buf;
 
-    RealHyp ryp(globVirt, nbDimlpNets, net->GetGlobalOut(), nbOut,
-                All, net, quant, nbIn, vecNbNeurons[1] / nbIn,
-                nbWeightLayers);
-
-    if (rulesFileInit != false) {
-      filebuf buf;
-
-      if (buf.open(rulesFile, ios_base::out) == nullptr) {
-        string errorMsg = "Cannot open file for writing";
-        WriteError(errorMsg, rulesFile);
-      }
+    if (buf.open(rulesFile, std::ios_base::out) == nullptr) {
+      throw CannotOpenFileError("Error : Cannot open rules file " + rulesFile);
+    }
 
-      ostream rulesFileost(&buf);
+    std::ostream rulesFileost(&buf);
+
+    if (params->isDoubleVectorSet(MUS)) {
+      ryp.RuleExtraction(All, Train, TrainClass, Valid, ValidClass,
+                         Test, TestClass, Attr, rulesFileost, mus, sigmas, normalizationIndices);
+    } else {
       ryp.RuleExtraction(All, Train, TrainClass, Valid, ValidClass,
                          Test, TestClass, Attr, rulesFileost);
+    }
 
-      if (ryp.TreeAborted()) {
-
-        std::shared_ptr<VirtualHyp> globVirt2 = net->MakeGlobalVirt(quant, nbIn,
-                                                                    vecNbNeurons[1] / nbIn);
-
-        RealHyp2 ryp2(globVirt2, nbDimlpNets, net->GetGlobalOut(), nbOut,
-                      All, net, quant, nbIn, vecNbNeurons[1] / nbIn,
-                      nbWeightLayers);
+    if (ryp.TreeAborted()) {
+      RealHyp2 ryp2(All, net, quant, nbIn,
+                    vecNbNeurons[1] / nbIn, nbWeightLayers);
 
+      if (params->isDoubleVectorSet(MUS)) {
+        ryp2.RuleExtraction(All, Train, TrainClass, Valid, ValidClass,
+                            Test, TestClass, Attr, rulesFileost, mus, sigmas, normalizationIndices);
+      } else {
         ryp2.RuleExtraction(All, Train, TrainClass, Valid, ValidClass,
                             Test, TestClass, Attr, rulesFileost);
       }
+    }
 
-      cout << "\n\n"
-           << rulesFile << ": "
-           << "Written.\n\n";
-    } else {
-      ryp.RuleExtraction(All, Train, TrainClass, Valid, ValidClass,
-                         Test, TestClass, Attr, cout);
+    std::cout << "\n\n"
+              << rulesFile << ": "
+              << "Written.\n"
+              << std::endl;
 
-      if (ryp.TreeAborted()) {
+    t2 = clock();
+    temps = (float)(t2 - t1) / CLOCKS_PER_SEC;
+    std::cout << "\nFull execution time = " << temps << " sec" << std::endl;
 
-        std::shared_ptr<VirtualHyp> globVirt3 = net->MakeGlobalVirt(quant, nbIn,
-                                                                    vecNbNeurons[1] / nbIn);
+    std::cout.rdbuf(cout_buff); // reset to standard output again
 
-        RealHyp2 ryp2(globVirt3, nbDimlpNets, net->GetGlobalOut(), nbOut,
-                      All, net, quant, nbIn, vecNbNeurons[1] / nbIn,
-                      nbWeightLayers);
+    BpNN::resetInitRandomGen();
 
-        ryp2.RuleExtraction(All, Train, TrainClass, Valid, ValidClass,
-                            Test, TestClass, Attr, cout);
-      }
-    }
-  }
+    Train.Del();
+    TrainClass.Del();
 
-  std::cout.rdbuf(cout_buff); // reset to standard output again
+    if (Test.GetNbEx() > 0) {
+      Test.Del();
+      TestClass.Del();
+    }
 
-  BpNN::resetInitRandomGen();
+    if (Valid.GetNbEx() > 0) {
+      Valid.Del();
+      ValidClass.Del();
+    }
 
+  } catch (const ErrorHandler &e) {
+    std::cout.rdbuf(cout_buff); // reset to standard output again
+    std::cerr << e.what() << std::endl;
+    return -1;
+  }
   return 0;
 }
-// Exemple to launch the code : densCls("DensCls -L datanormTrain -1 dataclass2Train -T datanormTest -2 dataclass2Test -I 16 -H2 5 -O 2 -N 2 -W dimlpDatanormBT -R -F dimlpDatanormDensClsRul.rls -p dimlpDatanormDensClsTrain.out -t dimlpDatanormDensClsTest.out -o dimlpDatanormDensClsStats -r dimlpDatanormDensClsResult.txt -S dimlp/datafiles");
+
+// Exemple to launch the code : dimlp.dimlpRul("dimlpRul --train_data_file datanormTrain --train_class_file dataclass2Train --weights_file dimlpDatanorm.wts --test_data_file datanormTest --test_class_file dataclass2Test --nb_attributes 16 --hidden_layers_file hidden_layers.out --nb_classes 2 --global_rules_outfile dimlpDatanormRul.rls --stats_file dimlpDatanormRulStats --console_file dimlpDatanormRulResult.txt --root_folder dimlp/datafiles")
```

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/DimlpBTFct.cpp` & `dimlpfidex-0.0.1/dimlp/cpp/src/densClsFct.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,768 +1,460 @@
-#include "DimlpBTFct.h"
+#include "densClsFct.h"
+
 const int BPNN = 1;
 
-using namespace std;
 ////////////////////////////////////////////////////////////
 
-void GiveAllParamDimlpBT()
+void showDensClsParams()
 
 {
-  cout << "\n-------------------------------------------------\n\n";
-
-  cout << "DimlpBT -L <training set file(path with respect to specified root folder)> ";
-  cout << "-I <number of input neurons> -O <number of output neurons>";
-
-  cout << " <Options>\n\n";
-
-  cout << "Options are: \n\n";
-  cout << "-S <Folder based on main folder dimlpfidex(default folder) where generated files will be saved. If a file name is specified with another option, his path will be configured with respect to this root folder>\n";
-  cout << "-N <number of networks>\n";
-  cout << "-A <file of attributes>\n";
-  cout << "-T <testing set file>\n";
-  cout << "-1 <file of train classes>\n";
-  cout << "-2 <file of test classes>\n";
-  cout << "-r <file where you redirect console result>\n";         // If we want to redirect console result to file
-  cout << "-w <output weights generic name file(without .wts)>\n"; // If we want to specify weights output generic file name, not to be dimlpBTx.wts
-  cout << "-p <output train prediction file>\n";                   // If we want to specify output train prediction file, not to be dimlpBT.out
-  cout << "-t <output test prediction file>\n";                    // If we want to specify output test prediction file, not to be dimlpBTTest.out
-  cout << "-o <output file with train, test and validation accuracy and with the global accuracy for train and test>\n";
-  cout << "-H1 <number of neurons in the first hidden layer> ";
-  cout << "(if not specified this number will be equal to the ";
-  cout << "number of input neurons)\n";
-  cout << "-Hk <number of neurons in the kth hidden layer>\n";
-  cout << "-R (RULE EXTRACTION)\n";
-  cout << "-F <extraction ruleFile>\n"; // If we want to extract rules in a rulesFile instead of console
-  cout << "-l <back-propagation learning parameter (Eta)>\n";
-  cout << "-m <back-propagation momentum parameter (Mu)>\n";
-  cout << "-f <back-propagation flat spot elimination parameter (Flat)>\n";
-  cout << "-q <number of stairs in staircase activation function>\n";
-  cout << "-e <error threshold>\n";
-  cout << "-a <accuracy threshold>\n";
-  cout << "-d <absolute difference error threshold>\n";
-  cout << "-i <number of epochs>\n";
-  cout << "-s <number of epochs to show error>\n";
-  cout << "-n <number of examples for one single network>\n";
-  cout << "-z <seed (0=ranodom)>";
-
-  cout << "\n-------------------------------------------------\n\n";
+  std::cout << std::endl
+            << "---------------------------------------------------------------------" << std::endl
+            << std::endl;
+  std::cout << "Warning! The files are localised with respect to root folder dimlpfidex." << std::endl;
+  std::cout << "The arguments can be specified in the command or in a json configuration file with --json_config_file your_config_file.json." << std::endl
+            << std::endl;
+
+  std::cout << "----------------------------" << std::endl
+            << std::endl;
+  std::cout << "Required parameters:" << std::endl
+            << std::endl;
+
+  printOptionDescription("--train_data_file <str>", "Train data file");
+  printOptionDescription("--weights_file <str>", "Weights file containing the weights of each network");
+  printOptionDescription("--nb_attributes <int [1,inf[>", "Number of input neurons");
+  printOptionDescription("--nb_classes <int [2,inf[>", "Number of output neurons");
+  printOptionDescription("--hidden_layers_file <str>", "Hidden layers file name");
+
+  std::cout << std::endl
+            << "----------------------------" << std::endl
+            << std::endl;
+  std::cout << "Optional parameters: " << std::endl
+            << std::endl;
+
+  printOptionDescription("--json_config_file <str>", "JSON file to configure all parameters. If used, this must be the sole argument and must specify the file's relative path");
+  printOptionDescription("--root_folder <str>", "Folder based on main folder dimlpfidex(default folder) containg all used files and where generated files will be saved. If a file name is specified with another option, his path will be configured with respect to this root folder");
+  printOptionDescription("--attributes_file <str>", "File of attributes");
+  printOptionDescription("--test_data_file <str>", "Test data file");
+  printOptionDescription("--train_class_file <str>", "Train true class file");
+  printOptionDescription("--test_class_file <str>", "Test true class file");
+  printOptionDescription("--console_file <str>", "File with console logs redirection");
+  printOptionDescription("--train_pred_outfile <str>", "Output train prediction file name (default: densClsTrain.out)");
+  printOptionDescription("--test_pred_outfile <str>", "Output test prediction file name (default: densClsTest.out)");
+  printOptionDescription("--stats_file <str>", "Output file name with global train and test accuracy");
+  printOptionDescription("--with_rule_extraction <bool>", "Whether to extract rules with dimlpBT algorithm");
+  printOptionDescription("--global_rules_outfile <str>", "Rules output file");
+  printOptionDescription("--nb_quant_levels <int [3,inf[>", "Number of stairs in staircase activation function (default: 50)");
+  printOptionDescription("--normalization_file <str>", "File containing the mean and std of some attributes. Used to denormalize the rules if specified");
+  printOptionDescription("--mus <list<float ]inf,inf[>>", "Mean or median of each attribute index to denormalize in the rules");
+  printOptionDescription("--sigmas <list<float ]inf,inf[>>", "Standard deviation of each attribute index to denormalize in the rules");
+  printOptionDescription("--normalization_indices <list<int [0,nb_attributes-1]>>", "Attribute indices to denormalize in the rules, only used when no normalization_file is given, index starts at 0 (default: [0,...,nb_attributes-1])");
+
+  std::cout << std::endl
+            << "----------------------------" << std::endl
+            << std::endl;
+  std::cout << "Execution example :" << std::endl
+            << std::endl;
+  std::cout << "dimlp.densCls(\"--train_data_file datanormTrain.txt --train_class_file dataclass2Train.txt --test_data_file datanormTest.txt --test_class_file dataclass2Test.txt --nb_attributes 16 --hidden_layers_file hidden_layers.out --nb_classes 2 --weights_file dimlpDatanormBT.wts --with_rule_extraction true --global_rules_outfile globalRules.rls --train_pred_outfile predTrain.out --test_pred_outfile testPred.out --stats_file stats.txt --root_folder dimlp/datafiles\")" << std::endl
+            << std::endl;
+  std::cout << "---------------------------------------------------------------------" << std::endl
+            << std::endl;
 }
 
 ////////////////////////////////////////////////////////////
 
-int dimlpBT(const string &command) {
-  float temps;
-  clock_t t1;
-  clock_t t2;
-
-  t1 = clock();
-
-  // Parsing the command
-  vector<string> commandList;
-  const char delim = ' ';
-  string s;
-  stringstream ss(command);
-  while (std::getline(ss, s, delim)) {
-    commandList.push_back(s);
-  }
-  size_t nbParam = commandList.size();
+/**
+ * @brief Used to set default hyperparameters values and to check the sanity of all used values like boundaries and logic.
+ *
+ * @param p is the Parameter class containing all hyperparameters that rule the entire algorithm execution.
+ */
+void checkDensClsParametersLogicValues(Parameters &p) {
+  // setting default values
+  p.setDefaultNbQuantLevels();
+  p.setDefaultBool(WITH_RULE_EXTRACTION, false);
+  p.setDefaultString(TRAIN_PRED_OUTFILE, "densClsTrain.out", true);
+  p.setDefaultString(TEST_PRED_OUTFILE, "densClsTest.out", true);
+
+  // this sections check if values comply with program logic
+
+  // asserting mandatory parameters
+  p.assertIntExists(NB_ATTRIBUTES);
+  p.assertIntExists(NB_CLASSES);
+  p.assertStringExists(TRAIN_DATA_FILE);
+  p.assertStringExists(WEIGHTS_FILE);
+  p.assertStringExists(HIDDEN_LAYERS_FILE);
+
+  // verifying logic between parameters, values range and so on...
+  p.checkParametersCommon();
+  p.checkParametersNormalization();
+}
 
-  DataSet Train;
-  DataSet Test;
-  DataSet TrainClass;
-  DataSet TestClass;
-  DataSet Valid;
-  DataSet ValidClass;
-  DataSet All;
-
-  AttrName Attr;
-
-  float eta = 0.1f;
-  float mu = 0.6f;
-  float flat = 0.01f;
-  float errThres = -1111111111.0f;
-  float accThres = 11111111111111.0f;
-  float deltaErr = 0;
-  int showErr = 10;
-  int epochs = 1500;
-  int quant = 50;
-  int nbDimlpNets = 25;
-
-  int ruleExtr = 0;
-
-  int nbIn = 0;
-  int nbOut = 0;
-  int nbExInOne = 0;
-  int seed = 0;
-
-  string learnFileTemp;
-  bool learnFileInit = false;
-  string testFileTemp;
-  bool testFileInit = false;
-  string validFileTemp;
-  bool validFileInit = false;
-  string weightFileTemp = "dimlp.wts";
-  string genericWeightsFileTemp = "dimlpBT";
-  string predTrainFileTemp = "dimlpBT.out";
-  string predTestFileTemp = "dimlpBTTest.out";
-  string rulesFileTemp;
-  bool rulesFileInit = false;
-  string consoleFileTemp;
-  bool consoleFileInit = false;
-  string accuracyFileTemp;
-  bool accuracyFileInit = false;
-  string learnTarTemp;
-  bool learnTarInit = false;
-  string testTarTemp;
-  bool testTarInit = false;
-  string validTarTemp;
-  bool validTarInit = false;
-  string attrFileTemp;
-  bool attrFileInit = false;
-  string rootFolderTemp;
-  bool rootFolderInit = false;
-
-  int flagEp = 0;
-
-  int nbLayers;
-  int nbWeightLayers;
-  std::vector<int> vecNbNeurons;
-
-  StringInt arch;
-  StringInt archInd;
-
-  if (nbParam <= 1) {
-    GiveAllParamDimlpBT();
-    return 0;
-  }
+int densCls(const std::string &command) {
 
-  int k = 1; // We skip "DimlpBT"
-  while (k < nbParam) {
-    if (commandList[k][0] == '-') {
-      k++;
-
-      if (k >= nbParam && commandList[k - 1][1] != 'R') {
-        cout << "Missing something at the end of the command.\n";
-        return -1;
-      }
+  // Save buffer where we output results
+  std::ofstream ofs;
+  std::streambuf *cout_buff = std::cout.rdbuf(); // Save old buf
+  try {
 
-      char option = commandList[k - 1][1];
-      const char *arg = &(commandList[k])[0];
-      const char *lastArg = &(commandList[k - 1])[0];
-      switch (option) {
-      case 'l':
-        if (CheckFloat(arg))
-          eta = static_cast<float>(atof(arg));
-        else
-          return -1;
-
-        break;
-
-      case 'm':
-        if (CheckFloat(arg))
-          mu = static_cast<float>(atof(arg));
-        else
-          return -1;
-
-        break;
-
-      case 'f':
-        if (CheckFloat(arg))
-          flat = static_cast<float>(atof(arg));
-        else
-          return -1;
-
-        break;
-
-      case 'e':
-        if (CheckFloat(arg))
-          errThres = static_cast<float>(atof(arg));
-        else
-          return -1;
-
-        if (flagEp == 0)
-          epochs = 2000000000;
-        break;
-
-      case 'a':
-        if (CheckFloat(arg))
-          accThres = static_cast<float>(atof(arg));
-        else
-          return -1;
-
-        if (flagEp == 0)
-          epochs = 2000000000;
-        break;
-
-      case 'd':
-        if (CheckFloat(arg))
-          deltaErr = static_cast<float>(atof(arg));
-        else
-          return -1;
-
-        if (flagEp == 0)
-          epochs = 2000000000;
-        break;
-
-      case 's':
-        if (CheckInt(arg))
-          showErr = atoi(arg);
-        else
-          return -1;
-
-        break;
-
-      case 'i':
-        if (CheckInt(arg)) {
-          epochs = atoi(arg);
-          flagEp = 1;
-        } else
-          return -1;
-
-        break;
-
-      case 'q':
-        if (CheckInt(arg))
-          quant = atoi(arg);
-        else
-          return -1;
-
-        break;
-
-      case 'n':
-        if (CheckInt(arg))
-          nbExInOne = atoi(arg);
-        else
-          return -1;
-
-        break;
-
-      case 'N':
-        if (CheckInt(arg))
-          nbDimlpNets = atoi(arg);
-        else
-          return -1;
-
-        break;
-
-      case 'I':
-        if (CheckInt(arg))
-          nbIn = atoi(arg);
-        else
-          return -1;
-
-        break;
-
-      case 'H':
-        if (CheckInt(arg)) {
-          arch.Insert(atoi(arg));
-
-          const char *ptrParam = lastArg;
-
-          if (ptrParam[2] != '\0') {
-            std::string str(ptrParam + 2);
-            archInd.Insert(std::atoi(str.c_str()));
-          } else {
-            cout << "Which hidden layer (-H) ?\n";
-            return -1;
-          }
-        } else
-          return -1;
+    float temps;
+    clock_t t1;
+    clock_t t2;
 
-        break;
+    t1 = clock();
 
-      case 'O':
-        if (CheckInt(arg))
-          nbOut = atoi(arg);
-        else
-          return -1;
-
-        break;
-
-      case 'z':
-        if (CheckInt(arg))
-          seed = atoi(arg);
-        else
-          return -1;
-
-        break;
-
-      case 'S':
-        rootFolderTemp = arg;
-        rootFolderInit = true;
-        break;
-
-      case 'A':
-        attrFileTemp = arg;
-        attrFileInit = true;
-        break;
-
-      case 'L':
-        learnFileTemp = arg;
-        learnFileInit = true;
-        break;
-
-      case 'T':
-        testFileTemp = arg;
-        testFileInit = true;
-        break;
-
-      case 'r':
-        consoleFileTemp = arg;
-        consoleFileInit = true;
-        break;
-
-      case 'w':
-        genericWeightsFileTemp = arg;
-        break;
-
-      case 'p':
-        predTrainFileTemp = arg;
-        break;
-
-      case 't':
-        predTestFileTemp = arg;
-        break;
-
-      case 'o':
-        accuracyFileTemp = arg;
-        accuracyFileInit = true;
-        break;
-
-      case '1':
-        learnTarTemp = arg;
-        learnTarInit = true;
-        break;
-
-      case '2':
-        testTarTemp = arg;
-        testTarInit = true;
-        break;
-
-      case 'R':
-        ruleExtr = 1;
-        k--;
-        break;
-
-      case 'F':
-        rulesFileTemp = arg;
-        rulesFileInit = true;
-        break;
-
-      default:
-        cout << "Illegal option: " << lastArg << "\n";
-        return -1;
-      }
-    }
+    // Parsing the command
+    std::vector<std::string> commandList = {"densCls"};
+    std::string s;
+    std::stringstream ss(command);
 
-    else {
-      cout << "Illegal option: " << &(commandList[k])[0] << "\n";
-      return -1;
+    while (ss >> s) {
+      commandList.push_back(s);
     }
-    k++;
-  }
-
-  // ----------------------------------------------------------------------
-
-  // create paths with root foler
-
-  const char *learnFile = nullptr;
-  const char *testFile = nullptr;
-  const char *validFile = nullptr;
-  const char *weightFile = nullptr;
-  const char *genericWeightsFile = nullptr;
-  const char *predTrainFile = nullptr;
-  const char *predTestFile = nullptr;
-  const char *rulesFile = nullptr;
-  const char *consoleFile = nullptr;
-  const char *accuracyFile = nullptr;
-  const char *learnTar = nullptr;
-  const char *testTar = nullptr;
-  const char *validTar = nullptr;
-  const char *attrFile = nullptr;
-
-  string root = "";
-  if (rootFolderInit) {
-#if defined(__unix__) || defined(__APPLE__)
-    root = rootFolderTemp + "/";
-#elif defined(_WIN32)
-    root = rootFolderTemp + "\\";
-#endif
-  }
-
-  if (learnFileInit) {
-    learnFileTemp = root + learnFileTemp;
-    learnFile = &learnFileTemp[0];
-  }
-
-  if (testFileInit) {
-    testFileTemp = root + testFileTemp;
-    testFile = &testFileTemp[0];
-  }
-
-  if (validFileInit) {
-    validFileTemp = root + validFileTemp;
-    validFile = &validFileTemp[0];
-  }
-
-  weightFileTemp = root + weightFileTemp;
-  weightFile = &weightFileTemp[0];
-
-  genericWeightsFileTemp = root + genericWeightsFileTemp;
-  genericWeightsFile = &genericWeightsFileTemp[0];
-
-  predTrainFileTemp = root + predTrainFileTemp;
-  predTrainFile = &predTrainFileTemp[0];
-
-  predTestFileTemp = root + predTestFileTemp;
-  predTestFile = &predTestFileTemp[0];
-
-  if (rulesFileInit) {
-    rulesFileTemp = root + rulesFileTemp;
-    rulesFile = &rulesFileTemp[0];
-  }
-
-  if (consoleFileInit) {
-    consoleFileTemp = root + consoleFileTemp;
-    consoleFile = &consoleFileTemp[0];
-  }
-
-  if (accuracyFileInit) {
-    accuracyFileTemp = root + accuracyFileTemp;
-    accuracyFile = &accuracyFileTemp[0];
-  }
-
-  if (learnTarInit) {
-    learnTarTemp = root + learnTarTemp;
-    learnTar = &learnTarTemp[0];
-  }
-
-  if (testTarInit) {
-    testTarTemp = root + testTarTemp;
-    testTar = &testTarTemp[0];
-  }
-
-  if (validTarInit) {
-    validTarTemp = root + validTarTemp;
-    validTar = &validTarTemp[0];
-  }
 
-  if (attrFileInit) {
-    attrFileTemp = root + attrFileTemp;
-    attrFile = &attrFileTemp[0];
-  }
-
-  // ----------------------------------------------------------------------
-
-  // Get console results to file
-  std::ofstream ofs;
-  std::streambuf *cout_buff = std::cout.rdbuf(); // Save old buf
-  if (consoleFileInit != false) {
-    ofs.open(consoleFile);
-    std::cout.rdbuf(ofs.rdbuf()); // redirect std::cout to file
-  }
+    size_t nbParam = commandList.size();
+    if (nbParam < 2 || commandList[1] == "-h" || commandList[1] == "--help") {
+      showDensClsParams();
+      return 0;
+    }
 
-  // ----------------------------------------------------------------------
+    // Import parameters
+    std::unique_ptr<Parameters> params;
 
-  if (eta <= 0) {
-    cout << "The learning parameter must be greater than 0.\n";
-    return -1;
-  }
+    std::vector<ParameterCode> validParams = {TRAIN_DATA_FILE, WEIGHTS_FILE, NB_ATTRIBUTES, NB_CLASSES,
+                                              ROOT_FOLDER, ATTRIBUTES_FILE, TEST_DATA_FILE, TRAIN_CLASS_FILE, TEST_CLASS_FILE,
+                                              CONSOLE_FILE, TRAIN_PRED_OUTFILE, TEST_PRED_OUTFILE, STATS_FILE, HIDDEN_LAYERS_FILE, WITH_RULE_EXTRACTION,
+                                              GLOBAL_RULES_OUTFILE, NB_QUANT_LEVELS, NORMALIZATION_FILE, MUS, SIGMAS, NORMALIZATION_INDICES};
+    if (commandList[1].compare("--json_config_file") == 0) {
+      if (commandList.size() < 3) {
+        throw CommandArgumentException("JSON config file name/path is missing");
+      } else if (commandList.size() > 3) {
+        throw CommandArgumentException("Option " + commandList[1] + " has to be the only option in the command if specified.");
+      }
+      try {
+        params = std::unique_ptr<Parameters>(new Parameters(commandList[2], validParams));
+      } catch (const std::out_of_range &e) {
+        throw CommandArgumentException("Some value inside your JSON config file '" + commandList[2] + "' is out of range.\n(Probably due to a too large or too tiny numeric value).");
+      } catch (const std::exception &e) {
+        std::string msg(e.what()) ;
+        throw CommandArgumentException("Unknown JSON config file error: " + msg);
+      }
+    } else {
+      // Read parameters from CLI
+      params = std::unique_ptr<Parameters>(new Parameters(commandList, validParams));
+    }
 
-  if (mu < 0) {
-    cout << "The momentum parameter must be greater or equal to 0.\n";
-    return -1;
-  }
+    // getting all program arguments from CLI
+    checkDensClsParametersLogicValues(*params);
 
-  if (showErr == 0) {
-    cout << "The number of epochs must be greater than 0.\n";
-    return -1;
-  }
+    // Get console results to file
+    if (params->isStringSet(CONSOLE_FILE)) {
+      ofs.open(params->getString(CONSOLE_FILE));
+      std::cout.rdbuf(ofs.rdbuf()); // redirect cout to file
+    }
 
-  if (quant == 0) {
-    cout << "The number of quantized levels must be greater than 0.\n";
-    return -1;
-  }
+    // Show chosen parameters
+    std::cout << *params;
 
-  if (nbIn == 0) {
-    cout << "The number of input neurons must be given with option -I.\n";
-    return -1;
-  }
+    // ----------------------------------------------------------------------
 
-  if (nbOut == 0) {
-    cout << "The number of output neurons must be given with option -O.\n";
-    return -1;
-  }
+    // Get parameters values
+    std::string weightFileSave = "dimlp.wts";
 
-  // ----------------------------------------------------------------------
+    int nbIn = params->getInt(NB_ATTRIBUTES);
+    int nbOut = params->getInt(NB_CLASSES);
+    std::string learnFile = params->getString(TRAIN_DATA_FILE);
+    std::string predTrainFile = params->getString(TRAIN_PRED_OUTFILE);
+    std::string predTestFile = params->getString(TEST_PRED_OUTFILE);
+    std::string weightFile = params->getString(WEIGHTS_FILE);
+    int nbDimlpNets = countNetworksInFile(weightFile);
+    int quant = params->getInt(NB_QUANT_LEVELS);
 
-  if (arch.GetNbEl() == 0) {
-    nbLayers = 3;
-    nbWeightLayers = nbLayers - 1;
-
-    vecNbNeurons.assign(nbLayers, 0);
-    vecNbNeurons[0] = nbIn;
-    vecNbNeurons[1] = nbIn;
-    vecNbNeurons[2] = nbOut;
-  }
+    int nbLayers;
+    int nbWeightLayers;
+    std::vector<int> vecNbNeurons;
+    StringInt arch;
+    StringInt archInd;
+    params->readHiddenLayersFile(arch, archInd);
 
-  else {
-    archInd.GoToBeg();
+    DataSet Train;
+    DataSet Test;
+    DataSet TrainClass;
+    DataSet TestClass;
+    DataSet Valid;
+    DataSet ValidClass;
+    DataSet All;
 
-    if (archInd.GetVal() == 1) {
-      arch.GoToBeg();
+    AttrName Attr;
 
-      if (arch.GetVal() % nbIn != 0) {
-        cout << "The number of neurons in the first hidden layer must be";
-        cout << " a multiple of the number of input neurons.\n";
-        return -1;
-      }
+    // ----------------------------------------------------------------------
 
-      nbLayers = arch.GetNbEl() + 2;
+    if (arch.GetNbEl() == 0) {
+      nbLayers = 3;
       nbWeightLayers = nbLayers - 1;
 
       vecNbNeurons.assign(nbLayers, 0);
       vecNbNeurons[0] = nbIn;
-      vecNbNeurons[nbLayers - 1] = nbOut;
+      vecNbNeurons[1] = nbIn;
+      vecNbNeurons[2] = nbOut;
+    }
+
+    else {
+      archInd.GoToBeg();
 
-      for (k = 1, arch.GoToBeg(); k <= arch.GetNbEl(); k++, arch.GoToNext()) {
-        vecNbNeurons[k] = arch.GetVal();
+      if (archInd.GetVal() == 1) {
+        arch.GoToBeg();
 
-        if (vecNbNeurons[k] == 0) {
-          cout << "The number of neurons must be greater than 0.\n";
-          return -1;
+        if (arch.GetVal() % nbIn != 0) {
+          throw InternalError("The number of neurons in the first hidden layer must be a multiple of the number of input neurons.");
         }
-      }
-    }
 
-    else {
-      nbLayers = arch.GetNbEl() + 3;
-      nbWeightLayers = nbLayers - 1;
+        nbLayers = arch.GetNbEl() + 2;
+        nbWeightLayers = nbLayers - 1;
 
-      vecNbNeurons.assign(nbLayers, 0);
-      vecNbNeurons[0] = nbIn;
-      vecNbNeurons[1] = nbIn;
-      vecNbNeurons[nbLayers - 1] = nbOut;
+        vecNbNeurons.assign(nbLayers, 0);
+        vecNbNeurons[0] = nbIn;
+        vecNbNeurons[nbLayers - 1] = nbOut;
+
+        arch.GoToBeg();
+        for (int p = 1; p <= arch.GetNbEl(); p++, arch.GoToNext()) {
+          vecNbNeurons[p] = arch.GetVal();
+
+          if (vecNbNeurons[p] == 0) {
+            throw InternalError("The number of neurons must be greater than 0.");
+          }
+        }
+      }
 
-      for (k = 1, arch.GoToBeg(); k <= arch.GetNbEl(); k++, arch.GoToNext()) {
-        vecNbNeurons[k + 1] = arch.GetVal();
+      else {
+        nbLayers = arch.GetNbEl() + 3;
+        nbWeightLayers = nbLayers - 1;
+
+        vecNbNeurons.assign(nbLayers, 0);
+        vecNbNeurons[0] = nbIn;
+        vecNbNeurons[1] = nbIn;
+        vecNbNeurons[nbLayers - 1] = nbOut;
+
+        arch.GoToBeg();
+        for (int p = 1; p <= arch.GetNbEl(); p++, arch.GoToNext()) {
+          vecNbNeurons[p + 1] = arch.GetVal();
 
-        if (vecNbNeurons[k + 1] == 0) {
-          cout << "The number of neurons must be greater than 0.\n";
-          return -1;
+          if (vecNbNeurons[p + 1] == 0) {
+            throw InternalError("The number of neurons must be greater than 0.");
+          }
         }
       }
     }
-  }
 
-  // ----------------------------------------------------------------------
-  if (learnFileInit == false) {
-    cout << "Give the training file with -L selection please."
-         << "\n";
-    return -1;
-  }
-  if (learnTarInit != false) {
-    DataSet train(learnFile, nbIn);
-    DataSet trainClass(learnTar, nbOut);
+    // ----------------------------------------------------------------------
 
-    Train = train;
-    TrainClass = trainClass;
-  } else {
-    DataSet data(learnFile, nbIn + nbOut);
+    if (params->isStringSet(TRAIN_CLASS_FILE) != false) {
+      DataSet train(learnFile, nbIn, nbOut);
+      DataSet trainClass(params->getString(TRAIN_CLASS_FILE), nbIn, nbOut);
 
-    DataSet train(data.GetNbEx());
-    DataSet trainClass(data.GetNbEx());
+      Train = train;
+      TrainClass = trainClass;
+    } else {
+      DataSet data(learnFile, nbIn, nbOut);
 
-    data.ExtractDataAndTarget(train, nbIn, trainClass, nbOut);
+      DataSet train(data.GetNbEx());
+      DataSet trainClass(data.GetNbEx());
 
-    Train = train;
-    TrainClass = trainClass;
+      data.ExtractDataAndTarget(train, nbIn, trainClass, nbOut);
 
-    data.Del();
-  }
+      Train = train;
+      TrainClass = trainClass;
 
-  if (validFileInit != false) {
-    if (validTarInit != false) {
-      DataSet valid(validFile, nbIn);
-      DataSet validClass(validTar, nbOut);
-
-      Valid = valid;
-      ValidClass = validClass;
+      data.Del();
     }
 
-    else {
-      DataSet data(validFile, nbIn + nbOut);
+    if (params->isStringSet(TEST_DATA_FILE)) {
+      if (params->isStringSet(TEST_CLASS_FILE)) {
+        DataSet test(params->getString(TEST_DATA_FILE), nbIn, nbOut);
+        DataSet testClass(params->getString(TEST_CLASS_FILE), nbIn, nbOut);
 
-      DataSet valid(data.GetNbEx());
-      DataSet validClass(data.GetNbEx());
+        Test = test;
+        TestClass = testClass;
+      }
 
-      data.ExtractDataAndTarget(valid, nbIn, validClass, nbOut);
+      else {
+        DataSet data(params->getString(TEST_DATA_FILE), nbIn, nbOut);
 
-      Valid = valid;
-      ValidClass = validClass;
+        DataSet test(data.GetNbEx());
+        DataSet testClass(data.GetNbEx());
 
-      data.Del();
-    }
-  }
+        data.ExtractDataAndTarget(test, nbIn, testClass, nbOut);
 
-  if (testFileInit != false) {
-    if (testTarInit != false) {
-      DataSet test(testFile, nbIn);
-      DataSet testClass(testTar, nbOut);
+        Test = test;
+        TestClass = testClass;
 
-      Test = test;
-      TestClass = testClass;
+        data.Del();
+      }
     }
 
-    else {
-      DataSet data(testFile, nbIn + nbOut);
+    auto net = std::make_shared<BagDimlp>(quant, nbLayers, vecNbNeurons, nbDimlpNets, weightFileSave);
 
-      DataSet test(data.GetNbEx());
-      DataSet testClass(data.GetNbEx());
+    net->DefNetsWithWeights(weightFile);
 
-      data.ExtractDataAndTarget(test, nbIn, testClass, nbOut);
+    float acc;
+    float accTest;
 
-      Test = test;
-      TestClass = testClass;
+    net->ComputeAcc(Train, TrainClass, &acc, 1, predTrainFile);
+    std::cout << "\n\n*** GLOBAL ACCURACY ON TRAINING SET = " << acc << "\n"
+              << std::endl;
 
-      data.Del();
-    }
-  }
-  auto net = std::make_shared<BagDimlp>(eta, mu, flat, errThres, accThres, deltaErr,
-                                        quant, showErr, epochs, nbLayers, vecNbNeurons,
-                                        nbDimlpNets, weightFile, seed);
-
-  if (nbExInOne == 0)
-    nbExInOne = Train.GetNbEx();
-  else if (nbExInOne > Train.GetNbEx())
-    nbExInOne = Train.GetNbEx();
-
-  net->MakeDataSets(Train, TrainClass, nbExInOne);
-  if (accuracyFileInit != false) {
-    ofstream accFile(accuracyFile);
-    if (accFile.is_open()) {
-      accFile << "Accuracy for Bag training : \n\n";
-      accFile.close();
-    } else {
-      string errorMsg = "Cannot open file for writing";
-      WriteError(errorMsg, accuracyFile);
+    if (Test.GetNbEx() != 0) {
+      net->ComputeAcc(Test, TestClass, &accTest, 1, predTestFile);
+      std::cout << "*** GLOBAL ACCURACY ON TESTING SET = " << accTest << "" << std::endl;
     }
-  }
-  net->TrainAll(Test, TestClass, genericWeightsFile, accuracyFile, seed);
-  float acc;
-  float accTest;
-
-  net->ComputeAcc(Train, TrainClass, &acc, 1, predTrainFile);
-  cout << "\n\n*** GLOBAL ACCURACY ON TRAINING SET = " << acc << "\n\n";
-
-  if (Test.GetNbEx() != 0) {
-    net->ComputeAcc(Test, TestClass, &accTest, 1, predTestFile);
-    cout << "*** GLOBAL ACCURACY ON TESTING SET = " << accTest << "\n";
-  }
 
-  // Output accuracy stats in file
-  if (accuracyFileInit != false) {
-    ofstream accFile(accuracyFile, ios::app);
-    if (accFile.is_open()) {
-      accFile << "-------------------------------------------------------\n";
-      accFile << "-------------------------------------------------------\n\n";
-      accFile << "Global accuracy on training set = " << acc << "\n";
-      if (Test.GetNbEx() != 0) {
-        accFile << "Global accuracy on testing set = " << accTest;
+    // Output accuracy stats in file
+    if (params->isStringSet(STATS_FILE)) {
+      std::ofstream accFile(params->getString(STATS_FILE));
+      if (accFile.is_open()) {
+        accFile << "Global accuracy on training set = " << acc << "" << std::endl;
+        if (Test.GetNbEx() != 0) {
+          accFile << "Global accuracy on testing set = " << accTest;
+        }
+        accFile.close();
+      } else {
+        throw CannotOpenFileError("Error : could not open accuracy file " + params->getString(STATS_FILE));
       }
-      accFile.close();
-    } else {
-      cout << "Error : could not open accuracy file " << accuracyFile << " not found.\n";
-      return -1;
     }
-  }
 
-  if (ruleExtr) {
-    if (attrFileInit != false) {
-      AttrName attr(attrFile, nbIn, nbOut);
+    if (params->getBool(WITH_RULE_EXTRACTION)) {
+      std::vector<std::string> attributeNames;
+      if (params->isStringSet(ATTRIBUTES_FILE)) {
+        AttrName attr(params->getString(ATTRIBUTES_FILE), nbIn, nbOut);
+
+        if (attr.ReadAttr())
+          std::cout << "\n\n"
+                    << params->getString(ATTRIBUTES_FILE) << ": Read file of attributes.\n"
+                    << std::endl;
 
-      if (attr.ReadAttr())
-        cout << "\n\n"
-             << attrFile << ": Read file of attributes.\n\n";
+        Attr = attr;
+        attributeNames = Attr.GetListAttr();
+      }
 
-      Attr = attr;
-    }
+      std::vector<int> normalizationIndices;
+      std::vector<double> mus;
+      std::vector<double> sigmas;
+
+      // Get mus, sigmas and normalizationIndices from normalizationFile for denormalization :
+      if (params->isStringSet(NORMALIZATION_FILE)) {
+        auto results = parseNormalizationStats(params->getString(NORMALIZATION_FILE), params->getInt(NB_ATTRIBUTES), attributeNames);
+        normalizationIndices = std::get<0>(results);
+        mus = std::get<2>(results);
+        sigmas = std::get<3>(results);
+        params->setIntVector(NORMALIZATION_INDICES, normalizationIndices);
+        params->setDoubleVector(MUS, mus);
+        params->setDoubleVector(SIGMAS, sigmas);
+      }
 
-    All = Train;
-    if (rulesFileInit != false) {
-      cout << "Extraction Part :: " << endl;
-    }
+      All = Train;
 
-    if (Valid.GetNbEx() > 0) {
-      DataSet all2(All, Valid);
-      All = all2;
-    }
+      std::cout << "\n\n****************************************************\n"
+                << std::endl;
+      std::cout << "*** RULE EXTRACTION" << std::endl;
+
+      std::shared_ptr<VirtualHyp> globVirt = net->MakeGlobalVirt(quant, nbIn,
+                                                                 vecNbNeurons[1] / nbIn);
 
-    cout << "\n\n****************************************************\n\n";
-    cout << "*** RULE EXTRACTION\n";
+      RealHyp ryp(globVirt, nbDimlpNets, net->GetGlobalOut(), nbOut,
+                  All, net, quant, nbIn, vecNbNeurons[1] / nbIn,
+                  nbWeightLayers);
 
-    std::shared_ptr<VirtualHyp> globVirt = net->MakeGlobalVirt(quant, nbIn,
-                                                               vecNbNeurons[1] / nbIn);
+      if (params->isStringSet(GLOBAL_RULES_OUTFILE)) {
+        std::filebuf buf;
 
-    RealHyp ryp(globVirt, nbDimlpNets, net->GetGlobalOut(), nbOut,
-                All, net, quant, nbIn, vecNbNeurons[1] / nbIn,
-                nbWeightLayers);
+        if (buf.open(params->getString(GLOBAL_RULES_OUTFILE), std::ios_base::out) == nullptr) {
+          throw CannotOpenFileError("Error : Cannot open rules file " + params->getString(GLOBAL_RULES_OUTFILE));
+        }
+
+        std::ostream rulesFileost(&buf);
+        if (params->isDoubleVectorSet(MUS)) {
+          ryp.RuleExtraction(All, Train, TrainClass, Valid, ValidClass,
+                             Test, TestClass, Attr, rulesFileost, mus, sigmas, normalizationIndices);
+        } else {
+          ryp.RuleExtraction(All, Train, TrainClass, Valid, ValidClass,
+                             Test, TestClass, Attr, rulesFileost);
+        }
 
-    if (rulesFileInit != false) {
-      filebuf buf;
+        if (ryp.TreeAborted()) {
 
-      if (buf.open(rulesFile, ios_base::out) == nullptr) {
-        string errorMsg = "Cannot open file for writing";
-        WriteError(errorMsg, rulesFile);
-      }
+          std::shared_ptr<VirtualHyp> globVirt2 = net->MakeGlobalVirt(quant, nbIn,
+                                                                      vecNbNeurons[1] / nbIn);
 
-      ostream rulesFileost(&buf);
-      ryp.RuleExtraction(All, Train, TrainClass, Valid, ValidClass,
-                         Test, TestClass, Attr, rulesFileost);
+          RealHyp2 ryp2(globVirt2, nbDimlpNets, net->GetGlobalOut(), nbOut,
+                        All, net, quant, nbIn, vecNbNeurons[1] / nbIn,
+                        nbWeightLayers);
+
+          if (params->isDoubleVectorSet(MUS)) {
+            ryp2.RuleExtraction(All, Train, TrainClass, Valid, ValidClass,
+                                Test, TestClass, Attr, rulesFileost, mus, sigmas, normalizationIndices);
+          } else {
+            ryp2.RuleExtraction(All, Train, TrainClass, Valid, ValidClass,
+                                Test, TestClass, Attr, rulesFileost);
+          }
+        }
 
-      if (ryp.TreeAborted()) {
+        std::cout << "\n\n"
+                  << params->getString(GLOBAL_RULES_OUTFILE) << ": "
+                  << "Written.\n"
+                  << std::endl;
+      } else {
+        if (params->isDoubleVectorSet(MUS)) {
+          ryp.RuleExtraction(All, Train, TrainClass, Valid, ValidClass,
+                             Test, TestClass, Attr, std::cout, mus, sigmas, normalizationIndices);
+        } else {
+          ryp.RuleExtraction(All, Train, TrainClass, Valid, ValidClass,
+                             Test, TestClass, Attr, std::cout);
+        }
 
-        std::shared_ptr<VirtualHyp> globVirt2 = net->MakeGlobalVirt(quant, nbIn,
-                                                                    vecNbNeurons[1] / nbIn);
+        if (ryp.TreeAborted()) {
 
-        RealHyp2 ryp2(globVirt2, nbDimlpNets, net->GetGlobalOut(), nbOut,
-                      All, net, quant, nbIn, vecNbNeurons[1] / nbIn,
-                      nbWeightLayers);
+          std::shared_ptr<VirtualHyp> globVirt3 = net->MakeGlobalVirt(quant, nbIn,
+                                                                      vecNbNeurons[1] / nbIn);
 
-        ryp2.RuleExtraction(All, Train, TrainClass, Valid, ValidClass,
-                            Test, TestClass, Attr, rulesFileost);
+          RealHyp2 ryp2(globVirt3, nbDimlpNets, net->GetGlobalOut(), nbOut,
+                        All, net, quant, nbIn, vecNbNeurons[1] / nbIn,
+                        nbWeightLayers);
+          if (params->isDoubleVectorSet(MUS)) {
+            ryp2.RuleExtraction(All, Train, TrainClass, Valid, ValidClass,
+                                Test, TestClass, Attr, std::cout, mus, sigmas, normalizationIndices);
+          } else {
+            ryp2.RuleExtraction(All, Train, TrainClass, Valid, ValidClass,
+                                Test, TestClass, Attr, std::cout);
+          }
+        }
       }
+    }
 
-      cout << "\n\n"
-           << rulesFile << ": "
-           << "Written.\n\n";
-    } else {
-      ryp.RuleExtraction(All, Train, TrainClass, Valid, ValidClass,
-                         Test, TestClass, Attr, cout);
+    t2 = clock();
+    temps = (float)(t2 - t1) / CLOCKS_PER_SEC;
+    std::cout << "\nFull execution time = " << temps << " sec" << std::endl;
 
-      if (ryp.TreeAborted()) {
+    std::cout.rdbuf(cout_buff); // reset to standard output again
 
-        std::shared_ptr<VirtualHyp> globVirt3 = net->MakeGlobalVirt(quant, nbIn,
-                                                                    vecNbNeurons[1] / nbIn);
+    BpNN::resetInitRandomGen();
 
-        RealHyp2 ryp2(globVirt3, nbDimlpNets, net->GetGlobalOut(), nbOut,
-                      All, net, quant, nbIn, vecNbNeurons[1] / nbIn,
-                      nbWeightLayers);
+    Train.Del();
+    TrainClass.Del();
 
-        ryp2.RuleExtraction(All, Train, TrainClass, Valid, ValidClass,
-                            Test, TestClass, Attr, cout);
-      }
+    if (Test.GetNbEx() > 0) {
+      Test.Del();
+      TestClass.Del();
     }
-  }
-
-  t2 = clock();
-  temps = (float)(t2 - t1) / CLOCKS_PER_SEC;
-  std::cout << "\nFull execution time = " << temps << " sec\n";
-
-  std::cout.rdbuf(cout_buff); // reset to standard output again
 
-  BpNN::resetInitRandomGen();
+    if (Valid.GetNbEx() > 0) {
+      Valid.Del();
+      ValidClass.Del();
+    }
 
+  } catch (const ErrorHandler &e) {
+    std::cout.rdbuf(cout_buff); // reset to standard output again
+    std::cerr << e.what() << std::endl;
+    return -1;
+  }
   return 0;
 }
 
-// Exemple to launch the code : dimlpBT("DimlpBT -L datanormTrain -1 dataclass2Train -T datanormTest -2 dataclass2Test -I 16 -H2 5 -O 2 -N 2 -w dimlpDatanormBT -p dimlpDatanormBTTrain.out -t dimlpDatanormBTTest.out -o dimlpDatanormBTStats -r dimlpDatanormBTResult.txt -S dimlp/datafiles");
+// Exemple to launch the code : dimlp.densCls("densCls --train_data_file datanormTrain --train_class_file dataclass2Train --test_data_file datanormTest --test_class_file dataclass2Test --nb_attributes 16 --hidden_layers_file hidden_layers.out --nb_classes 2 --weights_file dimlpDatanormBT.wts --with_rule_extraction true --global_rules_outfile dimlpDatanormDensClsRul.rls --train_pred_outfile dimlpDatanormDensClsTrain.out --test_pred_outfile dimlpDatanormDensClsTest.out --stats_file dimlpDatanormDensClsStats --console_file dimlpDatanormDensClsResult.txt --root_folder dimlp/datafiles");
```

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/DimlpClsFct.cpp` & `dimlpfidex-0.0.1/dimlp/cpp/src/dimlpClsFct.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -1,475 +1,371 @@
-#include "DimlpClsFct.h"
-using namespace std;
+#include "dimlpClsFct.h"
 
 ////////////////////////////////////////////////////////////
 
-void GiveAllParamDimlpCls()
+void showDimlpClsParams()
 
 {
-  cout << "\n-------------------------------------------------\n\n";
-
-  cout << "DimlpCls -T <file of examples(path with respect to specified root folder)> ";
-  cout << "-W <file of weights> ";
-  cout << "-I <number of input neurons> -O <number of output neurons>";
-  cout << " <Options>\n\n";
-
-  cout << "Options are: \n\n";
-  cout << "-S <Folder based on main folder dimlpfidex(default folder) where generated files will be saved. If a file name is specified with another option, his path will be configured with respect to this root folder>\n";
-  cout << "-2 <file of classes>\n";
-  cout << "-p <output prediction file>\n";                 // If we want to specify output prediction file, not to be dimlp.out
-  cout << "-r <file where you redirect console result>\n"; // If we want to redirect console result to file
-  cout << "-o <output file with test accuracy>\n";
-  cout << "-h <output file with first hidden layer values>\n"; // Not to be dimlp.hid
-  cout << "-H1 <number of neurons in the first hidden layer> ";
-  cout << "(if not specified this number will be equal to the ";
-  cout << "number of input neurons)\n";
-  cout << "-Hk <number of neurons in the kth hidden layer>\n";
-  cout << "-q <number of stairs in staircase activation function>\n";
-
-  cout << "\n-------------------------------------------------\n\n";
+  std::cout << std::endl
+            << "---------------------------------------------------------------------" << std::endl
+            << std::endl;
+  std::cout << "Warning! The files are localised with respect to root folder dimlpfidex." << std::endl;
+  std::cout << "The arguments can be specified in the command or in a json configuration file with --json_config_file your_config_file.json." << std::endl
+            << std::endl;
+
+  std::cout << "----------------------------" << std::endl
+            << std::endl;
+  std::cout << "Required parameters:" << std::endl
+            << std::endl;
+
+  printOptionDescription("--test_data_file <str>", "Test data file");
+  printOptionDescription("--weights_file <str>", "Weights file");
+  printOptionDescription("--nb_attributes <int [1,inf[>", "Number of input neurons");
+  printOptionDescription("--nb_classes <int [2,inf[>", "Number of output neurons");
+  printOptionDescription("--hidden_layers_file <str>", "Hidden layers file name");
+
+  std::cout << std::endl
+            << "----------------------------" << std::endl
+            << std::endl;
+  std::cout << "Optional parameters: " << std::endl
+            << std::endl;
+
+  printOptionDescription("--json_config_file <str>", "JSON file to configure all parameters. If used, this must be the sole argument and must specify the file's relative path");
+  printOptionDescription("--root_folder <str>", "Folder based on main folder dimlpfidex(default folder) containg all used files and where generated files will be saved. If a file name is specified with another option, his path will be configured with respect to this root folder");
+  printOptionDescription("--test_class_file <str>", "Test true class file");
+  printOptionDescription("--test_pred_outfile <str>", "Output test prediction file name (default: dimlpTest.out)");
+  printOptionDescription("--console_file <str>", "File with console logs redirection");
+  printOptionDescription("--stats_file <str>", "Output file name with test accuracy");
+  printOptionDescription("--hid_file <str>", "Output file name with first hidden layer values (default: dimlpTest.hid)");
+  printOptionDescription("--nb_quant_levels <int [3,inf[>", "Number of stairs in staircase activation function (default: 50)");
+
+  std::cout << std::endl
+            << "----------------------------" << std::endl
+            << std::endl;
+  std::cout << "Execution example :" << std::endl
+            << std::endl;
+  std::cout << "dimlp.dimlpCls(\"--test_data_file datanormTest.txt --test_class_file dataclass2Test.txt --weights_file weights.wts --nb_attributes 16 --hidden_layers_file hidden_layers.out --nb_classes 2 --test_pred_outfile predTest.out --stats_file stats.txt --root_folder dimlp/datafiles\")" << std::endl
+            << std::endl;
+  std::cout << "---------------------------------------------------------------------" << std::endl
+            << std::endl;
 }
 
 ////////////////////////////////////////////////////////////
 
 static void SaveOutputs(
     DataSet &data,
     Dimlp *net,
     int nbOut,
     int nbWeightLayers,
-    const char *outfile)
+    const std::string &outfile)
 
 {
-  filebuf buf;
+  std::filebuf buf;
 
-  if (buf.open(outfile, ios_base::out) == nullptr) {
-    string errorMsg = "Cannot open file for writing";
-    WriteError(errorMsg, outfile);
+  if (buf.open(outfile, std::ios_base::out) == nullptr) {
+    throw CannotOpenFileError("Error : Cannot open output file " + outfile);
   }
 
   std::shared_ptr<Layer> layer = net->GetLayer(nbWeightLayers - 1);
   const float *out = layer->GetUp();
 
-  cout << "\n\n"
-       << outfile << ": "
-       << "Writing ...\n";
+  std::cout << "\n\n"
+            << outfile << ": "
+            << "Writing ..." << std::endl;
 
-  ostream outFile(&buf);
+  std::ostream outFile(&buf);
 
   for (int p = 0; p < data.GetNbEx(); p++) {
     net->ForwardOneExample1(data, p);
 
     for (int o = 0; o < nbOut; o++) {
       outFile << out[o] << " ";
     }
 
-    outFile << "\n";
+    outFile << "" << std::endl;
   }
 
-  cout << outfile << ": "
-       << "Written.\n\n";
+  std::cout << outfile << ": "
+            << "Written.\n"
+            << std::endl;
 }
 
 ////////////////////////////////////////////////////////////
 
 void SaveFirstHid(
     DataSet &data,
     Dimlp *net,
     int nbHid,
-    const char *outfile,
-    const char *firsthidFile)
+    const std::string &outfile,
+    const std::string &firsthidFile)
 
 {
-  filebuf buf;
+  std::filebuf buf;
 
-  if (buf.open(firsthidFile, ios_base::out) == nullptr) {
-    string errorMsg = "Cannot open file for writing";
-    WriteError(errorMsg, outfile);
+  if (buf.open(firsthidFile, std::ios_base::out) == nullptr) {
+    throw CannotOpenFileError("Error : Cannot open output file " + outfile);
   }
 
   std::shared_ptr<Layer> layer = net->GetLayer(0);
   const float *hid = layer->GetUp();
 
-  cout << "\n\n"
-       << firsthidFile << ": "
-       << "Writing ...\n";
+  std::cout << "\n\n"
+            << firsthidFile << ": "
+            << "Writing ..." << std::endl;
 
-  ostream outFile(&buf);
+  std::ostream outFile(&buf);
 
   for (int p = 0; p < data.GetNbEx(); p++) {
     net->ForwardOneExample1(data, p);
 
     for (int h = 0; h < nbHid; h++) {
       outFile << hid[h] << " ";
     }
 
-    outFile << "\n";
+    outFile << "" << std::endl;
   }
 
-  cout << firsthidFile << ": "
-       << "Written.\n\n";
+  std::cout << firsthidFile << ": "
+            << "Written.\n"
+            << std::endl;
 }
 
 ////////////////////////////////////////////////////////////
 
-int dimlpCls(const string &command) {
+/**
+ * @brief Used to set default hyperparameters values and to check the sanity of all used values like boundaries and logic.
+ *
+ * @param p is the Parameter class containing all hyperparameters that rule the entire algorithm execution.
+ */
+void checkDimlpClsParametersLogicValues(Parameters &p) {
+  // setting default values
+  p.setDefaultNbQuantLevels();
+  p.setDefaultString(TEST_PRED_OUTFILE, "dimlpTest.out", true);
+  p.setDefaultString(HID_FILE, "dimlpTest.hid", true);
+
+  // this sections check if values comply with program logic
+
+  // asserting mandatory parameters
+  p.assertIntExists(NB_ATTRIBUTES);
+  p.assertIntExists(NB_CLASSES);
+  p.assertStringExists(TEST_DATA_FILE);
+  p.assertStringExists(WEIGHTS_FILE);
+  p.assertStringExists(HIDDEN_LAYERS_FILE);
 
-  // Parsing the command
-  vector<string> commandList;
-  const char delim = ' ';
-  string s;
-  stringstream ss(command);
-  while (std::getline(ss, s, delim)) {
-    commandList.push_back(s);
-  }
-  size_t nbParam = commandList.size();
-
-  DataSet Test;
-  DataSet TestClass;
+  // verifying logic between parameters, values range and so on...
+  p.checkParametersCommon();
+}
 
-  int quant = 50;
-  int nbIn = 0;
-  int nbOut = 0;
-
-  string testFileTemp;
-  bool testFileInit = false;
-  string weightFileTemp;
-  bool weightFileInit = false;
-  string predFileTemp = "dimlp.out";
-  string consoleFileTemp;
-  bool consoleFileInit = false;
-  string accuracyFileTemp;
-  bool accuracyFileInit = false;
-  string testTarTemp;
-  bool testTarInit = false;
-  string hidFileTemp = "dimlp.hid";
-  string rootFolderTemp;
-  bool rootFolderInit = false;
-
-  int nbLayers;
-  int nbWeightLayers;
-  std::vector<int> vecNbNeurons;
-
-  StringInt arch;
-  StringInt archInd;
-
-  if (nbParam <= 1) {
-    GiveAllParamDimlpCls();
-    return 0;
-  }
+int dimlpCls(const std::string &command) {
+  // Save buffer where we output results
+  std::ofstream ofs;
+  std::streambuf *cout_buff = std::cout.rdbuf(); // Save old buf
+  try {
 
-  int k = 1; // We skip "DimlpCls"
-  while (k < nbParam) {
-    if (commandList[k][0] == '-') {
-      k++;
-
-      if (k >= nbParam) {
-        cout << "Missing something at the end of the command.\n";
-        return -1;
-      }
+    float temps;
+    clock_t t1;
+    clock_t t2;
 
-      char option = commandList[k - 1][1];
-      const char *arg = &(commandList[k])[0];
-      const char *lastArg = &(commandList[k - 1])[0];
-      switch (option) {
-      case 'q':
-        if (CheckInt(arg))
-          quant = atoi(arg);
-        else
-          return -1;
-
-        break;
-
-      case 'I':
-        if (CheckInt(arg))
-          nbIn = atoi(arg);
-        else
-          return -1;
-
-        break;
-
-      case 'H':
-        if (CheckInt(arg)) {
-          arch.Insert(atoi(arg));
-
-          const char *ptrParam = lastArg;
-
-          if (ptrParam[2] != '\0') {
-            std::string str(ptrParam + 2);
-            archInd.Insert(std::atoi(str.c_str()));
-          } else {
-            cout << "Which hidden layer (-H) ?\n";
-            return -1;
-          }
-        } else
-          return -1;
+    t1 = clock();
 
-        break;
+    // Parsing the command
+    std::vector<std::string> commandList = {"dimlpCls"};
+    std::string s;
+    std::stringstream ss(command);
 
-      case 'O':
-        if (CheckInt(arg))
-          nbOut = atoi(arg);
-        else
-          return -1;
-
-        break;
-
-      case 'S':
-        rootFolderTemp = arg;
-        rootFolderInit = true;
-        break;
-
-      case 'W':
-        weightFileTemp = arg;
-        weightFileInit = true;
-        break;
-
-      case 'p':
-        predFileTemp = arg;
-        break;
-
-      case 'r':
-        consoleFileTemp = arg;
-        consoleFileInit = true;
-        break;
-
-      case 'o':
-        accuracyFileTemp = arg;
-        accuracyFileInit = true;
-        break;
-
-      case 'h':
-        hidFileTemp = arg;
-        break;
-
-      case 'T':
-        testFileTemp = arg;
-        testFileInit = true;
-        break;
-
-      case '2':
-        testTarTemp = arg;
-        testTarInit = true;
-        break;
-
-      default:
-        cout << "Illegal option: " << lastArg << "\n";
-        return -1;
-      }
+    while (ss >> s) {
+      commandList.push_back(s);
     }
 
-    else {
-      cout << "Illegal option: " << &(commandList[k])[0] << "\n";
-      return -1;
+    size_t nbParam = commandList.size();
+    if (nbParam < 2 || commandList[1] == "-h" || commandList[1] == "--help") {
+      showDimlpClsParams();
+      return 0;
     }
-    k++;
-  }
-
-  // ----------------------------------------------------------------------
 
-  // create paths with root foler
+    // Import parameters
+    std::unique_ptr<Parameters> params;
+    std::vector<ParameterCode> validParams = {TEST_DATA_FILE, WEIGHTS_FILE, NB_ATTRIBUTES, NB_CLASSES, ROOT_FOLDER, TEST_CLASS_FILE,
+                                              TEST_PRED_OUTFILE, CONSOLE_FILE, STATS_FILE, HID_FILE, HIDDEN_LAYERS_FILE, NB_QUANT_LEVELS};
+    if (commandList[1].compare("--json_config_file") == 0) {
+      if (commandList.size() < 3) {
+        throw CommandArgumentException("JSON config file name/path is missing");
+      } else if (commandList.size() > 3) {
+        throw CommandArgumentException("Option " + commandList[1] + " has to be the only option in the command if specified.");
+      }
+      try {
+        params = std::unique_ptr<Parameters>(new Parameters(commandList[2], validParams));
+      } catch (const std::out_of_range &e) {
+        throw CommandArgumentException("Some value inside your JSON config file '" + commandList[2] + "' is out of range.\n(Probably due to a too large or too tiny numeric value).");
+      } catch (const std::exception &e) {
+        std::string msg(e.what()) ;
+        throw CommandArgumentException("Unknown JSON config file error: " + msg);
+      }
+    } else {
+      // Read parameters from CLI
+      params = std::unique_ptr<Parameters>(new Parameters(commandList, validParams));
+    }
 
-  const char *testFile = nullptr;
-  const char *weightFile = nullptr;
-  const char *predFile = nullptr;
-  const char *consoleFile = nullptr;
-  const char *accuracyFile = nullptr;
-  const char *testTar = nullptr;
-  const char *hidFile = nullptr;
-
-  string root = "";
-  if (rootFolderInit) {
-#if defined(__unix__) || defined(__APPLE__)
-    root = rootFolderTemp + "/";
-#elif defined(_WIN32)
-    root = rootFolderTemp + "\\";
-#endif
-  }
+    // getting all program arguments from CLI
+    checkDimlpClsParametersLogicValues(*params);
 
-  if (testFileInit) {
-    testFileTemp = root + testFileTemp;
-    testFile = &testFileTemp[0];
-  }
+    // Get console results to file
+    if (params->isStringSet(CONSOLE_FILE)) {
+      ofs.open(params->getString(CONSOLE_FILE));
+      std::cout.rdbuf(ofs.rdbuf()); // redirect cout to file
+    }
 
-  if (weightFileInit) {
-    weightFileTemp = root + weightFileTemp;
-    weightFile = &weightFileTemp[0];
-  }
+    // Show chosen parameters
+    std::cout << *params;
 
-  predFileTemp = root + predFileTemp;
-  predFile = &predFileTemp[0];
+    // ----------------------------------------------------------------------
 
-  if (consoleFileInit) {
-    consoleFileTemp = root + consoleFileTemp;
-    consoleFile = &consoleFileTemp[0];
-  }
+    // Get parameters values
 
-  if (accuracyFileInit) {
-    accuracyFileTemp = root + accuracyFileTemp;
-    accuracyFile = &accuracyFileTemp[0];
-  }
+    int nbIn = params->getInt(NB_ATTRIBUTES);
+    int nbOut = params->getInt(NB_CLASSES);
+    std::string testFile = params->getString(TEST_DATA_FILE);
+    std::string weightFile = params->getString(WEIGHTS_FILE);
+    std::string hidFile = params->getString(HID_FILE);
+    std::string predFile = params->getString(TEST_PRED_OUTFILE);
+    int quant = params->getInt(NB_QUANT_LEVELS);
+
+    DataSet Test;
+    DataSet TestClass;
+    int nbLayers;
+    int nbWeightLayers;
+    std::vector<int> vecNbNeurons;
+    StringInt arch;
+    StringInt archInd;
+    params->readHiddenLayersFile(arch, archInd);
+
+    // ----------------------------------------------------------------------
+    if (arch.GetNbEl() == 0) {
+      nbLayers = 3;
+      nbWeightLayers = nbLayers - 1;
 
-  if (testTarInit) {
-    testTarTemp = root + testTarTemp;
-    testTar = &testTarTemp[0];
-  }
+      vecNbNeurons.assign(nbLayers, 0);
+      vecNbNeurons[0] = nbIn;
+      vecNbNeurons[1] = nbIn;
+      vecNbNeurons[2] = nbOut;
+    } else {
+      archInd.GoToBeg();
 
-  hidFileTemp = root + hidFileTemp;
-  hidFile = &hidFileTemp[0];
+      if (archInd.GetVal() == 1) {
+        arch.GoToBeg();
 
-  // ----------------------------------------------------------------------
-  // Get console results to file
-  std::ofstream ofs;
-  std::streambuf *cout_buff = std::cout.rdbuf(); // Save old buf
-  if (consoleFileInit != false) {
-    ofs.open(consoleFile);
-    std::cout.rdbuf(ofs.rdbuf()); // redirect std::cout to file
-  }
+        if (arch.GetVal() % nbIn != 0) {
+          throw InternalError("The number of neurons in the first hidden layer must be a multiple of the number of input neurons.");
+        }
 
-  // ----------------------------------------------------------------------
+        nbLayers = arch.GetNbEl() + 2;
+        nbWeightLayers = nbLayers - 1;
 
-  if (quant <= 2) {
-    cout << "The number of quantized levels must be greater than 2.\n";
-    return -1;
-  }
+        vecNbNeurons.assign(nbLayers, 0);
+        vecNbNeurons[0] = nbIn;
+        vecNbNeurons[nbLayers - 1] = nbOut;
+        arch.GoToBeg();
+        for (int p = 1; p <= arch.GetNbEl(); p++, arch.GoToNext()) {
+          vecNbNeurons[p] = arch.GetVal();
 
-  if (nbIn == 0) {
-    cout << "The number of input neurons must be given with option -I.\n";
-    return -1;
-  }
-
-  if (nbOut <= 1) {
-    cout << "At least two output neurons must be given with option -O.\n";
-    return -1;
-  }
-
-  // ----------------------------------------------------------------------
-  if (arch.GetNbEl() == 0) {
-    nbLayers = 3;
-    nbWeightLayers = nbLayers - 1;
-
-    vecNbNeurons.assign(nbLayers, 0);
-    vecNbNeurons[0] = nbIn;
-    vecNbNeurons[1] = nbIn;
-    vecNbNeurons[2] = nbOut;
-  } else {
-    archInd.GoToBeg();
-
-    if (archInd.GetVal() == 1) {
-      arch.GoToBeg();
-
-      if (arch.GetVal() % nbIn != 0) {
-        cout << "The number of neurons in the first hidden layer must be";
-        cout << " a multiple of the number of input neurons.\n";
-        return -1;
+          if (vecNbNeurons[p] == 0) {
+            throw InternalError("The number of neurons must be greater than 0.");
+          }
+        }
       }
 
-      nbLayers = arch.GetNbEl() + 2;
-      nbWeightLayers = nbLayers - 1;
-
-      vecNbNeurons.assign(nbLayers, 0);
-      vecNbNeurons[0] = nbIn;
-      vecNbNeurons[nbLayers - 1] = nbOut;
-
-      for (k = 1, arch.GoToBeg(); k <= arch.GetNbEl(); k++, arch.GoToNext()) {
-        vecNbNeurons[k] = arch.GetVal();
+      else {
+        nbLayers = arch.GetNbEl() + 3;
+        nbWeightLayers = nbLayers - 1;
+
+        vecNbNeurons.assign(nbLayers, 0);
+        vecNbNeurons[0] = nbIn;
+        vecNbNeurons[1] = nbIn;
+        vecNbNeurons[nbLayers - 1] = nbOut;
+
+        arch.GoToBeg();
+        for (int p = 1; p <= arch.GetNbEl(); p++, arch.GoToNext()) {
+          vecNbNeurons[p + 1] = arch.GetVal();
 
-        if (vecNbNeurons[k] == 0) {
-          cout << "The number of neurons must be greater than 0.\n";
-          return -1;
+          if (vecNbNeurons[p + 1] == 0) {
+            throw InternalError("The number of neurons must be greater than 0.");
+          }
         }
       }
     }
+    // ----------------------------------------------------------------------
 
-    else {
-      nbLayers = arch.GetNbEl() + 3;
-      nbWeightLayers = nbLayers - 1;
+    if (params->isStringSet(TEST_DATA_FILE)) {
+      if (params->isStringSet(TEST_CLASS_FILE)) {
 
-      vecNbNeurons.assign(nbLayers, 0);
-      vecNbNeurons[0] = nbIn;
-      vecNbNeurons[1] = nbIn;
-      vecNbNeurons[nbLayers - 1] = nbOut;
+        DataSet test(testFile, nbIn, nbOut);
+        DataSet testClass(params->getString(TEST_CLASS_FILE), nbIn, nbOut);
 
-      for (k = 1, arch.GoToBeg(); k <= arch.GetNbEl(); k++, arch.GoToNext()) {
-        vecNbNeurons[k + 1] = arch.GetVal();
-
-        if (vecNbNeurons[k + 1] == 0) {
-          cout << "The number of neurons must be greater than 0.\n";
-          return -1;
-        }
+        Test = test;
+        TestClass = testClass;
       }
-    }
-  }
-  // ----------------------------------------------------------------------
 
-  if (testFileInit == false) {
-    cout << "Give a testing file with -T selection please."
-         << "\n";
-    return -1;
-  }
+      else {
+        DataSet data(testFile, nbIn, nbOut);
+
+        DataSet test(data.GetNbEx());
+        DataSet testClass(data.GetNbEx());
 
-  else // if (testFileInit != false)
-  {
-    if (testTarInit != false) {
+        data.ExtractDataAndTarget(test, nbIn, testClass, nbOut);
 
-      DataSet test(testFile, nbIn);
-      DataSet testClass(testTar, nbOut);
+        Test = test;
+        TestClass = testClass;
 
-      Test = test;
-      TestClass = testClass;
+        data.Del();
+      }
     }
 
-    else {
-      DataSet data(testFile, nbIn + nbOut);
+    Dimlp net(weightFile, nbLayers, vecNbNeurons, quant);
 
-      DataSet test(data.GetNbEx());
-      DataSet testClass(data.GetNbEx());
+    float acc;
 
-      data.ExtractDataAndTarget(test, nbIn, testClass, nbOut);
+    float err = net.Error(Test, TestClass, &acc);
 
-      Test = test;
-      TestClass = testClass;
+    std::cout << "\n\n*** SUM SQUARED ERROR = " << err;
+    std::cout << "\n\n*** ACCURACY = " << acc << "" << std::endl;
 
-      data.Del();
+    // Output accuracy stats in file
+    if (params->isStringSet(STATS_FILE)) {
+      std::ofstream accFile(params->getString(STATS_FILE));
+      if (accFile.is_open()) {
+        accFile << "Sum squared error = " << err << "" << std::endl;
+        accFile << "Accuracy = " << acc;
+        accFile.close();
+      } else {
+        throw CannotOpenFileError("Error : could not open accuracy file " + params->getString(STATS_FILE));
+      }
     }
-  }
-  if (weightFileInit == false) {
-    cout << "Give a file of weights with -W selection please."
-         << "\n";
-    return -1;
-  }
-
-  Dimlp net(weightFile, nbLayers, vecNbNeurons, quant);
 
-  float acc;
+    SaveOutputs(Test, &net, nbOut, nbWeightLayers, predFile);
+    SaveFirstHid(Test, &net, vecNbNeurons[1], predFile, hidFile);
 
-  float err = net.Error(Test, TestClass, &acc);
+    std::cout << "\n-------------------------------------------------\n"
+              << std::endl;
 
-  cout << "\n\n*** SUM SQUARED ERROR = " << err;
-  cout << "\n\n*** ACCURACY = " << acc << "\n";
+    t2 = clock();
+    temps = (float)(t2 - t1) / CLOCKS_PER_SEC;
+    std::cout << "\nFull execution time = " << temps << " sec" << std::endl;
 
-  // Output accuracy stats in file
-  if (accuracyFileInit != false) {
-    ofstream accFile(accuracyFile);
-    if (accFile.is_open()) {
-      accFile << "Sum squared error = " << err << "\n";
-      accFile << "Accuracy = " << acc;
-      accFile.close();
-    } else {
-      cout << "Error : could not open accuracy file " << accuracyFile << " not found.\n";
-      return -1;
-    }
-  }
+    std::cout.rdbuf(cout_buff); // reset to standard output again
 
-  SaveOutputs(Test, &net, nbOut, nbWeightLayers, predFile);
-  SaveFirstHid(Test, &net, vecNbNeurons[1], predFile, hidFile);
+    BpNN::resetInitRandomGen();
 
-  cout << "\n-------------------------------------------------\n\n";
-
-  std::cout.rdbuf(cout_buff); // reset to standard output again
+    if (Test.GetNbEx() > 0) {
+      Test.Del();
+      TestClass.Del();
+    }
 
-  BpNN::resetInitRandomGen();
+  } catch (const ErrorHandler &e) {
+    std::cout.rdbuf(cout_buff); // reset to standard output again
+    std::cerr << e.what() << std::endl;
+    return -1;
+  }
 
   return 0;
 }
 
-// Exemple to launch the code : dimlpCls("DimlpCls -T datanormTest -2 dataclass2Test -W dimlpDatanorm.wts -I 16 -H2 5 -O 2 -q 50 -p dimlpDatanormTest.out -o dimlpDatanormClsStats -r dimlpDatanormClsResult.txt -S dimlp/datafiles");
+// Exemple to launch the code : dimlp.dimlpCls("dimlpCls --test_data_file datanormTest --test_class_file dataclass2Test --weights_file dimlpDatanorm.wts --nb_attributes 16 --hidden_layers_file hidden_layers.out --nb_classes 2 --nb_quant_levels 50 --test_pred_outfile dimlpDatanormTest.out --stats_file dimlpDatanormClsStats --console_file dimlpDatanormClsResult.txt --root_folder dimlp/datafiles");
```

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/attrName.h` & `dimlpfidex-0.0.1/dimlp/cpp/src/attrName.h`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #ifndef ATTRNAME_H
 #define ATTRNAME_H
 
-#include "writeErr.h"
+#include "../../../common/cpp/src/checkFun.h"
+#include "../../../common/cpp/src/errorHandler.h"
 #include <fstream>
 #include <iostream>
 #include <string.h>
 #include <vector>
 
 class AttrName {
   int NbAttr;
@@ -20,12 +21,12 @@
 
 public:
   int ReadAttr();
   int IsFileAttr() const { return (FileAttr.empty() ? 0 : 1); }
   std::vector<std::string> GetListAttr() const { return VarNames; }
   std::vector<std::string> GetListClasses() const { return ClassNames; }
 
-  AttrName(const char *fileAttr, int nbAttr, int nbClasses);
+  AttrName(const std::string &fileAttr, int nbAttr, int nbClasses);
   AttrName() = default;
 };
 
 #endif
```

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/bagDimlp.cpp` & `dimlpfidex-0.0.1/dimlp/cpp/src/bagDimlp.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 #ifndef BAG
-#include "writeErr.h"
 #include <stdio.h>
 #include <string.h>
 #endif
 
 #include "bagDimlp.h"
 
 #include <fstream>
-using namespace std;
 
 ///////////////////////////////////////////////////////////////////
 
 void BagDimlp::MakeDataSets(
     DataSet &masterTrain,
     DataSet &masterClass,
     int nbPat)
@@ -35,16 +33,16 @@
     for (p = 0; p < nbPat; p++) {
       val = ri.RandomInteger();
       indPat[p] = val;
       busy[val] = 1;
     }
 
     count = static_cast<int>(std::count(busy.begin(), busy.end(), 0));
-    cout << "Network " << n + 1 << " Number of Validation Examples = ";
-    cout << count << "\n";
+    std::cout << "Network " << n + 1 << " Number of Validation Examples = ";
+    std::cout << count << "" << std::endl;
 
     // indVal = new int[count];
     std::vector<int> indVal(count);
 
     for (p = 0, k = 0; p < nbPat; p++)
       if (busy[p] == 0) {
         indVal[k] = p;
@@ -59,69 +57,69 @@
 }
 
 ///////////////////////////////////////////////////////////////////
 
 void BagDimlp::TrainAll(
     DataSet &test,
     DataSet &testTar,
-    const char genericWeightsFile[],
-    const char *accuracyFile,
+    const std::string &weightsFile,
+    const std::string &accuracyFile,
     int seed)
 
 {
-  string str1;
+  std::string str1;
+
+  // Remove content from weightsFile
+  std::ofstream(weightsFile, std::ios::out).close();
 
   for (int n = 0; n < NbDimlpNets; n++) {
-    cout << "\n\n-------------------------------------------------------";
-    cout << "---------------------------";
+    std::cout << "\n\n-------------------------------------------------------";
+    std::cout << "---------------------------";
 
-    cout << "\n\nTraining network " << n + 1 << "\n";
+    std::cout << "\n\nTraining network " << n + 1 << "" << std::endl;
 
     // Output accuracy on file
-    if (accuracyFile != nullptr) {
-      ofstream accFile(accuracyFile, ios::app);
+    if (!accuracyFile.empty()) {
+      std::ofstream accFile(accuracyFile, std::ios::app);
       if (accFile.is_open()) {
-        accFile << "Network " << n + 1 << " : \n\n";
+        accFile << "Network " << n + 1 << " : \n"
+                << std::endl;
         accFile.close();
       } else {
-        string errorMsg = "Cannot open file for writing";
-        WriteError(errorMsg, accuracyFile);
+        throw CannotOpenFileError("Error : Cannot open accuracy file " + accuracyFile);
       }
     }
 
     VectDimlp[n] = std::make_shared<Dimlp>(Eta, Mu, Flat, ErrParam, AccuracyParam,
                                            DeltaErrParam, DiscrLevels, ShowErrParam,
                                            NbEpochsParam, NbLayers, NbNeurons, WeightFile, seed);
     bool fromBT = true;
     VectDimlp[n]->Dimlp::Train(*(VectData[n]), *(VectDataClass[n]),
                                test, testTar,
                                *(ValData[n]), *(ValDataClass[n]), accuracyFile, fromBT);
 
-    str1 = genericWeightsFile + std::to_string(n + 1) + ".wts";
-
-    VectDimlp[n]->Dimlp::SaveWeights(str1.c_str());
+    VectDimlp[n]->Dimlp::SaveWeights(weightsFile, n + 1);
   }
 }
 
 ///////////////////////////////////////////////////////////////////
 
-void BagDimlp::DefNetsWithWeights(const char *prefix)
+void BagDimlp::DefNetsWithWeights(const std::string &prefix)
 
 {
-  string str1;
+  std::string str1;
 
   for (int n = 0; n < NbDimlpNets; n++) {
-    cout << "\n\n-------------------------------------------------------";
-    cout << "---------------------------";
+    std::cout << "\n\n-------------------------------------------------------";
+    std::cout << "---------------------------";
 
-    cout << "\n\nBuilding network " << n + 1 << "\n";
+    std::cout << "\n\nBuilding network " << n + 1 << "" << std::endl;
 
-    str1 = prefix + std::to_string(n + 1) + ".wts";
-    VectDimlp[n] = std::make_shared<Dimlp>(str1.c_str(), NbLayers, NbNeurons,
-                                           DiscrLevels);
+    VectDimlp[n] = std::make_shared<Dimlp>(prefix, NbLayers, NbNeurons,
+                                           DiscrLevels, n + 1);
   }
 }
 
 ///////////////////////////////////////////////////////////////////
 
 std::shared_ptr<VirtualHyp> BagDimlp::MakeGlobalVirt(int nbBins, int nbIn, int multiple)
 
@@ -194,37 +192,37 @@
 ///////////////////////////////////////////////////////////////////
 
 void BagDimlp::ComputeAcc(
     DataSet &data,
     DataSet &target,
     float *accuracy,
     int toWrite,
-    const char predFile[])
+    const std::string &predFile)
 
 {
   int p;
   int ansNet;
   int ansTar;
   int good;
   int bad;
   std::vector<float> ptrOut;
   std::vector<float> ptrTar;
-  ofstream buf;
+  std::ofstream buf;
 
   const int nbPat = data.GetNbEx();
   const int nbOut = target.GetNbAttr();
 
   if (toWrite) {
-    cout << "\n\n"
-         << predFile << ": "
-         << "Writing ...\n";
+    std::cout << "\n\n"
+              << predFile << ": "
+              << "Writing ..." << std::endl;
   }
   buf.open(predFile);
   if (!buf)
-    cout << "Cannot open file for writing";
+    std::cout << "Cannot open file for writing";
 
   for (p = 0, good = 0, bad = 0; p < nbPat; p++) {
     BagDimlp::ForwardOneExample1(data, p);
 
     ptrOut = GlobalOut;
     ptrTar.assign(target.GetExample(p), target.GetExample(p) + nbOut);
 
@@ -237,20 +235,21 @@
       bad++;
 
     if (toWrite) {
       for (int o = 0; o < nbOut; o++) {
         buf << ptrOut[o] << " ";
       }
 
-      buf << "\n";
+      buf << "" << std::endl;
     }
   }
   if (toWrite) {
-    cout << predFile << ": "
-         << "Written.\n\n";
+    std::cout << predFile << ": "
+              << "Written.\n"
+              << std::endl;
   }
 
   *accuracy = static_cast<float>(good) + static_cast<float>(bad);
   *accuracy = (float)good / *accuracy;
 }
 
 ///////////////////////////////////////////////////////////////////
@@ -264,15 +263,15 @@
     float deltaErrParam,
     int discrLevels,
     int showErrParam,
     int nbEpochsParam,
     int nbLayers,
     std::vector<int> nbNeurons,
     int nbDimlpNets,
-    const char weightFile[],
+    const std::string &weightFile,
     int seed) :
 
                 Dimlp(eta, mu, flat, errParam, accuracyParam, deltaErrParam,
                       discrLevels, showErrParam, nbEpochsParam, nbLayers, nbNeurons, weightFile, seed),
                 NbDimlpNets(nbDimlpNets), Eta(eta), Mu(mu), Flat(flat), ErrParam(errParam), AccuracyParam(accuracyParam),
                 DeltaErrParam(deltaErrParam), DiscrLevels(discrLevels), ShowErrParam(showErrParam),
                 NbEpochsParam(nbEpochsParam), NbLayers(nbLayers), WeightFile(weightFile)
@@ -280,15 +279,16 @@
 {
 
   NbNeurons.assign(nbLayers, 0);
 
   for (int n = 0; n < nbLayers; n++)
     NbNeurons[n] = nbNeurons[n];
 
-  cout << "Number of networks = " << nbDimlpNets << "\n\n";
+  std::cout << "Number of networks = " << nbDimlpNets << "\n"
+            << std::endl;
 
   VectData.resize(nbDimlpNets);
   VectDataClass.resize(nbDimlpNets);
   ValData.resize(nbDimlpNets);
   ValDataClass.resize(nbDimlpNets);
 
   VectDimlp.resize(nbDimlpNets);
@@ -300,27 +300,28 @@
 ///////////////////////////////////////////////////////////////////
 
 BagDimlp::BagDimlp(
     int discrLevels,
     int nbLayers,
     std::vector<int> nbNeurons,
     int nbDimlpNets,
-    const char weightFile[],
+    const std::string &weightFile,
     int seed) :
 
                 Dimlp(0, 0, 0, 0, 0, 0, discrLevels, 0, 0, nbLayers, nbNeurons, weightFile, seed),
                 NbDimlpNets(nbDimlpNets), DiscrLevels(discrLevels), NbLayers(nbLayers), WeightFile(weightFile)
 
 {
   NbNeurons.assign(nbLayers, 0);
 
   for (int n = 0; n < nbLayers; n++)
     NbNeurons[n] = nbNeurons[n];
 
-  cout << "Number of networks = " << nbDimlpNets << "\n\n";
+  std::cout << "Number of networks = " << nbDimlpNets << "\n"
+            << std::endl;
 
   VectDimlp.resize(nbDimlpNets);
 
   NbOut = nbNeurons[NbLayers - 1];
   // GlobalOut = new float[NbOut];
   GlobalOut.resize(NbOut);
 }
```

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/bagDimlp.h` & `dimlpfidex-0.0.1/dimlp/cpp/src/bagDimlp.h`

 * *Files 26% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   float ErrParam;
   float AccuracyParam;
   float DeltaErrParam;
   int DiscrLevels;
   int ShowErrParam;
   int NbEpochsParam;
   int NbLayers;
-  const char *WeightFile;
+  const std::string &WeightFile;
 
   std::vector<int> NbNeurons;
 
   std::vector<float> GlobalOut;
 
   std::vector<std::shared_ptr<Dimlp>> VectDimlp;
   std::vector<std::shared_ptr<DataSet>> VectData;
@@ -39,46 +39,46 @@
 public:
   float *GetGlobalOut() { return GlobalOut.data(); }
   void MakeDataSets(DataSet &masterTrain, DataSet &masterClass, int nbPat);
 
   void TrainAll(
       DataSet &test,
       DataSet &testTar,
-      const char genericWeightsFile[],
-      const char *accuracyFile,
+      const std::string &genericWeightsFile,
+      const std::string &accuracyFile,
       int seed = 0);
-  void DefNetsWithWeights(const char *prefix);
+  void DefNetsWithWeights(const std::string &prefix);
 
   std::shared_ptr<VirtualHyp> MakeGlobalVirt(int nbBins, int nbIn, int multiple);
 
   using BpNN::ForwardOneExample1;
   void ForwardOneExample1(DataSet &data, int index) override;
   void ForwardOneExample1() override;
 
-  void ComputeAcc(DataSet &data, DataSet &target, float *accuracy, int tW, const char predFile[]);
+  void ComputeAcc(DataSet &data, DataSet &target, float *accuracy, int tW, const std::string &predFile);
 
   BagDimlp(
       float eta,
       float mu,
       float flat,
       float errParam,
       float accuracyParam,
       float deltaErrParam,
       int discrLevels,
       int showErrParam,
       int nbEpochsParam,
       int nbLayers,
       std::vector<int> nbNeurons,
       int nbDimlpNets,
-      const char weightFile[],
+      const std::string &weightFile,
       int seed = 0);
 
   BagDimlp(
       int discrLevels,
       int nbLayers,
       std::vector<int> nbNeurons,
       int nbDimlpNets,
-      const char weightFile[],
+      const std::string &weightFile,
       int seed = 0);
 };
 
 #endif
```

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/bpNN.cpp` & `dimlpfidex-0.0.1/dimlp/cpp/src/bpNN.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 #include "bpNN.h"
 
 const int LLL = 1;
 const int LD3 = 1;
 const int LD4 = 1;
 
-using namespace std;
-
 ///////////////////////////////////////////////////////////////////
 
 int BpNN::Max(const std::vector<float> &vec) const
 
 {
   float max = vec[0];
   int indMax = 0;
@@ -37,15 +35,16 @@
   if (initRandomGen == 0) {
 
     IntRandomFunction irf(seed);
     FloatRandomFunction frf(seed);
 
     initRandomGen++;
 
-    cout << "\nRandom number generator initialized.\n\n";
+    std::cout << "\nRandom number generator initialized.\n"
+              << std::endl;
   }
 }
 
 ///////////////////////////////////////////////////////////////////
 
 void BpNN::CreateNetStruct(std::vector<int> nbNeurons)
 
@@ -75,19 +74,20 @@
 ///////////////////////////////////////////////////////////////////
 
 void BpNN::WriteArchParam() const
 
 {
   int l;
 
-  cout << "\n\nArchitecture: ";
+  std::cout << "\n\nArchitecture: ";
 
   for (l = 0; l < NbLayers - 1; l++)
-    cout << NbNeurons[l] << "-";
-  cout << NbNeurons[l] << "\n\n";
+    std::cout << NbNeurons[l] << "-";
+  std::cout << NbNeurons[l] << "\n"
+            << std::endl;
 }
 
 ///////////////////////////////////////////////////////////////////
 
 void BpNN::AssignParam(
     float eta,
     float mu,
@@ -114,109 +114,154 @@
 
   NbWeightLayers = nbLayers - 1;
 }
 
 ///////////////////////////////////////////////////////////////////
 
 void BpNN::WriteParam() const {
-  cout << "Parameters:\n\n";
+  std::cout << "Parameters:\n"
+            << std::endl;
 
-  cout << "Eta                   = " << Eta << "\n";
-  cout << "Mu                    = " << Mu << "\n";
-  cout << "Flat                  = " << Flat << "\n";
+  std::cout << "Eta                   = " << Eta << "" << std::endl;
+  std::cout << "Mu                    = " << Mu << "" << std::endl;
+  std::cout << "Flat                  = " << Flat << "" << std::endl;
 
   if (ErrParam >= 0)
-    cout << "Error Threshold       = " << ErrParam << "\n";
+    std::cout << "Error Threshold       = " << ErrParam << "" << std::endl;
 
   if (AccuracyParam <= 1)
-    cout << "Accuracy Threshold    = " << AccuracyParam << "\n";
+    std::cout << "Accuracy Threshold    = " << AccuracyParam << "" << std::endl;
 
   if (DeltaErrParam != 0)
-    cout << "Delta Error Threshold = " << DeltaErrParam << "\n";
+    std::cout << "Delta Error Threshold = " << DeltaErrParam << "" << std::endl;
 
-  cout << "Show Error            = " << ShowErrParam << "\n";
+  std::cout << "Show Error            = " << ShowErrParam << "" << std::endl;
 
   if (NbEpochsParam < 1000000000)
-    cout << "Epochs                = " << NbEpochsParam << "\n";
+    std::cout << "Epochs                = " << NbEpochsParam << "" << std::endl;
 
-  cout << "\n";
+  std::cout << "" << std::endl;
 }
 
 ///////////////////////////////////////////////////////////////////
 
 void BpNN::SaveWeights() const
 
 {
-  filebuf buf;
+  std::filebuf buf;
 
-  if (buf.open(SaveFile, ios_base::out) == nullptr) {
-    string errorMsg = "Cannot open file for writing";
-    WriteError(errorMsg, SaveFile);
+  if (buf.open(SaveFile, std::ios_base::out) == nullptr) {
+    throw CannotOpenFileError("Error : Cannot open save file " + std::string(SaveFile));
   }
 
-  ostream outFile(&buf);
+  std::ostream outFile(&buf);
 
-  cout << "\n\n"
-       << SaveFile << ": "
-       << "Writing ...\n";
+  std::cout << "\n\n"
+            << SaveFile << ": "
+            << "Writing ..." << std::endl;
 
   for (int n = 0; n < NbWeightLayers; n++)
     VecLayer[n]->WriteWeights(outFile);
 
-  cout << SaveFile << ": "
-       << "Written.\n\n";
+  std::cout << SaveFile << ": "
+            << "Written.\n"
+            << std::endl;
 }
 
 ///////////////////////////////////////////////////////////////////
 
-void BpNN::SaveWeights(const char *strSave) const
+void BpNN::SaveWeights(const std::string &strSave, int netId) const
 
 {
-  filebuf buf;
+  std::filebuf buf;
 
-  if (buf.open(strSave, ios_base::out) == nullptr) {
-    string errorMsg = "Cannot open file for writing";
-    WriteError(errorMsg, strSave);
+  if (buf.open(strSave, std::ios_base::out | std::ios_base::app) == nullptr) {
+    throw CannotOpenFileError("Error : Cannot open save file " + strSave);
   }
-  ostream outFile(&buf);
+  std::ostream outFile(&buf);
 
-  cout << "\n\n"
-       << strSave << ": "
-       << "Writing ...\n";
+  std::cout << "\n\n"
+            << strSave << ": "
+            << "Writing net " << netId << "..." << std::endl;
 
+  outFile << "Network " << netId << " " << std::endl
+          << std::endl;
   for (int n = 0; n < NbWeightLayers; n++)
     VecLayer[n]->WriteWeights(outFile);
 
-  cout << strSave << ": "
-       << "Written.\n\n";
+  outFile << std::endl;
+
+  std::cout << strSave << ": "
+            << "Written network " << netId << ".\n"
+            << std::endl;
 }
 
 ///////////////////////////////////////////////////////////////////
 
 void BpNN::ReadWeights() const
 
 {
-  filebuf buf;
+  std::filebuf buf;
 
-  if (buf.open(ReadFile, ios_base::in) == nullptr) {
-    string errorMsg = "Cannot open input file ";
-    WriteError(errorMsg, ReadFile);
+  if (buf.open(ReadFile, std::ios_base::in) == nullptr) {
+    throw CannotOpenFileError("Cannot open input file " + ReadFile);
   }
 
-  istream inFile(&buf);
+  std::istream inFile(&buf);
+
+  std::string line;
+  bool isCurrentNetwork = false;
+  bool containsNetworkMarkers = false;
+
+  while (std::getline(inFile, line)) {
+    if (line.find("Network ") != std::string::npos) {
+      containsNetworkMarkers = true; // Network markers found
+      break;
+    }
+  }
+  inFile.clear();
+  inFile.seekg(0, std::ios::beg); // Reinitialise cursor to the beginning
 
-  cout << "\n\n"
-       << ReadFile << ": "
-       << "Reading ...\n";
+  // If the file contains network markers, look for the specific network ID.
+  if (containsNetworkMarkers) {
+    std::cout << "\n\n"
+              << ReadFile << " network " << NetId << ": "
+              << "Reading ..." << std::endl;
+    int n = 0;
+    while (std::getline(inFile, line)) {
+      if (line.find("Network " + std::to_string(NetId)) != std::string::npos) {
+        isCurrentNetwork = true; // Start of the desired network block
+        continue;
+      }
+      if (isCurrentNetwork && line.find("Network ") != std::string::npos) {
+        break; // Start of the next network block, stop reading
+      }
 
-  for (int n = 0; n < NbLayers - 1; n++)
-    VecLayer[n]->ReadWeights(inFile);
+      // When in the desired network block
+      if (isCurrentNetwork && !checkStringEmpty(line) && n < NbLayers - 1) {
+        std::string weightsData = line + "\n";
+        if (std::getline(inFile, line)) { // Assuming the next line of weights immediately follows
+          weightsData += line;            // Merge two lines for weights
+          std::istringstream iss(weightsData);
+          VecLayer[n]->ReadWeights(iss);
+          n += 1;
+        }
+      }
+    }
+  } else { // The file contains just one network
+    std::cout << "\n\n"
+              << ReadFile << ": "
+              << "Reading ..." << std::endl;
+    for (int m = 0; m < NbLayers - 1; m++)
+      VecLayer[m]->ReadWeights(inFile);
+  }
 
-  cout << ReadFile << ": "
-       << "Read.\n\n";
+  std::cout << ReadFile << ": "
+            << "Read.\n"
+            << std::endl;
 }
 
 ///////////////////////////////////////////////////////////////////
 
 void BpNN::Push() const
 
 {
@@ -566,36 +611,32 @@
 {
   int p;
   int ansNet;
   int ansTar;
   int good;
   int bad;
   float sum;
-  vector<float> ptrOut;
-  vector<float> ptrTar;
+  std::vector<float> ptrOut;
+  std::vector<float> ptrTar;
   const int nbPat = data.GetNbEx();
   const int nbOut = target.GetNbAttr();
-
   for (p = 0, sum = 0.0, good = 0, bad = 0; p < nbPat; p++) {
     ForwardOneExample1(data, p);
-
     ptrOut.assign(VecLayer[NbWeightLayers - 1]->GetUp(), VecLayer[NbWeightLayers - 1]->GetUp() + nbOut);
     ptrTar.assign(target.GetExample(p), target.GetExample(p) + nbOut);
-
     ansNet = Max(ptrOut);
     ansTar = Max(ptrTar);
 
     sum += VecLayer[NbWeightLayers - 1]->HalfErrFunct(nbOut, ptrOut, ptrTar);
 
     if (ansNet == ansTar)
       good++;
     else
       bad++;
   }
-
   *accuracy = static_cast<float>(good) + static_cast<float>(bad);
   *accuracy = (float)good / *accuracy;
 
   return sum;
 }
 
 ///////////////////////////////////////////////////////////////////
@@ -603,15 +644,15 @@
 void BpNN::TrainPhase(
     DataSet &train,
     DataSet &trainTar,
     DataSet &test,
     DataSet &testTar,
     DataSet &valid,
     DataSet &validTar,
-    const char *accuracyFile,
+    const std::string &accuracyFile,
     bool fromBT)
 
 {
   float oldErr = 0;
   float acc;
   float err;
   float specAcc;
@@ -631,38 +672,42 @@
 
   specErr = ComputeErrorSameAct(train, trainTar, &specAcc);
   PrintSpecErr(specErr, specAcc);
 
   if (valid.GetNbEx() != 0) {
     prevValidErr = ComputeError(valid, validTar, &accValid);
 
-    cout << "Validation set: ";
+    std::cout << "Validation set: ";
     std::ostringstream ossVal;
-    ossVal << " SSE = " << std::setprecision(12) << prevValidErr << "    ACC = " << std::setprecision(8) << accValid << "\n\n";
+    ossVal << " SSE = " << std::setprecision(12) << prevValidErr << "    ACC = " << std::setprecision(8) << accValid << "\n"
+           << std::endl;
     temp = ossVal.str();
     std::cout << temp;
 
     Push();
   }
 
   if (acc >= AccuracyParam) {
-    cout << "\n\n*** REACHED ACCURACY THRESHOLD";
-    cout << " (" << AccuracyParam << ")\n\n";
+    std::cout << "\n\n*** REACHED ACCURACY THRESHOLD";
+    std::cout << " (" << AccuracyParam << ")\n"
+              << std::endl;
     return;
   }
 
   if (err < ErrParam) {
-    cout << "\n\n*** REACHED ERROR THRESHOLD";
-    cout << " (" << ErrParam << ")\n\n";
+    std::cout << "\n\n*** REACHED ERROR THRESHOLD";
+    std::cout << " (" << ErrParam << ")\n"
+              << std::endl;
     return;
   }
 
   if (fabs(oldErr - specErr) < DeltaErrParam) {
-    cout << "\n\n*** REACHED VARIATION CRITERION THRESHOLD";
-    cout << " (" << DeltaErrParam << ")\n\n";
+    std::cout << "\n\n*** REACHED VARIATION CRITERION THRESHOLD";
+    std::cout << " (" << DeltaErrParam << ")\n"
+              << std::endl;
     return;
   }
 
   for (int e = 1; e <= NbEpochsParam; e++) {
     TrainOneEpoch(train, trainTar, &randInt);
 
     if (e % ShowErrParam == 0) {
@@ -675,88 +720,95 @@
 
       specErr = ComputeErrorSameAct(train, trainTar, &specAcc);
       PrintSpecErr(specErr, specAcc);
 
       if (valid.GetNbEx() != 0) {
         validErr = ComputeError(valid, validTar, &accValid);
 
-        cout << "Validation set: ";
+        std::cout << "Validation set: ";
         std::ostringstream ossVal2;
-        ossVal2 << " SSE = " << std::setprecision(12) << validErr << "    ACC = " << std::setprecision(8) << accValid << "\n\n";
+        ossVal2 << " SSE = " << std::setprecision(12) << validErr << "    ACC = " << std::setprecision(8) << accValid << "\n"
+                << std::endl;
         temp = ossVal2.str();
         std::cout << temp;
 
         if (validErr < prevValidErr) {
-          cout << " (Better validation error, saving weights)";
+          std::cout << " (Better validation error, saving weights)";
           Push();
           prevValidErr = validErr;
         }
 
-        cout << "\n"
-             << endl;
+        std::cout << "\n"
+                  << std::endl;
       }
 
       if (acc >= AccuracyParam) {
-        cout << "\n\n*** REACHED ACCURACY THRESHOLD";
-        cout << " (" << AccuracyParam << ")\n\n";
+        std::cout << "\n\n*** REACHED ACCURACY THRESHOLD";
+        std::cout << " (" << AccuracyParam << ")\n"
+                  << std::endl;
         break;
       }
 
       if (err < ErrParam) {
-        cout << "\n\n*** REACHED ERROR THRESHOLD";
-        cout << " (" << ErrParam << ")\n\n";
+        std::cout << "\n\n*** REACHED ERROR THRESHOLD";
+        std::cout << " (" << ErrParam << ")\n"
+                  << std::endl;
         break;
       }
 
       if (fabs(oldErr - specErr) < DeltaErrParam) {
-        cout << "\n\n*** REACHED VARIATION CRITERION THRESHOLD";
-        cout << " (" << DeltaErrParam << ")\n\n";
+        std::cout << "\n\n*** REACHED VARIATION CRITERION THRESHOLD";
+        std::cout << " (" << DeltaErrParam << ")\n"
+                  << std::endl;
         break;
       }
 
       oldErr = specErr;
     }
   }
 
   err = ComputeError(train, trainTar, &acc);
 
-  cout << "\n\n*** SUM SQUARED ERROR ON TRAINING SET = " << err;
-  cout << "\n\n*** ACCURACY ON TRAINING SET = " << acc << "\n\n";
+  std::cout << "\n\n*** SUM SQUARED ERROR ON TRAINING SET = " << err;
+  std::cout << "\n\n*** ACCURACY ON TRAINING SET = " << acc << "\n"
+            << std::endl;
   if (valid.GetNbEx() != 0) {
     Pop(); // Get the right weights from best validation error
     validErr = ComputeError(valid, validTar, &accValid);
 
-    cout << "\n\n*** SUM SQUARED ERROR ON VALIDATION SET = " << validErr;
-    cout << "\n\n*** ACCURACY ON VALIDATION SET = " << accValid << "\n";
+    std::cout << "\n\n*** SUM SQUARED ERROR ON VALIDATION SET = " << validErr;
+    std::cout << "\n\n*** ACCURACY ON VALIDATION SET = " << accValid << "" << std::endl;
   }
 
   if (test.GetNbEx() != 0) {
     testErr = ComputeError(test, testTar, &accTest);
 
-    cout << "\n\n*** SUM SQUARED ERROR ON TESTING SET = " << testErr;
-    cout << "\n\n*** ACCURACY ON TESTING SET = " << accTest << "\n";
+    std::cout << "\n\n*** SUM SQUARED ERROR ON TESTING SET = " << testErr;
+    std::cout << "\n\n*** ACCURACY ON TESTING SET = " << accTest << "" << std::endl;
   }
   // Output accuracy stats in file
-  if (accuracyFile != nullptr) {
-    ofstream accFile(accuracyFile, ios::app);
+  if (!accuracyFile.empty()) {
+    std::ofstream accFile(accuracyFile, std::ios::app);
     if (accFile.is_open()) {
-      accFile << "Sum squared error on training set = " << err << "\n";
-      accFile << "Accuracy on training set = " << acc << "\n\n";
+      accFile << "Sum squared error on training set = " << err << "" << std::endl;
+      accFile << "Accuracy on training set = " << acc << "\n"
+              << std::endl;
       if (valid.GetNbEx() > 0) {
-        accFile << "Sum squared error on validation set = " << validErr << "\n";
-        accFile << "Accuracy on validation set = " << accValid << "\n\n";
+        accFile << "Sum squared error on validation set = " << validErr << "" << std::endl;
+        accFile << "Accuracy on validation set = " << accValid << "\n"
+                << std::endl;
       }
       if (test.GetNbEx() > 0) {
-        accFile << "Sum squared error on testing set = " << testErr << "\n";
-        accFile << "Accuracy on testing set = " << accTest << "\n\n";
+        accFile << "Sum squared error on testing set = " << testErr << "" << std::endl;
+        accFile << "Accuracy on testing set = " << accTest << "\n"
+                << std::endl;
       }
       accFile.close();
     } else {
-      string errorMsg = "Cannot open file for writing";
-      WriteError(errorMsg, accuracyFile);
+      throw CannotOpenFileError("Error : Cannot open accuracy file " + accuracyFile);
     }
   }
 
   if (!fromBT) {
     SaveWeights();
   }
 }
@@ -771,59 +823,65 @@
     float accuracyParam,
     float deltaErrParam,
     int showErrParam,
     int nbEpochsParam,
     int nbLayers,
     const std::vector<int> &nbNeurons,
     const std::string &saveFile,
-    const char printNetType[],
+    const std::string &printNetType,
     int seed)
 
 {
+
   InitRandomGen(seed);
 
-  cout << "\n\n-----------------------------------------";
-  cout << "-------------------------------------\n"
-       << endl;
-  cout << "Creating " << printNetType << " structures ...";
+  std::cout << "\n\n-----------------------------------------";
+  std::cout << "-------------------------------------\n"
+            << std::endl;
+  std::cout << "Creating " << printNetType << " structures ...";
 
   AssignParam(eta, mu, flat, errParam, accuracyParam, deltaErrParam,
               showErrParam, nbEpochsParam, nbLayers, saveFile);
 
   CreateNetStruct(nbNeurons);
 
   WriteArchParam();
   WriteParam();
 
-  cout << printNetType << " network created.\n\n";
-  cout << "\n\n-----------------------------------------";
-  cout << "-------------------------------------\n\n";
+  std::cout << printNetType << " network created.\n"
+            << std::endl;
+  std::cout << "\n\n-----------------------------------------";
+  std::cout << "-------------------------------------\n"
+            << std::endl;
 }
 
 ///////////////////////////////////////////////////////////////////
 
 BpNN::BpNN(
     const std::string &readFile,
     int nbLayers,
     const std::vector<int> &nbNeurons,
-    const char printNetType[])
-    : ReadFile(readFile), NbLayers(nbLayers), NbWeightLayers(nbLayers - 1) {
-
-  cout << "\n\n-----------------------------------------";
-  cout << "-------------------------------------\n"
-       << endl;
-  cout << "Creating " << printNetType << " structures ...";
+    const std::string &printNetType,
+    int netId)
+    : ReadFile(readFile), NetId(netId), NbLayers(nbLayers), NbWeightLayers(nbLayers - 1) {
+
+  std::cout << "\n\n-----------------------------------------";
+  std::cout << "-------------------------------------\n"
+            << std::endl;
+  std::cout << "Creating " << printNetType << " structures ...";
 
   CreateNetStruct(nbNeurons);
 
   WriteArchParam();
 
-  cout << printNetType << " network created.\n\n";
-  cout << "\n\n-----------------------------------------";
-  cout << "-------------------------------------\n\n";
+  std::cout << printNetType << " network created.\n"
+            << std::endl;
+  std::cout << "\n\n-----------------------------------------";
+  std::cout << "-------------------------------------\n"
+            << std::endl;
 }
 
 ///////////////////////////////////////////////////////////////////
 
 BpNN::BpNN(
     const std::string &readFile,
     float eta,
@@ -833,31 +891,33 @@
     float accuracyParam,
     float deltaErrParam,
     int showErrParam,
     int nbEpochsParam,
     int nbLayers,
     const std::vector<int> &nbNeurons,
     const std::string &saveFile,
-    const char printNetType[],
+    const std::string &printNetType,
     int seed)
     : ReadFile(readFile) {
   InitRandomGen(seed);
 
-  cout << "\n\n-----------------------------------------";
-  cout << "-------------------------------------\n"
-       << endl;
-  cout << "Creating " << printNetType << " structures ...";
+  std::cout << "\n\n-----------------------------------------";
+  std::cout << "-------------------------------------\n"
+            << std::endl;
+  std::cout << "Creating " << printNetType << " structures ...";
 
   AssignParam(eta, mu, flat, errParam, accuracyParam, deltaErrParam,
               showErrParam, nbEpochsParam, nbLayers, saveFile);
 
   CreateNetStruct(nbNeurons);
 
   WriteArchParam();
   WriteParam();
 
-  cout << printNetType << " network created.\n\n";
-  cout << "\n\n-----------------------------------------";
-  cout << "-------------------------------------\n\n";
+  std::cout << printNetType << " network created.\n"
+            << std::endl;
+  std::cout << "\n\n-----------------------------------------";
+  std::cout << "-------------------------------------\n"
+            << std::endl;
 }
 
 ///////////////////////////////////////////////////////////////////
```

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/bpNN.h` & `dimlpfidex-0.0.1/dimlp/cpp/src/bpNN.h`

 * *Files 7% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 #ifndef DATASETS
 #include "dataSet.h"
 #endif
 
 #include "layerD2.h"
 #include "layerDmp.h"
 
-#include "writeErr.h"
 #include <math.h>
 
 #include "layerD3.h"
 #include "layerD4.h"
 #include "layerFdp.h"
 
+#include "../../../common/cpp/src/checkFun.h"
 #include "layerRad.h"
 #include "layerSD.h"
 #include "layerSP3.h"
 #include "layerSP4.h"
 #include "layerSP5.h"
 #include <algorithm>
 #include <fstream>
@@ -43,14 +43,15 @@
 
   float ErrParam;
   float AccuracyParam;
   float DeltaErrParam;
   int ShowErrParam;
   int NbEpochsParam;
 
+  int NetId = 1;
   int NbLayers; // Including Input and Output
   int NbWeightLayers;
   std::vector<int> NbNeurons;
 
   std::vector<std::shared_ptr<Layer>> VecLayer;
 
   static int initRandomGen;
@@ -97,15 +98,15 @@
 public:
   static void resetInitRandomGen();
   int GetNbLayers() const { return NbLayers; }
   int GetNbWeightLayers() const { return NbWeightLayers; }
   int Max(const std::vector<float> &vec) const;
   std::shared_ptr<Layer> GetLayer(int indLayer) { return VecLayer[indLayer]; }
 
-  void SaveWeights(const char *str) const;
+  void SaveWeights(const std::string &str, int netId) const;
 
   virtual void ForwardOneExample1(DataSet &data, int index);
   virtual void ForwardOneExample1(float *ex);
   virtual void ForwardOneExample1();
 
   void ReadWeights() const;
 
@@ -134,15 +135,15 @@
 
   void TrainPhase(DataSet &train,
                   DataSet &trainTar,
                   DataSet &test,
                   DataSet &testTar,
                   DataSet &valid,
                   DataSet &validTar,
-                  const char *accuracyFile,
+                  const std::string &accuracyFile,
                   bool fromBT = false);
 
   //------------------------------------------------------------------------
 
   BpNN(const BpNN &) = default;            // Default copy constructor
   BpNN &operator=(const BpNN &) = default; // Default copy assignment operator
 
@@ -156,36 +157,37 @@
       float accuracyParam,
       float deltaErrParam,
       int showErrParam,
       int nbEpochsParam,
       int nbLayers,
       const std::vector<int> &nbNeurons,
       const std::string &saveFile,
-      const char printNetType[],
+      const std::string &printNetType,
       int seed = 0);
 
   BpNN(
       const std::string &readFile,
       int nbLayers,
       const std::vector<int> &nbNeurons,
-      const char printNetType[]);
+      const std::string &printNetType,
+      int netId = 1);
 
   BpNN(
       const std::string &readFile,
       float eta,
       float mu,
       float flat,
       float errParam,
       float accuracyParam,
       float deltaErrParam,
       int showErrParam,
       int nbEpochsParam,
       int nbLayers,
       const std::vector<int> &nbNeurons,
       const std::string &saveFile,
-      const char printNetType[],
+      const std::string &printNetType,
       int seed = 0);
 };
 
 //------------------------------------------------------------------------
 
 #endif
```

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/cleanRS.cpp` & `dimlpfidex-0.0.1/dimlp/cpp/src/cleanRS.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 #include "cleanRS.h"
 #include <stdlib.h>
 #include <string.h>
 
-using namespace std;
-
 ////////////////////////////////////////////////////////////////////////
 
 void CleanRuleStruct::ResetFlag() const
 
 {
   for (int r = 0; r < NbRules; r++)
     Clean[r]->Flag = 0;
@@ -216,15 +214,16 @@
   int count;
   int cl;
   int clNet;
 
   for (e = 0, count = 0; e < nbEl; e++) {
     if (vecWrong[e] == -1) // -1 -> Non Carried
     {
-      cout << "Warning ***\n\n";
+      std::cout << "Warning ***\n"
+                << std::endl;
 
       Bpnn->ForwardOneExample1(data, e);
       clNet = Bpnn->Max(std::vector<float>(Out, Out + NbOut));
       cl = DefaultClass;
 
       if (cl == clNet)
         vecWrong[e] = 0;
@@ -281,15 +280,15 @@
     *acc = (float)*correct / (float)*nbPat;
   else
     *acc = -1;
 }
 
 ////////////////////////////////////////////////////////////////////////
 
-void CleanRuleStruct::SetSevInfo(std::shared_ptr<Rule> rule, int indClean)
+void CleanRuleStruct::SetSevInfo(std::shared_ptr<DimlpRule> rule, int indClean)
 
 {
   std::shared_ptr<StringInt> carried;
 
   carried = All.Select(rule);
   carried->GoToBeg();
   Bpnn->ForwardOneExample1(All, carried->GetVal());
@@ -352,15 +351,15 @@
 
 void CleanRuleStruct::CreateStructures() {
   const int nbPrunedRules = Pruned->GetNbRules();
 
   int a;
   int r;
   int allAnt;
-  std::shared_ptr<Rule> rule;
+  std::shared_ptr<DimlpRule> rule;
 
   Clean.resize(NbRules + 1);
 
   Clean[NbRules] = std::make_shared<CleanRule>(); // for Def
   Clean[NbRules]->Classification = -1;
 
   int countEffectRules = 0;
@@ -400,17 +399,34 @@
   }
 
   SortRules(0);
 }
 
 ////////////////////////////////////////////////////////////////////////
 
-void CleanRuleStruct::WriteRules(int def, ostream &ruleFile)
+void CleanRuleStruct::WriteRules(
+    int def,
+    std::ostream &ruleFile,
+    const std::vector<double> &mus,
+    const std::vector<double> &sigmas,
+    const std::vector<int> &normalizationIndices)
 
 {
+
+  bool denormalizing = false;
+  // Check if we need to denormalize
+  if (!mus.empty() && !sigmas.empty() && !normalizationIndices.empty()) {
+    denormalizing = true;
+    if (!(mus.size() == sigmas.size() && mus.size() == normalizationIndices.size())) {
+      throw InternalError("Error during rule extraction : Means, standard deviations, and normalization indices must have the same number of elements.");
+    }
+  } else if (!mus.empty() || !sigmas.empty() || !normalizationIndices.empty()) {
+    throw InternalError("Error during rule extraction : Means, standard deviations, and normalization indices must either all be specified or none at all.");
+  }
+
   int r;
   int count;
   int nbRules;
 
   const AssocAnte *ptrAnt;
 
   if (def == 1) {
@@ -420,50 +436,73 @@
   }
 
   else {
     SetFlagToOne();
     nbRules = NbRules;
   }
 
-  ruleFile << "\n\n---------------------------------------------------------\n\n";
+  ruleFile << "\n\n---------------------------------------------------------\n"
+           << std::endl;
 
   for (r = 0, count = 0; r < NbRules; r++) {
     if (Clean[r]->Flag != 1)
       continue;
 
     count++;
     ruleFile << "Rule " << count << ": ";
 
     ptrAnt = const_cast<const AssocAnte *>(Clean[r]->SevAnt.data());
 
     for (int a = 0; a < Clean[r]->NbAnt; a++, ptrAnt++) {
+
+      // Denormalization of values in case it was previously normalized
+      float hypValue = ptrAnt->Val;
+      if (denormalizing) {
+        // Check if the attribute needs to be denormalized
+        int index = -1;
+        for (size_t i = 0; i < normalizationIndices.size(); ++i) {
+          if (normalizationIndices[i] == ptrAnt->Var) {
+            index = static_cast<int>(i);
+            break;
+          }
+        }
+        if (index != -1) {
+          hypValue = static_cast<float>(hypValue * sigmas[index] + mus[index]);
+        }
+      }
+
       ruleFile << "(" << ptrAnt->Str << " ";
       ruleFile << ptrAnt->Rel << " ";
-      ruleFile << ptrAnt->Val << ") ";
+      ruleFile << hypValue << ") ";
     }
 
     ruleFile << "Class = " << Clean[r]->StrClass;
     ruleFile << " (" << Clean[r]->NbAllCarried << ")";
 
-    ruleFile << "\n\n";
+    ruleFile << "\n"
+             << std::endl;
   }
 
   if (def == 1) {
     ruleFile << "Default Rule: "
              << "Class " << Clean[NbRules]->StrClass;
   }
   if (def == 1) {
-    ruleFile << " (" << Clean[NbRules]->NbAllCarried << ")\n\n";
+    ruleFile << " (" << Clean[NbRules]->NbAllCarried << ")\n"
+             << std::endl;
   }
 
-  ruleFile << "---------------------------------------------------------\n\n";
+  ruleFile << "---------------------------------------------------------\n"
+           << std::endl;
 
-  ruleFile << "Training set:\n\n";
+  ruleFile << "Training set:\n"
+           << std::endl;
 
-  ruleFile << "---------------------------------------------------------\n\n";
+  ruleFile << "---------------------------------------------------------\n"
+           << std::endl;
 
   for (r = 0, count = 0; r < nbRules; r++) {
     if (Clean[r]->Flag != 1)
       continue;
 
     if (r != NbRules) {
       ruleFile << "Rule ";
@@ -488,28 +527,33 @@
       ruleFile << Clean[r]->AccuracyTrain << " ";
     } else {
       ruleFile << "              ";
     }
 
     ruleFile << "      Class = " << Clean[r]->StrClass;
 
-    ruleFile << "\n";
+    ruleFile << "" << std::endl;
   }
 
-  ruleFile << "\n---------------------------------------------------------\n\n";
+  ruleFile << "\n---------------------------------------------------------\n"
+           << std::endl;
 
   ruleFile << "Accuracy of rules on training set = ";
-  ruleFile << GlobalAcc(Train, WrongTrain.data(), Train.GetNbEx()) << "\n\n";
+  ruleFile << GlobalAcc(Train, WrongTrain.data(), Train.GetNbEx()) << "\n"
+           << std::endl;
 
   if (Valid.GetNbEx() != 0) {
-    ruleFile << "---------------------------------------------------------\n\n";
+    ruleFile << "---------------------------------------------------------\n"
+             << std::endl;
 
-    ruleFile << "Validation set:\n\n";
+    ruleFile << "Validation set:\n"
+             << std::endl;
 
-    ruleFile << "---------------------------------------------------------\n\n";
+    ruleFile << "---------------------------------------------------------\n"
+             << std::endl;
 
     for (r = 0, count = 0; r < nbRules; r++) {
       if (Clean[r]->Flag != 1)
         continue;
 
       if (r != NbRules) {
         ruleFile << "Rule ";
@@ -533,36 +577,42 @@
         ruleFile.width(12);
         ruleFile << Clean[r]->AccuracyValid << " ";
       } else {
         ruleFile << "              ";
       }
 
       ruleFile << "      Class = " << Clean[r]->StrClass;
-      ruleFile << "\n";
+      ruleFile << "" << std::endl;
     }
 
-    ruleFile << "\n";
-    ruleFile << "---------------------------------------------------------\n\n";
+    ruleFile << "" << std::endl;
+    ruleFile << "---------------------------------------------------------\n"
+             << std::endl;
 
     ruleFile << "Accuracy of rules on validation set = ";
-    ruleFile << GlobalAcc(Valid, WrongValid.data(), Valid.GetNbEx()) << "\n\n";
+    ruleFile << GlobalAcc(Valid, WrongValid.data(), Valid.GetNbEx()) << "\n"
+             << std::endl;
   }
 
-  ruleFile << "---------------------------------------------------------\n\n";
+  ruleFile << "---------------------------------------------------------\n"
+           << std::endl;
 
-  ruleFile << "---------------------------------------------------------\n\n";
+  ruleFile << "---------------------------------------------------------\n"
+           << std::endl;
 
-  ruleFile << "--- Number of rules = " << CountFlaggedRules(1) << "\n";
-  ruleFile << "--- Number of antecedents = " << CountFlaggedAnt(1) << "\n";
+  ruleFile << "--- Number of rules = " << CountFlaggedRules(1) << "" << std::endl;
+  ruleFile << "--- Number of antecedents = " << CountFlaggedAnt(1) << "" << std::endl;
   ruleFile << "--- Number of antecedents per rule = ";
-  ruleFile << ComputeAvgAnt(1) << "\n";
+  ruleFile << ComputeAvgAnt(1) << "" << std::endl;
   ruleFile << "--- Number of examples per rule = ";
-  ruleFile << ComputeAvgCar(1) << "\n\n";
+  ruleFile << ComputeAvgCar(1) << "\n"
+           << std::endl;
 
-  ruleFile << "---------------------------------------------------------\n\n";
+  ruleFile << "---------------------------------------------------------\n"
+           << std::endl;
 
   if (def == 0 && Test.GetNbEx() != 0)
     UnordAccWithDef2(ruleFile);
 }
 
 ////////////////////////////////////////////////////////////////////////
 
@@ -894,15 +944,15 @@
   for (r = 0; r < NbRules + 1; r++) {
     sumCov += Clean[r]->NbCarriedTest;
     sumCor += Clean[r]->NbCorrectTest;
   }
 
   float trueAcc = (float)sumCor / (float)sumCov;
 
-  cout << "VERIFYING: " << trueAcc << "(" << sumCor << " " << sumCov << ")";
+  std::cout << "VERIFYING: " << trueAcc << "(" << sumCor << " " << sumCov << ")";
 }
 
 ////////////////////////////////////////////////////////////////////////
 
 void CleanRuleStruct::ElseRepValid()
 
 {
@@ -1090,15 +1140,15 @@
             continue;
 
           ant->Val = thres;
           expanded = Fidelity100();
 
           if (expanded) {
             if (Clean[r]->NbAllCarried > prevCarried) {
-              // cout << prevCarried << " " << Clean[r]->NbAllCarried << "\n";
+              // cout << prevCarried << " " << Clean[r]->NbAllCarried << "" << std::endl;
 
               // prevCarried = Clean[r]->NbAllCarried;
 
               break;
             } else {
               expanded = 0;
               Clean[r]->NbAllCarried = prevCarried;
@@ -1277,20 +1327,20 @@
   int r;
   int n;
 
   for (r = 0, n = 0; r < NbRules; r++)
     if (CheckAnt(r))
       n++;
 
-  cout << "\nNumber of rules = " << n;
+  std::cout << "\nNumber of rules = " << n;
 
   for (r = 0, n = 0; r < NbRules; r++)
     n += CheckAnt(r);
 
-  cout << "\nNumber of antecedents = " << n << "\n";
+  std::cout << "\nNumber of antecedents = " << n << "" << std::endl;
 }
 
 ////////////////////////////////////////////////////////////////////////
 
 void CleanRuleStruct::SimplifyElse(ThresDescr *descr)
 
 {
@@ -1446,15 +1496,15 @@
     strRev += str[i - 1 - k];
 
   return strRev;
 }
 
 ////////////////////////////////////////////////////////////////////////
 
-void CleanRuleStruct::SetAttr(vector<string> listAttr) const
+void CleanRuleStruct::SetAttr(std::vector<std::string> listAttr) const
 
 {
   int a;
   int nbAnt;
   AssocAnte *ptr;
 
   for (int r = 0; r < NbRules; r++) {
@@ -1481,15 +1531,15 @@
       ptr->Str = str;
     }
   }
 }
 
 ////////////////////////////////////////////////////////////////////////
 
-void CleanRuleStruct::SetStrClass(vector<string> listClass, int def) const
+void CleanRuleStruct::SetStrClass(std::vector<std::string> listClass, int def) const
 
 {
   for (int r = 0; r < NbRules + def; r++) {
     Clean[r]->StrClass = listClass[Clean[r]->Classification];
   }
 }
 
@@ -1523,29 +1573,31 @@
   }
 
   r++;
 
   for (i = 0, count = 0; i < r; i++)
     count += Clean[i]->NbAnt;
 
-  cout << "\nUnordered rules = " << NbRules << "\n";
-  cout << "Unordered rules - default rule = " << r << "\n";
-  cout << "True antecedents = " << count << "\n\n";
+  std::cout << "\nUnordered rules = " << NbRules << "" << std::endl;
+  std::cout << "Unordered rules - default rule = " << r << "" << std::endl;
+  std::cout << "True antecedents = " << count << "\n"
+            << std::endl;
 
   for (i = 0, count = 0; i < NbRules; i++)
     count += Clean[i]->NbAnt;
 
-  cout << "Antecedents = " << count << "\n\n";
+  std::cout << "Antecedents = " << count << "\n"
+            << std::endl;
 
   return r;
 }
 
 ////////////////////////////////////////////////////////////////////////
 
-void CleanRuleStruct::UnordAccWithDef(ostream &ruleFile)
+void CleanRuleStruct::UnordAccWithDef(std::ostream &ruleFile)
 
 {
   int r;
   int c;
   int s;
   int count;
   int z;
@@ -1569,34 +1621,34 @@
     Bpnn->ForwardOneExample1(Test, p);
     clNet = Bpnn->Max(std::vector<float>(Out, Out + NbOut));
 
     for (r = 0, c = 0, z = 0; r < nbRules; r++) {
       if (IsExampleCarried(Test, p, Clean[r]) == 1) {
         z = 1;
 
-        cout << p + 1 << ": "
-             << "-- R" << r + 1 << " " << 1 + Clean[r]->Classification << " " << clNet + 1 << " " << ClassPatNetTest[p] + 1 << "\n";
+        std::cout << p + 1 << ": "
+                  << "-- R" << r + 1 << " " << 1 + Clean[r]->Classification << " " << clNet + 1 << " " << ClassPatNetTest[p] + 1 << "" << std::endl;
 
         Clean[r]->NbCarriedTest += 1;
 
         vectRulCar[c] = r;
         c++;
 
         if (Clean[r]->Classification == ClassPatNetTest[p])
           Clean[r]->NbCorrectTest += 1;
         else
           Clean[r]->NbWrongTest += 1;
       }
     }
 
     if (z == 0)
-      cout << p + 1 << ": "
-           << "-- Default"
-           << " " << 1 + Clean[nbRules]->Classification << " " << clNet + 1 << " " << ClassPatNetTest[p] + 1 << "\n";
-    cout << "\n";
+      std::cout << p + 1 << ": "
+                << "-- Default"
+                << " " << 1 + Clean[nbRules]->Classification << " " << clNet + 1 << " " << ClassPatNetTest[p] + 1 << "" << std::endl;
+    std::cout << "" << std::endl;
 
     if (c == 0) /* Default */
     {
       Clean[nbRules]->NbCarriedTest += 1;
 
       if (Clean[nbRules]->Classification == ClassPatNetTest[p]) {
         Clean[nbRules]->NbCorrectTest += 1;
@@ -1666,24 +1718,28 @@
             break;
           }
         }
       }
     }
   }
 
-  cout << "--- Accuracy on testing set = " << (float)globalAcc * 100.0 / (float)nbEx << "\n";
-  cout << "--- Fidelity = " << (float)fidelity * 100.0 / (float)nbEx << "\n";
-  cout << "--- Acc on Fid = " << (float)globalWithout * 100.0 / (float)fidelity << "\n";
-  cout << "--- Contradictions = " << (float)contr * 100.0 / (float)nbEx << "\n\n";
+  std::cout << "--- Accuracy on testing set = " << (float)globalAcc * 100.0 / (float)nbEx << "" << std::endl;
+  std::cout << "--- Fidelity = " << (float)fidelity * 100.0 / (float)nbEx << "" << std::endl;
+  std::cout << "--- Acc on Fid = " << (float)globalWithout * 100.0 / (float)fidelity << "" << std::endl;
+  std::cout << "--- Contradictions = " << (float)contr * 100.0 / (float)nbEx << "\n"
+            << std::endl;
 
-  ruleFile << "---------------------------------------------------------\n\n";
+  ruleFile << "---------------------------------------------------------\n"
+           << std::endl;
 
-  ruleFile << "Testing set:\n\n";
+  ruleFile << "Testing set:\n"
+           << std::endl;
 
-  ruleFile << "---------------------------------------------------------\n\n";
+  ruleFile << "---------------------------------------------------------\n"
+           << std::endl;
 
   for (r = 0, count = 0; r < nbRules; r++) {
     if (r != NbRules) {
       ruleFile << "Rule ";
       ruleFile.width(4);
       count++;
       ruleFile << count << ": ";
@@ -1704,23 +1760,24 @@
       ruleFile.width(12);
       ruleFile << Clean[r]->AccuracyTest << " ";
     } else
       ruleFile << "              ";
 
     ruleFile << "      Class = " << Clean[r]->StrClass;
 
-    ruleFile << "\n";
+    ruleFile << "" << std::endl;
   }
 
-  ruleFile << "\n---------------------------------------------------------\n\n";
+  ruleFile << "\n---------------------------------------------------------\n"
+           << std::endl;
 }
 
 ////////////////////////////////////////////////////////////////////////
 
-void CleanRuleStruct::UnordAccWithDef2(ostream &ruleFile)
+void CleanRuleStruct::UnordAccWithDef2(std::ostream &ruleFile)
 
 {
   int r;
   int c;
   int s;
   int count;
   int z;
@@ -1737,53 +1794,55 @@
   int nbRules = NbRules;
   int countDef = 0;
   int noFid = 0;
   int noFidBad = 0;
 
   ResetSomeFields();
 
-  cout << "CLASSIFICATION ON THE TESTING SET\n\n";
-  cout << "(Case: Activated Rule -- Rule Class, Net Class, True Class):\n\n";
+  std::cout << "CLASSIFICATION ON THE TESTING SET\n"
+            << std::endl;
+  std::cout << "(Case: Activated Rule -- Rule Class, Net Class, True Class):\n"
+            << std::endl;
 
   for (int p = 0; p < nbEx; p++) {
     std::vector<int> vectRulCar(nbRules);
 
     Bpnn->ForwardOneExample1(Test, p);
     clNet = Bpnn->Max(std::vector<float>(Out, Out + NbOut));
 
     for (r = 0, c = 0, z = 0; r < nbRules; r++) {
       if (IsExampleCarried(Test, p, Clean[r]) == 1) {
         z = 1;
 
-        cout << p + 1 << ": R" << r + 1 << " -- " << 1 + Clean[r]->Classification << " " << clNet + 1 << " " << ClassPatNetTest[p] + 1;
+        std::cout << p + 1 << ": R" << r + 1 << " -- " << 1 + Clean[r]->Classification << " " << clNet + 1 << " " << ClassPatNetTest[p] + 1;
         if (Clean[r]->Classification != clNet)
-          cout << " ***";
+          std::cout << " ***";
         if ((Clean[r]->Classification == clNet) && (clNet != ClassPatNetTest[p]))
-          cout << " ---";
-        cout << "\n";
+          std::cout << " ---";
+        std::cout << "" << std::endl;
         Clean[r]->NbCarriedTest += 1;
 
         vectRulCar[c] = r;
         c++;
 
         if (Clean[r]->Classification == ClassPatNetTest[p])
           Clean[r]->NbCorrectTest += 1;
         else
           Clean[r]->NbWrongTest += 1;
       }
     }
 
     if (z == 0) {
-      cout << p + 1 << ": "
-           << " -- Net Class: " << clNet + 1 << " True Class: " << ClassPatNetTest[p] + 1;
+      std::cout << p + 1 << ": "
+                << " -- Net Class: " << clNet + 1 << " True Class: " << ClassPatNetTest[p] + 1;
       if (clNet != ClassPatNetTest[p])
-        cout << " ---";
-      cout << "\n";
+        std::cout << " ---";
+      std::cout << "" << std::endl;
     }
-    cout << "\n";
+    std::cout << "" << std::endl;
 
     if (z == 0) /* Default */
     {
       countDef++;
       fidelity++;
 
       if (clNet == ClassPatNetTest[p]) {
@@ -1862,24 +1921,29 @@
           else
             noFidBad++;
         }
       }
     }
   }
 
-  ruleFile << "--- Accuracy of rules on testing set = " << (float)globalAcc / (float)nbEx << "\n";
-  ruleFile << "--- Fidelity on testing set (" << fidelity << "/" << nbEx << ") = " << (float)fidelity / (float)nbEx << "\n";
-  ruleFile << "--- Accuracy when rules and network agree (" << globalWithout << "/" << fidelity << ") = " << (float)globalWithout / (float)fidelity << "\n\n";
-  ruleFile << "--- Default rule activations rate (network classification) = " << (float)countDef / (float)nbEx << "\n\n";
+  ruleFile << "--- Accuracy of rules on testing set = " << (float)globalAcc / (float)nbEx << "" << std::endl;
+  ruleFile << "--- Fidelity on testing set (" << fidelity << "/" << nbEx << ") = " << (float)fidelity / (float)nbEx << "" << std::endl;
+  ruleFile << "--- Accuracy when rules and network agree (" << globalWithout << "/" << fidelity << ") = " << (float)globalWithout / (float)fidelity << "\n"
+           << std::endl;
+  ruleFile << "--- Default rule activations rate (network classification) = " << (float)countDef / (float)nbEx << "\n"
+           << std::endl;
 
-  ruleFile << "---------------------------------------------------------\n\n";
+  ruleFile << "---------------------------------------------------------\n"
+           << std::endl;
 
-  ruleFile << "Testing set:\n\n";
+  ruleFile << "Testing set:\n"
+           << std::endl;
 
-  ruleFile << "---------------------------------------------------------\n\n";
+  ruleFile << "---------------------------------------------------------\n"
+           << std::endl;
 
   for (r = 0, count = 0; r < nbRules; r++) {
     if (r != NbRules) {
       ruleFile << "Rule ";
       ruleFile.width(4);
       count++;
       ruleFile << count << ": ";
@@ -1901,14 +1965,15 @@
       ruleFile << Clean[r]->AccuracyTest << " ";
     } else {
       ruleFile << "              ";
     }
 
     ruleFile << "      Class = " << Clean[r]->StrClass;
 
-    ruleFile << "\n";
+    ruleFile << "" << std::endl;
   }
 
-  ruleFile << "\n---------------------------------------------------------\n\n";
+  ruleFile << "\n---------------------------------------------------------\n"
+           << std::endl;
 }
 
 ////////////////////////////////////////////////////////////////////////
```

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/cleanRS.h` & `dimlpfidex-0.0.1/dimlp/cpp/src/cleanRS.h`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
       DataSet &data,
       DataSet &dataClass,
       int *nbPat,
       int *correct,
       int *wrong,
       float *acc) const;
 
-  void SetSevInfo(std::shared_ptr<Rule> rule, int indClean);
+  void SetSevInfo(std::shared_ptr<DimlpRule> rule, int indClean);
   void CreateWrongVect();
   void CreateStructures();
 
   void ResetSomeFields() const;
   int IsExampleCarried(DataSet &data, int index, std::shared_ptr<CleanRule> rule) const;
   int Fidelity100();
   int Fidelity100Def();
@@ -126,15 +126,20 @@
   int DefDef() const;
   void UnordAccWithDef(std::ostream &ruleFile);
   void UnordAccWithDef2(std::ostream &ruleFile);
 
   // ------------------------------------------------------------------------
 
 public:
-  void WriteRules(int def, std::ostream &ruleFile);
+  void WriteRules(
+      int def,
+      std::ostream &ruleFile,
+      const std::vector<double> &mus = std::vector<double>(),
+      const std::vector<double> &sigmas = std::vector<double>(),
+      const std::vector<int> &normalizationIndices = std::vector<int>());
   void ElseRepresentation();
   void SimplifyElse(ThresDescr *descr);
 
   void Del() { NbRules = 0; };
 
   void SetAttr(std::vector<std::string> listAttr) const;
   void SetAttr();
```

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/dimlp.cpp` & `dimlpfidex-0.0.1/dimlp/cpp/src/dimlp.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,80 @@
 #include "dimlp.h"
-using namespace std;
 
 ////////////////////////////////////////////////////////////////////////
-const char netType[] = "Discretized Interpretable Multi-Layer Perceptron";
+const std::string &netType = "Discretized Interpretable Multi-Layer Perceptron";
 
 Dimlp::Dimlp(
     float eta,
     float mu,
     float flat,
     float errParam,
     float accuracyParam,
     float deltaErrParam,
     int discrLevels,
     int showErrParam,
     int nbEpochsParam,
     int nbLayers,
     const std::vector<int> &nbNeurons,
-    const char weightFile[],
+    const std::string &weightFile,
     int seed) :
 
                 BpNN(eta, mu, flat, errParam, accuracyParam, deltaErrParam,
                      showErrParam, nbEpochsParam, nbLayers, nbNeurons, weightFile,
                      netType, seed)
 
 {
-  cout << "Number of quantized levels = " << discrLevels << "\n"
-       << endl;
+  std::cout << "Number of quantized levels = " << discrLevels << "\n"
+            << std::endl;
 
   DefineDimlp(discrLevels);
 }
 
 ////////////////////////////////////////////////////////////////////////
 
 Dimlp::Dimlp(
-    const char readFile[],
+    const std::string &readFile,
     int nbLayers,
     const std::vector<int> &nbNeurons,
-    int discrLevels) :
+    int discrLevels,
+    int netId) :
 
-                       BpNN(readFile, nbLayers, nbNeurons,
-                            netType)
+                 BpNN(readFile, nbLayers, nbNeurons,
+                      netType, netId)
 
 {
-  cout << "Number of quantized levels = " << discrLevels << "\n"
-       << endl;
+  std::cout << "Number of quantized levels = " << discrLevels << "\n"
+            << std::endl;
 
   DefineDimlp(discrLevels);
   ReadWeights();
 }
 
 ////////////////////////////////////////////////////////////////////////
 
 Dimlp::Dimlp(
-    const char readFile[],
+    const std::string &readFile,
     float eta,
     float mu,
     float flat,
     float errParam,
     float accuracyParam,
     float deltaErrParam,
     int discrLevels,
     int showErrParam,
     int nbEpochsParam,
     int nbLayers,
     const std::vector<int> &nbNeurons,
-    const char weightFile[],
+    const std::string &weightFile,
     int seed) :
 
                 BpNN(readFile, eta, mu, flat, errParam, accuracyParam, deltaErrParam,
                      showErrParam, nbEpochsParam, nbLayers, nbNeurons, weightFile,
                      netType, seed) {
-  cout << "Number of quantized levels = " << discrLevels << "\n"
-       << endl;
+  std::cout << "Number of quantized levels = " << discrLevels << "\n"
+            << std::endl;
 
   DefineDimlp(discrLevels);
   ReadWeights();
 }
 
 ////////////////////////////////////////////////////////////////////////
```

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/dimlp.h` & `dimlpfidex-0.0.1/dimlp/cpp/src/dimlp.h`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
   void Train(DataSet &train,
              DataSet &trainTar,
              DataSet &test,
              DataSet &testTar,
              DataSet &valid,
              DataSet &validTar,
-             const char *accuracyFile,
+             const std::string &accuracyFile,
              bool fromBT = false)
 
   { TrainPhase(train, trainTar, test, testTar, valid, validTar, accuracyFile, fromBT); }
 
   //---------------------------------------------------------------------
 
   ~Dimlp() override = default; // Virtual destructor
@@ -36,30 +36,30 @@
       float accuracyParam,
       float deltaErrParam,
       int discrLevels,
       int showErrParam,
       int nbEpochsParam,
       int nbLayers,
       const std::vector<int> &nbNeurons,
-      const char weightFile[],
+      const std::string &weightFile,
       int seed = 0);
 
-  Dimlp(const char readFile[], int nbLayers, const std::vector<int> &nbNeurons, int discrLevels);
+  Dimlp(const std::string &readFile, int nbLayers, const std::vector<int> &nbNeurons, int discrLevels, int netId = 1);
 
   Dimlp(
-      const char readFile[],
+      const std::string &readFile,
       float eta,
       float mu,
       float flat,
       float errParam,
       float accuracyParam,
       float deltaErrParam,
       int discrLevels,
       int showErrParam,
       int nbEpochsParam,
       int nbLayers,
       const std::vector<int> &nbNeurons,
-      const char weightFile[],
+      const std::string &weightFile,
       int seed = 0);
 };
 
 #endif
```

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/layer.cpp` & `dimlpfidex-0.0.1/dimlp/cpp/src/layer.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #include "layer.h"
 
-using namespace std;
 ///////////////////////////////////////////////////////////////////
 
 void Layer::AssignParam(
     float eta,
     float mu,
     float flat,
     int nbDown,
@@ -184,50 +183,49 @@
     biasDelta = (EtaSpread * (*deltaUp) * norm);
     *bias += biasDelta;
   }
 }
 
 ///////////////////////////////////////////////////////////////////
 
-void Layer::ReadWeights(istream &inFile)
+void Layer::ReadWeights(std::istream &inFile)
 
 {
   int w;
   float *ptrW;
 
   float *ptrOldW = OldBiasWeights.data();
 
   for (w = 0, ptrW = BiasWeights.data(); w < NbUp; w++, ptrW++, ptrOldW++) {
     inFile >> *ptrW;
     *ptrOldW = *ptrW;
   }
 
   ptrOldW = OldWeights.data();
-
   for (w = 0, ptrW = Weights.data(); w < NbWeights; w++, ptrW++, ptrOldW++) {
     inFile >> *ptrW;
     *ptrOldW = *ptrW;
   }
 }
 
 ///////////////////////////////////////////////////////////////////
 
-void Layer::WriteWeights(ostream &outFile)
+void Layer::WriteWeights(std::ostream &outFile)
 
 {
   int w;
   const float *ptrW;
 
   for (w = 0, ptrW = BiasWeights.data(); w < NbUp; w++, ptrW++)
     outFile << *ptrW << " ";
-  outFile << "\n";
+  outFile << "" << std::endl;
 
   for (w = 0, ptrW = Weights.data(); w < NbWeights; w++, ptrW++)
     outFile << *ptrW << " ";
-  outFile << "\n";
+  outFile << "" << std::endl;
 }
 
 ///////////////////////////////////////////////////////////////////
 
 void Layer::PushWeights()
 
 {
```

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/layer.h` & `dimlpfidex-0.0.1/dimlp/cpp/src/layer.h`

 * *Files identical despite different names*

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/layerD2.h` & `dimlpfidex-0.0.1/dimlp/cpp/src/layerD2.h`

 * *Files identical despite different names*

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/layerD3.h` & `dimlpfidex-0.0.1/dimlp/cpp/src/layerD3.h`

 * *Files identical despite different names*

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/layerD4.h` & `dimlpfidex-0.0.1/dimlp/cpp/src/layerD4.h`

 * *Files identical despite different names*

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/layerDmp.h` & `dimlpfidex-0.0.1/dimlp/cpp/src/layerDmp.h`

 * *Files identical despite different names*

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/layerFdp.h` & `dimlpfidex-0.0.1/dimlp/cpp/src/layerFdp.h`

 * *Files identical despite different names*

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/layerRad.h` & `dimlpfidex-0.0.1/dimlp/cpp/src/layerRad.h`

 * *Files identical despite different names*

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/layerSD.h` & `dimlpfidex-0.0.1/dimlp/cpp/src/layerSD.h`

 * *Files identical despite different names*

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/layerSP3.h` & `dimlpfidex-0.0.1/dimlp/cpp/src/layerSP3.h`

 * *Files identical despite different names*

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/layerSP4.h` & `dimlpfidex-0.0.1/dimlp/cpp/src/layerSP4.h`

 * *Files identical despite different names*

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/layerSP5.h` & `dimlpfidex-0.0.1/dimlp/cpp/src/layerSP5.h`

 * *Files identical despite different names*

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/misc.cpp` & `dimlpfidex-0.0.1/dimlp/cpp/src/misc.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include "stringI.h"
+#include "../../../common/cpp/src/stringI.h"
 #include <iostream>
 #include <vector>
 
 ////////////////////////////////////////////////////////////////////////
 
 int Compare(const void *x, const void *y)
```

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/oneVarTD.cpp` & `dimlpfidex-0.0.1/dimlp/cpp/src/oneVarTD.cpp`

 * *Files identical despite different names*

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/oneVarTD.h` & `dimlpfidex-0.0.1/dimlp/cpp/src/oneVarTD.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #ifndef ONEVARTD_H
 #define ONEVARTD_H
 
 #ifndef STRINGINT
-#include "stringI.h"
+#include "../../../common/cpp/src/stringI.h"
 #endif
 #include <memory>
 
 ///////////////////////////////////////////////////////////////////
 
 class OneVarThresDescr {
   struct Elem {
```

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/randFun.cpp` & `dimlpfidex-0.0.1/dimlp/cpp/src/randFun.cpp`

 * *Files 23% similar despite different names*

```diff
@@ -5,26 +5,23 @@
 #include "randFun.h"
 
 ///////////////////////////////////////////////////////////////////
 
 void IntRandomFunction::StartOnlyOnece(int seed) const
 
 {
-#if defined(__unix__) || defined(__APPLE__)
+
   if (seed == 0) {
-    srandom(getpid());
-  } else {
-    srandom(seed);
+    seed = static_cast<int>(std::chrono::system_clock::now().time_since_epoch().count());
   }
+
+#if defined(__unix__) || defined(__APPLE__)
+  srandom(seed);
 #elif defined(_WIN32)
-  if (seed == 0) {
-    srand(getpid());
-  } else {
-    srand(seed);
-  }
+  srand(seed);
 #endif
 }
 
 ///////////////////////////////////////////////////////////////////
 
 IntRandomFunction::IntRandomFunction(int seed)
 
@@ -52,26 +49,21 @@
 }
 
 ///////////////////////////////////////////////////////////////////
 
 void FloatRandomFunction::StartOnlyOnece(int seed) const
 
 {
-#if defined(__unix__) || defined(__APPLE__)
   if (seed == 0) {
-    srand48(getpid());
-  } else {
-    srand48(seed);
+    seed = static_cast<int>(std::chrono::system_clock::now().time_since_epoch().count());
   }
+#if defined(__unix__) || defined(__APPLE__)
+  srand48(seed);
 #elif defined(_WIN32)
-  if (seed == 0) {
-    srand(getpid());
-  } else {
-    srand(seed);
-  }
+  srand(seed);
 #endif
 }
 
 ///////////////////////////////////////////////////////////////////
 
 FloatRandomFunction::FloatRandomFunction(int seed)
```

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/randFun.h` & `dimlpfidex-0.0.1/dimlp/cpp/src/randFun.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #ifndef RANDFUN_H
 #define RANDFUN_H
+#include <chrono>
 
 ///////////////////////////////////////////////////////////////////
 
 class IntRandomFunction {
 
   int LowBound;
   int HiBound;
```

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/realHyp.cpp` & `dimlpfidex-0.0.1/dimlp/cpp/src/realHyp.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 #include "realHyp.h"
 #include "misc.h"
 #define STRINGINT 1
 
 #define FROMREAL 1
 #include "cleanRS.h"
 
-using namespace std;
-
 ////////////////////////////////////////////////////////////////////////
 
 int RealHyp::MaxOnPos(const std::vector<int> &vec) const
 
 {
   int max = vec[0];
 
@@ -48,15 +46,16 @@
   int nbPat = data.GetNbEx();
   int *hyp;
   int h;
   int v;
   int indVirt;
   const float *pat;
 
-  cout << "\n\n*** EXCLUDING UNRELEVANT HYPER-PLANES ...\n\n";
+  std::cout << "\n\n*** EXCLUDING UNRELEVANT HYPER-PLANES ...\n"
+            << std::endl;
 
   for (v = 0; v < NbIn; v++) {
     ConfBefFirstHyp[v] = 0;
 
     hyp = ConfirmedVirt[v].data();
 
     for (h = 0; h < NbHyp; h++, hyp++)
@@ -70,49 +69,52 @@
       indVirt = Virt->KnotInd(v, *pat);
 
       if ((indVirt >= 0) && (indVirt <= NbHyp - 1))
         *(ConfirmedVirt[v].data() + indVirt) = 1;
       else if (indVirt == -1)
         ConfBefFirstHyp[v] = 1;
       else
-        cout << "*** ELSE WARNING !\n\n";
+        std::cout << "*** ELSE WARNING !\n"
+                  << std::endl;
     }
   }
 
   int count = 0;
 
   for (v = 0; v < NbIn; v++) {
     hyp = ConfirmedVirt[v].data();
 
     for (h = 0; h < NbHyp; h++, hyp++)
       if (*hyp == 1)
         count++;
   }
 
-  cout << "*** RELEVANT VIRTUAL HYPER-PLANES = " << count << "\n\n";
+  std::cout << "*** RELEVANT VIRTUAL HYPER-PLANES = " << count << "\n"
+            << std::endl;
 }
 
 ////////////////////////////////////////////////////////////////////////
 
 void RealHyp::SetConfirmedVirt2()
 
 {
   const int nbRules = SavedRules->GetNbRules();
-  std::shared_ptr<Rule> rule;
+  std::shared_ptr<DimlpRule> rule;
   int *hyp;
   int a;
   int h;
   int r;
   int v;
   int var;
   int indVirt;
   int nbAnt;
   float val;
 
-  cout << "\n\n*** EXCLUDING UNRELEVANT HYPER-PLANES FROM RULES ...\n\n";
+  std::cout << "\n\n*** EXCLUDING UNRELEVANT HYPER-PLANES FROM RULES ...\n"
+            << std::endl;
 
   for (v = 0; v < NbIn; v++) {
     hyp = ConfirmedVirt[v].data();
 
     for (h = 0; h < NbHyp; h++, hyp++)
       *hyp = 0;
   }
@@ -129,15 +131,15 @@
       if (rule->IsAntDeleted() == 0) {
         var = rule->GetVar();
         val = rule->GetVal();
 
         indVirt = Virt->GetInd(var, val);
 
         if (indVirt == -1) {
-          cout << "Warning ... " << var << " " << val << "\n";
+          std::cout << "Warning ... " << var << " " << val << "" << std::endl;
         }
 
         else
           *(ConfirmedVirt[var].data() + indVirt) = 1;
       }
     }
   }
@@ -148,15 +150,16 @@
     hyp = ConfirmedVirt[v].data();
 
     for (h = 0; h < NbHyp; h++, hyp++)
       if (*hyp == 1)
         count++;
   }
 
-  cout << "*** RELEVANT VIRTUAL HYPER-PLANES = " << count << "\n\n";
+  std::cout << "*** RELEVANT VIRTUAL HYPER-PLANES = " << count << "\n"
+            << std::endl;
 }
 
 ////////////////////////////////////////////////////////////////////////
 
 void RealHyp::Gr1(
     int var,
     int indPat,
@@ -336,36 +339,37 @@
 void RealHyp::SetRealHyp(DataSet &data)
 
 {
   int p;
   int modulo;
   const int nbEx = data.GetNbEx();
 
-  cout << "*** ESTIMATING RELEVANCE OF DISCRIMINANT HYPER-PLANES ";
-  cout << "WITH AVAILABLE EXAMPLES ...\n"
-       << endl;
+  std::cout << "*** ESTIMATING RELEVANCE OF DISCRIMINANT HYPER-PLANES ";
+  std::cout << "WITH AVAILABLE EXAMPLES ...\n"
+            << std::endl;
 
   if (nbEx >= 10)
     modulo = nbEx / 10;
   else
     modulo = 1;
 
   for (p = 0; p < nbEx; p++) {
     if (p % modulo == 0)
-      cout << p << endl;
+      std::cout << p << std::endl;
 
     OneExRealHyp(data, p);
   }
 
-  cout << p << "\n\n\n";
+  std::cout << p << "\n\n"
+            << std::endl;
 }
 
 ////////////////////////////////////////////////////////////////////////
 
-void RealHyp::SetCountPatDiscr(std::shared_ptr<StringInt> listPat, std::shared_ptr<Rule> r) const
+void RealHyp::SetCountPatDiscr(std::shared_ptr<StringInt> listPat, std::shared_ptr<DimlpRule> r) const
 
 {
   int a;
   int j;
   int t;
   int nbThres;
   int nbPatThres;
@@ -453,37 +457,33 @@
   auto ant = std::make_shared<Ante>(var, val, '?');
 
   return ant;
 }
 
 ////////////////////////////////////////////////////////////////////////
 
-void RealHyp::DeepSearch(DataSet &data, std::shared_ptr<Rule> path, std::shared_ptr<StringInt> subSet)
+void RealHyp::DeepSearch(DataSet &data, std::shared_ptr<DimlpRule> path, std::shared_ptr<StringInt> subSet)
 
 {
-  Rule newLeftPath;
-  Rule newRightPath;
-
+  DimlpRule newLeftPath;
+  DimlpRule newRightPath;
   std::shared_ptr<StringInt> newListPat = data.Select(path, subSet);
-
   if (newListPat->GetNbEl() == 0) {
     newListPat->Del();
     path->Del();
 
     return;
   }
-
   if (AreSameClass(newListPat, ClassPatNet) == 1) {
     newListPat->Del();
     SaveRule(path);
     path->Del();
 
     return;
   }
-
   SetCountPatDiscr(newListPat, path);
 
   std::shared_ptr<Ante> ant = FindMostDiscrAnt(0);
   int var = ant->GetVarAnte();
   float val = ant->GetValAnte();
 
   if (var < 0) {
@@ -497,16 +497,16 @@
 
   (newLeftPath.Copy(path))->Insert(var, val, '<');
   (newRightPath.Copy(path))->Insert(var, val, '>');
 
   path->Del();
   ant->DelAnte();
 
-  DeepSearch(data, std::make_shared<Rule>(newLeftPath), newListPat);
-  DeepSearch(data, std::make_shared<Rule>(newRightPath), newListPat);
+  DeepSearch(data, std::make_shared<DimlpRule>(newLeftPath), newListPat);
+  DeepSearch(data, std::make_shared<DimlpRule>(newRightPath), newListPat);
 
   newListPat->Del();
 }
 
 ////////////////////////////////////////////////////////////////////////
 
 int RealHyp::ComputeCorrect(
@@ -548,28 +548,28 @@
   max = MaxOnPos(vectMax);
 
   return max;
 }
 
 ////////////////////////////////////////////////////////////////////////
 
-void RealHyp::SetCountPatDiscr2(DataSet &data, std::shared_ptr<Rule> r)
+void RealHyp::SetCountPatDiscr2(DataSet &data, std::shared_ptr<DimlpRule> r)
 
 {
   int a;
   int t;
   int nbThres;
   static int nbCorrect;
   float thres;
 
   OneVarThresDescr *varDescr;
   std::shared_ptr<StringInt> newListPatLeft;
   std::shared_ptr<StringInt> newListPatRight;
-  auto newLeftPath = std::make_shared<Rule>();
-  auto newRightPath = std::make_shared<Rule>();
+  auto newLeftPath = std::make_shared<DimlpRule>();
+  auto newRightPath = std::make_shared<DimlpRule>();
 
   Descr->ResetAllCountPatDiscr();
   int nbRuleAnt = r->GetNbAnt();
 
   for (int v = 0; v < NbIn; v++) {
     varDescr = Descr->GetDescr(v);
     nbThres = varDescr->GetNbThres();
@@ -602,19 +602,19 @@
       newListPatRight->Del();
     }
   }
 }
 
 ////////////////////////////////////////////////////////////////////////
 
-void RealHyp::DeepSearch2(DataSet &data, std::shared_ptr<Rule> path)
+void RealHyp::DeepSearch2(DataSet &data, std::shared_ptr<DimlpRule> path)
 
 {
-  Rule newLeftPath;
-  Rule newRightPath;
+  DimlpRule newLeftPath;
+  DimlpRule newRightPath;
 
   std::shared_ptr<StringInt> newListPat = data.Select(path);
 
   if (newListPat->GetNbEl() == 0) {
     newListPat->Del();
     path->Del();
     return;
@@ -645,163 +645,178 @@
   (newLeftPath.Copy(path))->Insert(var, val, '<');
   (newRightPath.Copy(path))->Insert(var, val, '>');
 
   path->Del();
   ant->DelAnte();
   newListPat->Del();
 
-  DeepSearch2(data, std::make_shared<Rule>(newLeftPath));
-  DeepSearch2(data, std::make_shared<Rule>(newRightPath));
+  DeepSearch2(data, std::make_shared<DimlpRule>(newLeftPath));
+  DeepSearch2(data, std::make_shared<DimlpRule>(newRightPath));
 }
 
 ////////////////////////////////////////////////////////////////////////
 
 void RealHyp::RuleExtraction(
     DataSet &data,
     const DataSet &train,
     const DataSet &trainClass,
     const DataSet &valid,
     const DataSet &validClass,
     const DataSet &test,
     const DataSet &testClass,
     const AttrName &attr,
-    ostream &ruleFile)
+    std::ostream &ruleFile,
+    const std::vector<double> &mus,
+    const std::vector<double> &sigmas,
+    const std::vector<int> &normalizationIndices)
 
 {
-  Rule empty;
+  DimlpRule empty;
   std::shared_ptr<StringInt> listAll;
   int nbAnt1;
   int nbAnt2;
 
   Aborted = 0;
 
   SavedRules = std::make_shared<RuleProcessing>(NbIn, NbHyp, data, ClassPatNet, Descr);
+  std::cout << "*** BUILDING DECISION TREE ...\n"
+            << std::endl;
 
-  cout << "*** BUILDING DECISION TREE ...\n"
-       << endl;
-
-  listAll = data.Select(std::make_shared<Rule>(empty));
-  DeepSearch(data, std::make_shared<Rule>(empty), listAll);
+  listAll = data.Select(std::make_shared<DimlpRule>(empty));
+  DeepSearch(data, std::make_shared<DimlpRule>(empty), listAll);
   listAll->Del();
   if (Aborted) {
-    cout << "*** TREE ABORTED !\n\n";
-    cout << "*** TRYING AN ALTERNATIVE ALGORITHM \n"
-         << endl;
+    std::cout << "*** TREE ABORTED !\n"
+              << std::endl;
+    std::cout << "*** TRYING AN ALTERNATIVE ALGORITHM \n"
+              << std::endl;
 
     SavedRules->Del();
     Descr->Del();
 
     return;
   }
 
   SavedRules->Clean();
-
+  std::cout << "4" << std::endl;
   if (SavedRules->CountAnt() == 0) {
-    cout << "*** NO RULES !\n\n";
-    cout << "--- Number of rules = 0\n";
-    cout << "--- Number of antecedents = 0\n";
-    cout << "--- Number of antecedents per rule = 0\n";
-    cout << "--- Number of examples per rule = 0\n";
-
-    cout << "*** NO RULES !\n\n";
-
-    cout << "--- Number of rules = 0\n";
-    cout << "--- Number of antecedents = 0\n";
-    cout << "--- Number of antecedents per rule = 0\n";
-    cout << "--- Number of examples per rule = 0" << endl;
+    std::cout << "*** NO RULES !\n"
+              << std::endl;
+    std::cout << "--- Number of rules = 0" << std::endl;
+    std::cout << "--- Number of antecedents = 0" << std::endl;
+    std::cout << "--- Number of antecedents per rule = 0" << std::endl;
+    std::cout << "--- Number of examples per rule = 0" << std::endl;
+
+    std::cout << "*** NO RULES !\n"
+              << std::endl;
+
+    std::cout << "--- Number of rules = 0" << std::endl;
+    std::cout << "--- Number of antecedents = 0" << std::endl;
+    std::cout << "--- Number of antecedents per rule = 0" << std::endl;
+    std::cout << "--- Number of examples per rule = 0" << std::endl;
 
     SavedRules->Del();
 
     Descr->Del();
 
     return;
   }
-  cout << "\n\n*** PRUNING ANTECEDENTS AND PRUNING RULES ...\n"
-       << endl;
+  std::cout << "\n\n*** PRUNING ANTECEDENTS AND PRUNING RULES ...\n"
+            << std::endl;
   SavedRules->MixPrune();
 
-  cout << "\n\n*** EXPANDING RULES ...\n"
-       << endl;
+  std::cout << "\n\n*** EXPANDING RULES ...\n"
+            << std::endl;
   SavedRules->EnlargeAndPrune();
 
   nbAnt1 = SavedRules->CountAnt();
 
-  cout << "\n\n*** RETRYING RULE EXTRACTION ...\n"
-       << endl;
+  std::cout << "\n\n*** RETRYING RULE EXTRACTION ...\n"
+            << std::endl;
 
   CleanRuleStruct clean(data, train, trainClass,
                         valid, validClass, test, testClass,
                         SavedRules, Bpnn, Out, NbOut);
 
   Descr->Del();
   SetConfirmedVirt2();
   SetRealHyp(data);
 
   SavedRules->Del();
-  cout << "*** BUILDING DECISION TREE ...\n"
-       << endl;
+  std::cout << "*** BUILDING DECISION TREE ...\n"
+            << std::endl;
 
-  listAll = data.Select(std::make_shared<Rule>(empty));
-  DeepSearch(data, std::make_shared<Rule>(empty), listAll);
+  listAll = data.Select(std::make_shared<DimlpRule>(empty));
+  DeepSearch(data, std::make_shared<DimlpRule>(empty), listAll);
   listAll->Del();
 
   if (Aborted) {
-    cout << "*** TREE ABORTED !\n\n";
+    std::cout << "*** TREE ABORTED !\n"
+              << std::endl;
     Aborted = 0;
     goto A;
   }
 
   SavedRules->Clean();
 
-  cout << "\n\n*** PRUNING ANTECEDENTS AND PRUNING RULES ...\n"
-       << endl;
+  std::cout << "\n\n*** PRUNING ANTECEDENTS AND PRUNING RULES ...\n"
+            << std::endl;
   SavedRules->MixPrune();
 
-  cout << "\n\n*** EXPANDING RULES ...\n"
-       << endl;
+  std::cout << "\n\n*** EXPANDING RULES ...\n"
+            << std::endl;
   SavedRules->EnlargeAndPrune();
 
   nbAnt2 = SavedRules->CountAnt();
   if (nbAnt2 < nbAnt1) {
-    cout << "\n\n*** RULE SET IMPROVED BY " << nbAnt1 - nbAnt2;
-    cout << " ANTECEDENTS" << endl;
+    std::cout << "\n\n*** RULE SET IMPROVED BY " << nbAnt1 - nbAnt2;
+    std::cout << " ANTECEDENTS" << std::endl;
 
     clean.Del();
     CleanRuleStruct clean2(data, train, trainClass,
                            valid, validClass, test, testClass,
                            SavedRules, Bpnn, Out, NbOut);
-    cout << "\n\n*** WRITING IF-THEN RULES ...\n"
-         << endl;
+    std::cout << "\n\n*** WRITING IF-THEN RULES ...\n"
+              << std::endl;
 
     if (attr.IsFileAttr()) {
       clean2.SetAttr(attr.GetListAttr());
       clean2.SetStrClass(attr.GetListClasses(), 0);
     } else {
       clean2.SetAttr();
       clean2.SetStrClass(0);
     }
-    clean2.WriteRules(0, ruleFile);
+    if (mus.empty()) {
+      clean2.WriteRules(0, ruleFile);
+    } else {
+      clean2.WriteRules(0, ruleFile, mus, sigmas, normalizationIndices);
+    }
   }
 
   else {
-    cout << "\n\n*** RULE SET DOES NOT IMPROVE (" << nbAnt1 - nbAnt2 << ")\n";
+    std::cout << "\n\n*** RULE SET DOES NOT IMPROVE (" << nbAnt1 - nbAnt2 << ")" << std::endl;
   A:
-    cout << "\n    (WRITING PREVIOUS ONE)\n";
+    std::cout << "\n    (WRITING PREVIOUS ONE)" << std::endl;
 
-    cout << "\n\n*** WRITING IF-THEN RULES ...\n\n";
+    std::cout << "\n\n*** WRITING IF-THEN RULES ...\n"
+              << std::endl;
 
     if (attr.IsFileAttr()) {
       clean.SetAttr(attr.GetListAttr());
       clean.SetStrClass(attr.GetListClasses(), 0);
     } else {
       clean.SetAttr();
       clean.SetStrClass(0);
     }
 
-    clean.WriteRules(0, ruleFile);
+    if (mus.empty()) {
+      clean.WriteRules(0, ruleFile);
+    } else {
+      clean.WriteRules(0, ruleFile, mus, sigmas, normalizationIndices);
+    }
   }
   SavedRules->Del();
 
   Descr->Del();
 }
 
 ////////////////////////////////////////////////////////////////////////
```

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/realHyp.h` & `dimlpfidex-0.0.1/dimlp/cpp/src/realHyp.h`

 * *Files 13% similar despite different names*

```diff
@@ -45,15 +45,15 @@
   std::vector<std::vector<int>> ConfirmedVirt;
   std::vector<int> ConfBefFirstHyp;
   std::vector<int> ClassPatNet;
 
   int Aborted;
   //----------------------------------------------------------------
 
-  void SaveRule(std::shared_ptr<Rule> path) const { SavedRules->Insert(path); }
+  void SaveRule(std::shared_ptr<DimlpRule> path) const { SavedRules->Insert(path); }
 
   int MaxOnPos(const std::vector<int> &vec) const;
   int GiveIndMax(const int *vec, int nbEl) const;
 
   void SetConfirmedVirt2();
 
   void Gl1(int var, int indPat, int startVirt, int netAns);
@@ -64,19 +64,19 @@
   virtual void GoRight(int var, int indPat, int startVirt, int netAns) { Gr1(var, indPat, startVirt, netAns); }
 
   void OneExRealHyp(DataSet &data, int indPat);
 
   std::shared_ptr<Ante> FindMostDiscrAnt(int sel) const;
 
   int ComputeCorrect(std::shared_ptr<StringInt> listPatLeft, std::shared_ptr<StringInt> listPatRight);
-  void SetCountPatDiscr(std::shared_ptr<StringInt> listPat, std::shared_ptr<Rule> r) const;
-  void SetCountPatDiscr2(DataSet &data, std::shared_ptr<Rule> r);
+  void SetCountPatDiscr(std::shared_ptr<StringInt> listPat, std::shared_ptr<DimlpRule> r) const;
+  void SetCountPatDiscr2(DataSet &data, std::shared_ptr<DimlpRule> r);
 
-  void DeepSearch(DataSet &data, std::shared_ptr<Rule> path, std::shared_ptr<StringInt> subSet);
-  void DeepSearch2(DataSet &data, std::shared_ptr<Rule> path);
+  void DeepSearch(DataSet &data, std::shared_ptr<DimlpRule> path, std::shared_ptr<StringInt> subSet);
+  void DeepSearch2(DataSet &data, std::shared_ptr<DimlpRule> path);
 
   //----------------------------------------------------------------
 
 public:
   int TreeAborted() const { return Aborted; }
 
   void SetConfirmedVirt(DataSet &data);
@@ -90,15 +90,18 @@
       const DataSet &train,
       const DataSet &trainClass,
       const DataSet &valid,
       const DataSet &validClass,
       const DataSet &test,
       const DataSet &testClass,
       const AttrName &attr,
-      std::ostream &ruleFile);
+      std::ostream &ruleFile,
+      const std::vector<double> &mus = std::vector<double>(),
+      const std::vector<double> &sigmas = std::vector<double>(),
+      const std::vector<int> &normalizationIndices = std::vector<int>());
 
   //----------------------------------------------------------------
 
   virtual ~RealHyp() = default;
 
   RealHyp(
       DataSet &data,
```

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/realHyp2.cpp` & `dimlpfidex-0.0.1/dimlp/cpp/src/realHyp2.cpp`

 * *Files identical despite different names*

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/realHyp2.h` & `dimlpfidex-0.0.1/dimlp/cpp/src/realHyp2.h`

 * *Files identical despite different names*

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/rule.cpp` & `dimlpfidex-0.0.1/dimlp/cpp/src/dimlpRule.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-#include "rule.h"
+#include "dimlpRule.h"
 
 ///////////////////////////////////////////////////////////////////
 
-int Rule::GetNbAntWithout()
+int DimlpRule::GetNbAntWithout()
 
 {
   int a;
   int count;
 
   for (a = 0, count = 0, GoToBeg(); a < NbAnt; a++, GoToNext())
     if (IsAntDeleted() == 0)
       count++;
 
   return count;
 }
 
 ///////////////////////////////////////////////////////////////////
 
-void Rule::DeleteRule()
+void DimlpRule::DeleteRule()
 
 {
   int a;
 
   for (a = 0, GoToBeg(); a < NbAnt; a++, GoToNext())
     RemAnt();
 }
 
 ///////////////////////////////////////////////////////////////////
 
-void Rule::Insert(int var, float val, char rel)
+void DimlpRule::Insert(int var, float val, char rel)
 
 {
   if (NbAnt == 0) {
     FirstAnt = std::make_shared<Antecedent>();
     // FirstAnt = new Antecedent;
     FirstAnt->Var = var;
     FirstAnt->Val = val;
@@ -55,15 +55,15 @@
   }
 
   NbAnt++;
 }
 
 ///////////////////////////////////////////////////////////////////
 
-Rule *Rule::Copy(std::shared_ptr<Rule> r)
+DimlpRule *DimlpRule::Copy(std::shared_ptr<DimlpRule> r)
 
 {
   int a;
   int nbAnt = r->GetNbAnt();
 
   for (a = 0, r->GoToBeg(); a < nbAnt; a++, r->GoToNext()) {
     this->Insert(r->GetVar(), r->GetVal(), r->GetRel());
```

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/rule.h` & `dimlpfidex-0.0.1/dimlp/cpp/src/dimlpRule.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-#ifndef RULE_H
-#define RULE_H
+#ifndef DIMLPRULE_H
+#define DIMLPRULE_H
 
 #include <memory>
 
 ////////////////////////////////////////////////////////////////////////
 
-class Rule {
+class DimlpRule {
   struct Antecedent {
     int Var;
     float Val;
     char Rel;
     std::shared_ptr<Antecedent> Next;
   };
 
@@ -35,18 +35,17 @@
   int IsAntDeleted() const { return ((PtrAnt->Var == -1) ? 1 : 0); }
   void SavePtrAnt() { Memory = PtrAnt; }
   void PrevPtrAnt() { PtrAnt = Memory; }
 
   int GetNbAntWithout();
   void DeleteRule();
   void Insert(int var, float val, char rel);
-  Rule *Copy(std::shared_ptr<Rule> r);
+  DimlpRule *Copy(std::shared_ptr<DimlpRule> r);
 
   void Del() {
     NbAnt = 0;
   }
 
-  Rule() = default;
-  ~Rule() = default;
+  DimlpRule() = default;
 };
 
 #endif
```

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/rulePro.cpp` & `dimlpfidex-0.0.1/dimlp/cpp/src/rulePro.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     return -1;
 
   return indMin;
 }
 
 ///////////////////////////////////////////////////////////////////
 
-int RuleProcessing::IsRuleEmpty(std::shared_ptr<Rule> rule) const
+int RuleProcessing::IsRuleEmpty(std::shared_ptr<DimlpRule> rule) const
 
 {
   int r;
   int nbAnt = rule->GetNbAnt();
 
   for (r = 0, rule->GoToBeg(); r < nbAnt; r++, rule->GoToNext())
     if (rule->IsAntDeleted() == 0)
@@ -89,15 +89,15 @@
 int RuleProcessing::CountAnt()
 
 {
   int a;
   int r;
   int nbAnt;
   int count;
-  std::shared_ptr<Rule> rule;
+  std::shared_ptr<DimlpRule> rule;
 
   for (r = 0, count = 0, GoToBeg(); r < NbRules; r++, GoToNext()) {
     rule = GetRule();
     nbAnt = rule->GetNbAnt();
 
     for (a = 0, rule->GoToBeg(); a < nbAnt; a++, rule->GoToNext())
       if (rule->IsAntDeleted() == 0)
@@ -127,15 +127,15 @@
 
 ////////////////////////////////////////////////////////////////////////
 
 void RuleProcessing::SetCarriedField()
 
 {
   int r;
-  std::shared_ptr<Rule> rule;
+  std::shared_ptr<DimlpRule> rule;
 
   for (r = 0, GoToBeg(); r < NbRules; r++, GoToNext()) {
     rule = GetRule();
 
     if (IsRuleEmpty(rule) == 1)
       continue;
 
@@ -145,15 +145,15 @@
 
 ////////////////////////////////////////////////////////////////////////
 
 void RuleProcessing::DelListCar()
 
 {
   int r;
-  std::shared_ptr<Rule> rule;
+  std::shared_ptr<DimlpRule> rule;
   std::shared_ptr<StringInt> carried;
 
   for (r = 0, GoToBeg(); r < NbRules; r++, GoToNext()) {
     rule = GetRule();
 
     if (IsRuleEmpty(rule) == 1)
       continue;
@@ -170,15 +170,15 @@
 {
   int p;
   int r;
   int nbEl;
 
   int nbEx = Data.GetNbEx();
   std::vector<int> checkTab(nbEx, 0);
-  std::shared_ptr<Rule> rule;
+  std::shared_ptr<DimlpRule> rule;
   std::shared_ptr<StringInt> carriedEx;
 
   for (r = 0, GoToBeg(); r < NbRules; r++, GoToNext()) {
     if (r == toDrop)
       continue;
 
     rule = GetRule();
@@ -204,15 +204,15 @@
 
 ////////////////////////////////////////////////////////////////////////
 
 void RuleProcessing::SetCountAntRules()
 
 {
   int r;
-  std::shared_ptr<Rule> rule;
+  std::shared_ptr<DimlpRule> rule;
 
   for (r = 0, GoToBeg(); r < NbRules; r++, GoToNext()) {
     rule = GetRule();
 
     if (IsRuleEmpty(rule)) {
       TabRules[r] = 0;
       continue;
@@ -224,15 +224,15 @@
 
 ////////////////////////////////////////////////////////////////////////
 
 int RuleProcessing::GoToSavedAndRemRule(int indPrune)
 
 {
   int r;
-  std::shared_ptr<Rule> rule;
+  std::shared_ptr<DimlpRule> rule;
 
   if (CheckAllCarried(indPrune) == 1) {
     for (r = 0, GoToBeg(); r < indPrune; r++, GoToNext())
       ;
 
     rule = GetRule();
     rule->DeleteRule();
@@ -314,15 +314,15 @@
 
 {
   int a;
   int r;
   int indRule;
   int indAnt;
   int remAnt;
-  std::shared_ptr<Rule> rule;
+  std::shared_ptr<DimlpRule> rule;
   std::shared_ptr<StringInt> newCarried;
 
   for (r = 0, RuleInd.GoToBeg(); r < indPrune; r++, RuleInd.GoToNext())
     ;
   indRule = RuleInd.GetVal();
 
   for (r = 0, AntInd.GoToBeg(); r < indPrune; r++, AntInd.GoToNext())
@@ -357,15 +357,15 @@
 
 {
   int a;
   int r;
   int nbAnt;
   int remAnt;
   int diff;
-  std::shared_ptr<Rule> rule;
+  std::shared_ptr<DimlpRule> rule;
   std::shared_ptr<StringInt> oldCarried;
   std::shared_ptr<StringInt> newCarried;
 
   for (r = 0, GoToBeg(); r < NbRules; r++, GoToNext()) {
     rule = GetRule();
 
     if (IsRuleEmpty(rule))
@@ -447,15 +447,15 @@
 
     FastRulePrune(NbRules);
   }
 }
 
 ////////////////////////////////////////////////////////////////////////
 
-void RuleProcessing::RemSevThres(std::shared_ptr<Rule> r) const
+void RuleProcessing::RemSevThres(std::shared_ptr<DimlpRule> r) const
 
 {
   int a;
   int h;
   int first;
   float min;
   float max;
@@ -544,25 +544,25 @@
 
   for (r = 0, GoToBeg(); r < NbRules; r++, GoToNext())
     RemSevThres(GetRule());
 }
 
 ////////////////////////////////////////////////////////////////////////
 
-void RuleProcessing::Insert(std::shared_ptr<Rule> r)
+void RuleProcessing::Insert(std::shared_ptr<DimlpRule> r)
 
 {
   int a;
   int nbAnt = r->GetNbAnt();
 
   if (NbRules != 0)
     Current = First;
 
   First = std::make_shared<Saved>();
-  auto ru = std::make_shared<Rule>();
+  auto ru = std::make_shared<DimlpRule>();
 
   for (a = 0, r->GoToBeg(); a < nbAnt; a++, r->GoToNext()) {
     ru->Insert(r->GetVar(), r->GetVal(), r->GetRel());
   }
 
   First->OneRule = ru;
 
@@ -588,15 +588,15 @@
 }
 
 ////////////////////////////////////////////////////////////////////////
 
 void RuleProcessing::RemCurrentRule() const
 
 {
-  std::shared_ptr<Rule> rule = GetRule();
+  std::shared_ptr<DimlpRule> rule = GetRule();
   int nbAnt = rule->GetNbAnt();
   int a;
 
   for (a = 0, rule->GoToBeg(); a < nbAnt; a++, rule->GoToNext())
     rule->RemAnt();
 }
 ////////////////////////////////////////////////////////////////////////
@@ -614,18 +614,18 @@
   int nbCarriedMod;
   int nbEnlarged;
   int indMax;
   int count;
   std::vector<int> vecCarried;
   float val;
   float thres;
-  Rule oneCopy;
-  std::shared_ptr<Rule> anotherCopy;
-  std::shared_ptr<Rule> rule;
-  std::vector<std::shared_ptr<Rule>> enlarged;
+  DimlpRule oneCopy;
+  std::shared_ptr<DimlpRule> anotherCopy;
+  std::shared_ptr<DimlpRule> rule;
+  std::vector<std::shared_ptr<DimlpRule>> enlarged;
 
   OneVarThresDescr *oneVarDescr;
   std::shared_ptr<StringInt> carried;
   std::shared_ptr<StringInt> carriedMod;
 
   int nbRules = NbRules;
 
@@ -670,24 +670,24 @@
 
           if (thres == val)
             continue;
 
           oneCopy.SetThres(thres);
 
           oneCopy.SavePtrAnt();
-          carriedMod = Data.Select(std::make_shared<Rule>(oneCopy));
+          carriedMod = Data.Select(std::make_shared<DimlpRule>(oneCopy));
           oneCopy.PrevPtrAnt();
 
           nbCarriedMod = carriedMod->GetNbEl();
 
           if (nbCarriedMod > nbCarried && AreSameClass(carriedMod, ClassPatNet) == 1) {
-            anotherCopy = std::make_shared<Rule>();
+            anotherCopy = std::make_shared<DimlpRule>();
 
             oneCopy.SavePtrAnt();
-            anotherCopy->Copy(std::make_shared<Rule>(oneCopy));
+            anotherCopy->Copy(std::make_shared<DimlpRule>(oneCopy));
             oneCopy.PrevPtrAnt();
 
             vecCarried[nbEnlarged] = nbCarriedMod;
             enlarged[nbEnlarged] = anotherCopy;
             nbEnlarged++;
           }
           carriedMod->Del();
```

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/rulePro.h` & `dimlpfidex-0.0.1/dimlp/cpp/src/rulePro.h`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   std::shared_ptr<ThresDescr> Descr;
 
   StringInt Gain;
   StringInt RuleInd;
   StringInt AntInd;
 
   struct Saved {
-    std::shared_ptr<Rule> OneRule;
+    std::shared_ptr<DimlpRule> OneRule;
     std::shared_ptr<StringInt> Carried;
     std::shared_ptr<Saved> Next;
   };
 
   std::shared_ptr<Saved> First;
   std::shared_ptr<Saved> Current;
   std::shared_ptr<Saved> Memory;
@@ -46,39 +46,39 @@
   void SetCountAntRules();
   void SetCarriedField();
   void DelListCar();
   int CheckAllCarried(int toDrop);
   void RemCurrentRule() const;
   int GoToSavedAndRemRule(int indPrune);
   void GoToRuleAndRemAnt(int indPrune);
-  void RemSevThres(std::shared_ptr<Rule> r) const;
+  void RemSevThres(std::shared_ptr<DimlpRule> r) const;
   void ComputeGain();
   void RulePruneByMinCar();
   void FastRulePrune(int nbIt);
   int TryEnlargedThres();
 
   //----------------------------------------------------------------
 
 public:
-  int IsRuleEmpty(std::shared_ptr<Rule> rule) const;
+  int IsRuleEmpty(std::shared_ptr<DimlpRule> rule) const;
   int GetNbRules() const { return NbRules; }
   void GoToBeg() { Current = First; }
   void GoToNext() { Current = Current->Next; }
-  std::shared_ptr<Rule> GetRule() const { return Current->OneRule; }
+  std::shared_ptr<DimlpRule> GetRule() const { return Current->OneRule; }
   void Save() { Memory = Current; }
   void Previous() { Current = Memory; }
 
   int CountAnt();
   int CountRules();
 
   void Clean();
   void MixPrune();
   void EnlargeAndPrune();
 
-  void Insert(std::shared_ptr<Rule> r);
+  void Insert(std::shared_ptr<DimlpRule> r);
   void Del();
 
   RuleProcessing(
       int nbVar,
       int nbHyp,
       DataSet data,
       const std::vector<int> &classPatNet,
```

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/stairObj.cpp` & `dimlpfidex-0.0.1/dimlp/cpp/src/stairObj.cpp`

 * *Files identical despite different names*

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/stairObj.h` & `dimlpfidex-0.0.1/dimlp/cpp/src/stairObj.h`

 * *Files identical despite different names*

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/standAct.cpp` & `dimlpfidex-0.0.1/dimlp/cpp/src/standAct.cpp`

 * *Files identical despite different names*

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/stringI.cpp` & `dimlpfidex-0.0.1/common/cpp/src/stringI.cpp`

 * *Files identical despite different names*

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/stringI.h` & `dimlpfidex-0.0.1/common/cpp/src/stringI.h`

 * *Files identical despite different names*

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/thresD.cpp` & `dimlpfidex-0.0.1/dimlp/cpp/src/thresD.cpp`

 * *Files identical despite different names*

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/thresD.h` & `dimlpfidex-0.0.1/dimlp/cpp/src/thresD.h`

 * *Files identical despite different names*

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/vectWRV.cpp` & `dimlpfidex-0.0.1/dimlp/cpp/src/vectWRV.cpp`

 * *Files identical despite different names*

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/virtHyp.cpp` & `dimlpfidex-0.0.1/dimlp/cpp/src/virtHyp.cpp`

 * *Files identical despite different names*

### Comparing `dimlpfidex-0.0.0/dimlp/cpp/src/virtHyp.h` & `dimlpfidex-0.0.1/dimlp/cpp/src/virtHyp.h`

 * *Files identical despite different names*

### Comparing `dimlpfidex-0.0.0/dimlp/crossValid.py` & `dimlpfidex-0.0.1/trainings/crossValid.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import os
 import shutil
 import sys
 import platform
 import random
 import math
 import time
+import numpy as np
+from sklearn.metrics import RocCurveDisplay
+import matplotlib.pyplot as plt
 
 # import modules :
 
 if sys.platform == 'win32':
     dir_path = os.path.abspath('dimlpfidex')
     os.add_dll_directory(dir_path)
 
 from dimlpfidex import dimlp
 from dimlpfidex import fidex
-from dimlpfidex import fidexGlo
-from dimlp.svmTrn import svmTrn
-from dimlp.mlpTrn import mlpTrn
-from dimlp.randForestsTrn import randForestsTrn
-from dimlp.gradBoostTrn import gradBoostTrn
-
+from trainings.svmTrn import svmTrn
+from trainings.mlpTrn import mlpTrn
+from trainings.randForestsTrn import randForestsTrn
+from trainings.gradBoostTrn import gradBoostTrn
+from trainings.computeRocCurve import computeRocCurve
+from trainings.trnFun import delete_file, get_data, get_data_class
 
 def create_or_clear_directory(folder_name):
     try:
         if not os.path.exists(folder_name):
             # Create folder if not exist
             os.makedirs(folder_name)
         else:
@@ -34,32 +37,14 @@
                     os.remove(file_path)
                 elif os.path.isdir(file_path):
                     # Delete recursively sub-folders
                     shutil.rmtree(file_path)
     except (OSError):
         raise ValueError(f"Error during the creation of the directory {folder_name}.")
 
-
-def get_data(file_name): # Get data from file
-    try:
-        with open(file_name, "r") as my_file:
-            data = []
-            line = my_file.readline()
-            while line:
-                line = line.strip()  # Remove the line break at the end of the line
-                if line.strip():
-                    data.append(line)
-                line = my_file.readline()
-            my_file.close()
-        return data
-    except (FileNotFoundError):
-        raise ValueError(f"Error : File {file_name} not found.")
-    except (IOError):
-        raise ValueError(f"Error : Couldn't open file {file_name}.")
-
 def get_dimlprul_stats(rule_file):
 
     try:
         with open(rule_file, "r") as my_file:
             lines = my_file.readlines()
             my_file.close()
 
@@ -106,107 +91,123 @@
                     return float(value.strip())
 
     except (FileNotFoundError):
         raise ValueError(f"Error : Train stat file {stats_file} not found.")
     except (IOError):
         raise ValueError(f"Error : Couldn't open train stat file {stats_file}.")
 
-
+def formatting(number):
+    if number == "N/A":
+        return number
+    else:
+        formatted_number = "{:.6f}".format(number).rstrip(".0")
+        if formatted_number == "":
+            formatted_number = "0"
+        return formatted_number
 
 def crossValid(*args, **kwargs):
     try:
-        if args or not kwargs:
+        if not kwargs:
             print("---------------------------------------------------------------------")
             print("Please specify arguments using named parameters.")
             print("Warning! The files are localised with respect to root folder dimlpfidex.")
 
             print("----------------------------")
-            print("Obligatory parameters :")
+            print("Required parameters :")
             print("train_method : dimlp, dimlpBT, svm, mlp, randForest or gradBoost")
             print("algo : fidex, fidexGlo or both")
             print("data_file : data file")
-            print("class_file : class file")
+            print("class_file : class file, not mandatory if classes are specified in train file")
+            print("nb_attributes : number of input neurons")
+            print("nb_classes : number of output neurons")
 
             print("----------------------------")
-            print("Obligatory parameters if training with dimlp :")
-            print("nb_in : number of input neurons")
-            print("nb_out : number of output neurons")
-            print("dimlpRul : 1(with dimlpRul, default) or 0")
+            print("Required parameters if training with dimlp and dimlpBT :")
+            print("dimlpRul : 1(with dimlpRul) or 0")
 
             print("----------------------------")
             print("Optional parameters :")
-            print("save_folder : Folder based on main folder dimlpfidex(default folder) where generated files will be saved. If a file name is specified with another option, his path will be configured with respect to this root folder.")
+            print("root_folder : Folder based on main folder dimlpfidex(default folder) containg all used files and where generated files will be saved. If a file name is specified with another option, his path will be configured with respect to this root folder.")
             print("crossVal_folder : Folder name where to save crossValidation data (CrossValidation by default)")
             print("K : K-fold cross-validation (10 by default)")
             print("N : number of times we do the cross-validation (10 by default)")
             print("fidexGlo_heuristic : 1: optimal fidexGlo(default), 2: fast fidexGlo 3: very fast fidexGlo")
             print("crossVal_stats : statistics of cross validation (crossValidationStats.txt by default)")
-            print("attr_file : file of attributes")
-            print("max_iter : maximum fidex and fidexGlo iteration number (100 by default)")
-            print("min_cov : minimum fidex and fidexGlo covering number (2 by default)")
+            print("attributes_file : file of attributes")
+            print("max_iterations : maximum fidex and fidexGlo iteration number (100 by default)")
+            print("min_covering : minimum fidex and fidexGlo covering number (2 by default)")
+            print("covering_strategy <Whether to use this strategy : if no rule is found with min_covering, find best rule with best covering using dichotomic search. Decreases min_fidelity if needed (True by default)>")
+            print("min_fidelity <minimal rule fidelity accepted when generating a rule [0,1] (1 by default)>")
+            print("lowest_min_fidelity <minimal min_fidelity to which we agree to go down during covering_strategy (0.75 by default)>")
             print("dropout_dim : dimension dropout parameter for fidex and fidexGlo")
             print("dropout_hyp : hyperplan dropout parameter for fidex and fidexGlo")
             print("seed : 0 = random (default)")
+            print("positive_class_index <index of positive class sample to compute true/false positive/negative rates and ROC curve (None by default, put 0 for first class)")
+            print("decision_threshold <decision threshold for predictions, need to specify the index of positive class if you want to use it (None by default)>")
+            print("normalization_file <file containing the mean and std of some attributes. Used to denormalize the rules if specified>")
+            print("mus <list of float in the form [1.1,3.5] without spaces(!) corresponding to mean or median of each attribute index to denormalize in the rules>")
+            print("sigmas <list of float in the form [4.5,12] without spaces(!) corresponding to standard deviation of each attribute index to denormalize in the rules>")
+            print("normalization_indices <list of integers in the form [0,3,7] without spaces(!) corresponding to attribute indices to denormalize in the rules (first column is index 0, all indices by default, only used when no normalization_file is given)>")
+            print("nb_threads <number of threads used for computing the fidexGloRules algorithm (default=1, this means by default its a sequential execution)>")
 
             print("----------------------------")
             print("Optional parameters if not training with decision trees :")
-            print("hiknot : high side of the interval (5 by default)")
-            print("nb_stairs : number of stairs in staircase activation function (50 by default)")
+            print("nb_quant_levels : number of stairs in staircase activation function (50 by default)")
 
             print("----------------------------")
             print("Optional parameters for dimlp and dimlpBT training:")
             print("pretrained_weights : file of pretrained weights")
-            print("H1 : number of neurons in the first hidden layer. If not specified this number will be equal to the number of input neurons.")
-            print("Hk : number of neurons in the kth hidden layer.")
-            print("eta : back-propagation learning parameter (0.1 by default)")
-            print("mu : back-propagation momentum parameter (0.6 by default)")
+            print("first_hidden_layer <int k*nb_attributes, k in [1,inf[> Number of neurons in the first hidden layer (default: nb_attributes)")
+            print("hidden_layers <list<int [1,inf[>> Number of neurons in each hidden layer, from the second layer through to the last.")
+            print("learning_rate : back-propagation learning parameter (0.1 by default)")
+            print("momentum : back-propagation momentum parameter (0.6 by default)")
             print("flat : back-propagation flat spot elimination parameter (0.01 by default)")
-            print("err_thresh : error threshold (-1111111111.0 by default)")
-            print("acc_thresh : accuracy threshold (11111111111111.0 by default)")
-            print("delta_err : absolute difference error threshold (0 by default)")
+            print("error_thresh : error threshold (None by default)")
+            print("acc_thresh : accuracy threshold (None by default)")
+            print("abs_error_thresh : absolute difference error threshold (0 by default)")
             print("nb_epochs : number of train epochs (1500 by default)")
-            print("show_err : number of train epochs to show error (10 by default)")
+            print("nb_epochs_error : number of train epochs to show error (10 by default)")
 
             print("----------------------------")
             print("Optional parameters for dimlpBT training:")
             print("nb_dimlp_nets : number of dimlp networks, integer >= 2 (25 by default)")
-            print("nb_ex_in_one : number of examples for one single network, positive integer, 0 = number of train examples (default)")
+            print("nb_ex_per_net : number of examples for one single network, positive integer, 0 = number of train examples (default)")
 
             print("----------------------------")
             print("Optional parameters for svm training:")
             print("svm_K : Parameter to improve dynamics (1 by default)")
             print("C : regularization, (1.0 by default)")
             print("kernel : linear, poly, rbf(default) or sigmoid")
             print("degree : polynomial degree (3 by default)")
             print("gamma : scale(default), auto or non negative float")
             print("coef0 : term in kernel function, float (0 by default)")
             print("shrinking : heuristic, True(default) or False")
             print("svm_tol : tolerance for stopping criterion (0.001 by default)")
             print("cache_size : kernel cache size (200 MB by default)")
             print("svm_class_weight : class balance, 'balanced' or a dictionary, for exemple with 2 classes : {0:1.2, 1:3.5} (None by default)")
-            print("svm_max_iter : maximal number of iterations (-1 for no limit (default))")
+            print("svm_max_iterations : maximal number of iterations (-1 for no limit (default))")
             print("decision_function_shape : decision function shape, ovo(one-vs-one) or ovr(one-vs-rest, default)")
             print("break_ties : break tie decision for ovr with more than 2 classes, True or False(default)")
 
             print("----------------------------")
             print("Optional parameters for mlp training:")
             print("mlp_K : Parameter to improve dynamics (1 by default)")
             print("hidden_layer_sizes : Size of each hidden layers. Array of shape (n_layers-2) ((100,) by default)")
             print("activation : activation function, identity, logistic, tanh or relu(default)")
             print("solver : solver for weight optimization, lbfgs, sgd or adam (default)")
             print("alpha : strength of the L2 regularization term, positive float (0.0001 by default)")
             print("batch_size : size of minibatches for stochastic optimizers for adam and sgd, auto(default) or positive integer")
             print("mlp_learning_rate : learning rate schedule for weight updates for sgd solver, constant(default), invscaling or adaptive")
             print("learning_rate_init : initial learning rate for adam and sgd, positive float (0.001 by default)")
             print("power_t : exponent for inverse scaling learning rate for sgd, positive float (0.5 by default)")
-            print("mlp_max_iter : maximum number of iterations, positive integer (200 by default)")
+            print("mlp_max_iterations : maximum number of iterations, positive integer (200 by default)")
             print("shuffle : whether to shuffle samples in each iteration for sgd and adam, True(default) or False")
             print("mlp_tol : tolerance for optimization (0.0001 by default)")
             print("mlp_warm_start : whether to reuse previous solution to fit initialization, True or False(default)")
-            print("momentum : Momentum for gradient descent update for sgd, between 0 and 1 (0.9 by default)")
+            print("mlp_momentum : Momentum for gradient descent update for sgd, between 0 and 1 (0.9 by default)")
             print("nesterovs_momentum : whether to use Nesterov’s momentum for sgd and momentum > 0, True(default) or False")
             print("early_stopping : whether to use early stopping to terminate training when validation score is not improving for sgd and adam, True or False(default)")
             print("mlp_validation_fraction : proportion of training data to set aside as validation set for early stopping, between 0 and 1 excluded (0.1 by default)")
             print("beta_1 : exponential decay rate for estimates of first moment vector in adam, between 0 and 1 excluded (0.9 by default)")
             print("beta_2 : exponential decay rate for estimates of second moment vector in adam, between 0 and 1 excluded (0.999 by default)")
             print("epsilon : value for numerical stability in adam, positive float (1e-8 by default)")
             print("mlp_n_iter_no_change : maximum number of epochs to not meet tol improvement for sgd and adam, integer >= 1 (10 by default)")
@@ -247,109 +248,117 @@
             print("gb_tol : tolerance for the early stopping (0.0001 by default)")
 
             print("----------------------------")
             print("----------------------------")
 
             print("Here is an example, keep same parameter names :")
             print("Exemple with Dimlp :")
-            print('crossValid(train_method="dimlp", algo="both", data_file="datanorm", class_file="dataclass2", dimlpRul=1, nb_in=16, nb_out=2, H2=5, save_folder="dimlp/datafiles", crossVal_folder="CrossValidationDIMLP")')
+            print('crossValid(train_method="dimlp", algo="both", data_file="datanorm", class_file="dataclass2", positive_class_index=1, dimlpRul=1, nb_attributes=16, nb_classes=2, hidden_layers=[5], root_folder="dimlp/datafiles", crossVal_folder="CrossValidationDIMLP")')
             print("----------------------------")
-            print("Exemple with DimlpBT :")
-            print('crossValid(train_method="dimlpBT", algo="both", data_file="datanorm", class_file="dataclass2", dimlpRul=1, nb_in=16, nb_out=2, H2=5, save_folder="dimlp/datafiles", crossVal_folder="CrossValidationDIMLPBT")')
+            print("Exemple with dimlpBT :")
+            print('crossValid(train_method="dimlpBT", algo="both", data_file="datanorm", class_file="dataclass2", positive_class_index=1, dimlpRul=1, nb_attributes=16, nb_classes=2, hidden_layers=[5], root_folder="dimlp/datafiles", crossVal_folder="CrossValidationDIMLPBT")')
             print("----------------------------")
             print("Exemple with SVM :")
-            print('crossValid(train_method="svm", algo="both", data_file="datanorm", class_file="dataclass2", save_folder="dimlp/datafiles", crossVal_folder="CrossValidationSVM")')
+            print('crossValid(train_method="svm", algo="both", data_file="datanorm", class_file="dataclass2", positive_class_index=1, nb_attributes=16, nb_classes=2, root_folder="dimlp/datafiles", crossVal_folder="CrossValidationSVM")')
             print("----------------------------")
             print("Exemple with MLP :")
-            print('crossValid(train_method="mlp", algo="both", data_file="datanorm", class_file="dataclass2", save_folder="dimlp/datafiles", crossVal_folder="CrossValidationMLP")')
+            print('crossValid(train_method="mlp", algo="both", data_file="datanorm", class_file="dataclass2", positive_class_index=1, nb_attributes=16, nb_classes=2, root_folder="dimlp/datafiles", crossVal_folder="CrossValidationMLP")')
             print("----------------------------")
             print("Exemple with Random forests :")
-            print('crossValid(train_method="randForest", algo="both", data_file="datanorm", class_file="dataclass2", save_folder="dimlp/datafiles", crossVal_folder="CrossValidationRF")')
+            print('crossValid(train_method="randForest", algo="both", data_file="datanorm", class_file="dataclass2", positive_class_index=1, nb_attributes=16, nb_classes=2, root_folder="dimlp/datafiles", crossVal_folder="CrossValidationRF")')
             print("---------------------------------------------------------------------")
             print("Exemple with Gradient boosting :")
-            print('crossValid(train_method="gradBoost", algo="both", data_file="datanorm", class_file="dataclass2", save_folder="dimlp/datafiles", crossVal_folder="CrossValidationGB")')
+            print('crossValid(train_method="gradBoost", algo="both", data_file="datanorm", class_file="dataclass2", positive_class_index=1, nb_attributes=16, nb_classes=2, root_folder="dimlp/datafiles", crossVal_folder="CrossValidationGB")')
             print("---------------------------------------------------------------------")
 
             return 0
 
         else:
 
             start_time = time.time()
 
             # Get parameters
             train_method = kwargs.get('train_method')
             algo = kwargs.get('algo')
             data_file = kwargs.get('data_file')
             class_file = kwargs.get('class_file')
 
-            nb_in = kwargs.get('nb_in')
-            nb_out = kwargs.get('nb_out')
+            nb_attributes = kwargs.get('nb_attributes')
+            nb_classes = kwargs.get('nb_classes')
             dimlprul = kwargs.get('dimlpRul')
 
-            save_folder = kwargs.get('save_folder')
+            root_folder = kwargs.get('root_folder')
             crossval_folder = kwargs.get('crossVal_folder')
             k = kwargs.get('K')
             n = kwargs.get('N')
             fidexglo_heuristic = kwargs.get('fidexGlo_heuristic')
             crossval_stats = kwargs.get('crossVal_stats')
-            attr_file = kwargs.get('attr_file')
-            max_iter = kwargs.get('max_iter')
-            min_cov = kwargs.get('min_cov')
+            attributes_file = kwargs.get('attributes_file')
+            max_iterations = kwargs.get('max_iterations')
+            min_covering = kwargs.get('min_covering')
+            covering_strategy = kwargs.get('covering_strategy')
+            min_fidelity = kwargs.get('min_fidelity')
+            lowest_min_fidelity = kwargs.get('lowest_min_fidelity')
             dropout_dim = kwargs.get('dropout_dim')
             dropout_hyp = kwargs.get('dropout_hyp')
+            positive_class_index = kwargs.get('positive_class_index')
+            decision_threshold = kwargs.get('decision_threshold')
             seed = kwargs.get('seed')
+            normalization_file = kwargs.get('normalization_file')
+            mus = kwargs.get('mus')
+            sigmas = kwargs.get('sigmas')
+            normalization_indices = kwargs.get('normalization_indices')
+            nb_threads = kwargs.get('nb_threads')
 
-            hiknot = kwargs.get('hiknot')
-            nb_stairs = kwargs.get('nb_stairs')
+            hiknot = 5
+            nb_quant_levels = kwargs.get('nb_quant_levels')
 
             pretrained_weights = kwargs.get('pretrained_weights')
-            hk = {}
-            for key, value in kwargs.items():
-                if key.startswith('H') and key[1:].isdigit():
-                    hk[key] = value
-            eta = kwargs.get('eta')
-            mu = kwargs.get('mu')
+            first_hidden_layer = kwargs.get('first_hidden_layer')
+            hidden_layers = kwargs.get('hidden_layers')
+            learning_rate = kwargs.get('learning_rate')
+            momentum = kwargs.get('momentum')
             flat = kwargs.get('flat')
-            err_thresh = kwargs.get('err_thresh')
+            error_thresh = kwargs.get('error_thresh')
             acc_thresh = kwargs.get('acc_thresh')
-            delta_err = kwargs.get('delta_err')
+            abs_error_thresh = kwargs.get('abs_error_thresh')
             nb_epochs = kwargs.get('nb_epochs')
-            show_err = kwargs.get('show_err')
+            nb_epochs_error = kwargs.get('nb_epochs_error')
 
             nb_dimlp_nets = kwargs.get('nb_dimlp_nets')
-            nb_ex_in_one = kwargs.get('nb_ex_in_one')
+            nb_ex_per_net = kwargs.get('nb_ex_per_net')
 
             svm_k = kwargs.get('svm_K')
             c_var = kwargs.get('C')
             kernel_var = kwargs.get('kernel')
             degree_var = kwargs.get('degree')
             gamma_var = kwargs.get('gamma')
             coef0_var = kwargs.get('coef0')
             shrinking_var = kwargs.get('shrinking')
             svm_tol_var = kwargs.get('svm_tol')
             cache_size_var = kwargs.get('cache_size')
             svm_class_weight_var = kwargs.get('svm_class_weight')
-            svm_max_iter_var = kwargs.get('svm_max_iter')
+            svm_max_iterations_var = kwargs.get('svm_max_iterations')
             decision_function_shape_var = kwargs.get('decision_function_shape')
             break_ties_var = kwargs.get('break_ties')
 
             mlp_k = kwargs.get('mlp_K')
             hidden_layer_sizes_var = kwargs.get('hidden_layer_sizes')
             activation_var = kwargs.get('activation')
             solver_var = kwargs.get('solver')
             alpha_var = kwargs.get('alpha')
             batch_size_var = kwargs.get('batch_size')
             mlp_learning_rate_var = kwargs.get('mlp_learning_rate')
             learning_rate_init_var = kwargs.get('learning_rate_init')
             power_t_var = kwargs.get('power_t')
-            mlp_max_iter_var = kwargs.get('mlp_max_iter')
+            mlp_max_iterations_var = kwargs.get('mlp_max_iterations')
             shuffle_var = kwargs.get('shuffle')
             mlp_tol_var = kwargs.get('mlp_tol')
             mlp_warm_start_var = kwargs.get('mlp_warm_start')
-            momentum_var = kwargs.get('momentum')
+            mlp_momentum_var = kwargs.get('mlp_momentum')
             nesterovs_momentum_var = kwargs.get('nesterovs_momentum')
             early_stopping_var = kwargs.get('early_stopping')
             mlp_validation_fraction_var = kwargs.get('mlp_validation_fraction')
             beta_1_var = kwargs.get('beta_1')
             beta_2_var = kwargs.get('beta_2')
             epsilon_var = kwargs.get('epsilon')
             mlp_n_iter_no_change_var = kwargs.get('mlp_n_iter_no_change')
@@ -381,254 +390,195 @@
             init_var = kwargs.get('init')
             gb_validation_fraction_var = kwargs.get('gb_validation_fraction')
             gb_n_iter_no_change_var = kwargs.get('gb_n_iter_no_change')
             gb_tol_var = kwargs.get('gb_tol')
 
             # Check parameters
 
-            obligatory_args = ['train_method', 'algo', 'data_file', 'class_file']
-            obligatory_dimlp_args = ['nb_in', 'nb_out', 'dimlpRul']
+            obligatory_args = ['train_method', 'algo', 'data_file','nb_attributes', 'nb_classes']
+            obligatory_dimlp_args = ['dimlpRul']
 
-            optional_args = ['save_folder', 'crossVal_folder', 'K', 'N', 'fidexGlo_heuristic', 'crossVal_stats', 'attr_file',
-                        'max_iter', 'min_cov', 'dropout_dim', 'dropout_hyp', 'seed']
+            optional_args = ['class_file', 'root_folder', 'crossVal_folder', 'K', 'N', 'fidexGlo_heuristic', 'crossVal_stats', 'attributes_file',
+                        'max_iterations', 'min_covering', 'covering_strategy', 'min_fidelity', 'lowest_min_fidelity', 'dropout_dim', 'dropout_hyp',
+                        'seed', 'positive_class_index', 'decision_threshold', 'normalization_file', 'mus', 'sigmas', 'normalization_indices', 'nb_threads']
 
-            optional_non_dt_args = ['hiknot', 'nb_stairs']
+            optional_non_dt_args = ['nb_quant_levels']
 
-            optional_dimlp_args = ['pretrained_weights', 'eta', 'mu', 'flat', 'err_thresh',
-                        'acc_thresh', 'delta_err', 'nb_epochs', 'show_err']
+            optional_dimlp_args = ['pretrained_weights', 'learning_rate', 'momentum', 'flat', 'error_thresh',
+                        'acc_thresh', 'abs_error_thresh', 'nb_epochs', 'nb_epochs_error', 'hidden_layers']
 
-            optional_dimlpBT_args = ['nb_dimlp_nets', 'nb_ex_in_one']
+            optional_dimlpBT_args = ['nb_dimlp_nets', 'nb_ex_per_net']
 
             optional_svm_args = ['svm_K', 'C', 'kernel', 'degree', 'gamma', 'coef0', 'shrinking',
-                        'svm_tol', 'cache_size', 'svm_class_weight', 'svm_max_iter', 'decision_function_shape', 'break_ties']
+                        'svm_tol', 'cache_size', 'svm_class_weight', 'svm_max_iterations', 'decision_function_shape', 'break_ties']
 
             optional_mlp_args = ['mlp_K', 'hidden_layer_sizes', 'activation', 'solver', 'alpha',
-                        'batch_size', 'mlp_learning_rate', 'learning_rate_init', 'power_t', 'mlp_max_iter',
-                        'shuffle', 'mlp_tol', 'mlp_warm_start', 'momentum', 'nesterovs_momentum',
+                        'batch_size', 'mlp_learning_rate', 'learning_rate_init', 'power_t', 'mlp_max_iterations',
+                        'shuffle', 'mlp_tol', 'mlp_warm_start', 'mlp_momentum', 'nesterovs_momentum',
                         'early_stopping', 'mlp_validation_fraction', 'beta_1', 'beta_2', 'epsilon', 'mlp_n_iter_no_change', 'max_fun']
 
             optional_dt_args = ['n_estimators', 'min_samples_split', 'min_samples_leaf', 'min_weight_fraction_leaf',
                                             'max_features', 'min_impurity_decrease', 'max_leaf_nodes', 'dt_warm_start', 'ccp_alpha']
 
             optional_rf_args = ['rf_criterion', 'rf_max_depth', 'bootstrap', 'oob_score', 'n_jobs', 'rf_class_weight', 'max_samples']
 
             optional_gb_args = ['loss', 'gb_learning_rate', 'subsample', 'gb_criterion', 'gb_max_depth', 'init'
                                 , 'gb_validation_fraction', 'gb_n_iter_no_change', 'gb_tol']
 
             # Check if wrong parameters are given
 
             train_methods = {"dimlp", "dimlpBT", "svm", "mlp", "randForest", "gradBoost"}
             if train_method is None:
-                raise ValueError('Error : train method is missing, add it with option train_method="dimlp", "dimlpBT", "svm", "mlp", randForest or gradBoost')
+                raise ValueError('Error : train method is missing, add it with option train_method="dimlp", "dimlpBT", "svm", "mlp", randForest or gradBoost.')
             elif (train_method not in train_methods):
-                raise ValueError('Error, parameter train_method is not "dimlp", "dimlpBT", "svm", "mlp", "randForest" or "gradBoost"')
+                raise ValueError('Error, parameter train_method is not "dimlp", "dimlpBT", "svm", "mlp", "randForest" or "gradBoost".')
 
             for arg_key in kwargs.keys():
                 if (train_method == "dimlp"):
-                    if (arg_key not in optional_args and arg_key not in optional_non_dt_args and arg_key not in optional_dimlp_args and not(arg_key.startswith('H') and arg_key[1:].isdigit()) and arg_key not in obligatory_args and arg_key not in obligatory_dimlp_args):
-                        raise ValueError(f"Invalid argument with dimlp training : {arg_key}")
+                    if (arg_key not in optional_args and arg_key not in optional_non_dt_args and arg_key not in optional_dimlp_args and arg_key not in obligatory_args and arg_key not in obligatory_dimlp_args):
+                        raise ValueError(f"Invalid argument with dimlp training : {arg_key}.")
                 elif (train_method == "dimlpBT"):
-                    if (arg_key not in optional_args and arg_key not in optional_non_dt_args and arg_key  not in optional_dimlp_args and not(arg_key.startswith('H') and arg_key[1:].isdigit()) and arg_key not in obligatory_args and arg_key not in obligatory_dimlp_args and arg_key not in optional_dimlpBT_args):
-                        raise ValueError(f"Invalid argument with dimlpBT training : {arg_key}")
+                    if (arg_key not in optional_args and arg_key not in optional_non_dt_args and arg_key  not in optional_dimlp_args and arg_key not in obligatory_args and arg_key not in obligatory_dimlp_args and arg_key not in optional_dimlpBT_args):
+                        raise ValueError(f"Invalid argument with dimlpBT training : {arg_key}.")
                 elif (train_method == "svm"):
                     if (arg_key not in optional_args and arg_key not in optional_non_dt_args and arg_key not in optional_svm_args and arg_key not in obligatory_args):
-                        raise ValueError(f"Invalid argument with svm training : {arg_key}")
+                        raise ValueError(f"Invalid argument with svm training : {arg_key}.")
                 elif (train_method == "mlp"):
                     if (arg_key not in optional_args and arg_key not in optional_non_dt_args and arg_key not in optional_mlp_args and arg_key not in obligatory_args):
-                        raise ValueError(f"Invalid argument with mlp training : {arg_key}")
+                        raise ValueError(f"Invalid argument with mlp training : {arg_key}.")
                 elif (train_method == "randForest"):
                     if (arg_key not in optional_args and arg_key not in optional_dt_args and arg_key not in optional_rf_args and arg_key not in obligatory_args):
-                        raise ValueError(f"Invalid argument with random forest training : {arg_key}")
+                        raise ValueError(f"Invalid argument with random forest training : {arg_key}.")
                 else:
                     if (arg_key not in optional_args and arg_key not in optional_dt_args and arg_key not in optional_gb_args and arg_key not in obligatory_args):
-                        raise ValueError(f"Invalid argument with gradient boosting training : {arg_key}")
+                        raise ValueError(f"Invalid argument with gradient boosting training : {arg_key}.")
 
 
             algos = {"fidex", "fidexGlo", "both"}
             if algo is None:
-                raise ValueError('Error : algorithm(s) is missing, add it with option algo="fidex" or "fidexGlo" or "both"')
+                raise ValueError('Error : algorithm(s) is missing, add it with option algo="fidex" or "fidexGlo" or "both".')
             elif (algo not in algos):
-                raise ValueError('Error, parameter algo is not fidex, fidexGlo or both')
+                raise ValueError('Error, parameter algo is not fidex, fidexGlo or both.')
 
             if data_file is None:
-                raise ValueError('Error : data file is missing, add it with option data_file="your_data_file_name"')
+                raise ValueError('Error : data file is missing, add it with option data_file="your_data_file_name".')
             elif not isinstance(data_file, str):
                 raise ValueError('Error : parameter data_file has to be a name contained in quotation marks "".')
 
-            if class_file is None:
-                raise ValueError('Error : class file is missing, add it with option class_file="your_class_file_name"')
-            elif not isinstance(class_file, str):
-                raise ValueError('Error : parameter class_file has to be a name contained in quotation marks "".')
+            if nb_attributes is None:
+                raise ValueError('Error : the number of input neurons is missing, add it with option nb_attributes=your_number.')
+            elif (not isinstance(nb_attributes, int) or nb_attributes<=0):
+                raise ValueError('Error, parameter nb_attributes is not an strictly positive integer.')
+
+            if nb_classes is None:
+                raise ValueError('Error : the number of output neurons is missing, add it with option nb_classes=your_number.')
+            elif (not isinstance(nb_classes, int) or nb_classes<=0):
+                raise ValueError('Error, parameter nb_classes is not an strictly positive integer.')
+
+            # Check optional parameters
 
-            if (save_folder is not None and (not isinstance(save_folder, str))):
-                raise ValueError('Error, parameter save_folder has to be a name contained in quotation marks "".')
+            if (root_folder is not None and (not isinstance(root_folder, str))):
+                raise ValueError('Error, parameter root_folder has to be a name contained in quotation marks "".')
 
             if crossval_folder is None:
                 crossval_folder = "CrossValidation"
             elif not isinstance(crossval_folder, str):
                 raise ValueError('Error, parameter crossval_folder has to be a name contained in quotation marks "".')
 
             if k is None:
                 k = 10
             elif (not isinstance(k, int) or k<3):
-                raise ValueError('Error, parameter K is not an integer greater than 2')
+                raise ValueError('Error, parameter K is not an integer greater than 2.')
 
             if n is None:
                 n = 10
             elif (not isinstance(n, int) or n<1):
-                raise ValueError('Error, parameter n is not an stryctly positive integer')
+                raise ValueError('Error, parameter n is not an stryctly positive integer.')
 
             if fidexglo_heuristic is None:
                 fidexglo_heuristic = 1
             elif (fidexglo_heuristic not in {1,2,3}):
-                raise ValueError('Error, parameter fidexglo_heuristic is not 1, 2 or 3')
+                raise ValueError('Error, parameter fidexglo_heuristic is not 1, 2 or 3.')
 
             if crossval_stats is None:
                 crossval_stats = "crossValidationStats.txt"
             elif (not isinstance(crossval_stats, str)):
                 raise ValueError('Error, parameter crossval_stats has to be a name contained in quotation marks "".')
 
-            if (attr_file is not None and (not isinstance(attr_file, str))):
-                raise ValueError('Error, parameter attr_file has to be a name contained in quotation marks "".')
+            if (attributes_file is not None and (not isinstance(attributes_file, str))):
+                raise ValueError('Error, parameter attributes_file has to be a name contained in quotation marks "".')
+
+            with_roc = True
+            if positive_class_index is None:
+                with_roc = False
 
             if train_method not in {"randForest", "gradBoost"}:
-                if hiknot is None:
-                    hiknot = 5
-                if nb_stairs is None:
-                    nb_stairs = 50
-
-            if max_iter is None:
-                max_iter = 100
-            if min_cov is None:
-                min_cov = 2
+                if nb_quant_levels is None:
+                    nb_quant_levels = 50
+
+            if max_iterations is None:
+                max_iterations = 100
+            if min_covering is None:
+                min_covering = 2
+
+            if min_fidelity is None:
+                min_fidelity = 1.0
+            if lowest_min_fidelity is None:
+                lowest_min_fidelity = 0.75
+            if covering_strategy is None:
+                covering_strategy = True
 
             if seed is None:
                 seed = 0
             elif (not isinstance(seed, int) or seed<0):
-                raise ValueError('Error, parameter seed is not an positive integer')
+                raise ValueError('Error, parameter seed is not an positive integer.')
+
+            # Check dimlpBT parameters
 
             if train_method == "dimlpBT":
                 if nb_dimlp_nets is None:
                     nb_dimlp_nets = 25
                 elif not isinstance(nb_dimlp_nets, int) or nb_dimlp_nets < 2:
-                    raise ValueError('Error, parameter nb_dimlp_nets is not an integer greater than 1')
+                    raise ValueError('Error, parameter nb_dimlp_nets is not an integer greater than 1.')
 
-                if nb_ex_in_one is None :
-                    nb_ex_in_one = 0
-                elif not isinstance(nb_ex_in_one, int) or nb_ex_in_one < 0:
-                    raise ValueError('Error, parameter nb_ex_in_one is not a positive integer')
+                if nb_ex_per_net is None :
+                    nb_ex_per_net = 0
+                elif not isinstance(nb_ex_per_net, int) or nb_ex_per_net < 0:
+                    raise ValueError('Error, parameter nb_ex_per_net is not a positive integer.')
+
+            # Check dimlp and dimlpBT parameters
 
             if train_method in {"dimlp", "dimlpBT"}:
 
                 if dimlprul is None:
-                    raise ValueError('Error : dimlpRul is missing, add it with option dimlpRul=1 or 0')
+                    raise ValueError('Error : dimlpRul is missing, add it with option dimlpRul=1 or 0.')
                 elif (dimlprul not in {0,1}):
-                    raise ValueError('Error, parameter dimlpRul is not 1 or 0')
-
-                if nb_in is None:
-                    raise ValueError('Error : the number of input neurons is missing, add it with option nb_in=your_number')
-                elif (not isinstance(nb_in, int) or nb_in<=0):
-                    raise ValueError('Error, parameter nb_in is not an strictly positive integer')
-
-                if nb_out is None:
-                    raise ValueError('Error : the number of output neurons is missing, add it with option nb_out=your_number')
-                elif (not isinstance(nb_out, int) or nb_out<=0):
-                    raise ValueError('Error, parameter nb_out is not an strictly positive integer')
+                    raise ValueError('Error, parameter dimlpRul is not 1 or 0.')
 
                 if (pretrained_weights is not None and (not isinstance(pretrained_weights, str))):
                     raise ValueError('Error, parameter pretrained_weights has to be a name contained in quotation marks "".')
 
-                if eta is None:
-                    eta = 0.1
-                if mu is None:
-                    mu = 0.6
+                if learning_rate is None:
+                    learning_rate = 0.1
+                if momentum is None:
+                    momentum = 0.6
                 if flat is None:
                     flat = 0.01
-                if err_thresh is None:
-                    err_thresh = -1111111111.0
+                if error_thresh is None:
+                    error_thresh = -1111111111.0
                 if acc_thresh is None:
                     acc_thresh = 11111111111111.0
-                if delta_err is None:
-                    delta_err = 0
+                if abs_error_thresh is None:
+                    abs_error_thresh = 0
                 if nb_epochs is None:
                     nb_epochs = 1500
-                if show_err is None:
-                    show_err = 10
+                if nb_epochs_error is None:
+                    nb_epochs_error = 10
 
-            elif train_method == "svm":
-                if svm_k is None:
-                    svm_k = 1
-                if c_var is None:
-                    c_var = 1.0
-                if kernel_var is None:
-                    kernel_var = "rbf"
-                if degree_var is None:
-                    degree_var = 3
-                if gamma_var is None:
-                    gamma_var = "scale"
-                if coef0_var is None:
-                    coef0_var = 0
-                if shrinking_var is None:
-                    shrinking_var = True
-                if svm_tol_var is None:
-                    svm_tol_var = 0.001
-                if cache_size_var is None:
-                    cache_size_var = 200
-                if svm_max_iter_var is None:
-                    svm_max_iter_var = -1
-                if decision_function_shape_var is None:
-                    decision_function_shape_var = "ovr"
-                if break_ties_var is None:
-                    break_ties_var = False
-
-            elif train_method == "mlp":
-                if mlp_k is None:
-                    mlp_k = 1
-                if hidden_layer_sizes_var is None:
-                    hidden_layer_sizes_var = (100,)
-                if activation_var is None:
-                    activation_var = "relu"
-                if solver_var is None:
-                    solver_var = "adam"
-                if alpha_var is None:
-                    alpha_var = 0.0001
-                if batch_size_var is None:
-                    batch_size_var = "auto"
-                if mlp_learning_rate_var is None:
-                    mlp_learning_rate_var = "constant"
-                if learning_rate_init_var is None:
-                    learning_rate_init_var = 0.001
-                if power_t_var is None:
-                    power_t_var = 0.5
-                if mlp_max_iter_var is None:
-                    mlp_max_iter_var = 200
-                if shuffle_var is None:
-                    shuffle_var = True
-                if mlp_tol_var is None:
-                    mlp_tol_var = 0.0001
-                if mlp_warm_start_var is None:
-                    mlp_warm_start_var = False
-                if momentum_var is None:
-                    momentum_var = 0.9
-                if nesterovs_momentum_var is None:
-                    nesterovs_momentum_var = True
-                if early_stopping_var is None:
-                    early_stopping_var = False
-                if mlp_validation_fraction_var is None:
-                    mlp_validation_fraction_var = 0.1
-                if beta_1_var is None:
-                    beta_1_var = 0.9
-                if beta_2_var is None:
-                    beta_2_var = 0.999
-                if epsilon_var is None:
-                    epsilon_var = 0.00000001
-                if mlp_n_iter_no_change_var is None:
-                    mlp_n_iter_no_change_var = 10
-                if max_fun_var is None:
-                    max_fun_var = 15000
+            # Check decision trees parameters
 
             else:
                 if n_estimators_var is None:
                     n_estimators_var = 100
 
                 if min_samples_split_var is None:
                     min_samples_split_var = 2
@@ -647,24 +597,27 @@
 
                 if dt_warm_start_var is None:
                     dt_warm_start_var = False
 
                 if ccp_alpha_var is None:
                     ccp_alpha_var = 0.0
 
+                # Check Random forests parameters
+
                 if train_method == "randForest":
                     if rf_criterion_var is None:
                         rf_criterion_var = "gini"
 
                     if bootstrap_var is None:
                         bootstrap_var = True
 
                     if oob_score_var is None:
                         oob_score_var = False
 
+                # Check Gradient boosting parameters
                 else:
                     if loss_var is None:
                         loss_var = "log_loss"
 
                     if gb_learning_rate_var is None:
                         gb_learning_rate_var = 0.1
 
@@ -698,33 +651,38 @@
             #create paths with root foler
             system = platform.system()
             if system == "Linux" or system == "Darwin":
                 separator = "/"
             elif system == "Windows":
                 separator = "\\"
 
-            if save_folder is not None:
-                root = save_folder + separator
+            if root_folder is not None:
+                root = root_folder + separator
             else:
                 root = ""
 
             data_file = root + data_file
-            class_file = root + class_file
             crossval_folder_temp = crossval_folder
             crossval_folder = root + crossval_folder
             crossval_stats = crossval_folder + separator + crossval_stats
 
             # Get datas in a list
-            datas = get_data(data_file)
+            datas, classes = get_data(data_file, nb_attributes, nb_classes)
+            if len(classes) == 0:
+                if class_file is None:
+                    raise ValueError('Error: class_file missing, add it with option class_file="your_class_file".')
+                elif not isinstance(class_file, str):
+                    raise ValueError('Error: parameter class_file has to be a name contained in quotation marks "".')
+                class_file = root + class_file
+                classes = get_data_class(class_file, nb_classes)
+
             nb_samples = len(datas)
             if k > nb_samples:
                 raise ValueError(f'The number of divisions K of the dataset must be less or equal to the number of train samples({nb_samples}).')
 
-            classes = get_data(class_file)
-
             if len(classes) != nb_samples:
                 raise ValueError('The number of samples in data file and class file need to be the same.')
 
 
             # Create folder if doesn't exist
             create_or_clear_directory(crossval_folder)
 
@@ -738,80 +696,72 @@
             temp_train_file= crossval_folder + separator + "tempTrain.txt"
             temp_test_file = crossval_folder + separator + "tempTest.txt"
             temp_valid_file = crossval_folder + separator + "tempValid.txt"
             temp_train_tar_file = crossval_folder + separator + "tempTarTrain.txt"
             temp_test_tar_file = crossval_folder + separator + "tempTarTest.txt"
             temp_valid_tar_file = crossval_folder + separator + "tempTarValid.txt"
 
+
+            # Statistics initialization
+
+            mean_fprs = [] #false positive rates for ROC curve
+            mean_tprs = [] #true positive rates for ROC curve
+            mean_aucs = []
+
             if is_fidex:
                 # statistics for Fidex
-                # One execution
                 mean_cov_size_fid = 0.0
                 mean_nb_ant_fid = 0.0
                 mean_fidel_fid = 0.0
                 mean_rules_acc_fid = 0.0
                 mean_confid_fid = 0.0
 
-                # All executions
-                mean_cov_size_fid_all = 0.0
-                mean_nb_ant_fid_all = 0.0
-                mean_fidel_fid_all = 0.0
-                mean_rules_acc_fid_all = 0.0
-                mean_confid_fid_all = 0.0
-
-                std_cov_size_fid_all = 0.0
-                std_nb_ant_fid_all = 0.0
-                std_fidel_fid_all = 0.0
-                std_rules_acc_fid_all = 0.0
-                std_confid_fid_all = 0.0
-
                 mean_exec_values_fidex = [] # each mean value in an entire fold for each fold for fidex
 
             if is_fidexglo:
                 # Statistics for FidexGlo
-                # One execution
                 mean_nb_rules = 0.0
                 mean_nb_cover = 0.0
                 mean_nb_antecedants = 0.0
                 mean_fidel_glo = 0.0
                 mean_rules_acc_glo = 0.0
                 mean_expl_glo = 0.0
                 mean_default_rate = 0.0
                 mean_nb_fidel_activations = 0.0
                 mean_wrong_activations = 0.0
                 mean_test_acc_glo = 0.0
                 mean_test_acc_when_rules_and_model_agree = 0.0
                 mean_test_acc_when_activated_rules_and_model_agree = 0.0
 
-                # All executions
-                mean_nb_rules_all = 0.0
-                mean_nb_cover_all = 0.0
-                mean_nb_antecedants_all = 0.0
-                mean_fidel_glo_all = 0.0
-                mean_rules_acc_glo_all = 0.0
-                mean_expl_glo_all = 0.0
-                mean_default_rate_all = 0.0
-                mean_nb_fidel_activations_all = 0.0
-                mean_wrong_activations_all = 0.0
-                mean_test_acc_glo_all = 0.0
-                mean_test_acc_when_rules_and_model_agree_all = 0.0
-                mean_test_acc_when_activated_rules_and_model_agree_all = 0.0
-
-                std_nb_rules_all = 0.0
-                std_nb_cover_all = 0.0
-                std_nb_antecedants_all = 0.0
-                std_fidel_glo_all = 0.0
-                std_rules_acc_glo_all = 0.0
-                std_expl_glo_all = 0.0
-                std_default_rate_all = 0.0
-                std_nb_fidel_activations_all = 0.0
-                std_wrong_activations_all = 0.0
-                std_test_acc_glo_all = 0.0
-                std_test_acc_when_rules_and_model_agree_all = 0.0
-                std_test_acc_when_activated_rules_and_model_agree_all = 0.0
+                if with_roc:
+                    mean_nb_true_positive = 0
+                    mean_nb_false_positive = 0
+                    mean_nb_true_negative = 0
+                    mean_nb_false_negative = 0
+                    mean_false_positive_rate = 0.0
+                    mean_false_negative_rate = 0.0
+                    mean_precision = 0.0
+                    mean_recall = 0.0
+                    nb_no_false_positive_rate = 0.0
+                    nb_no_false_negative_rate = 0.0
+                    nb_no_precision = 0.0
+                    nb_no_recall = 0.0
+
+                    mean_nb_true_positive_rule = 0
+                    mean_nb_false_positive_rule = 0
+                    mean_nb_true_negative_rule = 0
+                    mean_nb_false_negative_rule = 0
+                    mean_false_positive_rate_rule = 0.0
+                    mean_false_negative_rate_rule = 0.0
+                    mean_precision_rule = 0.0
+                    mean_recall_rule = 0.0
+                    nb_no_false_positive_rate_rule = 0.0
+                    nb_no_false_negative_rate_rule = 0.0
+                    nb_no_precision_rule = 0.0
+                    nb_no_recall_rule = 0.0
 
                 mean_exec_values_fidexglo = [] # each mean value in an entire fold for each fold for fidexGlo
 
             if is_dimlprul:
                 # Statistics for Dimlp Rules
                 # One execution
                 mean_nb_rules_dimlp = 0.0
@@ -829,57 +779,53 @@
                 mean_nb_antecedants_dimlp_all = 0.0
                 mean_fidel_dimlp_all = 0.0
                 mean_rules_acc_dimlp_all = 0.0
                 mean_default_rate_dimlp_all = 0.0
                 mean_test_acc_dimlp_all = 0.0
                 mean_test_acc_when_rules_and_model_agree_dimlp_all = 0.0
 
-                std_nb_rules_dimlp_all = 0.0
-                std_nb_cover_dimlp_all = 0.0
-                std_nb_antecedants_dimlp_all = 0.0
-                std_fidel_dimlp_all = 0.0
-                std_rules_acc_dimlp_all = 0.0
-                std_default_rate_dimlp_all = 0.0
-                std_test_acc_dimlp_all = 0.0
-                std_test_acc_when_rules_and_model_agree_dimlp_all = 0.0
-
                 mean_exec_values_dimlp = []
 
                 nb_no_rules_dimlp = 0.0 # If there is no rule found for a Fold
 
 
             # Write parameters on stats file
 
             try:
                 with open(crossval_stats, "w") as outputStatsFile:
 
                     outputStatsFile.write(f"Parameters for {n} times {k}-Cross validation :\n")
                     outputStatsFile.write(f"Training with {train_method}\n")
                     outputStatsFile.write("---------------------------------------------------------\n")
+                    if train_method not in {"dimlp", "dimlpBT"}:
+                        outputStatsFile.write(f"There are {nb_attributes} attributes and {nb_classes} classes\n")
                     if train_method in {"dimlp", "dimlpBT"}:
-                        outputStatsFile.write(f"Training with {nb_in} input neurons and {nb_out} output neurons\n")
-                        for key, value in hk.items():
-                            outputStatsFile.write(f"Layer {key} has {value} neurons\n")
+                        outputStatsFile.write(f"Training with {nb_attributes} input neurons and {nb_classes} output neurons\n")
+                        if first_hidden_layer is not None:
+                            outputStatsFile.write(f"Layer 1 has {first_hidden_layer} neurons\n")
+                        if hidden_layers is not None:
+                            for key,value in enumerate(hidden_layers):
+                                outputStatsFile.write(f"Layer {key+2} has {value} neurons\n")
                     if train_method not in {"randForest", "gradBoost"}:
-                        outputStatsFile.write(f"The number of stairs in staircase activation function is {nb_stairs} and the interval in which hyperplans are contained is [-{hiknot},{hiknot}]\n")
+                        outputStatsFile.write(f"The number of stairs in staircase activation function is {nb_quant_levels} and the interval in which hyperplans are contained is [-{hiknot},{hiknot}]\n")
                     if train_method == "dimlpBT":
                         outputStatsFile.write(f"The number of dimlp networks is {nb_dimlp_nets}\n")
-                        if nb_ex_in_one == 0:
+                        if nb_ex_per_net == 0:
                             outputStatsFile.write("The number of examples for one single network is the number of train examples\n")
                         else:
-                            outputStatsFile.write(f"The number of examples for one single network is {nb_ex_in_one} (but not more than the number of train examples)\n")
+                            outputStatsFile.write(f"The number of examples for one single network is {nb_ex_per_net} (but not more than the number of train examples)\n")
                     if train_method in {"dimlp", "dimlpBT"}:
-                        outputStatsFile.write(f"The back-propagation learning parameter (Eta) is {eta}\n")
-                        outputStatsFile.write(f"The back-propagation momentum parameter (Mu) is {mu}\n")
+                        outputStatsFile.write(f"The back-propagation learning parameter (Eta) is {learning_rate}\n")
+                        outputStatsFile.write(f"The back-propagation momentum parameter (Mu) is {momentum}\n")
                         outputStatsFile.write(f"The back-propagation flat spot elimination parameter (Flat) is {flat}\n")
-                        outputStatsFile.write(f"The error threshold is {err_thresh}\n")
+                        outputStatsFile.write(f"The error threshold is {error_thresh}\n")
                         outputStatsFile.write(f"The accuracy threshold is {acc_thresh}\n")
-                        outputStatsFile.write(f"The absolute difference error threshold is {delta_err}\n")
+                        outputStatsFile.write(f"The absolute difference error threshold is {abs_error_thresh}\n")
                         outputStatsFile.write(f"The number of train epochs is {nb_epochs}\n")
-                        outputStatsFile.write(f"The number of train epochs to show error is {show_err}\n")
+                        outputStatsFile.write(f"The number of train epochs to show error is {nb_epochs_error}\n")
                     elif train_method == "svm":
                         outputStatsFile.write(f"The K parameter to improve dynamics is {svm_k}\n")
                         outputStatsFile.write(f"The regularization parameter C is {c_var}\n")
                         outputStatsFile.write(f"The kernel is {kernel_var}\n")
                         if kernel_var == "poly":
                             outputStatsFile.write(f"The polynomial degree is {degree_var}\n")
                         if kernel_var in {"rbf", "poly", "sigmoid"}:
@@ -891,18 +837,18 @@
                         else:
                             outputStatsFile.write("No using of the shrinking heuristic\n")
                         outputStatsFile.write(f"The tolerance for stopping criterion is {svm_tol_var}\n")
                         if svm_class_weight_var == None:
                             outputStatsFile.write("Class weights are unchanged\n")
                         else:
                             outputStatsFile.write(f"Class weights are {svm_class_weight_var}\n")
-                        if svm_max_iter_var == -1:
+                        if svm_max_iterations_var == -1:
                             outputStatsFile.write("There is no limit in the number of iterations\n")
                         else:
-                            outputStatsFile.write(f"The maximal number of iterations is {svm_max_iter_var}\n")
+                            outputStatsFile.write(f"The maximal number of iterations is {svm_max_iterations_var}\n")
                         if decision_function_shape_var == "ovr":
                             outputStatsFile.write("The decision function shape is one-vs-rest\n")
                             if break_ties_var:
                                 outputStatsFile.write("Using break tie decision\n")
                         else:
                             outputStatsFile.write("The decision function shape is one-vs-one\n")
                     elif train_method == "mlp":
@@ -915,22 +861,22 @@
                             outputStatsFile.write(f"The batch size is {alpha_var}\n")
                         if solver_var =="sgd":
                             outputStatsFile.write(f"The learning rate is {mlp_learning_rate_var}\n")
                         if solver_var in {"adam", "sgd"}:
                             outputStatsFile.write(f"The initial learning rate is {learning_rate_init_var}\n")
                         if solver_var =="sgd":
                             outputStatsFile.write(f"The power_t exponent for inverse scaling learning rate is {power_t_var}\n")
-                        outputStatsFile.write(f"The maximum number of iterations is {mlp_max_iter_var}\n")
+                        outputStatsFile.write(f"The maximum number of iterations is {mlp_max_iterations_var}\n")
                         if solver_var in {"adam", "sgd"} and shuffle_var == True:
                             outputStatsFile.write("Samples are shuffled in each iteration")
                         outputStatsFile.write(f"The tolerance for optimization is {mlp_tol_var}\n")
                         if mlp_warm_start_var == True:
                             outputStatsFile.write("Previous solution is reused to fit initialization")
                         if solver_var =="sgd":
-                            outputStatsFile.write(f"The momentum for gradient descent update is {momentum_var}\n")
+                            outputStatsFile.write(f"The momentum for gradient descent update is {mlp_momentum_var}\n")
                             if nesterovs_momentum_var == True:
                                 outputStatsFile.write("Using Nesterov’s momentum")
                         if solver_var in {"adam", "sgd"} and early_stopping_var == True:
                             outputStatsFile.write("Using early stopping")
                             outputStatsFile.write(f"The proportion of training data to set aside as validation set is {mlp_validation_fraction_var}\n")
                         if solver_var =="adam":
                             outputStatsFile.write(f"Exponential decay rate for estimates of first moment vector is {beta_1_var}\n")
@@ -1012,37 +958,43 @@
                                 outputStatsFile.write("Special zero estimator is used\n")
                             if gb_n_iter_no_change_var is None:
                                 outputStatsFile.write("Early stopping is disabled\n")
                             else:
                                 outputStatsFile.write(f"Stopping if validation score doesn't improve during {gb_n_iter_no_change_var} iterations\n")
                                 outputStatsFile.write(f"The proportion of training data to set aside as validation set for early stopping is {gb_validation_fraction_var} \n")
                                 outputStatsFile.write(f"The tolerance for the early stopping is {gb_tol_var} \n")
-                    outputStatsFile.write(f"The max fidex and fidexGlo iteration number is {max_iter}\n")
-                    outputStatsFile.write(f"The minimum fidex and fidexGlo covering number is {min_cov}\n")
+                    outputStatsFile.write(f"The max fidex and fidexGlo iteration number is {max_iterations}\n")
+                    outputStatsFile.write(f"The minimum fidex and fidexGlo covering number is {min_covering}\n")
+                    outputStatsFile.write(f"The minimum fidex and fidexGlo accepted fidelity is {min_fidelity}\n")
+                    if covering_strategy:
+                        outputStatsFile.write("The covering strategy is set\n")
+                        outputStatsFile.write(f"The minimum fidex and fidexGlo accepted fidelity during covering strategy is {lowest_min_fidelity}\n")
                     if is_fidexglo:
                         outputStatsFile.write(f"The fidexGlo heuristic is {fidexglo_heuristic}\n")
                     if dropout_hyp:
                         outputStatsFile.write(f"The hyperplan dropout parameter for fidex and fidexGlo is {dropout_hyp}\n")
                     else:
                         outputStatsFile.write("There is no hyperplan dropout\n")
                     if dropout_dim:
                         outputStatsFile.write(f"The dimension dropout parameter for fidex and fidexGlo is {dropout_dim}\n")
                     else:
                         outputStatsFile.write("There is no dimension dropout\n")
+                    if decision_threshold is not None :
+                        outputStatsFile.write(f"We use a decision threshold of {decision_threshold} with positive class of index {positive_class_index}\n")
+                    if normalization_file is not None or normalization_indices is not None:
+                        outputStatsFile.write("We denormalize the rules\n")
 
                     outputStatsFile.write("---------------------------------------------------------\n\n")
 
                     outputStatsFile.close()
             except (FileNotFoundError):
                 raise ValueError(f"Error : File for stats extraction ({crossval_stats}) not found.")
             except (IOError):
                 raise ValueError(f"Error : Couldn't open stats extraction file {crossval_stats}.")
 
-            has_confidence = True # Check if we have confidence statistics
-
             # Loop on N executions of cross-validation
             for ni in range(n):
                 print(f"n={ni+1}")
 
                 #  Create folder for this execution
                 if system == "Linux" or system == "Darwin":
                     folder_name = crossval_folder + "/Execution" + str(ni+1) + "/"
@@ -1073,14 +1025,18 @@
                     temp_vect = [datas[indexes[ind]] for ind in range(start, end)]
                     temp_vect_tar = [classes[indexes[ind]] for ind in range(start, end)]
                     data_split.append(temp_vect)
                     tar_data_split.append(temp_vect_tar)
 
                 nb_no_rules_current_exec_dimlp = 0.0 # If there is no rule found for a Fold in this execution
 
+                fprs = [] #false positive rates for ROC curve
+                tprs = [] #true positive rates for ROC curve
+                aucs = []
+
                 for ki in range(k): # K-fold, we shift each time groups by 1.
                     print("----")
                     print(f"k={ki+1}")
 
                     #  Create folder for this fold
                     folder_path = crossval_folder + separator + "Execution" + str(ni+1) + separator + "Fold" + str(ki+1)
                     if system == "Linux" or system == "Darwin":
@@ -1101,62 +1057,68 @@
                     if train_method in {"dimlpBT", "svm", "mlp", "randForest", "gradBoost"}: # There is no validation data to be provided to tune hyperparameters
                         train_idx.append(validation_idx)
 
                     # Creation of train, test and validation files (temp files)
                     try:
                         with open(temp_train_file, "w") as trn_file:
                             for id in train_idx:
-                                for line_trn in data_split[id]:
-                                    trn_file.write(f"{line_trn}\n")
+                                for sample_trn in data_split[id]:
+                                    for attr in sample_trn:
+                                        trn_file.write(f"{str(attr)} ")
+                                    trn_file.write("\n")
                         trn_file.close()
 
                     except (IOError):
                         raise ValueError(f"Error : Couldn't open file {temp_train_file}.")
 
                     try:
                         with open(temp_test_file, "w") as tst_file:
-                            for line_tst in data_split[test_idx]:
-                                tst_file.write(f"{line_tst}\n")
+                            for sample_tst in data_split[test_idx]:
+                                for attr in sample_tst:
+                                    tst_file.write(f"{str(attr)} ")
+                                tst_file.write("\n")
                         tst_file.close()
 
                     except (IOError):
                         raise ValueError(f"Error : Couldn't open file {temp_test_file}.")
                     if train_method == "dimlp":
                         try:
                             with open(temp_valid_file, "w") as val_file:
-                                for line_val in data_split[validation_idx]:
-                                    val_file.write(f"{line_val}\n")
+                                for sample_val in data_split[validation_idx]:
+                                    for attr in sample_val:
+                                        val_file.write(f"{str(attr)} ")
+                                    val_file.write("\n")
                             val_file.close()
 
                         except (IOError):
                             raise ValueError(f"Error : Couldn't open file {temp_valid_file}.")
 
                     try:
                         with open(temp_train_tar_file, "w") as trn_val_file:
                             for id in train_idx:
                                 for line_trn_tar in tar_data_split[id]:
-                                    trn_val_file.write(f"{line_trn_tar}\n")
+                                    trn_val_file.write(f"{int(line_trn_tar)} \n")
                         trn_val_file.close()
 
                     except (IOError):
                         raise ValueError(f"Error : Couldn't open file {temp_train_tar_file}.")
 
                     try:
                         with open(temp_test_tar_file, "w") as tst_tar_file:
                             for line_tst_tar in tar_data_split[test_idx]:
-                                tst_tar_file.write(f"{line_tst_tar}\n")
+                                tst_tar_file.write(f"{int(line_tst_tar)} \n")
                         tst_tar_file.close()
 
                     except (IOError):
                         raise ValueError(f"Error : Couldn't open file {temp_test_tar_file}.")
                     if train_method == "dimlp":
                         try:
                             with open(temp_valid_tar_file, "w") as val_tar_file:
                                 for line_val_tar in tar_data_split[validation_idx]:
-                                    val_tar_file.write(f"{line_val_tar}\n")
+                                    val_tar_file.write(f"{int(line_val_tar)} \n")
                             val_tar_file.close()
 
                         except (IOError):
                             raise ValueError(f"Error : Couldn't open file {temp_valid_tar_file}.")
 
                     # Get train, test and validation files in folder
 
@@ -1196,145 +1158,176 @@
                     # Training with dimlp
                     folder_path_from_root = str(crossval_folder_temp) + separator + "Execution" + str(ni + 1) + separator + "Fold" + str(ki + 1)
                     if train_method in {"dimlp", "dimlpBT"}:
                         if train_method == "dimlp":
                             dimlp_command = "dimlpTrn"
                         else:
                             dimlp_command = "dimlpBT"
-                            dimlp_command += " -N " + str(nb_dimlp_nets)
-                            dimlp_command += " -n " + str(nb_ex_in_one)
+                            dimlp_command += " --nb_dimlp_nets " + str(nb_dimlp_nets)
+                            dimlp_command += " --nb_ex_per_net " + str(nb_ex_per_net)
 
-                        dimlp_command += " -l " + str(eta)
-                        dimlp_command += " -m " + str(mu)
-                        dimlp_command += " -f " + str(flat)
-                        dimlp_command += " -e " + str(err_thresh)
-                        dimlp_command += " -a " + str(acc_thresh)
-                        dimlp_command += " -d " + str(delta_err)
-                        dimlp_command += " -s " + str(show_err)
-                        dimlp_command += " -i " + str(nb_epochs)
-                        dimlp_command += " -I " + str(nb_in)
-                        dimlp_command += " -O " + str(nb_out)
-                        if save_folder is not None:
-                            dimlp_command += " -S " + save_folder
-                        if attr_file is not None:
-                            dimlp_command += " -A " + attr_file
+                        dimlp_command += " --learning_rate " + str(learning_rate)
+                        dimlp_command += " --momentum " + str(momentum)
+                        dimlp_command += " --flat " + str(flat)
+                        dimlp_command += " --error_thresh " + str(error_thresh)
+                        dimlp_command += " --acc_thresh " + str(acc_thresh)
+                        dimlp_command += " --abs_error_thresh " + str(abs_error_thresh)
+                        dimlp_command += " --nb_epochs_error " + str(nb_epochs_error)
+                        dimlp_command += " --nb_epochs " + str(nb_epochs)
+                        dimlp_command += " --nb_attributes " + str(nb_attributes)
+                        dimlp_command += " --nb_classes " + str(nb_classes)
+                        if root_folder is not None:
+                            dimlp_command += " --root_folder " + root_folder
+                        if attributes_file is not None:
+                            dimlp_command += " --attributes_file " + attributes_file
                         if pretrained_weights is not None:
-                            dimlp_command += " -W " + pretrained_weights
-                        dimlp_command += " -z " + str(seed)
-                        dimlp_command += " -q " + str(nb_stairs)
-                        for key, value in hk.items():
-                            dimlp_command += " -" + key + " " + str(value)
-
-                        dimlp_command += " -L " + folder_path_from_root + separator + "train.txt "
-                        dimlp_command += "-T " + folder_path_from_root + separator + "test.txt "
-                        dimlp_command += "-1 " + folder_path_from_root + separator + "trainTarget.txt "
-                        dimlp_command += "-2 " + folder_path_from_root + separator + "testTarget.txt "
-
-                        dimlp_command += "-p " + folder_path_from_root + separator + "train.out "   # Output train pred file
-                        dimlp_command += "-t " + folder_path_from_root + separator + "test.out "    # Output test pred file
-                        dimlp_command += "-o " + folder_path_from_root + separator + "stats.txt "    # Output stats file
+                            dimlp_command += " --weights_file " + pretrained_weights
+                        dimlp_command += " --seed " + str(seed)
+                        dimlp_command += " --nb_quant_levels " + str(nb_quant_levels)
+                        if first_hidden_layer is not None:
+                            dimlp_command += " --first_hidden_layer " + str(first_hidden_layer)
+                        if hidden_layers is not None:
+                            dimlp_command += " --hidden_layers [" + ", ".join(str(value) for value in hidden_layers) + "]"
+
+                        dimlp_command += " --train_data_file " + folder_path_from_root + separator + "train.txt "
+                        dimlp_command += "--test_data_file " + folder_path_from_root + separator + "test.txt "
+                        dimlp_command += "--train_class_file " + folder_path_from_root + separator + "trainTarget.txt "
+                        dimlp_command += "--test_class_file " + folder_path_from_root + separator + "testTarget.txt "
+
+                        dimlp_command += "--train_pred_outfile " + folder_path_from_root + separator + "train.out "   # Output train pred file
+                        dimlp_command += "--test_pred_outfile " + folder_path_from_root + separator + "test.out "    # Output test pred file
+                        dimlp_command += "--stats_file " + folder_path_from_root + separator + "stats.txt "    # Output stats file
+                        dimlp_command += "--hidden_layers_outfile " + folder_path_from_root + separator + "hidden_layers.out "    # Output hidden layers file
 
                         if train_method == "dimlp":
-                            dimlp_command += "-V " + folder_path_from_root + separator + "valid.txt "
-                            dimlp_command += "-3 " + folder_path_from_root + separator + "validTarget.txt "
-                            dimlp_command += "-v " + folder_path_from_root + separator + "valid.out "   # Output validation pred file
-                            dimlp_command += "-w " + folder_path_from_root + separator + "weights.wts " # Output weight file
+                            dimlp_command += "--valid_data_file " + folder_path_from_root + separator + "valid.txt "
+                            dimlp_command += "--valid_class_file " + folder_path_from_root + separator + "validTarget.txt "
+                            dimlp_command += "--valid_pred_outfile " + folder_path_from_root + separator + "valid.out "   # Output validation pred file
+                            dimlp_command += "--weights_outfile " + folder_path_from_root + separator + "weights.wts " # Output weight file
                         else:
-                            dimlp_command += "-w " + folder_path_from_root + separator + "weightsBT " # Output weight generic filename
+                            dimlp_command += "--weights_outfile " + folder_path_from_root + separator + "weights.wts " # Output weight filename
 
                         if is_dimlprul:
-                            dimlp_command += "-R -F " + folder_path_from_root + separator + "dimlpRules.rls "
+                            dimlp_command += "--with_rule_extraction true --global_rules_outfile " + folder_path_from_root + separator + "dimlpRules.rls "
+
+                        if normalization_file is not None:
+                            dimlp_command += "--normalization_file " + normalization_file + " "
+                        if mus is not None:
+                            dimlp_command += "--mus " + mus + " "
+                        if sigmas is not None:
+                            dimlp_command += "--sigmas " + sigmas + " "
+                        if normalization_indices is not None:
+                            dimlp_command += "--normalization_indices " + normalization_indices + " "
 
-                        dimlp_command += "-r " + str(crossval_folder_temp) + separator + "consoleTemp.txt" # To not show console result
+                        dimlp_command += "--console_file " + str(crossval_folder_temp) + separator + "consoleTemp.txt" # To not show console result
 
                         if train_method == "dimlp":
-                            print("Enter in DimlpTrn function")
+                            print("Enter in dimlpTrn function")
                             res = dimlp.dimlpTrn(dimlp_command)
                         else:
-                            print("Enter in DimlpBT function")
+                            print("Enter in dimlpBT function")
                             res = dimlp.dimlpBT(dimlp_command)
                         if (res == -1):
-                            return -1 # If there is an error in the Trn
+                            raise ValueError('Error during training with Dimlp or dimlpBT.')
 
                     # Training with svm
                     elif train_method == "svm":
                         print("Enter in svmTrn function")
-                        res = svmTrn(train_data=folder_path_from_root + separator + "train.txt",train_class=folder_path_from_root + separator + "trainTarget.txt",
-                                     test_data=folder_path_from_root + separator + "test.txt",test_class=folder_path_from_root + separator + "testTarget.txt",
-                                     weights = folder_path_from_root + separator + "weights", stats = folder_path_from_root + separator + "stats.txt",
-                                     output_file = crossval_folder_temp + separator + "consoleTemp.txt", train_pred = folder_path_from_root + separator + "train",
-                                     test_pred = folder_path_from_root + separator + "test", save_folder = save_folder, nb_stairs = nb_stairs, hiknot = hiknot,
-                                     K = svm_k, C = c_var, kernel = kernel_var, degree = degree_var, gamma = gamma_var, coef0 = coef0_var, shrinking = shrinking_var,
-                                     tol = svm_tol_var, cache_size = cache_size_var, class_weight = svm_class_weight_var, max_iter = svm_max_iter_var,
-                                     decision_function_shape = decision_function_shape_var, break_ties = break_ties_var)
+                        return_roc_var = False
+                        if with_roc:
+                            return_roc_var = True
+                        res = svmTrn(f"--train_data_file {folder_path_from_root + separator + 'train.txt'} --train_class_file {folder_path_from_root + separator + 'trainTarget.txt'} "
+                                     f"--test_data_file {folder_path_from_root + separator + 'test.txt'} --test_class_file {folder_path_from_root + separator + 'testTarget.txt'} "
+                                     f"--weights_outfile {folder_path_from_root + separator + 'weights.wts'} --stats_file {folder_path_from_root + separator + 'stats.txt'} --nb_attributes {nb_attributes} "
+                                     f"--nb_classes {nb_classes} --console_file {crossval_folder_temp + separator + 'consoleTemp.txt'} --train_pred_outfile {folder_path_from_root + separator + 'train.out'} "
+                                     f"--test_pred_outfile {folder_path_from_root + separator + 'test.out'} --positive_class_index {positive_class_index} "
+                                     f"--output_roc {folder_path_from_root + separator + 'ROC_curve'} --root_folder {root_folder} --nb_quant_levels {nb_quant_levels} "
+                                     f"--K {svm_k} --C {c_var} --kernel {kernel_var} --degree {degree_var} --gamma {gamma_var} --coef0 {coef0_var} --shrinking {shrinking_var} "
+                                     f"--tol {svm_tol_var} --cache_size {cache_size_var} --class_weight {svm_class_weight_var} --max_iterations {svm_max_iterations_var} "
+                                     f"--decision_function_shape {decision_function_shape_var} --break_ties {break_ties_var} --return_roc {return_roc_var}")
 
                         if (res == -1):
-                            return -1 # If there is an error in the Trn
+                            raise ValueError('Error during training with SVM.')
+                        elif with_roc:
+                            fprs.append(res[0])
+                            tprs.append(res[1])
+                            aucs.append(res[2])
 
                     # Training with mlp
                     elif train_method == "mlp":
                         print("Enter in mlpTrn function")
-                        random_state_var = seed
+                        seed_var = seed
                         if seed == 0:
-                            random_state_var = None
-                        res = mlpTrn(train_data=folder_path_from_root + separator + "train.txt",train_class=folder_path_from_root + separator + "trainTarget.txt",
-                                     test_data=folder_path_from_root + separator + "test.txt",test_class=folder_path_from_root + separator + "testTarget.txt",
-                                     weights = folder_path_from_root + separator + "weights", stats = folder_path_from_root + separator + "stats.txt",
-                                     output_file = crossval_folder_temp + separator + "consoleTemp.txt", train_pred = folder_path_from_root + separator + "train",
-                                     test_pred = folder_path_from_root + separator + "test", save_folder = save_folder, nb_stairs = nb_stairs, hiknot = hiknot,
-                                     K = mlp_k, hidden_layer_sizes = hidden_layer_sizes_var, activation = activation_var, solver = solver_var, alpha = alpha_var,
-                                     batch_size = batch_size_var, learning_rate = mlp_learning_rate_var, learning_rate_init = learning_rate_init_var, power_t = power_t_var,
-                                     max_iter = mlp_max_iter_var, shuffle = shuffle_var, tol = mlp_tol_var, warm_start = mlp_warm_start_var, momentum = momentum_var,
-                                     nesterovs_momentum = nesterovs_momentum_var, early_stopping = early_stopping_var, validation_fraction = mlp_validation_fraction_var,
-                                     beta_1 = beta_1_var, beta_2 = beta_2_var, epsilon = epsilon_var, n_iter_no_change = mlp_n_iter_no_change_var, max_fun = max_fun_var,
-                                     random_state = random_state_var)
+                            seed_var = None
+                        res = mlpTrn(f"--train_data_file {folder_path_from_root + separator + 'train.txt'} --train_class_file {folder_path_from_root + separator + 'trainTarget.txt'} "
+                                     f"--test_data_file {folder_path_from_root + separator + 'test.txt'} --test_class_file {folder_path_from_root + separator + 'testTarget.txt'} "
+                                     f"--weights_outfile {folder_path_from_root + separator + 'weights.wts'} --stats_file {folder_path_from_root + separator + 'stats.txt'} --nb_attributes {nb_attributes} "
+                                     f"--nb_classes {nb_classes} --console_file {crossval_folder_temp + separator + 'consoleTemp.txt'} --train_pred_outfile {folder_path_from_root + separator + 'train.out'} "
+                                     f"--test_pred_outfile {folder_path_from_root + separator + 'test.out'} --root_folder {root_folder} --nb_quant_levels {nb_quant_levels} "
+                                     f"--K {mlp_k} --hidden_layer_sizes {hidden_layer_sizes_var} --activation {activation_var} --solver {solver_var} --alpha {alpha_var} "
+                                     f"--batch_size {batch_size_var} --learning_rate {mlp_learning_rate_var} --learning_rate_init {learning_rate_init_var} --power_t {power_t_var} "
+                                     f"--max_iterations {mlp_max_iterations_var} --shuffle {shuffle_var} --tol {mlp_tol_var} --warm_start {mlp_warm_start_var} --momentum {mlp_momentum_var} "
+                                     f"--nesterovs_momentum {nesterovs_momentum_var} --early_stopping {early_stopping_var} --validation_fraction {mlp_validation_fraction_var} "
+                                     f"--beta_1 {beta_1_var} --beta_2 {beta_2_var} --epsilon {epsilon_var} --n_iter_no_change {mlp_n_iter_no_change_var} --max_fun {max_fun_var} "
+                                     f"--seed {seed_var}")
 
                         if (res == -1):
-                            return -1 # If there is an error in the Trn
+                            raise ValueError('Error during training with MLP.')
 
                     # Training with random forests
                     elif train_method == "randForest":
                         print("Enter in randForestsTrn function")
-                        random_state_var = seed
+                        seed_var = seed
                         if seed == 0:
-                            random_state_var = None
-                        res = randForestsTrn(train_data=folder_path_from_root + separator + "train.txt",train_class=folder_path_from_root + separator + "trainTarget.txt",
-                                     test_data=folder_path_from_root + separator + "test.txt",test_class=folder_path_from_root + separator + "testTarget.txt",
-                                     stats = folder_path_from_root + separator + "stats.txt", output_file = crossval_folder_temp + separator + "consoleTemp.txt",
-                                     train_pred = folder_path_from_root + separator + "train", test_pred = folder_path_from_root + separator + "test",
-                                     rules_file = folder_path_from_root + separator + "treesRules", save_folder = save_folder, n_estimators = n_estimators_var,
-                                     min_samples_split = min_samples_split_var, min_samples_leaf = min_samples_leaf_var, min_weight_fraction_leaf = min_weight_fraction_leaf_var,
-                                     max_features = max_features_var, min_impurity_decrease = min_impurity_decrease_var, max_leaf_nodes = max_leaf_nodes_var,
-                                     warm_start = dt_warm_start_var, ccp_alpha = ccp_alpha_var, criterion = rf_criterion_var, max_depth = rf_max_depth_var,
-                                     bootstrap = bootstrap_var, oob_score = oob_score_var, n_jobs = n_jobs_var, class_weight = rf_class_weight_var,
-                                     max_samples = max_samples_var, random_state = random_state_var)
+                            seed_var = None
+                        res = randForestsTrn(f"--train_data_file {folder_path_from_root + separator + 'train.txt'} --train_class_file {folder_path_from_root + separator + 'trainTarget.txt'} "
+                                     f"--test_data_file {folder_path_from_root + separator + 'test.txt'} --test_class_file {folder_path_from_root + separator + 'testTarget.txt'} "
+                                     f"--stats_file {folder_path_from_root + separator + 'stats.txt'} --console_file {crossval_folder_temp + separator + 'consoleTemp.txt'} "
+                                     f"--train_pred_outfile {folder_path_from_root + separator + 'train.out'} --test_pred_outfile {folder_path_from_root + separator + 'test.out'} --nb_attributes {nb_attributes} "
+                                     f"--nb_classes {nb_classes} --rules_outfile {folder_path_from_root + separator + 'treesRules.rls'} --root_folder {root_folder} --n_estimators {n_estimators_var} "
+                                     f"--min_samples_split {min_samples_split_var} --min_samples_leaf {min_samples_leaf_var} --min_weight_fraction_leaf {min_weight_fraction_leaf_var} "
+                                     f"--max_features {max_features_var} --min_impurity_decrease {min_impurity_decrease_var} --max_leaf_nodes {max_leaf_nodes_var} "
+                                     f"--warm_start {dt_warm_start_var} --ccp_alpha {ccp_alpha_var} --criterion {rf_criterion_var} --max_depth {rf_max_depth_var} "
+                                     f"--bootstrap {bootstrap_var} --oob_score {oob_score_var} --n_jobs {n_jobs_var} --class_weight {rf_class_weight_var} "
+                                     f"--max_samples {max_samples_var} --seed {seed_var}")
 
                         if (res == -1):
-                            return -1 # If there is an error in the Trn
+                            raise ValueError('Error during training with Random Forests.')
 
                     # Training with gradient boosting
                     else:
                         print("Enter in gradBoostTrn function")
-                        random_state_var = seed
+                        seed_var = seed
                         if seed == 0:
-                            random_state_var = None
-                        res = gradBoostTrn(train_data=folder_path_from_root + separator + "train.txt",train_class=folder_path_from_root + separator + "trainTarget.txt",
-                                     test_data=folder_path_from_root + separator + "test.txt",test_class=folder_path_from_root + separator + "testTarget.txt",
-                                     stats = folder_path_from_root + separator + "stats.txt", output_file = crossval_folder_temp + separator + "consoleTemp.txt",
-                                     train_pred = folder_path_from_root + separator + "train", test_pred = folder_path_from_root + separator + "test",
-                                     rules_file = folder_path_from_root + separator + "treesRules", save_folder = save_folder, n_estimators = n_estimators_var,
-                                     min_samples_split = min_samples_split_var, min_samples_leaf = min_samples_leaf_var, min_weight_fraction_leaf = min_weight_fraction_leaf_var,
-                                     max_features = max_features_var, min_impurity_decrease = min_impurity_decrease_var, max_leaf_nodes = max_leaf_nodes_var,
-                                     warm_start = dt_warm_start_var, ccp_alpha = ccp_alpha_var, loss = loss_var, learning_rate = gb_learning_rate_var,
-                                     subsample = subsample_var, criterion = gb_criterion_var, max_depth = gb_max_depth_var, init = init_var,
-                                     validation_fraction = gb_validation_fraction_var, n_iter_no_change = gb_n_iter_no_change_var, tol = gb_tol_var,
-                                     random_state = random_state_var)
+                            seed_var = None
+                        res = gradBoostTrn(f"--train_data_file {folder_path_from_root + separator + 'train.txt'} --train_class_file {folder_path_from_root + separator + 'trainTarget.txt'} "
+                                     f"--test_data_file {folder_path_from_root + separator + 'test.txt'} --test_class_file {folder_path_from_root + separator + 'testTarget.txt'} "
+                                     f"--stats_file {folder_path_from_root + separator + 'stats.txt'} --console_file {crossval_folder_temp + separator + 'consoleTemp.txt'} "
+                                     f"--train_pred_outfile {folder_path_from_root + separator + 'train.out'} --test_pred_outfile {folder_path_from_root + separator + 'test.out'} --nb_attributes {nb_attributes} "
+                                     f"--nb_classes {nb_classes} --rules_outfile {folder_path_from_root + separator + 'treesRules.rls'} --root_folder {root_folder} --n_estimators {n_estimators_var} "
+                                     f"--min_samples_split {min_samples_split_var} --min_samples_leaf {min_samples_leaf_var} --min_weight_fraction_leaf {min_weight_fraction_leaf_var} "
+                                     f"--max_features {max_features_var} --min_impurity_decrease {min_impurity_decrease_var} --max_leaf_nodes {max_leaf_nodes_var} "
+                                     f"--warm_start {dt_warm_start_var} --ccp_alpha {ccp_alpha_var} --loss {loss_var} --learning_rate {gb_learning_rate_var} "
+                                     f"--subsample {subsample_var} --criterion {gb_criterion_var} --max_depth {gb_max_depth_var} --init {init_var} "
+                                     f"--validation_fraction {gb_validation_fraction_var} --n_iter_no_change {gb_n_iter_no_change_var} --tol {gb_tol_var} "
+                                     f"--seed {seed_var}")
+
+                        if (res == -1):
+                            raise ValueError('Error during training with Gradient Boosting.')
 
+                    if train_method != "svm" and with_roc:
+                        res = computeRocCurve(f"--test_class_file {folder_path_from_root + separator + 'testTarget.txt'} --test_pred_file {folder_path_from_root + separator + 'test.out'} "
+                                              f"--positive_class_index {positive_class_index} --nb_classes {nb_classes} --output_roc {folder_path_from_root + separator + 'ROC_curve'} "
+                                              f"--stats_file {folder_path_from_root + separator + 'stats.txt'} --root_folder {root_folder} --show_params False")
                         if (res == -1):
-                            return -1 # If there is an error in the Trn
+                            raise ValueError('Error during computation of ROC curve.')
+                        else:
+                            fprs.append(res[0])
+                            tprs.append(res[1])
+                            aucs.append(res[2])
 
                     if is_dimlprul:
                         folder_path_from_real_root = str(crossval_folder) + separator + "Execution" + str(ni + 1) + separator + "Fold" + str(ki + 1)
                         # Get statistics from dimlpRul
                         stats = get_dimlprul_stats(folder_path_from_real_root + separator + "dimlpRules.rls")
                         test_acc = get_test_acc(folder_path_from_real_root + separator + "stats.txt", train_method)
 
@@ -1352,50 +1345,64 @@
                         mean_test_acc_dimlp += test_acc
 
 
                     if is_fidex:
                         # Compute fidex stats in folder
                         fidex_command = "fidex"
                         if train_method in {"dimlp", "dimlpBT", "svm", "mlp"}:
-                            fidex_command +=  " -I " + str(hiknot)
-                            fidex_command +=  " -Q " + str(nb_stairs)
-                        if save_folder is not None:
-                            fidex_command +=  " -R " + save_folder
-                        if attr_file is not None:
-                            fidex_command +=  " -A " + attr_file
-                        fidex_command +=  " -i " + str(max_iter)
-                        fidex_command +=  " -v " + str(min_cov)
+                            fidex_command +=  " --nb_quant_levels " + str(nb_quant_levels)
+                        if root_folder is not None:
+                            fidex_command +=  " --root_folder " + root_folder
+                        fidex_command += " --nb_attributes " + str(nb_attributes)
+                        fidex_command += " --nb_classes " + str(nb_classes)
+                        if attributes_file is not None:
+                            fidex_command +=  " --attributes_file " + attributes_file
+                        fidex_command +=  " --max_iterations " + str(max_iterations)
+                        fidex_command +=  " --min_covering " + str(min_covering)
+                        fidex_command +=  " --min_fidelity " + str(min_fidelity)
+                        fidex_command +=  " --lowest_min_fidelity " + str(lowest_min_fidelity)
+                        fidex_command +=  " --covering_strategy " + str(covering_strategy)
                         if dropout_dim != None:
-                            fidex_command +=  " -d " + str(dropout_dim)
+                            fidex_command +=  " --dropout_dim " + str(dropout_dim)
                         if dropout_hyp != None:
-                            fidex_command +=  " -h " + str(dropout_hyp)
-                        fidex_command +=  " -z " + str(seed)
+                            fidex_command +=  " --dropout_hyp " + str(dropout_hyp)
+                        fidex_command +=  " --seed " + str(seed)
+
+                        if train_method in {"dimlp", "dimlpBT", "svm", "mlp"}:
+                            fidex_command +=  " --weights_file " + folder_path_from_root + separator + "weights.wts"
+                        else:
+                            fidex_command += " --rules_file " + folder_path_from_root + separator + "treesRules.rls"
 
-                        if train_method in {"dimlp", "svm", "mlp"}:
-                            fidex_command +=  " -W " + folder_path_from_root + separator + "weights.wts"
-                        elif train_method == "dimlpBT":
-                            fidex_command +=  " -W " + folder_path_from_root + separator + "weightsBT"
-                            fidex_command +=  " -N " + str(nb_dimlp_nets)
-                        else:
-                            fidex_command += " -f " + folder_path_from_root + separator + "treesRules.rls"
-
-                        fidex_command += " -T " + folder_path_from_root + separator + "train.txt"
-                        fidex_command += " -P " + folder_path_from_root + separator + "train.out"
-                        fidex_command += " -C " + folder_path_from_root + separator + "trainTarget.txt"
-                        fidex_command += " -S " + folder_path_from_root + separator + "test.txt"
-                        fidex_command += " -p " + folder_path_from_root + separator + "test.out"
-                        fidex_command += " -c " + folder_path_from_root + separator + "testTarget.txt"
-                        fidex_command += " -O " + folder_path_from_root + separator + "fidexRule.txt"
-                        fidex_command += " -s " + folder_path_from_root + separator + "fidexStats.txt"
-                        fidex_command += " -r " + folder_path_from_root + separator + "fidexResult.txt"
+                        fidex_command += " --train_data_file " + folder_path_from_root + separator + "train.txt"
+                        fidex_command += " --train_pred_file " + folder_path_from_root + separator + "train.out"
+                        fidex_command += " --train_class_file " + folder_path_from_root + separator + "trainTarget.txt"
+                        fidex_command += " --test_data_file " + folder_path_from_root + separator + "test.txt"
+                        fidex_command += " --test_pred_file " + folder_path_from_root + separator + "test.out"
+                        fidex_command += " --test_class_file " + folder_path_from_root + separator + "testTarget.txt"
+                        fidex_command += " --rules_outfile " + folder_path_from_root + separator + "fidexRule.txt"
+                        fidex_command += " --stats_file " + folder_path_from_root + separator + "fidexStats.txt"
+                        fidex_command += " --console_file " + folder_path_from_root + separator + "fidexResult.txt"
+                        if with_roc:
+                            fidex_command += " --positive_class_index " + str(positive_class_index)
+                        if decision_threshold is not None:
+                            fidex_command += " --decision_threshold " + str(decision_threshold)
+
+                        if normalization_file is not None:
+                            fidex_command += " --normalization_file " + normalization_file
+                        if mus is not None:
+                            fidex_command += " --mus " + mus
+                        if sigmas is not None:
+                            fidex_command += " --sigmas " + sigmas
+                        if normalization_indices is not None:
+                            fidex_command += " --normalization_indices " + normalization_indices
 
                         print("Enter in fidex function")
                         res_fid = fidex.fidex(fidex_command)
                         if res_fid == -1:
-                            return -1 # If there is an error in fidex
+                            raise ValueError('Error during execution of Fidex.')
 
                         # Get statistics from fidex
                         stats_file = folder_path + separator + "fidexStats.txt"
 
                         try:
                             with open(stats_file, "r") as my_file:
                                 line = my_file.readline()
@@ -1414,110 +1421,131 @@
                         except (IOError):
                             raise ValueError(f"Error : Couldn't open fidex stat file {stats_file}.")
 
                         mean_cov_size_fid += stat_vals[0]
                         mean_nb_ant_fid += stat_vals[1]
                         mean_fidel_fid += stat_vals[2]
                         mean_rules_acc_fid += stat_vals[3]
-                        if len(stat_vals) == 5:
-                            mean_confid_fid += stat_vals[4]
-                        else:
-                            has_confidence = False
+                        mean_confid_fid += stat_vals[4]
 
                     if is_fidexglo:
                         # Compute fidexGlo rules in folder
                         fidexglo_rules_command = "fidexGloRules"
                         if train_method in {"dimlp", "dimlpBT", "svm", "mlp"}:
-                            fidexglo_rules_command +=  " -I " + str(hiknot)
-                            fidexglo_rules_command +=  " -Q " + str(nb_stairs)
-                        if save_folder is not None:
-                            fidexglo_rules_command +=  " -S " + save_folder
-                        if attr_file is not None:
-                            fidexglo_rules_command +=  " -A " + attr_file
-                        fidexglo_rules_command +=  " -i " + str(max_iter)
-                        fidexglo_rules_command +=  " -v " + str(min_cov)
+                            fidexglo_rules_command +=  " --nb_quant_levels " + str(nb_quant_levels)
+                        if root_folder is not None:
+                            fidexglo_rules_command +=  " --root_folder " + root_folder
+                        fidexglo_rules_command += " --nb_attributes " + str(nb_attributes)
+                        fidexglo_rules_command += " --nb_classes " + str(nb_classes)
+                        if attributes_file is not None:
+                            fidexglo_rules_command +=  " --attributes_file " + attributes_file
+                        fidexglo_rules_command +=  " --max_iterations " + str(max_iterations)
+                        fidexglo_rules_command +=  " --min_covering " + str(min_covering)
+                        fidexglo_rules_command +=  " --min_fidelity " + str(min_fidelity)
+                        fidexglo_rules_command +=  " --lowest_min_fidelity " + str(lowest_min_fidelity)
+                        fidexglo_rules_command +=  " --covering_strategy " + str(covering_strategy)
                         if dropout_dim != None:
-                            fidexglo_rules_command +=  " -d " + str(dropout_dim)
+                            fidexglo_rules_command +=  " --dropout_dim " + str(dropout_dim)
                         if dropout_hyp != None:
-                            fidexglo_rules_command +=  " -h " + str(dropout_hyp)
-                        fidexglo_rules_command +=  " -z " + str(seed)
-                        if train_method in {"dimlp", "svm", "mlp"}:
-                            fidexglo_rules_command +=  " -W " + folder_path_from_root + separator + "weights.wts"
-                        elif train_method == "dimlpBT":
-                            fidexglo_rules_command +=  " -W " + folder_path_from_root + separator + "weightsBT"
-                            fidexglo_rules_command +=  " -N " + str(nb_dimlp_nets)
-                        else:
-                            fidexglo_rules_command += " -f " + folder_path_from_root + separator + "treesRules.rls"
-
-                        fidexglo_rules_command += " -T " + folder_path_from_root + separator + "train.txt"
-                        fidexglo_rules_command += " -P " + folder_path_from_root + separator + "train.out"
-                        fidexglo_rules_command += " -C " + folder_path_from_root + separator + "trainTarget.txt"
-                        fidexglo_rules_command += " -O " + folder_path_from_root + separator + "fidexGloRules.txt"
-                        fidexglo_rules_command += " -r " + folder_path_from_root + separator + "fidexGloResult.txt"
-                        fidexglo_rules_command += " -M " + str(fidexglo_heuristic)
+                            fidexglo_rules_command +=  " --dropout_hyp " + str(dropout_hyp)
+                        fidexglo_rules_command +=  " --seed " + str(seed)
+                        if train_method in {"dimlp", "dimlpBT", "svm", "mlp"}:
+                            fidexglo_rules_command +=  " --weights_file " + folder_path_from_root + separator + "weights.wts"
+                        else:
+                            fidexglo_rules_command += " --rules_file " + folder_path_from_root + separator + "treesRules.rls"
 
+                        fidexglo_rules_command += " --train_data_file " + folder_path_from_root + separator + "train.txt"
+                        fidexglo_rules_command += " --train_pred_file " + folder_path_from_root + separator + "train.out"
+                        fidexglo_rules_command += " --train_class_file " + folder_path_from_root + separator + "trainTarget.txt"
+                        fidexglo_rules_command += " --global_rules_outfile " + folder_path_from_root + separator + "fidexGloRules.txt"
+                        fidexglo_rules_command += " --console_file " + folder_path_from_root + separator + "fidexGloResult.txt"
+                        fidexglo_rules_command += " --heuristic " + str(fidexglo_heuristic)
+                        if with_roc:
+                            fidexglo_rules_command += " --positive_class_index " + str(positive_class_index)
+                        if decision_threshold is not None:
+                            fidexglo_rules_command += " --decision_threshold " + str(decision_threshold)
+
+                        if normalization_file is not None:
+                            fidexglo_rules_command += " --normalization_file " + normalization_file
+                        if mus is not None:
+                            fidexglo_rules_command += " --mus " + mus
+                        if sigmas is not None:
+                            fidexglo_rules_command += " --sigmas " + sigmas
+                        if normalization_indices is not None:
+                            fidexglo_rules_command += " --normalization_indices " + normalization_indices
+                        if nb_threads is not None:
+                            fidexglo_rules_command += " --nb_threads " + str(nb_threads)
                         print("Enter in fidexGloRules function")
-                        res_fid_glo_rules = fidexGlo.fidexGloRules(fidexglo_rules_command)
+                        res_fid_glo_rules = fidex.fidexGloRules(fidexglo_rules_command)
                         if res_fid_glo_rules == -1:
-                            return -1 # If there is an error in fidexGloRules
+                            raise ValueError('Error during execution of FidexGloRules.')
 
                         # Compute fidexGlo statistics in folder
                         fidexglo_stats_command = "fidexGloStats"
-                        if save_folder is not None:
-                            fidexglo_stats_command +=  " -S " + save_folder
-                        if attr_file is not None:
-                            fidexglo_stats_command +=  " -A " + attr_file
-                        fidexglo_stats_command += " -T " + folder_path_from_root + separator + "test.txt"
-                        fidexglo_stats_command += " -P " + folder_path_from_root + separator + "test.out"
-                        fidexglo_stats_command += " -C " + folder_path_from_root + separator + "testTarget.txt"
-                        fidexglo_stats_command += " -R " + folder_path_from_root + separator + "fidexGloRules.txt"
-                        fidexglo_stats_command += " -O " + folder_path_from_root + separator + "fidexGloStats.txt"
-                        fidexglo_stats_command += " -r " + folder_path_from_root + separator + "fidexGloStatsResult.txt"
+                        if root_folder is not None:
+                            fidexglo_stats_command +=  " --root_folder " + root_folder
+                        fidexglo_stats_command += " --nb_attributes " + str(nb_attributes)
+                        fidexglo_stats_command += " --nb_classes " + str(nb_classes)
+                        if attributes_file is not None:
+                            fidexglo_stats_command +=  " --attributes_file " + attributes_file
+                        fidexglo_stats_command += " --test_data_file " + folder_path_from_root + separator + "test.txt"
+                        fidexglo_stats_command += " --test_pred_file " + folder_path_from_root + separator + "test.out"
+                        fidexglo_stats_command += " --test_class_file " + folder_path_from_root + separator + "testTarget.txt"
+                        fidexglo_stats_command += " --global_rules_file " + folder_path_from_root + separator + "fidexGloRules.txt"
+                        fidexglo_stats_command += " --stats_file " + folder_path_from_root + separator + "fidexGloStats.txt"
+                        fidexglo_stats_command += " --console_file " + folder_path_from_root + separator + "fidexGloStatsResult.txt"
+                        fidexglo_stats_command += " --global_rules_outfile " + folder_path_from_root + separator + "fidexGloRules.txt"
+                        if decision_threshold is not None:
+                            fidexglo_stats_command += " --decision_threshold " + str(decision_threshold)
+                        if with_roc:
+                            fidexglo_stats_command += " --positive_class_index " + str(positive_class_index)
 
                         print("Enter in fidexGloStats function")
-                        res_fid_glo_stats = fidexGlo.fidexGloStats(fidexglo_stats_command)
+                        res_fid_glo_stats = fidex.fidexGloStats(fidexglo_stats_command)
                         if res_fid_glo_stats == -1:
-                            return -1 # If there is an error in fidexGloStats
-
+                            raise ValueError('Error during execution of FidexGloStats.')
                         # Get statistics from fidexGlo
                         stats_glo_file = folder_path + separator + "fidexGloStats.txt"
-
                         try:
                             with open(stats_glo_file, "r") as my_file:
                                 line_stats_glo = my_file.readline()
                                 line_stats_glo = my_file.readline()
                                 line_stats_glo = line_stats_glo.strip()
                                 if line_stats_glo != "":
                                     values = line_stats_glo.split()
                                     if "rules" in values:
                                         mean_nb_rules += float(values[values.index("rules") + 2].rstrip(','))
                                     else:
-                                        raise ValueError("Error in second line of fidexGlo stat file, there is not the number of rules")
+                                        raise ValueError("Error in second line of fidexGlo stat file, there is not the number of rules.")
                                     if "sample" in values:
                                         mean_nb_cover += float(values[values.index("sample") + 6].rstrip(','))
                                     else:
-                                        raise ValueError("Error in second line of fidexGlo stat file, there is not the mean sample covering number per rule")
+                                        raise ValueError("Error in second line of fidexGlo stat file, there is not the mean sample covering number per rule.")
                                     if "antecedents" in values:
                                         mean_nb_antecedants += float(values[values.index("antecedents") + 4])
                                     else:
-                                        raise ValueError("Error in second line of fidexGlo stat file, there is not the mean number of antecedents per rule")
+                                        raise ValueError("Error in second line of fidexGlo stat file, there is not the mean number of antecedents per rule.")
 
                                 else:
                                     raise ValueError("Error in second line of fidexGlo stat file.")
-
                                 line_stats_glo = my_file.readline()
                                 line_stats_glo = my_file.readline()
                                 line_stats_glo = my_file.readline()
                                 line_stats_glo = my_file.readline()
                                 stat_glo_vals = []
                                 while line_stats_glo:
+                                    if line_stats_glo.startswith("With positive") or line_stats_glo.startswith("Computation with"):
+                                        line_stats_glo = my_file.readline()
                                     line_stats_glo = line_stats_glo.strip()  # Remove the line break at the end of the line
                                     if line_stats_glo != "":
                                         elements = line_stats_glo.split()
-                                        stat_glo_vals.append(float(elements[-1]))
+                                        if elements[-1] == "N/A":
+                                            stat_glo_vals.append("N/A")
+                                        else:
+                                            stat_glo_vals.append(float(elements[-1]))
                                     line_stats_glo = my_file.readline()
 
                                 my_file.close()
                         except (FileNotFoundError):
                             raise ValueError(f"Error : FidexGlo stat file {stats_glo_file} not found.")
                         except (IOError):
                             raise ValueError(f"Error : Couldn't open fidexGlo stat file {stats_glo_file}.")
@@ -1527,18 +1555,72 @@
                         mean_expl_glo += stat_glo_vals[2]
                         mean_default_rate += stat_glo_vals[3]
                         mean_nb_fidel_activations += stat_glo_vals[4]
                         mean_wrong_activations += stat_glo_vals[5]
                         mean_test_acc_glo += stat_glo_vals[6]
                         mean_test_acc_when_rules_and_model_agree += stat_glo_vals[7]
                         mean_test_acc_when_activated_rules_and_model_agree += stat_glo_vals[8]
+                        if with_roc:
+                            mean_nb_true_positive += stat_glo_vals[9]
+                            mean_nb_false_positive += stat_glo_vals[10]
+                            mean_nb_true_negative += stat_glo_vals[11]
+                            mean_nb_false_negative += stat_glo_vals[12]
+                            if stat_glo_vals[13] == "N/A":
+                                nb_no_false_positive_rate += 1
+                            else:
+                                mean_false_positive_rate += stat_glo_vals[13]
+                            if stat_glo_vals[14] == "N/A":
+                                nb_no_false_negative_rate += 1
+                            else:
+                                mean_false_negative_rate += stat_glo_vals[14]
+                            if stat_glo_vals[15] == "N/A":
+                                nb_no_precision += 1
+                            else:
+                                mean_precision += stat_glo_vals[15]
+                            if stat_glo_vals[16] == "N/A":
+                                nb_no_recall += 1
+                            else:
+                                mean_recall += stat_glo_vals[16]
+
+                            mean_nb_true_positive_rule += stat_glo_vals[17]
+                            mean_nb_false_positive_rule += stat_glo_vals[18]
+                            mean_nb_true_negative_rule += stat_glo_vals[19]
+                            mean_nb_false_negative_rule += stat_glo_vals[20]
+                            if stat_glo_vals[21] == "N/A":
+                                nb_no_false_positive_rate_rule += 1
+                            else:
+                                mean_false_positive_rate_rule += stat_glo_vals[21]
+                            if stat_glo_vals[22] == "N/A":
+                                nb_no_false_negative_rate_rule += 1
+                            else:
+                                mean_false_negative_rate_rule += stat_glo_vals[22]
+                            if stat_glo_vals[23] == "N/A":
+                                nb_no_precision_rule += 1
+                            else:
+                                mean_precision_rule += stat_glo_vals[23]
+                            if stat_glo_vals[24] == "N/A":
+                                nb_no_recall_rule += 1
+                            else:
+                                mean_recall_rule += stat_glo_vals[24]
                 # Compute execution Stats
 
+                if with_roc:
+                    mean_aucs.append(np.mean(np.array(aucs)))
+                    mean_tprs.append(np.mean(np.array(tprs), axis=0))
+                    mean_fprs.append(np.mean(np.array(fprs), axis=0))
+                    formatted_mean_aucs = formatting(mean_aucs[-1])
+                    viz = RocCurveDisplay(fpr=mean_fprs[-1],
+                    tpr=mean_tprs[-1],
+                    roc_auc=mean_aucs[-1]).plot(color="darkorange", plot_chance_level=True)
+
+                    viz.figure_.savefig(str(crossval_folder) + separator + "Execution" + str(ni + 1) + separator + "ROC_curve.png")
+                    plt.close(viz.figure_)
+
                 mean_current_exec_values_dimlp = []
-                if is_dimlprul: # For DimlpRul
+                if is_dimlprul: # For dimlpRul
                     nb_fold_with_rules_dimlp = k-nb_no_rules_current_exec_dimlp
 
                     mean_current_exec_values_dimlp.append(mean_nb_rules_dimlp / nb_fold_with_rules_dimlp)
                     mean_nb_rules_dimlp = 0
                     mean_current_exec_values_dimlp.append(mean_nb_cover_dimlp / nb_fold_with_rules_dimlp)
                     mean_nb_cover_dimlp = 0
                     mean_current_exec_values_dimlp.append(mean_nb_antecedants_dimlp / nb_fold_with_rules_dimlp)
@@ -1592,30 +1674,96 @@
                     mean_wrong_activations = 0
                     mean_current_exec_values_fidexglo.append(mean_test_acc_glo / k)
                     mean_test_acc_glo = 0
                     mean_current_exec_values_fidexglo.append(mean_test_acc_when_rules_and_model_agree / k)
                     mean_test_acc_when_rules_and_model_agree = 0
                     mean_current_exec_values_fidexglo.append(mean_test_acc_when_activated_rules_and_model_agree / k)
                     mean_test_acc_when_activated_rules_and_model_agree = 0
+                    if with_roc:
+                        mean_current_exec_values_fidexglo.append(mean_nb_true_positive / k)
+                        mean_nb_true_positive = 0
+                        mean_current_exec_values_fidexglo.append(mean_nb_false_positive / k)
+                        mean_nb_false_positive = 0
+                        mean_current_exec_values_fidexglo.append(mean_nb_true_negative / k)
+                        mean_nb_true_negative = 0
+                        mean_current_exec_values_fidexglo.append(mean_nb_false_negative / k)
+                        mean_nb_false_negative = 0
+                        if nb_no_false_positive_rate == k:
+                            mean_current_exec_values_fidexglo.append("N/A")
+                        else:
+                            mean_current_exec_values_fidexglo.append(mean_false_positive_rate / (k-nb_no_false_positive_rate))
+                        mean_false_positive_rate = 0
+                        nb_no_false_positive_rate = 0
+                        if nb_no_false_negative_rate == k:
+                            mean_current_exec_values_fidexglo.append("N/A")
+                        else:
+                            mean_current_exec_values_fidexglo.append(mean_false_negative_rate / (k-nb_no_false_negative_rate))
+                        mean_false_negative_rate = 0
+                        nb_no_false_negative_rate = 0
+                        if nb_no_precision == k:
+                            mean_current_exec_values_fidexglo.append("N/A")
+                        else:
+                            mean_current_exec_values_fidexglo.append(mean_precision / (k-nb_no_precision))
+                        mean_precision = 0
+                        nb_no_precision = 0
+                        if nb_no_recall == k:
+                            mean_current_exec_values_fidexglo.append("N/A")
+                        else:
+                            mean_current_exec_values_fidexglo.append(mean_recall / (k-nb_no_recall))
+                        mean_recall = 0
+                        nb_no_recall = 0
+
+                        mean_current_exec_values_fidexglo.append(mean_nb_true_positive_rule / k)
+                        mean_nb_true_positive_rule = 0
+                        mean_current_exec_values_fidexglo.append(mean_nb_false_positive_rule / k)
+                        mean_nb_false_positive_rule = 0
+                        mean_current_exec_values_fidexglo.append(mean_nb_true_negative_rule / k)
+                        mean_nb_true_negative_rule = 0
+                        mean_current_exec_values_fidexglo.append(mean_nb_false_negative_rule / k)
+                        mean_nb_false_negative_rule = 0
+                        if nb_no_false_positive_rate_rule == k:
+                            mean_current_exec_values_fidexglo.append("N/A")
+                        else:
+                            mean_current_exec_values_fidexglo.append(mean_false_positive_rate_rule / (k-nb_no_false_positive_rate_rule))
+                        mean_false_positive_rate_rule = 0
+                        nb_no_false_positive_rate_rule = 0
+                        if nb_no_false_negative_rate_rule == k:
+                            mean_current_exec_values_fidexglo.append("N/A")
+                        else:
+                            mean_current_exec_values_fidexglo.append(mean_false_negative_rate_rule / (k-nb_no_false_negative_rate_rule))
+                        mean_false_negative_rate_rule = 0
+                        nb_no_false_negative_rate_rule = 0
+                        if nb_no_precision_rule == k:
+                            mean_current_exec_values_fidexglo.append("N/A")
+                        else:
+                            mean_current_exec_values_fidexglo.append(mean_precision_rule / (k-nb_no_precision_rule))
+                        mean_precision_rule = 0
+                        nb_no_precision_rule = 0
+                        if nb_no_recall_rule == k:
+                            mean_current_exec_values_fidexglo.append("N/A")
+                        else:
+                            mean_current_exec_values_fidexglo.append(mean_recall_rule / (k-nb_no_recall_rule))
+                        mean_recall_rule = 0
+                        nb_no_recall_rule = 0
                     mean_exec_values_fidexglo.append(mean_current_exec_values_fidexglo)
 
                 # Output and show stats
                 try:
                     with open(crossval_stats, "a") as outputStatsFile:
                         outputStatsFile.write(f"Results for execution {ni + 1} of {k}-Cross validation :\n\n")
                         print("\n---------------------------------------------------------")
                         print("---------------------------------------------------------\n")
                         print(f"Results for execution {ni + 1} of {k}-Cross validation :\n")
+                        if with_roc:
+                            outputStatsFile.write(f"The mean AUC score is: {formatted_mean_aucs}\n\n")
+                            print(f"The mean AUC score is: {formatted_mean_aucs}\n")
                         if is_dimlprul:
                             formatted_mean_current_exec_values_dimlp = []
                             for i in range(len(mean_current_exec_values_dimlp)):
-                                formatted_val = "{:.6f}".format(mean_current_exec_values_dimlp[i]).rstrip(".0")
-                                if formatted_val == "":
-                                    formatted_val = "0"
-                                formatted_mean_current_exec_values_dimlp.append(formatted_val)
+                                formatted_mean_current_exec_values_dimlp.append(formatting(mean_current_exec_values_dimlp[i]))
                             outputStatsFile.write("Dimlp :\n")
                             outputStatsFile.write(f"The mean number of rules is: {formatted_mean_current_exec_values_dimlp[0]}\n")
                             if nb_no_rules_current_exec_dimlp > 0:
                                 if nb_no_rules_current_exec_dimlp == 1:
                                     outputStatsFile.write(f"We didn't found any rule {int(nb_no_rules_current_exec_dimlp)} time\n")
                                 else:
                                     outputStatsFile.write(f"We didn't found any rule {int(nb_no_rules_current_exec_dimlp)} times\n")
@@ -1643,82 +1791,131 @@
                             print("\n---------------------------------------------------------")
                             print("---------------------------------------------------------")
                             outputStatsFile.write("\n---------------------------------------------------------\n")
                             print("")
                         if is_fidex:
                             formatted_mean_current_exec_values_fidex = []
                             for i in range(len(mean_current_exec_values_fidex)):
-                                formatted_val = "{:.6f}".format(mean_current_exec_values_fidex[i]).rstrip(".0")
-                                if formatted_val == "":
-                                    formatted_val = "0"
-                                formatted_mean_current_exec_values_fidex.append(formatted_val)
+                                formatted_mean_current_exec_values_fidex.append(formatting(mean_current_exec_values_fidex[i]))
                             outputStatsFile.write("Fidex :\n")
                             outputStatsFile.write(f"The mean covering size per rule is: {formatted_mean_current_exec_values_fidex[0]}\n")
                             outputStatsFile.write(f"The mean number of antecedents per rule is: {formatted_mean_current_exec_values_fidex[1]}\n")
                             outputStatsFile.write(f"The mean rule fidelity rate is: {formatted_mean_current_exec_values_fidex[2]}\n")
                             outputStatsFile.write(f"The mean rule accuracy is: {formatted_mean_current_exec_values_fidex[3]}\n")
-                            if has_confidence:
-                                outputStatsFile.write(f"The mean rule confidence is: {formatted_mean_current_exec_values_fidex[4]}\n")
+                            outputStatsFile.write(f"The mean rule confidence is: {formatted_mean_current_exec_values_fidex[4]}\n")
                             print("Fidex :")
                             print(f"The mean covering size per rule is: {formatted_mean_current_exec_values_fidex[0]}")
                             print(f"The mean number of antecedents per rule is: {formatted_mean_current_exec_values_fidex[1]}")
                             print(f"The mean rule fidelity rate is: {formatted_mean_current_exec_values_fidex[2]}")
                             print(f"The mean rule accuracy is: {formatted_mean_current_exec_values_fidex[3]}")
-                            if has_confidence:
-                                print(f"The mean rule confidence is: {formatted_mean_current_exec_values_fidex[4]}")
+                            print(f"The mean rule confidence is: {formatted_mean_current_exec_values_fidex[4]}")
                             print("\n---------------------------------------------------------")
                             print("---------------------------------------------------------")
                         if is_fidex and is_fidexglo:
                             outputStatsFile.write("\n---------------------------------------------------------\n")
                             print("")
                         if is_fidexglo:
                             formatted_mean_current_exec_values_fidexglo = []
                             for i in range(len(mean_current_exec_values_fidexglo)):
-                                formatted_val = "{:.6f}".format(mean_current_exec_values_fidexglo[i]).rstrip(".0")
-                                if formatted_val == "":
-                                    formatted_val = "0"
-                                formatted_mean_current_exec_values_fidexglo.append(formatted_val)
+                                formatted_mean_current_exec_values_fidexglo.append(formatting(mean_current_exec_values_fidexglo[i]))
                             outputStatsFile.write("FidexGlo :\n")
                             outputStatsFile.write(f"The mean number of rules is: {formatted_mean_current_exec_values_fidexglo[0]}\n")
                             outputStatsFile.write(f"The mean sample covering number per rule is: {formatted_mean_current_exec_values_fidexglo[1]}\n")
                             outputStatsFile.write(f"The mean number of antecedents per rule is: {formatted_mean_current_exec_values_fidexglo[2]}\n")
                             outputStatsFile.write(f"The mean global rule fidelity rate is: {formatted_mean_current_exec_values_fidexglo[3]}\n")
                             outputStatsFile.write(f"The mean global rule accuracy is: {formatted_mean_current_exec_values_fidexglo[4]}\n")
                             outputStatsFile.write(f"The mean explainability rate (when we can find a rule) is: {formatted_mean_current_exec_values_fidexglo[5]}\n")
                             outputStatsFile.write(f"The mean default rule rate (when we can't find a rule) is: {formatted_mean_current_exec_values_fidexglo[6]}\n")
                             outputStatsFile.write(f"The mean number of correct (fidel) activated rules per sample is: {formatted_mean_current_exec_values_fidexglo[7]}\n")
                             outputStatsFile.write(f"The mean number of wrong (not fidel) activated rules per sample is: {formatted_mean_current_exec_values_fidexglo[8]}\n")
                             outputStatsFile.write(f"The mean model test accuracy is: {formatted_mean_current_exec_values_fidexglo[9]}\n")
                             outputStatsFile.write(f"The mean model test accuracy when rules and model agree is: {formatted_mean_current_exec_values_fidexglo[10]}\n")
                             outputStatsFile.write(f"The mean model test accuracy when activated rules and model agree is: {formatted_mean_current_exec_values_fidexglo[11]}\n")
+                            if with_roc:
+                                outputStatsFile.write(f"\nWith positive class {positive_class_index} :\n\n")
+                                outputStatsFile.write("Computation with model decision :\n\n")
+                                outputStatsFile.write(f"The mean number of true positive test samples is : {formatted_mean_current_exec_values_fidexglo[12]}\n")
+                                outputStatsFile.write(f"The mean number of false positive test samples is : {formatted_mean_current_exec_values_fidexglo[13]}\n")
+                                outputStatsFile.write(f"The mean number of true negative test samples is : {formatted_mean_current_exec_values_fidexglo[14]}\n")
+                                outputStatsFile.write(f"The mean number of false negative test samples is : {formatted_mean_current_exec_values_fidexglo[15]}\n")
+                                outputStatsFile.write(f"The mean false positive rate is : {formatted_mean_current_exec_values_fidexglo[16]}\n")
+                                outputStatsFile.write(f"The mean false negative rate is : {formatted_mean_current_exec_values_fidexglo[17]}\n")
+                                outputStatsFile.write(f"The mean precision is : {formatted_mean_current_exec_values_fidexglo[18]}\n")
+                                outputStatsFile.write(f"The mean recall is : {formatted_mean_current_exec_values_fidexglo[19]}\n")
+                                outputStatsFile.write("\nComputation with model decision :\n\n")
+                                outputStatsFile.write(f"The mean number of true positive test samples is : {formatted_mean_current_exec_values_fidexglo[20]}\n")
+                                outputStatsFile.write(f"The mean number of false positive test samples is : {formatted_mean_current_exec_values_fidexglo[21]}\n")
+                                outputStatsFile.write(f"The mean number of true negative test samples is : {formatted_mean_current_exec_values_fidexglo[22]}\n")
+                                outputStatsFile.write(f"The mean number of false negative test samples is : {formatted_mean_current_exec_values_fidexglo[23]}\n")
+                                outputStatsFile.write(f"The mean false positive rate is : {formatted_mean_current_exec_values_fidexglo[24]}\n")
+                                outputStatsFile.write(f"The mean false negative rate is : {formatted_mean_current_exec_values_fidexglo[25]}\n")
+                                outputStatsFile.write(f"The mean precision is : {formatted_mean_current_exec_values_fidexglo[26]}\n")
+                                outputStatsFile.write(f"The mean recall is : {formatted_mean_current_exec_values_fidexglo[27]}\n")
                             print("FidexGlo :")
                             print(f"The mean number of rules is: {formatted_mean_current_exec_values_fidexglo[0]}")
                             print(f"The mean sample covering number per rule is: {formatted_mean_current_exec_values_fidexglo[1]}")
                             print(f"The mean number of antecedents per rule is: {formatted_mean_current_exec_values_fidexglo[2]}")
                             print(f"The mean global rule fidelity rate is: {formatted_mean_current_exec_values_fidexglo[3]}")
                             print(f"The mean global rule accuracy is: {formatted_mean_current_exec_values_fidexglo[4]}")
                             print(f"The mean explainability rate (when we can find a rule) is: {formatted_mean_current_exec_values_fidexglo[5]}")
                             print(f"The mean default rule rate (when we can't find a rule) is: {formatted_mean_current_exec_values_fidexglo[6]}")
                             print(f"The mean number of correct (fidel) activated rules per sample is: {formatted_mean_current_exec_values_fidexglo[7]}")
                             print(f"The mean number of wrong (not fidel) activated rules per sample is: {formatted_mean_current_exec_values_fidexglo[8]}")
                             print(f"The mean model test accuracy is: {formatted_mean_current_exec_values_fidexglo[9]}")
                             print(f"The mean model test accuracy when rules and model agree is: {formatted_mean_current_exec_values_fidexglo[10]}")
                             print(f"The mean model test accuracy when activated rules and model agree is: {formatted_mean_current_exec_values_fidexglo[11]}")
+                            if with_roc:
+                                print(f"\nWith positive class {positive_class_index} :\n")
+                                print("Computation with model decision :\n")
+                                print(f"The mean number of true positive test samples is : {formatted_mean_current_exec_values_fidexglo[12]}")
+                                print(f"The mean number of false positive test samples is : {formatted_mean_current_exec_values_fidexglo[13]}")
+                                print(f"The mean number of true negative test samples is : {formatted_mean_current_exec_values_fidexglo[14]}")
+                                print(f"The mean number of false negative test samples is : {formatted_mean_current_exec_values_fidexglo[15]}")
+                                print(f"The mean false positive rate is : {formatted_mean_current_exec_values_fidexglo[16]}")
+                                print(f"The mean false negative rate is : {formatted_mean_current_exec_values_fidexglo[17]}")
+                                print(f"The mean precision is : {formatted_mean_current_exec_values_fidexglo[18]}")
+                                print(f"The mean recall is : {formatted_mean_current_exec_values_fidexglo[19]}")
+                                print("\nComputation with rules decision :\n")
+                                print(f"The mean number of true positive test samples is : {formatted_mean_current_exec_values_fidexglo[20]}")
+                                print(f"The mean number of false positive test samples is : {formatted_mean_current_exec_values_fidexglo[21]}")
+                                print(f"The mean number of true negative test samples is : {formatted_mean_current_exec_values_fidexglo[22]}")
+                                print(f"The mean number of false negative test samples is : {formatted_mean_current_exec_values_fidexglo[23]}")
+                                print(f"The mean false positive rate is : {formatted_mean_current_exec_values_fidexglo[24]}")
+                                print(f"The mean false negative rate is : {formatted_mean_current_exec_values_fidexglo[25]}")
+                                print(f"The mean precision is : {formatted_mean_current_exec_values_fidexglo[26]}")
+                                print(f"The mean recall is : {formatted_mean_current_exec_values_fidexglo[27]}")
                             print("\n---------------------------------------------------------")
                             print("---------------------------------------------------------")
                         outputStatsFile.write("\n---------------------------------------------------------\n")
                         outputStatsFile.write("---------------------------------------------------------\n\n")
 
                         outputStatsFile.close()
                 except (FileNotFoundError):
                     raise ValueError(f"Error : File for stats extraction ({crossval_stats}) not found.")
                 except (IOError):
                     raise ValueError(f"Error : Couldn't open stats extraction file {crossval_stats}.")
 
             # Compute stats on all executions
+            if with_roc:
+                mean_all_aucs = np.mean(np.array(mean_aucs))
+                std_all_aucs = np.std(np.array(mean_aucs))
+
+                mean_all_fprs = np.mean(np.array(mean_fprs), axis=0)
+                mean_all_tprs = np.mean(np.array(mean_tprs), axis=0)
+
+                viz = RocCurveDisplay(fpr=mean_all_fprs,
+                                    tpr=mean_all_tprs,
+                                    roc_auc=mean_all_aucs).plot(color="darkorange", plot_chance_level=True)
+
+                viz.figure_.savefig(crossval_folder + separator + "ROC_curve.png")
+                plt.close(viz.figure_)
+
+                formatted_mean_all_aucs = formatting(mean_all_aucs)
+                formatted_std_all_aucs = formatting(std_all_aucs)
+
 
             if is_dimlprul: # For dimlpRul
                 for exec in range(n):
                     multiplier = k-mean_exec_values_dimlp[exec][8] # If there is lack of some datas (sometimes we didnt found any rules), we need to take it into account
                     mean_nb_rules_dimlp_all += multiplier*mean_exec_values_dimlp[exec][0]
                     mean_nb_cover_dimlp_all += multiplier*mean_exec_values_dimlp[exec][1]
                     mean_nb_antecedants_dimlp_all += multiplier*mean_exec_values_dimlp[exec][2]
@@ -1734,188 +1931,172 @@
                 mean_nb_antecedants_dimlp_all /= divider
                 mean_fidel_dimlp_all /= divider
                 mean_rules_acc_dimlp_all /= divider
                 mean_default_rate_dimlp_all /= divider
                 mean_test_acc_dimlp_all /= divider
                 mean_test_acc_when_rules_and_model_agree_dimlp_all /= divider
 
-                for exec in range(n):
-                    std_nb_rules_dimlp_all += pow(mean_exec_values_dimlp[exec][0] - mean_nb_rules_dimlp_all, 2)
-                    std_nb_cover_dimlp_all += pow(mean_exec_values_dimlp[exec][1] - mean_nb_cover_dimlp_all, 2)
-                    std_nb_antecedants_dimlp_all += pow(mean_exec_values_dimlp[exec][2] - mean_nb_antecedants_dimlp_all, 2)
-                    std_fidel_dimlp_all += pow(mean_exec_values_dimlp[exec][3] - mean_fidel_dimlp_all, 2)
-                    std_rules_acc_dimlp_all += pow(mean_exec_values_dimlp[exec][4] - mean_rules_acc_dimlp_all, 2)
-                    std_default_rate_dimlp_all += pow(mean_exec_values_dimlp[exec][5] - mean_default_rate_dimlp_all, 2)
-                    std_test_acc_dimlp_all += pow(mean_exec_values_dimlp[exec][6] - mean_test_acc_dimlp_all, 2)
-                    std_test_acc_when_rules_and_model_agree_dimlp_all += pow(mean_exec_values_dimlp[exec][7] - mean_test_acc_when_rules_and_model_agree_dimlp_all, 2)
-
-                std_nb_rules_dimlp_all = math.sqrt(std_nb_rules_dimlp_all / n)
-                std_nb_cover_dimlp_all = math.sqrt(std_nb_cover_dimlp_all / n)
-                std_nb_antecedants_dimlp_all = math.sqrt(std_nb_antecedants_dimlp_all / n)
-                std_fidel_dimlp_all = math.sqrt(std_fidel_dimlp_all / n)
-                std_rules_acc_dimlp_all = math.sqrt(std_rules_acc_dimlp_all / n)
-                std_default_rate_dimlp_all = math.sqrt(std_default_rate_dimlp_all / n)
-                std_test_acc_dimlp_all = math.sqrt(std_test_acc_dimlp_all / n)
-                std_test_acc_when_rules_and_model_agree_dimlp_all = math.sqrt(std_test_acc_when_rules_and_model_agree_dimlp_all / n)
+                std_nb_rules_dimlp_all = np.std(np.array(mean_exec_values_dimlp)[:,0].astype(float))
+                std_nb_cover_dimlp_all = np.std(np.array(mean_exec_values_dimlp)[:,1].astype(float))
+                std_nb_antecedants_dimlp_all = np.std(np.array(mean_exec_values_dimlp)[:,2].astype(float))
+                std_fidel_dimlp_all = np.std(np.array(mean_exec_values_dimlp)[:,3].astype(float))
+                std_rules_acc_dimlp_all = np.std(np.array(mean_exec_values_dimlp)[:,4].astype(float))
+                std_default_rate_dimlp_all = np.std(np.array(mean_exec_values_dimlp)[:,5].astype(float))
+                std_test_acc_dimlp_all = np.std(np.array(mean_exec_values_dimlp)[:,6].astype(float))
+                std_test_acc_when_rules_and_model_agree_dimlp_all = np.std(np.array(mean_exec_values_dimlp)[:,7].astype(float))
 
             if is_fidex: # For Fidex
-                for exec in range(n):
-                    mean_cov_size_fid_all += mean_exec_values_fidex[exec][0]
-                    mean_nb_ant_fid_all += mean_exec_values_fidex[exec][1]
-                    mean_fidel_fid_all += mean_exec_values_fidex[exec][2]
-                    mean_rules_acc_fid_all += mean_exec_values_fidex[exec][3]
-                    mean_confid_fid_all += mean_exec_values_fidex[exec][4]
-
-                mean_cov_size_fid_all /= n
-                mean_nb_ant_fid_all /= n
-                mean_fidel_fid_all /= n
-                mean_rules_acc_fid_all /= n
-                mean_confid_fid_all /= n
 
-                for exec in range(n):
-                    std_cov_size_fid_all += pow(mean_exec_values_fidex[exec][0] - mean_cov_size_fid_all, 2)
-                    std_nb_ant_fid_all += pow(mean_exec_values_fidex[exec][1] - mean_nb_ant_fid_all, 2)
-                    std_fidel_fid_all += pow(mean_exec_values_fidex[exec][2] - mean_fidel_fid_all, 2)
-                    std_rules_acc_fid_all += pow(mean_exec_values_fidex[exec][3] - mean_rules_acc_fid_all, 2)
-                    std_confid_fid_all += pow(mean_exec_values_fidex[exec][4] - mean_confid_fid_all, 2)
-
-                std_cov_size_fid_all = math.sqrt(std_cov_size_fid_all / n)
-                std_nb_ant_fid_all = math.sqrt(std_nb_ant_fid_all / n)
-                std_fidel_fid_all = math.sqrt(std_fidel_fid_all / n)
-                std_rules_acc_fid_all = math.sqrt(std_rules_acc_fid_all / n)
-                std_confid_fid_all = math.sqrt(std_confid_fid_all / n)
+                mean_cov_size_fid_all = np.mean(np.array(mean_exec_values_fidex)[:,0].astype(float))
+                mean_nb_ant_fid_all = np.mean(np.array(mean_exec_values_fidex)[:,1].astype(float))
+                mean_fidel_fid_all = np.mean(np.array(mean_exec_values_fidex)[:,2].astype(float))
+                mean_rules_acc_fid_all = np.mean(np.array(mean_exec_values_fidex)[:,3].astype(float))
+                mean_confid_fid_all = np.mean(np.array(mean_exec_values_fidex)[:,4].astype(float))
+
+                std_cov_size_fid_all = np.std(np.array(mean_exec_values_fidex)[:,0].astype(float))
+                std_nb_ant_fid_all = np.std(np.array(mean_exec_values_fidex)[:,1].astype(float))
+                std_fidel_fid_all = np.std(np.array(mean_exec_values_fidex)[:,2].astype(float))
+                std_rules_acc_fid_all = np.std(np.array(mean_exec_values_fidex)[:,3].astype(float))
+                std_confid_fid_all = np.std(np.array(mean_exec_values_fidex)[:,4].astype(float))
 
             if is_fidexglo: # For FidexGlo
-                for exec in range(n):
-                    mean_nb_rules_all += mean_exec_values_fidexglo[exec][0]
-                    mean_nb_cover_all += mean_exec_values_fidexglo[exec][1]
-                    mean_nb_antecedants_all += mean_exec_values_fidexglo[exec][2]
-                    mean_fidel_glo_all += mean_exec_values_fidexglo[exec][3]
-                    mean_rules_acc_glo_all += mean_exec_values_fidexglo[exec][4]
-                    mean_expl_glo_all += mean_exec_values_fidexglo[exec][5]
-                    mean_default_rate_all += mean_exec_values_fidexglo[exec][6]
-                    mean_nb_fidel_activations_all += mean_exec_values_fidexglo[exec][7]
-                    mean_wrong_activations_all += mean_exec_values_fidexglo[exec][8]
-                    mean_test_acc_glo_all += mean_exec_values_fidexglo[exec][9]
-                    mean_test_acc_when_rules_and_model_agree_all += mean_exec_values_fidexglo[exec][10]
-                    mean_test_acc_when_activated_rules_and_model_agree_all += mean_exec_values_fidexglo[exec][11]
-
-                mean_nb_rules_all /= n
-                mean_nb_cover_all /= n
-                mean_nb_antecedants_all /= n
-                mean_fidel_glo_all /= n
-                mean_rules_acc_glo_all /= n
-                mean_expl_glo_all /= n
-                mean_default_rate_all /= n
-                mean_nb_fidel_activations_all /= n
-                mean_wrong_activations_all /= n
-                mean_test_acc_glo_all /= n
-                mean_test_acc_when_rules_and_model_agree_all /= n
-                mean_test_acc_when_activated_rules_and_model_agree_all /= n
+                mean_nb_rules_all = np.mean(np.array(mean_exec_values_fidexglo)[:,0].astype(float))
+                mean_nb_cover_all = np.mean(np.array(mean_exec_values_fidexglo)[:,1].astype(float))
+                mean_nb_antecedants_all = np.mean(np.array(mean_exec_values_fidexglo)[:,2].astype(float))
+                mean_fidel_glo_all = np.mean(np.array(mean_exec_values_fidexglo)[:,3].astype(float))
+                mean_rules_acc_glo_all = np.mean(np.array(mean_exec_values_fidexglo)[:,4].astype(float))
+                mean_expl_glo_all = np.mean(np.array(mean_exec_values_fidexglo)[:,5].astype(float))
+                mean_default_rate_all = np.mean(np.array(mean_exec_values_fidexglo)[:,6].astype(float))
+                mean_nb_fidel_activations_all = np.mean(np.array(mean_exec_values_fidexglo)[:,7].astype(float))
+                mean_wrong_activations_all = np.mean(np.array(mean_exec_values_fidexglo)[:,8].astype(float))
+                mean_test_acc_glo_all = np.mean(np.array(mean_exec_values_fidexglo)[:,9].astype(float))
+                mean_test_acc_when_rules_and_model_agree_all = np.mean(np.array(mean_exec_values_fidexglo)[:,10].astype(float))
+                mean_test_acc_when_activated_rules_and_model_agree_all = np.mean(np.array(mean_exec_values_fidexglo)[:,11].astype(float))
+
+                if with_roc:
+                    mean_nb_true_positive_all = np.mean(np.array(mean_exec_values_fidexglo)[:,12].astype(float))
+                    mean_nb_false_positive_all = np.mean(np.array(mean_exec_values_fidexglo)[:,13].astype(float))
+                    mean_nb_true_negative_all = np.mean(np.array(mean_exec_values_fidexglo)[:,14].astype(float))
+                    mean_nb_false_negative_all = np.mean(np.array(mean_exec_values_fidexglo)[:,15].astype(float))
+                    false_positive_rate_exec_temp = [v for v in np.array(mean_exec_values_fidexglo)[:,16] if v != "N/A"]
+                    false_negative_rate_exec_temp = [v for v in np.array(mean_exec_values_fidexglo)[:,17] if v != "N/A"]
+                    precision_exec_temp = [v for v in np.array(mean_exec_values_fidexglo)[:,18] if v != "N/A"]
+                    recall_exec_temp = [v for v in np.array(mean_exec_values_fidexglo)[:,19] if v != "N/A"]
+                    if len(false_positive_rate_exec_temp) == 0:
+                           mean_false_positive_rate_all = "N/A"
+                           std_false_positive_rate_all = "N/A"
+                    else:
+                        mean_false_positive_rate_all = np.mean(np.array(false_positive_rate_exec_temp).astype(float))
+                        std_false_positive_rate_all = np.std(np.array(false_positive_rate_exec_temp).astype(float))
+                    if len(false_negative_rate_exec_temp) == 0:
+                           mean_false_negative_rate_all = "N/A"
+                           std_false_negative_rate_all = "N/A"
+                    else:
+                        mean_false_negative_rate_all = np.mean(np.array(false_negative_rate_exec_temp).astype(float))
+                        std_false_negative_rate_all = np.mean(np.array(false_negative_rate_exec_temp).astype(float))
+                    if len(precision_exec_temp) == 0:
+                           mean_precision_all = "N/A"
+                           std_precision_all = "N/A"
+                    else:
+                        mean_precision_all = np.mean(np.array(precision_exec_temp).astype(float))
+                        std_precision_all = np.mean(np.array(precision_exec_temp).astype(float))
+                    if len(recall_exec_temp) == 0:
+                           mean_recall_all = "N/A"
+                           std_recall_all = "N/A"
+                    else:
+                        mean_recall_all = np.mean(np.array(recall_exec_temp).astype(float))
+                        std_recall_all = np.mean(np.array(recall_exec_temp).astype(float))
 
-                for exec in range(n):
-                    std_nb_rules_all += pow(mean_exec_values_fidexglo[exec][0] - mean_nb_rules_all, 2)
-                    std_nb_cover_all += pow(mean_exec_values_fidexglo[exec][1] - mean_nb_cover_all, 2)
-                    std_nb_antecedants_all += pow(mean_exec_values_fidexglo[exec][2] - mean_nb_antecedants_all, 2)
-                    std_fidel_glo_all += pow(mean_exec_values_fidexglo[exec][3] - mean_fidel_glo_all, 2)
-                    std_rules_acc_glo_all += pow(mean_exec_values_fidexglo[exec][4] - mean_rules_acc_glo_all, 2)
-                    std_expl_glo_all += pow(mean_exec_values_fidexglo[exec][5] - mean_expl_glo_all, 2)
-                    std_default_rate_all += pow(mean_exec_values_fidexglo[exec][6] - mean_default_rate_all, 2)
-                    std_nb_fidel_activations_all += pow(mean_exec_values_fidexglo[exec][7] - mean_nb_fidel_activations_all, 2)
-                    std_wrong_activations_all += pow(mean_exec_values_fidexglo[exec][8] - mean_wrong_activations_all, 2)
-                    std_test_acc_glo_all += pow(mean_exec_values_fidexglo[exec][9] - mean_test_acc_glo_all, 2)
-                    std_test_acc_when_rules_and_model_agree_all += pow(mean_exec_values_fidexglo[exec][10] - mean_test_acc_when_rules_and_model_agree_all, 2)
-                    std_test_acc_when_activated_rules_and_model_agree_all += pow(mean_exec_values_fidexglo[exec][11] - mean_test_acc_when_activated_rules_and_model_agree_all, 2)
-
-                std_nb_rules_all = math.sqrt(std_nb_rules_all / n)
-                std_nb_cover_all = math.sqrt(std_nb_cover_all / n)
-                std_nb_antecedants_all = math.sqrt(std_nb_antecedants_all / n)
-                std_fidel_glo_all = math.sqrt(std_fidel_glo_all / n)
-                std_rules_acc_glo_all = math.sqrt(std_rules_acc_glo_all / n)
-                std_expl_glo_all = math.sqrt(std_expl_glo_all / n)
-                std_default_rate_all = math.sqrt(std_default_rate_all / n)
-                std_nb_fidel_activations_all = math.sqrt(std_nb_fidel_activations_all / n)
-                std_wrong_activations_all = math.sqrt(std_wrong_activations_all / n)
-                std_test_acc_glo_all = math.sqrt(std_test_acc_glo_all / n)
-                std_test_acc_when_rules_and_model_agree_all = math.sqrt(std_test_acc_when_rules_and_model_agree_all / n)
-                std_test_acc_when_activated_rules_and_model_agree_all = math.sqrt(std_test_acc_when_activated_rules_and_model_agree_all / n)
+                    mean_nb_true_positive_rule_all = np.mean(np.array(mean_exec_values_fidexglo)[:,20].astype(float))
+                    mean_nb_false_positive_rule_all = np.mean(np.array(mean_exec_values_fidexglo)[:,21].astype(float))
+                    mean_nb_true_negative_rule_all = np.mean(np.array(mean_exec_values_fidexglo)[:,22].astype(float))
+                    mean_nb_false_negative_rule_all = np.mean(np.array(mean_exec_values_fidexglo)[:,23].astype(float))
+                    false_positive_rate_exec_rule_temp = [v for v in np.array(mean_exec_values_fidexglo)[:,24] if v != "N/A"]
+                    false_negative_rate_exec_rule_temp = [v for v in np.array(mean_exec_values_fidexglo)[:,25] if v != "N/A"]
+                    precision_exec_rule_temp = [v for v in np.array(mean_exec_values_fidexglo)[:,26] if v != "N/A"]
+                    recall_exec_rule_temp = [v for v in np.array(mean_exec_values_fidexglo)[:,27] if v != "N/A"]
+                    if len(false_positive_rate_exec_rule_temp) == 0:
+                           mean_false_positive_rate_rule_all = "N/A"
+                           std_false_positive_rate_rule_all = "N/A"
+                    else:
+                        mean_false_positive_rate_rule_all = np.mean(np.array(false_positive_rate_exec_rule_temp).astype(float))
+                        std_false_positive_rate_rule_all = np.std(np.array(false_positive_rate_exec_rule_temp).astype(float))
+                    if len(false_negative_rate_exec_rule_temp) == 0:
+                           mean_false_negative_rate_rule_all = "N/A"
+                           std_false_negative_rate_rule_all = "N/A"
+                    else:
+                        mean_false_negative_rate_rule_all = np.mean(np.array(false_negative_rate_exec_rule_temp).astype(float))
+                        std_false_negative_rate_rule_all = np.mean(np.array(false_negative_rate_exec_rule_temp).astype(float))
+                    if len(precision_exec_rule_temp) == 0:
+                           mean_precision_rule_all = "N/A"
+                           std_precision_rule_all = "N/A"
+                    else:
+                        mean_precision_rule_all = np.mean(np.array(precision_exec_rule_temp).astype(float))
+                        std_precision_rule_all = np.mean(np.array(precision_exec_rule_temp).astype(float))
+                    if len(recall_exec_rule_temp) == 0:
+                           mean_recall_rule_all = "N/A"
+                           std_recall_rule_all = "N/A"
+                    else:
+                        mean_recall_rule_all = np.mean(np.array(recall_exec_rule_temp).astype(float))
+                        std_recall_rule_all = np.mean(np.array(recall_exec_rule_temp).astype(float))
+
+                std_nb_rules_all = np.std(np.array(mean_exec_values_fidexglo)[:,0].astype(float))
+                std_nb_cover_all = np.std(np.array(mean_exec_values_fidexglo)[:,1].astype(float))
+                std_nb_antecedants_all = np.std(np.array(mean_exec_values_fidexglo)[:,2].astype(float))
+                std_fidel_glo_all = np.std(np.array(mean_exec_values_fidexglo)[:,3].astype(float))
+                std_rules_acc_glo_all = np.std(np.array(mean_exec_values_fidexglo)[:,4].astype(float))
+                std_expl_glo_all = np.std(np.array(mean_exec_values_fidexglo)[:,5].astype(float))
+                std_default_rate_all = np.std(np.array(mean_exec_values_fidexglo)[:,6].astype(float))
+                std_nb_fidel_activations_all = np.std(np.array(mean_exec_values_fidexglo)[:,7].astype(float))
+                std_wrong_activations_all = np.std(np.array(mean_exec_values_fidexglo)[:,8].astype(float))
+                std_test_acc_glo_all = np.std(np.array(mean_exec_values_fidexglo)[:,9].astype(float))
+                std_test_acc_when_rules_and_model_agree_all = np.std(np.array(mean_exec_values_fidexglo)[:,10].astype(float))
+                std_test_acc_when_activated_rules_and_model_agree_all = np.std(np.array(mean_exec_values_fidexglo)[:,11].astype(float))
+                if with_roc:
+                    std_nb_true_positive_all = np.std(np.array(mean_exec_values_fidexglo)[:,12].astype(float))
+                    std_nb_false_positive_all = np.std(np.array(mean_exec_values_fidexglo)[:,13].astype(float))
+                    std_nb_true_negative_all = np.std(np.array(mean_exec_values_fidexglo)[:,14].astype(float))
+                    std_nb_false_negative_all = np.std(np.array(mean_exec_values_fidexglo)[:,15].astype(float))
+
+                    std_nb_true_positive_rule_all = np.std(np.array(mean_exec_values_fidexglo)[:,20].astype(float))
+                    std_nb_false_positive_rule_all = np.std(np.array(mean_exec_values_fidexglo)[:,21].astype(float))
+                    std_nb_true_negative_rule_all = np.std(np.array(mean_exec_values_fidexglo)[:,22].astype(float))
+                    std_nb_false_negative_rule_all = np.std(np.array(mean_exec_values_fidexglo)[:,23].astype(float))
 
             # Show and save results
             try:
                 with open(crossval_stats, "a") as outputStatsFile:
                     outputStatsFile.write(f"Results for {n} times {k}-Cross validation :\n\n")
                     print("\n---------------------------------------------------------")
                     print("---------------------------------------------------------\n")
                     print(f"Results for {n} times {k}-Cross validation :\n")
-                    if is_dimlprul:
+                    if with_roc:
+                        outputStatsFile.write(f"The mean AUC score is: {formatted_mean_all_aucs}\n")
+                        outputStatsFile.write(f"The standard deviation of the AUC score is: {formatted_std_all_aucs}\n\n")
+                        print(f"The mean AUC score is: {formatted_mean_all_aucs}")
+                        print(f"The standard deviation of the AUC score is: {formatted_std_all_aucs}\n")
 
-                        formatted_mean_nb_rules_dimlp_all = "{:.6f}".format(mean_nb_rules_dimlp_all).rstrip(".0")
-                        if formatted_mean_nb_rules_dimlp_all == "":
-                            formatted_mean_nb_rules_dimlp_all = "0"
-
-                        formatted_std_nb_rules_dimlp_all = "{:.6f}".format(std_nb_rules_dimlp_all).rstrip(".0")
-                        if formatted_std_nb_rules_dimlp_all == "":
-                            formatted_std_nb_rules_dimlp_all = "0"
-
-                        formatted_mean_nb_cover_dimlp_all = "{:.6f}".format(mean_nb_cover_dimlp_all).rstrip(".0")
-                        if formatted_mean_nb_cover_dimlp_all == "":
-                            formatted_mean_nb_cover_dimlp_all = "0"
-
-                        formatted_std_nb_cover_dimlp_all = "{:.6f}".format(std_nb_cover_dimlp_all).rstrip(".0")
-                        if formatted_std_nb_cover_dimlp_all == "":
-                            formatted_std_nb_cover_dimlp_all = "0"
-
-                        formatted_mean_nb_antecedants_dimlp_all = "{:.6f}".format(mean_nb_antecedants_dimlp_all).rstrip(".0")
-                        if formatted_mean_nb_antecedants_dimlp_all == "":
-                            formatted_mean_nb_antecedants_dimlp_all = "0"
-
-                        formatted_std_nb_antecedants_dimlp_all = "{:.6f}".format(std_nb_antecedants_dimlp_all).rstrip(".0")
-                        if formatted_std_nb_antecedants_dimlp_all == "":
-                            formatted_std_nb_antecedants_dimlp_all = "0"
-
-                        formatted_mean_fidel_dimlp_all = "{:.6f}".format(mean_fidel_dimlp_all).rstrip(".0")
-                        if formatted_mean_fidel_dimlp_all == "":
-                            formatted_mean_fidel_dimlp_all = "0"
-
-                        formatted_std_fidel_dimlp_all = "{:.6f}".format(std_fidel_dimlp_all).rstrip(".0")
-                        if formatted_std_fidel_dimlp_all == "":
-                            formatted_std_fidel_dimlp_all = "0"
-
-                        formatted_mean_rules_acc_dimlp_all = "{:.6f}".format(mean_rules_acc_dimlp_all).rstrip(".0")
-                        if formatted_mean_rules_acc_dimlp_all == "":
-                            formatted_mean_rules_acc_dimlp_all = "0"
-
-                        formatted_std_rules_acc_dimlp_all = "{:.6f}".format(std_rules_acc_dimlp_all).rstrip(".0")
-                        if formatted_std_rules_acc_dimlp_all == "":
-                            formatted_std_rules_acc_dimlp_all = "0"
-
-                        formatted_mean_default_rate_dimlp_all = "{:.6f}".format(mean_default_rate_dimlp_all).rstrip(".0")
-                        if formatted_mean_default_rate_dimlp_all == "":
-                            formatted_mean_default_rate_dimlp_all = "0"
-
-                        formatted_std_default_rate_dimlp_all = "{:.6f}".format(std_default_rate_dimlp_all).rstrip(".0")
-                        if formatted_std_default_rate_dimlp_all == "":
-                            formatted_std_default_rate_dimlp_all = "0"
-
-                        formatted_mean_test_acc_dimlp_all = "{:.6f}".format(mean_test_acc_dimlp_all).rstrip(".0")
-                        if formatted_mean_test_acc_dimlp_all == "":
-                            formatted_mean_test_acc_dimlp_all = "0"
-
-                        formatted_std_test_acc_dimlp_all = "{:.6f}".format(std_test_acc_dimlp_all).rstrip(".0")
-                        if formatted_std_test_acc_dimlp_all == "":
-                            formatted_std_test_acc_dimlp_all = "0"
-
-                        formatted_mean_test_acc_when_rules_and_model_agree_dimlp_all = "{:.6f}".format(mean_test_acc_when_rules_and_model_agree_dimlp_all).rstrip(".0")
-                        if formatted_mean_test_acc_when_rules_and_model_agree_dimlp_all == "":
-                            formatted_mean_test_acc_when_rules_and_model_agree_dimlp_all = "0"
-
-                        formatted_std_test_acc_when_rules_and_model_agree_dimlp_all = "{:.6f}".format(std_test_acc_when_rules_and_model_agree_dimlp_all).rstrip(".0")
-                        if formatted_std_test_acc_when_rules_and_model_agree_dimlp_all == "":
-                            formatted_std_test_acc_when_rules_and_model_agree_dimlp_all = "0"
+                    if is_dimlprul:
 
+                        formatted_mean_nb_rules_dimlp_all = formatting(mean_nb_rules_dimlp_all)
+                        formatted_std_nb_rules_dimlp_all = formatting(std_nb_rules_dimlp_all)
+                        formatted_mean_nb_cover_dimlp_all = formatting(mean_nb_cover_dimlp_all)
+                        formatted_std_nb_cover_dimlp_all = formatting(std_nb_cover_dimlp_all)
+                        formatted_mean_nb_antecedants_dimlp_all = formatting(mean_nb_antecedants_dimlp_all)
+                        formatted_std_nb_antecedants_dimlp_all = formatting(std_nb_antecedants_dimlp_all)
+                        formatted_mean_fidel_dimlp_all = formatting(mean_fidel_dimlp_all)
+                        formatted_std_fidel_dimlp_all = formatting(std_fidel_dimlp_all)
+                        formatted_mean_rules_acc_dimlp_all = formatting(mean_rules_acc_dimlp_all)
+                        formatted_std_rules_acc_dimlp_all = formatting(std_rules_acc_dimlp_all)
+                        formatted_mean_default_rate_dimlp_all = formatting(mean_default_rate_dimlp_all)
+                        formatted_std_default_rate_dimlp_all = formatting(std_default_rate_dimlp_all)
+                        formatted_mean_test_acc_dimlp_all = formatting(mean_test_acc_dimlp_all)
+                        formatted_std_test_acc_dimlp_all = formatting(std_test_acc_dimlp_all)
+                        formatted_mean_test_acc_when_rules_and_model_agree_dimlp_all = formatting(mean_test_acc_when_rules_and_model_agree_dimlp_all)
+                        formatted_std_test_acc_when_rules_and_model_agree_dimlp_all = formatting(std_test_acc_when_rules_and_model_agree_dimlp_all)
                         outputStatsFile.write("Dimlp :\n")
                         outputStatsFile.write(f"The mean number of rules is: {formatted_mean_nb_rules_dimlp_all}\n")
                         if nb_no_rules_dimlp > 0:
                                 if nb_no_rules_dimlp == 1:
                                     outputStatsFile.write(f"We didn't found any rule {int(nb_no_rules_dimlp)} time\n")
                                 else:
                                     outputStatsFile.write(f"We didn't found any rule {int(nb_no_rules_dimlp)} times\n")
@@ -1961,182 +2142,115 @@
                         print("\n---------------------------------------------------------")
                         print("---------------------------------------------------------")
                         print("")
                         outputStatsFile.write("\n---------------------------------------------------------\n\n")
 
                     if is_fidex:
 
-                        formatted_mean_cov_size_fid_all = "{:.6f}".format(mean_cov_size_fid_all).rstrip(".0")
-                        if formatted_mean_cov_size_fid_all == "":
-                            formatted_mean_cov_size_fid_all = "0"
-
-                        formatted_std_cov_size_fid_all = "{:.6f}".format(std_cov_size_fid_all).rstrip(".0")
-                        if formatted_std_cov_size_fid_all == "":
-                            formatted_std_cov_size_fid_all = "0"
-
-                        formatted_mean_nb_ant_fid_all = "{:.6f}".format(mean_nb_ant_fid_all).rstrip(".0")
-                        if formatted_mean_nb_ant_fid_all == "":
-                            formatted_mean_nb_ant_fid_all = "0"
-
-                        formatted_std_nb_ant_fid_all = "{:.6f}".format(std_nb_ant_fid_all).rstrip(".0")
-                        if formatted_std_nb_ant_fid_all == "":
-                            formatted_std_nb_ant_fid_all = "0"
-
-                        formatted_mean_fidel_fid_all = "{:.6f}".format(mean_fidel_fid_all).rstrip(".0")
-                        if formatted_mean_fidel_fid_all == "":
-                            formatted_mean_fidel_fid_all = "0"
-
-                        formatted_std_fidel_fid_all = "{:.6f}".format(std_fidel_fid_all).rstrip(".0")
-                        if formatted_std_fidel_fid_all == "":
-                            formatted_std_fidel_fid_all = "0"
-
-                        formatted_mean_rules_acc_fid_all = "{:.6f}".format(mean_rules_acc_fid_all).rstrip(".0")
-                        if formatted_mean_rules_acc_fid_all == "":
-                            formatted_mean_rules_acc_fid_all = "0"
-
-                        formatted_std_rules_acc_fid_all = "{:.6f}".format(std_rules_acc_fid_all).rstrip(".0")
-                        if formatted_std_rules_acc_fid_all == "":
-                            formatted_std_rules_acc_fid_all = "0"
-
-                        formatted_mean_confid_fid_all = "{:.6f}".format(mean_confid_fid_all).rstrip(".0")
-                        if formatted_mean_confid_fid_all == "":
-                            formatted_mean_confid_fid_all = "0"
-
-                        formatted_std_confid_fid_all = "{:.6f}".format(std_confid_fid_all).rstrip(".0")
-                        if formatted_std_confid_fid_all == "":
-                            formatted_std_confid_fid_all = "0"
+                        formatted_mean_cov_size_fid_all = formatting(mean_cov_size_fid_all)
+                        formatted_std_cov_size_fid_all = formatting(std_cov_size_fid_all)
+                        formatted_mean_nb_ant_fid_all = formatting(mean_nb_ant_fid_all)
+                        formatted_std_nb_ant_fid_all = formatting(std_nb_ant_fid_all)
+                        formatted_mean_fidel_fid_all = formatting(mean_fidel_fid_all)
+                        formatted_std_fidel_fid_all = formatting(std_fidel_fid_all)
+                        formatted_mean_rules_acc_fid_all = formatting(mean_rules_acc_fid_all)
+                        formatted_std_rules_acc_fid_all = formatting(std_rules_acc_fid_all)
+                        formatted_mean_confid_fid_all = formatting(mean_confid_fid_all)
+                        formatted_std_confid_fid_all = formatting(std_confid_fid_all)
 
                         outputStatsFile.write("Fidex :\n")
                         outputStatsFile.write(f"The mean covering size per rule is : {formatted_mean_cov_size_fid_all}\n")
                         outputStatsFile.write(f"The standard deviation of the covering size per rule is : {formatted_std_cov_size_fid_all}\n")
                         outputStatsFile.write(f"The mean number of antecedents per rule is : {formatted_mean_nb_ant_fid_all}\n")
                         outputStatsFile.write(f"The standard deviation of the number of antecedents per rule is : {formatted_std_nb_ant_fid_all}\n")
                         outputStatsFile.write(f"The mean rule fidelity rate is : {formatted_mean_fidel_fid_all}\n")
                         outputStatsFile.write(f"The standard deviation of the rule fidelity rate is : {formatted_std_fidel_fid_all}\n")
                         outputStatsFile.write(f"The mean rule accuracy is : {formatted_mean_rules_acc_fid_all}\n")
                         outputStatsFile.write(f"The standard deviation of the rule accuracy is : {formatted_std_rules_acc_fid_all}\n")
-                        if has_confidence:
-                            outputStatsFile.write(f"The mean rule confidence is : {formatted_mean_confid_fid_all}\n")
-                            outputStatsFile.write(f"The standard deviation of the rule confidence is : {formatted_std_confid_fid_all}\n")
+                        outputStatsFile.write(f"The mean rule confidence is : {formatted_mean_confid_fid_all}\n")
+                        outputStatsFile.write(f"The standard deviation of the rule confidence is : {formatted_std_confid_fid_all}\n")
                         print("Fidex :")
                         print(f"The mean covering size per rule is : {formatted_mean_cov_size_fid_all}")
                         print(f"The standard deviation of the covering size per rule is : {formatted_std_cov_size_fid_all}")
                         print(f"The mean number of antecedents per rule is : {formatted_mean_nb_ant_fid_all}")
                         print(f"The standard deviation of the number of antecedents per rule is : {formatted_std_nb_ant_fid_all}")
                         print(f"The mean rule fidelity rate is : {formatted_mean_fidel_fid_all}")
                         print(f"The standard deviation of the rule fidelity rate is : {formatted_std_fidel_fid_all}")
                         print(f"The mean rule accuracy is : {formatted_mean_rules_acc_fid_all}")
                         print(f"The standard deviation of the rule accuracy is : {formatted_std_rules_acc_fid_all}")
-                        if has_confidence:
-                            print(f"The mean rule confidence is : {formatted_mean_confid_fid_all}")
-                            print(f"The standard deviation of the rule confidence is : {formatted_std_confid_fid_all}")
+                        print(f"The mean rule confidence is : {formatted_mean_confid_fid_all}")
+                        print(f"The standard deviation of the rule confidence is : {formatted_std_confid_fid_all}")
                         print("\n---------------------------------------------------------")
                         print("---------------------------------------------------------")
 
                     if is_fidex and is_fidexglo:
                         print("")
                         outputStatsFile.write("\n---------------------------------------------------------\n\n")
 
                     if is_fidexglo:
 
-                        formatted_mean_nb_rules_all = "{:.6f}".format(mean_nb_rules_all).rstrip(".0")
-                        if formatted_mean_nb_rules_all == "":
-                            formatted_mean_nb_rules_all = "0"
-
-                        formatted_std_nb_rules_all = "{:.6f}".format(std_nb_rules_all).rstrip(".0")
-                        if formatted_std_nb_rules_all == "":
-                            formatted_std_nb_rules_all = "0"
-
-                        formatted_mean_nb_cover_all = "{:.6f}".format(mean_nb_cover_all).rstrip(".0")
-                        if formatted_mean_nb_cover_all == "":
-                            formatted_mean_nb_cover_all = "0"
-
-                        formatted_std_nb_cover_all = "{:.6f}".format(std_nb_cover_all).rstrip(".0")
-                        if formatted_std_nb_cover_all == "":
-                            formatted_std_nb_cover_all = "0"
-
-                        formatted_mean_nb_antecedants_all = "{:.6f}".format(mean_nb_antecedants_all).rstrip(".0")
-                        if formatted_mean_nb_antecedants_all == "":
-                            formatted_mean_nb_antecedants_all = "0"
-
-                        formatted_std_nb_antecedants_all = "{:.6f}".format(std_nb_antecedants_all).rstrip(".0")
-                        if formatted_std_nb_antecedants_all == "":
-                            formatted_std_nb_antecedants_all = "0"
-
-                        formatted_mean_fidel_glo_all = "{:.6f}".format(mean_fidel_glo_all).rstrip(".0")
-                        if formatted_mean_fidel_glo_all == "":
-                            formatted_mean_fidel_glo_all = "0"
-
-                        formatted_std_fidel_glo_all = "{:.6f}".format(std_fidel_glo_all).rstrip(".0")
-                        if formatted_std_fidel_glo_all == "":
-                            formatted_std_fidel_glo_all = "0"
-
-                        formatted_mean_rules_acc_glo_all = "{:.6f}".format(mean_rules_acc_glo_all).rstrip(".0")
-                        if formatted_mean_rules_acc_glo_all == "":
-                            formatted_mean_rules_acc_glo_all = "0"
-
-                        formatted_std_rules_acc_glo_all = "{:.6f}".format(std_rules_acc_glo_all).rstrip(".0")
-                        if formatted_std_rules_acc_glo_all == "":
-                            formatted_std_rules_acc_glo_all = "0"
-
-                        formatted_mean_expl_glo_all = "{:.6f}".format(mean_expl_glo_all).rstrip(".0")
-                        if formatted_mean_expl_glo_all == "":
-                            formatted_mean_expl_glo_all = "0"
-
-                        formatted_std_expl_glo_all = "{:.6f}".format(std_expl_glo_all).rstrip(".0")
-                        if formatted_std_expl_glo_all == "":
-                            formatted_std_expl_glo_all = "0"
-
-                        formatted_mean_default_rate_all = "{:.6f}".format(mean_default_rate_all).rstrip(".0")
-                        if formatted_mean_default_rate_all == "":
-                            formatted_mean_default_rate_all = "0"
-
-                        formatted_std_default_rate_all = "{:.6f}".format(std_default_rate_all).rstrip(".0")
-                        if formatted_std_default_rate_all == "":
-                            formatted_std_default_rate_all = "0"
-
-                        formatted_mean_nb_fidel_activations_all = "{:.6f}".format(mean_nb_fidel_activations_all).rstrip(".0")
-                        if formatted_mean_nb_fidel_activations_all == "":
-                            formatted_mean_nb_fidel_activations_all = "0"
-
-                        formatted_std_nb_fidel_activations_all = "{:.6f}".format(std_nb_fidel_activations_all).rstrip(".0")
-                        if formatted_std_nb_fidel_activations_all == "":
-                            formatted_std_nb_fidel_activations_all = "0"
-
-                        formatted_mean_wrong_activations_all = "{:.6f}".format(mean_wrong_activations_all).rstrip(".0")
-                        if formatted_mean_wrong_activations_all == "":
-                            formatted_mean_wrong_activations_all = "0"
-
-                        formatted_std_wrong_activations_all = "{:.6f}".format(std_wrong_activations_all).rstrip(".0")
-                        if formatted_std_wrong_activations_all == "":
-                            formatted_std_wrong_activations_all = "0"
-
-                        formatted_mean_test_acc_glo_all = "{:.6f}".format(mean_test_acc_glo_all).rstrip(".0")
-                        if formatted_mean_test_acc_glo_all == "":
-                            formatted_mean_test_acc_glo_all = "0"
-
-                        formatted_std_test_acc_glo_all = "{:.6f}".format(std_test_acc_glo_all).rstrip(".0")
-                        if formatted_std_test_acc_glo_all == "":
-                            formatted_std_test_acc_glo_all = "0"
-
-                        formatted_mean_test_acc_when_rules_and_model_agree_all = "{:.6f}".format(mean_test_acc_when_rules_and_model_agree_all).rstrip(".0")
-                        if formatted_mean_test_acc_when_rules_and_model_agree_all == "":
-                            formatted_mean_test_acc_when_rules_and_model_agree_all = "0"
-
-                        formatted_std_test_acc_when_rules_and_model_agree_all = "{:.6f}".format(std_test_acc_when_rules_and_model_agree_all).rstrip(".0")
-                        if formatted_std_test_acc_when_rules_and_model_agree_all == "":
-                            formatted_std_test_acc_when_rules_and_model_agree_all = "0"
-
-                        formatted_mean_test_acc_when_activated_rules_and_model_agree_all = "{:.6f}".format(mean_test_acc_when_activated_rules_and_model_agree_all).rstrip(".0")
-                        if formatted_mean_test_acc_when_activated_rules_and_model_agree_all == "":
-                            formatted_mean_test_acc_when_activated_rules_and_model_agree_all = "0"
-
-                        formatted_std_test_acc_when_activated_rules_and_model_agree_all = "{:.6f}".format(std_test_acc_when_activated_rules_and_model_agree_all).rstrip(".0")
-                        if formatted_std_test_acc_when_activated_rules_and_model_agree_all == "":
-                            formatted_std_test_acc_when_activated_rules_and_model_agree_all = "0"
+                        formatted_mean_nb_rules_all = formatting(mean_nb_rules_all)
+                        formatted_std_nb_rules_all = formatting(std_nb_rules_all)
+                        formatted_mean_nb_cover_all = formatting(mean_nb_cover_all)
+                        formatted_std_nb_cover_all = formatting(std_nb_cover_all)
+                        formatted_mean_nb_antecedants_all = formatting(mean_nb_antecedants_all)
+                        formatted_std_nb_antecedants_all = formatting(std_nb_antecedants_all)
+                        formatted_mean_fidel_glo_all = formatting(mean_fidel_glo_all)
+                        formatted_std_fidel_glo_all = formatting(std_fidel_glo_all)
+                        formatted_mean_rules_acc_glo_all = formatting(mean_rules_acc_glo_all)
+                        formatted_std_rules_acc_glo_all = formatting(std_rules_acc_glo_all)
+                        formatted_mean_expl_glo_all = formatting(mean_expl_glo_all)
+                        formatted_std_expl_glo_all = formatting(std_expl_glo_all)
+                        formatted_mean_default_rate_all = formatting(mean_default_rate_all)
+                        formatted_std_default_rate_all = formatting(std_default_rate_all)
+                        formatted_mean_nb_fidel_activations_all = formatting(mean_nb_fidel_activations_all)
+                        formatted_std_nb_fidel_activations_all = formatting(std_nb_fidel_activations_all)
+                        formatted_mean_wrong_activations_all = formatting(mean_wrong_activations_all)
+                        formatted_std_wrong_activations_all = formatting(std_wrong_activations_all)
+                        formatted_mean_test_acc_glo_all = formatting(mean_test_acc_glo_all)
+                        formatted_std_test_acc_glo_all = formatting(std_test_acc_glo_all)
+                        formatted_mean_test_acc_when_rules_and_model_agree_all = formatting(mean_test_acc_when_rules_and_model_agree_all)
+                        formatted_std_test_acc_when_rules_and_model_agree_all = formatting(std_test_acc_when_rules_and_model_agree_all)
+                        formatted_mean_test_acc_when_activated_rules_and_model_agree_all = formatting(mean_test_acc_when_activated_rules_and_model_agree_all)
+                        formatted_std_test_acc_when_activated_rules_and_model_agree_all = formatting(std_test_acc_when_activated_rules_and_model_agree_all)
+
+                        if with_roc:
+
+                            formatted_mean_nb_true_positive_all = formatting(mean_nb_true_positive_all)
+                            formatted_std_nb_true_positive_all = formatting(std_nb_true_positive_all)
+                            formatted_mean_nb_false_positive_all = formatting(mean_nb_false_positive_all)
+                            formatted_std_nb_false_positive_all = formatting(std_nb_false_positive_all)
+                            formatted_mean_nb_true_negative_all = formatting(mean_nb_true_negative_all)
+                            formatted_std_nb_true_negative_all = formatting(std_nb_true_negative_all)
+                            formatted_mean_nb_false_negative_all = formatting(mean_nb_false_negative_all)
+                            formatted_std_nb_false_negative_all = formatting(std_nb_false_negative_all)
+                            formatted_mean_false_positive_rate_all = formatting(mean_false_positive_rate_all)
+                            formatted_std_false_positive_rate_all = formatting(std_false_positive_rate_all)
+                            formatted_mean_false_negative_rate_all = formatting(mean_false_negative_rate_all)
+                            formatted_std_false_negative_rate_all = formatting(std_false_negative_rate_all)
+                            formatted_mean_precision_all = formatting(mean_precision_all)
+                            formatted_std_precision_all = formatting(std_precision_all)
+                            formatted_mean_recall_all = formatting(mean_recall_all)
+                            formatted_std_recall_all = formatting(std_recall_all)
+                            formatted_mean_nb_true_positive_rule_all = formatting(mean_nb_true_positive_rule_all)
+                            formatted_std_nb_true_positive_rule_all = formatting(std_nb_true_positive_rule_all)
+                            formatted_mean_nb_false_positive_rule_all = formatting(mean_nb_false_positive_rule_all)
+                            formatted_std_nb_false_positive_rule_all = formatting(std_nb_false_positive_rule_all)
+                            formatted_mean_nb_true_negative_rule_all = formatting(mean_nb_true_negative_rule_all)
+                            formatted_std_nb_true_negative_rule_all = formatting(std_nb_true_negative_rule_all)
+                            formatted_mean_nb_false_negative_rule_all = formatting(mean_nb_false_negative_rule_all)
+                            formatted_std_nb_false_negative_rule_all = formatting(std_nb_false_negative_rule_all)
+                            formatted_mean_false_positive_rate_rule_all = formatting(mean_false_positive_rate_rule_all)
+                            formatted_std_false_positive_rate_rule_all = formatting(std_false_positive_rate_rule_all)
+                            formatted_mean_false_negative_rate_rule_all = formatting(mean_false_negative_rate_rule_all)
+                            formatted_std_false_negative_rate_rule_all = formatting(std_false_negative_rate_rule_all)
+                            formatted_mean_precision_rule_all = formatting(mean_precision_rule_all)
+                            formatted_std_precision_rule_all = formatting(std_precision_rule_all)
+                            formatted_mean_recall_rule_all = formatting(mean_recall_rule_all)
+                            formatted_std_recall_rule_all = formatting(std_recall_rule_all)
 
                         outputStatsFile.write("FidexGlo :\n")
                         outputStatsFile.write(f"The mean number of rules is : {formatted_mean_nb_rules_all}\n")
                         outputStatsFile.write(f"The standard deviation of the number of rules is : {formatted_std_nb_rules_all}\n")
                         outputStatsFile.write(f"The mean sample covering number per rule is : {formatted_mean_nb_cover_all}\n")
                         outputStatsFile.write(f"The standard deviation of the sample covering number per rule is : {formatted_std_nb_cover_all}\n")
                         outputStatsFile.write(f"The mean number of antecedents per rule is : {formatted_mean_nb_antecedants_all}\n")
@@ -2155,14 +2269,50 @@
                         outputStatsFile.write(f"The standard deviation of the number of wrong(not fidel) activated rules per sample is : {formatted_std_wrong_activations_all}\n")
                         outputStatsFile.write(f"The mean model test accuracy is : {formatted_mean_test_acc_glo_all}\n")
                         outputStatsFile.write(f"The standard deviation of the model test accuracy is : {formatted_std_test_acc_glo_all}\n")
                         outputStatsFile.write(f"The mean model test accuracy when rules and model agree is : {formatted_mean_test_acc_when_rules_and_model_agree_all}\n")
                         outputStatsFile.write(f"The standard deviation of the model test accuracy when rules and model agree is : {formatted_std_test_acc_when_rules_and_model_agree_all}\n")
                         outputStatsFile.write(f"The mean model test accuracy when activated rules and model agree is : {formatted_mean_test_acc_when_activated_rules_and_model_agree_all}\n")
                         outputStatsFile.write(f"The standard deviation of the model test accuracy when activated rules and model agree is : {formatted_std_test_acc_when_activated_rules_and_model_agree_all}\n")
+                        if with_roc:
+                            outputStatsFile.write(f"\nWith positive class {positive_class_index} :\n\n")
+                            outputStatsFile.write("Computation with model decision :\n\n")
+                            outputStatsFile.write(f"The mean number of true positive test samples is : {formatted_mean_nb_true_positive_all}\n")
+                            outputStatsFile.write(f"The standard deviation number of true positive test samples is : {formatted_std_nb_true_positive_all}\n")
+                            outputStatsFile.write(f"The mean number of false positive test samples is : {formatted_mean_nb_false_positive_all}\n")
+                            outputStatsFile.write(f"The standard deviation number of false positive test samples is : {formatted_std_nb_false_positive_all}\n")
+                            outputStatsFile.write(f"The mean number of true negative test samples is : {formatted_mean_nb_true_negative_all}\n")
+                            outputStatsFile.write(f"The standard deviation number of true negative test samples is : {formatted_std_nb_true_negative_all}\n")
+                            outputStatsFile.write(f"The mean number of false negative test samples is : {formatted_mean_nb_false_negative_all}\n")
+                            outputStatsFile.write(f"The standard deviation number of false negative test samples is : {formatted_std_nb_false_negative_all}\n")
+                            outputStatsFile.write(f"The mean false positive rate is : {formatted_mean_false_positive_rate_all}\n")
+                            outputStatsFile.write(f"The standard deviation false positive rate is : {formatted_std_false_positive_rate_all}\n")
+                            outputStatsFile.write(f"The mean false negative rate is : {formatted_mean_false_negative_rate_all}\n")
+                            outputStatsFile.write(f"The standard deviation false negative rate is : {formatted_std_false_negative_rate_all}\n")
+                            outputStatsFile.write(f"The mean precision is : {formatted_mean_precision_all}\n")
+                            outputStatsFile.write(f"The standard deviation precision is : {formatted_std_precision_all}\n")
+                            outputStatsFile.write(f"The mean recall is : {formatted_mean_recall_all}\n")
+                            outputStatsFile.write(f"The standard deviation recall is : {formatted_std_recall_all}\n")
+                            outputStatsFile.write("\nComputation with rules decision :\n\n")
+                            outputStatsFile.write(f"The mean number of true positive test samples is : {formatted_mean_nb_true_positive_rule_all}\n")
+                            outputStatsFile.write(f"The standard deviation number of true positive test samples is : {formatted_std_nb_true_positive_rule_all}\n")
+                            outputStatsFile.write(f"The mean number of false positive test samples is : {formatted_mean_nb_false_positive_rule_all}\n")
+                            outputStatsFile.write(f"The standard deviation number of false positive test samples is : {formatted_std_nb_false_positive_rule_all}\n")
+                            outputStatsFile.write(f"The mean number of true negative test samples is : {formatted_mean_nb_true_negative_rule_all}\n")
+                            outputStatsFile.write(f"The standard deviation number of true negative test samples is : {formatted_std_nb_true_negative_rule_all}\n")
+                            outputStatsFile.write(f"The mean number of false negative test samples is : {formatted_mean_nb_false_negative_rule_all}\n")
+                            outputStatsFile.write(f"The standard deviation number of false negative test samples is : {formatted_std_nb_false_negative_rule_all}\n")
+                            outputStatsFile.write(f"The mean false positive rate is : {formatted_mean_false_positive_rate_rule_all}\n")
+                            outputStatsFile.write(f"The standard deviation false positive rate is : {formatted_std_false_positive_rate_rule_all}\n")
+                            outputStatsFile.write(f"The mean false negative rate is : {formatted_mean_false_negative_rate_rule_all}\n")
+                            outputStatsFile.write(f"The standard deviation false negative rate is : {formatted_std_false_negative_rate_rule_all}\n")
+                            outputStatsFile.write(f"The mean precision is : {formatted_mean_precision_rule_all}\n")
+                            outputStatsFile.write(f"The standard deviation precision is : {formatted_std_precision_rule_all}\n")
+                            outputStatsFile.write(f"The mean recall is : {formatted_mean_recall_rule_all}\n")
+                            outputStatsFile.write(f"The standard deviation recall is : {formatted_std_recall_rule_all}\n")
                         print("FidexGlo :")
                         print(f"The mean number of rules is : {formatted_mean_nb_rules_all}")
                         print(f"The standard deviation of the number of rules is : {formatted_std_nb_rules_all}")
                         print(f"The mean sample covering number per rule is : {formatted_mean_nb_cover_all}")
                         print(f"The standard deviation of the sample covering number per rule is : {formatted_std_nb_cover_all}")
                         print(f"The mean number of antecedents per rule is : {formatted_mean_nb_antecedants_all}")
                         print(f"The standard deviation of the number of antecedents per rule is : {formatted_std_nb_antecedants_all}")
@@ -2180,83 +2330,71 @@
                         print(f"The standard deviation of the number of wrong(not fidel) activated rules per sample is : {formatted_std_wrong_activations_all}")
                         print(f"The mean model test accuracy is : {formatted_mean_test_acc_glo_all}")
                         print(f"The standard deviation of the model test accuracy is : {formatted_std_test_acc_glo_all}")
                         print(f"The mean model test accuracy when rules and model agree is : {formatted_mean_test_acc_when_rules_and_model_agree_all}")
                         print(f"The standard deviation of the model test accuracy when rules and model agree is : {formatted_std_test_acc_when_rules_and_model_agree_all}")
                         print(f"The mean model test accuracy when activated rules and model agree is : {formatted_mean_test_acc_when_activated_rules_and_model_agree_all}")
                         print(f"The standard deviation of the model test accuracy when activated rules and model agree is : {formatted_std_test_acc_when_activated_rules_and_model_agree_all}")
+                        if with_roc:
+                            print(f"\nWith positive class {positive_class_index} :\n")
+                            print("Computation with model decision :\n")
+                            print(f"The mean number of true positive test samples is : {formatted_mean_nb_true_positive_all}")
+                            print(f"The standard deviation number of true positive test samples is : {formatted_std_nb_true_positive_all}")
+                            print(f"The mean number of false positive test samples is : {formatted_mean_nb_false_positive_all}")
+                            print(f"The standard deviation number of false positive test samples is : {formatted_std_nb_false_positive_all}")
+                            print(f"The mean number of true negative test samples is : {formatted_mean_nb_true_negative_all}")
+                            print(f"The standard deviation number of true negative test samples is : {formatted_std_nb_true_negative_all}")
+                            print(f"The mean number of false negative test samples is : {formatted_mean_nb_false_negative_all}")
+                            print(f"The standard deviation number of false negative test samples is : {formatted_std_nb_false_negative_all}")
+                            print(f"The mean false positive rate is : {formatted_mean_false_positive_rate_all}")
+                            print(f"The standard deviation false positive rate is : {formatted_std_false_positive_rate_all}")
+                            print(f"The mean false negative rate is : {formatted_mean_false_negative_rate_all}")
+                            print(f"The standard deviation false negative rate is : {formatted_std_false_negative_rate_all}")
+                            print(f"The mean precision is : {formatted_mean_precision_all}")
+                            print(f"The standard deviation precision is : {formatted_std_precision_all}")
+                            print(f"The mean recall is : {formatted_mean_recall_all}")
+                            print(f"The standard deviation recall is : {formatted_std_recall_all}")
+                            print("\nComputation with rules decision :\n")
+                            print(f"The mean number of true positive test samples is : {formatted_mean_nb_true_positive_rule_all}")
+                            print(f"The standard deviation number of true positive test samples is : {formatted_std_nb_true_positive_rule_all}")
+                            print(f"The mean number of false positive test samples is : {formatted_mean_nb_false_positive_rule_all}")
+                            print(f"The standard deviation number of false positive test samples is : {formatted_std_nb_false_positive_rule_all}")
+                            print(f"The mean number of true negative test samples is : {formatted_mean_nb_true_negative_rule_all}")
+                            print(f"The standard deviation number of true negative test samples is : {formatted_std_nb_true_negative_rule_all}")
+                            print(f"The mean number of false negative test samples is : {formatted_mean_nb_false_negative_rule_all}")
+                            print(f"The standard deviation number of false negative test samples is : {formatted_std_nb_false_negative_rule_all}")
+                            print(f"The mean false positive rate is : {formatted_mean_false_positive_rate_rule_all}")
+                            print(f"The standard deviation false positive rate is : {formatted_std_false_positive_rate_rule_all}")
+                            print(f"The mean false negative rate is : {formatted_mean_false_negative_rate_rule_all}")
+                            print(f"The standard deviation false negative rate is : {formatted_std_false_negative_rate_rule_all}")
+                            print(f"The mean precision is : {formatted_mean_precision_rule_all}")
+                            print(f"The standard deviation precision is : {formatted_std_precision_rule_all}")
+                            print(f"The mean recall is : {formatted_mean_recall_rule_all}")
+                            print(f"The standard deviation recall is : {formatted_std_recall_rule_all}")
                         print("\n---------------------------------------------------------")
                         print("---------------------------------------------------------")
 
 
 
                     outputStatsFile.close()
             except (FileNotFoundError):
                 raise ValueError(f"Error : File for stats extraction ({crossval_stats}) not found.")
             except (IOError):
                 raise ValueError(f"Error : Couldn't open stats extraction file {crossval_stats}.")
 
 
             # Delete temporary files
-            try:
-                console_file = crossval_folder + separator + "consoleTemp.txt"
-                os.remove(console_file)
-            except FileNotFoundError:
-                print(f"Error : File '{console_file}' not found.")
-            except Exception:
-                print(f"Error during delete of file {console_file}")
-
-            try:
-                train_file = crossval_folder + separator + "tempTrain.txt"
-                os.remove(train_file)
-            except FileNotFoundError:
-                print(f"Error : File '{train_file}' not found.")
-            except Exception:
-                print(f"Error during delete of file {train_file}")
-
-            try:
-                test_file = crossval_folder + separator + "tempTest.txt"
-                os.remove(test_file)
-            except FileNotFoundError:
-                print(f"Error : File '{test_file}' not found.")
-            except Exception:
-                print(f"Error during delete of file {test_file}")
-
-            try:
-                tar_train_file = crossval_folder + separator + "tempTarTrain.txt"
-                os.remove(tar_train_file)
-            except FileNotFoundError:
-                print(f"Error : File '{tar_train_file}' not found.")
-            except Exception:
-                print(f"Error during delete of file {tar_train_file}")
-
-            try:
-                tar_test_file = crossval_folder + separator + "tempTarTest.txt"
-                os.remove(tar_test_file)
-            except FileNotFoundError:
-                print(f"Error : File '{tar_test_file}' not found.")
-            except Exception:
-                print(f"Error during delete of file {tar_test_file}")
-
+            delete_file(crossval_folder + separator + "consoleTemp.txt")
+            delete_file(crossval_folder + separator + "tempTrain.txt")
+            delete_file(crossval_folder + separator + "tempTest.txt")
+            delete_file(crossval_folder + separator + "tempTarTrain.txt")
+            delete_file(crossval_folder + separator + "tempTarTest.txt")
             if train_method == "dimlp":
-                try:
-                    valid_file = crossval_folder + separator + "tempValid.txt"
-                    os.remove(valid_file)
-                except FileNotFoundError:
-                    print(f"Error : File '{valid_file}' not found.")
-                except Exception:
-                    print(f"Error during delete of file {valid_file}")
-
-                try:
-                    tar_valid_file = crossval_folder + separator + "tempTarValid.txt"
-                    os.remove(tar_valid_file)
-                except FileNotFoundError:
-                    print(f"Error : File '{tar_valid_file}' not found.")
-                except Exception:
-                    print(f"Error during delete of file {tar_valid_file}")
+                delete_file(crossval_folder + separator + "tempValid.txt")
+                delete_file(crossval_folder + separator + "tempTarValid.txt")
 
         end_time = time.time()
         full_time = end_time - start_time
         full_time = "{:.6f}".format(full_time).rstrip(".0")
 
         print(f"\nFull execution time = {full_time} sec")
 
@@ -2271,12 +2409,15 @@
             raise ValueError(f"Error : Couldn't open stats extraction file {crossval_stats}.")
 
         return 0
     except ValueError as error:
         print(error)
         return -1
 
-
-# Exemple Dimlp : crossValid(train_method="dimlp", algo="both", data_file="datanorm", class_file="dataclass2", nb_in=16, nb_out=2, H2=5, save_folder="dimlp/datafiles", crossVal_folder="CrossValidationDIMLP", K=3, N=2, seed=33)
-# Exemple DimlpBT : crossValid(train_method="dimlpBT", algo="both", data_file="datanorm", class_file="dataclass2", nb_in=16, nb_out=2, H2=5, save_folder="dimlp/datafiles", crossVal_folder="CrossValidationDIMLPBT", K=3, N=2, seed=33)
-# Exemple SVM : crossValid(train_method="svm", algo="both", data_file="datanorm", class_file="dataclass2", save_folder="dimlp/datafiles", crossVal_folder="CrossValidationSVM", K=3, N=2, seed=33)
-# Exemple MLP : crossValid(train_method="mlp", algo="both", data_file="datanorm", class_file="dataclass2", save_folder="dimlp/datafiles", crossVal_folder="CrossValidationMLP", K=3, N=2, seed=33)
+if __name__ == "__main__":
+    cmdline_args = " ".join(sys.argv[1:])
+    mlpTrn(cmdline_args)
+
+# Exemple Dimlp : crossValid(train_method="dimlp", algo="both", data_file="datanorm", class_file="dataclass2", positive_class_index=1, dimlpRul=1, nb_attributes=16, nb_classes=2, hidden_layers=[5], root_folder="dimlp/datafiles", crossVal_folder="CrossValidationDIMLP", K=3, N=2, seed=33)
+# Exemple dimlpBT : crossValid(train_method="dimlpBT", algo="both", data_file="datanorm", class_file="dataclass2", positive_class_index=1, dimlpRul=1, nb_attributes=16, nb_classes=2, hidden_layers=[5], root_folder="dimlp/datafiles", crossVal_folder="CrossValidationDIMLPBT", K=3, N=2, seed=33)
+# Exemple SVM : crossValid(train_method="svm", algo="both", data_file="datanorm", class_file="dataclass2", positive_class_index=1, nb_attributes=16, nb_classes=2, root_folder="dimlp/datafiles", crossVal_folder="CrossValidationSVM", K=3, N=2, seed=33)
+# Exemple MLP : crossValid(train_method="mlp", algo="both", data_file="datanorm", class_file="dataclass2", positive_class_index=1, nb_attributes=16, nb_classes=2, root_folder="dimlp/datafiles", crossVal_folder="CrossValidationMLP", K=3, N=2, seed=33)
```

### Comparing `dimlpfidex-0.0.0/dimlp/pybind/bindings.cpp` & `dimlpfidex-0.0.1/dimlp/pybind/bindings.cpp`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-#include "../cpp/src/DensClsFct.h"
-#include "../cpp/src/DimlpBTFct.h"
-#include "../cpp/src/DimlpClsFct.h"
-#include "../cpp/src/DimlpPredFct.h"
-#include "../cpp/src/DimlpRulFct.h"
-#include "../cpp/src/DimlpTrnFct.h"
+#include "../cpp/src/densClsFct.h"
+#include "../cpp/src/dimlpBTFct.h"
+#include "../cpp/src/dimlpClsFct.h"
+#include "../cpp/src/dimlpPredFct.h"
+#include "../cpp/src/dimlpRulFct.h"
+#include "../cpp/src/dimlpTrnFct.h"
 #include <pybind11/pybind11.h>
 
 namespace py = pybind11;
 
 PYBIND11_MODULE(dimlp, m) {
   m.doc() = "pybind11 dimlp plugin"; // optional module docstring
-  m.def("dimlpPred", &dimlpPred, "A function to get predictions on test set, training needs to be done before.");
-  m.def("dimlpCls", &dimlpCls, "A function to get predictions and accuracy on test set, need to give test classess and training needs to be done before.");
-  m.def("dimlpRul", &dimlpRul, "A function to get rules with stats for train, test and validation sets, gives also accuracy and error.");
-  m.def("dimlpTrn", &dimlpTrn, "A function to train dimlp model on training set, get accuracies and errors on train, test and validation sets, get the model weights and the predictions on train and test sets. Extract rules with stats for each set");
-  m.def("dimlpBT", &dimlpBT, "A function to train N dimlp models with bagging on training set, get accuracies and errors on train, test and validation sets, get the model weights and the predictions on train and test sets. Extract rules with stats for each set");
-  m.def("densCls", &densCls, "A function to get rules and precision and global accuracy on train and test on a bag of models, training needs to be done before.");
+  m.def("dimlpPred", &dimlpPred, pybind11::arg("command") = "", "A function to get predictions on test set, training needs to be done before.");
+  m.def("dimlpCls", &dimlpCls, pybind11::arg("command") = "", "A function to get predictions and accuracy on test set, need to give test classess and training needs to be done before.");
+  m.def("dimlpRul", &dimlpRul, pybind11::arg("command") = "", "A function to get rules with stats for train, test and validation sets, gives also accuracy and error.");
+  m.def("dimlpTrn", &dimlpTrn, pybind11::arg("command") = "", "A function to train dimlp model on training set, get accuracies and errors on train, test and validation sets, get the model weights and the predictions on train and test sets. Extract rules with stats for each set");
+  m.def("dimlpBT", &dimlpBT, pybind11::arg("command") = "", "A function to train N dimlp models with bagging on training set, get accuracies and errors on train, test and validation sets, get the model weights and the predictions on train and test sets. Extract rules with stats for each set");
+  m.def("densCls", &densCls, pybind11::arg("command") = "", "A function to get rules and precision and global accuracy on train and test on a bag of models, training needs to be done before.");
 }
```

### Comparing `dimlpfidex-0.0.0/example/CMakeLists.txt` & `dimlpfidex-0.0.1/example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dimlpfidex-0.0.0/example/cpp/CMakeLists.txt` & `dimlpfidex-0.0.1/example/cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dimlpfidex-0.0.0/fidex/CMakeLists.txt` & `dimlpfidex-0.0.1/fidex/CMakeLists.txt`

 * *Files 11% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 set(CMAKE_CXX_EXTENSIONS OFF)
 
 if(NOT CMAKE_BUILD_TYPE)
     set(CMAKE_BUILD_TYPE Release)
 endif()
 
-set(CMAKE_CXX_FLAGS "-O3")
-set(CMAKE_CXX_FLAGS_RELEASE "-O3")
+set(CMAKE_CXX_FLAGS "-O3 -fopenmp")
+set(CMAKE_CXX_FLAGS_RELEASE "-O3 -fopenmp")
 set(CMAKE_POSITION_INDEPENDENT_CODE ON)
 
 # Enable static compilation for MingW
 # see https://cython.readthedocs.io/en/latest/src/tutorial/appendix.html
 if (WIN32)
     if(MINGW)
         set(CMAKE_C_LINK_EXECUTABLE "${CMAKE_C_LINK_EXECUTABLE} -static-libgcc -Wl,-Bstatic,--whole-archive -lwinpthread -Wl,--no-whole-archive")
@@ -26,14 +26,15 @@
     endif()
 endif()
 
 
 add_subdirectory("cpp")
 include_directories("${CMAKE_SOURCE_DIR}/pybind")
 
+
 file(GLOB PYTHON_FILES "pybind/*.cpp" "pybind/*.h")
 
 # Check Python
 find_package(Python COMPONENTS Interpreter Development REQUIRED)
 if(Python_FOUND)
     message(STATUS "Found Python ${Python_VERSION} ${Python_EXECUTABLE}")
     message(STATUS "Found Python libs: ${Python_LIBRARIES}")
@@ -55,17 +56,23 @@
     include_directories(
         ${pybind11_INCLUDE_DIRS}
     )
 endif()
 
 # Build binding lib
 pybind11_add_module(fidex
-    ${COMMON_SRC_FIDEX}
+    ${FIDEX_COMMON_SRC}
+    ${COMMON_SRC}
     ${FIDEX_SRC}
+    ${FIDEXGLO_SRC}
+    ${FIDEXGLORULES_SRC}
+    ${FIDEXGLOSTATS_SRC}
     ${PYTHON_FILES}
 )
 
 set_target_properties(
     fidex PROPERTIES LIBRARY_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/dimlpfidex
 )
 
-target_link_libraries(fidex PUBLIC)
+target_link_libraries(fidex PUBLIC common)
+
+install(TARGETS fidex LIBRARY DESTINATION ./dimlpfidex)
```

### Comparing `dimlpfidex-0.0.0/fidex/cpp/src/fidexFct.h` & `dimlpfidex-0.0.1/fidex/cpp/src/fidexGloRulesFct.h`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-#ifndef FIDEXFCT_H
-#define FIDEXFCT_H
+#ifndef FIDEXGLORULESFCT_H
+#define FIDEXGLORULESFCT_H
 
-#include "../../../fidexCommon/cpp/src/checkFun.h"
-#include "../../../fidexCommon/cpp/src/dataSet.h"
-#include "../../../fidexCommon/cpp/src/errorHandler.h"
-#include "../../../fidexCommon/cpp/src/hyperLocus.h"
-#include "hyperspace.h"
+#include "../../../common/cpp/src/checkFun.h"
+#include "../../../common/cpp/src/dataSet.h"
+#include "../../../common/cpp/src/errorHandler.h"
+#include "../../../common/cpp/src/parameters.h"
+#include "../../../common/cpp/src/rule.h"
+#include "fidexAlgo.h"
+#include "hyperLocus.h"
 #include <algorithm>
 #include <chrono>
-#include <ctime>
-#include <fstream>
-#include <iostream>
-#include <memory>
+#include <limits.h>
 #include <numeric>
+#include <omp.h>
 #include <random>
 #include <sstream>
+#include <string>
 #include <time.h>
-#include <tuple>
-#include <vector>
 
-void showFidexParams();
-int fidex(const std::string &command);
+void showRulesParams();
+void checkRulesParametersLogicValues(Parameters &p);
+int fidexGloRules(const std::string &command = "");
 
 #endif
```

### Comparing `dimlpfidex-0.0.0/fidexGlo/cpp/src/fidexGloRulesFct.cpp` & `dimlpfidex-0.0.1/fidex/cpp/src/fidexGloFct.cpp`

 * *Files 23% similar despite different names*

```diff
@@ -1,884 +1,604 @@
-#include "fidexGloRulesFct.h"
+#include "fidexGloFct.h"
 
-using namespace std;
+void showParams() {
+  std::cout << std::endl
+            << "---------------------------------------------------------------------" << std::endl
+            << std::endl;
+  std::cout << "Warning! The files are localised with respect to root folder dimlpfidex." << std::endl;
+  std::cout << "The arguments can be specified in the command or in a json configuration file with --json_config_file your_config_file.json." << std::endl
+            << std::endl;
+
+  std::cout << "----------------------------" << std::endl
+            << std::endl;
+  std::cout << "Required parameters:" << std::endl
+            << std::endl;
+
+  printOptionDescription("--test_data_file <str>", "Test sample(s) data file with data and prediction(if no --test_pred_file), classes may been added here if launching with fidex(--with_fidex)");
+  printOptionDescription("--global_rules_file <str>", "Ruleset input file");
+  printOptionDescription("--nb_attributes <int [1,inf[>", "Number of attributes in dataset");
+  printOptionDescription("--nb_classes <int [2,inf[>", "Number of classes in dataset");
+
+  std::cout << std::endl
+            << "----------------------------" << std::endl
+            << std::endl;
+  std::cout << "Optional parameters: " << std::endl
+            << std::endl;
+
+  printOptionDescription("--json_config_file <str>", "JSON file to configure all parameters. If used, this must be the sole argument and must specify the file's relative path");
+  printOptionDescription("--root_folder <str>", "Folder based on main folder dimlpfidex(default folder) containg all used files and where generated files will be saved. If a file name is specified with another option, his path will be configured with respect to this root folder");
+  printOptionDescription("--attributes_file <str>", "File of attributes> Mandatory if rules file contains attribute names, if not, do not add it");
+  printOptionDescription("--test_pred_file <str>", "Test prediction file> if given, --test_data_file needs to have only test datas");
+  printOptionDescription("--explanation_file <str>", "Explanation(s) output file name");
+  printOptionDescription("--console_file <str>", "File with console logs redirection");
+  printOptionDescription("--with_fidex <bool>", "Whether to use Fidex if no rule is found in global rules (default: False)");
+  printOptionDescription("--with_minimal_version <bool>", "Whether to use minimal version, which only gets correct activated rules and if with_fidex, launches Fidex when no such rule is found (default: False)");
+
+  std::cout << std::endl
+            << "----------------------------" << std::endl
+            << std::endl;
+  std::cout << "If using fidex :" << std::endl
+            << std::endl;
+
+  std::cout << "Required :" << std::endl
+            << std::endl;
+  printOptionDescription("--train_data_file <str>", "Train data file");
+  printOptionDescription("--train_pred_file <str>", "Train prediction file");
+  printOptionDescription("--train_class_file <str>", "Train true class file, not mandatory if classes are specified in train data file");
+  printOptionDescription("--weights_file <str>", "Weights file (not mandatory if a rules file is given with --rules_file)");
+  printOptionDescription("--rules_file <str>", "Rules file to be converted to hyperlocus (not mandatory if a weights file is given with --weights_file)");
+
+  std::cout << std::endl
+            << "Optional :" << std::endl
+            << std::endl;
+
+  printOptionDescription("--test_class_file <str>", "Test true class file, classes can be specified in test data file");
+  printOptionDescription("--max_iterations <int [1,inf[>", "Max iteration number, also the max possible number of attributs in a rule, should be 25 if working with images (default: 10)");
+  printOptionDescription("--min_covering <int [1,inf[>", "Minimum covering number (default: 2)");
+  printOptionDescription("--covering_strategy <bool>", "Whether to use this strategy : if no rule is found with min_covering, find best rule with best covering using dichotomic search. Decreases min_fidelity if needed (default: True)");
+  printOptionDescription("--max_failed_attempts <int [0,inf[>", "Maximum number of failed attempts to find Fidex rule when covering is 1 and covering strategy is used (default: 30)");
+  printOptionDescription("--min_fidelity <float [0,1]>", "Minimal rule fidelity accepted when generating a rule (default: 1.0)");
+  printOptionDescription("--lowest_min_fidelity <float [0,1]>", "Minimal min_fidelity to which we agree to go down during covering_strategy (default: 0.75)");
+  printOptionDescription("--dropout_dim <float [0,1]>", "Dimension dropout parameter (default: 0.0)");
+  printOptionDescription("--dropout_hyp <float [0,1]>", "Hyperplan dropout parameter (default: 0.0)");
+  printOptionDescription("--nb_quant_levels <int [3,inf[>", "Number of stairs in staircase activation function (default: 50)");
+  printOptionDescription("--normalization_file <str>", "File containing the mean and std of some attributes. Used to denormalize the rules if specified");
+  printOptionDescription("--mus <list<float ]inf,inf[>>", "Mean or median of each attribute index to denormalize in the rules");
+  printOptionDescription("--sigmas <list<float ]inf,inf[>>", "Standard deviation of each attribute index to denormalize in the rules");
+  printOptionDescription("--normalization_indices <list<int [0,nb_attributes-1]>>", "Attribute indices to denormalize in the rules, only used when no normalization_file is given, index starts at 0 (default: [0,...,nb_attributes-1])");
+  printOptionDescription("--seed <int [0,inf[>", "Seed, 0=random (default: 0)");
+
+  std::cout << std::endl
+            << "----------------------------" << std::endl
+            << std::endl;
+  std::cout << "Execution example :" << std::endl
+            << std::endl;
+  std::cout << "fidex.fidexGlo(\"--test_data_file datanormTest.txt --test_pred_file predTest.out --global_rules_file globalRules.rls --nb_attributes 16 --nb_classes 2 --explanation_file explanation.txt --root_folder dimlp/datafiles --with_fidex true --train_data_file datanormTrain.txt --train_pred_file predTrain.out --train_class_file dataclass2Train.txt --test_class_file dataclass2Test.txt --weights_file weights.wts\")" << std::endl
+            << std::endl;
+  std::cout << "---------------------------------------------------------------------" << std::endl
+            << std::endl;
+}
+
+void executeFidex(std::vector<std::string> &lines, DataSetFid &trainDataset, Parameters &p, Hyperspace &hyperspace, std::vector<double> &mainSampleValues, int mainSamplePred, double mainSamplePredValue, int mainSampleClass, const std::vector<std::string> &attributeNames, const std::vector<std::string> &classNames) {
+
+  std::cout << "\nWe launch Fidex." << std::endl;
+  lines.emplace_back("\nWe launch Fidex.\n");
+
+  Rule rule;
+
+  auto fidex = Fidex(trainDataset, p, hyperspace, true);
+
+  // Launch fidexAlgo
+  fidex.setMainSamplePredValue(mainSamplePredValue);
+  fidex.launchFidex(rule, mainSampleValues, mainSamplePred, mainSampleClass);
 
-void showRulesParams() {
-  std::cout << "\n-------------------------------------------------\n\n";
+  std::cout << "\nLocal rule :" << std::endl;
+  lines.emplace_back("Local rule :\n");
+  std::cout << rule.toString(attributeNames, classNames) << std::endl;
+  lines.emplace_back(rule.toString(attributeNames, classNames) + "\n");
+}
+
+/**
+ * @brief Used to set default hyperparameters values and to check the sanity of all used values like boundaries and logic.
+ *
+ * @param p is the Parameter class containing all hyperparameters that rule the entire algorithm execution.
+ */
+void checkParametersLogicValues(Parameters &p) {
+  // setting default values
+  p.setDefaultBool(WITH_FIDEX, false);
+  p.setDefaultBool(WITH_MINIMAL_VERSION, false);
+
+  // this sections check if values comply with program logic
+
+  // asserting mandatory parameters
+  p.assertStringExists(TEST_DATA_FILE);
+  p.assertStringExists(GLOBAL_RULES_FILE);
+  p.assertIntExists(NB_ATTRIBUTES);
+  p.assertIntExists(NB_CLASSES);
+
+  // verifying logic between parameters, values range and so on...
+  p.checkAttributeAndClassCounts();
+
+  // If using Fidex :
+  if (p.getBool(WITH_FIDEX)) {
+    // setting default values
+    p.setDefaultNbQuantLevels();
+    p.setDefaultFidex();
+
+    // this sections check if values comply with program logic
+
+    // asserting mandatory parameters
+    p.assertStringExists(TRAIN_DATA_FILE);
+    p.assertStringExists(TRAIN_PRED_FILE);
+
+    // verifying logic between parameters, values range and so on...
+    p.checkParametersFidex();
+    p.checkParametersNormalization();
 
-  std::cout << "Obligatory parameters : \n\n";
-  std::cout << "fidexGloRules -T <train dataset file> -P <train prediction file> -C <train true class file> ";
-  std::cout << "-W <weights file. In case of bagging, put prefix of files, ex: DimlpBT, files need to be in the form DimlpBTi.wts, i=1,2,3,... and you need to specify the number of networks with -N> [Not mendatory if a rules file is given with -f] ";
-  std::cout << "-f <rules file to be converted to hyperlocus> [Not mendatory if a weights file is given] ";
-  std::cout << "-O <Rules output file> ";
-  std::cout << "-M <Heuristic 1: optimal fidexGlo, 2: fast fidexGlo 3: very fast fidexGlo> ";
-  std::cout << "<Options>\n\n";
-
-  std::cout << "Options are: \n\n";
-  std::cout << "-S <Folder based on main folder dimlpfidex(default folder) where generated files will be saved. If a file name is specified with another option, his path will be configured with respect to this root folder>\n";
-  std::cout << "-N <number of networks for bagging, 1 means no bagging, necessary to use bagging>";
-  std::cout << "-A <file of attributes>\n";
-  std::cout << "-r <file where you redirect console result>\n"; // If we want to redirect console result to file
-  std::cout << "-i <max iteration number>\n";
-  std::cout << "-v <minimum covering number>\n";
-  std::cout << "-d <dimension dropout parameter>\n";
-  std::cout << "-h <hyperplan dropout parameter>\n";
-  std::cout << "-Q <number of stairs in staircase activation function (50 by default)>\n";
-  std::cout << "-I <high side of the interval (5 by default)>\n";
-  std::cout << "-z <seed (0=ranodom)>";
+    if (p.isStringSet(TEST_CLASS_FILE) && !p.isStringSet(TEST_PRED_FILE)) {
+      throw CommandArgumentException("Error : The test prediction data file(--test_pred_file) needs to be specified if the test class data file(--test_class_file) is given.");
+    }
 
-  std::cout << "\n-------------------------------------------------\n\n";
+    if (p.getInt(NB_QUANT_LEVELS) <= 2) {
+      throw CommandArgumentException("Error : Number of stairs in staircase activation function must be greater than 2.");
+    }
+  }
 }
 
-int fidexGloRules(const string &command) {
+int fidexGlo(const std::string &command) {
+  // Save buffer where we output results
+  std::ofstream ofs;
+  std::streambuf *cout_buff = std::cout.rdbuf(); // Save old buf
   try {
 
     float temps;
     clock_t t1;
     clock_t t2;
 
     t1 = clock();
 
     // Parsing the command
-    vector<string> commandList;
-    const char delim = ' ';
-    string s;
-    stringstream ss(command);
-    while (std::getline(ss, s, delim)) {
+    std::vector<std::string> commandList = {"fidexGlo"};
+    std::string s;
+    std::stringstream ss(command);
+
+    while (ss >> s) {
       commandList.push_back(s);
     }
-    size_t nbParam = commandList.size();
-
-    // Parameters declaration
-
-    int seed = 0;
-
-    string trainDataFileTemp; // Train data
-    bool trainDataFileInit = false;
-    string trainDataFilePredTemp; // Train class predictions from dimlp
-    bool trainDataFilePredInit = false;
-    string trainDataFileTrueClassTemp; // Train true classes
-    bool trainDataFileTrueClassInit = false;
-
-    std::string weightsFileTemp;
-    std::vector<std::string> weightsFilesTemp;
-    string inputRulesFileTemp; // Rule file to be converted to hyperlocus, replace weight file
-    bool inputRulesFileInit = false;
-
-    bool weightsFileInit = false;
-    string rulesFileTemp;
-    bool rulesFileInit = false;
-    string consoleFileTemp;
-    bool consoleFileInit = false;
-    string rootFolderTemp;
-    bool rootFolderInit = false;
-    string attributFileTemp; // attribut file
-    bool attributFileInit = false;
-
-    int nbDimlpNets = 1; // Number of networks. 1 means no bagging
-
-    int nbQuantLevels = 50; // Number of steps of the step function
-    double hiKnot = 5;      // High end of the interval for each dimension, a hyperplan can't be after
-
-    int heuristic = -1;
-    bool heuristicInit = false;
-
-    int itMax = 100;         // We stop if we have more than itMax iterations
-    int minNbCover = 2;      // Minimum size of covering that we ask
-    bool dropoutHyp = false; // We dropout a bunch of hyperplans each iteration (could accelerate the processus)
-    double dropoutHypParam = 0.5;
-    bool dropoutDim = false; // We dropout a bunch of dimensions each iteration (could accelerate the processus)
-    double dropoutDimParam = 0.5;
-
-    int nbRules; // Number of rules created
+    std::size_t nbParam = commandList.size();
+    if (nbParam < 2 || commandList[1] == "-h" || commandList[1] == "--help") {
+      showParams();
+      return 0;
+    }
 
     // Import parameters
-
-    if (nbParam <= 1) {
-      showRulesParams();
-      return 0;
+    std::unique_ptr<Parameters> params;
+    std::vector<ParameterCode> validParams = {TEST_DATA_FILE, GLOBAL_RULES_FILE, NB_ATTRIBUTES, NB_CLASSES, ROOT_FOLDER, ATTRIBUTES_FILE,
+                                              TEST_PRED_FILE, EXPLANATION_FILE, CONSOLE_FILE,
+                                              WITH_FIDEX, WITH_MINIMAL_VERSION, TRAIN_DATA_FILE, TRAIN_PRED_FILE, TRAIN_CLASS_FILE, WEIGHTS_FILE,
+                                              RULES_FILE, TEST_CLASS_FILE, MAX_ITERATIONS, MIN_COVERING, COVERING_STRATEGY,
+                                              MAX_FAILED_ATTEMPTS, MIN_FIDELITY, LOWEST_MIN_FIDELITY, DROPOUT_DIM, DROPOUT_HYP, NB_QUANT_LEVELS,
+                                              NORMALIZATION_FILE, MUS, SIGMAS, NORMALIZATION_INDICES, SEED};
+    if (commandList[1].compare("--json_config_file") == 0) {
+      if (commandList.size() < 3) {
+        throw CommandArgumentException("JSON config file name/path is missing");
+      } else if (commandList.size() > 3) {
+        throw CommandArgumentException("Option " + commandList[1] + " has to be the only option in the command if specified.");
+      }
+      try {
+        params = std::unique_ptr<Parameters>(new Parameters(commandList[2], validParams));
+      } catch (const std::out_of_range &e) {
+        throw CommandArgumentException("Some value inside your JSON config file '" + commandList[2] + "' is out of range.\n(Probably due to a too large or too tiny numeric value).");
+      } catch (const std::exception &e) {
+        std::string msg(e.what()) ;
+        throw CommandArgumentException("Unknown JSON config file error: " + msg);
+      }
+    } else {
+      // Read parameters from CLI
+      params = std::unique_ptr<Parameters>(new Parameters(commandList, validParams));
     }
 
-    int p = 1; // We skip "fidexGloRules"
-    while (p < nbParam) {
-      if (commandList[p][0] == '-') {
-        p++;
+    // getting all program arguments from CLI
+    checkParametersLogicValues(*params);
 
-        if (p >= nbParam) {
-          throw CommandArgumentException("Missing something at the end of the command.");
-        }
+    // Get console results to file
+    if (params->isStringSet(CONSOLE_FILE)) {
+      std::string consoleFile = params->getString(CONSOLE_FILE);
+      ofs.open(consoleFile);
+      std::cout.rdbuf(ofs.rdbuf()); // redirect std::cout to file
+    }
 
-        char option = commandList[p - 1][1];
-        const char *arg = &(commandList[p])[0];
-        const char *lastArg = &(commandList[p - 1])[0];
-        switch (option) { // Get letter after the -
-
-        case 'T':
-          trainDataFileTemp = arg; // Parameter after -T
-          trainDataFileInit = true;
-          break;
-
-        case 'P':
-          trainDataFilePredTemp = arg;
-          trainDataFilePredInit = true;
-          break;
-
-        case 'C':
-          trainDataFileTrueClassTemp = arg;
-          trainDataFileTrueClassInit = true;
-          break;
-
-        case 'W': {
-          weightsFileTemp = arg;
-          weightsFileInit = true;
-        } break;
-
-        case 'f': {
-          inputRulesFileTemp = arg;
-          inputRulesFileInit = true;
-        } break;
-
-        case 'N':
-          if (CheckPositiveInt(arg))
-            nbDimlpNets = atoi(arg);
-          else
-            return -1;
-
-          break;
-
-        case 'Q':
-          if (CheckPositiveInt(arg)) {
-            nbQuantLevels = atoi(arg);
-          } else {
-            throw CommandArgumentException("Error : invalide type for parameter " + std::string(lastArg) + ", positive integer requested");
-          }
-          break;
+    // Show chosen parameters
+    std::cout << *params;
 
-        case 'I':
-          if (CheckFloatFid(arg) && atof(arg) > 0) {
-            hiKnot = atof(arg);
-          } else {
-            throw CommandArgumentException("Error : invalide type for parameter " + std::string(lastArg) + ", strictly positive float requested");
-          }
-          break;
+    // ----------------------------------------------------------------------
 
-        case 'O':
-          rulesFileTemp = arg;
-          rulesFileInit = true;
-          break;
-
-        case 'r':
-          consoleFileTemp = arg;
-          consoleFileInit = true;
-          break;
-
-        case 'A':
-          attributFileTemp = arg;
-          attributFileInit = true;
-          break;
-
-        case 'S':
-          rootFolderTemp = arg;
-          rootFolderInit = true;
-          break;
-
-        case 'M':
-          if (CheckPositiveInt(arg) && atoi(arg) >= 1 && atoi(arg) <= 3) {
-            heuristic = atoi(arg);
-            heuristicInit = true;
-          } else {
-            throw CommandArgumentException("Error : invalide type for parameter " + string(lastArg) + ", heuristic must be an integer between 1 and 3(1: optimal fidexGlo, 2: fast fidexGlo 3: very fast fidexGlo)");
-          }
-          break;
+    // Get parameters values
 
-        case 'i':
-          if (CheckPositiveInt(arg)) {
-            itMax = atoi(arg);
-          } else {
-            throw CommandArgumentException("Error : invalide type for parameter " + string(lastArg) + ", positive integer requested");
-          }
-          break;
+    int nbAttributes = params->getInt(NB_ATTRIBUTES);
+    int nbClasses = params->getInt(NB_CLASSES);
+    std::string testSamplesDataFile = params->getString(TEST_DATA_FILE);
+    bool withFidex = params->getBool(WITH_FIDEX);
+    bool minimalVersion = params->getBool(WITH_MINIMAL_VERSION);
+    float decisionThreshold;
+    int positiveClassIndex;
+    getThresholdFromRulesFile(params->getString(GLOBAL_RULES_FILE), decisionThreshold, positiveClassIndex);
 
-        case 'v':
-          if (CheckPositiveInt(arg) && atoi(arg) >= 1) {
-            minNbCover = atoi(arg);
-          } else {
-            throw CommandArgumentException("Error : invalide type for parameter " + string(lastArg) + ", strictly positive integer requested");
-          }
-          break;
+    // ----------------------------------------------------------------------
 
-        case 'd':
-          if (CheckFloatFid(arg) && atof(arg) >= 0 && atof(arg) <= 1) {
-            dropoutDimParam = atof(arg);
-            dropoutDim = true; // We dropout a bunch of dimensions each iteration (accelerate the processus)
-          } else {
-            throw CommandArgumentException("Error : invalide type for parameter " + string(lastArg) + ", float included in [0,1] requested");
-          }
-          break;
+    std::cout << "Importing files..." << std::endl
+              << std::endl;
 
-        case 'h':
-          if (CheckFloatFid(arg) && atof(arg) >= 0 && atof(arg) <= 1) {
-            dropoutHypParam = atof(arg);
-            dropoutHyp = true; // We dropout a bunch of hyperplans each iteration (accelerate the processus)
-          } else {
-            throw CommandArgumentException("Error : invalide type for parameter " + string(lastArg) + ", float included in [0,1] requested");
-          }
-          break;
+    // Get test data
 
-        case 'z':
-          if (CheckPositiveInt(arg))
-            seed = atoi(arg);
-          else
-            throw CommandArgumentException("Error : invalide type for parameter " + string(lastArg) + ", positive integer requested");
+    std::unique_ptr<DataSetFid> testDatas;
+    if (!params->isStringSet(TEST_PRED_FILE)) { // If we have only one test data file with data and prediction
+      testDatas.reset(new DataSetFid("testDatas from FidexGlo", testSamplesDataFile, nbAttributes, nbClasses, decisionThreshold, positiveClassIndex));
+    } else { // We have a different file for test predictions
+      testDatas.reset(new DataSetFid("testDatas from FidexGlo", testSamplesDataFile, params->getString(TEST_PRED_FILE), nbAttributes, nbClasses, decisionThreshold, positiveClassIndex));
+    }
+    std::vector<std::vector<double>> testSamplesValues = testDatas->getDatas();
+    std::vector<int> testSamplesPreds = testDatas->getPredictions();
+    std::vector<std::vector<double>> testSamplesOutputValuesPredictions = testDatas->getOutputValuesPredictions();
 
-          break;
+    int nbSamples = testDatas->getNbSamples();
 
-        default: // If we put another -X option
-          throw CommandArgumentException("Illegal option : " + string(lastArg));
-        }
+    // Get attributes
+    std::vector<std::string> attributeNames;
+    std::vector<std::string> classNames;
+    bool hasClassNames = false;
+    if (params->isStringSet(ATTRIBUTES_FILE)) {
+      testDatas->setAttributes(params->getString(ATTRIBUTES_FILE), nbAttributes, nbClasses);
+      attributeNames = testDatas->getAttributeNames();
+      hasClassNames = testDatas->getHasClassNames();
+      if (hasClassNames) {
+        classNames = testDatas->getClassNames();
       }
-
-      p++;
     }
 
-    // Fill weights vector
-    if (weightsFileInit) {
-      if (nbDimlpNets == 1) {
-        weightsFilesTemp.push_back(weightsFileTemp);
-      } else {
-        for (int n = 0; n < nbDimlpNets; n++) {
-          weightsFilesTemp.push_back(weightsFileTemp + std::to_string(n + 1) + ".wts");
+    // If we use Fidex
+    std::vector<int> testSamplesClasses;
+    std::unique_ptr<DataSetFid> trainDatas;
+    std::vector<std::vector<double>> matHypLocus;
+    bool hasTrueClasses;
+    if (withFidex) {
+
+      std::vector<int> normalizationIndices;
+      std::vector<double> mus;
+      std::vector<double> sigmas;
+
+      // Get mus, sigmas and normalizationIndices from normalizationFile for denormalization :
+      if (params->isStringSet(NORMALIZATION_FILE)) {
+        auto results = parseNormalizationStats(params->getString(NORMALIZATION_FILE), params->getInt(NB_ATTRIBUTES), attributeNames);
+        normalizationIndices = std::get<0>(results);
+        mus = std::get<2>(results);
+        sigmas = std::get<3>(results);
+        params->setIntVector(NORMALIZATION_INDICES, normalizationIndices);
+        params->setDoubleVector(MUS, mus);
+        params->setDoubleVector(SIGMAS, sigmas);
+      }
+
+      // Import files for Fidex
+      std::cout << "Importing files for Fidex..." << std::endl;
+
+      // Get test class data :
+      hasTrueClasses = true;
+      if (!params->isStringSet(TEST_CLASS_FILE)) {
+        if (!testDatas->getHasClasses()) {
+          hasTrueClasses = false;
         }
+      } else {
+        testDatas->setClassFromFile(params->getString(TEST_CLASS_FILE), nbClasses);
+      }
+      if (hasTrueClasses) {
+        testSamplesClasses = testDatas->getClasses();
       }
-    }
-
-    // ----------------------------------------------------------------------
-    // create paths with root foler
-
-    const char *trainDataFile = nullptr;
-    const char *trainDataFilePred = nullptr;
-    const char *trainDataFileTrueClass = nullptr;
-    const char *rulesFile = nullptr;
-    std::vector<const char *> weightsFiles;
-    const char *inputRulesFile = nullptr;
-    const char *consoleFile = nullptr;
-    const char *attributFile = nullptr;
-
-    string root = "";
-    if (rootFolderInit) {
-#if defined(__unix__) || defined(__APPLE__)
-      root = rootFolderTemp + "/";
-#elif defined(_WIN32)
-      root = rootFolderTemp + "\\";
-#endif
-    }
-
-    if (trainDataFileInit) {
-      trainDataFileTemp = root + trainDataFileTemp;
-      trainDataFile = &trainDataFileTemp[0];
-    }
-
-    if (trainDataFilePredInit) {
-      trainDataFilePredTemp = root + trainDataFilePredTemp;
-      trainDataFilePred = &trainDataFilePredTemp[0];
-    }
 
-    if (trainDataFileTrueClassInit) {
-      trainDataFileTrueClassTemp = root + trainDataFileTrueClassTemp;
-      trainDataFileTrueClass = &trainDataFileTrueClassTemp[0];
-    }
+      if (!params->isStringSet(TRAIN_CLASS_FILE)) {
+        trainDatas.reset(new DataSetFid("trainDatas from FidexGloRules",
+                                        params->getString(TRAIN_DATA_FILE),
+                                        params->getString(TRAIN_PRED_FILE),
+                                        params->getInt(NB_ATTRIBUTES),
+                                        params->getInt(NB_CLASSES),
+                                        decisionThreshold,
+                                        positiveClassIndex));
 
-    if (rulesFileInit) {
-      rulesFileTemp = root + rulesFileTemp;
-      rulesFile = &rulesFileTemp[0];
-    }
+        if (!trainDatas->getHasClasses()) {
+          throw CommandArgumentException("The train true classes file has to be given with option --train_class_file or classes have to be given in the train data file.");
+        }
+      } else {
+        trainDatas.reset(new DataSetFid("trainDatas from FidexGloRules",
+                                        params->getString(TRAIN_DATA_FILE),
+                                        params->getString(TRAIN_PRED_FILE),
+                                        params->getInt(NB_ATTRIBUTES),
+                                        params->getInt(NB_CLASSES),
+                                        decisionThreshold,
+                                        positiveClassIndex,
+                                        params->getString(TRAIN_CLASS_FILE)));
+      }
 
-    if (weightsFileInit) {
-      for (int i; i < weightsFilesTemp.size(); i++) {
-        weightsFilesTemp[i] = root + weightsFilesTemp[i];
-        weightsFiles.push_back(&weightsFilesTemp[i][0]);
+      int nbTrainSamples = trainDatas->getNbSamples();
+      if (params->getInt(MIN_COVERING) > nbTrainSamples) {
+        throw CommandArgumentException("Error : invalide type for parameter --min_covering, strictly positive integer smaller or equal than the number of train data samples requested.");
       }
-    }
 
-    if (inputRulesFileInit) {
-      inputRulesFileTemp = root + inputRulesFileTemp;
-      inputRulesFile = &inputRulesFileTemp[0];
-    }
+      // compute hyperspace
 
-    if (consoleFileInit) {
-      consoleFileTemp = root + consoleFileTemp;
-      consoleFile = &consoleFileTemp[0];
-    }
+      std::cout << "Creation of hyperspace..." << std::endl;
 
-    if (attributFileInit) {
-      attributFileTemp = root + attributFileTemp;
-      attributFile = &attributFileTemp[0];
-    }
+      std::string weightsFile;
+      if (params->isStringSet(WEIGHTS_FILE)) {
+        weightsFile = params->getString(WEIGHTS_FILE);
+      }
+      std::string inputRulesFile;
+      if (params->isStringSet(RULES_FILE)) {
+        inputRulesFile = params->getString(RULES_FILE);
+      }
+      int nbQuantLevels = params->getInt(NB_QUANT_LEVELS);
+      float hiKnot = params->getFloat(HI_KNOT);
 
-    // ----------------------------------------------------------------------
+      if (params->isStringSet(WEIGHTS_FILE)) {
+        matHypLocus = calcHypLocus(weightsFile, nbQuantLevels, hiKnot); // Get hyperlocus
+      } else {
+        matHypLocus = calcHypLocus(inputRulesFile, *testDatas);
+      }
 
-    if (!trainDataFileInit) {
-      throw CommandArgumentException("The train data file has to be given with option -T");
-    }
-    if (!trainDataFilePredInit) {
-      throw CommandArgumentException("The train prediction file has to be given with option -P");
-    }
-    if (!trainDataFileTrueClassInit) {
-      throw CommandArgumentException("The train true classes file has to be given with option -C");
-    }
-    if (!weightsFileInit && !inputRulesFileInit) {
-      throw CommandArgumentException("A weight file or a rules file has to be given. Give the weights file with option -W or the rules file with option -f");
-    } else if (weightsFileInit && inputRulesFileInit) {
-      throw CommandArgumentException("Do not specify both a weight file(-W) and a rules file(-f). Choose one of them.");
-    }
-    if (!rulesFileInit) {
-      throw CommandArgumentException("The output rules file has to be given with option -O");
-    }
-    if (!heuristicInit) {
-      throw CommandArgumentException("The heuristic(1: optimal fidexGlo, 2: fast fidexGlo 3: very fast fidexGlo) has to be given with option -M");
-    }
+      // Number of neurons in the first hidden layer (May be the number of input variables or a multiple)
+      auto nbIn = static_cast<int>(matHypLocus.size());
 
-    // ----------------------------------------------------------------------
+      // Check size of hyperlocus
+      if (nbIn == 0 || nbIn % nbAttributes != 0) {
+        throw InternalError("Error : the size of hyperLocus - " + std::to_string(nbIn) + " is not a multiple of the number of attributs - " + std::to_string(nbAttributes));
+      }
 
-    // Get console results to file
-    std::ofstream ofs;
-    std::streambuf *cout_buff = std::cout.rdbuf(); // Save old buf
-    if (consoleFileInit != false) {
-      ofs.open(consoleFile);
-      std::cout.rdbuf(ofs.rdbuf()); // redirect std::cout to file
+      std::cout << "Hyperspace created." << std::endl
+                << std::endl;
     }
 
-    // ----------------------------------------------------------------------
-
-    std::cout << "\nParameters :\n\n";
-    std::cout << "- Max iteration number : " << itMax << endl;
-    std::cout << "- Min size of covering : " << minNbCover << endl;
-    if (dropoutDim) {
-      std::cout << "- We use a dimension dropout of " << dropoutDimParam << endl
-                << endl;
-    } else {
-      std::cout << "- We don't use dimension dropout\n\n";
-    }
-    if (dropoutHyp) {
-      std::cout << "- We use a hyperplan dropout of " << dropoutHypParam << endl
-                << endl;
-    } else {
-      std::cout << "- We don't use hyperplan dropout\n\n";
-    }
+    // Get rules
+    std::vector<Rule> rules;
+    std::vector<std::string> lines;
+    std::string statsLine;
+    std::fstream rulesData;
+    std::string rulesFile = params->getString(GLOBAL_RULES_FILE);
+    lines.emplace_back("Global statistics of the rule set : ");
 
-    // Import files
+    if (rulesFile.substr(rulesFile.find_last_of(".") + 1) == "json") {
+      rules = Rule::fromJsonFile(rulesFile, decisionThreshold, positiveClassIndex);
 
-    std::cout << "Import files..." << endl;
+      double meanCovering = 0;
+      double meanNbAntecedantsPerRule = 0;
+      auto nbRules = static_cast<int>(rules.size());
 
-    std::unique_ptr<DataSetFid> trainDatas(new DataSetFid(trainDataFile, trainDataFilePred, trainDataFileTrueClass));
+      for (Rule r : rules) {
+        meanCovering += static_cast<double>(r.getCoveredSamples().size());
+        meanNbAntecedantsPerRule += static_cast<double>(r.getAntecedants().size());
+      }
+      meanCovering /= nbRules;
+      meanNbAntecedantsPerRule /= nbRules;
 
-    vector<vector<double>> *trainData = trainDatas->getDatas();
-    vector<int> *trainPreds = trainDatas->getPredictions();
+      statsLine += "Number of rules : " + std::to_string(nbRules);
+      statsLine += ", mean sample covering number per rule : ";
+      statsLine += std::to_string(meanCovering) + ", mean number of antecedents per rule : ";
+      statsLine += std::to_string(meanNbAntecedantsPerRule) + "\n";
 
-    vector<vector<double>> *trainOutputValuesPredictions = nullptr;
-    bool hasConfidence;
-    if (trainDatas->hasConfidence()) {
-      trainOutputValuesPredictions = trainDatas->getOutputValuesPredictions();
-      hasConfidence = true;
     } else {
-      hasConfidence = false;
-    }
-    vector<int> *trainTrueClass = trainDatas->getTrueClasses();
-
-    const auto nbDatas = static_cast<int>((*trainData).size());
-    const auto nbAttributs = static_cast<int>((*trainData)[0].size());
-    const auto nbClass = trainDatas->getNbClasses();
-    if ((*trainPreds).size() != nbDatas || (*trainTrueClass).size() != nbDatas) {
-      throw FileFormatError("All the train files need to have the same amount of datas");
+      rulesData.open(rulesFile, std::ios::in); // Read data file
+      if (rulesData.fail()) {
+        throw FileNotFoundError("Error : file " + rulesFile + " not found.");
+      }
+      getline(rulesData, statsLine);
+      statsLine += "\n";
+      getRules(rules, rulesFile, *testDatas, decisionThreshold, positiveClassIndex);
     }
+    lines.emplace_back(statsLine);
 
-    if (minNbCover > nbDatas) {
-      throw CommandArgumentException("Error : invalide type for parameter -c, strictly positive integer smaller or equal than the number of data sample requested");
+    std::cout << "Files imported" << std::endl
+              << std::endl;
+    if (nbSamples > 1) {
+      std::cout << "Find explanation for each sample..." << std::endl
+                << std::endl;
     }
 
-    // Get attributes
-    vector<string> attributeNames;
-    vector<string> classNames;
-    bool hasClassNames = false;
-    if (attributFileInit) {
-      std::unique_ptr<Attribute> attributesData(new Attribute(attributFile));
-      attributeNames = (*attributesData->getAttributes());
-      if (attributeNames.size() < nbAttributs) {
-        throw FileContentError("Error : in file " + std::string(attributFile) + ", there is not enough attribute names");
-      } else if (attributeNames.size() == nbAttributs) {
-        hasClassNames = false;
-      } else if (attributeNames.size() != nbAttributs + nbClass) {
-        throw FileContentError("Error : in file " + std::string(attributFile) + ", there is not the good amount of attribute and class names");
+    if (decisionThreshold != -1) {
+      std::string classDecision;
+      if (hasClassNames) {
+        classDecision = classNames[positiveClassIndex];
       } else {
-        hasClassNames = true;
-        auto firstEl = attributeNames.end() - nbClass;
-        auto lastEl = attributeNames.end();
-        classNames.insert(classNames.end(), firstEl, lastEl);
-        attributeNames.erase(firstEl, lastEl);
-      }
-    }
-
-    std::cout << "Files imported" << endl
-              << endl;
-
-    // compute hyperspace
-
-    std::cout << "Creation of hyperspace..." << endl;
-
-    std::vector<std::vector<double>> matHypLocus;
-
-    if (weightsFileInit) {
-      for (const auto &weightsFile : weightsFiles) {
-        std::vector<std::vector<double>> hypLocus = calcHypLocus(weightsFile, nbQuantLevels, hiKnot); // Get hyperlocus
-        matHypLocus.insert(matHypLocus.end(), hypLocus.begin(), hypLocus.end());                      // Concatenate hypLocus to matHypLocus
+        classDecision = std::to_string(positiveClassIndex);
       }
-    } else {
-      matHypLocus = calcHypLocus(inputRulesFile, nbAttributs);
-    }
-
-    FidexGloNameSpace::Hyperspace hyperspace(matHypLocus); // Initialize hyperbox and get hyperplans
-
-    const auto nbIn = static_cast<int>(hyperspace.getHyperLocus().size()); // Number of neurons in the first hidden layer (May be the number of input variables or a multiple)
-
-    // Check size of hyperlocus
-    if (nbIn == 0 || nbIn % nbAttributs != 0) {
-      throw InternalError("Error : the size of hyperLocus - " + std::to_string(nbIn) + " is not a multiple of the number of attributs - " + std::to_string(nbAttributs));
+      lines.emplace_back("Using a decision threshold of " + formattingDoubleToString(decisionThreshold) + " for class " + classDecision + "\n");
     }
 
-    std::cout << "Hyperspace created" << endl
-              << endl;
+    lines.emplace_back("\n--------------------------------------------------------------------\n");
+    std::cout << "\n--------------------------------------------------------------------" << std::endl;
 
-    // Samples not yet covered by any rules
-    vector<int> notCoveredSamples(nbDatas);
-    std::iota(std::begin(notCoveredSamples), std::end(notCoveredSamples), 0); // Vector from 0 to nbDatas-1
+    // we search explanation for each sample
 
-    vector<tuple<vector<tuple<int, bool, double>>, vector<int>, int, double, double>> chosenRules; // antecedents, cover vector, class, rule accuracy, rule confidence
-
-    //--------------------------------------------------------------------------------------------------------------------
-    //--------------------------------------------------------------------------------------------------------------------
-
-    // Initialize random number generator
-
-    if (seed == 0) {
-      auto currentTime = std::chrono::high_resolution_clock::now();
-      auto seedValue = currentTime.time_since_epoch().count();
-      seed = static_cast<unsigned int>(seedValue);
+    if (nbSamples == 1) {
+      lines.emplace_back("Explanation for the sample :\n");
+      std::cout << "Explanation for the sample :" << std::endl
+                << std::endl;
     }
-    std::mt19937 gen(seed);
-
-    // First heuristic : optimal (slower)
-    float temps1;
-    clock_t c1;
-    clock_t c2;
-
-    c1 = clock();
-    if (heuristic == 1) {
-      std::cout << "Optimal FidexGlo" << endl
-                << endl;
-
-      vector<tuple<vector<tuple<int, bool, double>>, vector<int>, int, double, double>> rules;
-      bool ruleCreated;
-      int nbProblems = 0;
-      int nbRulesNotFound = 0;
-      int currentMinNbCov;
-      tuple<vector<tuple<int, bool, double>>, vector<int>, int, double, double> rule; // Ex: ([X2<3.5 X3>=4], covering, class)
-      auto exp = FidexAlgo();
-
-      // Get the rule for each data sample from fidex
-      std::cout << "Computing fidex rules..." << endl
-                << endl;
-
-      for (int idSample = 0; idSample < nbDatas; idSample++) {
-
-        if (int(nbDatas / 100) != 0 && idSample % int(nbDatas / 100) == 0 && consoleFileInit == false) {
-          cout << "Processing : " << int((double(idSample) / nbDatas) * 100) << "%\r";
-          std::cout.flush();
-        }
-        currentMinNbCov = minNbCover;
-        ruleCreated = false;
-        int counterFailed = 0; // If we can't find a good rule after a lot of tries
-        while (!ruleCreated) {
-          ruleCreated = exp.fidex(rule, trainData, trainPreds, hasConfidence, trainOutputValuesPredictions, trainTrueClass, &(*trainData)[idSample], (*trainPreds)[idSample], &hyperspace, nbIn, nbAttributs, itMax, currentMinNbCov, dropoutDim, dropoutDimParam, dropoutHyp, dropoutHypParam, gen);
-          if (currentMinNbCov >= 2) {
-            currentMinNbCov -= 1; // If we didnt found a rule with desired covering, we check with a lower covering
+    int nb_fidex = 0; // Number of times Fidex is used
+    bool launchingFidex;
+    for (int currentSample = 0; currentSample < nbSamples; currentSample++) {
+      launchingFidex = false;
+      if (nbSamples > 1) {
+        lines.push_back("Explanation for sample " + std::to_string(currentSample) + " :\n");
+        std::cout << "Explanation for sample " << std::to_string(currentSample) << " :" << std::endl
+                  << std::endl;
+      }
+      int currentPredId = testSamplesPreds[currentSample];
+      std::string currentPred;
+      if (hasClassNames) {
+        currentPred = classNames[currentPredId];
+      } else {
+        currentPred = std::to_string(currentPredId);
+      }
+      lines.emplace_back("The model predict class " + currentPred + " with probability " + std::to_string(testSamplesOutputValuesPredictions[currentSample][currentPredId]) + "\n");
+      std::cout << "The model predict class " << currentPred << " with probability " << std::to_string(testSamplesOutputValuesPredictions[currentSample][currentPredId]) << std::endl
+                << std::endl;
+      // Find rules activated by this sample
+      std::vector<int> activatedRules;
+      getActivatedRules(activatedRules, rules, testSamplesValues[currentSample]);
+      // Check which rules are correct
+      std::vector<int> correctRules;
+      std::vector<int> notcorrectRules;
+      bool notShowUncorrectRules = false;
+      if (activatedRules.empty()) { // If there is no activated rule
+        std::cout << "There is no rule activated" << std::endl;
+        std::cout << "We couldn't find any global explanation for this sample." << std::endl; // There is no explanation, we choose the model decision
+        std::cout << "We choose the model prediction." << std::endl;
+        std::cout << "The predicted class is " << std::to_string(testSamplesPreds[currentSample]) << std::endl;
+        lines.emplace_back("We couldn't find any global explanation for this sample."); // There is no explanation, we choose the model decision
+        lines.emplace_back("We choose the model prediction.");
+        lines.emplace_back("The predicted class is " + std::to_string(testSamplesPreds[currentSample]));
+        if (withFidex) {
+          launchingFidex = true;
+          nb_fidex += 1;
+        }
+
+      } else { // There are some activated rules
+        for (int v : activatedRules) {
+          if (rules[v].getOutputClass() == testSamplesPreds[currentSample]) { // Check if the class of the rule is the predicted one
+            correctRules.push_back(v);
           } else {
-            counterFailed += 1;
-          }
-          if (counterFailed >= 30) {
-            nbRulesNotFound += 1;
-            auto it = std::find(notCoveredSamples.begin(), notCoveredSamples.end(), idSample);
-            if (it != notCoveredSamples.end()) {
-              notCoveredSamples.erase(it);
-            }
-            break;
+            notcorrectRules.push_back(v);
           }
         }
-        if (currentMinNbCov + 1 < minNbCover) {
-          nbProblems += 1;
-        }
-
-        rules.push_back(rule);
-      }
-
-      std::cout << "\nNumber of sample with lower covering than " << minNbCover << " : " << nbProblems << endl;
-      if (nbRulesNotFound > 0) {
-        std::cout << "Number of rules not found : " << nbRulesNotFound << endl;
-      }
-
-      std::cout << "Fidex rules computed" << endl
-                << endl;
-
-      std::cout << "Computing global ruleset..." << endl
-                << endl;
-
-      nbRules = 0;
-
-      // While there is some not covered samples
-      tuple<vector<tuple<int, bool, double>>, vector<int>, int, double, double> currentRule;
-      std::vector<int>::iterator ite;
-      vector<int> newNotCoveredSamples;
-      vector<int> bestNewNotCoveredSamples;
-      while (!notCoveredSamples.empty()) {
-
-        // Get rule that covers the most new samples
-        int bestRule = -1;
-        int bestCovering = INT_MAX;
-        int currentCovering; // Size of new covering if we choose this rule
-        for (int r = 0; r < rules.size(); r++) {
-          newNotCoveredSamples = notCoveredSamples;
-          // Remove samples that are in current covering
-          ite = std::set_difference(newNotCoveredSamples.begin(), newNotCoveredSamples.end(), get<1>(rules[r]).begin(), get<1>(rules[r]).end(), newNotCoveredSamples.begin()); // vectors have to be sorted
-          newNotCoveredSamples.resize(ite - newNotCoveredSamples.begin());
-          currentCovering = static_cast<int>(newNotCoveredSamples.size());
-
-          if (currentCovering < bestCovering) {
-            bestRule = r;
-            bestCovering = currentCovering;
-            bestNewNotCoveredSamples = newNotCoveredSamples;
+        if (correctRules.empty()) { // If there is no correct rule
+          int ancientClass = rules[activatedRules[0]].getOutputClass();
+          bool allSameClass = true; // Check if all the rules choose the same class
+          for (int v : activatedRules) {
+            if (rules[v].getOutputClass() != ancientClass) {
+              allSameClass = false;
+              break;
+            }
           }
-        }
-        currentRule = rules[bestRule];
-        notCoveredSamples = bestNewNotCoveredSamples; // Delete new covered samples
-        nbRules += 1;
-        chosenRules.push_back(currentRule);    // add best rule with maximum covering
-        rules.erase(rules.begin() + bestRule); // Remove this rule
-      }
-
-      std::cout << "Global ruleset Computed" << endl
-                << endl;
-
-      std::cout << "We created " << nbRules << " rules." << endl
-                << endl;
-
-      c2 = clock();
-      temps1 = (float)(c2 - c1) / CLOCKS_PER_SEC;
-      std::cout << "\nTime first heuristic = " << temps1 << " sec\n\n";
-    }
-
-    //--------------------------------------------------------------------------------------------------------------------
-    //--------------------------------------------------------------------------------------------------------------------
-
-    // Second heuristic : fast
-    float temps2;
-    clock_t d1;
-    clock_t d2;
-
-    d1 = clock();
-    if (heuristic == 2) {
-      std::cout << "Fast FidexGlo" << endl
-                << endl;
-
-      vector<tuple<vector<tuple<int, bool, double>>, vector<int>, int, double, double>> rules;
-      bool ruleCreated;
-      int nbProblems = 0;
-      int nbRulesNotFound = 0;
-      int currentMinNbCov;
-      tuple<vector<tuple<int, bool, double>>, vector<int>, int, double, double> rule; // Ex: ([X2<3.5 X3>=4], covering, class)
-      auto exp = FidexAlgo();
-
-      // Get the rule for each data sample from fidex
-      std::cout << "Computing fidex rules..." << endl
-                << endl;
-      for (int idSample = 0; idSample < nbDatas; idSample++) {
-
-        if (int(nbDatas / 100) != 0 && idSample % int(nbDatas / 100) == 0 && consoleFileInit == false) {
-          cout << "Processing : " << int((double(idSample) / nbDatas) * 100) << "%\r";
-          std::cout.flush();
-        }
-        currentMinNbCov = minNbCover;
-        ruleCreated = false;
-        int counterFailed = 0; // If we can't find a good rule after a lot of tries
-        while (!ruleCreated) {
-          ruleCreated = exp.fidex(rule, trainData, trainPreds, hasConfidence, trainOutputValuesPredictions, trainTrueClass, &(*trainData)[idSample], (*trainPreds)[idSample], &hyperspace, nbIn, nbAttributs, itMax, currentMinNbCov, dropoutDim, dropoutDimParam, dropoutHyp, dropoutHypParam, gen);
-          if (currentMinNbCov >= 2) {
-            currentMinNbCov -= 1; // If we didnt found a rule with desired covering, we check with a lower covering
+          if (allSameClass && !minimalVersion) {
+            notShowUncorrectRules = true;
+            if (activatedRules.size() > 1) {
+              lines.emplace_back("We didn't found any rule with same prediction as the model (class " + std::to_string(testSamplesPreds[currentSample]) + "), but we found " + std::to_string(activatedRules.size()) + " rules with class " + std::to_string(ancientClass) + " :\n");
+              std::cout << "We didn't found any rule with same prediction as the model (class " << std::to_string(testSamplesPreds[currentSample]) << "), but we found " << std::to_string(activatedRules.size()) << " rules with class " << std::to_string(ancientClass) << " :" << std::endl
+                        << std::endl;
+            } else {
+              lines.emplace_back("We didn't found any rule with same prediction as the model (class " + std::to_string(testSamplesPreds[currentSample]) + "), but we found 1 rule with class " + std::to_string(ancientClass) + " :\n");
+              std::cout << "We didn't found any rule with same prediction as the model (class " << std::to_string(testSamplesPreds[currentSample]) << "), but we found 1 rule with class " << std::to_string(ancientClass) << " :" << std::endl
+                        << std::endl;
+            }
+            for (int v = 0; v < activatedRules.size(); v++) {
+              lines.emplace_back("R" + std::to_string(v + 1) + ": " + rules[activatedRules[v]].toString(attributeNames, classNames));
+              std::cout << "R" << std::to_string(v + 1) << ": " << rules[activatedRules[v]].toString(attributeNames, classNames) << std::endl;
+            }
           } else {
-            counterFailed += 1;
-          }
-          if (counterFailed >= 30) {
-            nbRulesNotFound += 1;
-            auto it = std::find(notCoveredSamples.begin(), notCoveredSamples.end(), idSample);
-            if (it != notCoveredSamples.end()) {
-              notCoveredSamples.erase(it);
+            if (minimalVersion) {
+              std::cout << "There is no correct activated rule for this sample." << std::endl;
+            } else {
+              std::cout << "There is no correct rule for this sample." << std::endl;
             }
-            break;
-          }
-        }
-        if (currentMinNbCov + 1 < minNbCover) {
-          nbProblems += 1;
-        }
-        if (ruleCreated) {
-          rules.push_back(rule);
-        }
-      }
-
-      std::cout << "\nNumber of sample with lower covering than " << minNbCover << " : " << nbProblems << endl;
-      if (nbRulesNotFound > 0) {
-        std::cout << "Number of rules not found : " << nbRulesNotFound << endl;
-      }
-
-      std::cout << "Fidex rules computed" << endl
-                << endl;
-
-      std::cout << "Computing global ruleset..." << endl
-                << endl;
-
-      // Sort the rules(dataIds) depending of their covering size
-      vector<int> dataIds = notCoveredSamples;
-      std::sort(dataIds.begin(), dataIds.end(), [&rules](int ruleBest, int ruleWorst) {
-        return std::get<1>(rules[ruleWorst]).size() < std::get<1>(rules[ruleBest]).size();
-      });
-
-      nbRules = 0;
-
-      // While there is some not covered samples
-      tuple<vector<tuple<int, bool, double>>, vector<int>, int, double, double> currentRule;
-      auto ancienNotCoveringSize = static_cast<int>(notCoveredSamples.size());
-      int dataId = 0;
-
-      std::vector<int>::iterator ite;
-      while (!notCoveredSamples.empty()) {
-        currentRule = rules[dataIds[dataId]];
-
-        // Delete covered samples
-        ite = std::set_difference(notCoveredSamples.begin(), notCoveredSamples.end(), get<1>(currentRule).begin(), get<1>(currentRule).end(), notCoveredSamples.begin()); // vectors have to be sorted
-        notCoveredSamples.resize(ite - notCoveredSamples.begin());
-
-        // If the rule coveres a new sample
-        if (ancienNotCoveringSize > notCoveredSamples.size()) {
-          nbRules += 1;
-          chosenRules.push_back(currentRule); // add best rule with maximum covering
-        }
-        ancienNotCoveringSize = static_cast<int>(notCoveredSamples.size());
-
-        dataId += 1;
-      }
-
-      std::cout << "Global ruleset Computed" << endl
-                << endl;
-
-      std::cout << "We created " << nbRules << " rules." << endl
-                << endl;
-
-      d2 = clock();
-      temps2 = (float)(d2 - d1) / CLOCKS_PER_SEC;
-      std::cout << "\nTime second heuristic = " << temps2 << " sec\n\n";
-    }
-
-    //--------------------------------------------------------------------------------------------------------------------
-    //--------------------------------------------------------------------------------------------------------------------
-
-    // Third heuristic : Very fast
-    float temps3;
-    clock_t e1;
-    clock_t e2;
-
-    e1 = clock();
 
-    if (heuristic == 3) {
-      std::cout << "Very fast FidexGlo" << endl
-                << endl;
-
-      //  Sort data randomly
-      std::shuffle(std::begin(notCoveredSamples), std::end(notCoveredSamples), gen);
-
-      nbRules = 0;
-      int idSample;
-      bool ruleCreated;
-      int currentMinNbCov;
-      int nbProblems = 0;
-      int nbRulesNotFound = 0;
-      tuple<vector<tuple<int, bool, double>>, vector<int>, int, double, double> rule; // Ex: ([X2<3.5 X3>=4], covering, class)
-      auto exp = FidexAlgo();
-
-      std::cout << "Computing rules..." << endl
-                << endl;
-
-      // While there is some not covered samples
-      while (!notCoveredSamples.empty()) {
-
-        if (int(nbDatas / 100) != 0 && (nbDatas - notCoveredSamples.size()) % int(nbDatas / 100) == 0 && consoleFileInit == false) {
-          cout << "Processing : " << int((double(nbDatas - notCoveredSamples.size()) / nbDatas) * 100) << "%r";
-          std::cout.flush();
-        }
+            std::cout << "We couldn't find any global explanation for this sample." << std::endl; // There is no explanation, we choose the model decision
+            std::cout << "We choose the model prediction." << std::endl;
+            std::cout << "The predicted class is " << std::to_string(testSamplesPreds[currentSample]) << std::endl;
+            lines.emplace_back("We couldn't find any global explanation for this sample."); // There is no explanation, we choose the model decision
+            lines.emplace_back("We choose the model prediction.");
+            lines.emplace_back("The predicted class is " + std::to_string(testSamplesPreds[currentSample]));
+            if (withFidex) {
+              launchingFidex = true;
+              nb_fidex += 1;
+            }
+          }
 
-        idSample = notCoveredSamples[0];
-        currentMinNbCov = minNbCover;
-        ruleCreated = false;
-        int counterFailed = 0; // If we can't find a good rule after a lot of tries
-        while (!ruleCreated) {
-          ruleCreated = exp.fidex(rule, trainData, trainPreds, hasConfidence, trainOutputValuesPredictions, trainTrueClass, &(*trainData)[idSample], (*trainPreds)[idSample], &hyperspace, nbIn, nbAttributs, itMax, currentMinNbCov, dropoutDim, dropoutDimParam, dropoutHyp, dropoutHypParam, gen);
-          if (currentMinNbCov >= 2) {
-            currentMinNbCov -= 1; // If we didnt found a rule with desired covering, we check with a lower covering
+        } else { // There is an explanation which is caracterised by the correct rules
+          if (correctRules.size() > 1) {
+            lines.emplace_back("We have found " + std::to_string(correctRules.size()) + " global rules explaining the model prediction :\n"); // There is no explanation, we choose the model decision
+            std::cout << "We have found " << std::to_string(correctRules.size()) << " global rules explaining the model prediction :" << std::endl
+                      << std::endl; // There is no explanation, we choose the model decision
           } else {
-            counterFailed += 1;
-          }
-          if (counterFailed >= 30) {
-            nbRulesNotFound += 1;
-            break;
-          }
-          if (currentMinNbCov + 1 < minNbCover) {
-            nbProblems += 1;
+            lines.emplace_back("We have found 1 global rule explaining the model prediction :\n"); // There is no explanation, we choose the model decision
+            std::cout << "We have found 1 global rule explaining the model prediction :" << std::endl
+                      << std::endl; // There is no explanation, we choose the model decision
+          }
+          for (int c = 0; c < correctRules.size(); c++) {
+            lines.emplace_back("R" + std::to_string(c + 1) + ": " + rules[correctRules[c]].toString(attributeNames, classNames));
+            std::cout << "R" << std::to_string(c + 1) << ": " << rules[correctRules[c]].toString(attributeNames, classNames) << std::endl;
           }
         }
-
-        if (ruleCreated) {
-          chosenRules.push_back(rule); // We add the new rule
-
-          // Delete covered samples
-          notCoveredSamples.erase(
-              std::remove_if(
-                  notCoveredSamples.begin(), notCoveredSamples.end(), [&rule](int x) {
-                    return std::find(get<1>(rule).begin(), get<1>(rule).end(), x) != get<1>(rule).end();
-                    // find index of coveredSamples which is x (x is element of notCoveredSamples), std::find returns last if x not found
-                    // -> Removes x if it appears on coveredSamples (found before the end of coveredSamples)
-                  }),
-              notCoveredSamples.end());
-
-          nbRules++;
+      }
+      if (minimalVersion) {
+        notShowUncorrectRules = true;
+      }
+      if (!notShowUncorrectRules) {
+        if (!notcorrectRules.empty()) {
+          lines.emplace_back("\nActivated rules without correct decision class :");
+          std::cout << "\nActivated rules without correct decision class :" << std::endl;
+          for (int n = 0; n < notcorrectRules.size(); n++) {
+            lines.emplace_back("F" + std::to_string(n + 1) + ": " + rules[notcorrectRules[n]].toString(attributeNames, classNames));
+            std::cout << "F" << std::to_string(n + 1) + ": " << rules[notcorrectRules[n]].toString(attributeNames, classNames) << std::endl;
+          }
         } else {
-          notCoveredSamples.erase(notCoveredSamples.begin());
+          lines.emplace_back("\nThere is no uncorrect rules.");
+          std::cout << "\nThere is no uncorrect rules." << std::endl;
         }
       }
 
-      std::cout << endl;
-
-      std::cout << "Number of sample with lower covering than " << minNbCover << " : " << nbProblems << endl;
-      if (nbRulesNotFound > 0) {
-        std::cout << "Number of rules not found : " << nbRulesNotFound << endl;
-      }
-
-      std::cout << "We created " << nbRules << " rules." << endl
-                << endl;
-
-      e2 = clock();
-      temps3 = (float)(e2 - e1) / CLOCKS_PER_SEC;
-      std::cout << "\nTime third heuristic = " << temps3 << " sec\n\n";
-    }
-
-    //--------------------------------------------------------------------------------------------------------------------
-    //--------------------------------------------------------------------------------------------------------------------
-
-    std::cout << "Rules extraction..." << endl
-              << endl;
-
-    double meanCovSize = 0;
-    double meanNbAntecedents = 0;
-
-    // Export rules
-    string inequality;
-    string line;
-    vector<string> lines;
-    // Sort the rules(RulesIds) depending of their covering size
-    vector<int> RulesIds(nbRules);                          // Rules indexes
-    std::iota(std::begin(RulesIds), std::end(RulesIds), 0); // Vector from 0 to nbRules-1
-    std::sort(RulesIds.begin(), RulesIds.end(), [&chosenRules](int ruleBest, int ruleWorst) {
-      return std::get<1>(chosenRules[ruleWorst]).size() < std::get<1>(chosenRules[ruleBest]).size();
-    });
-    for (int c = 0; c < nbRules; c++) { // each rule
-      int r = RulesIds[c];
-      meanCovSize += static_cast<double>(get<1>(chosenRules[r]).size());
-      meanNbAntecedents += static_cast<double>(get<0>(chosenRules[r]).size());
-      line = "Rule " + std::to_string(c + 1) + ": ";
-      line += std::to_string(get<0>(chosenRules[r]).size()) + " : "; // If we need to specify the antecedant number
-      for (const auto &rule : get<0>(chosenRules[r])) {              // each antecedant
-        if (get<1>(rule) == 1) {                                     // check inequality
-          inequality = ">=";
-        } else {
-          inequality = "<";
-        }
-        if (attributFileInit) {
-          line += attributeNames[get<0>(rule)];
+      if (launchingFidex) {
+        auto trainDataset = *trainDatas.get();
+        Hyperspace hyperspace(matHypLocus);
+        std::vector<double> mainSampleValues = testSamplesValues[currentSample];
+        int mainSamplePred = testSamplesPreds[currentSample];
+        double mainSamplePredValue = testSamplesOutputValuesPredictions[currentSample][mainSamplePred];
+        int mainSampleClass;
+        if (hasTrueClasses) {
+          mainSampleClass = testSamplesClasses[currentSample];
         } else {
-          line += "X" + std::to_string(get<0>(rule));
+          mainSampleClass = -1;
         }
-        line += inequality + std::to_string(get<2>(rule)) + " ";
+        executeFidex(lines, trainDataset, *params, hyperspace, mainSampleValues, mainSamplePred, mainSamplePredValue, mainSampleClass, attributeNames, classNames);
       }
-      // class of the rule
-      if (hasClassNames) {
-        line += "-> " + classNames[std::get<2>(chosenRules[r])];
-      } else {
-        line += "-> class " + std::to_string(std::get<2>(chosenRules[r]));
-      }
-      line += " Covering size : " + std::to_string(std::get<1>(chosenRules[r]).size()); // Covering size
-      line += " Fidelity : 1";                                                          // Rule fidelity
-      line += " Accuracy : " + std::to_string(std::get<3>(chosenRules[r]));             // Rule accuracy
-      if (hasConfidence) {
-        line += " Confidence : " + std::to_string(std::get<4>(chosenRules[r])) + "\n"; // Rule confidence
+
+      lines.emplace_back("\n--------------------------------------------------------------------\n");
+      std::cout << "\n--------------------------------------------------------------------" << std::endl;
+    }
+
+    if (withFidex) {
+      double fidex_mean;
+      if (nb_fidex == 0) {
+        fidex_mean = 0;
       } else {
-        line += "\n";
+        fidex_mean = (static_cast<double>(nb_fidex) / static_cast<double>(nbSamples)) * 100;
       }
-      lines.push_back(line);
-    }
 
-    meanCovSize /= nbRules;
-    meanNbAntecedents /= nbRules;
+      lines.emplace_back("\nFidex is used for " + std::to_string(fidex_mean) + "% of samples.");
+      std::cout << "\nFidex is used for " + std::to_string(fidex_mean) + "% of samples." << std::endl;
+    }
 
-    ofstream file2(rulesFile);
-    if (file2.is_open()) {
-      // We add to the file the number of rules, the mean covering per rule and the mean number of antecedents per rule
-      string startLine = "Number of rules : " + std::to_string(nbRules) + ", mean sample covering number per rule : " + std::to_string(meanCovSize) + ", mean number of antecedents per rule : " + std::to_string(meanNbAntecedents) + "\n";
-      file2 << startLine;
-      string secondLine = "The name of the attributes and classes are not specified\n";
-      if (attributFileInit) {
-        secondLine = "The name of the attributes is specified\n";
-        if (hasClassNames) {
-          secondLine = "The name of the attributes and classes are specified\n";
+    // Output global explanation result
+    if (params->isStringSet(EXPLANATION_FILE)) {
+      std::ofstream outputFile(params->getString(EXPLANATION_FILE));
+      if (outputFile.is_open()) {
+        for (const auto &line : lines) {
+          outputFile << line << "" << std::endl;
         }
+        outputFile.close();
+      } else {
+        throw CannotOpenFileError("Error : Couldn't open explanation extraction file " + params->getString(EXPLANATION_FILE) + ".");
       }
-      file2 << secondLine;
-      for (const auto &l : lines) {
-        file2 << l;
-      }
-
-      file2.close();
-
-    } else {
-      throw CannotOpenFileError("Error : Couldn't open rules extraction file " + std::string(rulesFile) + ".");
     }
 
-    std::cout << "Mean covering size per rule : " << meanCovSize << endl;
-    std::cout << "Mean number of antecedents per rule : " << meanNbAntecedents << endl;
-
     t2 = clock();
     temps = (float)(t2 - t1) / CLOCKS_PER_SEC;
-    std::cout << "\nFull execution time = " << temps << " sec\n";
+    std::cout << "\nFull execution time = " << temps << " sec" << std::endl;
 
     std::cout.rdbuf(cout_buff); // reset to standard output again
 
-  } catch (const char *msg) {
-    cerr << msg << endl;
+  } catch (const ErrorHandler &e) {
+    std::cout.rdbuf(cout_buff); // reset to standard output again
+    std::cerr << e.what() << std::endl;
+    return -1;
   }
 
   return 0;
 }
 
-/* Exemples pour lancer le code :
-
-./fidexGloRules -T datanormTrain -P dimlpDatanormTrain.out -C dataclass2Train -W dimlpDatanorm.wts -Q 50 -I 5 -O globalRulesDatanorm.txt -M 1 -i 100 -v 2 -d 0.5 -h 0.5 -r rulesResult -S ../fidexGlo/datafiles
-
-./fidexGloRules -T covidTrainData.txt -P covidTrainPred.out -C covidTrainClass.txt -W covid.wts -Q 50 -I 5 -O globalRulesCovid.txt -M 1 -i 100 -v 2 -d 0.5 -h 0.5 -r rulesCovidResult -S ../dimlp/datafiles/covidDataset
-./fidexGloRules -T spamTrainData.txt -P spamTrainPred.out -C spamTrainClass.txt -W spam.wts -Q 50 -I 5 -O globalRulesSpam.txt -M 1 -i 100 -v 2 -d 0.5 -h 0.5 -r rulesSpamResult -S ../dimlp/datafiles/spamDataset
-./fidexGloRules -T isoletTrainData.txt -P isoletTrainPredV2.out -C isoletTrainClass.txt -W isoletV2.wts -Q 50 -I 5 -O globalRulesIsoletV2.txt -M 1 -i 100 -v 2 -d 0.5 -h 0.5 -r rulesIsoletResultV2 -S ../dimlp/datafiles/isoletDataset
-./fidexGloRules -T Train/X_train.txt -P Train/pred_trainV2.out -C Train/y_train.txt -W HAPTV2.wts -Q 50 -I 5 -O globalRulesHAPTV2.txt -M 1 -i 100 -v 2 -d 0.5 -h 0.5 -r rulesHAPTResultV2 -S ../dimlp/datafiles/HAPTDataset
-
-*/
+// Exemple pour lancer le code : ./fidexGlo --test_data_file datanormTest --test_pred_file dimlpDatanormTest.out --global_rules_file globalRulesDatanorm.txt --nb_attributes 16 --nb_classes 2 --explanation_file explanation.txt --root_folder ../fidex/datafiles --with_fidex true --train_data_file datanormTrain --train_pred_file dimlpDatanormTrain.out --train_class_file dataclass2Train --test_class_file dataclass2Test --weights_file dimlpDatanorm.wts
```

### Comparing `dimlpfidex-0.0.0/fidexGlo/cpp/src/hyperspace.h` & `dimlpfidex-0.0.1/fidex/cpp/src/hyperspace.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 #ifndef HYPERSPACEGLO_H
 #define HYPERSPACEGLO_H
 
-#include "../../../fidexCommon/cpp/src/errorHandler.h"
-#include "../../../fidexCommon/cpp/src/hyperbox.h"
+#include "../../../common/cpp/src/errorHandler.h"
+#include "../../../common/cpp/src/rule.h"
+#include "hyperbox.h"
 #include <cstring>
 #include <fstream>
 #include <iostream>
 #include <memory>
 #include <sstream>
 #include <tuple>
 #include <vector>
 
-namespace FidexGloNameSpace {
 class Hyperspace {
-
   std::vector<std::vector<double>> hyperLocus; // All the possible hyperplans
   std::shared_ptr<Hyperbox> hyperbox;
 
 public:
   Hyperspace();
   explicit Hyperspace(const std::vector<std::vector<double>> &matHypLocus);
 
   std::shared_ptr<Hyperbox> getHyperbox() const;
   std::vector<std::vector<double>> getHyperLocus() const;
-  std::tuple<std::vector<std::tuple<int, bool, double>>, std::vector<int>, int, double, double> ruleExtraction(std::vector<double> *mainSampleData, const int mainSamplePred, double ruleAccuracy, double ruleConfidence);
-  double computeRuleAccuracy(std::vector<int> *trainPreds, std::vector<int> *trainTrueClass) const;
-  double computeRuleConfidence(std::vector<std::vector<double>> *trainOutputValuesPredictions, const int mainSamplePred) const;
+  Rule ruleExtraction(std::vector<double> &mainSampleData, const int mainSamplePred, double ruleAccuracy, double ruleConfidence, const std::vector<double> &mus = std::vector<double>(), const std::vector<double> &sigmas = std::vector<double>(), const std::vector<int> &normalizationIndices = std::vector<int>());
+  double computeRuleAccuracy(std::vector<int> &trainPreds, std::vector<int> &trainTrueClass, bool hasTrueClasses, bool mainSampleCorrect = false) const;
+  double computeRuleConfidence(std::vector<std::vector<double>> &trainOutputValuesPredictions, const int mainSamplePred, double mainSamplePredValue = -1.0) const;
 };
-} // namespace FidexGloNameSpace
 
 #endif
```

### Comparing `dimlpfidex-0.0.0/fidexGlo/pybind/bindings.cpp` & `dimlpfidex-0.0.1/fidex/pybind/bindings.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+#include "../cpp/src/fidexFct.h"
 #include "../cpp/src/fidexGloFct.h"
 #include "../cpp/src/fidexGloRulesFct.h"
 #include "../cpp/src/fidexGloStatsFct.h"
 #include <pybind11/pybind11.h>
 
 namespace py = pybind11;
 
-PYBIND11_MODULE(fidexGlo, m) {
-  m.doc() = "pybind11 fidexGlo plugin"; // optional module docstring
-  m.def("fidexGlo", &fidexGlo, "A function to get explanation rule for one or many particular samples using pretrained rules.");
-  m.def("fidexGloRules", &fidexGloRules, "A function to get rules from a train dataSet.");
-  m.def("fidexGloStats", &fidexGloStats, "A function to get statistics from pretrained rules.");
+PYBIND11_MODULE(fidex, m) {
+  m.doc() = "pybind11 fidex plugin"; // optional module docstring
+  m.def("fidex", &fidex, pybind11::arg("command") = "", "A function to get explanation rule for one or many particular samples.");
+  m.def("fidexGlo", &fidexGlo, pybind11::arg("command") = "", "A function to get explanation rule for one or many particular samples using pretrained rules.");
+  m.def("fidexGloRules", &fidexGloRules, pybind11::arg("command") = "", "A function to get rules from a train dataSet.");
+  m.def("fidexGloStats", &fidexGloStats, pybind11::arg("command") = "", "A function to get statistics from pretrained rules.");
 }
```

### Comparing `dimlpfidex-0.0.0/PKG-INFO` & `dimlpfidex-0.0.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 Metadata-Version: 2.1
 Name: dimlpfidex
-Version: 0.0.0
+Version: 0.0.1
 Summary: Discretized Interpretable Multi Layer Perceptron (DIMLP) and related algorithms
-Home-page: https://hes-xplain.github.io/
-License: BSD-3-Clause
-Keywords: machine learning,xai
-Author: Jean-Marc Boutay
-Author-email: jean-marc.boutay@hesge.ch
-Requires-Python: >=3.9,<3.11
+Keywords: machine learning xai
+Author-Email: Jean-Marc Boutay <jean-marc.boutay@hesge.ch>, Guido Bologna <guido.bologna@hesge.ch>
+License: BSD License (BSD-3-Clause)
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: C++
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: numpy (>=1.22,<=1.24.3)
-Requires-Dist: pybind11 (>=2.10.4,<3.0.0)
-Requires-Dist: pybind11-global (>=2.10.4,<3.0.0)
-Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
-Requires-Dist: tensorflow (>=2.13.0,<3.0.0)
-Requires-Dist: tensorflow-io-gcs-filesystem (==0.31.0)
-Project-URL: Repository, https://github.com/HES-XPLAIN/dimlpfidex
+Classifier: Programming Language :: C++
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8.1
+Requires-Dist: pybind11>=2.10.4
+Requires-Dist: pybind11-global>=2.10.4
+Requires-Dist: numpy>=1.22
+Requires-Dist: scikit-learn>=1.2.2
+Requires-Dist: tensorflow>=2.13
+Requires-Dist: tensorflow-io-gcs-filesystem>=0.31.0
+Requires-Dist: matplotlib>=3.7.4
+Requires-Dist: build>=1.0.3
 Description-Content-Type: text/markdown
 
-# dimlpfidex
+# dimlpfidex ![build](https://github.com/HES-XPLAIN/dimlpfidex/actions/workflows/build.yml/badge.svg)
 Discretized Interpretable Multi Layer Perceptron (DIMLP) and related algorithms
 
 ## Contribution
 
+### Get the project code
+
+To get the latest source code, install [git](https://git-scm.com/) and [clone](https://docs.github.com/en/get-started/getting-started-with-git/about-remote-repositories) the repository:
+
+```sh
+$ git clone https://github.com/HES-XPLAIN/dimlpfidex.git
+```
+
+To download the required dependencies on your system, run:
+
+```sh
+$ git submodule init
+$ git submodule update
+```
+
 ### Install C++ toolchain
 
 #### Linux, macOS, Windows/WSL
 
 Install with your package manager:
 
 * a C++ compiler (gcc/g++)
@@ -60,82 +72,100 @@
 
 Ensure `cmake.exe` is accessible in the `$PATH` environment variable.
 
 ```shell
 cmake.exe --version
 ```
 
-### Install Python and Poetry
+### Install Python
 
-#### Linux, macOS, Windows/WSL
+Install [Python](https://www.python.org/):
 
-Use your package manager to install:
+#### Manually
 
-* python
-* poetry
+* **Linux, macOS, Windows/WSL**: Use your package manager to install `python3` and `python3-dev`
+* **Windows**: `winget install Python.Python.3.11`
 
-#### Windows
+> [!IMPORTANT]
+> On Windows, avoid installing Python through the Microsoft Store as the package has additional permission restrictions.
 
-* Install [Python](https://www.python.org/)
+#### Using Rye
 
-```shell
-winget install Python.Python.3.10
-```
+- Install [Rye](https://rye-up.com/) and [add shims](https://rye-up.com/guide/installation/) to your PATH.
 
-* Install [poetry](https://python-poetry.org/docs/#installation) and add it to your PATH.
+Ensure `rye` is accessible in the `$PATH` environment variable.
+Rye will automatically download the suitable Python toolchain as needed.
 
-Ensure `python.exe` and `poetry.exe` are accessible in the `$PATH` environment variable.
-
-To check the installation, check these commands return an output:
+To check the installation, check the following commands return an output:
 
 ```shell
-python.exe --version
-poetry.exe --version
+rye --version
 ```
 
-### Compile
+### Install Python dependencies
 
-Activate the virtual environment:
+#### Using pip
 
 ```shell
-poetry shell
+python -m venv .venv
+source .venv/bin/activate
+pip install .
 ```
 
-Install python dependencies and compile:
+> [!NOTE]
+> On Windows, use `.venv\Scripts\activate` instead.
+
+#### Using Rye
+
+Install python dependencies and create a virtualenv in `.venv`:
 
 ```shell
-poetry install
-poetry build
+rye sync
 ```
 
-If CMake complains about not finding pybind11, ensure to activate the shell first.
+#### Add dependencies
+
+To add new dependencies to the project, either add them to the `pyproject.toml` file or use `rye add <dependency>`.
+To add them to the virtualenv, use `pip install .` or `rye sync`.
+
+### Work with virtualenv
+
+To activate the virtualenv, use the standard methods:
+
+* Unix: `source .venv/bin/activate`
+* Windows: `.venv\Scripts\activate`
 
-**Note**: If you still have an issue on Windows, try the following commands to
-build manually:
+To leave the virtualenv, use `deactivate`.
+
+### Compile and Package
+
+Compile and create archives for distribution:
 
 ```shell
-mkdir build && cd build
-$path = (poetry env info | Select-String -Pattern 'Path:\s+(.*)').Matches.Groups[1].Value
-cmake.exe -G "MinGW Makefiles" -DCMAKE_PREFIX_PATH="$path" ..
-cmake.exe --build .
+python -m build
 ```
 
 ### Install Pre-commit hooks
 
 Git hooks are used to ensure quality checks are run by all developers every time
 before a commit.
 
+Install with `pip install pre-commit` or`rye sync`.
+
+To enable pre-commit:
+
 ```shell
-poetry shell
 pre-commit install
 ```
 
 Pre-commit hooks can be run manually with:
 
 ```shell
 pre-commit run --all-files
 ```
 
 ## Release
 
 To publish the package on [PyPI](https://pypi.org/project/dimlpfidex/), refer to [RELEASE](RELEASE.md).
 
+## Credits
+Our test suite is using [Obesity or CVD risk dataset](https://www.kaggle.com/datasets/aravindpcoder/obesity-or-cvd-risk-classifyregressorcluster) from [AravindPCoder](https://www.kaggle.com/aravindpcoder) (under CC BY-SA 4.0 license)
```

