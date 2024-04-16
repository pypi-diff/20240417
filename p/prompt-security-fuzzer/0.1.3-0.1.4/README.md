# Comparing `tmp/prompt_security_fuzzer-0.1.3.tar.gz` & `tmp/prompt_security_fuzzer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt_security_fuzzer-0.1.3.tar", last modified: Tue Apr 16 22:11:05 2024, max compression
+gzip compressed data, was "prompt_security_fuzzer-0.1.4.tar", last modified: Tue Apr 16 22:25:36 2024, max compression
```

## Comparing `prompt_security_fuzzer-0.1.3.tar` & `prompt_security_fuzzer-0.1.4.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:11:05.988988 prompt_security_fuzzer-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8588 2024-04-16 22:11:05.988988 prompt_security_fuzzer-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7232 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:11:05.988988 prompt_security_fuzzer-0.1.3/prompt_security_fuzzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8588 2024-04-16 22:11:05.000000 prompt_security_fuzzer-0.1.3/prompt_security_fuzzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-16 22:11:05.000000 prompt_security_fuzzer-0.1.3/prompt_security_fuzzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:11:05.000000 prompt_security_fuzzer-0.1.3/prompt_security_fuzzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-16 22:11:05.000000 prompt_security_fuzzer-0.1.3/prompt_security_fuzzer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-16 22:11:05.000000 prompt_security_fuzzer-0.1.3/prompt_security_fuzzer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 22:11:05.000000 prompt_security_fuzzer-0.1.3/prompt_security_fuzzer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:11:05.984988 prompt_security_fuzzer-0.1.3/ps_fuzz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6889 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/app_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/attack_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:11:05.984988 prompt_security_fuzzer-0.1.3/ps_fuzz/attack_data/
--rw-r--r--   0 runner    (1001) docker     (127)    82151 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/attack_data/harmful_behavior.csv
--rw-r--r--   0 runner    (1001) docker     (127)    23984 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/attack_data/prompt_injections_for_base64.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/attack_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/attack_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:11:05.984988 prompt_security_fuzzer-0.1.3/ps_fuzz/attacks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/attacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/attacks/aim.py
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/attacks/base64_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/attacks/complimentary_transition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/attacks/dan.py
--rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/attacks/dynamic_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/attacks/ethical_compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/attacks/harmful_behavior.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/attacks/self_refine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/attacks/translation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/attacks/typoglycemia.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/attacks/ucar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/chat_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/client_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/interactive_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/interactive_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/langchain_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/logo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/prompt_injection_fuzzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/ps_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/results_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/ps_fuzz/work_progress_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 22:11:05.988988 prompt_security_fuzzer-0.1.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1786 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:11:05.984988 prompt_security_fuzzer-0.1.3/system_prompt.examples/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/system_prompt.examples/medium_system_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/system_prompt.examples/strong_system_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/system_prompt.examples/weak_system_prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:11:05.984988 prompt_security_fuzzer-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/tests/test_chat_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-16 22:11:02.000000 prompt_security_fuzzer-0.1.3/tests/test_is_response_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:25:36.478560 prompt_security_fuzzer-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8588 2024-04-16 22:25:36.478560 prompt_security_fuzzer-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7232 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:25:36.474560 prompt_security_fuzzer-0.1.4/prompt_security_fuzzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8588 2024-04-16 22:25:36.000000 prompt_security_fuzzer-0.1.4/prompt_security_fuzzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-16 22:25:36.000000 prompt_security_fuzzer-0.1.4/prompt_security_fuzzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:25:36.000000 prompt_security_fuzzer-0.1.4/prompt_security_fuzzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-16 22:25:36.000000 prompt_security_fuzzer-0.1.4/prompt_security_fuzzer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-16 22:25:36.000000 prompt_security_fuzzer-0.1.4/prompt_security_fuzzer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 22:25:36.000000 prompt_security_fuzzer-0.1.4/prompt_security_fuzzer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:25:36.470560 prompt_security_fuzzer-0.1.4/ps_fuzz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6889 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/app_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/attack_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:25:36.474560 prompt_security_fuzzer-0.1.4/ps_fuzz/attack_data/
+-rw-r--r--   0 runner    (1001) docker     (127)    82151 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/attack_data/harmful_behavior.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    23984 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/attack_data/prompt_injections_for_base64.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/attack_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/attack_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:25:36.474560 prompt_security_fuzzer-0.1.4/ps_fuzz/attacks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/attacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/attacks/aim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/attacks/base64_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/attacks/complimentary_transition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/attacks/dan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/attacks/dynamic_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/attacks/ethical_compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/attacks/harmful_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/attacks/self_refine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/attacks/translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/attacks/typoglycemia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/attacks/ucar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/chat_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/client_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/interactive_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/interactive_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/langchain_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/prompt_injection_fuzzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/ps_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/results_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/ps_fuzz/work_progress_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 22:25:36.478560 prompt_security_fuzzer-0.1.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1786 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:25:36.474560 prompt_security_fuzzer-0.1.4/system_prompt.examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/system_prompt.examples/medium_system_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/system_prompt.examples/strong_system_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/system_prompt.examples/weak_system_prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:25:36.474560 prompt_security_fuzzer-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/tests/test_chat_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-16 22:25:29.000000 prompt_security_fuzzer-0.1.4/tests/test_is_response_list.py
```

### Comparing `prompt_security_fuzzer-0.1.3/CONTRIBUTING.md` & `prompt_security_fuzzer-0.1.4/CONTRIBUTING.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 ### Install dependencies
 
 Install the project dependencies in editable mode (with the '-e' argument).
 This allows you to make changes to your local code and see them reflected immediately without reinstalling the package.
 
 ```bash
-pip install -e .[dev]
+pip install -e ".[dev]"
 ```
 
 ### Run tests
 
 ```bash
 pytest
 ```
