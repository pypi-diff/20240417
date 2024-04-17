# Comparing `tmp/qbraid-0.6.1.tar.gz` & `tmp/qbraid-0.7.0.dev20240417171913.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid-0.6.1.tar", last modified: Wed Apr 10 00:39:54 2024, max compression
+gzip compressed data, was "qbraid-0.7.0.dev20240417171913.tar", last modified: Wed Apr 17 17:19:16 2024, max compression
```

## Comparing `qbraid-0.6.1.tar` & `qbraid-0.7.0.dev20240417171913.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.729268 qbraid-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-10 00:39:49.000000 qbraid-0.6.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-10 00:39:49.000000 qbraid-0.6.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-10 00:39:49.000000 qbraid-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-10 00:39:49.000000 qbraid-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    55209 2024-04-10 00:39:54.729268 qbraid-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-04-10 00:39:49.000000 qbraid-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.701268 qbraid-0.6.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.701268 qbraid-0.6.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.701268 qbraid-0.6.1/docs/_static/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/cards/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/cards/python.png
--rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/cards/terminal.png
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.701268 qbraid-0.6.1/docs/_static/pkg-logos/
--rw-r--r--   0 runner    (1001) docker     (127)    36600 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/pkg-logos/braket.png
--rw-r--r--   0 runner    (1001) docker     (127)    53519 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/pkg-logos/cirq.png
--rw-r--r--   0 runner    (1001) docker     (127)    26788 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/pkg-logos/pennylane.png
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/pkg-logos/pyquil.png
--rw-r--r--   0 runner    (1001) docker     (127)   125852 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/pkg-logos/qasm.png
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/pkg-logos/qir.png
--rw-r--r--   0 runner    (1001) docker     (127)    13073 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/pkg-logos/qiskit.png
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/pkg-logos/quantinuum.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.705268 qbraid-0.6.1/docs/_static/sdk-files/
--rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/sdk-files/batch_counts.png
--rw-r--r--   0 runner    (1001) docker     (127)    35963 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/sdk-files/conversion_graph.png
--rw-r--r--   0 runner    (1001) docker     (127)   447304 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/sdk-files/get_devices.png
--rw-r--r--   0 runner    (1001) docker     (127)   180765 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/sdk-files/hub_spokes.png
--rw-r--r--   0 runner    (1001) docker     (127)   707295 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/sdk-files/lab_jobs.png
--rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/_static/sdk-files/plot_counts.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.705268 qbraid-0.6.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/api/qbraid.compiler.rst
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/api/qbraid.interface.rst
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/api/qbraid.programs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/api/qbraid.providers.rst
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/api/qbraid.rst
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/api/qbraid.transpiler.rst
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/api/qbraid.visualization.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.709268 qbraid-0.6.1/docs/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/sdk/devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/sdk/jobs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/sdk/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/sdk/programs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/sdk/providers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/sdk/results.rst
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-10 00:39:49.000000 qbraid-0.6.1/docs/sdk/transpiler.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-04-10 00:39:49.000000 qbraid-0.6.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.709268 qbraid-0.6.1/qbraid/
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/_about.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/_import.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.709268 qbraid-0.6.1/qbraid/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.709268 qbraid-0.6.1/qbraid/compiler/braket/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/compiler/braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/compiler/braket/ionq.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/compiler/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/get_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/get_jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.709268 qbraid-0.6.1/qbraid/interface/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/interface/circuit_equality.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.713268 qbraid-0.6.1/qbraid/interface/random/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/interface/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/interface/random/cirq_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/interface/random/qasm3_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/interface/random/qiskit_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/interface/random/random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.713268 qbraid-0.6.1/qbraid/programs/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/abc_program.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.713268 qbraid-0.6.1/qbraid/programs/libs/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/libs/braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/libs/cirq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/libs/pennylane.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/libs/pyquil.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/libs/pytket.py
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/libs/qasm2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/libs/qasm3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/libs/qiskit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/qasm_passes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/programs/qasm_qelib1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.717268 qbraid-0.6.1/qbraid/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/_import.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.717268 qbraid-0.6.1/qbraid/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/aws/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/aws/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/aws/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/aws/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/aws/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    19188 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.717268 qbraid-0.6.1/qbraid/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/ibm/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/ibm/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/ibm/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/ibm/result.py
--rw-r--r--   0 runner    (1001) docker     (127)    10095 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/providers/status_maps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.717268 qbraid-0.6.1/qbraid/transpiler/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.717268 qbraid-0.6.1/qbraid/transpiler/conversions/
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.721268 qbraid-0.6.1/qbraid/transpiler/conversions/braket/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/braket/cirq_from_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)    13215 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/braket/cirq_to_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/braket/conversions_cirq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/braket/conversions_qasm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/braket/custom_instr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.721268 qbraid-0.6.1/qbraid/transpiler/conversions/cirq/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/cirq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23224 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/cirq/cirq_qasm_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/cirq/conversions_qasm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/cirq/custom_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.721268 qbraid-0.6.1/qbraid/transpiler/conversions/openqasm3/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/openqasm3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/openqasm3/conversions_qasm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.721268 qbraid-0.6.1/qbraid/transpiler/conversions/pennylane/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/pennylane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/pennylane/conversions_qasm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.721268 qbraid-0.6.1/qbraid/transpiler/conversions/pyquil/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/pyquil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10806 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/pyquil/cirq_quil_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    21811 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/pyquil/cirq_quil_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/pyquil/conversions_cirq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.721268 qbraid-0.6.1/qbraid/transpiler/conversions/pytket/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/pytket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/pytket/conversions_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/pytket/conversions_qasm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.721268 qbraid-0.6.1/qbraid/transpiler/conversions/qiskit/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/qiskit/conversions_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/conversions/qiskit/conversions_qasm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/transpiler/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.725268 qbraid-0.6.1/qbraid/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/visualization/draw_circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/visualization/draw_qasm3.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/visualization/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/visualization/plot_conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10107 2024-04-10 00:39:49.000000 qbraid-0.6.1/qbraid/visualization/plot_counts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.725268 qbraid-0.6.1/qbraid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    55209 2024-04-10 00:39:54.000000 qbraid-0.6.1/qbraid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-10 00:39:54.000000 qbraid-0.6.1/qbraid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 00:39:54.000000 qbraid-0.6.1/qbraid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-10 00:39:54.000000 qbraid-0.6.1/qbraid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-10 00:39:54.000000 qbraid-0.6.1/qbraid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 00:39:54.000000 qbraid-0.6.1/qbraid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-10 00:39:49.000000 qbraid-0.6.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-10 00:39:49.000000 qbraid-0.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 00:39:54.729268 qbraid-0.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:39:54.725268 qbraid-0.6.1/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-10 00:39:49.000000 qbraid-0.6.1/tools/set_provider_configs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4480 2024-04-10 00:39:49.000000 qbraid-0.6.1/tools/verify_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-10 00:39:49.000000 qbraid-0.6.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.055361 qbraid-0.7.0.dev20240417171913/
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    55229 2024-04-17 17:19:16.055361 qbraid-0.7.0.dev20240417171913/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11630 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.023361 qbraid-0.7.0.dev20240417171913/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.023361 qbraid-0.7.0.dev20240417171913/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.023361 qbraid-0.7.0.dev20240417171913/docs/_static/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/cards/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/cards/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/cards/terminal.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.027361 qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/
+-rw-r--r--   0 runner    (1001) docker     (127)    36600 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/braket.png
+-rw-r--r--   0 runner    (1001) docker     (127)    53519 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/cirq.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26788 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/pennylane.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/pyquil.png
+-rw-r--r--   0 runner    (1001) docker     (127)   125852 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/qasm.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/qir.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13073 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/qiskit.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/quantinuum.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.027361 qbraid-0.7.0.dev20240417171913/docs/_static/sdk-files/
+-rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/sdk-files/batch_counts.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35963 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/sdk-files/conversion_graph.png
+-rw-r--r--   0 runner    (1001) docker     (127)   447304 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/sdk-files/get_devices.png
+-rw-r--r--   0 runner    (1001) docker     (127)   180765 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/sdk-files/hub_spokes.png
+-rw-r--r--   0 runner    (1001) docker     (127)   707295 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/sdk-files/lab_jobs.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/_static/sdk-files/plot_counts.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.031361 qbraid-0.7.0.dev20240417171913/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/api/qbraid.interface.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/api/qbraid.programs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/api/qbraid.providers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/api/qbraid.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/api/qbraid.transforms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/api/qbraid.transpiler.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/api/qbraid.visualization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.031361 qbraid-0.7.0.dev20240417171913/docs/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/sdk/devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/sdk/jobs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/sdk/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/sdk/programs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/sdk/providers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/sdk/results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/docs/sdk/transpiler.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.031361 qbraid-0.7.0.dev20240417171913/qbraid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/_about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-17 17:19:13.000000 qbraid-0.7.0.dev20240417171913/qbraid/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/get_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/get_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.035361 qbraid-0.7.0.dev20240417171913/qbraid/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/interface/circuit_equality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.035361 qbraid-0.7.0.dev20240417171913/qbraid/interface/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/interface/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/interface/random/cirq_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/interface/random/qasm3_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/interface/random/qiskit_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/interface/random/random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.035361 qbraid-0.7.0.dev20240417171913/qbraid/programs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/abc_program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.039361 qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/cirq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/pennylane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/pyquil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/pytket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/qasm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/qasm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/qasm_passes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/programs/qasm_qelib1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.039361 qbraid-0.7.0.dev20240417171913/qbraid/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.039361 qbraid-0.7.0.dev20240417171913/qbraid/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/aws/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/aws/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/aws/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/aws/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/aws/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18460 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.043361 qbraid-0.7.0.dev20240417171913/qbraid/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/ibm/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/ibm/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/ibm/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/ibm/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10095 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/providers/status_maps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.043361 qbraid-0.7.0.dev20240417171913/qbraid/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transforms/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.043361 qbraid-0.7.0.dev20240417171913/qbraid/transforms/pytket/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transforms/pytket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transforms/pytket/ionq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.043361 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.043361 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.043361 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/braket/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/braket/cirq_from_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13215 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/braket/cirq_to_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/braket/conversions_cirq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/braket/conversions_qasm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/braket/custom_instr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.047361 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/cirq/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/cirq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23224 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/cirq/cirq_qasm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/cirq/conversions_qasm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/cirq/custom_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.047361 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/openqasm3/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/openqasm3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/openqasm3/conversions_qasm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.047361 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pennylane/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pennylane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pennylane/conversions_qasm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.047361 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pyquil/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pyquil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10806 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pyquil/cirq_quil_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21811 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pyquil/cirq_quil_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pyquil/conversions_cirq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.047361 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pytket/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pytket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pytket/conversions_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pytket/conversions_qasm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.047361 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/qiskit/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/qiskit/conversions_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/qiskit/conversions_qasm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/transpiler/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.051361 qbraid-0.7.0.dev20240417171913/qbraid/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/visualization/draw_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/visualization/draw_qasm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/visualization/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/visualization/plot_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10107 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/qbraid/visualization/plot_counts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.051361 qbraid-0.7.0.dev20240417171913/qbraid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    55229 2024-04-17 17:19:15.000000 qbraid-0.7.0.dev20240417171913/qbraid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-17 17:19:16.000000 qbraid-0.7.0.dev20240417171913/qbraid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 17:19:15.000000 qbraid-0.7.0.dev20240417171913/qbraid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-17 17:19:15.000000 qbraid-0.7.0.dev20240417171913/qbraid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-17 17:19:15.000000 qbraid-0.7.0.dev20240417171913/qbraid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 17:19:15.000000 qbraid-0.7.0.dev20240417171913/qbraid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 17:19:16.055361 qbraid-0.7.0.dev20240417171913/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:19:16.051361 qbraid-0.7.0.dev20240417171913/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/tools/set_provider_configs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4480 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/tools/verify_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-17 17:19:05.000000 qbraid-0.7.0.dev20240417171913/tox.ini
```

### Comparing `qbraid-0.6.1/CODE_OF_CONDUCT.md` & `qbraid-0.7.0.dev20240417171913/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/CONTRIBUTING.md` & `qbraid-0.7.0.dev20240417171913/CONTRIBUTING.md`

 * *Files 5% similar despite different names*

```diff
@@ -13,49 +13,49 @@
 3. `tox -e format-check`: Code passes linters and formatters checks. Any exceptions or updates to code style configs are documented.
 4. `python tools/verify_headers.py`: New files have appropriate licensing headers. Running headers script passes checks.
 
 ## Installing from source
 
 You can install the qBraid-SDK from source by cloning this repository and running a pip install command in the root directory:
 
