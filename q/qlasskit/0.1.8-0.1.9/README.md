# Comparing `tmp/qlasskit-0.1.8.tar.gz` & `tmp/qlasskit-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qlasskit-0.1.8.tar", last modified: Mon Dec  4 07:05:10 2023, max compression
+gzip compressed data, was "qlasskit-0.1.9.tar", last modified: Wed Dec 13 16:39:34 2023, max compression
```

## Comparing `qlasskit-0.1.8.tar` & `qlasskit-0.1.9.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2023-12-04 07:05:10.336302 qlasskit-0.1.8/
--rw-r--r--   0 dakk      (1000) dakk      (1000)    10255 2023-09-26 10:07:38.000000 qlasskit-0.1.8/LICENSE
--rw-r--r--   0 dakk      (1000) dakk      (1000)     3874 2023-12-04 07:05:10.336302 qlasskit-0.1.8/PKG-INFO
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2911 2023-11-28 11:56:47.000000 qlasskit-0.1.8/README.md
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2023-12-04 07:05:10.232965 qlasskit-0.1.8/qlasskit/
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1063 2023-12-03 17:19:49.000000 qlasskit-0.1.8/qlasskit/__init__.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2023-12-04 07:05:10.242966 qlasskit-0.1.8/qlasskit/algorithms/
--rw-r--r--   0 dakk      (1000) dakk      (1000)      846 2023-11-27 12:39:22.000000 qlasskit-0.1.8/qlasskit/algorithms/__init__.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2261 2023-11-27 12:41:06.000000 qlasskit-0.1.8/qlasskit/algorithms/deutschjozsa.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     4069 2023-11-27 11:23:46.000000 qlasskit-0.1.8/qlasskit/algorithms/grover.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1685 2023-11-27 09:00:31.000000 qlasskit-0.1.8/qlasskit/algorithms/qalgorithm.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1958 2023-11-27 12:22:59.000000 qlasskit-0.1.8/qlasskit/algorithms/simon.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)    16091 2023-11-27 08:26:38.000000 qlasskit-0.1.8/qlasskit/ast2ast.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2023-12-04 07:05:10.266300 qlasskit-0.1.8/qlasskit/ast2logic/
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1095 2023-10-27 06:09:02.000000 qlasskit-0.1.8/qlasskit/ast2logic/__init__.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     3782 2023-10-30 09:26:36.000000 qlasskit-0.1.8/qlasskit/ast2logic/env.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1867 2023-10-27 07:09:22.000000 qlasskit-0.1.8/qlasskit/ast2logic/exceptions.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2837 2023-11-27 08:29:15.000000 qlasskit-0.1.8/qlasskit/ast2logic/t_arguments.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1743 2023-12-03 17:08:08.000000 qlasskit-0.1.8/qlasskit/ast2logic/t_ast.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)    13118 2023-12-03 12:29:19.000000 qlasskit-0.1.8/qlasskit/ast2logic/t_expression.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     3570 2023-11-27 08:12:21.000000 qlasskit-0.1.8/qlasskit/ast2logic/t_statement.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1253 2023-11-15 14:03:40.000000 qlasskit-0.1.8/qlasskit/ast2logic/typing.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)      963 2023-10-23 07:20:26.000000 qlasskit-0.1.8/qlasskit/ast2logic/utils.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2023-12-04 07:05:10.269633 qlasskit-0.1.8/qlasskit/boolopt/
--rw-r--r--   0 dakk      (1000) dakk      (1000)      734 2023-12-03 17:08:08.000000 qlasskit-0.1.8/qlasskit/boolopt/__init__.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2683 2023-12-03 17:08:08.000000 qlasskit-0.1.8/qlasskit/boolopt/bool_optimizer.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2074 2023-11-15 10:20:57.000000 qlasskit-0.1.8/qlasskit/boolopt/exp_transformers.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1052 2023-11-09 09:18:36.000000 qlasskit-0.1.8/qlasskit/boolopt/sympytransformer.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1198 2023-11-16 07:43:18.000000 qlasskit-0.1.8/qlasskit/boolquant.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2023-12-04 07:05:10.276300 qlasskit-0.1.8/qlasskit/compiler/
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1742 2023-11-15 13:53:06.000000 qlasskit-0.1.8/qlasskit/compiler/__init__.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1003 2023-11-15 13:16:12.000000 qlasskit-0.1.8/qlasskit/compiler/compiler.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1312 2023-10-25 10:03:44.000000 qlasskit-0.1.8/qlasskit/compiler/expqmap.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     4893 2023-12-03 17:04:27.000000 qlasskit-0.1.8/qlasskit/compiler/internalcompiler.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     4318 2023-11-15 13:28:35.000000 qlasskit-0.1.8/qlasskit/compiler/tweedledumcompiler.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2023-12-04 07:05:10.292967 qlasskit-0.1.8/qlasskit/qcircuit/
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1070 2023-11-16 08:02:56.000000 qlasskit-0.1.8/qlasskit/qcircuit/__init__.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2168 2023-11-16 08:49:08.000000 qlasskit-0.1.8/qlasskit/qcircuit/cnotsim.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)      767 2023-10-27 09:53:02.000000 qlasskit-0.1.8/qlasskit/qcircuit/exporter.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     3250 2023-11-15 13:50:57.000000 qlasskit-0.1.8/qlasskit/qcircuit/exporter_cirq.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1311 2023-10-27 09:52:45.000000 qlasskit-0.1.8/qlasskit/qcircuit/exporter_qasm.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2086 2023-11-30 11:21:12.000000 qlasskit-0.1.8/qlasskit/qcircuit/exporter_qiskit.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2038 2023-10-26 14:34:03.000000 qlasskit-0.1.8/qlasskit/qcircuit/exporter_sympy.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2344 2023-11-30 11:21:12.000000 qlasskit-0.1.8/qlasskit/qcircuit/gates.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     8226 2023-12-03 17:08:08.000000 qlasskit-0.1.8/qlasskit/qcircuit/qcircuit.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     4534 2023-10-27 14:07:18.000000 qlasskit-0.1.8/qlasskit/qcircuit/qcircuitenhanced.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2924 2023-11-27 12:10:44.000000 qlasskit-0.1.8/qlasskit/qcircuit/qcircuitwrapper.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     9476 2023-12-03 17:08:08.000000 qlasskit-0.1.8/qlasskit/qlassfun.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2023-12-04 07:05:10.296301 qlasskit-0.1.8/qlasskit/types/
--rw-r--r--   0 dakk      (1000) dakk      (1000)     3969 2023-11-27 12:10:44.000000 qlasskit-0.1.8/qlasskit/types/__init__.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)      847 2023-10-18 14:41:59.000000 qlasskit-0.1.8/qlasskit/types/qbool.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     8097 2023-12-03 16:46:58.000000 qlasskit-0.1.8/qlasskit/types/qint.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)      988 2023-11-01 14:35:20.000000 qlasskit-0.1.8/qlasskit/types/qlist.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1140 2023-11-26 17:32:02.000000 qlasskit-0.1.8/qlasskit/types/qmatrix.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     4312 2023-12-03 12:28:38.000000 qlasskit-0.1.8/qlasskit/types/qtype.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2023-12-04 07:05:10.242966 qlasskit-0.1.8/qlasskit.egg-info/
--rw-r--r--   0 dakk      (1000) dakk      (1000)     3874 2023-12-04 07:05:09.000000 qlasskit-0.1.8/qlasskit.egg-info/PKG-INFO
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2145 2023-12-04 07:05:09.000000 qlasskit-0.1.8/qlasskit.egg-info/SOURCES.txt
--rw-r--r--   0 dakk      (1000) dakk      (1000)        1 2023-12-04 07:05:09.000000 qlasskit-0.1.8/qlasskit.egg-info/dependency_links.txt
--rw-r--r--   0 dakk      (1000) dakk      (1000)        1 2023-09-26 08:32:13.000000 qlasskit-0.1.8/qlasskit.egg-info/not-zip-safe
--rw-r--r--   0 dakk      (1000) dakk      (1000)       44 2023-12-04 07:05:09.000000 qlasskit-0.1.8/qlasskit.egg-info/requires.txt
--rw-r--r--   0 dakk      (1000) dakk      (1000)        9 2023-12-04 07:05:09.000000 qlasskit-0.1.8/qlasskit.egg-info/top_level.txt
--rw-r--r--   0 dakk      (1000) dakk      (1000)      382 2023-12-04 07:05:10.336302 qlasskit-0.1.8/setup.cfg
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1502 2023-11-28 08:17:59.000000 qlasskit-0.1.8/setup.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2023-12-04 07:05:10.336302 qlasskit-0.1.8/test/
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2852 2023-11-09 17:00:19.000000 qlasskit-0.1.8/test/test_algo.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2213 2023-12-03 17:08:08.000000 qlasskit-0.1.8/test/test_algo_deutschjozsa.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     3208 2023-11-24 11:29:39.000000 qlasskit-0.1.8/test/test_algo_grover.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1459 2023-12-03 17:19:59.000000 qlasskit-0.1.8/test/test_algo_simon.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     4463 2023-11-01 11:10:12.000000 qlasskit-0.1.8/test/test_ast2logic_t_arg.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)      971 2023-10-06 06:44:47.000000 qlasskit-0.1.8/test/test_ast2logic_t_exp.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)      965 2023-10-19 14:21:44.000000 qlasskit-0.1.8/test/test_ast2logic_t_stmt.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)      770 2023-11-09 09:18:36.000000 qlasskit-0.1.8/test/test_bool_optimizer.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2131 2023-10-30 08:37:27.000000 qlasskit-0.1.8/test/test_compiler.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     6818 2023-11-14 07:58:46.000000 qlasskit-0.1.8/test/test_qcircuit.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     6627 2023-11-24 11:31:20.000000 qlasskit-0.1.8/test/test_qlassf.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     8559 2023-11-09 09:48:50.000000 qlasskit-0.1.8/test/test_qlassf_bool.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     6531 2023-11-08 16:39:21.000000 qlasskit-0.1.8/test/test_qlassf_builtin.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     3397 2023-11-01 16:22:24.000000 qlasskit-0.1.8/test/test_qlassf_for_loop.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     3490 2023-10-30 08:37:27.000000 qlasskit-0.1.8/test/test_qlassf_functiondef.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1772 2023-11-23 10:26:52.000000 qlasskit-0.1.8/test/test_qlassf_hybrid_quantum.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2762 2023-11-09 09:18:36.000000 qlasskit-0.1.8/test/test_qlassf_ifthenelse.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)    18415 2023-12-03 16:51:06.000000 qlasskit-0.1.8/test/test_qlassf_int.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     4603 2023-11-16 16:22:10.000000 qlasskit-0.1.8/test/test_qlassf_list.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     4574 2023-11-27 08:23:15.000000 qlasskit-0.1.8/test/test_qlassf_matrix.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     8013 2023-11-09 09:18:36.000000 qlasskit-0.1.8/test/test_qlassf_tuple.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2558 2023-11-09 17:00:19.000000 qlasskit-0.1.8/test/test_types.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2023-12-13 16:39:34.461268 qlasskit-0.1.9/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)    10255 2023-09-26 10:07:38.000000 qlasskit-0.1.9/LICENSE
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     3874 2023-12-13 16:39:34.461268 qlasskit-0.1.9/PKG-INFO
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2911 2023-11-28 11:56:47.000000 qlasskit-0.1.9/README.md
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2023-12-13 16:39:34.444601 qlasskit-0.1.9/qlasskit/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1063 2023-12-13 16:38:51.000000 qlasskit-0.1.9/qlasskit/__init__.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2023-12-13 16:39:34.447934 qlasskit-0.1.9/qlasskit/algorithms/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      846 2023-11-27 12:39:22.000000 qlasskit-0.1.9/qlasskit/algorithms/__init__.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2287 2023-12-07 08:07:08.000000 qlasskit-0.1.9/qlasskit/algorithms/deutschjozsa.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     4100 2023-12-07 08:07:18.000000 qlasskit-0.1.9/qlasskit/algorithms/grover.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1685 2023-11-27 09:00:31.000000 qlasskit-0.1.9/qlasskit/algorithms/qalgorithm.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1982 2023-12-07 08:07:29.000000 qlasskit-0.1.9/qlasskit/algorithms/simon.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)    16091 2023-11-27 08:26:38.000000 qlasskit-0.1.9/qlasskit/ast2ast.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2023-12-13 16:39:34.447934 qlasskit-0.1.9/qlasskit/ast2logic/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1095 2023-10-27 06:09:02.000000 qlasskit-0.1.9/qlasskit/ast2logic/__init__.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     3782 2023-10-30 09:26:36.000000 qlasskit-0.1.9/qlasskit/ast2logic/env.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1867 2023-10-27 07:09:22.000000 qlasskit-0.1.9/qlasskit/ast2logic/exceptions.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2837 2023-11-27 08:29:15.000000 qlasskit-0.1.9/qlasskit/ast2logic/t_arguments.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1743 2023-12-13 16:39:00.000000 qlasskit-0.1.9/qlasskit/ast2logic/t_ast.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)    13118 2023-12-03 12:29:19.000000 qlasskit-0.1.9/qlasskit/ast2logic/t_expression.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     3570 2023-11-27 08:12:21.000000 qlasskit-0.1.9/qlasskit/ast2logic/t_statement.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1253 2023-11-15 14:03:40.000000 qlasskit-0.1.9/qlasskit/ast2logic/typing.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      963 2023-10-23 07:20:26.000000 qlasskit-0.1.9/qlasskit/ast2logic/utils.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2023-12-13 16:39:34.447934 qlasskit-0.1.9/qlasskit/boolopt/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      762 2023-12-06 14:00:46.000000 qlasskit-0.1.9/qlasskit/boolopt/__init__.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2833 2023-12-13 16:39:00.000000 qlasskit-0.1.9/qlasskit/boolopt/bool_optimizer.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2074 2023-11-15 10:20:57.000000 qlasskit-0.1.9/qlasskit/boolopt/exp_transformers.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1052 2023-11-09 09:18:36.000000 qlasskit-0.1.9/qlasskit/boolopt/sympytransformer.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1198 2023-12-13 16:38:31.000000 qlasskit-0.1.9/qlasskit/boolquant.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2023-12-13 16:39:34.451268 qlasskit-0.1.9/qlasskit/compiler/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1742 2023-11-15 13:53:06.000000 qlasskit-0.1.9/qlasskit/compiler/__init__.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1003 2023-11-15 13:16:12.000000 qlasskit-0.1.9/qlasskit/compiler/compiler.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1312 2023-10-25 10:03:44.000000 qlasskit-0.1.9/qlasskit/compiler/expqmap.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     4954 2023-12-13 16:18:30.000000 qlasskit-0.1.9/qlasskit/compiler/internalcompiler.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     4318 2023-11-15 13:28:35.000000 qlasskit-0.1.9/qlasskit/compiler/tweedledumcompiler.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2023-12-13 16:39:34.454601 qlasskit-0.1.9/qlasskit/qcircuit/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1070 2023-11-16 08:02:56.000000 qlasskit-0.1.9/qlasskit/qcircuit/__init__.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2168 2023-11-16 08:49:08.000000 qlasskit-0.1.9/qlasskit/qcircuit/cnotsim.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      767 2023-10-27 09:53:02.000000 qlasskit-0.1.9/qlasskit/qcircuit/exporter.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     3250 2023-12-13 16:36:42.000000 qlasskit-0.1.9/qlasskit/qcircuit/exporter_cirq.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1311 2023-10-27 09:52:45.000000 qlasskit-0.1.9/qlasskit/qcircuit/exporter_qasm.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2086 2023-11-30 11:21:12.000000 qlasskit-0.1.9/qlasskit/qcircuit/exporter_qiskit.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2038 2023-10-26 14:34:03.000000 qlasskit-0.1.9/qlasskit/qcircuit/exporter_sympy.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2344 2023-12-13 16:36:34.000000 qlasskit-0.1.9/qlasskit/qcircuit/gates.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     8426 2023-12-13 16:39:00.000000 qlasskit-0.1.9/qlasskit/qcircuit/qcircuit.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     4534 2023-10-27 14:07:18.000000 qlasskit-0.1.9/qlasskit/qcircuit/qcircuitenhanced.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2924 2023-11-27 12:10:44.000000 qlasskit-0.1.9/qlasskit/qcircuit/qcircuitwrapper.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     9452 2023-12-05 17:14:45.000000 qlasskit-0.1.9/qlasskit/qlassfun.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2023-12-13 16:39:34.454601 qlasskit-0.1.9/qlasskit/types/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     3969 2023-11-27 12:10:44.000000 qlasskit-0.1.9/qlasskit/types/__init__.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      847 2023-10-18 14:41:59.000000 qlasskit-0.1.9/qlasskit/types/qbool.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     8187 2023-12-06 14:01:57.000000 qlasskit-0.1.9/qlasskit/types/qint.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      988 2023-11-01 14:35:20.000000 qlasskit-0.1.9/qlasskit/types/qlist.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1140 2023-11-26 17:32:02.000000 qlasskit-0.1.9/qlasskit/types/qmatrix.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     4312 2023-12-03 12:28:38.000000 qlasskit-0.1.9/qlasskit/types/qtype.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2023-12-13 16:39:34.444601 qlasskit-0.1.9/qlasskit.egg-info/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     3874 2023-12-13 16:39:34.000000 qlasskit-0.1.9/qlasskit.egg-info/PKG-INFO
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2145 2023-12-13 16:39:34.000000 qlasskit-0.1.9/qlasskit.egg-info/SOURCES.txt
+-rw-r--r--   0 dakk      (1000) dakk      (1000)        1 2023-12-13 16:39:34.000000 qlasskit-0.1.9/qlasskit.egg-info/dependency_links.txt
+-rw-r--r--   0 dakk      (1000) dakk      (1000)        1 2023-09-26 08:32:13.000000 qlasskit-0.1.9/qlasskit.egg-info/not-zip-safe
+-rw-r--r--   0 dakk      (1000) dakk      (1000)       44 2023-12-13 16:39:34.000000 qlasskit-0.1.9/qlasskit.egg-info/requires.txt
+-rw-r--r--   0 dakk      (1000) dakk      (1000)        9 2023-12-13 16:39:34.000000 qlasskit-0.1.9/qlasskit.egg-info/top_level.txt
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      382 2023-12-13 16:39:34.461268 qlasskit-0.1.9/setup.cfg
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1502 2023-11-28 08:17:59.000000 qlasskit-0.1.9/setup.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2023-12-13 16:39:34.461268 qlasskit-0.1.9/test/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2852 2023-11-09 17:00:19.000000 qlasskit-0.1.9/test/test_algo.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2213 2023-12-03 17:08:08.000000 qlasskit-0.1.9/test/test_algo_deutschjozsa.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     3208 2023-11-24 11:29:39.000000 qlasskit-0.1.9/test/test_algo_grover.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1459 2023-12-13 16:19:18.000000 qlasskit-0.1.9/test/test_algo_simon.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     4463 2023-11-01 11:10:12.000000 qlasskit-0.1.9/test/test_ast2logic_t_arg.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      971 2023-10-06 06:44:47.000000 qlasskit-0.1.9/test/test_ast2logic_t_exp.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      965 2023-10-19 14:21:44.000000 qlasskit-0.1.9/test/test_ast2logic_t_stmt.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      770 2023-11-09 09:18:36.000000 qlasskit-0.1.9/test/test_bool_optimizer.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2131 2023-10-30 08:37:27.000000 qlasskit-0.1.9/test/test_compiler.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     6818 2023-11-14 07:58:46.000000 qlasskit-0.1.9/test/test_qcircuit.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     6619 2023-12-05 17:14:45.000000 qlasskit-0.1.9/test/test_qlassf.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     8559 2023-11-09 09:48:50.000000 qlasskit-0.1.9/test/test_qlassf_bool.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     6531 2023-11-08 16:39:21.000000 qlasskit-0.1.9/test/test_qlassf_builtin.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     3397 2023-11-01 16:22:24.000000 qlasskit-0.1.9/test/test_qlassf_for_loop.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     3490 2023-10-30 08:37:27.000000 qlasskit-0.1.9/test/test_qlassf_functiondef.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2104 2023-12-13 16:38:24.000000 qlasskit-0.1.9/test/test_qlassf_hybrid_quantum.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2762 2023-11-09 09:18:36.000000 qlasskit-0.1.9/test/test_qlassf_ifthenelse.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)    18415 2023-12-03 16:51:06.000000 qlasskit-0.1.9/test/test_qlassf_int.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     4603 2023-11-16 16:22:10.000000 qlasskit-0.1.9/test/test_qlassf_list.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     4574 2023-11-27 08:23:15.000000 qlasskit-0.1.9/test/test_qlassf_matrix.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     8013 2023-11-09 09:18:36.000000 qlasskit-0.1.9/test/test_qlassf_tuple.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2558 2023-11-09 17:00:19.000000 qlasskit-0.1.9/test/test_types.py
```

### Comparing `qlasskit-0.1.8/LICENSE` & `qlasskit-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/PKG-INFO` & `qlasskit-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qlasskit
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python-to-quantum compiler
 Home-page: https://github.com/dakk/qlasskit
 Author: Davide Gessa
 Author-email: gessadavide@gmail.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/dakk/qlasskit/issues/
 Project-URL: Documentation, https://dakk.github.io/qlasskit