@@ -64,15 +64,15 @@
 OPENAI_API_KEY=sk-....
 ```
 The tool would automatically recognize that the file is present and will try to load the environment variables (including your API key) from it.
 
 ### Running the Tool
 
 To run the tool from your development environment, you can use the command-line interface set up in the project.
-Since the package is installed in editable mode (e.g. via `pip install -e .[dev]`), you can run the tool directly from the source code without
+Since the package is installed in editable mode (e.g. via `pip install -e ".[dev]"`), you can run the tool directly from the source code without
 needing a separate installation step for testing changes.
 
 To execute the tool, use the following command:
 ```bash
 prompt-security-fuzzer --help
 ```
```

### Comparing `prompt_security_fuzzer-0.1.3/LICENSE` & `prompt_security_fuzzer-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/PKG-INFO` & `prompt_security_fuzzer-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-security-fuzzer
-Version: 0.1.3
+Version: 0.1.4
 Summary: LLM and System Prompt vulnerability scanner tool
 Home-page: https://github.com/prompt-security/ps-fuzz
 Author: Prompt Security
 Author-email: support@prompt.security
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `prompt_security_fuzzer-0.1.3/README.md` & `prompt_security_fuzzer-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/prompt_security_fuzzer.egg-info/PKG-INFO` & `prompt_security_fuzzer-0.1.4/prompt_security_fuzzer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-security-fuzzer
-Version: 0.1.3
+Version: 0.1.4
 Summary: LLM and System Prompt vulnerability scanner tool
 Home-page: https://github.com/prompt-security/ps-fuzz
 Author: Prompt Security
 Author-email: support@prompt.security
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `prompt_security_fuzzer-0.1.3/prompt_security_fuzzer.egg-info/SOURCES.txt` & `prompt_security_fuzzer-0.1.4/prompt_security_fuzzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/app_config.py` & `prompt_security_fuzzer-0.1.4/ps_fuzz/app_config.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/attack_data/harmful_behavior.csv` & `prompt_security_fuzzer-0.1.4/ps_fuzz/attack_data/harmful_behavior.csv`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/attack_data/prompt_injections_for_base64.parquet` & `prompt_security_fuzzer-0.1.4/ps_fuzz/attack_data/prompt_injections_for_base64.parquet`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/attack_registry.py` & `prompt_security_fuzzer-0.1.4/ps_fuzz/attack_registry.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/attacks/aim.py` & `prompt_security_fuzzer-0.1.4/ps_fuzz/attacks/aim.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/attacks/base64_injection.py` & `prompt_security_fuzzer-0.1.4/ps_fuzz/attacks/base64_injection.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/attacks/complimentary_transition.py` & `prompt_security_fuzzer-0.1.4/ps_fuzz/attacks/complimentary_transition.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/attacks/dan.py` & `prompt_security_fuzzer-0.1.4/ps_fuzz/attacks/dan.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/attacks/dynamic_test.py` & `prompt_security_fuzzer-0.1.4/ps_fuzz/attacks/dynamic_test.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/attacks/ethical_compliance.py` & `prompt_security_fuzzer-0.1.4/ps_fuzz/attacks/ethical_compliance.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/attacks/harmful_behavior.py` & `prompt_security_fuzzer-0.1.4/ps_fuzz/attacks/harmful_behavior.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/attacks/self_refine.py` & `prompt_security_fuzzer-0.1.4/ps_fuzz/attacks/self_refine.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/attacks/translation.py` & `prompt_security_fuzzer-0.1.4/ps_fuzz/attacks/translation.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/attacks/typoglycemia.py` & `prompt_security_fuzzer-0.1.4/ps_fuzz/attacks/typoglycemia.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/attacks/ucar.py` & `prompt_security_fuzzer-0.1.4/ps_fuzz/attacks/ucar.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/chat_clients.py` & `prompt_security_fuzzer-0.1.4/ps_fuzz/chat_clients.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/cli.py` & `prompt_security_fuzzer-0.1.4/ps_fuzz/cli.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/client_config.py` & `prompt_security_fuzzer-0.1.4/ps_fuzz/client_config.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/interactive_chat.py` & `prompt_security_fuzzer-0.1.4/ps_fuzz/interactive_chat.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/interactive_mode.py` & `prompt_security_fuzzer-0.1.4/ps_fuzz/interactive_mode.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/langchain_integration.py` & `prompt_security_fuzzer-0.1.4/ps_fuzz/langchain_integration.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/logo.py` & `prompt_security_fuzzer-0.1.4/ps_fuzz/logo.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/prompt_injection_fuzzer.py` & `prompt_security_fuzzer-0.1.4/ps_fuzz/prompt_injection_fuzzer.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/ps_logging.py` & `prompt_security_fuzzer-0.1.4/ps_fuzz/ps_logging.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/results_table.py` & `prompt_security_fuzzer-0.1.4/ps_fuzz/results_table.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/test_base.py` & `prompt_security_fuzzer-0.1.4/ps_fuzz/test_base.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/util.py` & `prompt_security_fuzzer-0.1.4/ps_fuzz/util.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/ps_fuzz/work_progress_pool.py` & `prompt_security_fuzzer-0.1.4/ps_fuzz/work_progress_pool.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/setup.py` & `prompt_security_fuzzer-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/system_prompt.examples/strong_system_prompt.txt` & `prompt_security_fuzzer-0.1.4/system_prompt.examples/strong_system_prompt.txt`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/tests/test_chat_clients.py` & `prompt_security_fuzzer-0.1.4/tests/test_chat_clients.py`

 * *Files identical despite different names*

### Comparing `prompt_security_fuzzer-0.1.3/tests/test_is_response_list.py` & `prompt_security_fuzzer-0.1.4/tests/test_is_response_list.py`

 * *Files identical despite different names*