-```bash
+```shell
 git clone https://github.com/qbraid/qBraid.git
 cd qBraid
-pip install -e '.[all]' # install all extensions
+pip install -e .
 ```
 
 ## Documentation
 
 To generate the API reference documentation locally:
 
-```bash
+```shell
 pip install 'tox>=4.2'
 tox -e docs
 ```
 
 Alternatively:
 
-```bash
+```shell
 pip install -e '.[docs]'
 cd docs
 make html
 ```
 
 Both methods will run Sphinx in your shell. If the build results in an `InvocationError` due to a 
 duplicate object description, try `rm docs/stubs/*` to empty the old stubs directory, and then 
 re-start the build. If the build succeeds, it will say `The HTML pages are in build/html`. You can 
 view the generated documentation in your browser (on OS X) using:
 
-```bash
+```shell
 open build/html/index.html
 ```
 
 You can also view it by running a web server in that directory:
 
-```bash
+```shell
 cd build/html
 python3 -m http.server
 ```
 
 Then open your browser to `http://localhost:8000`. If you make changes to the docs that aren't
 reflected in subsequent builds, run `make clean html`, which will force a full rebuild.
 
@@ -70,39 +70,39 @@
 so to add relative links, in-line markup, bulleted lists, code-blocks, or do other types of formatting inside of docstrings, use
 the `reST` syntax mentioned (linked) above.
 
 ## Testing
 
 To run all unit tests:
 
-```bash
+```shell
 pip install 'tox>=4.2'
 tox -e unit-tests
 ```
 
 You can also pass in various pytest arguments to run selected tests:
 
-```bash
+```shell
 tox -e unit-tests -- {your-arguments}
 ```
 
 Alternatively:
 
-```bash
+```shell
 pip install pytest
 pytest {path-to-test}
 ```
 
 Running unit tests with tox will automatically generate a coverage report, which can be viewed by
 opening `tests/_coverage/index.html` in your browser. The latest code coverage report generated
 from the `main` branch can be viewed at https://app.codecov.io/gh/qBraid/qBraid/tree/main.
 
 To run linters and doc generators and unit tests:
 
-```bash
+```shell
 tox
 ```
 
 ## Code Style
 
 For code style, our project uses a combination of [isort](https://github.com/PyCQA/isort), [pylint](https://github.com/pylint-dev/pylint),
 and [black](https://github.com/psf/black). Each of these tools is setup with its own default configuration specific to this project in `pyproject.toml`.
```

### Comparing `qbraid-0.6.1/LICENSE` & `qbraid-0.7.0.dev20240417171913/LICENSE`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/PKG-INFO` & `qbraid-0.7.0.dev20240417171913/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid
-Version: 0.6.1
+Version: 0.7.0.dev20240417171913
 Summary: A Python toolkit for cross-framework abstraction of quantum programs.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -699,17 +699,17 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: networkx<4.0,>=2.5
 Requires-Dist: numpy<1.27,>=1.17
 Requires-Dist: openqasm3[parser]<0.6.0,>=0.4.0
 Requires-Dist: ply>=3.6
-Requires-Dist: qbraid-core<0.2.0,>=0.1.1
+Requires-Dist: qbraid-core<0.2.0,>=0.1.3
 Provides-Extra: braket
-Requires-Dist: amazon-braket-sdk<1.77.0,>=1.42.1; extra == "braket"
+Requires-Dist: amazon-braket-sdk<1.78.0,>=1.42.1; extra == "braket"
 Provides-Extra: cirq
 Requires-Dist: cirq-core<1.4.0,>=1.3.0; extra == "cirq"
 Provides-Extra: pennylane
 Requires-Dist: pennylane<0.36.0,>=0.33.1; extra == "pennylane"
 Provides-Extra: pytket
 Requires-Dist: pytket<1.27.0,>=1.16.0; extra == "pytket"
 Provides-Extra: pyquil
@@ -736,15 +736,15 @@
 Requires-Dist: black; extra == "lint"
 Requires-Dist: isort; extra == "lint"
 Requires-Dist: pylint; extra == "lint"
 Provides-Extra: docs
 Requires-Dist: sphinx~=7.2.6; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints<2.1,>=1.24; extra == "docs"
 Requires-Dist: sphinx-rtd-theme<2.1,>=1.3; extra == "docs"
-Requires-Dist: docutils<0.21; extra == "docs"
+Requires-Dist: docutils<0.22; extra == "docs"
 
 <img width=full alt="qbraid-sdk-header" src="https://user-images.githubusercontent.com/46977852/224456452-605e51f2-193d-4789-863e-e51cdd4b0a54.png">
 
 <p align="center">
   <a href="https://github.com/qBraid/qBraid/actions/workflows/main.yml">
     <img src="https://github.com/qBraid/qBraid/actions/workflows/main.yml/badge.svg?branch=main" alt="CI"/>
   </a>
@@ -795,21 +795,21 @@
 
 Using the SDK on [qBraid Lab](https://docs.qbraid.com/projects/lab/en/latest/lab/overview.html) means direct, pre-configured access to QPUs from IonQ, Oxford Quantum Circuits, QuEra, and Rigetti, as well as on-demand simulators from AWS, all with no additional access keys or API tokens required. See [qBraid Quantum Jobs](https://docs.qbraid.com/projects/lab/en/latest/lab/quantum_jobs.html) for more.
 
 ### Local install
 
 The qBraid-SDK, and all of its dependencies, can also be installed using pip:
 
-```bash
+```shell
 pip install qbraid
 ```
 
 You can also [install from source](CONTRIBUTING.md#installing-from-source) by cloning this repository and running a pip install command in the root directory of the repository:
 
-```bash
+```shell
 git clone https://github.com/qBraid/qBraid.git
 cd qBraid
 pip install .
 ```
 
 *Note*: The qBraid-SDK requires Python 3.9 or greater.
```

### Comparing `qbraid-0.6.1/README.md` & `qbraid-0.7.0.dev20240417171913/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -51,21 +51,21 @@
 
 Using the SDK on [qBraid Lab](https://docs.qbraid.com/projects/lab/en/latest/lab/overview.html) means direct, pre-configured access to QPUs from IonQ, Oxford Quantum Circuits, QuEra, and Rigetti, as well as on-demand simulators from AWS, all with no additional access keys or API tokens required. See [qBraid Quantum Jobs](https://docs.qbraid.com/projects/lab/en/latest/lab/quantum_jobs.html) for more.
 
 ### Local install
 
 The qBraid-SDK, and all of its dependencies, can also be installed using pip:
 
-```bash
+```shell
 pip install qbraid
 ```
 
 You can also [install from source](CONTRIBUTING.md#installing-from-source) by cloning this repository and running a pip install command in the root directory of the repository:
 
-```bash
+```shell
 git clone https://github.com/qBraid/qBraid.git
 cd qBraid
 pip install .
 ```
 
 *Note*: The qBraid-SDK requires Python 3.9 or greater.
```

#### html2text {}

```diff
@@ -17,18 +17,18 @@
 docs.qbraid.com/projects/lab/en/latest/lab/environments.html#install-
 environment). Using the SDK on [qBraid Lab](https://docs.qbraid.com/projects/
 lab/en/latest/lab/overview.html) means direct, pre-configured access to QPUs
 from IonQ, Oxford Quantum Circuits, QuEra, and Rigetti, as well as on-demand
 simulators from AWS, all with no additional access keys or API tokens required.
 See [qBraid Quantum Jobs](https://docs.qbraid.com/projects/lab/en/latest/lab/
 quantum_jobs.html) for more. ### Local install The qBraid-SDK, and all of its
-dependencies, can also be installed using pip: ```bash pip install qbraid ```
+dependencies, can also be installed using pip: ```shell pip install qbraid ```
 You can also [install from source](CONTRIBUTING.md#installing-from-source) by
 cloning this repository and running a pip install command in the root directory
-of the repository: ```bash git clone https://github.com/qBraid/qBraid.git cd
+of the repository: ```shell git clone https://github.com/qBraid/qBraid.git cd
 qBraid pip install . ``` *Note*: The qBraid-SDK requires Python 3.9 or greater.
 If using locally, follow linked instructions to configure your [qBraid](#local-
 account-setup), [AWS](https://github.com/aws/amazon-braket-sdk-python#boto3-
 and-setting-up-aws-credentials), and [IBMQ](https://github.com/Qiskit/qiskit-
 ibm-provider#provider-setup) credentials. ### Check version You can view the
 version of the qBraid-SDK you have installed within Python using the following:
 ```python In [1]: import qbraid In [2]: qbraid.__version__ ``` ## Documentation
```

### Comparing `qbraid-0.6.1/docs/_static/cards/jupyter.png` & `qbraid-0.7.0.dev20240417171913/docs/_static/cards/jupyter.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/docs/_static/cards/python.png` & `qbraid-0.7.0.dev20240417171913/docs/_static/cards/python.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/docs/_static/cards/terminal.png` & `qbraid-0.7.0.dev20240417171913/docs/_static/cards/terminal.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/docs/_static/favicon.ico` & `qbraid-0.7.0.dev20240417171913/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/docs/_static/logo.png` & `qbraid-0.7.0.dev20240417171913/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/docs/_static/pkg-logos/braket.png` & `qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/braket.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/docs/_static/pkg-logos/cirq.png` & `qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/cirq.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/docs/_static/pkg-logos/pennylane.png` & `qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/pennylane.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/docs/_static/pkg-logos/pyquil.png` & `qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/pyquil.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/docs/_static/pkg-logos/qasm.png` & `qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/qasm.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/docs/_static/pkg-logos/qir.png` & `qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/qir.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/docs/_static/pkg-logos/qiskit.png` & `qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/qiskit.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/docs/_static/pkg-logos/quantinuum.png` & `qbraid-0.7.0.dev20240417171913/docs/_static/pkg-logos/quantinuum.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/docs/_static/sdk-files/batch_counts.png` & `qbraid-0.7.0.dev20240417171913/docs/_static/sdk-files/batch_counts.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/docs/_static/sdk-files/conversion_graph.png` & `qbraid-0.7.0.dev20240417171913/docs/_static/sdk-files/conversion_graph.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/docs/_static/sdk-files/get_devices.png` & `qbraid-0.7.0.dev20240417171913/docs/_static/sdk-files/get_devices.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/docs/_static/sdk-files/hub_spokes.png` & `qbraid-0.7.0.dev20240417171913/docs/_static/sdk-files/hub_spokes.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/docs/_static/sdk-files/lab_jobs.png` & `qbraid-0.7.0.dev20240417171913/docs/_static/sdk-files/lab_jobs.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/docs/_static/sdk-files/plot_counts.png` & `qbraid-0.7.0.dev20240417171913/docs/_static/sdk-files/plot_counts.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/docs/conf.py` & `qbraid-0.7.0.dev20240417171913/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/docs/index.rst` & `qbraid-0.7.0.dev20240417171913/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
    :caption: SDK API Reference
    :hidden:
 
    api/qbraid
    api/qbraid.programs
    api/qbraid.interface
    api/qbraid.transpiler
-   api/qbraid.compiler
+   api/qbraid.transforms
    api/qbraid.providers
    api/qbraid.visualization
 
 
 .. Indices and Tables
 .. ------------------
```

#### html2text {}

```diff
@@ -6,10 +6,11 @@
 _**_**_**_**_ _CC_LL_II_ _**_**_**_**
 _[_t_e_r_m_i_n_a_l_]
 _**_**_**_**_ _SS_DD_KK_ _**_**_**_**
 _[_t_e_r_m_i_n_a_l_]
 | .. toctree:: :maxdepth: 1 :caption: SDK User Guide :hidden: sdk/overview sdk/
 programs sdk/transpiler sdk/providers sdk/devices sdk/jobs sdk/results ..
 toctree:: :maxdepth: 1 :caption: SDK API Reference :hidden: api/qbraid api/
-qbraid.programs api/qbraid.interface api/qbraid.transpiler api/qbraid.compiler
-api/qbraid.providers api/qbraid.visualization .. Indices and Tables .. --------
----------- .. * :ref:`genindex` .. * :ref:`modindex` .. * :ref:`search`
+qbraid.programs api/qbraid.interface api/qbraid.transpiler api/
+qbraid.transforms api/qbraid.providers api/qbraid.visualization .. Indices and
+Tables .. ------------------ .. * :ref:`genindex` .. * :ref:`modindex` .. * :
+ref:`search`
```

### Comparing `qbraid-0.6.1/docs/sdk/devices.rst` & `qbraid-0.7.0.dev20240417171913/docs/sdk/devices.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/docs/sdk/jobs.rst` & `qbraid-0.7.0.dev20240417171913/docs/sdk/jobs.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/docs/sdk/overview.rst` & `qbraid-0.7.0.dev20240417171913/docs/sdk/overview.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/docs/sdk/programs.rst` & `qbraid-0.7.0.dev20240417171913/docs/sdk/programs.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/docs/sdk/results.rst` & `qbraid-0.7.0.dev20240417171913/docs/sdk/results.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/docs/sdk/transpiler.rst` & `qbraid-0.7.0.dev20240417171913/docs/sdk/transpiler.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/pyproject.toml` & `qbraid-0.7.0.dev20240417171913/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,39 +24,39 @@
     "Topic :: Scientific/Engineering :: Physics"
 ]
 dependencies = [
     "networkx>=2.5,<4.0",
     "numpy>=1.17,<1.27",
     "openqasm3[parser]>=0.4.0,<0.6.0",
     "ply>=3.6",
-    "qbraid-core>=0.1.1,<0.2.0"
+    "qbraid-core>=0.1.3,<0.2.0"
 ]
 requires-python = ">= 3.9"
 
 [project.urls]
 Homepage = "https://www.qbraid.com/"
 Documentation = "https://docs.qbraid.com/en/stable/"
 "Source Code" = "https://github.com/qBraid/qBraid"
 "Bug Tracker" = "https://github.com/qBraid/qBraid/issues"
 Discord = "https://discord.gg/TPBU2sa8Et"
 "Launch on Lab" = "https://account.qbraid.com/?gitHubUrl=https://github.com/qBraid/qBraid.git"
 
 [project.optional-dependencies]
-braket = ["amazon-braket-sdk>=1.42.1,<1.77.0"]
+braket = ["amazon-braket-sdk>=1.42.1,<1.78.0"]
 cirq = ["cirq-core>=1.3.0,<1.4.0"]
 pennylane = ["pennylane>=0.33.1,<0.36.0"]
 pytket = ["pytket>=1.16.0,<1.27.0"]
 pyquil = ["pyquil>=3.5.4,<4.4.0"]
 qir = ["qbraid-qir>=0.1.1,<0.2.0"]
 qiskit = ["qiskit>=0.44.0,<1.1.0", "qiskit-ibm-provider>=0.5.3,<0.11.0", "qiskit-ibm-runtime>=0.18.0,<0.21.0", "qiskit[visualization]"]
 ionq = ["cirq-core>=1.3.0,<1.4.0", "cirq-ionq>=1.3.0,<1.4.0", "pytket-braket>=0.30.0,<0.36.0"]
 visualization = ["ipython", "matplotlib", "pylatexenc"]
 test = ["pytest", "pytest-cov"]
 lint = ["black", "isort", "pylint"]
-docs = ["sphinx~=7.2.6", "sphinx-autodoc-typehints>=1.24,<2.1", "sphinx-rtd-theme>=1.3,<2.1", "docutils<0.21"]
+docs = ["sphinx~=7.2.6", "sphinx-autodoc-typehints>=1.24,<2.1", "sphinx-rtd-theme>=1.3,<2.1", "docutils<0.22"]
 
 [project.entry-points."qbraid.programs"]
 braket = "qbraid.programs.libs.braket:BraketCircuit"
 cirq = "qbraid.programs.libs.cirq:CirqCircuit"
 pennylane = "qbraid.programs.libs.pennylane:PennylaneTape"
 pyquil = "qbraid.programs.libs.pyquil:PyQuilProgram"
 qiskit = "qbraid.programs.libs.qiskit:QiskitCircuit"
```

### Comparing `qbraid-0.6.1/qbraid/__init__.py` & `qbraid-0.7.0.dev20240417171913/qbraid/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -48,27 +48,27 @@
 from ._import import LazyLoader
 from ._version import __version__
 from .exceptions import QbraidError
 from .get_devices import get_devices
 from .get_jobs import get_jobs
 
 if "sphinx" in sys.modules:
-    from . import compiler, interface, programs, providers, transpiler, visualization
+    from . import interface, programs, providers, transforms, transpiler, visualization
 else:
-    compiler = LazyLoader("compiler", globals(), "qbraid.compiler")
+    transforms = LazyLoader("transforms", globals(), "qbraid.transforms")
     interface = LazyLoader("interface", globals(), "qbraid.interface")
     programs = LazyLoader("programs", globals(), "qbraid.programs")
     providers = LazyLoader("providers", globals(), "qbraid.providers")
     transpiler = LazyLoader("transpiler", globals(), "qbraid.transpiler")
     visualization = LazyLoader("visualization", globals(), "qbraid.visualization")
 
 
 __all__ = [
     "about",
-    "compiler",
+    "transforms",
     "get_devices",
     "get_jobs",
     "interface",
     "LazyLoader",
     "programs",
     "providers",
     "QbraidError",
```

### Comparing `qbraid-0.6.1/qbraid/_about.py` & `qbraid-0.7.0.dev20240417171913/qbraid/_about.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/_compat.py` & `qbraid-0.7.0.dev20240417171913/qbraid/_compat.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/_display.py` & `qbraid-0.7.0.dev20240417171913/qbraid/_display.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/_import.py` & `qbraid-0.7.0.dev20240417171913/qbraid/_import.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/_version.py` & `qbraid-0.7.0.dev20240417171913/qbraid/exceptions.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,13 +5,14 @@
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Module containing version information
-
-Version number (major.minor.patch[-label])
+Module defining exceptions for errors raised by qBraid.
 
 """
-__version__ = "0.6.1"
+
+
+class QbraidError(Exception):
+    """Base class for errors raised by qBraid."""
```

### Comparing `qbraid-0.6.1/qbraid/compiler/__init__.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transforms/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Module for device-specific quantum program conversions
+Module for runtime quantum program transformations.
 
-.. currentmodule:: qbraid.compiler
+.. currentmodule:: qbraid.transforms
 
 Exceptions
 -----------
 
 .. autosummary::
    :toctree: ../stubs/
 
-   CompilerError
+   CompilationError
 
 """
-from .exceptions import CompilerError
+from .exceptions import CompilationError
```

### Comparing `qbraid-0.6.1/qbraid/compiler/braket/__init__.py` & `qbraid-0.7.0.dev20240417171913/qbraid/interface/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Module for compiling programs targeted at Amazon Braket
-supported devices.
+Module providing utilities for interfacing with supported quantum programs.
 
-.. currentmodule:: qbraid.compiler.braket
+.. currentmodule:: qbraid.interface
 
 Functions
-----------
+-----------
 
 .. autosummary::
    :toctree: ../stubs/
 
-   braket_ionq_compile
+   circuits_allclose
+   assert_allclose_up_to_global_phase
 
 """
-from .ionq import braket_ionq_compile
+from .circuit_equality import assert_allclose_up_to_global_phase, circuits_allclose
+from .random import random_circuit, random_unitary_matrix
```

### Comparing `qbraid-0.6.1/qbraid/compiler/braket/ionq.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transforms/pytket/ionq.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Module for converting generic quantum circuits to basis gate set compatible with IonQ devices.
 
 """
-from typing import Union
+from typing import TYPE_CHECKING
 
 import pytket
-from braket.circuits import Circuit
 
 try:
     # pytket >= 1.22
     from pytket.circuit_library import TK1_to_RzRx  # type: ignore
 except (ModuleNotFoundError, ImportError):  # prama: no cover
     try:
         # pytket >1.18,<1.22
@@ -35,16 +34,18 @@
     MaxNQubitsPredicate,
     NoClassicalControlPredicate,
     NoFastFeedforwardPredicate,
     NoMidMeasurePredicate,
     NoSymbolsPredicate,
 )
 
-from qbraid.compiler.exceptions import CompilerError
-from qbraid.transpiler import transpile
+from qbraid.transforms.exceptions import CompilationError
+
+if TYPE_CHECKING:
+    import pytket.circuit
 
 HARMONY_MAX_QUBITS = 11
 
 ionq_gates = {
     pytket.circuit.OpType.X,
     pytket.circuit.OpType.Y,
     pytket.circuit.OpType.Z,
@@ -81,24 +82,23 @@
 ionq_rebase_pass = RebaseCustom(
     ionq_gates,
     pytket.Circuit(),  # cx_replacement (irrelevant)
     TK1_to_RzRx,
 )  # tk1_replacement
 
 
-def braket_ionq_compile(circuit: Union[Circuit, pytket.circuit.Circuit]) -> Circuit:
+def pytket_ionq_transform(circuit: "pytket.circuit.Circuit") -> "pytket.circuit.Circuit":
     """
     Compiles a Braket circuit to a Braket circuit that can run on IonQ Harmony.
 
     Args:
-        circuit (Union[braket.circuits.Circuit, pytket.circuit.Circuit]):
-            The input Braket or PyTKET circuit to be compiled.
+        circuit (pytket.circuit.Circuit): The input PyTKET circuit to be transformed.
 
     Returns:
-        braket.circuits.Circuit: The compiled Braket circuit that can run on IonQ Harmony.
+        pytket.circuit.Circuit: The transformed PyTKET circuit that can run on IonQ Harmony.
 
     Notes:
         - If the input circuit is a braket Circuit, the function
           transpiles it to a ``pytket.circuit.Circuit`` before compilation.
         - The circuit is transpiled using qBraid's transpiler, if it contains
           any of the following gates::
 
@@ -112,17 +112,12 @@
                 MS
                 PSwap
                 Unitary
 
         - Otherwise, the circuit is transpiled using ``pytket-braket``'s ``braket_to_tk``.
 
     """
-    if isinstance(circuit, Circuit):
-        tk_circuit = transpile(circuit, "pytket")
-    else:
-        tk_circuit = circuit
-
-    cu = CompilationUnit(tk_circuit, preds)
+    cu = CompilationUnit(circuit, preds)
     ionq_rebase_pass.apply(cu)
     if not cu.check_all_predicates():
-        raise CompilerError("Circuit cannot be compiled to IonQ Harmony.")
-    return transpile(cu.circuit, "braket")
+        raise CompilationError("Circuit cannot be compiled to IonQ Harmony.")
+    return cu.circuit
```

### Comparing `qbraid-0.6.1/qbraid/compiler/exceptions.py` & `qbraid-0.7.0.dev20240417171913/qbraid/visualization/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
-
 """
-Module defining exceptions for errors raised by the qBraid compiler.
+Module for exceptions raised by visualization tools.
 
 """
-
 from qbraid.exceptions import QbraidError
 
 
-class CompilerError(QbraidError):
-    """Base class for errors raised by the qBraid compiler."""
+class VisualizationError(QbraidError):
+    """Class for errors raised when using visualization features."""
```

### Comparing `qbraid-0.6.1/qbraid/exceptions.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transforms/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Module defining exceptions for errors raised by qBraid.
+Module defining exceptions for errors raised by qBraid transforms.
 
 """
 
+from qbraid.exceptions import QbraidError
 
-class QbraidError(Exception):
-    """Base class for errors raised by qBraid."""
+
+class CompilationError(QbraidError):
+    """Base class for errors raised during circuit compilation processes."""
```

### Comparing `qbraid-0.6.1/qbraid/get_devices.py` & `qbraid-0.7.0.dev20240417171913/qbraid/get_devices.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/get_jobs.py` & `qbraid-0.7.0.dev20240417171913/qbraid/get_jobs.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/interface/__init__.py` & `qbraid-0.7.0.dev20240417171913/qbraid/interface/random/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Module providing utilities for interfacing with supported quantum programs.
+Module for generaing random quantum circuits and unitary matrices
+for testing.
 
-.. currentmodule:: qbraid.interface
+.. currentmodule:: qbraid.interface.random
 
 Functions
------------
+----------
 
 .. autosummary::
    :toctree: ../stubs/
 
-   circuits_allclose
-   assert_allclose_up_to_global_phase
+   random_circuit
+   random_unitary_matrix
 
 """
-from .circuit_equality import assert_allclose_up_to_global_phase, circuits_allclose
 from .random import random_circuit, random_unitary_matrix
```

### Comparing `qbraid-0.6.1/qbraid/interface/circuit_equality.py` & `qbraid-0.7.0.dev20240417171913/qbraid/interface/circuit_equality.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/interface/random/cirq_random.py` & `qbraid-0.7.0.dev20240417171913/qbraid/interface/random/cirq_random.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/interface/random/qasm3_random.py` & `qbraid-0.7.0.dev20240417171913/qbraid/interface/random/qasm3_random.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/interface/random/qiskit_random.py` & `qbraid-0.7.0.dev20240417171913/qbraid/interface/random/qiskit_random.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/interface/random/random.py` & `qbraid-0.7.0.dev20240417171913/qbraid/interface/random/random.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/programs/__init__.py` & `qbraid-0.7.0.dev20240417171913/qbraid/programs/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/programs/_import.py` & `qbraid-0.7.0.dev20240417171913/qbraid/programs/_import.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/programs/abc_program.py` & `qbraid-0.7.0.dev20240417171913/qbraid/programs/abc_program.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/programs/exceptions.py` & `qbraid-0.7.0.dev20240417171913/qbraid/programs/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/programs/inspector.py` & `qbraid-0.7.0.dev20240417171913/qbraid/programs/inspector.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/programs/libs/__init__.py` & `qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/programs/libs/braket.py` & `qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/programs/libs/cirq.py` & `qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/cirq.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/programs/libs/pennylane.py` & `qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/pennylane.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/programs/libs/pyquil.py` & `qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/pyquil.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/programs/libs/pytket.py` & `qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/pytket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/programs/libs/qasm2.py` & `qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/qasm2.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/programs/libs/qasm3.py` & `qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/qasm3.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/programs/libs/qiskit.py` & `qbraid-0.7.0.dev20240417171913/qbraid/programs/libs/qiskit.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/programs/loader.py` & `qbraid-0.7.0.dev20240417171913/qbraid/programs/loader.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/programs/qasm_passes.py` & `qbraid-0.7.0.dev20240417171913/qbraid/programs/qasm_passes.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/programs/qasm_qelib1.py` & `qbraid-0.7.0.dev20240417171913/qbraid/programs/qasm_qelib1.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/providers/__init__.py` & `qbraid-0.7.0.dev20240417171913/qbraid/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/providers/_import.py` & `qbraid-0.7.0.dev20240417171913/qbraid/providers/_import.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/providers/aws/__init__.py` & `qbraid-0.7.0.dev20240417171913/qbraid/providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/providers/aws/device.py` & `qbraid-0.7.0.dev20240417171913/qbraid/providers/aws/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from braket.device_schema import ExecutionDay
 
 from qbraid.programs._import import QPROGRAM_LIBS
 from qbraid.programs.libs.braket import BraketCircuit
 from qbraid.providers.device import QuantumDevice
 from qbraid.providers.enums import DeviceStatus, DeviceType
+from qbraid.transpiler import CircuitConversionError, ConversionPathNotFoundError, transpile
 
 from .job import BraketQuantumTask
 
 if TYPE_CHECKING:
     import braket.aws
     import braket.circuits
 
@@ -195,30 +196,33 @@
         for queue_type in ["Normal", "Priority"]:
             num_queued = queue_depth_info.quantum_tasks[queue_type]
             if isinstance(num_queued, str) and num_queued.startswith(">"):
                 num_queued = num_queued[1:]
             total_queued += int(num_queued)
         return total_queued
 
-    def _transpile(self, run_input):
+    def transform(self, run_input: "braket.circuits.Circuit") -> "braket.circuits.Circuit":
         """Transpile a circuit for the device."""
         if self._device_type.name == "SIMULATOR":
             program = BraketCircuit(run_input)
             program.remove_idle_qubits()
             run_input = program.program
 
-        return run_input
-
-    def _compile(self, run_input):
-        """Compile a circuit for the device."""
         if self.provider.lower() == "ionq" and "pytket" in QPROGRAM_LIBS:
+
             # pylint: disable=import-outside-toplevel
-            from qbraid.compiler.braket.ionq import braket_ionq_compile
+            from qbraid.transforms.pytket.ionq import pytket_ionq_transform
+
+            try:
+                tk_circuit = transpile(run_input, "pytket", max_path_depth=1)
+                tk_transformed = pytket_ionq_transform(tk_circuit)
+                run_input = transpile(tk_transformed, "braket", max_path_depth=1)
+            except (ConversionPathNotFoundError, CircuitConversionError):
+                pass
 
-            run_input = braket_ionq_compile(run_input)
         return run_input
 
     def _run(self, run_input: "braket.circuits.Circuit", *args, **kwargs) -> Dict[str, Any]:
         """Run a quantum task specification on this quantum device. Task must represent a
         quantum circuit, annealing problems not supported.
 
         Args:
```

### Comparing `qbraid-0.6.1/qbraid/providers/aws/job.py` & `qbraid-0.7.0.dev20240417171913/qbraid/providers/aws/job.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/providers/aws/provider.py` & `qbraid-0.7.0.dev20240417171913/qbraid/providers/aws/provider.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/providers/aws/result.py` & `qbraid-0.7.0.dev20240417171913/qbraid/providers/aws/result.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/providers/aws/tracker.py` & `qbraid-0.7.0.dev20240417171913/qbraid/providers/aws/tracker.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/providers/device.py` & `qbraid-0.7.0.dev20240417171913/qbraid/providers/device.py`

 * *Files 3% similar despite different names*

```diff
@@ -219,49 +219,34 @@
         if input_run_package != self._run_package:
             try:
                 run_input = transpile(
                     run_input, self._run_package, conversion_graph=conversion_graph
                 )
             except CircuitConversionError as err:
                 raise QbraidRuntimeError from err
-        return self._transpile(run_input)
-
-    def compile(self, run_input: "qbraid.programs.QPROGRAM") -> "qbraid.programs.QPROGRAM":
-        """Compile run input.
-
-        Returns:
-            :data:`~qbraid.programs.QPROGRAM`: Compiled quantum program (circuit) object
-
-        Raises:
-            QbraidRuntimeError: If circuit conversion fails
-
-        """
-        return self._compile(run_input)
+        return run_input
 
     def process_run_input(
         self,
         run_input: "qbraid.programs.QPROGRAM",
-        auto_compile: bool = False,
         conversion_graph: "Optional[qbraid.transpiler.ConversionGraph]" = None,
     ) -> Tuple[Any, Dict[str, Any]]:
         """Process quantum program before passing to device run method.
 
         Returns:
             Tupe of run input and job data dictionary (num_qubits, depth, openqasm string)
 
         Raises:
             QbraidRuntimeError: If error processing run input
 
         """
         safe_mode = conversion_graph is not None
         qprogram = self.verify_run(run_input, safe_mode=safe_mode)
         run_input = self.transpile(run_input, conversion_graph=conversion_graph)
-
-        if auto_compile:
-            run_input = self._compile(run_input)
+        run_input = self.transform(run_input)
 
         if qprogram is None:
             try:
                 qprogram = load_program(run_input)
             except Exception as err:  # pylint: disable=broad-exception-caught
                 if not safe_mode:
                     raise
@@ -372,21 +357,24 @@
             try:
                 return client.get_job(vendor_id=vendor_job_id)
             except IndexError as err:
                 raise QbraidRuntimeError(f"{self.vendor} job {vendor_job_id} not found") from err
 
         return client.create_job(data=init_data)
 
-    @abstractmethod
-    def _transpile(self, run_input):
-        """Applies any software/device specific modifications to run input."""
+    def transform(
+        self, run_input: Union["qbraid.programs.QPROGRAM", Any]
+    ) -> Union["qbraid.programs.QPROGRAM", Any]:
+        """
+        Override this method with any runtime transformations to apply to the run
+        input, e.g. circuit optimizations, device-specific gate set conversions, etc.
+        Program input type should match output type.
 
-    @abstractmethod
-    def _compile(self, run_input):
-        """Applies any software/device specific modifications to run input."""
+        """
+        return run_input
 
     @abstractmethod
     def _run(self, run_input: "qbraid.programs.QPROGRAM", *args, **kwargs) -> Dict[str, Any]:
         """Vendor run method. Should return dictionary with the following keys:
 
         * "shots" (int): Number of shots. For jobs that don't support shots, set to 0.
         * "tags" (Dict[str, str]): Dictionary of tags. For providers that use list of tags,
@@ -438,69 +426,63 @@
             device=self,
         )
 
     def run(
         self,
         run_input: "qbraid.programs.QPROGRAM",
         *args,
-        auto_compile: bool = False,
         conversion_graph: "Optional[qbraid.transpiler.ConversionGraph]" = None,
         **kwargs,
     ) -> "qbraid.providers.QuantumJob":
         """Run a quantum job specification on this quantum device.
 
         Args:
             run_input: Specification of a task to run on device.
 
         Keyword Args:
             conversion_graph (optional, ConversionGraph): Graph of conversion functions to
                                                           apply to the circuit.
-            auto_compile (bool): Whether to compile the circuit for the device before running.
-                                 Default is False.
             shots (int): The number of times to run the task on the device.
 
         Returns:
             The job like object for the run.
 
         """
         run_input, program_data = self.process_run_input(
-            run_input, auto_compile=auto_compile, conversion_graph=conversion_graph
+            run_input, conversion_graph=conversion_graph
         )
         vendor_job_data = self._run(run_input, *args, **kwargs)
         return self.process_vendor_job_data(vendor_job_data, program_data)
 
     def run_batch(
         self,
         run_input: "List[qbraid.programs.QPROGRAM]",
         *args,
-        auto_compile: bool = False,
         conversion_graph: "Optional[qbraid.transpiler.ConversionGraph]" = None,
         **kwargs,
     ) -> "Union[qbraid.providers.QuantumJob, List[qbraid.providers.QuantumJob]]":
         """Run a quantum job specification on this quantum device.
 
         Args:
             run_input: Specification of a task to run on device.
 
         Keyword Args:
             conversion_graph (optional, ConversionGraph): Graph of conversion functions to
                                                           apply to the circuit.
-            auto_compile (bool): Whether to compile the circuit for the device before running.
-                                 Default is False.
             shots (int): The number of times to run the task on the device.
 
         Returns:
             The job like object for the run.
 
         """
         program_data_batch = []
         run_input_batch = []
         for program in run_input:
             run_input_transpiled, program_data = self.process_run_input(
-                program, auto_compile=auto_compile, conversion_graph=conversion_graph
+                program, conversion_graph=conversion_graph
             )
             run_input_batch.append(run_input_transpiled)
             program_data_batch.append(program_data)
         num_qubits_batch = [data.get("num_qubits") for data in program_data_batch]
         depth_batch = [data.get("depth") for data in program_data_batch]
         openqasm_batch = [data.get("openqasm") for data in program_data_batch]
         program_data = {
```

### Comparing `qbraid-0.6.1/qbraid/providers/enums.py` & `qbraid-0.7.0.dev20240417171913/qbraid/providers/enums.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/providers/exceptions.py` & `qbraid-0.7.0.dev20240417171913/qbraid/providers/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/providers/ibm/__init__.py` & `qbraid-0.7.0.dev20240417171913/qbraid/providers/ibm/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/providers/ibm/device.py` & `qbraid-0.7.0.dev20240417171913/qbraid/providers/ibm/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,25 +81,22 @@
         except (AttributeError, TranspilerError):
             self._num_qubits = (
                 5000
                 if device.name == "simulator_stabilizer"
                 else 63 if device.name == "simulator_extended_stabilizer" else None
             )
 
-    def _transpile(self, run_input):
+    def transform(self, run_input: "qiskit.QuantumCircuit") -> "qiskit.QuantumCircuit":
         if self._device_type.name != "FAKE" and self._device.local:
             program = QiskitCircuit(run_input)
             program.remove_idle_qubits()
             run_input = program.program
 
         return transpile(run_input, backend=self._device)
 
-    def _compile(self, run_input):
-        return run_input
-
     def status(self):
         """Return the status of this Device.
 
         Returns:
             str: The status of this Device
         """
         if self._device_type == DeviceType("FAKE"):
```

### Comparing `qbraid-0.6.1/qbraid/providers/ibm/job.py` & `qbraid-0.7.0.dev20240417171913/qbraid/providers/ibm/job.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/providers/ibm/provider.py` & `qbraid-0.7.0.dev20240417171913/qbraid/providers/ibm/provider.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,18 +41,14 @@
         Args:
             qiskit_ibm_token (str, optional): IBM Quantum token. Defaults to None.
         """
         self.qiskit_ibm_token = qiskit_ibm_token or os.getenv("QISKIT_IBM_TOKEN")
         self._provider = self._get_ibm_provider(**kwargs)
 
     @abstractmethod
-    def save_config(self):
-        """Save the current configuration."""
-
-    @abstractmethod
     def _get_ibm_provider(self, **kwargs):
         """Returns the IBM Quantum provider."""
 
     def get_devices(
         self, operational=True, **kwargs
     ) -> List[Union["qiskit_ibm_provider.IBMBackend", "qiskit_ibm_runtime.IBMBackend"]]:
         """Returns the IBM Quantum provider backends."""
@@ -107,18 +103,14 @@
         backends = self.get_devices(simulator=False, operational=True)
         return least_busy(backends)
 
 
 class QiskitRuntime(QiskitRemoteService):
     """Wrapper for qiskit_ibm_runtime.QiskitRuntimeService class."""
 
-    def save_config(self):
-        """Save the current configuration."""
-        raise NotImplementedError
-
     def _get_ibm_provider(
         self, channel: str = "ibm_quantum", **kwargs
     ) -> "qiskit_ibm_runtime.QiskitRuntimeService":
         """Returns the IBM Qiskt Runtime service."""
         # pylint: disable-next=import-outside-toplevel
         from qiskit_ibm_runtime import QiskitRuntimeService
```

### Comparing `qbraid-0.6.1/qbraid/providers/ibm/result.py` & `qbraid-0.7.0.dev20240417171913/qbraid/providers/ibm/result.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/providers/job.py` & `qbraid-0.7.0.dev20240417171913/qbraid/providers/job.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/providers/provider.py` & `qbraid-0.7.0.dev20240417171913/qbraid/providers/provider.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/providers/result.py` & `qbraid-0.7.0.dev20240417171913/qbraid/providers/result.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/providers/status_maps.py` & `qbraid-0.7.0.dev20240417171913/qbraid/providers/status_maps.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/__init__.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/annotations.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/annotations.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/conversions/__init__.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/conversions/braket/__init__.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/braket/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/conversions/braket/cirq_from_braket.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/braket/cirq_from_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/conversions/braket/cirq_to_braket.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/braket/cirq_to_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/conversions/braket/conversions_cirq.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/braket/conversions_cirq.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/conversions/braket/conversions_qasm.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/braket/conversions_qasm.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/conversions/braket/custom_instr.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/braket/custom_instr.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/conversions/cirq/__init__.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/cirq/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/conversions/cirq/cirq_qasm_parser.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/cirq/cirq_qasm_parser.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/conversions/cirq/conversions_qasm.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/cirq/conversions_qasm.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/conversions/cirq/custom_ops.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/cirq/custom_ops.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/conversions/openqasm3/__init__.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/openqasm3/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/conversions/openqasm3/conversions_qasm.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/openqasm3/conversions_qasm.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/conversions/pennylane/__init__.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pennylane/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/conversions/pennylane/conversions_qasm.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pennylane/conversions_qasm.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/conversions/pyquil/__init__.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pyquil/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/conversions/pyquil/cirq_quil_input.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pyquil/cirq_quil_input.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/conversions/pyquil/cirq_quil_output.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pyquil/cirq_quil_output.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/conversions/pyquil/conversions_cirq.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pyquil/conversions_cirq.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/conversions/pytket/__init__.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pytket/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/conversions/pytket/conversions_braket.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pytket/conversions_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/conversions/pytket/conversions_qasm.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/pytket/conversions_qasm.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/conversions/qiskit/__init__.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/qiskit/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/conversions/qiskit/conversions_braket.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/qiskit/conversions_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/conversions/qiskit/conversions_qasm.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/conversions/qiskit/conversions_qasm.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/converter.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/converter.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/edge.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/edge.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/exceptions.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/transpiler/graph.py` & `qbraid-0.7.0.dev20240417171913/qbraid/transpiler/graph.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/visualization/__init__.py` & `qbraid-0.7.0.dev20240417171913/qbraid/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/visualization/draw_circuit.py` & `qbraid-0.7.0.dev20240417171913/qbraid/visualization/draw_circuit.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/visualization/draw_qasm3.py` & `qbraid-0.7.0.dev20240417171913/qbraid/visualization/draw_qasm3.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/visualization/plot_conversions.py` & `qbraid-0.7.0.dev20240417171913/qbraid/visualization/plot_conversions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid/visualization/plot_counts.py` & `qbraid-0.7.0.dev20240417171913/qbraid/visualization/plot_counts.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid.egg-info/PKG-INFO` & `qbraid-0.7.0.dev20240417171913/qbraid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid
-Version: 0.6.1
+Version: 0.7.0.dev20240417171913
 Summary: A Python toolkit for cross-framework abstraction of quantum programs.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -699,17 +699,17 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: networkx<4.0,>=2.5
 Requires-Dist: numpy<1.27,>=1.17
 Requires-Dist: openqasm3[parser]<0.6.0,>=0.4.0
 Requires-Dist: ply>=3.6
-Requires-Dist: qbraid-core<0.2.0,>=0.1.1
+Requires-Dist: qbraid-core<0.2.0,>=0.1.3
 Provides-Extra: braket
-Requires-Dist: amazon-braket-sdk<1.77.0,>=1.42.1; extra == "braket"
+Requires-Dist: amazon-braket-sdk<1.78.0,>=1.42.1; extra == "braket"
 Provides-Extra: cirq
 Requires-Dist: cirq-core<1.4.0,>=1.3.0; extra == "cirq"
 Provides-Extra: pennylane
 Requires-Dist: pennylane<0.36.0,>=0.33.1; extra == "pennylane"
 Provides-Extra: pytket
 Requires-Dist: pytket<1.27.0,>=1.16.0; extra == "pytket"
 Provides-Extra: pyquil
@@ -736,15 +736,15 @@
 Requires-Dist: black; extra == "lint"
 Requires-Dist: isort; extra == "lint"
 Requires-Dist: pylint; extra == "lint"
 Provides-Extra: docs
 Requires-Dist: sphinx~=7.2.6; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints<2.1,>=1.24; extra == "docs"
 Requires-Dist: sphinx-rtd-theme<2.1,>=1.3; extra == "docs"
-Requires-Dist: docutils<0.21; extra == "docs"
+Requires-Dist: docutils<0.22; extra == "docs"
 
 <img width=full alt="qbraid-sdk-header" src="https://user-images.githubusercontent.com/46977852/224456452-605e51f2-193d-4789-863e-e51cdd4b0a54.png">
 
 <p align="center">
   <a href="https://github.com/qBraid/qBraid/actions/workflows/main.yml">
     <img src="https://github.com/qBraid/qBraid/actions/workflows/main.yml/badge.svg?branch=main" alt="CI"/>
   </a>
@@ -795,21 +795,21 @@
 
 Using the SDK on [qBraid Lab](https://docs.qbraid.com/projects/lab/en/latest/lab/overview.html) means direct, pre-configured access to QPUs from IonQ, Oxford Quantum Circuits, QuEra, and Rigetti, as well as on-demand simulators from AWS, all with no additional access keys or API tokens required. See [qBraid Quantum Jobs](https://docs.qbraid.com/projects/lab/en/latest/lab/quantum_jobs.html) for more.
 
 ### Local install
 
 The qBraid-SDK, and all of its dependencies, can also be installed using pip:
 
-```bash
+```shell
 pip install qbraid
 ```
 
 You can also [install from source](CONTRIBUTING.md#installing-from-source) by cloning this repository and running a pip install command in the root directory of the repository:
 
-```bash
+```shell
 git clone https://github.com/qBraid/qBraid.git
 cd qBraid
 pip install .
 ```
 
 *Note*: The qBraid-SDK requires Python 3.9 or greater.
```

### Comparing `qbraid-0.6.1/qbraid.egg-info/SOURCES.txt` & `qbraid-0.7.0.dev20240417171913/qbraid.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 docs/_static/pkg-logos/quantinuum.png
 docs/_static/sdk-files/batch_counts.png
 docs/_static/sdk-files/conversion_graph.png
 docs/_static/sdk-files/get_devices.png
 docs/_static/sdk-files/hub_spokes.png
 docs/_static/sdk-files/lab_jobs.png
 docs/_static/sdk-files/plot_counts.png
-docs/api/qbraid.compiler.rst
 docs/api/qbraid.interface.rst
 docs/api/qbraid.programs.rst
 docs/api/qbraid.providers.rst
 docs/api/qbraid.rst
+docs/api/qbraid.transforms.rst
 docs/api/qbraid.transpiler.rst
 docs/api/qbraid.visualization.rst
 docs/sdk/devices.rst
 docs/sdk/jobs.rst
 docs/sdk/overview.rst
 docs/sdk/programs.rst
 docs/sdk/providers.rst
@@ -53,18 +53,14 @@
 qbraid/get_jobs.py
 qbraid.egg-info/PKG-INFO
 qbraid.egg-info/SOURCES.txt
 qbraid.egg-info/dependency_links.txt
 qbraid.egg-info/entry_points.txt
 qbraid.egg-info/requires.txt
 qbraid.egg-info/top_level.txt
-qbraid/compiler/__init__.py
-qbraid/compiler/exceptions.py
-qbraid/compiler/braket/__init__.py
-qbraid/compiler/braket/ionq.py
 qbraid/interface/__init__.py
 qbraid/interface/circuit_equality.py
 qbraid/interface/random/__init__.py
 qbraid/interface/random/cirq_random.py
 qbraid/interface/random/qasm3_random.py
 qbraid/interface/random/qiskit_random.py
 qbraid/interface/random/random.py
@@ -101,14 +97,18 @@
 qbraid/providers/aws/result.py
 qbraid/providers/aws/tracker.py
 qbraid/providers/ibm/__init__.py
 qbraid/providers/ibm/device.py
 qbraid/providers/ibm/job.py
 qbraid/providers/ibm/provider.py
 qbraid/providers/ibm/result.py
+qbraid/transforms/__init__.py
+qbraid/transforms/exceptions.py
+qbraid/transforms/pytket/__init__.py
+qbraid/transforms/pytket/ionq.py
 qbraid/transpiler/__init__.py
 qbraid/transpiler/annotations.py
 qbraid/transpiler/converter.py
 qbraid/transpiler/edge.py
 qbraid/transpiler/exceptions.py
 qbraid/transpiler/graph.py
 qbraid/transpiler/conversions/__init__.py
```

### Comparing `qbraid-0.6.1/qbraid.egg-info/entry_points.txt` & `qbraid-0.7.0.dev20240417171913/qbraid.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/qbraid.egg-info/requires.txt` & `qbraid-0.7.0.dev20240417171913/qbraid.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 networkx<4.0,>=2.5
 numpy<1.27,>=1.17
 openqasm3[parser]<0.6.0,>=0.4.0
 ply>=3.6
-qbraid-core<0.2.0,>=0.1.1
+qbraid-core<0.2.0,>=0.1.3
 
 [braket]
-amazon-braket-sdk<1.77.0,>=1.42.1
+amazon-braket-sdk<1.78.0,>=1.42.1
 
 [cirq]
 cirq-core<1.4.0,>=1.3.0
 
 [docs]
 sphinx~=7.2.6
 sphinx-autodoc-typehints<2.1,>=1.24
 sphinx-rtd-theme<2.1,>=1.3
-docutils<0.21
+docutils<0.22
 
 [ionq]
 cirq-core<1.4.0,>=1.3.0
 cirq-ionq<1.4.0,>=1.3.0
 pytket-braket<0.36.0,>=0.30.0
 
 [lint]
```

### Comparing `qbraid-0.6.1/tools/verify_headers.py` & `qbraid-0.7.0.dev20240417171913/tools/verify_headers.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.6.1/tox.ini` & `qbraid-0.7.0.dev20240417171913/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -24,26 +24,23 @@
 [testenv:unit-tests]
 description = Run pytests and generate coverage report.
 commands =
     python3 tools/set_provider_configs.py
     coverage run -m pytest -x tests/programs \
                               tests/transpiler \
                               tests/providers \
-                              tests/compiler \
+                              tests/transforms \
                               tests/visualization \
                               tests/top_level \
                            -W ignore::DeprecationWarning \
                            -W ignore::PendingDeprecationWarning \
                            -W ignore::urllib3.exceptions.InsecureRequestWarning \
                            -W ignore::RuntimeWarning
     coverage combine
-    coverage report --omit=qbraid/transpiler/conversions/cirq/custom_ops.py \
-                           qbraid/visualization/draw_circuit.py \
-                           qbraid/visualization/plot_conversions.py \
-                           qbraid/_compat.py
+    coverage report --omit=qbraid/transpiler/conversions/cirq/custom_ops.py,qbraid/visualization/draw_circuit.py,qbraid/visualization/plot_conversions.py,qbraid/_compat.py
     coverage html
     coverage xml
 
 [testenv:docs]
 description = Use sphinx to build the HTML docs.
 extras =
     docs
```

