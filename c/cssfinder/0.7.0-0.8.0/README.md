# Comparing `tmp/cssfinder-0.7.0.tar.gz` & `tmp/cssfinder-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cssfinder-0.7.0.tar", max compression
+gzip compressed data, was "cssfinder-0.8.0.tar", max compression
```

## Comparing `cssfinder-0.7.0.tar` & `cssfinder-0.8.0.tar`

### file list

```diff
@@ -1,86 +1,88 @@
--rw-r--r--   0        0        0     1069 2023-05-19 13:27:27.719206 cssfinder-0.7.0/LICENSE.md
--rw-r--r--   0        0        0    14948 2023-05-19 13:27:27.719206 cssfinder-0.7.0/README.md
--rw-r--r--   0        0        0     1417 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/__init__.py
--rw-r--r--   0        0        0     1280 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/__main__.py
--rw-r--r--   0        0        0     1224 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/algorithm/__init__.py
--rw-r--r--   0        0        0     1308 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/algorithm/backend/__init__.py
--rw-r--r--   0        0        0     3951 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/algorithm/backend/base.py
--rw-r--r--   0        0        0     6456 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/algorithm/backend/loader.py
--rw-r--r--   0        0        0     6934 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/algorithm/gilbert.py
--rw-r--r--   0        0        0     6857 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/algorithm/mode_util.py
--rw-r--r--   0        0        0    10007 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/api.py
--rw-r--r--   0        0        0     1676 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/base_model.py
--rw-r--r--   0        0        0    21413 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/cli.py
--rw-r--r--   0        0        0     3875 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/constants.py
--rw-r--r--   0        0        0     4915 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/crossplatform.py
--rw-r--r--   0        0        0    23376 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/cssfproject.py
--rw-r--r--   0        0        0     2169 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/enums.py
--rw-r--r--   0        0        0       10 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/.gitignore
--rw-r--r--   0        0        0     1192 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/5qubits_json/5qubits_in.mtx
--rw-r--r--   0        0        0     1819 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/5qubits_json/cssfproject.json
--rw-r--r--   0        0        0     1192 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/5qubits_py/5qubits_in.mtx
--rw-r--r--   0        0        0     2667 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/5qubits_py/cssfproject.py
--rw-r--r--   0        0        0     1036 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ3_json/GHZ3_in.mtx
--rw-r--r--   0        0        0     2874 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ3_json/cssfproject.json
--rw-r--r--   0        0        0      175 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_0_0.mtx
--rw-r--r--   0        0        0      175 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_0_1.mtx
--rw-r--r--   0        0        0      175 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_0.mtx
--rw-r--r--   0        0        0     1762 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_1.mtx
--rw-r--r--   0        0        0      166 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_2.mtx
--rw-r--r--   0        0        0     1762 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_3.mtx
--rw-r--r--   0        0        0      183 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_4.mtx
--rw-r--r--   0        0        0     1762 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_5.mtx
--rw-r--r--   0        0        0      166 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_6.mtx
--rw-r--r--   0        0        0     1762 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_7.mtx
--rw-r--r--   0        0        0     3638 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ4_json/GHZ4_in.mtx
--rw-r--r--   0        0        0     1174 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ4_json/cssfproject.json
--rw-r--r--   0        0        0     2593 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/SBiPa_json/cssfproject.json
--rw-r--r--   0        0        0     1270 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/SBiPa_json/projection.mtx
--rw-r--r--   0        0        0     1270 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/SBiPa_json/state.mtx
--rw-r--r--   0        0        0     5139 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/__init__.py
--rw-r--r--   0        0        0     1192 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/benchmark_32x32/5qubits_in.mtx
--rw-r--r--   0        0        0     2957 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/benchmark_32x32/cssfproject.py
--rw-r--r--   0        0        0    54182 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/10_in.mtx
--rw-r--r--   0        0        0     3693 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/cssfproject.py
--rw-r--r--   0        0        0     4265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_0.mtx
--rw-r--r--   0        0        0   108265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_1.mtx
--rw-r--r--   0        0        0   108265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_2.mtx
--rw-r--r--   0        0        0   108265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_3.mtx
--rw-r--r--   0        0        0     4297 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_4.mtx
--rw-r--r--   0        0        0   108265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_5.mtx
--rw-r--r--   0        0        0   108265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_6.mtx
--rw-r--r--   0        0        0   108265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_7.mtx
--rw-r--r--   0        0        0     4265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_0.mtx
--rw-r--r--   0        0        0   106596 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_1.mtx
--rw-r--r--   0        0        0   106596 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_2.mtx
--rw-r--r--   0        0        0   106596 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_3.mtx
--rw-r--r--   0        0        0     4281 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_4.mtx
--rw-r--r--   0        0        0   106596 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_5.mtx
--rw-r--r--   0        0        0   106596 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_6.mtx
--rw-r--r--   0        0        0   106596 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_7.mtx
--rw-r--r--   0        0        0     4265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_0.mtx
--rw-r--r--   0        0        0   108265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_1.mtx
--rw-r--r--   0        0        0   108265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_2.mtx
--rw-r--r--   0        0        0   108265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_3.mtx
--rw-r--r--   0        0        0     4297 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_4.mtx
--rw-r--r--   0        0        0   108265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_5.mtx
--rw-r--r--   0        0        0   108265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_6.mtx
--rw-r--r--   0        0        0   108265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_7.mtx
--rw-r--r--   0        0        0    14212 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/interactive.py
--rw-r--r--   0        0        0     1227 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/io/__init__.py
--rw-r--r--   0        0        0     6003 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/io/gilbert_io.py
--rw-r--r--   0        0        0     4182 2023-05-19 13:27:27.727206 cssfinder-0.7.0/cssfinder/io/matrix.py
--rwxr-xr-x   0        0        0    12147 2023-05-19 13:27:27.727206 cssfinder-0.7.0/cssfinder/log.py
--rw-r--r--   0        0        0     1666 2023-05-19 13:27:27.727206 cssfinder-0.7.0/cssfinder/reports/__init__.py
--rw-r--r--   0        0        0     1291 2023-05-19 13:27:27.727206 cssfinder-0.7.0/cssfinder/reports/archive.py
--rw-r--r--   0        0        0     2200 2023-05-19 13:27:27.727206 cssfinder-0.7.0/cssfinder/reports/html.py
--rw-r--r--   0        0        0     1845 2023-05-19 13:27:27.727206 cssfinder-0.7.0/cssfinder/reports/json.py
--rw-r--r--   0        0        0     4292 2023-05-19 13:27:27.727206 cssfinder-0.7.0/cssfinder/reports/manager.py
--rw-r--r--   0        0        0     9298 2023-05-19 13:27:27.727206 cssfinder-0.7.0/cssfinder/reports/math.py
--rw-r--r--   0        0        0     2937 2023-05-19 13:27:27.727206 cssfinder-0.7.0/cssfinder/reports/pdf.py
--rw-r--r--   0        0        0     8299 2023-05-19 13:27:27.727206 cssfinder-0.7.0/cssfinder/reports/plotting.py
--rw-r--r--   0        0        0     4889 2023-05-19 13:27:27.727206 cssfinder-0.7.0/cssfinder/reports/renderer.py
--rw-r--r--   0        0        0     1203 2023-05-19 13:27:27.727206 cssfinder-0.7.0/cssfinder/reports/txt.py
--rw-r--r--   0        0        0     3947 2023-05-19 13:27:27.727206 cssfinder-0.7.0/cssfinder/templates/report.html.jinja2
--rw-r--r--   0        0        0    17232 2023-05-19 13:27:27.731206 cssfinder-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    16452 1970-01-01 00:00:00.000000 cssfinder-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-16 23:11:37.552849 cssfinder-0.8.0/LICENSE.md
+-rw-r--r--   0        0        0     6494 2024-04-16 23:11:37.552849 cssfinder-0.8.0/README.md
+-rw-r--r--   0        0        0     1417 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/__init__.py
+-rw-r--r--   0        0        0     1280 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/__main__.py
+-rw-r--r--   0        0        0     1224 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/algorithm/__init__.py
+-rw-r--r--   0        0        0     1308 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/algorithm/backend/__init__.py
+-rw-r--r--   0        0        0     3943 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/algorithm/backend/base.py
+-rw-r--r--   0        0        0     6482 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/algorithm/backend/loader.py
+-rw-r--r--   0        0        0     6960 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/algorithm/gilbert.py
+-rw-r--r--   0        0        0     6857 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/algorithm/mode_util.py
+-rw-r--r--   0        0        0    10977 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/api.py
+-rw-r--r--   0        0        0     1676 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/base_model.py
+-rw-r--r--   0        0        0    29010 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/cli.py
+-rw-r--r--   0        0        0     3875 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/constants.py
+-rw-r--r--   0        0        0     4915 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/crossplatform.py
+-rw-r--r--   0        0        0    24857 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/cssfproject.py
+-rw-r--r--   0        0        0     2169 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/enums.py
+-rw-r--r--   0        0        0       10 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/.gitignore
+-rw-r--r--   0        0        0     1192 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/5qubits_json/5qubits_in.mtx
+-rw-r--r--   0        0        0     1819 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/5qubits_json/cssfproject.json
+-rw-r--r--   0        0        0     1192 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/5qubits_py/5qubits_in.mtx
+-rw-r--r--   0        0        0     2666 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/5qubits_py/cssfproject.py
+-rw-r--r--   0        0        0     1036 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/GHZ3_json/GHZ3_in.mtx
+-rw-r--r--   0        0        0     2874 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/GHZ3_json/cssfproject.json
+-rw-r--r--   0        0        0      175 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_0_0.mtx
+-rw-r--r--   0        0        0      175 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_0_1.mtx
+-rw-r--r--   0        0        0      175 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_0.mtx
+-rw-r--r--   0        0        0     1762 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_1.mtx
+-rw-r--r--   0        0        0      166 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_2.mtx
+-rw-r--r--   0        0        0     1762 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_3.mtx
+-rw-r--r--   0        0        0      183 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_4.mtx
+-rw-r--r--   0        0        0     1762 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_5.mtx
+-rw-r--r--   0        0        0      166 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_6.mtx
+-rw-r--r--   0        0        0     1762 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_7.mtx
+-rw-r--r--   0        0        0     3638 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/GHZ4_json/GHZ4_in.mtx
+-rw-r--r--   0        0        0     1174 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/GHZ4_json/cssfproject.json
+-rw-r--r--   0        0        0     2593 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/SBiPa_json/cssfproject.json
+-rw-r--r--   0        0        0     1270 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/SBiPa_json/projection.mtx
+-rw-r--r--   0        0        0     1270 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/SBiPa_json/state.mtx
+-rw-r--r--   0        0        0     5140 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/__init__.py
+-rw-r--r--   0        0        0     1192 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/benchmark_32x32/5qubits_in.mtx
+-rw-r--r--   0        0        0     2957 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/benchmark_32x32/cssfproject.py
+-rw-r--r--   0        0        0    54182 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/10_in.mtx
+-rw-r--r--   0        0        0     3693 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/cssfproject.py
+-rw-r--r--   0        0        0     4265 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_0.mtx
+-rw-r--r--   0        0        0   108265 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_1.mtx
+-rw-r--r--   0        0        0   108265 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_2.mtx
+-rw-r--r--   0        0        0   108265 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_3.mtx
+-rw-r--r--   0        0        0     4297 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_4.mtx
+-rw-r--r--   0        0        0   108265 2024-04-16 23:11:37.556849 cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_5.mtx
+-rw-r--r--   0        0        0   108265 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_6.mtx
+-rw-r--r--   0        0        0   108265 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_7.mtx
+-rw-r--r--   0        0        0     4265 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_0.mtx
+-rw-r--r--   0        0        0   106596 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_1.mtx
+-rw-r--r--   0        0        0   106596 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_2.mtx
+-rw-r--r--   0        0        0   106596 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_3.mtx
+-rw-r--r--   0        0        0     4281 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_4.mtx
+-rw-r--r--   0        0        0   106596 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_5.mtx
+-rw-r--r--   0        0        0   106596 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_6.mtx
+-rw-r--r--   0        0        0   106596 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_7.mtx
+-rw-r--r--   0        0        0     4265 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_0.mtx
+-rw-r--r--   0        0        0   108265 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_1.mtx
+-rw-r--r--   0        0        0   108265 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_2.mtx
+-rw-r--r--   0        0        0   108265 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_3.mtx
+-rw-r--r--   0        0        0     4297 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_4.mtx
+-rw-r--r--   0        0        0   108265 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_5.mtx
+-rw-r--r--   0        0        0   108265 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_6.mtx
+-rw-r--r--   0        0        0   108265 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_7.mtx
+-rw-r--r--   0        0        0    14513 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/interactive.py
+-rw-r--r--   0        0        0     1227 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/io/__init__.py
+-rw-r--r--   0        0        0     6037 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/io/gilbert_io.py
+-rw-r--r--   0        0        0     4264 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/io/matrix.py
+-rw-r--r--   0        0        0      352 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/jinja2_tools.py
+-rwxr-xr-x   0        0        0    12192 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/log.py
+-rw-r--r--   0        0        0     1666 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/reports/__init__.py
+-rw-r--r--   0        0        0     1291 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/reports/archive.py
+-rw-r--r--   0        0        0     2153 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/reports/html.py
+-rw-r--r--   0        0        0     1845 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/reports/json.py
+-rw-r--r--   0        0        0     4358 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/reports/manager.py
+-rw-r--r--   0        0        0     9250 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/reports/math.py
+-rw-r--r--   0        0        0     2937 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/reports/pdf.py
+-rw-r--r--   0        0        0     8324 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/reports/plotting.py
+-rw-r--r--   0        0        0     4892 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/reports/renderer.py
+-rw-r--r--   0        0        0     1203 2024-04-16 23:11:37.560849 cssfinder-0.8.0/cssfinder/reports/txt.py
+-rw-r--r--   0        0        0     1756 2024-04-16 23:11:37.564849 cssfinder-0.8.0/cssfinder/templates/python_base_project.pyjinja2
+-rw-r--r--   0        0        0     3947 2024-04-16 23:11:37.564849 cssfinder-0.8.0/cssfinder/templates/report.html.jinja2
+-rw-r--r--   0        0        0    12407 2024-04-16 23:11:37.568849 cssfinder-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     8095 1970-01-01 00:00:00.000000 cssfinder-0.8.0/PKG-INFO
```

### Comparing `cssfinder-0.7.0/LICENSE.md` & `cssfinder-0.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/__init__.py` & `cssfinder-0.8.0/cssfinder/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 """CSSFinder (Closest Separable State Finder) is a package containing implementation of
 Gilbert algorithm for finding an upper bound on the Hilbert-Schmidt distance between a
 given state and the set of separable states.
 """
 
 from __future__ import annotations
 
