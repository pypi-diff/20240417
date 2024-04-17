# Comparing `tmp/qiskit-ibm-provider-0.8.0.tar.gz` & `tmp/qiskit-ibm-provider-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-ibm-provider-0.8.0.tar", last modified: Fri Jan  5 17:57:23 2024, max compression
+gzip compressed data, was "qiskit-ibm-provider-0.9.0.tar", last modified: Wed Feb  7 17:12:56 2024, max compression
```

## Comparing `qiskit-ibm-provider-0.8.0.tar` & `qiskit-ibm-provider-0.9.0.tar`

### file list

```diff
@@ -1,202 +1,201 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.409020 qiskit-ibm-provider-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-01-05 17:57:23.409020 qiskit-ibm-provider-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.381020 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.385020 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/accounts/
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/accounts/account.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/accounts/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6133 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/accounts/management.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/accounts/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.385020 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/client_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.385020 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/clients/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/clients/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/clients/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/clients/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/clients/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/clients/runtime_ws.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/clients/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/clients/websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.389020 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/rest/
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/rest/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/rest/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/rest/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/rest/program_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/rest/root.py
--rw-r--r--   0 runner    (1001) docker     (127)     7263 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/rest/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/rest/runtime_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.389020 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/rest/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/rest/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/rest/utils/data_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    13683 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/apiconstants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/hub_group_project.py
--rw-r--r--   0 runner    (1001) docker     (127)    40211 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/ibm_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    29974 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/ibm_backend_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    25331 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/ibm_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/ibm_qubit_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.389020 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/job/
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/job/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/job/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    32999 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/job/ibm_circuit_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    48947 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/job/ibm_composite_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     7826 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/job/ibm_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/job/job_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6792 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/job/queueinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/job/sub_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/job/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.389020 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/backend_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/config_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.393020 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/dashboard/backend_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/dashboard/backend_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/dashboard/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/dashboard/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/dashboard/job_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/dashboard/provider_buttons.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/dashboard/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/dashboard/watcher_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/gates_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/jobs_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/qubits_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.393020 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/proxies/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/proxies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/proxies/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.393020 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/qpy/
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/qpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.393020 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/qpy/binary_io/
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/qpy/binary_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51916 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/qpy/binary_io/circuits.py
--rw-r--r--   0 runner    (1001) docker     (127)    24145 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/qpy/binary_io/schedules.py
--rw-r--r--   0 runner    (1001) docker     (127)    26286 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/qpy/binary_io/value.py
--rw-r--r--   0 runner    (1001) docker     (127)    10861 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/qpy/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/qpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/qpy/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)    11208 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/qpy/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    15967 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/qpy/type_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.393020 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/transpiler/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/transpiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.393020 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/transpiler/passes/
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/transpiler/passes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.397020 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/transpiler/passes/basis/
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/transpiler/passes/basis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/transpiler/passes/basis/convert_id_to_delay.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.397020 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/transpiler/passes/scheduling/
--rw-r--r--   0 runner    (1001) docker     (127)    13125 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/transpiler/passes/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25338 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/transpiler/passes/scheduling/block_base_padder.py
--rw-r--r--   0 runner    (1001) docker     (127)    27158 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/transpiler/passes/scheduling/dynamical_decoupling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/transpiler/passes/scheduling/pad_delay.py
--rw-r--r--   0 runner    (1001) docker     (127)    28286 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/transpiler/passes/scheduling/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/transpiler/passes/scheduling/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/transpiler/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.397020 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/utils/backend_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/utils/hgp.py
--rw-r--r--   0 runner    (1001) docker     (127)    11926 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    15554 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/utils/json_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/utils/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/utils/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/utils/qobj_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.397020 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/visualization/colormaps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/visualization/device_layouts.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/visualization/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.401020 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/visualization/interactive/
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/visualization/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16847 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/visualization/interactive/error_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/visualization/interactive/gate_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/visualization/interactive/plotly_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.409020 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-01-05 17:57:23.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-01-05 17:57:23.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-05 17:57:23.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-01-05 17:57:23.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-05 17:57:23.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-01-05 17:57:23.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-05 17:57:23.000000 qiskit-ibm-provider-0.8.0/qiskit_ibm_provider.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-01-05 17:57:23.409020 qiskit-ibm-provider-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.401020 qiskit-ibm-provider-0.8.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/contextmanagers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.401020 qiskit-ibm-provider-0.8.0/test/e2e/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/e2e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/e2e/test_real_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/e2e/test_tutorials.py
--rw-r--r--   0 runner    (1001) docker     (127)    18373 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/fake_account_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/http_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/ibm_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.405020 qiskit-ibm-provider-0.8.0/test/integration/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/integration/test_account_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/integration/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/integration/test_basic_server_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)    40183 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/integration/test_composite_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/integration/test_filter_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/integration/test_ibm_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    19938 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/integration/test_ibm_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    14070 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/integration/test_ibm_job_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14240 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/integration/test_ibm_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/integration/test_ibm_qasm_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/integration/test_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/integration/test_proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)     9271 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/integration/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/integration/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     8803 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/integration/test_websocket_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/jobtestcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/proxy_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.405020 qiskit-ibm-provider-0.8.0/test/unit/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.405020 qiskit-ibm-provider-0.8.0/test/unit/mock/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/unit/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/unit/mock/fake_account_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/unit/mock/fake_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    16245 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/unit/test_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    12181 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/unit/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    19649 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/unit/test_ibm_job_states.py
--rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/unit/test_ibm_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/unit/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/unit/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/unit/test_utils_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/unit/test_websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.405020 qiskit-ibm-provider-0.8.0/test/unit/transpiler/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/unit/transpiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.405020 qiskit-ibm-provider-0.8.0/test/unit/transpiler/passes/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/unit/transpiler/passes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.405020 qiskit-ibm-provider-0.8.0/test/unit/transpiler/passes/basis/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/unit/transpiler/passes/basis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/unit/transpiler/passes/basis/test_convert_id_to_delay.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.409020 qiskit-ibm-provider-0.8.0/test/unit/transpiler/passes/scheduling/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/unit/transpiler/passes/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/unit/transpiler/passes/scheduling/control_flow_test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)    34139 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/unit/transpiler/passes/scheduling/test_dynamical_decoupling.py
--rw-r--r--   0 runner    (1001) docker     (127)    63425 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/unit/transpiler/passes/scheduling/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/unit/transpiler/passes/scheduling/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:57:23.409020 qiskit-ibm-provider-0.8.0/test/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/unit/utils/ws_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-01-05 17:57:13.000000 qiskit-ibm-provider-0.8.0/test/ws_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.731935 qiskit-ibm-provider-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7183 2024-02-07 17:12:56.731935 qiskit-ibm-provider-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.703935 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.703935 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/accounts/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/accounts/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/accounts/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6133 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/accounts/management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/accounts/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.707935 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/client_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.707935 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/clients/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/clients/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/clients/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/clients/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/clients/runtime_ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/clients/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/clients/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.707935 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/rest/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/rest/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/rest/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/rest/program_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/rest/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7263 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/rest/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/rest/runtime_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.707935 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/rest/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/rest/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/rest/utils/data_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13683 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/apiconstants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/hub_group_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40201 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/ibm_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29974 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/ibm_backend_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25331 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/ibm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/ibm_qubit_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.711935 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/job/
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/job/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/job/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32999 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/job/ibm_circuit_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48947 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/job/ibm_composite_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7826 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/job/ibm_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/job/job_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6792 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/job/queueinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/job/sub_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/job/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.711935 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/backend_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/config_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.715936 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/dashboard/backend_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/dashboard/backend_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/dashboard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11737 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/dashboard/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/dashboard/job_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/dashboard/provider_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/dashboard/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/dashboard/watcher_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/gates_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10003 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/jobs_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/qubits_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.715936 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/proxies/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/proxies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/proxies/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.715936 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/qpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/qpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.715936 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/qpy/binary_io/
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/qpy/binary_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51509 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/qpy/binary_io/circuits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24145 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/qpy/binary_io/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26286 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/qpy/binary_io/value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10861 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/qpy/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/qpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/qpy/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11208 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/qpy/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15967 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/qpy/type_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.715936 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/transpiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/transpiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.715936 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/transpiler/passes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/transpiler/passes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.715936 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/transpiler/passes/basis/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/transpiler/passes/basis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/transpiler/passes/basis/convert_id_to_delay.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.719936 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/transpiler/passes/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (127)    13390 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/transpiler/passes/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25338 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/transpiler/passes/scheduling/block_base_padder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27355 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/transpiler/passes/scheduling/dynamical_decoupling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/transpiler/passes/scheduling/pad_delay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28286 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/transpiler/passes/scheduling/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14869 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/transpiler/passes/scheduling/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/transpiler/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.719936 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/utils/backend_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/utils/hgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15554 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/utils/json_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/utils/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/utils/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6385 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/utils/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/utils/qobj_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.719936 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/visualization/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/visualization/device_layouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/visualization/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.719936 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/visualization/interactive/
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/visualization/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17191 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/visualization/interactive/error_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/visualization/interactive/gate_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/visualization/interactive/plotly_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.731935 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7183 2024-02-07 17:12:56.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-02-07 17:12:56.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 17:12:56.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-07 17:12:56.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 17:12:56.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-07 17:12:56.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-07 17:12:56.000000 qiskit-ibm-provider-0.9.0/qiskit_ibm_provider.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-02-07 17:12:56.731935 qiskit-ibm-provider-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.723935 qiskit-ibm-provider-0.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/contextmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.723935 qiskit-ibm-provider-0.9.0/test/e2e/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/e2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/e2e/test_real_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/e2e/test_tutorials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18416 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/fake_account_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/http_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/ibm_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.727935 qiskit-ibm-provider-0.9.0/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/integration/test_account_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/integration/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/integration/test_basic_server_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/integration/test_filter_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/integration/test_ibm_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19859 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/integration/test_ibm_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14067 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/integration/test_ibm_job_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14186 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/integration/test_ibm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/integration/test_ibm_qasm_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/integration/test_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/integration/test_proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9198 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/integration/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/integration/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/integration/test_websocket_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/jobtestcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/proxy_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.727935 qiskit-ibm-provider-0.9.0/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.727935 qiskit-ibm-provider-0.9.0/test/unit/mock/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/unit/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/unit/mock/fake_account_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/unit/mock/fake_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16245 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/unit/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/unit/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19662 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/unit/test_ibm_job_states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/unit/test_ibm_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/unit/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/unit/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/unit/test_utils_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/unit/test_websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.727935 qiskit-ibm-provider-0.9.0/test/unit/transpiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/unit/transpiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.727935 qiskit-ibm-provider-0.9.0/test/unit/transpiler/passes/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/unit/transpiler/passes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.727935 qiskit-ibm-provider-0.9.0/test/unit/transpiler/passes/basis/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/unit/transpiler/passes/basis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/unit/transpiler/passes/basis/test_convert_id_to_delay.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.731935 qiskit-ibm-provider-0.9.0/test/unit/transpiler/passes/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/unit/transpiler/passes/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34539 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/unit/transpiler/passes/scheduling/test_dynamical_decoupling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63256 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/unit/transpiler/passes/scheduling/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/unit/transpiler/passes/scheduling/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:12:56.731935 qiskit-ibm-provider-0.9.0/test/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/unit/utils/ws_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7711 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-02-07 17:12:47.000000 qiskit-ibm-provider-0.9.0/test/ws_server.py
```

### Comparing `qiskit-ibm-provider-0.8.0/LICENSE.txt` & `qiskit-ibm-provider-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/PKG-INFO` & `qiskit-ibm-provider-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ibm-provider
-Version: 0.8.0
+Version: 0.9.0
 Summary: Qiskit IBM Quantum Provider for accessing the quantum devices and simulators at IBM
 Home-page: https://github.com/Qiskit/qiskit-ibm-provider
 Author: Qiskit Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-ibm-provider/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
@@ -119,15 +119,15 @@
 from qiskit_ibm_provider import IBMProvider
 provider = IBMProvider(token='MY_API_TOKEN')
 ```
 
 ## Next Steps
 
 Now you're set up and ready to check out some of the tutorials.
-- [Qiskit IBM Provider]
+- [IBM Quantum Learning]
 - [Qiskit]
 
 ## Contribution Guidelines
 
 If you'd like to contribute to qiskit-ibm-provider, please take a look at our
 [contribution guidelines]. This project adheres to Qiskit's [code of conduct].
 By participating, you are expect to uphold to this code.
@@ -155,12 +155,12 @@
 [code of conduct]: https://github.com/Qiskit/qiskit-ibm-provider/blob/main/CODE_OF_CONDUCT.md
 [GitHub issues]: https://github.com/Qiskit/qiskit-ibm-provider/issues
 [slack]: https://qiskit.slack.com
 [Qiskit.org]: https://qiskit.org
 [Stack Exchange]: https://quantumcomputing.stackexchange.com/questions/tagged/qiskit
 [Qiskit Tutorial]: https://github.com/Qiskit/qiskit-tutorial
 [many people]: https://github.com/Qiskit/qiskit-ibm-provider/graphs/contributors
-[Qiskit IBM Provider]: https://github.com/Qiskit/qiskit-ibm-provider/tree/main/docs/tutorials
+[IBM Quantum Learning]: https://learning.quantum.ibm.com/catalog/tutorials
 [Qiskit]: https://github.com/Qiskit/qiskit-tutorial
 [BibTeX file]: https://github.com/Qiskit/qiskit/blob/master/Qiskit.bib
 [Apache License 2.0]: https://github.com/Qiskit/qiskit-ibm-provider/blob/main/LICENSE.txt
 [migration guide]: https://github.com/Qiskit/qiskit-ibm-provider/blob/6be5f3297ede75bb062b20601058b55a397668e3/docs/tutorials/Migration_Guide_from_qiskit-ibmq-provider.ipynb
```

### Comparing `qiskit-ibm-provider-0.8.0/README.md` & `qiskit-ibm-provider-0.9.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 from qiskit_ibm_provider import IBMProvider
 provider = IBMProvider(token='MY_API_TOKEN')
 ```
 
 ## Next Steps
 
 Now you're set up and ready to check out some of the tutorials.
-- [Qiskit IBM Provider]
+- [IBM Quantum Learning]
 - [Qiskit]
 
 ## Contribution Guidelines
 
 If you'd like to contribute to qiskit-ibm-provider, please take a look at our
 [contribution guidelines]. This project adheres to Qiskit's [code of conduct].
 By participating, you are expect to uphold to this code.
@@ -107,12 +107,12 @@
 [code of conduct]: https://github.com/Qiskit/qiskit-ibm-provider/blob/main/CODE_OF_CONDUCT.md
 [GitHub issues]: https://github.com/Qiskit/qiskit-ibm-provider/issues
 [slack]: https://qiskit.slack.com
 [Qiskit.org]: https://qiskit.org
 [Stack Exchange]: https://quantumcomputing.stackexchange.com/questions/tagged/qiskit
 [Qiskit Tutorial]: https://github.com/Qiskit/qiskit-tutorial
 [many people]: https://github.com/Qiskit/qiskit-ibm-provider/graphs/contributors
-[Qiskit IBM Provider]: https://github.com/Qiskit/qiskit-ibm-provider/tree/main/docs/tutorials
+[IBM Quantum Learning]: https://learning.quantum.ibm.com/catalog/tutorials
 [Qiskit]: https://github.com/Qiskit/qiskit-tutorial
 [BibTeX file]: https://github.com/Qiskit/qiskit/blob/master/Qiskit.bib
 [Apache License 2.0]: https://github.com/Qiskit/qiskit-ibm-provider/blob/main/LICENSE.txt
 [migration guide]: https://github.com/Qiskit/qiskit-ibm-provider/blob/6be5f3297ede75bb062b20601058b55a397668e3/docs/tutorials/Migration_Guide_from_qiskit-ibmq-provider.ipynb
```

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/__init__.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/accounts/__init__.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/accounts/account.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/accounts/account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/accounts/exceptions.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/accounts/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/accounts/management.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/accounts/management.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/accounts/storage.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/accounts/storage.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/__init__.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/auth.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/auth.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/client_parameters.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/client_parameters.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/clients/__init__.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/clients/account.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/clients/account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/clients/auth.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/clients/auth.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/clients/base.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/clients/base.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/clients/runtime.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/clients/runtime.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/clients/runtime_ws.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/clients/runtime_ws.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/clients/version.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/clients/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/clients/websocket.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/clients/websocket.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/exceptions.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/rest/__init__.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/rest/backend.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/rest/backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/rest/base.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/rest/base.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/rest/job.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/rest/job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/rest/program_job.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/rest/program_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/rest/root.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/rest/root.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/rest/runtime.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/rest/runtime.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/rest/runtime_session.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/rest/runtime_session.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/rest/utils/__init__.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/rest/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/rest/utils/data_mapper.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/rest/utils/data_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/api/session.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/api/session.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/apiconstants.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/apiconstants.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/exceptions.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/hub_group_project.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/hub_group_project.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/ibm_backend.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/ibm_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     AcquireChannel,
     ControlChannel,
     DriveChannel,
     MeasureChannel,
 )
 
 from qiskit.qobj.utils import MeasLevel, MeasReturnType