```

### Comparing `qlasskit-0.1.8/README.md` & `qlasskit-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/__init__.py` & `qlasskit-0.1.9/qlasskit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # isort:skip_file
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 from .qcircuit import QCircuit, SupportedFrameworks, SupportedFramework  # noqa: F401
 from .qlassfun import QlassF, qlassf, qlassfa  # noqa: F401
 from .ast2ast import ast2ast  # noqa: F401
 from .ast2logic import exceptions  # noqa: F401
 from .types import (  # noqa: F401, F403
     const_to_qtype,
```

### Comparing `qlasskit-0.1.8/qlasskit/algorithms/__init__.py` & `qlasskit-0.1.9/qlasskit/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/algorithms/deutschjozsa.py` & `qlasskit-0.1.9/qlasskit/algorithms/deutschjozsa.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         if len(f.args) != 1:
             raise Exception("f should receive exactly one parameter")
         if f.returns.ttype != bool:
             raise Exception("f should returns bool")
 
         self.f: QlassF = f
         self.search_space_size = len(f.args[0])
-        self._qcircuit = QCircuit(self.f.num_qubits)
+        self._qcircuit = QCircuit(self.f.num_qubits, name=f"deutsch_{f.name}")
 
         self._f_circuit = self.f.circuit()
 
         # State preparation
         self._qcircuit.barrier(label="s")
         for i in range(self.search_space_size):
             self._qcircuit.h(i)
```

### Comparing `qlasskit-0.1.8/qlasskit/algorithms/grover.py` & `qlasskit-0.1.9/qlasskit/algorithms/grover.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         if n_iterations is None:
             n_iterations = math.ceil(
                 math.pi / 4.0 * math.sqrt(2**self.search_space_size / self.n_matching)
             )
 
         self.n_iterations = n_iterations
 
-        self._qcircuit = QCircuit(self.search_space_size)
+        self._qcircuit = QCircuit(self.search_space_size, name=f"grover__{oracle.name}")
 
         # State preparation
         self._qcircuit.barrier(label="s")
         for i in range(self.search_space_size):
             self._qcircuit.h(i)
 
         # Prepare and add the quantum oracle
```

### Comparing `qlasskit-0.1.8/qlasskit/algorithms/qalgorithm.py` & `qlasskit-0.1.9/qlasskit/algorithms/qalgorithm.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/algorithms/simon.py` & `qlasskit-0.1.9/qlasskit/algorithms/simon.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             f (QlassF): our f(x)
         """
         if len(f.args) != 1:
             raise Exception("f should receive exactly one parameter")
 
         self.f: QlassF = f
         self.search_space_size = len(f.args[0])
-        self._qcircuit = QCircuit(self.f.num_qubits)
+        self._qcircuit = QCircuit(self.f.num_qubits, name=f"simon_{f.name}")
 
         # State preparation
         self._qcircuit.barrier(label="s")
         for i in range(self.search_space_size):
             self._qcircuit.h(i)
 
         # Prepare and add the f
```

### Comparing `qlasskit-0.1.8/qlasskit/ast2ast.py` & `qlasskit-0.1.9/qlasskit/ast2ast.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/ast2logic/__init__.py` & `qlasskit-0.1.9/qlasskit/ast2logic/__init__.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/ast2logic/env.py` & `qlasskit-0.1.9/qlasskit/ast2logic/env.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/ast2logic/exceptions.py` & `qlasskit-0.1.9/qlasskit/ast2logic/exceptions.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/ast2logic/t_arguments.py` & `qlasskit-0.1.9/qlasskit/ast2logic/t_arguments.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/ast2logic/t_ast.py` & `qlasskit-0.1.9/qlasskit/ast2logic/t_ast.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/ast2logic/t_expression.py` & `qlasskit-0.1.9/qlasskit/ast2logic/t_expression.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/ast2logic/t_statement.py` & `qlasskit-0.1.9/qlasskit/ast2logic/t_statement.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/ast2logic/typing.py` & `qlasskit-0.1.9/qlasskit/ast2logic/typing.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/ast2logic/utils.py` & `qlasskit-0.1.9/qlasskit/ast2logic/utils.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/boolopt/__init__.py` & `qlasskit-0.1.9/test/test_bool_optimizer.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,11 +7,15 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# isort:skip_file
 
-from .sympytransformer import SympyTransformer  # noqa: F401
-from .bool_optimizer import BoolOptimizerProfile, bestWorkingOptimizer  # noqa: F401
+import unittest
+
+from parameterized import parameterized_class
+from sympy import And, Not, Or, Symbol, symbols
+from sympy.logic.boolalg import BooleanTrue
+
+from qlasskit.boolopt import bool_optimizer
```

### Comparing `qlasskit-0.1.8/qlasskit/boolopt/bool_optimizer.py` & `qlasskit-0.1.9/qlasskit/boolopt/bool_optimizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,31 +79,41 @@
             if isinstance(opt, SympyTransformer):
                 exps = list(map(lambda e: (e[0], opt.visit(e[1])), exps))
             else:
                 exps = opt(exps)
         return exps
 
 
-bestWorkingOptimizer = BoolOptimizerProfile(
+defaultOptimizer = BoolOptimizerProfile(
     [
         merge_expressions,
         apply_cse,
         remove_ITE(),
         remove_Implies(),
         transform_or2xor(),
         transform_or2and(),
     ]
 )
 
 
-bestWorkingOptimizerDebug = BoolOptimizerProfile(
+defaultOptimizerDebug = BoolOptimizerProfile(
     [
         print_step("before"),
         merge_expressions,
         apply_cse,
         remove_ITE(),
         remove_Implies(),
         transform_or2xor(),
         transform_or2and(),
         print_step("after"),
     ]
 )
+
+
+fastOptimizer = BoolOptimizerProfile(
+    [
+        remove_ITE(),
+        remove_Implies(),
+        transform_or2xor(),
+        transform_or2and(),
+    ]
+)
```

### Comparing `qlasskit-0.1.8/qlasskit/boolopt/exp_transformers.py` & `qlasskit-0.1.9/qlasskit/boolopt/exp_transformers.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/boolopt/sympytransformer.py` & `qlasskit-0.1.9/qlasskit/boolopt/sympytransformer.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/boolquant.py` & `qlasskit-0.1.9/qlasskit/boolquant.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/compiler/__init__.py` & `qlasskit-0.1.9/qlasskit/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/compiler/compiler.py` & `qlasskit-0.1.9/qlasskit/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/compiler/expqmap.py` & `qlasskit-0.1.9/qlasskit/compiler/expqmap.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/compiler/internalcompiler.py` & `qlasskit-0.1.9/qlasskit/compiler/internalcompiler.py`

 * *Files 11% similar despite different names*

```diff
@@ -52,15 +52,16 @@
                     a_false = qc.add_qubit("FALSE")
                 iret = a_false
             elif isinstance(symp_exp, BooleanTrue):
                 if not a_true:
                     a_true = qc.add_qubit("TRUE")
                     qc.x(a_true)
                 iret = a_true
-            elif isinstance(symp_exp, Symbol):
+            # Qubit mapped to another qubit (iff sym.name is a _ret)
+            elif isinstance(symp_exp, Symbol) and sym.name.startswith("_ret"):
                 iret = qc.add_qubit(sym.name)
                 qc.cx(qc[symp_exp.name], iret)
             else:
                 iret = self.compile_expr(qc, symp_exp)
 
             self.expqmap[sym] = iret
             qc.map_qubit(sym, iret, promote=not is_temp)
@@ -87,22 +88,22 @@
                 raise CompilerException(f"Symbol not found in qc: {expr.name}")
 
         elif expr in self.expqmap:
             return self.expqmap[expr]
 
         elif isinstance(expr, Xor):
             d = qc.get_free_ancilla()
-            neg = False
+
             for e in expr.args:
                 if isinstance(e, Symbol):
                     qc.cx(qc[e], d)
                 else:
-                    d = self.compile_expr(qc, e, dest=d)
-            if neg:
-                qc.x(d)
+                    d2 = self.compile_expr(qc, e)
+                    qc.cx(d2, d)
+
             self.expqmap[expr] = d
             return d
 
         elif isinstance(expr, Not):
             eret = self.compile_expr(qc, expr.args[0])
 
             if eret in qc.ancilla_lst:
```

### Comparing `qlasskit-0.1.8/qlasskit/compiler/tweedledumcompiler.py` & `qlasskit-0.1.9/qlasskit/compiler/tweedledumcompiler.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/qcircuit/__init__.py` & `qlasskit-0.1.9/qlasskit/qcircuit/__init__.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/qcircuit/cnotsim.py` & `qlasskit-0.1.9/qlasskit/qcircuit/cnotsim.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/qcircuit/exporter.py` & `qlasskit-0.1.9/qlasskit/qcircuit/exporter.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/qcircuit/exporter_cirq.py` & `qlasskit-0.1.9/qlasskit/qcircuit/exporter_cirq.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/qcircuit/exporter_qasm.py` & `qlasskit-0.1.9/qlasskit/qcircuit/exporter_qasm.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/qcircuit/exporter_qiskit.py` & `qlasskit-0.1.9/qlasskit/qcircuit/exporter_qiskit.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/qcircuit/exporter_sympy.py` & `qlasskit-0.1.9/qlasskit/qcircuit/exporter_sympy.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/qcircuit/gates.py` & `qlasskit-0.1.9/qlasskit/qcircuit/gates.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/qcircuit/qcircuit.py` & `qlasskit-0.1.9/qlasskit/qcircuit/qcircuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,20 @@
     def get_key_by_index(self, i: int):
         """Return the qubit name given its index"""
         for key in self.qubit_map:
             if self.qubit_map[key] == i:
                 return key
         raise Exception(f"Qubit with index {i} not found")
 
+    def __repr__(self):
+        """Return a string representation of the QCircuit"""
+        return (
+            f"QCircuit<{self.name}>({self.num_gates} gates, {self.num_qubits} qubits)"
+        )
+
     def __contains__(self, key: Union[str, Symbol, int]):
         """Return True if the circuit contain a qubit with a given name/symbol"""
         if isinstance(key, str):
             return key in self.qubit_map
         elif isinstance(key, Symbol):
             return key.name in self.qubit_map
         return False
```

### Comparing `qlasskit-0.1.8/qlasskit/qcircuit/qcircuitenhanced.py` & `qlasskit-0.1.9/qlasskit/qcircuit/qcircuitenhanced.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/qcircuit/qcircuitwrapper.py` & `qlasskit-0.1.9/qlasskit/qcircuit/qcircuitwrapper.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/qlassfun.py` & `qlasskit-0.1.9/qlasskit/qlassfun.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from functools import reduce
 from typing import Callable, Dict, List, Tuple, Union, get_args  # noqa: F401
 
 from sympy import Symbol
 
 from .ast2ast import ast2ast
 from .ast2logic import Arg, Args, BoolExpList, LogicFun, flatten, translate_ast
-from .boolopt import BoolOptimizerProfile, bestWorkingOptimizer
+from .boolopt import BoolOptimizerProfile, defaultOptimizer
 from .boolopt.bool_optimizer import merge_expressions
 from .boolquant import Q  # noqa: F403, F401
 from .compiler import SupportedCompiler, to_quantum
 from .qcircuit import QCircuitWrapper
 from .types import *  # noqa: F403, F401
 from .types import Qtype, format_outcome, interpret_as_qtype, type_repr
 
@@ -183,27 +183,27 @@
     @staticmethod
     def from_function(
         f: Union[str, Callable],
         types: List[Qtype] = [],
         defs: List[LogicFun] = [],
         to_compile: bool = True,
         compiler: SupportedCompiler = "internal",
-        bool_optimizer: BoolOptimizerProfile = bestWorkingOptimizer,
+        bool_optimizer: BoolOptimizerProfile = defaultOptimizer,
         uncompute: bool = True,
     ) -> "QlassF":
         """Create a QlassF from a function or a string containing a function
 
         Args:
             f (Union[str, Callable]): the function to be parsed, as a str code or callable
             types (List[Qtype]): list of qtypes to inject
             defs (List[LogicFun]): list of LogicFun to inject
             to_compile (boolean, optional): if True, compile to quantum circuit (default: True)
             compiler (SupportedCompiler, optional): override default compiler (default: internal)
             bool_optimizer (BoolOptimizerProfile, optional): override default optimizer
-                (default: bestWorkingOptimizer)
+                (default: defaultOptimizer)
             uncompute (bool, optional): whenever uncompute input qubits during compilation
                 (default: True)
         """
         if isinstance(f, str):
             exec(f)
 
         fun_ast = ast.parse(f if isinstance(f, str) else inspect.getsource(f))
@@ -224,27 +224,27 @@
 
 def qlassf(
     f: Union[str, Callable],
     types: List[Qtype] = [],
     defs: List[QlassF] = [],
     to_compile: bool = True,
     compiler: SupportedCompiler = "internal",
-    bool_optimizer: BoolOptimizerProfile = bestWorkingOptimizer,
+    bool_optimizer: BoolOptimizerProfile = defaultOptimizer,
     uncompute: bool = True,
 ) -> QlassF:
     """Decorator / function creating a QlassF object
 
     Args:
         f (Union[str, Callable]): the function to be parsed, as a str code or callable
         types (List[Qtype]): list of qtypes to inject
         defs (List[Qlassf]): list of qlassf to inject
         to_compile (boolean, optional): if True, compile to quantum circuit (default: True)
         compiler (SupportedCompiler, optional): override default compiler (default: internal)
         bool_optimizer (BoolOptimizerProfile, optional): override default optimizer
-            (default: bestWorkingOptimizer)
+            (default: defaultOptimizer)
         uncompute (bool, optional): whenever uncompute input qubits during compilation
             (default: True)
     """
     defs_fun = list(map(lambda q: q.to_logicfun(), defs))
 
     return QlassF.from_function(
         f,
@@ -258,15 +258,15 @@
 
 
 def qlassfa(
     types: List[Qtype] = [],
     defs: List[QlassF] = [],
     to_compile: bool = True,
     compiler: SupportedCompiler = "internal",
-    bool_optimizer: BoolOptimizerProfile = bestWorkingOptimizer,
+    bool_optimizer: BoolOptimizerProfile = defaultOptimizer,
     uncompute: bool = True,
 ):
     """Decorator with parameters for qlassf"""
 
     def _inner(fun):
         return qlassf(fun, types, defs, to_compile, compiler, bool_optimizer, uncompute)
```

### Comparing `qlasskit-0.1.8/qlasskit/types/__init__.py` & `qlasskit-0.1.9/qlasskit/types/__init__.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/types/qbool.py` & `qlasskit-0.1.9/qlasskit/types/qbool.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/types/qint.py` & `qlasskit-0.1.9/qlasskit/types/qint.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,15 +177,15 @@
     @classmethod
     def mul(cls, tleft: TExp, tright: TExp) -> TExp:  # noqa: C901
         # TODO: use RGQFT multiplier
         n = len(tleft[1])
         m = len(tright[1])
 
         if n != m:
-            raise Exception("Mul works only on same size Qint")
+            raise Exception(f"Mul works only on same size Qint: {n} != {m}")
 
         product = [False] * (n + m)
 
         for i in range(n):
             carry = False
             for j in range(m):
                 partial_product = And(tleft[1][i], tright[1][j])
@@ -206,14 +206,16 @@
             return Qint4, product
         elif (n + m) > 4 and (n + m) <= 8:
             return Qint8, product
         elif (n + m) > 8 and (n + m) <= 12:
             return Qint12, product
         elif (n + m) > 12 and (n + m) <= 16:
             return Qint16, product
+        elif (n + m) > 16:
+            return Qint16.crop((Qint16, product))
 
         raise Exception(f"Mul result size is too big ({n+m})")
 
     @classmethod
     def sub(cls, tleft: TExp, tright: TExp) -> TExp:
         """Subtract two Qint"""
         an = cls.bitwise_not(cls.fill(tleft))  # type: ignore
```

### Comparing `qlasskit-0.1.8/qlasskit/types/qlist.py` & `qlasskit-0.1.9/qlasskit/types/qlist.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/types/qmatrix.py` & `qlasskit-0.1.9/qlasskit/types/qmatrix.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit/types/qtype.py` & `qlasskit-0.1.9/qlasskit/types/qtype.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/qlasskit.egg-info/PKG-INFO` & `qlasskit-0.1.9/qlasskit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qlasskit
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python-to-quantum compiler
 Home-page: https://github.com/dakk/qlasskit
 Author: Davide Gessa
 Author-email: gessadavide@gmail.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/dakk/qlasskit/issues/
 Project-URL: Documentation, https://dakk.github.io/qlasskit
```

### Comparing `qlasskit-0.1.8/qlasskit.egg-info/SOURCES.txt` & `qlasskit-0.1.9/qlasskit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/setup.py` & `qlasskit-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/test/test_algo.py` & `qlasskit-0.1.9/test/test_algo.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/test/test_algo_deutschjozsa.py` & `qlasskit-0.1.9/test/test_algo_deutschjozsa.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/test/test_algo_grover.py` & `qlasskit-0.1.9/test/test_algo_grover.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/test/test_algo_simon.py` & `qlasskit-0.1.9/test/test_algo_simon.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,9 +35,9 @@
 
         qc = algo.circuit().export("circuit", "qiskit")
         counts = qiskit_measure_and_count(qc, shots=1024)
         counts_readable = algo.decode_counts(counts)
 
         for x in [0, 8]:
             self.assertEqual(x in counts_readable, True)
-            self.assertEqual(counts_readable[x] > 480, True)
+            self.assertEqual(counts_readable[x] > 400, True)
         self.assertEqual(algo.output_qubits, [0, 1, 2, 3])
```

### Comparing `qlasskit-0.1.8/test/test_ast2logic_t_arg.py` & `qlasskit-0.1.9/test/test_ast2logic_t_arg.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/test/test_ast2logic_t_exp.py` & `qlasskit-0.1.9/test/test_ast2logic_t_exp.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/test/test_ast2logic_t_stmt.py` & `qlasskit-0.1.9/test/test_ast2logic_t_stmt.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/test/test_compiler.py` & `qlasskit-0.1.9/test/test_compiler.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/test/test_qcircuit.py` & `qlasskit-0.1.9/test/test_qcircuit.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/test/test_qlassf.py` & `qlasskit-0.1.9/test/test_qlassf.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 import unittest
 
 from parameterized import parameterized_class
 
 from qlasskit import Qint, Qint2, Qint4, Qint12, QlassF, exceptions, qlassf
-from qlasskit.boolopt.bool_optimizer import bestWorkingOptimizerDebug
+from qlasskit.boolopt.bool_optimizer import defaultOptimizerDebug
 
 from . import utils
 from .utils import COMPILATION_ENABLED, ENABLED_COMPILERS, compute_and_compare_results
 
 
 class TestQlassfDecorator(unittest.TestCase):
     def test_decorator(self):
@@ -30,15 +30,15 @@
 
 
 class TestQlassfOptimizerSelection(unittest.TestCase):
     def test_debug_optimizer(self):
         qf = qlassf(
             "def t(a: bool) -> bool: return a",
             to_compile=COMPILATION_ENABLED,
-            bool_optimizer=bestWorkingOptimizerDebug,
+            bool_optimizer=defaultOptimizerDebug,
         )
         compute_and_compare_results(self, qf)
 
 
 @parameterized_class(("compiler"), ENABLED_COMPILERS)
 class TestQlassfCustomTypes(unittest.TestCase):
     def test_custom_qint5(self):
```

### Comparing `qlasskit-0.1.8/test/test_qlassf_bool.py` & `qlasskit-0.1.9/test/test_qlassf_bool.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/test/test_qlassf_builtin.py` & `qlasskit-0.1.9/test/test_qlassf_builtin.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/test/test_qlassf_for_loop.py` & `qlasskit-0.1.9/test/test_qlassf_for_loop.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/test/test_qlassf_functiondef.py` & `qlasskit-0.1.9/test/test_qlassf_functiondef.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/test/test_qlassf_hybrid_quantum.py` & `qlasskit-0.1.9/test/test_qlassf_hybrid_quantum.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,7 +36,13 @@
 
     def test_bell(self):
         f = "def test(a: bool, b: bool) -> bool:\n\treturn Q.CX(Q.H(a), b)"
         qf = qlassf(f, to_compile=COMPILATION_ENABLED, uncompute=False)
         count = qiskit_measure_and_count(qf.circuit().export(), 1024)
         [self.assertEqual(x in count, True) for x in ["00", "11"]]
         self.assertEqual(len(count.keys()), 2)
+
+    def test_h_and_add(self):
+        f = "def test(a: Qint2) -> Qint2:\n\ta = Q.H(a)\n\treturn a + 1"
+        qf = qlassf(f, to_compile=COMPILATION_ENABLED, uncompute=False)
+        count = qiskit_measure_and_count(qf.circuit().export(), 128)
+        [self.assertEqual(x in count, True) for x in ["1110", "0011", "1001", "0100"]]
```

### Comparing `qlasskit-0.1.8/test/test_qlassf_ifthenelse.py` & `qlasskit-0.1.9/test/test_qlassf_ifthenelse.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/test/test_qlassf_int.py` & `qlasskit-0.1.9/test/test_qlassf_int.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/test/test_qlassf_list.py` & `qlasskit-0.1.9/test/test_qlassf_list.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/test/test_qlassf_matrix.py` & `qlasskit-0.1.9/test/test_qlassf_matrix.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/test/test_qlassf_tuple.py` & `qlasskit-0.1.9/test/test_qlassf_tuple.py`

 * *Files identical despite different names*

### Comparing `qlasskit-0.1.8/test/test_types.py` & `qlasskit-0.1.9/test/test_types.py`

 * *Files identical despite different names*