-__version__ = "0.7.0"
+__version__ = "0.8.0"
```

### Comparing `cssfinder-0.7.0/cssfinder/__main__.py` & `cssfinder-0.8.0/cssfinder/__main__.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/algorithm/__init__.py` & `cssfinder-0.8.0/cssfinder/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/algorithm/backend/__init__.py` & `cssfinder-0.8.0/cssfinder/algorithm/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/algorithm/backend/base.py` & `cssfinder-0.8.0/cssfinder/algorithm/backend/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 class BackendBase:
     """Gilbert algorithm backend (implementation)."""
 
     author: ClassVar[str] = ""
     description: ClassVar[str] = ""
 
-    def __init__(  # noqa: PLR0913
+    def __init__(
         self,
         initial: npt.NDArray[np.complex128],
         depth: int,
         quantity: int,
         mode: AlgoMode,
         visibility: float,
         *,
@@ -57,15 +57,16 @@
         self.quantity = quantity
         self.initial = initial
         self.visibility = visibility
         self.mode = mode
         self.is_debug = is_debug
 
     def set_symmetries(
-        self, symmetries: list[list[npt.NDArray[np.complex128]]]
+        self,
+        symmetries: list[list[npt.NDArray[np.complex128]]],
     ) -> None:
         """Set symmetries to use during calculations.
 
         This operation may involve type conversion and copying of symmetries, therefore
         if may be slow and should should be done only once.
 
         Parameters
```

### Comparing `cssfinder-0.7.0/cssfinder/algorithm/backend/loader.py` & `cssfinder-0.8.0/cssfinder/algorithm/backend/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 LEN_KEY_TUPLE = 2
 
 
 class Loader:
     """Backend loader class."""
 
     BACKEND_NAME_REGEX: ClassVar[re.Pattern] = re.compile(
-        r"cssfinder(_|-)backend(_|-)[a-z0-9_\-]+", re.IGNORECASE
+        r"cssfinder(_|-)backend(_|-)[a-z0-9_\-]+",
+        re.IGNORECASE,
     )
 
     def __init__(self) -> None:
         self.reload()
 
     def reload(self) -> None:
         """Load all backends available in python environment.
@@ -165,15 +166,15 @@
                 table.add_row(
                     name,
                     precision.name,
                     getattr(cls, "author", ""),
                     f"{cls.__module__}.{cls.__qualname__}",
                     getattr(cls, "description", ""),
                 )
-            except (TypeError, ValueError):
+            except (TypeError, ValueError):  # noqa: PERF203
                 logging.warning("Failed to display information about backed %r", value)
 
         return table
 
 
 class BackendNotAvailableError(KeyError):
     """Raised when backend with specified features can not be found."""
```

### Comparing `cssfinder-0.7.0/cssfinder/algorithm/gilbert.py` & `cssfinder-0.8.0/cssfinder/algorithm/gilbert.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     from cssfinder.cssfproject import AlgoMode, Precision
 
 
 class Gilbert:
     """Class interface of gilbert algorithm."""
 
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         *,
         initial: npt.NDArray[np.complex128],
         depth: int,
         quantity: int,
         mode: AlgoMode,
         backend: str,
@@ -68,15 +68,16 @@
             self.quantity,
             self.mode,
             self.visibility,
             is_debug=self.is_debug,
         )
 
     def set_symmetries(
-        self, symmetries: list[list[npt.NDArray[np.complex128]]]
+        self,
+        symmetries: list[list[npt.NDArray[np.complex128]]],
     ) -> None:
         """Set symmetries to use during calculations.
 
         This operation may involve type conversion and copying of symmetries, therefore
         if may be slow and should should be done only once.
 
         Parameters
```

### Comparing `cssfinder-0.7.0/cssfinder/algorithm/mode_util.py` & `cssfinder-0.8.0/cssfinder/algorithm/mode_util.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/api.py` & `cssfinder-0.8.0/cssfinder/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 import traceback
 from concurrent.futures import ProcessPoolExecutor
 from dataclasses import dataclass
 from itertools import repeat
 from typing import TYPE_CHECKING, Iterable
 
 import psutil
+import rich
+from rich.panel import Panel
 
 from cssfinder.algorithm.gilbert import Gilbert
 from cssfinder.algorithm.mode_util import ModeUtil
 from cssfinder.crossplatform import IoPriority, Priority, set_priority
 from cssfinder.cssfproject import CSSFProject, GilbertCfg, Task
 from cssfinder.io.gilbert_io import GilbertIO
 from cssfinder.reports.manager import ReportManager
@@ -46,14 +48,15 @@
 
 
 def run_project_from(
     project_file_path: Path | str,
     tasks: list[str] | None = None,
     *,
     is_debug: bool = False,
+    is_rich: bool = True,
     force_sequential: bool = False,
     max_parallel: int = -1,
 ) -> None:
     """Load project and run all tasks."""
     project = CSSFProject.load_project(project_file_path)
     logging.info(
         "Loaded project %r by %r <%r>.",
@@ -61,61 +64,68 @@
         project.meta.author,
         project.meta.email,
     )
     run_project(
         project,
         tasks,
         is_debug=is_debug,
+        is_rich=is_rich,
         force_sequential=force_sequential,
         max_parallel=max_parallel,
     )
 
 
 def run_project(
     project: CSSFProject,
     tasks: list[str] | None = None,
     *,
     is_debug: bool = False,
+    is_rich: bool = True,
     force_sequential: bool = False,
     max_parallel: int = -1,
 ) -> list[Task]:
     """Run all tasks defined in project."""
     logging.debug("Running project %r", project.meta.name)
 
     message = "\n    |  ".join(project.json(indent=2).split("\n"))
     logging.info("%s", "\n    |  " + message)
 
     task_list = project.select_tasks(tasks)
 
     if force_sequential:
-        for _ in map(
+        for out in map(
             run_task,
             task_list,
             repeat(TaskOptions(is_debug=is_debug)),
         ):
-            pass
+            if isinstance(out, BaseException):
+                raise out
 
     else:
         with ProcessPoolExecutor(
-            max_parallel if max_parallel > 0 else None
+            max_parallel if max_parallel > 0 else None,
         ) as executor:
-            executor.map(
+            out = executor.map(
                 run_task,
                 task_list,
-                repeat(TaskOptions(is_debug=is_debug)),
+                repeat(TaskOptions(is_debug=is_debug, is_rich=is_rich)),
             )
+        for o in out:
+            if isinstance(o, BaseException):
+                raise o
 
     return task_list
 
 
 @dataclass
 class TaskOptions:
     """Container for extra task options."""
 
     is_debug: bool
+    is_rich: bool = True
 
 
 def run_task(task: Task, options: TaskOptions) -> None:
     """Run task until completed."""
     try:
         return _run_task(task, options)
     except Exception as e:
@@ -138,32 +148,45 @@
             "To allow automated priority elevation run this program as super user. "
             "You can change priority manually for process PID %r.",
             os.getpid(),
             stack_info=False,
         )
 
     if task.gilbert:
-        run_gilbert(task.gilbert, task.task_output_directory, is_debug=options.is_debug)
+        run_gilbert(
+            task.gilbert,
+            task.task_output_directory,
+            is_debug=options.is_debug,
+            is_rich=options.is_rich,
+        )
 
 
 def run_gilbert(
     config: GilbertCfg,
     task_output_directory: Path,
     *,
     is_debug: bool = False,
+    is_rich: bool = True,
 ) -> None:
     """Run Gilbert algorithm part of task."""
     asset_io = GilbertIO()
 
     task_output_directory.mkdir(0o777, parents=True, exist_ok=True)
     logging.debug("Created directory: %r", task_output_directory.as_posix())
 
     algorithm = create_gilbert(config, asset_io, is_debug=is_debug)
 
-    logging.warning("Task %r started.", config.task_name)
+    logging.info("Task %r started.", config.task_name)
+
+    if is_rich:
+        rich.print(Panel.fit(f"[blue]Task {config.task_name} started."))
+    else:
+        print("-----------------------")
+        print(f"| Task {config.task_name} started |")
+        print("-----------------------")
 
     for epoch_index in algorithm.run(
         max_epochs=config.runtime.max_epochs,
         iterations_per_epoch=config.runtime.iters_per_epoch,
         max_corrections=config.runtime.max_corrections,
     ):
         if corrections_count := algorithm.get_corrections_count():
@@ -187,17 +210,27 @@
                 epoch_index + 1,
                 config.runtime.max_epochs,
                 ((epoch_index + 1) / config.runtime.max_epochs) * 100,
             )
 
     logging.warning("Task %r finished.", config.task_name)
 
+    if is_rich:
+        rich.print(Panel.fit(f"[blue]Task {config.task_name} finished."))
+    else:
+        print("-----------------------")
+        print(f"| Task {config.task_name} finished |")
+        print("-----------------------")
+
 
 def create_gilbert(
-    config: GilbertCfg, asset_io: GilbertIO, *, is_debug: bool
+    config: GilbertCfg,
+    asset_io: GilbertIO,
+    *,
+    is_debug: bool,
 ) -> Gilbert:
     """Create Gilbert object from configuration with help of specified IO.
 
     Parameters
     ----------
     config : GilbertCfg
         Algorithm configuration.
@@ -210,15 +243,15 @@
     -------
     Gilbert
         Initialized
 
     """
     state_config = config.get_state()
 
-    initial_state = asset_io.load_state(state_config.file)
+    initial_state = asset_io.load_state(state_config.expanded_file)
 
     if state_config.is_predefined_dimensions():
         depth = state_config.get_depth()
         quantity = state_config.get_quantity()
         logging.info("Using fixed dimensions depth=%r quantity=%r", depth, quantity)
 
     else:
@@ -255,15 +288,17 @@
     if projection is not None:
         algorithm.set_projection(projection)
 
     return algorithm
 
 
 def create_report_from(
-    project_file_path: Path | str, task: str, reports: list[ReportType]
+    project_file_path: Path | str,
+    task: str,
+    reports: list[ReportType],
 ) -> Iterable[Report]:
     """Load project (`cssfproject.json`) and create report for task selected by pattern.
 
     Parameters
     ----------
     project_file_path : Path | str
         Path to cssfproject.json file or directory containing one.
@@ -291,27 +326,31 @@
         project.meta.author,
         project.meta.email,
     )
     yield from create_report(project, task, reports)
 
 
 def create_report(
-    project: CSSFProject, task: str, reports: list[ReportType]
+    project: CSSFProject,
+    task: str,
+    reports: list[ReportType],
 ) -> Iterable[Report]:
     """Create report for task selected by pattern from project object."""
     tasks = project.select_tasks([task])
 
     for task_object in tasks:
         logging.info("Creating summary for task %s", task_object.task_name)
 
         manager = ReportManager(project, task_object)
         prepared_manager = manager.prepare()
 
         for report_type in reports:
             logging.info(
-                "Report for task %s of type %s", task_object.task_name, report_type.name
+                "Report for task %s of type %s",
+                task_object.task_name,
+                report_type.name,
             )
             yield prepared_manager.request_report(report_type)
 
 
 class AmbiguousTaskKeyError(KeyError):
     """Raised during report creation when name pattern selects more than one task."""