-from qiskit.tools.events.pubsub import Publisher
 from qiskit.transpiler.passmanager import PassManager
 from qiskit.transpiler.target import Target
 
 from qiskit_ibm_provider import (  # pylint: disable=unused-import
     ibm_provider,
 )
 from .session import Session
@@ -56,14 +55,15 @@
 
 from .job import IBMJob, IBMCircuitJob
 from .transpiler.passes.basis.convert_id_to_delay import (
     ConvertIdToDelay,
 )
 from .utils import validate_job_tags, are_circuits_dynamic
 from .utils.options import QASM2Options, QASM3Options
+from .utils.pubsub import Publisher
 from .utils.converters import local_to_utc
 from .utils.json_decoder import (
     defaults_from_server_data,
     properties_from_server_data,
     target_from_server_data,
 )
 from .api.exceptions import RequestsApiError
@@ -589,15 +589,15 @@
 
         This data describes qubits properties (such as T1 and T2),
         gates properties (such as gate length and error), and other general
         properties of the backend.
 
         The schema for backend properties can be found in
         `Qiskit/ibm-quantum-schemas
-        <https://github.com/Qiskit/ibm-quantum-schemas/blob/main/schemas/backend_properties_schema.json>`_.
+        <https://github.com/Qiskit/ibm-quantum-schemas/blob/main/schemas/backend_properties_schema.json>`__.
 
         Args:
             refresh: If ``True``, re-query the server for the backend properties.
                 Otherwise, return a cached version.
             datetime: By specifying `datetime`, this function returns an instance
                 of the :class:`BackendProperties<qiskit.providers.models.BackendProperties>`
                 whose timestamp is closest to, but older than, the specified `datetime`.
@@ -661,15 +661,15 @@
             ) from ex
 
     def defaults(self, refresh: bool = False) -> Optional[PulseDefaults]:
         """Return the pulse defaults for the backend.
 
         The schema for default pulse configuration can be found in
         `Qiskit/ibm-quantum-schemas
-        <https://github.com/Qiskit/ibm-quantum-schemas/blob/main/schemas/default_pulse_configuration_schema.json>`_.
+        <https://github.com/Qiskit/ibm-quantum-schemas/blob/main/schemas/default_pulse_configuration_schema.json>`__.
 
         Args:
             refresh: If ``True``, re-query the server for the backend pulse defaults.
                 Otherwise, return a cached version.
 
         Returns:
             The backend pulse defaults or ``None`` if the backend does not support pulse.
@@ -691,15 +691,15 @@
         """Return the backend configuration.
 
         Backend configuration contains fixed information about the backend, such
         as its name, number of qubits, basis gates, coupling map, quantum volume, etc.
 
         The schema for backend configuration can be found in
         `Qiskit/ibm-quantum-schemas
-        <https://github.com/Qiskit/ibm-quantum-schemas/blob/main/schemas/backend_configuration_schema.json>`_.
+        <https://github.com/Qiskit/ibm-quantum-schemas/blob/main/schemas/backend_configuration_schema.json>`__.
 
         Returns:
             The configuration for the backend.
         """
         return self._configuration
 
     def drive_channel(self, qubit: int) -> DriveChannel:
```

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/ibm_backend_service.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/ibm_backend_service.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/ibm_provider.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/ibm_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/ibm_qubit_properties.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/ibm_qubit_properties.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/job/__init__.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/job/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/job/constants.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/job/constants.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/job/exceptions.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/job/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/job/ibm_circuit_job.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/job/ibm_circuit_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/job/ibm_composite_job.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/job/ibm_composite_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/job/ibm_job.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/job/ibm_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/job/job_monitor.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/job/job_monitor.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/job/queueinfo.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/job/queueinfo.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/job/sub_job.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/job/sub_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/job/utils.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/job/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/__init__.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ========================================
 
 .. jupyter-execute::
     :hide-code:
     :hide-output:
 
     from qiskit_ibm_provider.test.ibm_provider_mock import mock_get_backend
-    mock_get_backend('FakeVigo')
+    mock_get_backend('Fake1Q')
 
 .. jupyter-execute::
 
     from qiskit_ibm_provider import IBMProvider
     import qiskit_ibm_provider.jupyter
 
     provider = IBMProvider(hub='ibm-q')
@@ -67,19 +67,19 @@
 
 """
 import sys
 
 if "ipykernel" in sys.modules:
 
     from IPython import get_ipython  # pylint: disable=import-error
+    from qiskit.providers import BackendV2
     from .dashboard.dashboard import IBMDashboardMagic
-    from qiskit.providers.fake_provider.fake_backend import FakeBackendV2 as FakeBackend
     from ..ibm_backend import IBMBackend
     from .backend_info import backend_widget
 
     _IP = get_ipython()
     if _IP is not None:
         _IP.register_magics(IBMDashboardMagic)
         HTML_FORMATTER = _IP.display_formatter.formatters["text/html"]
         # Make backend_widget the html repr for IBM Quantum backends
         HTML_FORMATTER.for_type(IBMBackend, backend_widget)
-        HTML_FORMATTER.for_type(FakeBackend, backend_widget)
+        HTML_FORMATTER.for_type(BackendV2, backend_widget)
```

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/backend_info.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/backend_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,53 +10,50 @@
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 # pylint: disable=protected-access
 
 """Interactive backend widget."""
 
 import threading
-from typing import Union
 
 import ipyvuetify as vue
 from IPython.display import display  # pylint: disable=import-error
-from qiskit.providers.fake_provider.fake_backend import FakeBackendV2 as FakeBackend
-
+from qiskit.providers import BackendV2
 from qiskit_ibm_provider.ibm_backend import IBMBackend
 from .config_widget import config_tab
 from .gates_widget import gates_tab
 from .jobs_widget import jobs_tab
 from .qubits_widget import qubits_tab
 from ..visualization.interactive import iplot_error_map
 from ..utils.hgp import to_instance_format
 
 
-def _async_job_loader(
-    tab: vue.TabItem, backend: Union[IBMBackend, FakeBackend]
-) -> None:
+def _async_job_loader(tab: vue.TabItem, backend: BackendV2) -> None:
     """Asynchronous job loader.
 
     Args:
         tab: Tab item.
         backend: Backend to use.
     """
     tab.children = [jobs_tab(backend)]
 
 
-def backend_widget(backend: Union[IBMBackend, FakeBackend]) -> None:
+def backend_widget(backend: BackendV2) -> None:
     """Display backend information as a widget.
 
     Args:
         backend: Display information about this backend.
     """
     vue.theme.dark = False
-    if isinstance(backend, FakeBackend):
+    if isinstance(backend, IBMBackend):
+        instance = backend._api_client._params.instance
+    else:
+        # fake backend
         cred = backend._credentials
         instance = to_instance_format(cred.hub, cred.group, cred.project)
-    else:
-        instance = backend._api_client._params.instance
     last_tab = vue.TabItem(children=[])
     card = vue.Card(
         height=600,
         outlined=True,
         children=[
             vue.Toolbar(
                 flat=True,
```

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/config_widget.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/config_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,24 +9,20 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 # pylint: disable=protected-access
 
 """Widget for the backend configuration tab."""
 
-from typing import Union
-
 import ipywidgets as wid
-from qiskit.providers.fake_provider.fake_backend import FakeBackendV2 as FakeBackend
-
-from qiskit_ibm_provider.ibm_backend import IBMBackend
+from qiskit.providers import BackendV2
 from qiskit_ibm_provider.visualization.interactive import iplot_gate_map
 
 
-def config_tab(backend: Union[IBMBackend, FakeBackend]) -> wid.GridBox:
+def config_tab(backend: BackendV2) -> wid.GridBox:
     """The backend configuration widget.
 
     Args:
         backend: Display configuration widget for this backend.
 
     Returns:
         A widget containing backend configuration information.
```

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/dashboard/__init__.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/dashboard/backend_update.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/dashboard/backend_update.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/dashboard/backend_widget.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/dashboard/backend_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/dashboard/constants.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/dashboard/constants.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/dashboard/dashboard.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/dashboard/dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 import threading
 from typing import List, Tuple, Dict, Any, Optional
 
 import ipywidgets as wid
 from IPython.core.magic import line_magic, Magics, magics_class
 from IPython.display import display, Javascript
 from qiskit.exceptions import QiskitError
-from qiskit.tools.events.pubsub import Subscriber
 
 from qiskit_ibm_provider.job.exceptions import IBMJobApiError
 from qiskit_ibm_provider.job.ibm_job import IBMJob
+from qiskit_ibm_provider.utils.pubsub import Subscriber
 from .backend_update import update_backend_info
 from .backend_widget import make_backend_widget
 from .job_widgets import make_clear_button, make_labels, create_job_widget
 from .utils import BackendWithProviders
 from .watcher_monitor import _job_monitor
 from ... import IBMProvider
```

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/dashboard/job_widgets.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/dashboard/job_widgets.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/dashboard/provider_buttons.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/dashboard/provider_buttons.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/dashboard/utils.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/dashboard/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/dashboard/watcher_monitor.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/dashboard/watcher_monitor.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/gates_widget.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/gates_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,23 +10,20 @@
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 # pylint: disable=invalid-name
 
 """Widget for backend gates tab."""
 
 import math
-from typing import Union
 
 import ipywidgets as wid
-from qiskit.providers.fake_provider.fake_backend import FakeBackendV2 as FakeBackend
+from qiskit.providers import BackendV2
 
-from qiskit_ibm_provider.ibm_backend import IBMBackend
 
-
-def gates_tab(backend: Union[IBMBackend, FakeBackend]) -> wid.GridBox:
+def gates_tab(backend: BackendV2) -> wid.GridBox:
     """Construct the multiple qubit gate error widget.
 
     Args:
         backend: The backend to display.
 
     Returns:
         A widget with gate information.
```

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/jobs_widget.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/jobs_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,21 +10,19 @@
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 # pylint: disable=protected-access
 
 """Interactive Jobs widget."""
 
 import datetime
-from typing import Any, Union
+from typing import Any
 
 import ipywidgets as wid
 import plotly.graph_objects as go
-from qiskit.providers.fake_provider.fake_backend import FakeBackendV2 as FakeBackend
-
-from ..ibm_backend import IBMBackend
+from qiskit.providers import BackendV2
 from ..visualization.interactive.plotly_wrapper import PlotlyWidget
 
 MONTH_NAMES = {
     1: "Jan.",
     2: "Feb.",
     3: "Mar.",
     4: "Apr.",
@@ -100,17 +98,15 @@
         else:
             name = jdata[1]
         table_html += _temp_str.format(time=date_str, jid=name, status=jdata[3])
     table_html += table_footer
     return table_html
 
 
-def _job_summary(
-    backend: Union[IBMBackend, FakeBackend], **kwargs: Any
-) -> PlotlyWidget:
+def _job_summary(backend: BackendV2, **kwargs: Any) -> PlotlyWidget:
     """Interactive jobs summary for a backend.
 
     Args:
         backend: Display jobs summary for this backend.
         **kwargs: Used only for testing purposes:
 
             * limit - Number of jobs to retrieve.
@@ -276,15 +272,15 @@
             sun_wid._active = idx
 
     sun = sun_wid.data[0]
     sun.on_click(callback)
     return sun_wid
 
 
-def jobs_tab(backend: Union[IBMBackend, FakeBackend], **kwargs: Any) -> wid.HBox:
+def jobs_tab(backend: BackendV2, **kwargs: Any) -> wid.HBox:
     """Construct a widget containing job information for an input backend.
 
     Args:
         backend: Input backend.
         **kwargs: Used only for testing purposes:
 
             * limit - Number of jobs to retrieve.
```

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/jupyter/qubits_widget.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/jupyter/qubits_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,23 +9,19 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 # pylint: disable=invalid-name
 
 """Widget for qubit properties tab."""
 
-from typing import Union
-
 import ipywidgets as wid