```

### Comparing `cssfinder-0.7.0/cssfinder/base_model.py` & `cssfinder-0.8.0/cssfinder/base_model.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/constants.py` & `cssfinder-0.8.0/cssfinder/constants.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/crossplatform.py` & `cssfinder-0.8.0/cssfinder/crossplatform.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/cssfproject.py` & `cssfinder-0.8.0/cssfinder/cssfproject.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Optional, Union
 
 import jsonref
 from pydantic import ConstrainedStr, EmailStr, Field, validator
 
 from cssfinder.base_model import CommonBaseModel
 from cssfinder.enums import CaseInsensitiveEnum
+from cssfinder.jinja2_tools import get_cssfinder_jinja2_environment
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
 
 def project_file_path(directory_or_file: Path) -> Path:
     """Return path to project file (JSON/PY)."""
@@ -176,39 +177,49 @@
 
         if project_path.suffix == ".py":
             return cls._load_py_cssfproject(project_path)
 
         msg = f"Unknown project format {project_path.suffix} of project {project_path}"
         raise FileNotFoundError(msg)
 
+    @staticmethod
+    def is_project_path(file_or_directory: Path) -> bool:
+        """Check if path points to CSSFinder project file or project directory."""
+        try:
+            project_file_path(file_or_directory)
+        except FileNotFoundError:
+            return False
+        else:
+            return True
+
     @classmethod
     def _load_json_project(cls, project_path: Path) -> Self:
         logging.debug("Resolved project path to %r", project_path.as_posix())
         try:
             content = project_path.read_text(encoding="utf-8")
         except FileNotFoundError as exc:
             error_message = f"Make sure you path is correct: {project_path}"
             raise ProjectFileNotFoundError(error_message) from exc
 
         try:
-            content = jsonref.loads(content)
+            decoded_content = jsonref.loads(content)
         except json.decoder.JSONDecodeError as exc:
             raise MalformedProjectFileError(exc.msg, exc.doc, exc.pos) from exc
 
-        if not isinstance(content, dict):
+        if not isinstance(decoded_content, dict):
             logging.critical("Content of cssfproject.json file is not a dictionary.")
-            raise InvalidCSSFProjectContentError(content)
+            raise InvalidCSSFProjectContentError(decoded_content)
 
-        project = cls(**content, project_path=project_path)
-        return project
+        return cls(**decoded_content, project_path=project_path)
 
     @classmethod
     def _load_py_cssfproject(cls, project_path: Path) -> Self:
         spec = importlib.util.spec_from_file_location(
-            project_path.name[:-3], project_path.as_posix()
+            project_path.name[:-3],
+            project_path.as_posix(),
         )
         if spec is None or spec.loader is None:
             msg = f"Failed to load project file {project_path}"
             raise ImportError(msg)
 
         project_module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(project_module)
@@ -220,33 +231,50 @@
                 "Missing '__project__' field containing CSSFProject object.\n"
                 f"From {project_path}."
             )
             raise ImportError(msg)
 
         if not isinstance(project_object, cls):
             msg = (
+                f"Expected CSSFProject object in '__project__' field in {project_path}."
+            )
+            raise TypeError(
+                msg,
+            )
+
+        if not isinstance(project_object, cls):
+            msg = (
                 "Incorrect object in '__project__' field, should contain "
                 f"CSSFProject object.\nFrom {project_path}."
             )
 
-        assert isinstance(project_object, cls)
         return project_object
 
     def select_tasks(self, patterns: list[str] | None = None) -> list[Task]:
         """Select all tasks matching list of patterns."""
         if patterns is None:
             return list(self.tasks.values())
 
         keys = set()
 
         for pattern in patterns:
             keys.update(fnmatch.filter(self.tasks.keys(), pattern))
 
         return [self.tasks[k] for k in keys]
 
+    def to_python_project_template(self) -> str:
+        """Convert contents of this project into Python project file."""
+        return (
+            get_cssfinder_jinja2_environment()
+            .get_template(
+                "python_base_project.pyjinja2",
+            )
+            .render(project=self)
+        )
+
 
 class InvalidCSSFProjectContentError(ValueError):
     """Raised by load_from() when file content is not a dictionary."""
 
 
 class IncorrectFormatOfTaskFieldError(ValueError):
     """Raised when "tasks" field contains incorrectly specified tasks."""