-from qiskit.providers.fake_provider.fake_backend import FakeBackendV2 as FakeBackend
-
-from qiskit_ibm_provider.ibm_backend import IBMBackend
+from qiskit.providers import BackendV2
 
 
-def qubits_tab(backend: Union[IBMBackend, FakeBackend]) -> wid.VBox:
+def qubits_tab(backend: BackendV2) -> wid.VBox:
     """The qubit properties widget.
 
     Args:
         backend: Display qubit properties for this backend.
 
     Returns:
         A widget containing qubit information.
```

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/proxies/__init__.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/proxies/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/proxies/configuration.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/proxies/configuration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/qpy/__init__.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/qpy/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/qpy/binary_io/__init__.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/qpy/binary_io/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/qpy/binary_io/circuits.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/qpy/binary_io/circuits.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,25 +20,23 @@
 import uuid
 import warnings
 
 from collections import defaultdict
 import numpy as np
 
 from qiskit import circuit as circuit_mod
-from qiskit import extensions
 from qiskit.circuit import library, controlflow, CircuitInstruction, ControlFlowOp
 from qiskit.circuit.classical import expr
 from qiskit.circuit.classicalregister import ClassicalRegister, Clbit
 from qiskit.circuit.gate import Gate
 from qiskit.circuit.singleton import SingletonInstruction, SingletonGate
 from qiskit.circuit.controlledgate import ControlledGate
 from qiskit.circuit.instruction import Instruction
 from qiskit.circuit.quantumcircuit import QuantumCircuit
 from qiskit.circuit.quantumregister import QuantumRegister, Qubit
-from qiskit.extensions import quantum_initializer
 from qiskit.quantum_info.operators import SparsePauliOp
 from qiskit.synthesis import evolution as evo_synth
 from qiskit.transpiler.layout import Layout, TranspileLayout
 from .. import common, formats, type_keys
 from . import value, schedules
 
 
@@ -303,18 +301,14 @@
             return inst_obj
         circuit._append(inst_obj, qargs, cargs)
         return None
     elif hasattr(library, gate_name):
         gate_class = getattr(library, gate_name)
     elif hasattr(circuit_mod, gate_name):
         gate_class = getattr(circuit_mod, gate_name)
-    elif hasattr(extensions, gate_name):
-        gate_class = getattr(extensions, gate_name)
-    elif hasattr(quantum_initializer, gate_name):
-        gate_class = getattr(quantum_initializer, gate_name)
     elif hasattr(controlflow, gate_name):
         gate_class = getattr(controlflow, gate_name)
     else:
         raise AttributeError("Invalid instruction type: %s" % gate_name)
 
     if instruction.label_size <= 0:
         label = None
@@ -633,16 +627,14 @@
 ):
     gate_class_name = instruction.operation.base_class.__name__
     custom_operations_list = []
     if (
         (
             not hasattr(library, gate_class_name)
             and not hasattr(circuit_mod, gate_class_name)
-            and not hasattr(extensions, gate_class_name)
-            and not hasattr(quantum_initializer, gate_class_name)
             and not hasattr(controlflow, gate_class_name)
         )
         or gate_class_name == "Gate"
         or gate_class_name == "Instruction"
         or isinstance(instruction.operation, library.BlueprintCircuit)
     ):
         if instruction.operation.name not in custom_operations:
```

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/qpy/binary_io/schedules.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/qpy/binary_io/schedules.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/qpy/binary_io/value.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/qpy/binary_io/value.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/qpy/common.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/qpy/common.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/qpy/exceptions.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/qpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/qpy/formats.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/qpy/formats.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/qpy/interface.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/qpy/interface.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/qpy/type_keys.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/qpy/type_keys.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/session.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,32 +28,38 @@
     Data used within a session, such as transpiled circuits, is also cached to avoid
     unnecessary overhead.
 
     You can open a Qiskit Runtime session using this ``Session`` class
     and submit one or more jobs.
 
     For example::
-
-        from qiskit.test.reference_circuits import ReferenceCircuits
         from qiskit_ibm_provider import IBMProvider
 
-        circ = ReferenceCircuits.bell()
+        # Bell Circuit
+        qr = QuantumRegister(2, name="qr")
+        cr = ClassicalRegister(2, name="cr")
+        qc = QuantumCircuit(qr, cr, name="bell")
+        qc.h(qr[0])
+        qc.cx(qr[0], qr[1])
+        qc.measure(qr, cr)
+
         backend = IBMProvider().get_backend("ibmq_qasm_simulator")
         backend.open_session()
-        job = backend.run(circ)
+
+        job = backend.run(qc)
         print(f"Job ID: {job.job_id()}")
         print(f"Result: {job.result()}")
         # Close the session only if all jobs are finished and
         # you don't need to run more in the session.
         backend.cancel_session()
 
     Session can also be used as a context manager::
 
         with backend.open_session() as session:
-            job = backend.run(ReferenceCircuits.bell())
+            job = backend.run(qc)
             assert job.job_id() == session.session_id
 
     """
 
     def __init__(
         self,
         max_time: Optional[Union[int, str]] = None,
```

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/transpiler/__init__.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/transpiler/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/transpiler/passes/__init__.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/transpiler/passes/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/transpiler/passes/basis/__init__.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/transpiler/passes/basis/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/transpiler/passes/basis/convert_id_to_delay.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/transpiler/passes/basis/convert_id_to_delay.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/transpiler/passes/scheduling/__init__.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/transpiler/passes/scheduling/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,26 +29,36 @@
     :func:`~qiskit.compiler.transpile` or
     :func:`~qiskit.transpiler.preset_passmanagers.generate_preset_pass_manager`.
 
 Below we demonstrate how to schedule and pad a teleportation circuit with delays
 for a dynamic circuit backend's execution model:
 
 .. jupyter-execute::
+    :hide-code:
+    :hide-output:
+
+    import warnings
+    warnings.filterwarnings("ignore", category=DeprecationWarning)
+
+.. jupyter-execute::
 
     from qiskit.circuit import ClassicalRegister, QuantumCircuit, QuantumRegister
     from qiskit.transpiler.preset_passmanagers import generate_preset_pass_manager
     from qiskit.transpiler.passmanager import PassManager
 
     from qiskit_ibm_provider.transpiler.passes.scheduling import DynamicCircuitInstructionDurations
     from qiskit_ibm_provider.transpiler.passes.scheduling import ALAPScheduleAnalysis
     from qiskit_ibm_provider.transpiler.passes.scheduling import PadDelay
-    from qiskit.providers.fake_provider import FakeJakarta
+    try:
+        from qiskit.providers.fake_provider import Fake7QPulseV1
+    except ImportError:
+        from qiskit.providers.fake_provider import FakeJakarta as Fake7QPulseV1
 
 
-    backend = FakeJakarta()
+    backend = Fake7QPulseV1()
 
     # Temporary workaround for mock backends. For real backends this is not required.
     backend.configuration().basis_gates.append("if_else")
 
 
     # Use this duration class to get appropriate durations for dynamic
     # circuit backend scheduling
```

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/transpiler/passes/scheduling/block_base_padder.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/transpiler/passes/scheduling/block_base_padder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/transpiler/passes/scheduling/dynamical_decoupling.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/transpiler/passes/scheduling/dynamical_decoupling.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,22 +19,26 @@
 import rustworkx as rx
 from qiskit.circuit import Qubit, Gate
 from qiskit.circuit.delay import Delay
 from qiskit.circuit.library.standard_gates import IGate, UGate, U3Gate
 from qiskit.circuit.reset import Reset
 from qiskit.dagcircuit import DAGCircuit, DAGNode, DAGInNode, DAGOpNode
 from qiskit.quantum_info.operators.predicates import matrix_equal
-from qiskit.quantum_info.synthesis import OneQubitEulerDecomposer
 from qiskit.transpiler.exceptions import TranspilerError
 from qiskit.transpiler.instruction_durations import InstructionDurations
 from qiskit.transpiler.passes.optimization import Optimize1qGates
 from qiskit.transpiler import CouplingMap
 
 from .block_base_padder import BlockBasePadder
 
+try:
+    from qiskit.quantum_info.synthesis import OneQubitEulerDecomposer
+except ImportError:
+    from qiskit.synthesis import OneQubitEulerDecomposer
+
 
 class PadDynamicalDecoupling(BlockBasePadder):
     """Dynamical decoupling insertion pass for IBM dynamic circuit backends.
 
     This pass works on a scheduled, physical circuit. It scans the circuit for
     idle periods of time (i.e. those containing delay instructions) and inserts
     a DD sequence of gates in those spots. These gates amount to the identity,
@@ -325,15 +329,19 @@
             # Precompute qubit-wise DD sequence length for performance
             for qubit in dag.qubits:
                 seq_length_ = []
                 if qubit not in self._dd_sequence_lengths:
                     self._dd_sequence_lengths[qubit] = []
 
                 physical_index = dag.qubits.index(qubit)
-                if self._qubits and physical_index not in self._qubits:
+                if (
+                    self._qubits
+                    and physical_index not in self._qubits
+                    or qubit in self._idle_qubits
+                ):
                     continue
 
                 for index, gate in enumerate(seq):
                     try:
                         # Check calibration.
                         gate_length = dag.calibrations[gate.name][
                             (physical_index, gate.params)
```

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/transpiler/passes/scheduling/pad_delay.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/transpiler/passes/scheduling/pad_delay.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/transpiler/passes/scheduling/scheduler.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/transpiler/passes/scheduling/scheduler.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/transpiler/passes/scheduling/utils.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/transpiler/passes/scheduling/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 
 from qiskit.circuit import ControlFlowOp, Measure, Reset, Parameter
 from qiskit.dagcircuit import DAGCircuit, DAGOpNode
 from qiskit.transpiler.instruction_durations import (
     InstructionDurations,
     InstructionDurationsType,
 )
+from qiskit.transpiler.target import Target
 from qiskit.transpiler.exceptions import TranspilerError
+from qiskit.providers import Backend, BackendV1
 
 
 def block_order_op_nodes(dag: DAGCircuit) -> Generator[DAGOpNode, None, None]:
     """Yield nodes such that they are sorted into groups of blocks that minimize synchronization.
 
     Measurements are also grouped.
     """
@@ -146,14 +148,91 @@
         dt: float = None,
         enable_patching: bool = True,
     ):
         """Dynamic circuit instruction durations."""
         self._enable_patching = enable_patching
         super().__init__(instruction_durations=instruction_durations, dt=dt)
 
+    @classmethod
+    def from_backend(cls, backend: Backend) -> "DynamicCircuitInstructionDurations":
+        """Construct a :class:`DynamicInstructionDurations` object from the backend.
+
+        Args:
+            backend: backend from which durations (gate lengths) and dt are extracted.
+
+        Returns:
+            DynamicInstructionDurations: The InstructionDurations constructed from backend.
+        """
+        if isinstance(backend, BackendV1):
+            # TODO Remove once https://github.com/Qiskit/qiskit/pull/11727 gets released in qiskit 0.46.1
+            # From here ---------------------------------------
+            def patch_from_backend(cls, backend: Backend):  # type: ignore
+                """
+                REMOVE me once https://github.com/Qiskit/qiskit/pull/11727 gets released in qiskit 0.46.1
+                """
+                instruction_durations = []
+                backend_properties = backend.properties()
+                if hasattr(backend_properties, "_gates"):
+                    for gate, insts in backend_properties._gates.items():
+                        for qubits, props in insts.items():
+                            if "gate_length" in props:
+                                gate_length = props["gate_length"][
+                                    0
+                                ]  # Throw away datetime at index 1
+                                instruction_durations.append(
+                                    (gate, qubits, gate_length, "s")
+                                )
+                    for (
+                        q,  # pylint: disable=invalid-name
+                        props,
+                    ) in backend.properties()._qubits.items():
+                        if "readout_length" in props:
+                            readout_length = props["readout_length"][
+                                0
+                            ]  # Throw away datetime at index 1
+                            instruction_durations.append(
+                                ("measure", [q], readout_length, "s")
+                            )
+                try:
+                    dt = backend.configuration().dt
+                except AttributeError:
+                    dt = None
+
+                return cls(instruction_durations, dt=dt)
+
+            return patch_from_backend(DynamicCircuitInstructionDurations, backend)
+            # To here --------------------------------------- (remove comment ignore annotations too)
+            return super(  # type: ignore  # pylint: disable=unreachable
+                DynamicCircuitInstructionDurations, cls
+            ).from_backend(backend)
+
+        # Get durations from target if BackendV2
+        return cls.from_target(backend.target)
+
+    @classmethod
+    def from_target(cls, target: Target) -> "DynamicCircuitInstructionDurations":
+        """Construct a :class:`DynamicInstructionDurations` object from the target.
+
+        Args:
+            target: target from which durations (gate lengths) and dt are extracted.
+
+        Returns:
+            DynamicInstructionDurations: The InstructionDurations constructed from backend.
+        """
+
+        instruction_durations_dict = target.durations().duration_by_name_qubits
+        instruction_durations = []
+        for instr_key, instr_value in instruction_durations_dict.items():
+            instruction_durations += [(*instr_key, *instr_value)]
+        try:
+            dt = target.dt
+        except AttributeError:
+            dt = None
+        return cls(instruction_durations, dt=dt)
+
     def update(
         self, inst_durations: Optional[InstructionDurationsType], dt: float = None
     ) -> "DynamicCircuitInstructionDurations":
         """Update self with inst_durations (inst_durations overwrite self). Overrides the default
         durations for certain hardcoded instructions.
 
         Args:
@@ -202,62 +281,61 @@
         """Dispatcher logic for instruction patches"""
         name = key[0]
         if name == "measure":
             self._patch_measurement(key)
         elif name == "reset":
             self._patch_reset(key)
 
+    def _convert_and_patch_key(self, key: InstrKey) -> None:
+        """Convert duration to dt and patch key"""
+        prev_duration, unit = self._get_duration(key)
+        if unit != "dt":
+            prev_duration = self._convert_unit(prev_duration, unit, "dt")
+            # raise TranspilerError('Can currently only patch durations of "dt".')
+        odd_cycle_correction = self._get_odd_cycle_correction()
+        new_duration = prev_duration + self.MEASURE_PATCH_CYCLES + odd_cycle_correction
+        if unit != "dt":  # convert back to original unit
+            new_duration = self._convert_unit(new_duration, "dt", unit)
+        self._patch_key(key, new_duration, unit)
+
     def _patch_measurement(self, key: InstrKey) -> None:
         """Patch measurement duration by extending duration by 160dt as temporarily
         required by the dynamic circuit backend.
         """
-        prev_duration, unit = self._get_duration_dt(key)
-        if unit != "dt":
-            raise TranspilerError('Can currently only patch durations of "dt".')
-        odd_cycle_correction = self._get_odd_cycle_correction()
-        self._patch_key(
-            key, prev_duration + self.MEASURE_PATCH_CYCLES + odd_cycle_correction, unit
-        )
+        self._convert_and_patch_key(key)
         # Enforce patching of reset on measurement update
         self._patch_reset(("reset", key[1], key[2]))
 
     def _patch_reset(self, key: InstrKey) -> None:
         """Patch reset duration by extending duration by measurement patch as temporarily
         required by the dynamic circuit backend.
         """
         # We patch the reset to be the duration of the measurement if it
         # is available as it currently
         # triggers the end of scheduling after the measurement pulse
         measure_key = ("measure", key[1], key[2])
         try:
-            measure_duration, unit = self._get_duration_dt(measure_key)
+            measure_duration, unit = self._get_duration(measure_key)
             self._patch_key(key, measure_duration, unit)
         except KeyError:
             # Fall back to reset key if measure not available
-            prev_duration, unit = self._get_duration_dt(key)
-            if unit != "dt":
-                raise TranspilerError('Can currently only patch durations of "dt".')
-            odd_cycle_correction = self._get_odd_cycle_correction()
-            self._patch_key(
-                key,
-                prev_duration + self.MEASURE_PATCH_CYCLES + odd_cycle_correction,
-                unit,
-            )
+            self._convert_and_patch_key(key)
 
-    def _get_duration_dt(self, key: InstrKey) -> Tuple[int, str]:
+    def _get_duration(self, key: InstrKey) -> Tuple[int, str]:
         """Handling for the complicated structure of this class.
 
         TODO: This class implementation should be simplified in Qiskit. Too many edge cases.
         """
         if key[1] is None and key[2] is None:
-            return self.duration_by_name[key[0]]
+            duration = self.duration_by_name[key[0]]
         elif key[2] is None:
-            return self.duration_by_name_qubits[(key[0], key[1])]
-
-        return self.duration_by_name_qubits_params[key]
+            duration = self.duration_by_name_qubits[(key[0], key[1])]
+        else:
+            duration = self.duration_by_name_qubits_params[key]
+        return duration
 
     def _patch_key(self, key: InstrKey, duration: int, unit: str) -> None:
         """Handling for the complicated structure of this class.
 
         TODO: This class implementation should be simplified in Qiskit. Too many edge cases.
         """
         if key[1] is None and key[2] is None:
```

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/transpiler/plugin.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/transpiler/plugin.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/utils/__init__.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/utils/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,17 +31,22 @@
 ==============
 .. autosummary::
     :toctree: ../stubs/
 
     to_python_identifier
     validate_job_tags
 
+Publisher/subscriber model
+==========================
+
+.. automodule:: qiskit_ibm_provider.utils.pubsub
 """
 
 from .converters import (
     utc_to_local,
     local_to_utc,
     seconds_to_duration,
     duration_difference,
 )
 from .utils import to_python_identifier, validate_job_tags, are_circuits_dynamic
 from .json import RuntimeEncoder, RuntimeDecoder
+from . import pubsub
```

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/utils/backend_decoder.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/utils/backend_decoder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/utils/converters.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/utils/converters.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/utils/hgp.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/utils/hgp.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/utils/json.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/utils/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,26 +51,25 @@
     ParameterExpression,
     ParameterVector,
     QuantumCircuit,
     QuantumRegister,
 )
 from qiskit.result import Result
 from qiskit.version import __version__ as _terra_version_string
-from qiskit.qpy import load
 from qiskit.utils import optionals
 