@@ -302,24 +330,26 @@
         return self.project.project_file
 
     @property
     def project_directory(self) -> Path:
         """Path to directory containing `cssfproject.json` file."""
         if self._project is None:
             raise NotBoundToProjectError(
-                self, "Access to 'project_directory' property."
+                self,
+                "Access to 'project_directory' property.",
             )
         return self.project.project_directory
 
     @property
     def project_output_directory(self) -> Path:
         """Path to output directory for this project."""
         if self._project is None:
             raise NotBoundToProjectError(
-                self, "Access to 'project_output_directory' property."
+                self,
+                "Access to 'project_output_directory' property.",
             )
         return self.project.project_output_directory
 
     def bind(self, project: CSSFProject) -> None:
         """Bind object to specific CSSFProject."""
         self._project = project
 
@@ -328,15 +358,15 @@
     """Raised when unbound object is used in context requiring it to be bound to
     CSSFProject instance.
     """
 
     def __init__(self, ob: Any, context_msg: str) -> None:
         super().__init__(
             f"Attempted to use unbound object {ob} in context requiring it to be "
-            f"bound. ({context_msg})"
+            f"bound. ({context_msg})",
         )
 
 
 class Meta(CommonBaseModel, _ProjectFieldMixin):
     """Project meta information."""
 
     author: str
@@ -381,15 +411,16 @@
     """Name of task assigned to it in project."""
 
     @property
     def task_output_directory(self) -> Path:
         """Path to output directory of task."""
         if self._task_name is None:
             raise NotBoundToTaskError(
-                self, "Access to 'task_output_directory' property."
+                self,
+                "Access to 'task_output_directory' property.",
             )
         return self.project.project_output_directory / self.task_name
 
     @property
     def output_state_file(self) -> Path:
         """Path to output state file."""
         return self.task_output_directory / "state.mtx"
@@ -514,22 +545,26 @@
         self,
         project: CSSFProject,
         task_name: Optional[str] = None,
         task: Optional[Task] = None,
     ) -> None:
         """Evaluate dynamic path expressions."""
         super().bind(project, task_name, task)
-        assert isinstance(self.state, State)
+        if not isinstance(self.state, State):
+            msg = "State field must be of State type."
+            raise TypeError(msg)
 
         self.state.bind(project, task_name, task)
         self.get_resources().bind(project, task_name, task)
 
     def get_state(self) -> State:
         """Return initial state information."""
-        assert isinstance(self.state, State)
+        if not isinstance(self.state, State):
+            msg = "State field must be of State type."
+            raise TypeError(msg)
         return self.state
 
 
 class AlgoMode(CaseInsensitiveEnum):
     """Mode of algorithm."""
 
     # pylint: disable=invalid-name
@@ -614,21 +649,14 @@
 
         """
         super().bind(project, task_name, task)
 
         if task_name is None or task is None:
             return
 
-        self.file = (
-            Path(self.file.format(project=project, task_name=task_name, task=task))
-            .expanduser()
-            .resolve()
-            .as_posix()
-        )
-
     def is_predefined_dimensions(self) -> bool:
         """Return True when both dimensions are available."""
         return self.depth is not None and self.quantity is not None
 
     def get_depth(self) -> int:
         """Return system depth or raise NoDimensionsError if not specified in config."""
         if self.depth is None:
@@ -641,14 +669,32 @@
         config.
         """
         if self.quantity is None:
             msg = "quantity is not specified."
             raise NoDimensionsError(msg)
         return self.quantity
 
+    @property
+    def expanded_file(self) -> str:
+        """Return expanded path to file."""
+        if self._project is None:
+            raise NotBoundToProjectError(self, "Access to 'expanded_file' property.")
+        return (
+            Path(
+                self.file.format(
+                    project=self.project,
+                    task_name=self.task_name,
+                    task=self.task,
+                ),
+            )
+            .expanduser()
+            .resolve()
+            .as_posix()
+        )
+
 
 class NoDimensionsError(ValueError):
     """Raised when system dimensions were requested but are not specified in config."""
 
 
 class RuntimeCfg(CommonBaseModel):
     """Configuration of runtime limits and parameters influencing algorithm run time."""
@@ -722,15 +768,15 @@
             self.symmetries = [
                 [
                     Path(
                         sym.format(
                             project=project,
                             task_name=task_name,
                             task=task,
-                        )
+                        ),
                     )
                     .expanduser()
                     .resolve()
                     .as_posix()
                     for sym in row
                 ]
                 for row in self.symmetries
@@ -739,15 +785,15 @@
         if self.projection is not None:
             self.projection = (
                 Path(
                     self.projection.format(
                         project=project,
                         task_name=task_name,
                         task=task,
-                    )
+                    ),
                 )
                 .expanduser()
                 .resolve()
                 .as_posix()
             )
```

### Comparing `cssfinder-0.7.0/cssfinder/enums.py` & `cssfinder-0.8.0/cssfinder/enums.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/5qubits_json/5qubits_in.mtx` & `cssfinder-0.8.0/cssfinder/examples/5qubits_json/5qubits_in.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/5qubits_json/cssfproject.json` & `cssfinder-0.8.0/cssfinder/examples/5qubits_json/cssfproject.json`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/5qubits_py/5qubits_in.mtx` & `cssfinder-0.8.0/cssfinder/examples/5qubits_py/5qubits_in.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/5qubits_py/cssfproject.py` & `cssfinder-0.8.0/cssfinder/examples/5qubits_py/cssfproject.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,29 +28,28 @@
 
 """
 
 from __future__ import annotations
 
 from pathlib import Path
 
-from pydantic import EmailStr
-
 from cssfinder.api import run_project
 from cssfinder.cssfproject import (
     AlgoMode,
     BackendCfg,
     CSSFProject,
     GilbertCfg,
     Meta,
     Precision,
     RuntimeCfg,
     SemVerStr,
     State,
     Task,
 )
+from pydantic import EmailStr
 
 TASKS = [
     Task(
         gilbert=GilbertCfg(
             mode=AlgoMode.FSnQd,
             backend=BackendCfg(
                 name="numpy",
```

### Comparing `cssfinder-0.7.0/cssfinder/examples/GHZ3_json/GHZ3_in.mtx` & `cssfinder-0.8.0/cssfinder/examples/GHZ3_json/GHZ3_in.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/GHZ3_json/cssfproject.json` & `cssfinder-0.8.0/cssfinder/examples/GHZ3_json/cssfproject.json`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_1.mtx` & `cssfinder-0.8.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_1.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_3.mtx` & `cssfinder-0.8.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_3.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_5.mtx` & `cssfinder-0.8.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_5.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_7.mtx` & `cssfinder-0.8.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_7.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/GHZ4_json/GHZ4_in.mtx` & `cssfinder-0.8.0/cssfinder/examples/GHZ4_json/GHZ4_in.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/GHZ4_json/cssfproject.json` & `cssfinder-0.8.0/cssfinder/examples/GHZ4_json/cssfproject.json`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/SBiPa_json/cssfproject.json` & `cssfinder-0.8.0/cssfinder/examples/SBiPa_json/cssfproject.json`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/SBiPa_json/projection.mtx` & `cssfinder-0.8.0/cssfinder/examples/SBiPa_json/projection.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/SBiPa_json/state.mtx` & `cssfinder-0.8.0/cssfinder/examples/SBiPa_json/state.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/__init__.py` & `cssfinder-0.8.0/cssfinder/examples/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     e5qubits_py = "5qubits_py"
     GHZ3_json = "GHZ3_json"
     GHZ4_json = "GHZ4_json"
     SBiPa_json = "SBiPa_json"
     benchmark_32x32 = "benchmark_32x32"
     benchmark_64x64 = "benchmark_64x64"
 
-    def get_sha256(self) -> hashlib._Hash:  # noqa: SLF001
+    def get_sha256(self) -> hashlib._Hash:
         """Calculate and return SHA-256 of example project file."""
         source = self.get_project().project_file
         content = source.read_bytes()
         return hashlib.sha256(content)
 
     def get_project(self) -> CSSFProject:
         """Return project object from example."""
@@ -89,15 +89,15 @@
                     entry.value,
                     entry.get_sha256().hexdigest()[:8],
                     project.meta.author,
                     project.meta.version,
                     f"{len(project.tasks)}",
                     project.meta.description,
                 )
-            except FileNotFoundError:
+            except FileNotFoundError:  # noqa: PERF203
                 table.add_row(
                     entry.value,
                     "---",
                     "Broken",
                     "---",
                     "---",
                     "---",
```

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_32x32/5qubits_in.mtx` & `cssfinder-0.8.0/cssfinder/examples/benchmark_32x32/5qubits_in.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_32x32/cssfproject.py` & `cssfinder-0.8.0/cssfinder/examples/benchmark_32x32/cssfproject.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,44 +28,43 @@
 
 """
 
 from __future__ import annotations
 
 from pathlib import Path
 
-from pydantic import EmailStr
-
 from cssfinder.api import run_project
 from cssfinder.cssfproject import (
     AlgoMode,
     BackendCfg,
     CSSFProject,
     GilbertCfg,
     Meta,
     Precision,
     RuntimeCfg,
     SemVerStr,
     State,
     Task,
 )
+from pydantic import EmailStr
 
 TASKS = {}
 
 for backend in ["numpy_cython", "numpy", "numpy_jit", "rust_naive"]:
     for precision in [Precision.SINGLE, Precision.DOUBLE]:
         for i in range(64):
             TASKS[f"{backend}_{precision.value}_{i}"] = Task(
                 gilbert=GilbertCfg(
                     mode=AlgoMode.FSnQd,
                     backend=BackendCfg(
                         name=backend,
                         precision=precision,
                     ),
                     state=State(
-                        file=(Path(__file__).parent / "5qubits_in.mtx").as_posix()
+                        file=(Path(__file__).parent / "5qubits_in.mtx").as_posix(),
                     ),
                     runtime=RuntimeCfg(
                         visibility=0.4,
                         max_epochs=1000,
                         iters_per_epoch=1000,
                         max_corrections=1000,
                     ),
```

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/10_in.mtx` & `cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/10_in.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/cssfproject.py` & `cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/cssfproject.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,30 +28,29 @@
 
 """
 
 from __future__ import annotations
 
 from pathlib import Path
 
-from pydantic import EmailStr
-
 from cssfinder.api import run_project
 from cssfinder.cssfproject import (
     AlgoMode,
     BackendCfg,
     CSSFProject,
     GilbertCfg,
     Meta,
     Precision,
     Resources,
     RuntimeCfg,
     SemVerStr,
     State,
     Task,
 )
+from pydantic import EmailStr
 
 PROJECT_DIR = Path(__file__).parent
 PROJECT_SYMMETRIES = PROJECT_DIR / "symmetries"
 
 TASKS = {}
 
 for backend in ["numpy_cython", "numpy", "numpy_jit", "rust_naive"]:
@@ -81,15 +80,15 @@
                                 p.as_posix()
                                 for p in PROJECT_SYMMETRIES.glob("sym_sym_1_*.mtx")
                             ],
                             [
                                 p.as_posix()
                                 for p in PROJECT_SYMMETRIES.glob("sym_sym_2_*.mtx")
                             ],
-                        ]
+                        ],
                     ),
                 ),
             )
 
 
 __project__ = CSSFProject(
     meta=Meta(
```

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_0.mtx` & `cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_0.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_1.mtx` & `cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_1.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_2.mtx` & `cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_2.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_3.mtx` & `cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_3.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_4.mtx` & `cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_4.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_5.mtx` & `cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_5.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_6.mtx` & `cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_6.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_7.mtx` & `cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_7.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_0.mtx` & `cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_0.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_1.mtx` & `cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_1.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_2.mtx` & `cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_2.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_3.mtx` & `cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_3.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_4.mtx` & `cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_4.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_5.mtx` & `cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_5.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_6.mtx` & `cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_6.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_7.mtx` & `cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_7.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_0.mtx` & `cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_0.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_1.mtx` & `cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_1.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_2.mtx` & `cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_2.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_3.mtx` & `cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_3.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_4.mtx` & `cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_4.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_5.mtx` & `cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_5.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_6.mtx` & `cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_6.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_7.mtx` & `cssfinder-0.8.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_7.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/interactive.py` & `cssfinder-0.8.0/cssfinder/interactive.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,18 @@
 
 def create_new_project(
     default_author: Optional[str] = None,
     default_email: Optional[str] = None,
     default_name: Optional[str] = None,
     default_description: Optional[str] = None,
     default_version_string: Optional[str] = None,
-) -> None:
+    *,
+    no_interactive: bool,
+    override_existing: bool,
+) -> CSSFProject:
     """Create new project directory and cssfinder.json file."""
     all_set = (
         default_author is not None
         and default_email is not None
         and default_name is not None
         and default_description is not None
         and default_version_string is not None
@@ -64,15 +67,15 @@
 
     author = default_author or _load_default_name_from_git()
     email = default_email or _load_default_email_from_git()
     name = default_name or "new_project"
     description = default_description or " "
     version_string = default_version_string or "1.0.0"
 
-    if all_set:
+    if all_set or no_interactive:
         meta = Meta(
             author=author,
             email=EmailStr(email),
             name=name,
             description=description,
             version=SemVerStr(version_string),
         )
@@ -82,57 +85,63 @@
             email,
             name,
             description,
             version_string,
         )
 
     project_file_path = Path.cwd() / meta.name / "cssfproject.json"
-    if project_file_path.exists():
+    if (not override_existing) and project_file_path.exists():
         if (
             input("Project already exists, override? (y/n) ").casefold()
             == "Y".casefold()
         ):
             project_file_path.unlink()
         else:
             print("Aborted.")
             raise SystemExit(1)
 
     project_file_path.parent.mkdir(0o777, parents=True, exist_ok=True)
     project_file_path.touch(0o777, exist_ok=True)
 
-    project = CSSFProject(
+    return CSSFProject(
         meta=meta,
         tasks=[],
         project_path=project_file_path.as_posix(),
     )
-    serialized = project.json(indent=4, ensure_ascii=False)
-    project_file_path.write_text(serialized)
 
 
 def _load_default_name_from_git() -> str:
     # Retrieve default from system name just in case, but git usually contains
     # better value.
     default_name = getpass.getuser()
 
     try:
-        retval = subprocess.run(["git", "config", "user.name"], capture_output=True)
+        retval = subprocess.run(
+            ["git", "config", "user.name"],
+            capture_output=True,
+            check=False,
+        )
         if retval.returncode == 0:
             default_name = retval.stdout.decode("utf-8").strip()
 
     except (FileNotFoundError, ValueError):
         pass
 
     return default_name
 
 
 def _load_default_email_from_git() -> EmailStr:
     default_email = EmailStr("unknown@unknown.com")
 
     try:
-        retval = subprocess.run(["git", "config", "user.email"], capture_output=True)
+        retval = subprocess.run(
+            ["git", "config", "user.email"],
+            capture_output=True,
+            check=False,
+        )
         if retval.returncode == 0:
             default_email = EmailStr(retval.stdout.decode("utf-8").strip())
 
     except (FileNotFoundError, ValueError, ValidationError):
         pass
 
     return default_email
@@ -172,15 +181,15 @@
                 description=default_project_description,
                 version=SemVerStr(default_project_version),
             )
         except ValidationError as e:
             message = f"[210 bold]{e}"
 
 
-def _get_project_fields_with_pytermgui(  # noqa: PLR0913
+def _get_project_fields_with_pytermgui(
     default_author_name: str,
     default_author_email: str,
     default_project_name: str,
     default_project_description: str,
     default_project_version: str,
     message: str,
 ) -> tuple[str, str, str, str, str]:
@@ -278,26 +287,35 @@
             ),
         )
 
 
 def add_task_gilbert(
     project: CSSFProject,
     spec: GilbertTaskSpec,
+    *,
+    no_interactive: bool,
+    override_existing: bool,
 ) -> None:
     """Add task to project and save it in place."""
     while True:
         try:
             task = spec.to_task()
             break
 
         except (ValueError, TypeError, ValidationError, KeyError):
+            if no_interactive:
+                raise
             spec = get_gilbert_task_fields_with_pytermgui(spec)
 
-    if spec.name in project.tasks and (
-        input("Task already exists, override? (y/n) ").casefold() != "Y".casefold()
+    if (
+        override_existing is False
+        and spec.name in project.tasks
+        and (
+            input("Task already exists, override? (y/n) ").casefold() != "Y".casefold()
+        )
     ):
         print("Aborted.")
         raise SystemExit(1)
 
     project.tasks[spec.name] = task
     project.project_file.write_text(project.json(indent=4, ensure_ascii=False))
 
@@ -317,15 +335,16 @@
             extend(ptg.break_line(line.replace("\n", "\\n"), width, fill=" "))
             extend("")
 
         return lines
 
 
 def get_gilbert_task_fields_with_pytermgui(
-    spec: GilbertTaskSpec, message: Optional[str] = None
+    spec: GilbertTaskSpec,
+    message: Optional[str] = None,
 ) -> GilbertTaskSpec:
     """Create temporary TUI prompt for entering task configuration."""
     is_interrupted: bool = True
     df_state = "{project.project_directory}/state.mtx"
 
     with ptg.WindowManager() as manager:
```

### Comparing `cssfinder-0.7.0/cssfinder/io/__init__.py` & `cssfinder-0.8.0/cssfinder/io/__init__.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/io/gilbert_io.py` & `cssfinder-0.8.0/cssfinder/io/gilbert_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,16 @@
 NUMBER_OF_DIMENSIONS_IN_MATRIX: int = 2
 
 
 class GilbertIO:
     """Loader of Gilbert algorithm assets."""
 
     def __init__(
-        self, matrix_format: MatrixFormat = MatrixFormat.MATRIX_MARKET
+        self,
+        matrix_format: MatrixFormat = MatrixFormat.MATRIX_MARKET,
     ) -> None:
         self.loader = MatrixIO.new(matrix_format)
 
     def load_state(self, source: str | Path) -> npt.NDArray[np.complex128]:
         """Load state matrix from file.
 
         Parameters
@@ -59,15 +60,17 @@
         -------
         npt.NDArray[np.complex128]
             Loaded matrix. Always returns np.complex128.
 
         """
         mtx = self.loader.load(source).astype(np.complex128)
         logging.info(
-            "Loaded matrix from %r of shape %r", Path(source).as_posix(), mtx.shape
+            "Loaded matrix from %r of shape %r",
+            Path(source).as_posix(),
+            mtx.shape,
         )
 
         # We are expecting loaded ndarray to be a square matrix, all other numbers of
         # dimensions cause crash.
         self._check_matrix_shape(mtx)
 
         return mtx
```

### Comparing `cssfinder-0.7.0/cssfinder/io/matrix.py` & `cssfinder-0.8.0/cssfinder/io/matrix.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,26 +66,28 @@
 
         """
         io = FORMAT_TO_LOADER[matrix_format]()
         logging.debug("Selected matrix IO %r for format %r", io, matrix_format.name)
         return io
 
     def load(
-        self, src: str | Path | IO[bytes]
+        self,
+        src: str | Path | IO[bytes],
     ) -> npt.NDArray[np.int64 | np.float64 | np.complex128]:
         """Load matrix from file as numpy array."""
         if isinstance(src, (str, Path)):
             with Path(src).open("rb") as file:
                 return self._load(file)
 
         return self._load(file)
 
     @abstractmethod
     def _load(
-        self, src: IO[bytes]
+        self,
+        src: IO[bytes],
     ) -> npt.NDArray[np.int64 | np.float64 | np.complex128]:
         ...
 
     def dump(
         self,
         data: npt.NDArray[np.int64 | np.float64 | np.complex128],
         dest: str | Path | IO[bytes],
@@ -97,33 +99,39 @@
             with file_path.open("wb") as file:
                 return self._dump(data, file)
 
         return self._dump(data, file)
 
     @abstractmethod
     def _dump(
-        self, data: npt.NDArray[np.int64 | np.float64 | np.complex128], dest: IO[bytes]
+        self,
+        data: npt.NDArray[np.int64 | np.float64 | np.complex128],
+        dest: IO[bytes],
     ) -> None:
         ...
 
 
 class MatrixMarketIO(MatrixIO):
     """MatrixIO implementation for loading MatrixMarket exchange format files."""
 
     matrix_format: ClassVar[MatrixFormat] = MatrixFormat.MATRIX_MARKET
 
     def _load(
-        self, dest: IO[bytes]
+        self,
+        dest: IO[bytes],
     ) -> npt.NDArray[np.int64 | np.float64 | np.complex128]:
         mtx = scipy.io.mmread(dest)
-        assert mtx is not None
+        if mtx is None:
+            raise TypeError
         return np.array(mtx)
 
     def _dump(
-        self, data: npt.NDArray[np.int64 | np.float64 | np.complex128], dest: IO[bytes]
+        self,
+        data: npt.NDArray[np.int64 | np.float64 | np.complex128],
+        dest: IO[bytes],
     ) -> None:
         scipy.io.mmwrite(
             dest,
             data,
             comment=f"Created with CSSFinder {cssfinder.__version__}.",
         )
```

### Comparing `cssfinder-0.7.0/cssfinder/log.py` & `cssfinder-0.8.0/cssfinder/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     Methods
     -------
     format(record: logging.LogRecord) -> str:
         Return a formatted and stripped version of the log message.
 
     """
 
-    def format(self, record: LogRecord) -> str:  # noqa: A003
+    def format(self, record: LogRecord) -> str:
         """Return the formatted string of a log record after stripping all formatting
         tags.
 
         _extended_summary_
 
         Parameters
         ----------
@@ -299,22 +299,24 @@
     from cssfinder.api import run_project
 
     def run_project_wrapper(
         project: CSSFProject,
         tasks: list[str] | None = None,
         *,
         is_debug: bool = False,
+        is_rich: bool = True,
         force_sequential: bool = False,
         max_parallel: int = -1,
     ) -> list[Task]:
         start_time = time.perf_counter()
         task_list = run_project(
             project,
             tasks,
             is_debug=is_debug,
+            is_rich=is_rich,
             force_sequential=force_sequential,
             max_parallel=max_parallel,
         )
         end_time = time.perf_counter()
         execution_time = end_time - start_time
 
         perf_file = Path.cwd() / f"perf_{project.meta.name}.json"
```

### Comparing `cssfinder-0.7.0/cssfinder/reports/__init__.py` & `cssfinder-0.8.0/cssfinder/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/reports/archive.py` & `cssfinder-0.8.0/cssfinder/reports/archive.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/reports/html.py` & `cssfinder-0.8.0/cssfinder/reports/json.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,37 +18,29 @@
 # CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE
 # OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 """HTML document based report renderer."""
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
-
-import jinja2
+import json
 
 from cssfinder.reports.renderer import Renderer, Report, ReportType
 
-if TYPE_CHECKING:
-    from cssfinder.cssfproject import Task
-    from cssfinder.reports.math import SlopeProperties
-    from cssfinder.reports.plotting import Plot
-
 
-class HTMLRenderer(Renderer):
+class JSONRenderer(Renderer):
     """Renderer implementation outputting HTML files content."""
 
-    def __init__(self, props: SlopeProperties, plots: list[Plot], task: Task) -> None:
-        super().__init__(props, plots, task)
-        self.env = jinja2.Environment(
-            loader=jinja2.PackageLoader("cssfinder"),
-            autoescape=jinja2.select_autoescape(),
-        )
-
     def render(self) -> Report:
         """Generate report content."""
-        template = self.env.get_template("report.html.jinja2")
         return Report(
-            template.render(ctx=self.ctx).encode("utf-8"),
-            ReportType.HTML,
-            self.ctx.task.task_output_directory / "report.html",
+            json.dumps(
+                {
+                    "title": self.ctx.title,
+                    "meta": self.ctx.meta,
+                    "math": self.ctx.math_props,
+                },
+                indent=4,
+            ).encode("utf-8"),
+            ReportType.JSON,
+            self.ctx.task.task_output_directory / "report.json",
         )
```

### Comparing `cssfinder-0.7.0/cssfinder/reports/json.py` & `cssfinder-0.8.0/cssfinder/reports/txt.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,33 +14,10 @@
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
 # INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
 # PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
 # HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
 # CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE
 # OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-"""HTML document based report renderer."""
+"""Text based report renderer."""
 
 from __future__ import annotations
-
-import json
-
-from cssfinder.reports.renderer import Renderer, Report, ReportType
-
-
-class JSONRenderer(Renderer):
-    """Renderer implementation outputting HTML files content."""
-
-    def render(self) -> Report:
-        """Generate report content."""
-        return Report(
-            json.dumps(
-                {
-                    "title": self.ctx.title,
-                    "meta": self.ctx.meta,
-                    "math": self.ctx.math_props,
-                },
-                indent=4,
-            ).encode("utf-8"),
-            ReportType.JSON,
-            self.ctx.task.task_output_directory / "report.json",
-        )
```

### Comparing `cssfinder-0.7.0/cssfinder/reports/manager.py` & `cssfinder-0.8.0/cssfinder/reports/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,19 @@
         plotter = Plotter(corrections)
 
         plots["decay"] = plotter.plot_corrections()
         plots["inverse_decay"] = plotter.plot_corrections_inverse()
         plots["iterations"] = plotter.plot_iteration()
 
         return PreparedReportManager(
-            self.project, plotter.slope_props, plots, self.task, corrections
+            self.project,
+            plotter.slope_props,
+            plots,
+            self.task,
+            corrections,
         )
 
 
 @dataclass
 class PreparedReportManager:
     """Report manager with calculated report values."""
 
@@ -93,15 +97,17 @@
     task: Task
     corrections: pd.DataFrame
 
     RENDERERS: ClassVar[dict[ReportType, Type[Renderer]]] = {}
 
     @classmethod
     def register_renderer(
-        cls, renderer_cls: Type[Renderer], report_type: ReportType
+        cls,
+        renderer_cls: Type[Renderer],
+        report_type: ReportType,
     ) -> None:
         """Register renderer for report type."""
         cls.RENDERERS[report_type] = renderer_cls
 
     def request_report(self, report_type: ReportType | Any) -> Report:
         """Generate report."""
         renderer_cls = self.RENDERERS.get(report_type)
```

### Comparing `cssfinder-0.7.0/cssfinder/reports/math.py` & `cssfinder-0.8.0/cssfinder/reports/math.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,31 +243,29 @@
 
     Returns
     -------
     numpy.float64
         The optimum correction value for the input array of values.
 
     """
-    values = values
     upper_half = values[len(values) // 2 :]
 
     optimum = upper_half[-1] - 1e-6
     step1 = optimum / 10000
 
     while R(upper_half, optimum - step1) > R(upper_half, optimum) and optimum > 0:
         optimum = optimum - step1
 
     return optimum  # type: ignore[no-any-return]
 
 
 @lru_cache(16)
 def _r_indexes(length: int) -> npt.NDArray[np.float64]:
     indexes = np.arange(length)
-    difference = np.mean(np.square(indexes)) - np.square(np.mean(indexes))
-    return difference  # type: ignore[no-any-return]
+    return np.mean(np.square(indexes)) - np.square(np.mean(indexes))  # type: ignore[no-any-return]
 
 
 @lru_cache(16)
 def _indexes(length: int) -> npt.NDArray[np.float64]:
     return np.arange(length, dtype=np.float64)
```

### Comparing `cssfinder-0.7.0/cssfinder/reports/pdf.py` & `cssfinder-0.8.0/cssfinder/reports/pdf.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.7.0/cssfinder/reports/plotting.py` & `cssfinder-0.8.0/cssfinder/reports/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,17 @@
 
         """
         if axes is None:
             plt.figure()
             axes = plt.subplot()
 
         axes.plot(
-            self.corrections[["index"]], self.corrections[["value"]], label="correction"
+            self.corrections[["index"]],
+            self.corrections[["value"]],
+            label="correction",
         )
         axes.hlines(
             [self.slope_props.optimum],
             xmin=-10,
             xmax=self.corrections[["index"]].max(),
             color="red",
             label="H-S distance",
```

### Comparing `cssfinder-0.7.0/cssfinder/reports/renderer.py` & `cssfinder-0.8.0/cssfinder/reports/renderer.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,29 +89,29 @@
             {
                 "Project name": self.task.project.meta.name,
                 "Task name": self.task.task_name,
                 "Author": self.task.project.meta.author,
                 "Email": self.task.project.meta.email,
                 "Description": self.task.project.meta.description,
                 "Version": self.task.project.meta.version,
-            }
+            },
         )
 
     @property
     def math_props(self) -> OrderedDict:
         """Return mathematical properties."""
         return OrderedDict(
             {
                 "Correction count": f"{self.props.correction_count}",
                 "Hilbert-Schmidt distance": f"{self.props.optimum:.3f}",
                 "Sample correlation coefficient": f"{self.props.r_value:.3f}",
                 "Offset (optimum)": f"{self.props.optimum:.3f}",
                 "Trend (aa1)": f"{self.props.aa1:.3f}",
                 "Exp Offset (bb1)": f"{self.props.bb1:.3f}",
-            }
+            },
         )
 
 
 @dataclass
 class Report:
     """Container for rendered report."""
 
@@ -146,9 +146,9 @@
 
 class DefaultDestinationNotSpecifiedError(Exception):
     """Raised when save_default() was called on Report object with no default_dest."""
 
     def __init__(self, report_type: ReportType) -> None:
         super().__init__(
             f"Default destination for report object of type {report_type.name!r} "
-            "was not specified."
+            "was not specified.",
         )
```

### Comparing `cssfinder-0.7.0/cssfinder/templates/report.html.jinja2` & `cssfinder-0.8.0/cssfinder/templates/report.html.jinja2`

 * *Files identical despite different names*