-from ..qpy import (
-    _write_parameter,
+from qiskit.qpy import (
     _write_parameter_expression,
     _read_parameter_expression,
     _read_parameter_expression_v3,
-    _read_parameter,
+    load,
     dump,
 )
 
+from qiskit.qpy.binary_io.value import _write_parameter, _read_parameter
 
 _TERRA_VERSION = tuple(
     int(x)
     for x in re.match(r"\d+\.\d+\.\d", _terra_version_string).group(0).split(".")[:3]
 )
 
 
@@ -220,18 +219,23 @@
         if isinstance(obj, set):
             return {"__type__": "set", "__value__": list(obj)}
         if isinstance(obj, Result):
             return {"__type__": "Result", "__value__": obj.to_dict()}
         if hasattr(obj, "to_json"):
             return {"__type__": "to_json", "__value__": obj.to_json()}
         if isinstance(obj, QuantumCircuit):
+            kwargs: Dict[str, object] = {"use_symengine": bool(optionals.HAS_SYMENGINE)}
+            if _TERRA_VERSION[0] >= 1:
+                # NOTE: This can be updated only after the server side has
+                # updated to a newer qiskit version.
+                kwargs["version"] = 10
             value = _serialize_and_encode(
                 data=obj,
                 serializer=lambda buff, data: dump(
-                    data, buff, RuntimeEncoder, use_symengine=optionals.HAS_SYMENGINE
+                    data, buff, RuntimeEncoder, **kwargs
                 ),  # type: ignore[no-untyped-call]
             )
             return {"__type__": "QuantumCircuit", "__value__": value}
         if isinstance(obj, Parameter):
             value = _serialize_and_encode(
                 data=obj,
                 serializer=_write_parameter,
@@ -239,25 +243,31 @@
             )
             return {"__type__": "Parameter", "__value__": value}
         if isinstance(obj, ParameterExpression):
             value = _serialize_and_encode(
                 data=obj,
                 serializer=_write_parameter_expression,
                 compress=False,
+                use_symengine=bool(optionals.HAS_SYMENGINE),
             )
             return {"__type__": "ParameterExpression", "__value__": value}
         if isinstance(obj, Instruction):
+            kwargs = {"use_symengine": bool(optionals.HAS_SYMENGINE)}
+            if _TERRA_VERSION[0] >= 1:
+                # NOTE: This can be updated only after the server side has
+                # updated to a newer qiskit version.
+                kwargs["version"] = 10
             # Append instruction to empty circuit
             quantum_register = QuantumRegister(obj.num_qubits)
             quantum_circuit = QuantumCircuit(quantum_register)
             quantum_circuit.append(obj, quantum_register)
             value = _serialize_and_encode(
                 data=quantum_circuit,
                 serializer=lambda buff, data: dump(
-                    data, buff, use_symengine=optionals.HAS_SYMENGINE
+                    data, buff, **kwargs
                 ),  # type: ignore[no-untyped-call]
             )
             return {"__type__": "Instruction", "__value__": value}
         if HAS_AER and isinstance(obj, qiskit_aer.noise.NoiseModel):
             return {"__type__": "NoiseModel", "__value__": obj.to_dict()}
         if hasattr(obj, "settings"):
             return {
```

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/utils/json_decoder.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/utils/json_decoder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/utils/json_encoder.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/utils/options.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/utils/options.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/utils/qobj_utils.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/utils/qobj_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/utils/utils.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/version.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/visualization/__init__.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/visualization/colormaps.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/visualization/colormaps.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/visualization/device_layouts.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/visualization/device_layouts.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/visualization/exceptions.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/visualization/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/visualization/interactive/__init__.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/visualization/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/visualization/interactive/error_map.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/visualization/interactive/error_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,23 +56,28 @@
 
     Example:
         .. jupyter-execute::
             :hide-code:
             :hide-output:
 
             from qiskit_ibm_provider.test.ibm_provider_mock import mock_get_backend
-            mock_get_backend('FakeVigo')
+            # Generate a mock provider for the sake of this example.
+            # This line will allow the mocked ``IBMProvider`` to return
+            # a fake backend in the following cell.
+            mock_get_backend('FakeOpenPulse2Q')
 
         .. jupyter-execute::
 
            from qiskit_ibm_provider import IBMProvider
            from qiskit_ibm_provider.visualization import iplot_error_map
 
            provider = IBMProvider(group='open', project='main')
-           backend = provider.get_backend('ibmq_vigo')
+           # Note that this is a mock provider, replace ``FakeOpenPulse2Q``
+           # with any of the currently available IBM devices.
+           backend = provider.get_backend('FakeOpenPulse2Q')
 
            iplot_error_map(backend, as_widget=True)
     """
     meas_text_color = "#000000"
     if background_color == "white":
         color_map = HELIX_LIGHT_CMAP
         text_color = "#000000"
```

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/visualization/interactive/gate_map.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/visualization/interactive/gate_map.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,23 +60,28 @@
     Example:
 
         .. jupyter-execute::
             :hide-code:
             :hide-output:
 
             from qiskit_ibm_provider.test.ibm_provider_mock import mock_get_backend
-            mock_get_backend('FakeVigo')
+            # Generate a mock provider for the sake of this example.
+            # This line will allow the mocked ``IBMProvider`` to return
+            # a fake backend in the following cell.
+            mock_get_backend('FakeOpenPulse2Q')
 
         .. jupyter-execute::
 
             from qiskit_ibm_provider import IBMProvider
             from qiskit_ibm_provider.visualization import iplot_gate_map
 
-            provider = IBMProvider(group='open', project='main')
-            backend = provider.get_backend('ibmq_vigo')
+           provider = IBMProvider(group='open', project='main')
+           # Note that this is a mock provider, replace ``FakeOpenPulse2Q``
+           # with any of the currently available IBM devices.
+           backend = provider.get_backend('FakeOpenPulse2Q')
 
             iplot_gate_map(backend, as_widget=True)
     """
 
     config = backend.configuration()
     n_qubits = config.n_qubits
     cmap = config.coupling_map
```

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider/visualization/interactive/plotly_wrapper.py` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider/visualization/interactive/plotly_wrapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider.egg-info/PKG-INFO` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ibm-provider
-Version: 0.8.0
+Version: 0.9.0
 Summary: Qiskit IBM Quantum Provider for accessing the quantum devices and simulators at IBM
 Home-page: https://github.com/Qiskit/qiskit-ibm-provider
 Author: Qiskit Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-ibm-provider/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
@@ -119,15 +119,15 @@
 from qiskit_ibm_provider import IBMProvider
 provider = IBMProvider(token='MY_API_TOKEN')
 ```
 
 ## Next Steps
 
 Now you're set up and ready to check out some of the tutorials.
-- [Qiskit IBM Provider]
+- [IBM Quantum Learning]
 - [Qiskit]
 
 ## Contribution Guidelines
 
 If you'd like to contribute to qiskit-ibm-provider, please take a look at our
 [contribution guidelines]. This project adheres to Qiskit's [code of conduct].
 By participating, you are expect to uphold to this code.
@@ -155,12 +155,12 @@
 [code of conduct]: https://github.com/Qiskit/qiskit-ibm-provider/blob/main/CODE_OF_CONDUCT.md
 [GitHub issues]: https://github.com/Qiskit/qiskit-ibm-provider/issues
 [slack]: https://qiskit.slack.com
 [Qiskit.org]: https://qiskit.org
 [Stack Exchange]: https://quantumcomputing.stackexchange.com/questions/tagged/qiskit
 [Qiskit Tutorial]: https://github.com/Qiskit/qiskit-tutorial
 [many people]: https://github.com/Qiskit/qiskit-ibm-provider/graphs/contributors
-[Qiskit IBM Provider]: https://github.com/Qiskit/qiskit-ibm-provider/tree/main/docs/tutorials
+[IBM Quantum Learning]: https://learning.quantum.ibm.com/catalog/tutorials
 [Qiskit]: https://github.com/Qiskit/qiskit-tutorial
 [BibTeX file]: https://github.com/Qiskit/qiskit/blob/master/Qiskit.bib
 [Apache License 2.0]: https://github.com/Qiskit/qiskit-ibm-provider/blob/main/LICENSE.txt
 [migration guide]: https://github.com/Qiskit/qiskit-ibm-provider/blob/6be5f3297ede75bb062b20601058b55a397668e3/docs/tutorials/Migration_Guide_from_qiskit-ibmq-provider.ipynb
```

### Comparing `qiskit-ibm-provider-0.8.0/qiskit_ibm_provider.egg-info/SOURCES.txt` & `qiskit-ibm-provider-0.9.0/qiskit_ibm_provider.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -102,14 +102,15 @@
 qiskit_ibm_provider/utils/backend_decoder.py
 qiskit_ibm_provider/utils/converters.py
 qiskit_ibm_provider/utils/hgp.py
 qiskit_ibm_provider/utils/json.py
 qiskit_ibm_provider/utils/json_decoder.py
 qiskit_ibm_provider/utils/json_encoder.py
 qiskit_ibm_provider/utils/options.py
+qiskit_ibm_provider/utils/pubsub.py
 qiskit_ibm_provider/utils/qobj_utils.py
 qiskit_ibm_provider/utils/utils.py
 qiskit_ibm_provider/visualization/__init__.py
 qiskit_ibm_provider/visualization/colormaps.py
 qiskit_ibm_provider/visualization/device_layouts.py
 qiskit_ibm_provider/visualization/exceptions.py
 qiskit_ibm_provider/visualization/interactive/__init__.py
@@ -130,15 +131,14 @@
 test/e2e/__init__.py
 test/e2e/test_real_devices.py
 test/e2e/test_tutorials.py
 test/integration/__init__.py
 test/integration/test_account_client.py
 test/integration/test_backend.py
 test/integration/test_basic_server_paths.py
-test/integration/test_composite_job.py
 test/integration/test_filter_backends.py
 test/integration/test_ibm_integration.py
 test/integration/test_ibm_job.py
 test/integration/test_ibm_job_attributes.py
 test/integration/test_ibm_provider.py
 test/integration/test_ibm_qasm_simulator.py
 test/integration/test_jupyter.py
@@ -159,12 +159,11 @@
 test/unit/mock/fake_account_client.py
 test/unit/mock/fake_provider.py
 test/unit/transpiler/__init__.py
 test/unit/transpiler/passes/__init__.py
 test/unit/transpiler/passes/basis/__init__.py
 test/unit/transpiler/passes/basis/test_convert_id_to_delay.py
 test/unit/transpiler/passes/scheduling/__init__.py
-test/unit/transpiler/passes/scheduling/control_flow_test_case.py
 test/unit/transpiler/passes/scheduling/test_dynamical_decoupling.py
 test/unit/transpiler/passes/scheduling/test_scheduler.py
 test/unit/transpiler/passes/scheduling/test_utils.py
 test/unit/utils/ws_handler.py
```

### Comparing `qiskit-ibm-provider-0.8.0/setup.cfg` & `qiskit-ibm-provider-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/setup.py` & `qiskit-ibm-provider-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/test/__init__.py` & `qiskit-ibm-provider-0.9.0/test/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/test/account.py` & `qiskit-ibm-provider-0.9.0/test/account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/test/contextmanagers.py` & `qiskit-ibm-provider-0.9.0/test/contextmanagers.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/test/decorators.py` & `qiskit-ibm-provider-0.9.0/test/decorators.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/test/e2e/test_real_devices.py` & `qiskit-ibm-provider-0.9.0/test/e2e/test_real_devices.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,25 +18,21 @@
 
 from qiskit import (
     transpile,
     ClassicalRegister,
     QuantumCircuit,
     QuantumRegister,
 )
-from qiskit.test.reference_circuits import ReferenceCircuits
 from qiskit.providers.jobstatus import JobStatus
 from qiskit_ibm_provider.job.exceptions import IBMJobFailureError
 
 from qiskit_ibm_provider.ibm_backend import IBMBackend, QOBJRUNNERPROGRAMID
 
 from ..ibm_test_case import IBMTestCase
-from ..utils import (
-    cancel_job,
-    submit_job_one_bad_instr,
-)
+from ..utils import cancel_job, submit_job_one_bad_instr, bell
 from ..decorators import (
     IntegrationTestDependencies,
     integration_test_setup_with_backend,
 )
 
 
 class TestRealDevices(IBMTestCase):
@@ -59,15 +55,15 @@
                 raise self.skipTest("Skip test because there is no private provider")
             backend = self.dependencies[provider].backends(
                 simulator=False,
                 operational=True,
                 filters=lambda b: b.configuration().n_qubits >= 5,
             )[0]
             with self.subTest(provider=provider, backend=backend):
-                job = self._submit_job_with_retry(ReferenceCircuits.bell(), backend)
+                job = self._submit_job_with_retry(bell(), backend)
 
                 # Fetch the results.
                 result = job.result()
                 self.assertTrue(result.success)
 
                 # Fetch the circuits.
                 circuit = (
@@ -84,34 +80,34 @@
                 raise self.skipTest("Skip test because there is no private provider")
             backend = self.dependencies[provider].backends(
                 simulator=False,
                 operational=True,
                 filters=lambda b: b.configuration().n_qubits >= 5,
             )[0]
             with self.subTest(backend=backend):
-                job = self._submit_job_with_retry(ReferenceCircuits.bell(), backend)
+                job = self._submit_job_with_retry(bell(), backend)
                 self.assertIsNotNone(job.properties())
                 self.assertTrue(job.status())
                 # Cancel job so it doesn't consume more resources.
                 cancel_job(job, verify=True)
 
     def test_run_device(self):
         """Test running in a real device."""
         shots = 8192
         job = self.real_device_backend.run(
-            transpile(ReferenceCircuits.bell(), backend=self.real_device_backend),
+            transpile(bell(), backend=self.real_device_backend),
             shots=shots,
             program_id=QOBJRUNNERPROGRAMID,
         )
 
         job.wait_for_final_state()
         result = job.result()
         counts_qx = result.get_counts(0)
         counts_ex = {"00": shots / 2, "11": shots / 2}
-        self.assertDictAlmostEqual(counts_qx, counts_ex, shots * 0.2)
+        self.assert_dict_almost_equal(counts_qx, counts_ex, shots * 0.2)
 
     def test_run_multiple_device(self):
         """Test running multiple jobs in a real device."""
 
         backend = self.real_device_backend
         num_qubits = 5
         quantum_register = QuantumRegister(num_qubits, "qr")
@@ -193,15 +189,15 @@
         self.assertTrue(custom_header.items() <= job.header().items())
         self.assertTrue(custom_header.items() <= result.header.to_dict().items())
         # self.assertEqual(result.results[0].header.some_field, 'extra info')
 
     def test_websockets_device(self):
         """Test checking status of a job via websockets for a device."""
         job = self.real_device_backend.run(
-            transpile(ReferenceCircuits.bell(), self.real_device_backend), shots=1
+            transpile(bell(), self.real_device_backend), shots=1
         )
 
         # Manually disable the non-websocket polling.
         # job._api_client._job_final_status_polling = self._job_final_status_polling
         job.wait_for_final_state()
         result = job.result()
```

### Comparing `qiskit-ibm-provider-0.8.0/test/e2e/test_tutorials.py` & `qiskit-ibm-provider-0.9.0/test/e2e/test_tutorials.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/test/fake_account_client.py` & `qiskit-ibm-provider-0.9.0/test/fake_account_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,18 @@
 import uuid
 import warnings
 from concurrent.futures import ThreadPoolExecutor, wait
 from datetime import timedelta, datetime
 from random import randrange
 from typing import Dict, Any
 
-from qiskit.providers.fake_provider.backends.poughkeepsie.fake_poughkeepsie import (
-    FakePoughkeepsie,
-)
+try:
+    from qiskit.providers.fake_provider import Fake20QV1
+except ImportError:
+    from qiskit.providers.fake_provider import FakePoughkeepsie as Fake20QV1
 
 from qiskit_ibm_provider.api.exceptions import (
     RequestsApiError,
     UserTimeoutExceededError,
 )
 from qiskit_ibm_provider.apiconstants import ApiJobStatus, API_JOB_FINAL_STATES
 
@@ -448,15 +449,15 @@
                 if status is ApiJobStatus.QUEUED:
                     data["infoQueue"] = {"status": "PENDING_IN_QUEUE", "position": 1}
                 _kwargs["status_queue"].put(status_data)
         return self.job_status(job_id)
 
     def job_properties(self, *_args, **_kwargs):
         """Return the backend properties of a job."""
-        props = FakePoughkeepsie().properties().to_dict()
+        props = Fake20QV1().properties().to_dict()
         if self._props_count > 0:
             self._props_count -= 1
             new_dt = datetime.now() + timedelta(hours=randrange(300))
             self._props_date = new_dt.isoformat()
         props["last_update_date"] = self._props_date
         return props
```

### Comparing `qiskit-ibm-provider-0.8.0/test/http_server.py` & `qiskit-ibm-provider-0.9.0/test/http_server.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/test/integration/test_account_client.py` & `qiskit-ibm-provider-0.9.0/test/integration/test_account_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/test/integration/test_backend.py` & `qiskit-ibm-provider-0.9.0/test/integration/test_backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 
 from unittest import mock, skip
 from unittest.mock import patch
 
 from qiskit import QuantumCircuit, transpile
 from qiskit.providers.models import QasmBackendConfiguration
 from qiskit.providers.exceptions import QiskitBackendNotFoundError
-from qiskit.test.reference_circuits import ReferenceCircuits
 
 from qiskit_ibm_provider import IBMBackend, IBMProvider
 from qiskit_ibm_provider.ibm_qubit_properties import IBMQubitProperties
 from qiskit_ibm_provider.exceptions import IBMBackendValueError
 
 from ..decorators import (
     IntegrationTestDependencies,
     integration_test_setup_with_backend,
     production_only,
 )
 from ..ibm_test_case import IBMTestCase
+from ..utils import bell
 
 
 class TestIBMBackend(IBMTestCase):
     """Test ibm_backend module."""
 
     @classmethod
     @integration_test_setup_with_backend(simulator=False, min_num_qubits=2)
@@ -87,29 +87,29 @@
 
     def test_sim_backend_options(self):
         """Test simulator backend options."""
         provider: IBMProvider = self.backend.provider
         backend = provider.get_backend("ibmq_qasm_simulator")
         backend.options.shots = 2048
         backend.set_options(memory=True)
-        job = backend.run(ReferenceCircuits.bell(), shots=1024, foo="foo")
+        job = backend.run(bell(), shots=1024, foo="foo")
         backend_options = provider.backend.retrieve_job(job.job_id()).backend_options()
         self.assertEqual(backend_options["shots"], 1024)
         self.assertTrue(backend_options["memory"])
         self.assertEqual(backend_options["foo"], "foo")
 
     @production_only
     def test_paused_backend_warning(self):
         """Test that a warning is given when running jobs on a paused backend."""
         backend = self.dependencies.provider.get_backend("ibmq_qasm_simulator")
         paused_status = backend.status()
         paused_status.status_msg = "internal"
         backend.status = mock.MagicMock(return_value=paused_status)
         with self.assertWarns(Warning):
-            backend.run(ReferenceCircuits.bell())
+            backend.run(bell())
 
     def test_deprecate_id_instruction(self):
         """Test replacement of 'id' Instructions with 'Delay' instructions."""
 
         circuit_with_id = QuantumCircuit(2)
         circuit_with_id.id(0)
         circuit_with_id.id(0)
@@ -182,11 +182,11 @@
         self.assertIn(
             f"Circuit contains {num_qubits} qubits, but backend has only {num}.",
             str(err.exception),
         )
 
     def test_job_backend_properties(self):
         """Test job backend properties."""
-        job = self.backend.run(ReferenceCircuits.bell())
+        job = self.backend.run(bell())
         backend_version = self.backend.properties().backend_version
         job_version = job.properties().backend_version
         self.assertEqual(job_version, backend_version)
```

### Comparing `qiskit-ibm-provider-0.8.0/test/integration/test_basic_server_paths.py` & `qiskit-ibm-provider-0.9.0/test/integration/test_basic_server_paths.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,27 +12,29 @@
 
 """Tests that hit all the basic server endpoints using both a public and premium provider."""
 
 import time
 from datetime import datetime, timedelta
 
 from qiskit import transpile
-from qiskit.test.reference_circuits import ReferenceCircuits
 
 from qiskit_ibm_provider.exceptions import IBMBackendJobLimitError
 from ..decorators import (
     IntegrationTestDependencies,
     integration_test_setup,
 )
 from ..ibm_test_case import IBMTestCase
+from ..utils import bell
 
 
 class TestBasicServerPaths(IBMTestCase):
     """Test the basic server endpoints using both a public and premium provider."""
 
+    last_week: datetime
+
     @classmethod
     @integration_test_setup()
     def setUpClass(cls, dependencies: IntegrationTestDependencies) -> None:
         # pylint: disable=arguments-differ
         super().setUpClass()
         cls.dependencies = dependencies
         cls.last_week = datetime.now() - timedelta(days=7)
@@ -41,15 +43,15 @@
         """Test retrieving jobs."""
         backend_name = "ibmq_qasm_simulator"
         for provider in ["provider", "private_provider"]:
             if not self.dependencies.instance_private:
                 raise self.skipTest("Skip test because there is no private provider")
             backend = self.dependencies[provider].get_backend(backend_name)
             with self.subTest(provider=provider, backend=backend):
-                job = self._submit_job_with_retry(ReferenceCircuits.bell(), backend)
+                job = self._submit_job_with_retry(bell(), backend)
                 job_id = job.job_id()
 
                 retrieved_jobs = self.dependencies[provider].backend.jobs(
                     backend_name=backend_name,
                     start_datetime=self.last_week,
                 )
                 self.assertGreaterEqual(len(retrieved_jobs), 1)
```

### Comparing `qiskit-ibm-provider-0.8.0/test/integration/test_filter_backends.py` & `qiskit-ibm-provider-0.9.0/test/integration/test_filter_backends.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/test/integration/test_ibm_integration.py` & `qiskit-ibm-provider-0.9.0/test/integration/test_ibm_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Integration tests."""
 
 import time
 
-from qiskit import ClassicalRegister, QuantumCircuit, QuantumRegister, execute
+from qiskit import ClassicalRegister, QuantumCircuit, QuantumRegister
 from qiskit.compiler import transpile
 from qiskit.result import Result
-from qiskit.test.reference_circuits import ReferenceCircuits
 
 from qiskit_ibm_provider import IBMBackend
 from qiskit_ibm_provider.job.exceptions import IBMJobApiError
 from ..decorators import (
     IntegrationTestDependencies,
     integration_test_setup_with_backend,
 )
 from ..ibm_test_case import IBMTestCase
+from ..utils import bell
 
 
 class TestIBMIntegration(IBMTestCase):
     """Integration tests."""
 
     @classmethod
     @integration_test_setup_with_backend(simulator=False, min_num_qubits=2)
@@ -53,15 +53,17 @@
         self._qc2 = QuantumCircuit(quantum_register, classical_register, name="qc2")
         self._qc1.measure(quantum_register[0], classical_register[0])
         self._qc2.x(quantum_register[0])
         self._qc2.measure(quantum_register[0], classical_register[0])
 
     def test_ibm_result_fields(self):
         """Test components of a result from a remote simulator."""
-        remote_result = execute(self._qc1, self.sim_backend).result()
+        remote_result = self.sim_backend.run(
+            transpile(self._qc1, self.sim_backend)
+        ).result()
         self.assertIsInstance(remote_result, Result)
         self.assertIn(
             remote_result.backend_name, [self.sim_backend.name, "qasm_simulator"]
         )
         self.assertIsInstance(remote_result.job_id, str)
         self.assertEqual(remote_result.status, "COMPLETED")
         self.assertEqual(remote_result.results[0].status, "DONE")
@@ -108,31 +110,33 @@
         )
         job = self.sim_backend.run(circs)
         result = job.result()
         self.assertIsInstance(result, Result)
 
     def test_execute_two_remote(self):
         """Test executing two circuits on a remote backend."""
-        quantum_circuit = ReferenceCircuits.bell()
+        quantum_circuit = bell()
         qc_extra = QuantumCircuit(2, 2)
         qc_extra.measure_all()
-        job = execute([quantum_circuit, qc_extra], self.sim_backend)
+        job = self.sim_backend.run(
+            transpile([quantum_circuit, qc_extra], self.sim_backend)
+        )
         results = job.result()
         self.assertIsInstance(results, Result)
 
     def test_private_job(self):
         """Test a private job."""
         if not self.dependencies.instance_private:
             print(self.skipTest("Skip test because no private instance is configured"))
 
         backend = self.dependencies.provider.get_backend(
             "ibmq_qasm_simulator", instance=self.dependencies.instance_private
         )
-        quantum_circuit = ReferenceCircuits.bell()
-        job = execute(quantum_circuit, backend=backend)
+        quantum_circuit = bell()
+        job = self.sim_backend.run(transpile(quantum_circuit, backend=backend))
         self.assertIsNotNone(job.circuits())
         self.assertIsNotNone(job.result())
 
         # Wait a bit for databases to update.
         time.sleep(2)
         rjob = self.dependencies.provider.backend.retrieve_job(job.job_id())
```

### Comparing `qiskit-ibm-provider-0.8.0/test/integration/test_ibm_job.py` & `qiskit-ibm-provider-0.9.0/test/integration/test_ibm_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,53 +18,51 @@
 from unittest import SkipTest, mock
 from unittest import skip
 
 from dateutil import tz
 from qiskit import ClassicalRegister, QuantumCircuit, QuantumRegister
 from qiskit.compiler import transpile
 from qiskit.providers.jobstatus import JobStatus, JOB_FINAL_STATES
-from qiskit.test.reference_circuits import ReferenceCircuits
 
-from qiskit_ibm_provider import IBMBackend
+from qiskit_ibm_provider import IBMBackend, IBMProvider
 from qiskit_ibm_provider.api.exceptions import RequestsApiError
 from qiskit_ibm_provider.api.rest.job import Job as RestJob
 from qiskit_ibm_provider.exceptions import IBMBackendApiError
 from qiskit_ibm_provider.job.exceptions import IBMJobTimeoutError
 from ..decorators import (
     IntegrationTestDependencies,
     integration_test_setup_with_backend,
     production_only,
 )
 from ..fake_account_client import BaseFakeAccountClient, CancelableFakeJob
 from ..ibm_test_case import IBMTestCase
-from ..utils import (
-    most_busy_backend,
-    cancel_job,
-    submit_and_cancel,
-)
+from ..utils import most_busy_backend, cancel_job, submit_and_cancel, bell
 
 
 class TestIBMJob(IBMTestCase):
     """Test ibm_job module."""
 
+    provider: IBMProvider
+    last_month: datetime
+
     @classmethod
     @integration_test_setup_with_backend(simulator=False, min_num_qubits=2)
     def setUpClass(
         cls, backend: IBMBackend, dependencies: IntegrationTestDependencies
     ) -> None:
         """Initial class level setup."""
         # pylint: disable=arguments-differ
         super().setUpClass()
         cls.provider = dependencies.provider
         cls.sim_backend = dependencies.provider.get_backend(
             "ibmq_qasm_simulator", instance=dependencies.instance
         )
         cls.real_device_backend = backend
         cls.dependencies = dependencies
-        cls.bell = transpile(ReferenceCircuits.bell(), cls.sim_backend)
+        cls.bell = transpile(bell(), cls.sim_backend)
         cls.sim_job = cls.sim_backend.run(cls.bell)
         cls.last_month = datetime.now() - timedelta(days=30)
 
     def test_run_multiple_simulator(self):
         """Test running multiple jobs in a simulator."""
         num_qubits = 16
         quantum_register = QuantumRegister(num_qubits, "qr")
@@ -206,16 +204,16 @@
         for my_backend in provider.backends():
             if my_backend.status().operational and my_backend.name != backend_1.name:
                 backend_2 = my_backend
                 break
         if not backend_2:
             raise SkipTest("Skipping test that requires multiple backends")
 
-        job_1 = backend_1.run(transpile(ReferenceCircuits.bell()))
-        job_2 = backend_2.run(transpile(ReferenceCircuits.bell()))
+        job_1 = backend_1.run(transpile(bell()))
+        job_2 = backend_2.run(transpile(bell()))
 
         # test a retrieved job's backend is the same as the queried backend
         self.assertEqual(
             provider.backend.retrieve_job(job_1.job_id()).backend().name, backend_1.name
         )
         self.assertEqual(
             provider.backend.retrieve_job(job_2.job_id()).backend().name, backend_2.name
@@ -430,15 +428,15 @@
                             thread.join(0.1)
         finally:
             self.sim_backend._api_client = saved_api
 
     def test_wait_for_final_state_timeout(self):
         """Test waiting for job to reach final state times out."""
         backend = most_busy_backend(self.provider, instance=self.dependencies.instance)
-        job = backend.run(transpile(ReferenceCircuits.bell(), backend=backend))
+        job = backend.run(transpile(bell(), backend=backend))
         try:
             self.assertRaises(IBMJobTimeoutError, job.wait_for_final_state, timeout=0.1)
         finally:
             # Ensure all threads ended.
             for thread in job._executor._threads:
                 thread.join(0.1)
             cancel_job(job)
```

### Comparing `qiskit-ibm-provider-0.8.0/test/integration/test_ibm_job_attributes.py` & `qiskit-ibm-provider-0.9.0/test/integration/test_ibm_job_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 import uuid
 from datetime import datetime, timedelta
 from unittest import mock, skip
 
 from dateutil import tz
 from qiskit.compiler import transpile
 from qiskit.providers.jobstatus import JobStatus, JOB_FINAL_STATES
-from qiskit.test.reference_circuits import ReferenceCircuits
 
+from qiskit_ibm_provider import IBMJob
 from qiskit_ibm_provider.api.clients.runtime import RuntimeClient
 from qiskit_ibm_provider.exceptions import (
     IBMBackendValueError,
 )
 from qiskit_ibm_provider.job.exceptions import IBMJobFailureError
 from ..decorators import (
     IntegrationTestDependencies,
@@ -35,38 +35,42 @@
 from ..fake_account_client import BaseFakeAccountClient
 from ..ibm_test_case import IBMTestCase
 from ..utils import (
     most_busy_backend,
     cancel_job,
     submit_job_bad_shots,
     submit_job_one_bad_instr,
+    bell,
 )
 
 
 class TestIBMJobAttributes(IBMTestCase):
     """Test IBMJob instance attributes."""
 
+    sim_job: IBMJob
+    last_week: datetime
+
     @classmethod
     @integration_test_setup()
     def setUpClass(cls, dependencies: IntegrationTestDependencies) -> None:
         """Initial class level setup."""
         # pylint: disable=arguments-differ
         super().setUpClass()
         cls.dependencies = dependencies
         cls.sim_backend = dependencies.provider.get_backend(
             "ibmq_qasm_simulator", instance=dependencies.instance
         )
-        cls.bell = transpile(ReferenceCircuits.bell(), cls.sim_backend)
+        cls.bell = transpile(bell(), cls.sim_backend)
         cls.sim_job = cls.sim_backend.run(cls.bell)
         cls.last_week = datetime.now() - timedelta(days=7)
 
     def setUp(self):
         """Initial test setup."""
         super().setUp()
-        self._qc = ReferenceCircuits.bell()
+        self._qc = bell()
 
     def test_job_id(self):
         """Test getting a job ID."""
         self.assertTrue(self.sim_job.job_id() is not None)
 
     def test_get_backend_name(self):
         """Test getting a backend name."""
```

### Comparing `qiskit-ibm-provider-0.8.0/test/integration/test_ibm_provider.py` & `qiskit-ibm-provider-0.9.0/test/integration/test_ibm_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from datetime import datetime
 from unittest import skip, mock
 
 from qiskit import ClassicalRegister, QuantumCircuit, QuantumRegister
 from qiskit.compiler import transpile
 from qiskit.providers.exceptions import QiskitBackendNotFoundError
 from qiskit.providers.models.backendproperties import BackendProperties
-from qiskit.test.reference_circuits import ReferenceCircuits
 
 from qiskit_ibm_provider import hub_group_project
 from qiskit_ibm_provider.api.clients import AccountClient, RuntimeClient
 from qiskit_ibm_provider.api.exceptions import RequestsApiError
 
 from qiskit_ibm_provider.job.ibm_job import IBMJob
 from qiskit_ibm_provider.ibm_backend import IBMBackend
@@ -33,14 +32,15 @@
 from ..decorators import (
     IntegrationTestDependencies,
     integration_test_setup,
     integration_test_setup_with_backend,
     production_only,
 )
 from ..ibm_test_case import IBMTestCase
+from ..utils import bell
 
 API_URL = "https://api.quantum-computing.ibm.com/api"
 AUTH_URL = "https://auth.quantum-computing.ibm.com/api"
 
 
 class TestIBMProviderEnableAccount(IBMTestCase):
     """Tests for IBMProvider."""
@@ -154,14 +154,15 @@
 
 
 class TestIBMProviderServices(IBMTestCase):
     """Tests for services provided by the IBMProvider class."""
 
     provider_cls = IBMProvider
     backend_name = "ibmq_qasm_simulator"
+    instance: str
 
     @classmethod
     @integration_test_setup_with_backend(simulator=False)
     def setUpClass(
         cls, backend: IBMBackend, dependencies: IntegrationTestDependencies
     ) -> None:
         """Initial class setup."""
@@ -247,16 +248,16 @@
 
     def test_backend_instance(self):
         """Test that the instance is saved correctly."""
         backend = self.dependencies.provider.get_backend(
             name=self.backend_name, instance=self.instance
         )
         backends = self.dependencies.provider.backends(instance=self.instance)
-        job = backend.run(ReferenceCircuits.bell())
-        job2 = backends[0].run(ReferenceCircuits.bell())
+        job = backend.run(bell())
+        job2 = backends[0].run(bell())
         self.assertEqual(self.instance, backend._instance)
         self.assertEqual(self.instance, backends[0]._instance)
         self.assertEqual(self.instance, job._backend._instance)
         self.assertEqual(self.instance, job2._backend._instance)
 
     def test_remote_backends_exist_real_device(self):
         """Test if there are remote backends that are devices."""
```

### Comparing `qiskit-ibm-provider-0.8.0/test/integration/test_ibm_qasm_simulator.py` & `qiskit-ibm-provider-0.9.0/test/integration/test_ibm_qasm_simulator.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,25 +13,23 @@
 """Test IBM Quantum online QASM simulator."""
 
 from unittest import mock
 from unittest import skip
 
 from qiskit import ClassicalRegister, QuantumCircuit, QuantumRegister
 from qiskit.compiler import transpile
-from qiskit.providers.aer.noise import (  # pylint: disable=import-error,no-name-in-module
-    NoiseModel,
-)
-from qiskit.test.reference_circuits import ReferenceCircuits
+from qiskit_aer.noise import NoiseModel
 
 from qiskit_ibm_provider import IBMBackend
 from ..decorators import (
     integration_test_setup_with_backend,
     IntegrationTestDependencies,
 )
 from ..ibm_test_case import IBMTestCase
+from ..utils import bell
 
 
 class TestIBMQasmSimulator(IBMTestCase):
     """Test IBM Quantum QASM Simulator."""
 
     @integration_test_setup_with_backend(simulator=False)
     def setUp(
@@ -58,15 +56,15 @@
         circs = transpile(quantum_circuit, backend=self.sim_backend)
         shots = 1024
         job = self.sim_backend.run(circs, shots=shots)
         result = job.result()
         counts = result.get_counts(quantum_circuit)
         target = {"0": shots / 2, "1": shots / 2}
         threshold = 0.1 * shots
-        self.assertDictAlmostEqual(counts, target, threshold)
+        self.assert_dict_almost_equal(counts, target, threshold)
 
     def test_execute_several_circuits_simulator_online(self):
         """Test execute_several_circuits_simulator_online."""
         quantum_register = QuantumRegister(2)
         classical_register = ClassicalRegister(2)
         qcr1 = QuantumCircuit(quantum_register, classical_register, name="qc1")
         qcr2 = QuantumCircuit(quantum_register, classical_register, name="qc2")
@@ -82,16 +80,16 @@
         job = self.sim_backend.run(circs, shots=shots)
         result = job.result()
         counts1 = result.get_counts(qcr1)
         counts2 = result.get_counts(qcr2)
         target1 = {"00": shots / 4, "01": shots / 4, "10": shots / 4, "11": shots / 4}
         target2 = {"00": shots / 2, "11": shots / 2}
         threshold = 0.1 * shots
-        self.assertDictAlmostEqual(counts1, target1, threshold)
-        self.assertDictAlmostEqual(counts2, target2, threshold)
+        self.assert_dict_almost_equal(counts1, target1, threshold)
+        self.assert_dict_almost_equal(counts2, target2, threshold)
 
     def test_online_qasm_simulator_two_registers(self):
         """Test online_qasm_simulator_two_registers."""
         qr1 = QuantumRegister(2)
         cr1 = ClassicalRegister(2)
         qr2 = QuantumRegister(2)
         cr2 = ClassicalRegister(2)
@@ -130,15 +128,15 @@
 
         sim_method = backend._configuration._data.get("simulation_method", None)
         submit_fn = backend._submit_job
 
         try:
             backend._configuration._data["simulation_method"] = "extended_stabilizer"
             backend._submit_job = _new_submit
-            circ = transpile(ReferenceCircuits.bell(), backend=backend)
+            circ = transpile(bell(), backend=backend)
             backend.run(circ, header={"test": "circuits"})
         finally:
             backend._configuration._data["simulation_method"] = sim_method
             backend._submit_job = submit_fn
 
     @skip("TODO refactor to use backend._runtime_run")
     def test_new_sim_method_no_overwrite(self):
@@ -155,25 +153,25 @@
 
         sim_method = backend._configuration._data.get("simulation_method", None)
         submit_fn = backend._submit_job
 
         try:
             backend._configuration._data["simulation_method"] = "extended_stabilizer"
             backend._submit_job = _new_submit
-            circ = transpile(ReferenceCircuits.bell(), backend=backend)
+            circ = transpile(bell(), backend=backend)
             backend.run(circ, method="my_method", header={"test": "circuits"})
         finally:
             backend._configuration._data["simulation_method"] = sim_method
             backend._submit_job = submit_fn
 
     @skip(
         "NoiseModel.from_backend does not currently support V2 Backends. \
         Skip test until it's fixed in aer."
     )
     def test_simulator_with_noise_model(self):
         """Test using simulator with a noise model."""
         noise_model = NoiseModel.from_backend(self.real_device_backend)
         result = self.sim_backend.run(
-            transpile(ReferenceCircuits.bell(), backend=self.sim_backend),
+            transpile(bell(), backend=self.sim_backend),
             noise_model=noise_model,
         ).result()
         self.assertTrue(result)
```

### Comparing `qiskit-ibm-provider-0.8.0/test/integration/test_jupyter.py` & `qiskit-ibm-provider-0.9.0/test/integration/test_jupyter.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 """Tests for Jupyter tools."""
 
 from datetime import datetime, timedelta
 from unittest import mock
 
 from qiskit import transpile
-from qiskit.test.reference_circuits import ReferenceCircuits
 
 from qiskit_ibm_provider.jupyter.config_widget import config_tab
 from qiskit_ibm_provider.jupyter.dashboard.backend_widget import make_backend_widget
 from qiskit_ibm_provider.jupyter.dashboard.job_widgets import create_job_widget
 from qiskit_ibm_provider.jupyter.dashboard.utils import BackendWithProviders
 from qiskit_ibm_provider.jupyter.dashboard.watcher_monitor import _job_checker
 from qiskit_ibm_provider.jupyter.gates_widget import gates_tab
@@ -28,14 +27,15 @@
 from qiskit_ibm_provider.jupyter.qubits_widget import qubits_tab
 from qiskit_ibm_provider.visualization.interactive.error_map import iplot_error_map
 from ..decorators import (
     IntegrationTestDependencies,
     integration_test_setup,
 )
 from ..ibm_test_case import IBMTestCase
+from ..utils import bell
 
 
 class TestBackendInfo(IBMTestCase):
     """Test backend information Jupyter widget."""
 
     @classmethod
     @integration_test_setup()
@@ -106,23 +106,23 @@
                     backend=backend, providers=[self.dependencies.instance]
                 )
                 make_backend_widget(backend_with_providers)
 
     def test_job_widget(self):
         """Test jobs tab."""
         backend = self.dependencies.provider.get_backend("ibmq_qasm_simulator")
-        job = backend.run(transpile(ReferenceCircuits.bell(), backend))
+        job = backend.run(transpile(bell(), backend))
         create_job_widget(
             mock.MagicMock(), job, backend=backend.name, status=job.status().value
         )
 
     def test_watcher_monitor(self):
         """Test job watcher."""
         backend = self.dependencies.provider.get_backend("ibmq_qasm_simulator")
-        job = backend.run(transpile(ReferenceCircuits.bell(), backend))
+        job = backend.run(transpile(bell(), backend))
         _job_checker(job=job, status=job.status(), watcher=mock.MagicMock())
 
 
 def _get_backends(provider):
     """Return backends for testing."""
     backends = []
     n_qubits = [1, 5]
```

### Comparing `qiskit-ibm-provider-0.8.0/test/integration/test_proxies.py` & `qiskit-ibm-provider-0.9.0/test/integration/test_proxies.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/test/integration/test_serialization.py` & `qiskit-ibm-provider-0.9.0/test/integration/test_serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,24 +15,23 @@
 from typing import Set, Any, Dict, Optional
 from unittest import SkipTest, skip
 import numpy as np
 
 import dateutil.parser
 from qiskit import transpile, schedule, QuantumCircuit
 from qiskit.circuit import Parameter
-from qiskit.test.reference_circuits import ReferenceCircuits
 from qiskit_ibm_provider import least_busy
 from qiskit_ibm_provider.utils.json_encoder import IBMJsonEncoder
 from ..decorators import (
     IntegrationTestDependencies,
     integration_test_setup,
     production_only,
 )
 from ..ibm_test_case import IBMTestCase
-from ..utils import cancel_job
+from ..utils import cancel_job, bell
 
 
 class TestSerialization(IBMTestCase):
     """Test data serialization."""
 
     @classmethod
     @integration_test_setup()
@@ -40,15 +39,15 @@
         """Initial class level setup."""
         # pylint: disable=arguments-differ
         super().setUpClass()
         cls.dependencies = dependencies
         cls.sim_backend = cls.dependencies.provider.get_backend(
             "ibmq_qasm_simulator",
         )
-        cls.bell = transpile(ReferenceCircuits.bell(), backend=cls.sim_backend)
+        cls.bell = transpile(bell(), backend=cls.sim_backend)
 
     @skip("See Terra issue #9488")
     def test_pulse_qobj(self):
         """Test serializing pulse qobj data."""
         backends = self.dependencies.provider.backends(
             operational=True, open_pulse=True, instance=self.dependencies.instance
         )
```

### Comparing `qiskit-ibm-provider-0.8.0/test/integration/test_session.py` & `qiskit-ibm-provider-0.9.0/test/integration/test_session.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """IBMBackend Test."""
 
-from qiskit.test.reference_circuits import ReferenceCircuits
 from qiskit.result import Result
 
 from qiskit_ibm_provider import IBMProvider
 
 from ..decorators import (
     IntegrationTestDependencies,
     integration_test_setup,
 )
 from ..ibm_test_case import IBMTestCase
+from ..utils import bell
 
 
 class TestIntegrationSession(IBMTestCase):
     """Test Session module."""
 
     @classmethod
     @integration_test_setup()
@@ -39,26 +39,26 @@
         """Test that session_id is updated correctly and maintained throughout the session"""
         provider = IBMProvider(self.dependencies.token, self.dependencies.url)
         backend = provider.get_backend("ibmq_qasm_simulator")
 
         backend.open_session()
         self.assertEqual(backend.session.session_id, None)
         self.assertTrue(backend.session.active)
-        job1 = backend.run(ReferenceCircuits.bell())
+        job1 = backend.run(bell())
         self.assertEqual(job1._session_id, job1.job_id())
-        job2 = backend.run(ReferenceCircuits.bell())
+        job2 = backend.run(bell())
         self.assertFalse(job2._session_id == job2.job_id())
 
     def test_backend_run_with_session(self):
         """Test that 'shots' parameter is transferred correctly"""
         shots = 1000
         provider = IBMProvider(self.dependencies.token, self.dependencies.url)
         backend = provider.get_backend("ibmq_qasm_simulator")
         backend.open_session()
-        result = backend.run(circuits=ReferenceCircuits.bell(), shots=shots).result()
+        result = backend.run(circuits=bell(), shots=shots).result()
         self.assertIsInstance(result, Result)
         self.assertEqual(result.results[0].shots, shots)
         self.assertAlmostEqual(
             result.get_counts()["00"], result.get_counts()["11"], delta=shots / 10
         )
 
     def test_session_cancel(self):
@@ -79,43 +79,43 @@
         backend.close_session()
         self.assertIsNone(backend.session)
 
     def test_run_after_cancel(self):
         """Test running after session is cancelled."""
         provider = IBMProvider(self.dependencies.token, self.dependencies.url)
         backend = provider.get_backend("ibmq_qasm_simulator")
-        job1 = backend.run(circuits=ReferenceCircuits.bell())
+        job1 = backend.run(circuits=bell())
         self.assertIsNone(backend.session)
         self.assertIsNone(job1._session_id)
 
         backend.open_session()
-        job2 = backend.run(ReferenceCircuits.bell())
+        job2 = backend.run(bell())
         self.assertIsNotNone(job2._session_id)
         backend.cancel_session()
 
-        job3 = backend.run(circuits=ReferenceCircuits.bell())
+        job3 = backend.run(circuits=bell())
         self.assertIsNone(backend.session)
         self.assertIsNone(job3._session_id)
 
     def test_session_as_context_manager(self):
         """Test session as a context manager"""
         provider = IBMProvider(self.dependencies.token, self.dependencies.url)
         backend = provider.get_backend("ibmq_qasm_simulator")
 
         with backend.open_session() as session:
-            job1 = backend.run(ReferenceCircuits.bell())
+            job1 = backend.run(bell())
             session_id = session.session_id
             self.assertEqual(session_id, job1.job_id())
-            job2 = backend.run(ReferenceCircuits.bell())
+            job2 = backend.run(bell())
             self.assertFalse(session_id == job2.job_id())
 
     def test_run_after_cancel_as_context_manager(self):
         """Test run after cancel in context manager"""
         provider = IBMProvider(self.dependencies.token, self.dependencies.url)
         backend = provider.get_backend("ibmq_qasm_simulator")
         with backend.open_session() as session:
-            _ = backend.run(ReferenceCircuits.bell())
+            _ = backend.run(bell())
         self.assertEqual(backend.session, session)
         backend.cancel_session()
-        job = backend.run(circuits=ReferenceCircuits.bell())
+        job = backend.run(circuits=bell())
         self.assertIsNone(backend.session)
         self.assertIsNone(job._session_id)
```

### Comparing `qiskit-ibm-provider-0.8.0/test/integration/test_websocket_integration.py` & `qiskit-ibm-provider-0.9.0/test/integration/test_websocket_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,25 +15,24 @@
 from queue import Queue
 from threading import Thread
 from unittest import mock
 
 from qiskit import transpile
 from qiskit.providers import JobTimeoutError
 from qiskit.providers.jobstatus import JobStatus
-from qiskit.test.reference_circuits import ReferenceCircuits
 from qiskit_ibm_provider import IBMBackend
 from qiskit_ibm_provider.api.clients import websocket
 from qiskit_ibm_provider.api.clients.runtime import RuntimeClient
 from ..decorators import (
     IntegrationTestDependencies,
     integration_test_setup_with_backend,
 )
 from ..ibm_test_case import IBMTestCase
 from ..proxy_server import MockProxyServer, use_proxies
-from ..utils import most_busy_backend, cancel_job
+from ..utils import most_busy_backend, cancel_job, bell
 
 
 class TestWebsocketIntegration(IBMTestCase):
     """Websocket integration tests."""
 
     @classmethod
     @integration_test_setup_with_backend(simulator=False)
@@ -43,15 +42,15 @@
         """Initial class level setup."""
         # pylint: disable=arguments-differ
         super().setUpClass()
         cls.dependencies = dependencies
         cls.sim_backend = dependencies.provider.get_backend(
             "ibmq_qasm_simulator", instance=dependencies.instance
         )
-        cls.bell = transpile(ReferenceCircuits.bell(), cls.sim_backend)
+        cls.bell = transpile(bell(), cls.sim_backend)
         cls.real_device_backend = backend
 
     def setUp(self):
         """Initial test setup."""
         super().setUp()
         self.saved_status_polling = (
             self.sim_backend._api_client._job_final_status_polling
@@ -159,15 +158,15 @@
                 ),
             )
 
     def test_websockets_timeout(self):
         """Test timeout checking status of a job via websockets."""
         backend = most_busy_backend(self.dependencies.provider)
         job = backend.run(
-            transpile(ReferenceCircuits.bell(), backend),
+            transpile(bell(), backend),
             shots=backend.configuration().max_shots,
         )
 
         try:
             with self.assertRaises(JobTimeoutError):
                 job.result(timeout=0.1)
         finally:
```

### Comparing `qiskit-ibm-provider-0.8.0/test/jobtestcase.py` & `qiskit-ibm-provider-0.9.0/test/jobtestcase.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/test/proxy_server.py` & `qiskit-ibm-provider-0.9.0/test/proxy_server.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/test/unit/mock/fake_account_client.py` & `qiskit-ibm-provider-0.9.0/test/unit/mock/fake_account_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,23 +11,27 @@
 # that they have been altered from the originals.
 
 """Fake AccountClient."""
 
 from datetime import datetime as python_datetime
 from typing import List, Dict, Any, Optional
 
-from qiskit.providers.fake_provider.backends.lima.fake_lima import FakeLima
 from qiskit.providers.exceptions import QiskitBackendNotFoundError
 
+try:
+    from qiskit.providers.fake_provider import Fake5QV1
+except ImportError:
+    from qiskit.providers.fake_provider import FakeLima as Fake5QV1
+
 
 class FakeApiBackend:
     """Fake backend."""
 
     def __init__(self, config_update=None, status_update=None):
-        fake_backend = FakeLima()
+        fake_backend = Fake5QV1()
         self.properties = fake_backend.properties().to_dict()
         self.defaults = fake_backend.defaults().to_dict()
 
         self.configuration = fake_backend.configuration().to_dict()
         self.configuration["online_date"] = python_datetime.now().isoformat()
         if config_update:
             self.configuration.update(**config_update)
@@ -56,15 +60,15 @@
                 configuration / status. For example::
 
                     specs = [ {"configuration": {"backend_name": "backend1"},
                                                  "status": {"operational": False}}
                     ]
         """
         self._hgp = hgp
-        self._fake_backend = FakeLima()
+        self._fake_backend = Fake5QV1()
         self._backends = []
         if not specs:
             specs = [{}] * num_backends
 
         for idx, backend_spec in enumerate(specs):
             config = backend_spec.get("configuration", {})
             status = backend_spec.get("status", {})
```

### Comparing `qiskit-ibm-provider-0.8.0/test/unit/mock/fake_provider.py` & `qiskit-ibm-provider-0.9.0/test/unit/mock/fake_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/test/unit/test_account.py` & `qiskit-ibm-provider-0.9.0/test/unit/test_account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/test/unit/test_backend.py` & `qiskit-ibm-provider-0.9.0/test/unit/test_backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,29 +13,33 @@
 """Tests for the backend functions."""
 import copy
 from datetime import datetime
 from unittest import mock
 import warnings
 
 from qiskit import transpile, qasm3, QuantumCircuit
-from qiskit.providers.fake_provider import FakeManila
 from qiskit.providers.models import BackendStatus, BackendProperties
 
+try:
+    from qiskit.providers.fake_provider import Fake5QV1
+except ImportError:
+    from qiskit.providers.fake_provider import FakeManila as Fake5QV1
+
 from qiskit_ibm_provider.ibm_backend import IBMBackend
 from qiskit_ibm_provider.exceptions import IBMBackendValueError
 
 from ..ibm_test_case import IBMTestCase
 
 
 class TestBackend(IBMTestCase):
     """Tests for IBMBackend class."""
 
     def test_raise_faulty_qubits(self):
         """Test faulty qubits is raised."""
-        fake_backend = FakeManila()
+        fake_backend = Fake5QV1()
         num_qubits = fake_backend.configuration().num_qubits
         circ = QuantumCircuit(num_qubits, num_qubits)
         for i in range(num_qubits):
             circ.x(i)
 
         transpiled = transpile(circ, backend=fake_backend)
         faulty_qubit = 4
@@ -46,15 +50,15 @@
         with self.assertRaises(ValueError) as err:
             ibm_backend.run(transpiled)
 
         self.assertIn(f"faulty qubit {faulty_qubit}", str(err.exception))
 
     def test_raise_faulty_qubits_many(self):
         """Test faulty qubits is raised if one circuit uses it."""
-        fake_backend = FakeManila()
+        fake_backend = Fake5QV1()
         num_qubits = fake_backend.configuration().num_qubits
 
         circ1 = QuantumCircuit(1, 1)
         circ1.x(0)
         circ2 = QuantumCircuit(num_qubits, num_qubits)
         for i in range(num_qubits):
             circ2.x(i)
@@ -68,15 +72,15 @@
         with self.assertRaises(ValueError) as err:
             ibm_backend.run(transpiled)
 
         self.assertIn(f"faulty qubit {faulty_qubit}", str(err.exception))
 
     def test_raise_faulty_edge(self):
         """Test faulty edge is raised."""
-        fake_backend = FakeManila()
+        fake_backend = Fake5QV1()
         num_qubits = fake_backend.configuration().num_qubits
         circ = QuantumCircuit(num_qubits, num_qubits)
         for i in range(num_qubits - 2):
             circ.cx(i, i + 1)
 
         transpiled = transpile(circ, backend=fake_backend)
         edge_qubits = [0, 1]
@@ -88,15 +92,15 @@
             ibm_backend.run(transpiled)
 
         self.assertIn("cx", str(err.exception))
         self.assertIn(f"faulty edge {tuple(edge_qubits)}", str(err.exception))
 
     def test_faulty_qubit_not_used(self):
         """Test faulty qubit is not raise if not used."""
-        fake_backend = FakeManila()
+        fake_backend = Fake5QV1()
         circ = QuantumCircuit(2, 2)
         for i in range(2):
             circ.x(i)
 
         transpiled = transpile(circ, backend=fake_backend, initial_layout=[0, 1])
         faulty_qubit = 4
         ibm_backend = self._create_faulty_backend(
@@ -107,15 +111,15 @@
             ibm_backend.run(circuits=transpiled)
 
         mock_run.assert_called_once()
 
     def test_faulty_edge_not_used(self):
         """Test faulty edge is not raised if not used."""
 
-        fake_backend = FakeManila()
+        fake_backend = Fake5QV1()
         coupling_map = fake_backend.configuration().coupling_map
 
         circ = QuantumCircuit(2, 2)
         circ.cx(0, 1)
 
         transpiled = transpile(
             circ, backend=fake_backend, initial_layout=coupling_map[0]
@@ -182,15 +186,15 @@
         return out_backend
 
     def test_dynamic_circuits_warning(self):
         """Test warning when user defines dynamic==False and circuits are dynamic"""
         # pylint: disable=not-context-manager
 
         # backend is not faulty because no faulty parameters given
-        backend = self._create_faulty_backend(model_backend=FakeManila())
+        backend = self._create_faulty_backend(model_backend=Fake5QV1())
 
         circuits = []
         circ = QuantumCircuit(2, 2)
         circ.h(0)
         circ.measure(0, 0)
         with circ.if_test((0, False)):
             circ.x(1)
@@ -224,15 +228,15 @@
             self.assertIn(
                 f"The backend {backend.name} does not support dynamic circuits.",
                 str(warn[1].message),
             )
 
     def _create_dc_test_backend(self):
         """Create a test backend with an IfElseOp enables."""
-        model_backend = FakeManila()
+        model_backend = Fake5QV1()
         properties = model_backend.properties()
 
         out_backend = IBMBackend(
             configuration=model_backend.configuration(),
             provider=mock.MagicMock(),
             api_client=None,
             instance=None,
@@ -340,15 +344,15 @@
         """Test that deepcopy of a backend works properly"""
         backend = self._create_dc_test_backend()
         backend_copy = copy.deepcopy(backend)
         self.assertEqual(backend_copy.name, backend.name)
 
     def test_too_many_circuits(self):
         """Test exception when number of circuits exceeds backend._max_circuits"""
-        model_backend = FakeManila()
+        model_backend = Fake5QV1()
         backend = IBMBackend(
             configuration=model_backend.configuration(),
             provider=mock.MagicMock(),
             api_client=None,
             instance=None,
         )
         max_circs = backend.configuration().max_experiments
```

### Comparing `qiskit-ibm-provider-0.8.0/test/unit/test_ibm_job_states.py` & `qiskit-ibm-provider-0.9.0/test/unit/test_ibm_job_states.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,28 +24,31 @@
 from unittest import mock
 from unittest.mock import MagicMock
 from typing import List, Any, Dict
 
 from qiskit import transpile
 from qiskit.providers import JobTimeoutError
 from qiskit.providers.jobstatus import JobStatus
-from qiskit.providers.fake_provider.backends.bogota.fake_bogota import FakeBogota
 
-from qiskit.test.reference_circuits import ReferenceCircuits
+try:
+    from qiskit.providers.fake_provider import Fake5QV1
+except ImportError:
+    from qiskit.providers.fake_provider import FakeBogota as Fake5QV1
 
 from qiskit_ibm_provider.api.exceptions import (
     ApiError,
     UserTimeoutExceededError,
     ApiIBMProtocolError,
 )
 from qiskit_ibm_provider.apiconstants import API_JOB_FINAL_STATES, ApiJobStatus
 
 from qiskit_ibm_provider.ibm_backend import IBMBackend
 from qiskit_ibm_provider.job.exceptions import IBMJobInvalidStateError
 from ..jobtestcase import JobTestCase
+from ..utils import bell
 
 MOCKED_ERROR_RESULT: Dict[str, Any] = {
     "qObjectResult": {
         "backend_name": "fake_backend",
         "backend_version": "0.1.1",
         "qobj_id": "123",
         "job_id": "123",
@@ -312,17 +315,17 @@
         """Test transpiling job state."""
         job = self.run_with_api(TranspilingStatusAPI())
         time.sleep(0.2)
         self.assertEqual(job.status(), JobStatus.INITIALIZING)
 
     def run_with_api(self, api):
         """Creates a new ``IBMJob`` running with the provided API object."""
-        backend = IBMBackend(FakeBogota().configuration(), MagicMock(), api_client=api)
+        backend = IBMBackend(Fake5QV1().configuration(), MagicMock(), api_client=api)
         backend._provider._runtime_client = api
-        circuit = transpile(ReferenceCircuits.bell())
+        circuit = transpile(bell())
         self._current_api = api
         self._current_qjob = backend.run(circuit)
         self._current_qjob.refresh = MagicMock()
         return self._current_qjob
 
 
 def _auto_progress_api(api, interval=0.2):
```

### Comparing `qiskit-ibm-provider-0.8.0/test/unit/test_ibm_logger.py` & `qiskit-ibm-provider-0.9.0/test/unit/test_ibm_logger.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/test/unit/test_serialization.py` & `qiskit-ibm-provider-0.9.0/test/unit/test_serialization.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 import warnings
 
 import numpy as np
 from ddt import data, ddt
 
 from qiskit import assemble, QuantumCircuit, QuantumRegister, ClassicalRegister
 from qiskit.circuit import Parameter
-from qiskit.providers.fake_provider import FakeNairobi
+
+try:
+    from qiskit.providers.fake_provider import Fake7QPulseV1
+except ImportError:
+    from qiskit.providers.fake_provider import FakeNairobi as Fake7QPulseV1
+
 from qiskit_aer.noise import NoiseModel
 
 from qiskit_ibm_provider.utils.json_encoder import IBMJsonEncoder
 from qiskit_ibm_provider.utils.json import RuntimeEncoder, RuntimeDecoder
 from ..ibm_test_case import IBMTestCase
 
 
@@ -89,15 +94,15 @@
         circ.metadata = {"test": metadata_test}
         payload = {"circuits": [circ]}
 
         self.assertTrue(json.dumps(payload, cls=RuntimeEncoder))
 
     def test_noise_model(self):
         """Test encoding and decoding a noise model."""
-        noise_model = NoiseModel.from_backend(FakeNairobi())
+        noise_model = NoiseModel.from_backend(Fake7QPulseV1())
         self.assertIsInstance(noise_model, NoiseModel)
         encoded = json.dumps(noise_model, cls=RuntimeEncoder)
         self.assertIsInstance(encoded, str)
         with warnings.catch_warnings():
             warnings.filterwarnings(
                 "ignore",
                 category=DeprecationWarning,
```

### Comparing `qiskit-ibm-provider-0.8.0/test/unit/test_session.py` & `qiskit-ibm-provider-0.9.0/test/unit/test_session.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,38 +9,42 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """IBMBackend Test."""
 
 from unittest import mock
-from qiskit.providers.fake_provider import FakeManila
+
+try:
+    from qiskit.providers.fake_provider import Fake5QV1
+except ImportError:
+    from qiskit.providers.fake_provider import FakeManila as Fake5QV1
 from qiskit_ibm_provider import IBMBackend
 
 from ..ibm_test_case import IBMTestCase
 
 
 class TestSession(IBMTestCase):
     """Test Session module."""
 
     def test_open_session(self):
         """Test opening a session instance."""
-        model_backend = FakeManila()
+        model_backend = Fake5QV1()
         backend = IBMBackend(
             configuration=model_backend.configuration(),
             provider=mock.MagicMock(),
             api_client=None,
         )
 
         backend.open_session()
         self.assertFalse(backend.session is None)
 
     def test_session_max_time(self):
         """Test max time parameter."""
-        model_backend = FakeManila()
+        model_backend = Fake5QV1()
         backend = IBMBackend(
             configuration=model_backend.configuration(),
             provider=mock.MagicMock(),
             api_client=None,
         )
 
         max_times = [
```

### Comparing `qiskit-ibm-provider-0.8.0/test/unit/test_utils_converters.py` & `qiskit-ibm-provider-0.9.0/test/unit/test_utils_converters.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/test/unit/test_websocket.py` & `qiskit-ibm-provider-0.9.0/test/unit/test_websocket.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/test/unit/transpiler/passes/basis/test_convert_id_to_delay.py` & `qiskit-ibm-provider-0.9.0/test/unit/transpiler/passes/basis/test_convert_id_to_delay.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,29 +9,30 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Test the conversion of Id gate operations to a delay."""
 
 from qiskit.circuit import QuantumCircuit
-from qiskit.test import QiskitTestCase
 from qiskit.transpiler.passmanager import PassManager
 
 from qiskit_ibm_provider.transpiler.passes.basis.convert_id_to_delay import (
     ConvertIdToDelay,
 )
 
 from qiskit_ibm_provider.transpiler.passes.scheduling.utils import (
     DynamicCircuitInstructionDurations,
 )
 
+from .....ibm_test_case import IBMTestCase
+
 # pylint: disable=invalid-name
 
 
-class TestConvertIdToDelay(QiskitTestCase):
+class TestConvertIdToDelay(IBMTestCase):
     """Tests the ConvertIdToDelay pass"""
 
     def setUp(self):
         """Setup."""
         super().setUp()
 
         self.durations = DynamicCircuitInstructionDurations(
```

### Comparing `qiskit-ibm-provider-0.8.0/test/unit/transpiler/passes/scheduling/test_dynamical_decoupling.py` & `qiskit-ibm-provider-0.9.0/test/unit/transpiler/passes/scheduling/test_dynamical_decoupling.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,21 +31,21 @@
 from qiskit_ibm_provider.transpiler.passes.scheduling.scheduler import (
     ASAPScheduleAnalysis,
 )
 from qiskit_ibm_provider.transpiler.passes.scheduling.utils import (
     DynamicCircuitInstructionDurations,
 )
 
-from .control_flow_test_case import ControlFlowTestCase
+from .....ibm_test_case import IBMTestCase
 
 # pylint: disable=invalid-name,not-context-manager
 
 
 @ddt
-class TestPadDynamicalDecoupling(ControlFlowTestCase):
+class TestPadDynamicalDecoupling(IBMTestCase):
     """Tests PadDynamicalDecoupling pass."""
 
     def setUp(self):
         """Circuits to test dynamical decoupling on."""
         super().setUp()
 
         self.ghz4 = QuantumCircuit(4)
@@ -1044,39 +1044,54 @@
             delay_dict[dag.find_bit(delay.qargs[0]).index] += [delay.op.duration]
         self.assertNotEqual(delay_dict[0], delay_dict[1])
         self.assertNotEqual(delay_dict[1], delay_dict[2])
         self.assertNotEqual(delay_dict[3], delay_dict[4])
         self.assertEqual(delay_dict[0], delay_dict[2])
 
     def test_no_unused_qubits(self):
-        """Test DD with if_test circuit that unused qubits are untouched and not scheduled.
+        """Test DD with if_test circuit that unused qubits are untouched and
+        not scheduled. Unused qubits may also have missing durations when
+        not operational.
 
-        This ensures that programs don't have unnecessary information for unused qubits.
+        This ensures that programs don't have unnecessary information for
+        unused qubits.
         Which might hurt performance in later executon stages.
         """
 
+        # Here "x" on qubit 3 is not defined
+        durations = DynamicCircuitInstructionDurations(
+            [
+                ("h", 0, 50),
+                ("x", 0, 50),
+                ("x", 1, 50),
+                ("x", 2, 50),
+                ("measure", 0, 840),
+                ("reset", 0, 1340),
+            ]
+        )
+
         dd_sequence = [XGate(), XGate()]
         pm = PassManager(
             [
                 ASAPScheduleAnalysis(self.durations),
                 PadDynamicalDecoupling(
-                    self.durations,
+                    durations,
                     dd_sequence,
                     pulse_alignment=1,
                     sequence_min_length_ratios=[0.0],
                 ),
             ]
         )
 
-        qc = QuantumCircuit(3, 1)
+        qc = QuantumCircuit(4, 1)
         qc.measure(0, 0)
         qc.x(1)
         with qc.if_test((0, True)):
             qc.x(1)
         qc.measure(0, 0)
         with qc.if_test((0, True)):
             qc.x(0)
         qc.x(1)
         qc_dd = pm.run(qc)
-        dont_use = qc_dd.qubits[-1]
+        dont_use = qc_dd.qubits[-2:]
         for op in qc_dd.data:
             self.assertNotIn(dont_use, op.qubits)
```

### Comparing `qiskit-ibm-provider-0.8.0/test/unit/transpiler/passes/scheduling/test_scheduler.py` & `qiskit-ibm-provider-0.9.0/test/unit/transpiler/passes/scheduling/test_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,35 +11,39 @@
 # that they have been altered from the originals.
 
 """Test the dynamic circuits scheduling analysis"""
 
 from unittest.mock import patch
 
 from qiskit import ClassicalRegister, QuantumCircuit, QuantumRegister, transpile
-from qiskit.providers.fake_provider import FakeJakarta
 from qiskit.pulse import Schedule, Play, Constant, DriveChannel
 from qiskit.transpiler.passes import ConvertConditionsToIfOps
 from qiskit.transpiler.passmanager import PassManager
 from qiskit.transpiler.exceptions import TranspilerError
 
+try:
+    from qiskit.providers.fake_provider import Fake7QPulseV1
+except ImportError:
+    from qiskit.providers.fake_provider import FakeJakarta as Fake7QPulseV1
+
 from qiskit_ibm_provider.transpiler.passes.scheduling.pad_delay import PadDelay
 from qiskit_ibm_provider.transpiler.passes.scheduling.scheduler import (
     ALAPScheduleAnalysis,
     ASAPScheduleAnalysis,
 )
 from qiskit_ibm_provider.transpiler.passes.scheduling.utils import (
     DynamicCircuitInstructionDurations,
 )
 
-from .control_flow_test_case import ControlFlowTestCase
+from .....ibm_test_case import IBMTestCase
 
 # pylint: disable=invalid-name,not-context-manager
 
 
-class TestASAPSchedulingAndPaddingPass(ControlFlowTestCase):
+class TestASAPSchedulingAndPaddingPass(IBMTestCase):
     """Tests the ASAP Scheduling passes"""
 
     def test_if_test_gate_after_measure(self):
         """Test if schedules circuits with c_if after measure with a common clbit.
         See: https://github.com/Qiskit/qiskit-terra/issues/7654"""
         qc = QuantumCircuit(2, 1)
         qc.measure(0, 0)
@@ -842,20 +846,20 @@
         self.assertEqual(expected, scheduled)
 
     def test_c_if_plugin_conversion_with_transpile(self):
         """Verify that old format c_if may be converted and scheduled
         after transpilation with the plugin."""
         # Patch the test backend with the plugin
         with patch.object(
-            FakeJakarta,
+            Fake7QPulseV1,
             "get_translation_stage_plugin",
             return_value="ibm_dynamic_circuits",
             create=True,
         ):
-            backend = FakeJakarta()
+            backend = Fake7QPulseV1()
             # Temporary workaround for mock backends. For real backends this is not required.
             backend.configuration().basis_gates.append("if_else")
 
             durations = DynamicCircuitInstructionDurations.from_backend(backend)
             pm = PassManager(
                 [ASAPScheduleAnalysis(durations), PadDelay(schedule_idle_qubits=True)]
             )
@@ -880,15 +884,15 @@
             expected.delay(160, qr1[4])
             expected.delay(160, qr1[5])
             expected.delay(160, qr1[6])
 
         self.assertEqual(expected, scheduled)
 
 
-class TestALAPSchedulingAndPaddingPass(ControlFlowTestCase):
+class TestALAPSchedulingAndPaddingPass(IBMTestCase):
     """Tests the ALAP Scheduling passes"""
 
     def test_alap(self):
         """Test standard ALAP scheduling"""
         durations = DynamicCircuitInstructionDurations(
             [("x", None, 200), ("measure", None, 840)]
         )
@@ -1859,15 +1863,15 @@
         expected.x(0)
         expected.delay(200, 1)
 
         self.assertEqual(expected, scheduled)
 
     def test_transpile_mock_backend(self):
         """Test scheduling works with transpilation."""
-        backend = FakeJakarta()
+        backend = Fake7QPulseV1()
         # Temporary workaround for mock backends. For real backends this is not required.
         backend.configuration().basis_gates.append("if_else")
         backend.configuration().basis_gates.append("while_loop")
 
         durations = DynamicCircuitInstructionDurations.from_backend(backend)
         pm = PassManager(
             [ALAPScheduleAnalysis(durations), PadDelay(schedule_idle_qubits=True)]
@@ -1907,15 +1911,15 @@
             expected.delay(160, qr[5])
             expected.delay(160, qr[6])
 
         self.assertEqual(expected, scheduled)
 
     def test_transpile_both_paths(self):
         """Test scheduling works with both fast- and standard path after transpiling."""
-        backend = FakeJakarta()
+        backend = Fake7QPulseV1()
         # Temporary workaround for mock backends. For real backends this is not required.
         backend.configuration().basis_gates.append("if_else")
 
         durations = DynamicCircuitInstructionDurations.from_backend(backend)
         pm = PassManager(
             [ALAPScheduleAnalysis(durations), PadDelay(schedule_idle_qubits=True)]
         )
@@ -1932,44 +1936,37 @@
 
         qc_transpiled = transpile(qc, backend, initial_layout=[0, 1, 2])
 
         scheduled = pm.run(qc_transpiled)
 
         qr = QuantumRegister(7, name="q")
         expected = QuantumCircuit(qr, cr)
-        expected.delay(24080, qr[1])
-        expected.delay(24080, qr[2])
-        expected.delay(24080, qr[3])
-        expected.delay(24080, qr[4])
-        expected.delay(24080, qr[5])
-        expected.delay(24080, qr[6])
+        for q_ind in range(1, 7):
+            expected.delay(24240, qr[q_ind])
         expected.measure(qr[0], cr[0])
         with expected.if_test((cr[0], 1)):
             expected.x(qr[0])
         with expected.if_test((cr[0], 1)):
-            expected.delay(160, qr[0])
             expected.x(qr[1])
-            expected.delay(160, qr[2])
-            expected.delay(160, qr[3])
-            expected.delay(160, qr[4])
-            expected.delay(160, qr[5])
-            expected.delay(160, qr[6])
+            for q_ind in range(7):
+                if q_ind != 1:
+                    expected.delay(160, qr[q_ind])
         self.assertEqual(expected, scheduled)
 
     def test_c_if_plugin_conversion_with_transpile(self):
         """Verify that old format c_if may be converted and scheduled after
         transpilation with the plugin."""
         # Patch the test backend with the plugin
         with patch.object(
-            FakeJakarta,
+            Fake7QPulseV1,
             "get_translation_stage_plugin",
             return_value="ibm_dynamic_circuits",
             create=True,
         ):
-            backend = FakeJakarta()
+            backend = Fake7QPulseV1()
             # Temporary workaround for mock backends. For real backends this is not required.
             backend.configuration().basis_gates.append("if_else")
 
             durations = DynamicCircuitInstructionDurations.from_backend(backend)
             pm = PassManager(
                 [ALAPScheduleAnalysis(durations), PadDelay(schedule_idle_qubits=True)]
             )
```

### Comparing `qiskit-ibm-provider-0.8.0/test/unit/transpiler/passes/scheduling/test_utils.py` & `qiskit-ibm-provider-0.9.0/test/unit/transpiler/passes/scheduling/test_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Tests for Qiskit scheduling utilities."""
 
-from qiskit.test import QiskitTestCase
-
+from qiskit_ibm_runtime.fake_provider import FakeKolkata, FakeKolkataV2
 from qiskit_ibm_provider.transpiler.passes.scheduling.utils import (
     DynamicCircuitInstructionDurations,
 )
 
+from .....ibm_test_case import IBMTestCase
+
 
-class TestDynamicCircuitInstructionDurations(QiskitTestCase):
+class TestDynamicCircuitInstructionDurations(IBMTestCase):
     """Tests the DynamicCircuitInstructionDurations patching"""
 
     def test_patch_measure(self):
         """Test if schedules circuits with c_if after measure with a common clbit.
         See: https://github.com/Qiskit/qiskit-terra/issues/7654"""
 
         durations = DynamicCircuitInstructionDurations(
@@ -60,7 +61,36 @@
             [("x", None, 200), ("measure", None, 1000), ("measure", (0, 1), 1200)],
             enable_patching=False,
         )
 
         self.assertEqual(durations.get("x", (0,)), 200)
         self.assertEqual(durations.get("measure", (0,)), 1000)
         self.assertEqual(durations.get("measure", (0, 1)), 1200)
+
+    def test_durations_from_backend_v1(self):
+        """Test loading and patching durations from a V1 Backend"""
+
+        durations = DynamicCircuitInstructionDurations.from_backend(FakeKolkata())
+
+        self.assertEqual(durations.get("x", (0,)), 160)
+        self.assertEqual(durations.get("measure", (0,)), 3200)
+        self.assertEqual(durations.get("reset", (0,)), 3200)
+
+    def test_durations_from_backend_v2(self):
+        """Test loading and patching durations from a V2 Backend"""
+
+        durations = DynamicCircuitInstructionDurations.from_backend(FakeKolkataV2())
+
+        self.assertEqual(durations.get("x", (0,)), 160)
+        self.assertEqual(durations.get("measure", (0,)), 3200)
+        self.assertEqual(durations.get("reset", (0,)), 3200)
+
+    def test_durations_from_target(self):
+        """Test loading and patching durations from a target"""
+
+        durations = DynamicCircuitInstructionDurations.from_target(
+            FakeKolkataV2().target
+        )
+
+        self.assertEqual(durations.get("x", (0,)), 160)
+        self.assertEqual(durations.get("measure", (0,)), 3200)
+        self.assertEqual(durations.get("reset", (0,)), 3200)
```

### Comparing `qiskit-ibm-provider-0.8.0/test/unit/utils/ws_handler.py` & `qiskit-ibm-provider-0.9.0/test/unit/utils/ws_handler.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.8.0/test/utils.py` & `qiskit-ibm-provider-0.9.0/test/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,21 +12,20 @@
 
 """General utility functions for testing."""
 
 import logging
 import os
 from typing import Optional
 
-from qiskit import QuantumCircuit
 from qiskit.compiler import assemble, transpile
 from qiskit.providers.exceptions import JobError
 from qiskit.providers.jobstatus import JobStatus
 from qiskit.pulse import Schedule
 from qiskit.qobj import QasmQobj
-from qiskit.test.reference_circuits import ReferenceCircuits
+from qiskit.circuit import QuantumCircuit, QuantumRegister, ClassicalRegister
 
 from qiskit_ibm_provider.hub_group_project import HubGroupProject
 from qiskit_ibm_provider.ibm_backend import IBMBackend
 from qiskit_ibm_provider.ibm_provider import IBMProvider
 from qiskit_ibm_provider.job import IBMJob
 
 
@@ -107,15 +106,15 @@
         backend: Backend to use for transpiling the circuit.
         shots: Number of shots.
 
     Returns:
         A bell circuit in Qobj format.
     """
     return assemble(
-        transpile(ReferenceCircuits.bell(), backend=backend),
+        transpile(bell(), backend=backend),
         backend=backend,
         shots=shots,
     )
 
 
 def cancel_job(job: IBMJob, verify: bool = False) -> bool:
     """Cancel a job.
@@ -167,15 +166,15 @@
 
     Args:
         backend: Backend to submit the job to.
 
     Returns:
         Submitted job.
     """
-    qc_new = transpile(ReferenceCircuits.bell(), backend)
+    qc_new = transpile(bell(), backend)
     if backend.configuration().simulator:
         # Specify method so it doesn't fail at method selection.
         qobj = assemble([qc_new] * 2, backend=backend, method="statevector")
     else:
         qobj = assemble([qc_new] * 2, backend=backend)
     qobj.experiments[1].instructions[1].name = "bad_instruction"
     job = backend._submit_job(qobj)
@@ -187,15 +186,15 @@
 
     Args:
         backend: Backend to submit the job to.
 
     Returns:
         Cancelled job.
     """
-    circuit = transpile(ReferenceCircuits.bell(), backend=backend)
+    circuit = transpile(bell(), backend=backend)
     job = backend.run(circuit)
     cancel_job(job, True)
     return job
 
 
 def get_pulse_schedule(backend: IBMBackend) -> Schedule:
     """Return a pulse schedule."""
@@ -231,7 +230,19 @@
         # Get a non default hgp (i.e. not the default open access hgp).
         hgps = provider._get_hgps()
         for hgp in hgps:
             if hgp != open_hgp:
                 hgp_to_return = hgp
                 break
     return hgp_to_return
+
+
+def bell():
+    """Return a Bell circuit."""
+    quantum_register = QuantumRegister(2, name="qr")
+    classical_register = ClassicalRegister(2, name="cr")
+    quantum_circuit = QuantumCircuit(quantum_register, classical_register, name="bell")
+    quantum_circuit.h(quantum_register[0])
+    quantum_circuit.cx(quantum_register[0], quantum_register[1])
+    quantum_circuit.measure(quantum_register, classical_register)
+
+    return quantum_circuit
```

### Comparing `qiskit-ibm-provider-0.8.0/test/ws_server.py` & `qiskit-ibm-provider-0.9.0/test/ws_server.py`

 * *Files identical despite different names*

