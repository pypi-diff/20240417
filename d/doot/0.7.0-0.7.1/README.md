# Comparing `tmp/doot-0.7.0.tar.gz` & `tmp/doot-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doot-0.7.0.tar", last modified: Mon Apr 15 22:34:36 2024, max compression
+gzip compressed data, was "doot-0.7.1.tar", last modified: Wed Apr 17 20:06:27 2024, max compression
```

## Comparing `doot-0.7.0.tar` & `doot-0.7.1.tar`

### file list

```diff
@@ -1,186 +1,185 @@
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.949531 doot-0.7.0/
--rw-rw-r--   0 john      (1000) john      (1000)     1421 2023-12-10 00:45:10.000000 doot-0.7.0/LICENSE
--rw-r--r--   0 john      (1000) john      (1000)    10267 2024-04-15 22:34:36.949531 doot-0.7.0/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)     7358 2024-04-15 22:32:56.000000 doot-0.7.0/README.md
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.929531 doot-0.7.0/doot/
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.929531 doot-0.7.0/doot/__data/
--rw-rw-r--   0 john      (1000) john      (1000)     5167 2024-04-15 22:30:11.000000 doot-0.7.0/doot/__data/aliases.toml
--rw-rw-r--   0 john      (1000) john      (1000)     2277 2024-04-15 22:30:11.000000 doot-0.7.0/doot/__data/constants.toml
--rw-rw-r--   0 john      (1000) john      (1000)     5218 2024-04-15 22:32:56.000000 doot-0.7.0/doot/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     3414 2024-04-15 22:30:11.000000 doot-0.7.0/doot/__main__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.929531 doot-0.7.0/doot/__templates/
--rw-rw-r--   0 john      (1000) john      (1000)     1413 2024-04-15 22:30:11.000000 doot-0.7.0/doot/__templates/basic_toml
--rw-rw-r--   0 john      (1000) john      (1000)     2000 2024-04-15 22:30:11.000000 doot-0.7.0/doot/__templates/stub_task_py
--rw-rw-r--   0 john      (1000) john      (1000)      357 2023-12-09 23:29:38.000000 doot-0.7.0/doot/__templates/tasks_toml
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.929531 doot-0.7.0/doot/__tests/
--rw-rw-r--   0 john      (1000) john      (1000)      996 2024-04-15 22:30:11.000000 doot-0.7.0/doot/__tests/test_basic.py
--rw-rw-r--   0 john      (1000) john      (1000)      615 2024-04-15 22:30:11.000000 doot-0.7.0/doot/__tests/test_inits.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.933531 doot-0.7.0/doot/_abstract/
--rw-rw-r--   0 john      (1000) john      (1000)      786 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_abstract/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1158 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_abstract/cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     2712 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_abstract/control.py
--rw-rwxr--   0 john      (1000) john      (1000)     1367 2023-10-17 22:05:44.000000 doot-0.7.0/doot/_abstract/dbm.py
--rw-rw-r--   0 john      (1000) john      (1000)     2464 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_abstract/loader.py
--rw-rw-r--   0 john      (1000) john      (1000)     1289 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_abstract/overlord.py
--rw-rw-r--   0 john      (1000) john      (1000)     1700 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_abstract/parser.py
--rw-rw-r--   0 john      (1000) john      (1000)     1004 2023-12-10 23:41:06.000000 doot-0.7.0/doot/_abstract/policy.py
--rw-rw-r--   0 john      (1000) john      (1000)     1695 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_abstract/reporter.py
--rw-rw-r--   0 john      (1000) john      (1000)     1408 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_abstract/structs.py
--rw-rw-r--   0 john      (1000) john      (1000)     4736 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_abstract/task.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.933531 doot-0.7.0/doot/_structs/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-12-09 23:29:38.000000 doot-0.7.0/doot/_structs/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.937531 doot-0.7.0/doot/_structs/__tests/
--rw-rw-r--   0 john      (1000) john      (1000)     1325 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_action_spec.py
--rw-rw-r--   0 john      (1000) john      (1000)     4945 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_artifact.py
--rw-rw-r--   0 john      (1000) john      (1000)     2034 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_code_ref.py
--rw-rw-r--   0 john      (1000) john      (1000)     3131 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_formatter.py
--rw-rw-r--   0 john      (1000) john      (1000)    13645 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_key.py
--rw-rw-r--   0 john      (1000) john      (1000)     5200 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_key_decorators.py
--rw-rw-r--   0 john      (1000) john      (1000)     2361 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_key_multi.py
--rw-rw-r--   0 john      (1000) john      (1000)     7054 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_key_path_expansion.py
--rw-rw-r--   0 john      (1000) john      (1000)     4431 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_key_string_expansion.py
--rw-rw-r--   0 john      (1000) john      (1000)     3700 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_key_type_expansion.py
--rw-rw-r--   0 john      (1000) john      (1000)     6022 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_param_spec.py
--rw-rw-r--   0 john      (1000) john      (1000)     3765 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_stub.py
--rw-rw-r--   0 john      (1000) john      (1000)     8076 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_task_name.py
--rw-rw-r--   0 john      (1000) john      (1000)     7701 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_task_spec.py
--rw-rw-r--   0 john      (1000) john      (1000)     5489 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/action_spec.py
--rw-rw-r--   0 john      (1000) john      (1000)     4980 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/artifact.py
--rw-rw-r--   0 john      (1000) john      (1000)     6769 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/code_ref.py
--rw-rw-r--   0 john      (1000) john      (1000)    32021 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/key.py
--rw-rw-r--   0 john      (1000) john      (1000)      172 2023-12-11 21:35:03.000000 doot-0.7.0/doot/_structs/log.doot
--rw-rw-r--   0 john      (1000) john      (1000)    11997 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/param_spec.py
--rw-rw-r--   0 john      (1000) john      (1000)     2509 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/sname.py
--rw-rw-r--   0 john      (1000) john      (1000)     3987 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/structured_name.py
--rw-rw-r--   0 john      (1000) john      (1000)     8066 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/stub.py
--rw-rw-r--   0 john      (1000) john      (1000)     7258 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/task_name.py
--rw-rw-r--   0 john      (1000) john      (1000)    12777 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/task_spec.py
--rw-rw-r--   0 john      (1000) john      (1000)     2472 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/toml_loc.py
--rw-rw-r--   0 john      (1000) john      (1000)     1956 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/trace.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.937531 doot-0.7.0/doot/actions/
--rw-rwxr--   0 john      (1000) john      (1000)        0 2023-10-17 22:05:44.000000 doot-0.7.0/doot/actions/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.937531 doot-0.7.0/doot/actions/__tests/
--rw-rw-r--   0 john      (1000) john      (1000)     1039 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/__tests/test_base_action.py
--rw-rw-r--   0 john      (1000) john      (1000)     1349 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/__tests/test_control_flow.py
--rw-rw-r--   0 john      (1000) john      (1000)     1349 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/__tests/test_io.py
--rw-rw-r--   0 john      (1000) john      (1000)     2925 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/__tests/test_job_actions.py
--rw-rw-r--   0 john      (1000) john      (1000)     3371 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/__tests/test_job_expansion.py
--rw-rw-r--   0 john      (1000) john      (1000)     4417 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/__tests/test_job_injection.py
--rw-rw-r--   0 john      (1000) john      (1000)     2896 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/__tests/test_job_queuing.py
--rw-rw-r--   0 john      (1000) john      (1000)     1349 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/__tests/test_postbox.py
--rw-rw-r--   0 john      (1000) john      (1000)     1349 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/__tests/test_shell.py
--rw-rw-r--   0 john      (1000) john      (1000)     1349 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/__tests/test_state.py
--rw-rw-r--   0 john      (1000) john      (1000)     1565 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/base_action.py
--rw-rw-r--   0 john      (1000) john      (1000)     5462 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/compression.py
--rw-rw-r--   0 john      (1000) john      (1000)     4973 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/control_flow.py
--rw-rw-r--   0 john      (1000) john      (1000)    12958 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/io.py
--rw-rw-r--   0 john      (1000) john      (1000)     3081 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/job_actions.py
--rw-rw-r--   0 john      (1000) john      (1000)     4930 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/job_expansion.py
--rw-rw-r--   0 john      (1000) john      (1000)     7012 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/job_injection.py
--rw-rw-r--   0 john      (1000) john      (1000)     4684 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/job_queuing.py
--rw-rw-r--   0 john      (1000) john      (1000)     3902 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/json.py
--rw-rw-r--   0 john      (1000) john      (1000)     5791 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/postbox.py
--rw-rw-r--   0 john      (1000) john      (1000)     6896 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/shell.py
--rw-rw-r--   0 john      (1000) john      (1000)     3112 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/speak.py
--rw-rw-r--   0 john      (1000) john      (1000)     4057 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/state.py
--rw-rw-r--   0 john      (1000) john      (1000)      939 2024-01-20 20:13:07.000000 doot-0.7.0/doot/actions/templater.py
--rw-rw-r--   0 john      (1000) john      (1000)     1973 2023-12-09 23:29:38.000000 doot-0.7.0/doot/actions/util.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.941531 doot-0.7.0/doot/cmds/
--rw-rwxr--   0 john      (1000) john      (1000)        0 2023-10-17 22:05:44.000000 doot-0.7.0/doot/cmds/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.941531 doot-0.7.0/doot/cmds/__tests/
--rw-rw-r--   0 john      (1000) john      (1000)     5119 2024-04-15 22:30:11.000000 doot-0.7.0/doot/cmds/__tests/test_list_cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     2473 2024-04-15 22:30:11.000000 doot-0.7.0/doot/cmds/base_cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     2146 2024-04-15 22:30:11.000000 doot-0.7.0/doot/cmds/clean_cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     5149 2024-04-15 22:30:11.000000 doot-0.7.0/doot/cmds/graph_cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     5900 2024-04-15 22:30:11.000000 doot-0.7.0/doot/cmds/help_cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     7784 2024-04-15 22:30:11.000000 doot-0.7.0/doot/cmds/list_cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     2606 2024-04-15 22:30:11.000000 doot-0.7.0/doot/cmds/locs_cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     4222 2024-04-15 22:30:11.000000 doot-0.7.0/doot/cmds/plugins_cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     4284 2024-04-15 22:30:11.000000 doot-0.7.0/doot/cmds/run_cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     3841 2024-04-15 22:30:11.000000 doot-0.7.0/doot/cmds/step_cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     9911 2024-04-15 22:30:11.000000 doot-0.7.0/doot/cmds/stub_cmd.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.941531 doot-0.7.0/doot/control/
--rw-rwxr--   0 john      (1000) john      (1000)       10 2023-10-17 22:05:44.000000 doot-0.7.0/doot/control/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.941531 doot-0.7.0/doot/control/__tests/
--rw-rw-r--   0 john      (1000) john      (1000)     8111 2024-04-15 22:30:11.000000 doot-0.7.0/doot/control/__tests/test_locations.py
--rw-rw-r--   0 john      (1000) john      (1000)     2887 2024-04-15 22:30:11.000000 doot-0.7.0/doot/control/__tests/test_overlord.py
--rw-rw-r--   0 john      (1000) john      (1000)     5794 2024-04-15 22:30:11.000000 doot-0.7.0/doot/control/__tests/test_runner.py
--rw-rw-r--   0 john      (1000) john      (1000)    13774 2024-04-15 22:30:11.000000 doot-0.7.0/doot/control/__tests/test_tracker.py
--rw-rw-r--   0 john      (1000) john      (1000)     6410 2024-04-15 22:30:11.000000 doot-0.7.0/doot/control/base_runner.py
--rw-rw-r--   0 john      (1000) john      (1000)    18149 2024-04-15 22:30:11.000000 doot-0.7.0/doot/control/base_tracker.py
--rw-rw-r--   0 john      (1000) john      (1000)     8389 2024-04-15 22:30:11.000000 doot-0.7.0/doot/control/locations.py
--rw-rw-r--   0 john      (1000) john      (1000)      172 2023-11-03 03:34:45.000000 doot-0.7.0/doot/control/log.doot
--rw-rw-r--   0 john      (1000) john      (1000)    11575 2024-04-15 22:30:11.000000 doot-0.7.0/doot/control/overlord.py
--rw-rw-r--   0 john      (1000) john      (1000)    11246 2024-04-15 22:30:11.000000 doot-0.7.0/doot/control/runner.py
--rw-rw-r--   0 john      (1000) john      (1000)     8423 2024-04-15 22:30:11.000000 doot-0.7.0/doot/control/step_runner.py
--rw-rw-r--   0 john      (1000) john      (1000)     8503 2024-04-15 22:30:11.000000 doot-0.7.0/doot/control/tracker.py
--rw-rw-r--   0 john      (1000) john      (1000)     3546 2024-04-15 22:30:11.000000 doot-0.7.0/doot/enums.py
--rw-rw-r--   0 john      (1000) john      (1000)     3023 2024-04-14 21:07:32.000000 doot-0.7.0/doot/errors.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.941531 doot-0.7.0/doot/loaders/
--rw-rwxr--   0 john      (1000) john      (1000)        0 2023-10-17 22:05:44.000000 doot-0.7.0/doot/loaders/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.941531 doot-0.7.0/doot/loaders/__tests/
--rw-rw-r--   0 john      (1000) john      (1000)     1851 2024-04-15 22:30:11.000000 doot-0.7.0/doot/loaders/__tests/test_cmd_loader.py
--rw-rw-r--   0 john      (1000) john      (1000)     1001 2024-04-15 22:30:11.000000 doot-0.7.0/doot/loaders/__tests/test_plugin_loader.py
--rw-rw-r--   0 john      (1000) john      (1000)     7251 2024-04-15 22:30:11.000000 doot-0.7.0/doot/loaders/__tests/test_task_loader.py
--rw-rw-r--   0 john      (1000) john      (1000)     2484 2023-12-10 23:41:06.000000 doot-0.7.0/doot/loaders/cmd_loader.py
--rw-rw-r--   0 john      (1000) john      (1000)     6048 2024-04-15 22:30:11.000000 doot-0.7.0/doot/loaders/plugin_loader.py
--rw-rw-r--   0 john      (1000) john      (1000)    12082 2024-04-15 22:30:11.000000 doot-0.7.0/doot/loaders/task_loader.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.945531 doot-0.7.0/doot/mixins/
--rw-r-xr--   0 john      (1000) john      (1000)       10 2023-10-05 00:53:38.000000 doot-0.7.0/doot/mixins/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1993 2024-04-15 22:30:11.000000 doot-0.7.0/doot/mixins/enums.py
--rw-rw-r--   0 john      (1000) john      (1000)     1161 2024-04-15 22:30:11.000000 doot-0.7.0/doot/mixins/fail_handler.py
--rw-rw-r--   0 john      (1000) john      (1000)     1719 2024-04-15 22:30:11.000000 doot-0.7.0/doot/mixins/human_numbers.py
--rw-rw-r--   0 john      (1000) john      (1000)     4443 2024-04-15 22:30:11.000000 doot-0.7.0/doot/mixins/importer.py
--rw-rw-r--   0 john      (1000) john      (1000)     1185 2024-04-15 22:30:11.000000 doot-0.7.0/doot/mixins/param_spec.py
--rw-rw-r--   0 john      (1000) john      (1000)     7321 2024-04-15 22:30:11.000000 doot-0.7.0/doot/mixins/path_manip.py
--rw-rw-r--   0 john      (1000) john      (1000)     8963 2024-04-15 22:30:11.000000 doot-0.7.0/doot/mixins/zipper.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.945531 doot-0.7.0/doot/parsers/
--rw-rwxr--   0 john      (1000) john      (1000)        0 2023-10-17 22:05:44.000000 doot-0.7.0/doot/parsers/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.945531 doot-0.7.0/doot/parsers/__tests/
--rw-rw-r--   0 john      (1000) john      (1000)    13792 2024-04-15 22:30:11.000000 doot-0.7.0/doot/parsers/__tests/test_flexible.py
--rw-rw-r--   0 john      (1000) john      (1000)    10925 2024-04-15 22:30:11.000000 doot-0.7.0/doot/parsers/flexible.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.945531 doot-0.7.0/doot/reporters/
--rw-r-xr--   0 john      (1000) john      (1000)        0 2023-10-05 00:53:38.000000 doot-0.7.0/doot/reporters/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.945531 doot-0.7.0/doot/reporters/__tests/
--rw-rw-r--   0 john      (1000) john      (1000)     4152 2024-04-15 22:30:11.000000 doot-0.7.0/doot/reporters/__tests/test_stack_manager.py
--rw-rw-r--   0 john      (1000) john      (1000)     2100 2024-04-15 22:30:11.000000 doot-0.7.0/doot/reporters/__tests/test_summary_manager.py
--rw-rw-r--   0 john      (1000) john      (1000)     1232 2024-04-15 22:30:11.000000 doot-0.7.0/doot/reporters/basic_reporters.py
--rw-rw-r--   0 john      (1000) john      (1000)     1533 2024-04-14 20:23:48.000000 doot-0.7.0/doot/reporters/stack_manager.py
--rw-rw-r--   0 john      (1000) john      (1000)     2933 2024-04-14 20:23:55.000000 doot-0.7.0/doot/reporters/summary_manager.py
--rw-rw-r--   0 john      (1000) john      (1000)     1258 2024-04-15 22:30:11.000000 doot-0.7.0/doot/structs.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.945531 doot-0.7.0/doot/task/
--rw-rw-r--   0 john      (1000) john      (1000)       89 2024-01-20 20:13:07.000000 doot-0.7.0/doot/task/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.945531 doot-0.7.0/doot/task/__tests/
--rw-rw-r--   0 john      (1000) john      (1000)     1536 2024-04-15 22:30:11.000000 doot-0.7.0/doot/task/__tests/test_base_job.py
--rw-rw-r--   0 john      (1000) john      (1000)     4104 2024-04-15 22:30:11.000000 doot-0.7.0/doot/task/__tests/test_base_task.py
--rw-rw-r--   0 john      (1000) john      (1000)      749 2024-04-15 22:30:11.000000 doot-0.7.0/doot/task/__tests/test_check_locs.py
--rw-rw-r--   0 john      (1000) john      (1000)     4452 2024-04-15 22:30:11.000000 doot-0.7.0/doot/task/base_job.py
--rw-rw-r--   0 john      (1000) john      (1000)     7941 2024-04-15 22:30:11.000000 doot-0.7.0/doot/task/base_task.py
--rw-rw-r--   0 john      (1000) john      (1000)     1813 2024-04-15 22:30:11.000000 doot-0.7.0/doot/task/check_locs.py
--rw-rw-r--   0 john      (1000) john      (1000)     1771 2024-01-20 20:13:07.000000 doot-0.7.0/doot/task/specialised_jobs.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.945531 doot-0.7.0/doot/utils/
--rw-r-xr--   0 john      (1000) john      (1000)       10 2023-10-05 00:53:38.000000 doot-0.7.0/doot/utils/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.949531 doot-0.7.0/doot/utils/__tests/
--rw-rw-r--   0 john      (1000) john      (1000)     6581 2024-04-15 22:30:11.000000 doot-0.7.0/doot/utils/__tests/test_decorators.py
--rw-rw-r--   0 john      (1000) john      (1000)     1596 2024-04-15 22:30:11.000000 doot-0.7.0/doot/utils/chain_get.py
--rw-rwxr--   0 john      (1000) john      (1000)     1180 2023-10-17 22:05:44.000000 doot-0.7.0/doot/utils/check_protocol.py
--rw-rw-r--   0 john      (1000) john      (1000)     7141 2024-04-15 22:30:11.000000 doot-0.7.0/doot/utils/decorators.py
--rw-rwxr--   0 john      (1000) john      (1000)     4525 2023-10-17 22:05:44.000000 doot-0.7.0/doot/utils/log_colour.py
--rw-rw-r--   0 john      (1000) john      (1000)     5750 2024-04-15 22:30:11.000000 doot-0.7.0/doot/utils/log_config.py
--rw-rw-r--   0 john      (1000) john      (1000)     1881 2024-02-23 23:43:30.000000 doot-0.7.0/doot/utils/log_context.py
--rw-rw-r--   0 john      (1000) john      (1000)     5221 2024-04-15 22:30:11.000000 doot-0.7.0/doot/utils/mock_gen.py
--rw-rw-r--   0 john      (1000) john      (1000)     2538 2024-04-15 22:30:11.000000 doot-0.7.0/doot/utils/plugin_selector.py
--rw-rw-r--   0 john      (1000) john      (1000)     1841 2024-04-15 22:30:11.000000 doot-0.7.0/doot/utils/retrievers.py
--rw-rw-r--   0 john      (1000) john      (1000)     1909 2024-02-23 23:43:30.000000 doot-0.7.0/doot/utils/signal_handler.py
--rw-rw-r--   0 john      (1000) john      (1000)     1350 2024-04-15 22:30:11.000000 doot-0.7.0/doot/utils/testing_fixtures.py
--rw-rw-r--   0 john      (1000) john      (1000)     1787 2024-04-15 20:38:01.000000 doot-0.7.0/doot/utils/trace_helper.py
--rw-rwxr--   0 john      (1000) john      (1000)     1363 2023-10-17 22:05:44.000000 doot-0.7.0/doot/utils/url_expand.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.949531 doot-0.7.0/doot.egg-info/
--rw-r--r--   0 john      (1000) john      (1000)    10267 2024-04-15 22:34:36.000000 doot-0.7.0/doot.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)     4521 2024-04-15 22:34:36.000000 doot-0.7.0/doot.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1000) john      (1000)        1 2024-04-15 22:34:36.000000 doot-0.7.0/doot.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1000) john      (1000)       44 2024-04-15 22:34:36.000000 doot-0.7.0/doot.egg-info/entry_points.txt
--rw-rw-r--   0 john      (1000) john      (1000)      197 2024-04-15 22:34:36.000000 doot-0.7.0/doot.egg-info/requires.txt
--rw-rw-r--   0 john      (1000) john      (1000)        5 2024-04-15 22:34:36.000000 doot-0.7.0/doot.egg-info/top_level.txt
--rw-rw-r--   0 john      (1000) john      (1000)     2505 2024-04-15 22:32:56.000000 doot-0.7.0/pyproject.toml
--rw-rw-r--   0 john      (1000) john      (1000)       38 2024-04-15 22:34:36.949531 doot-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:27.000570 doot-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-17 20:06:21.000000 doot-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-04-17 20:06:27.000570 doot-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-04-17 20:06:21.000000 doot-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.972570 doot-0.7.1/doot/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.972570 doot-0.7.1/doot/__data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-04-17 20:06:21.000000 doot-0.7.1/doot/__data/aliases.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-17 20:06:21.000000 doot-0.7.1/doot/__data/constants.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-17 20:06:21.000000 doot-0.7.1/doot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-17 20:06:21.000000 doot-0.7.1/doot/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.976570 doot-0.7.1/doot/__templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-17 20:06:21.000000 doot-0.7.1/doot/__templates/basic_toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-17 20:06:21.000000 doot-0.7.1/doot/__templates/stub_task_py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-17 20:06:21.000000 doot-0.7.1/doot/__templates/tasks_toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.976570 doot-0.7.1/doot/__tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-17 20:06:21.000000 doot-0.7.1/doot/__tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-17 20:06:21.000000 doot-0.7.1/doot/__tests/test_inits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.976570 doot-0.7.1/doot/_abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_abstract/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_abstract/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_abstract/dbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_abstract/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_abstract/overlord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_abstract/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_abstract/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_abstract/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_abstract/structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_abstract/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.980569 doot-0.7.1/doot/_structs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.980569 doot-0.7.1/doot/_structs/__tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_action_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_code_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8946 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_key_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_key_multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_key_path_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_key_string_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_key_type_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_param_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_task_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/__tests/test_task_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/action_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/code_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27177 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/param_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/sname.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/structured_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/task_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12733 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/task_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/toml_loc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-17 20:06:21.000000 doot-0.7.1/doot/_structs/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.984570 doot-0.7.1/doot/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.988570 doot-0.7.1/doot/actions/__tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/__tests/test_base_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/__tests/test_control_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/__tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/__tests/test_job_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/__tests/test_job_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/__tests/test_job_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/__tests/test_job_queuing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/__tests/test_postbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/__tests/test_shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/__tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/base_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/control_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12967 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/job_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/job_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/job_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/job_queuing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/postbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/speak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/templater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-17 20:06:21.000000 doot-0.7.1/doot/actions/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.988570 doot-0.7.1/doot/cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:21.000000 doot-0.7.1/doot/cmds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.988570 doot-0.7.1/doot/cmds/__tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-17 20:06:21.000000 doot-0.7.1/doot/cmds/__tests/test_list_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-17 20:06:21.000000 doot-0.7.1/doot/cmds/base_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-17 20:06:21.000000 doot-0.7.1/doot/cmds/clean_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-04-17 20:06:21.000000 doot-0.7.1/doot/cmds/graph_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5900 2024-04-17 20:06:21.000000 doot-0.7.1/doot/cmds/help_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-04-17 20:06:21.000000 doot-0.7.1/doot/cmds/list_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-17 20:06:21.000000 doot-0.7.1/doot/cmds/locs_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-17 20:06:21.000000 doot-0.7.1/doot/cmds/plugins_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-17 20:06:21.000000 doot-0.7.1/doot/cmds/run_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-17 20:06:21.000000 doot-0.7.1/doot/cmds/step_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-17 20:06:21.000000 doot-0.7.1/doot/cmds/stub_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.992570 doot-0.7.1/doot/control/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 20:06:21.000000 doot-0.7.1/doot/control/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.992570 doot-0.7.1/doot/control/__tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-04-17 20:06:21.000000 doot-0.7.1/doot/control/__tests/test_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-17 20:06:21.000000 doot-0.7.1/doot/control/__tests/test_overlord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-17 20:06:21.000000 doot-0.7.1/doot/control/__tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13774 2024-04-17 20:06:21.000000 doot-0.7.1/doot/control/__tests/test_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-04-17 20:06:21.000000 doot-0.7.1/doot/control/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19677 2024-04-17 20:06:21.000000 doot-0.7.1/doot/control/base_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-04-17 20:06:21.000000 doot-0.7.1/doot/control/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11575 2024-04-17 20:06:21.000000 doot-0.7.1/doot/control/overlord.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-04-17 20:06:21.000000 doot-0.7.1/doot/control/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-04-17 20:06:21.000000 doot-0.7.1/doot/control/step_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-04-17 20:06:21.000000 doot-0.7.1/doot/control/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-04-17 20:06:21.000000 doot-0.7.1/doot/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-17 20:06:21.000000 doot-0.7.1/doot/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.992570 doot-0.7.1/doot/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:21.000000 doot-0.7.1/doot/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.992570 doot-0.7.1/doot/loaders/__tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-17 20:06:21.000000 doot-0.7.1/doot/loaders/__tests/test_cmd_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-17 20:06:21.000000 doot-0.7.1/doot/loaders/__tests/test_plugin_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-04-17 20:06:21.000000 doot-0.7.1/doot/loaders/__tests/test_task_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-17 20:06:21.000000 doot-0.7.1/doot/loaders/cmd_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-17 20:06:21.000000 doot-0.7.1/doot/loaders/plugin_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-04-17 20:06:21.000000 doot-0.7.1/doot/loaders/task_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.992570 doot-0.7.1/doot/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 20:06:21.000000 doot-0.7.1/doot/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-17 20:06:21.000000 doot-0.7.1/doot/mixins/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-17 20:06:21.000000 doot-0.7.1/doot/mixins/fail_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-17 20:06:21.000000 doot-0.7.1/doot/mixins/human_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-17 20:06:21.000000 doot-0.7.1/doot/mixins/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-17 20:06:21.000000 doot-0.7.1/doot/mixins/param_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-04-17 20:06:21.000000 doot-0.7.1/doot/mixins/path_manip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-04-17 20:06:21.000000 doot-0.7.1/doot/mixins/zipper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.992570 doot-0.7.1/doot/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:21.000000 doot-0.7.1/doot/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.992570 doot-0.7.1/doot/parsers/__tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13792 2024-04-17 20:06:21.000000 doot-0.7.1/doot/parsers/__tests/test_flexible.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10925 2024-04-17 20:06:21.000000 doot-0.7.1/doot/parsers/flexible.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.996570 doot-0.7.1/doot/reporters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:21.000000 doot-0.7.1/doot/reporters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.996570 doot-0.7.1/doot/reporters/__tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-17 20:06:21.000000 doot-0.7.1/doot/reporters/__tests/test_stack_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-17 20:06:21.000000 doot-0.7.1/doot/reporters/__tests/test_summary_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-17 20:06:21.000000 doot-0.7.1/doot/reporters/basic_reporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-17 20:06:21.000000 doot-0.7.1/doot/reporters/stack_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-17 20:06:21.000000 doot-0.7.1/doot/reporters/summary_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-17 20:06:21.000000 doot-0.7.1/doot/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.996570 doot-0.7.1/doot/task/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-17 20:06:21.000000 doot-0.7.1/doot/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:26.996570 doot-0.7.1/doot/task/__tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-17 20:06:21.000000 doot-0.7.1/doot/task/__tests/test_base_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-17 20:06:21.000000 doot-0.7.1/doot/task/__tests/test_base_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-17 20:06:21.000000 doot-0.7.1/doot/task/__tests/test_check_locs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-04-17 20:06:21.000000 doot-0.7.1/doot/task/base_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7996 2024-04-17 20:06:21.000000 doot-0.7.1/doot/task/base_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-17 20:06:21.000000 doot-0.7.1/doot/task/check_locs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-17 20:06:21.000000 doot-0.7.1/doot/task/specialised_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:27.000570 doot-0.7.1/doot/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:27.000570 doot-0.7.1/doot/utils/__tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/__tests/test_action_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/action_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/chain_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/check_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9018 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/log_colour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/log_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/mock_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/plugin_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/signal_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/testing_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/trace_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-17 20:06:21.000000 doot-0.7.1/doot/utils/url_expand.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:06:27.000570 doot-0.7.1/doot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-04-17 20:06:26.000000 doot-0.7.1/doot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-04-17 20:06:26.000000 doot-0.7.1/doot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:06:26.000000 doot-0.7.1/doot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 20:06:26.000000 doot-0.7.1/doot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-17 20:06:26.000000 doot-0.7.1/doot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-17 20:06:26.000000 doot-0.7.1/doot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-17 20:06:21.000000 doot-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 20:06:27.000570 doot-0.7.1/setup.cfg
```

### Comparing `doot-0.7.0/LICENSE` & `doot-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/PKG-INFO` & `doot-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doot
-Version: 0.7.0
+Version: 0.7.1
 Summary: An opinionated, TOML based task runner
 Author-email: jgrey <jgrey.n.plus.one@gmail.com>
 License:  ACAB License © 2022-12-09 John Grey
         
         
         To the maximum extent applicable by law, and any licenses of components of this work:
         
@@ -67,15 +67,15 @@
 Requires-Dist: pytest-mock; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pipreqs; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 
 ![doot](https://github.com/jgrey4296/doot/assets/5943270/170a5631-6175-4d92-8d66-e26aa2c2e472)
 # doot
-Version : 0.7.0  
+Version : 0.7.1  
 Author  : John Grey  
 Date    : 2022-12-09  
 
 ## Overview
 This started out as an opinionated rewrite of the [doit](https://pydoit.org/contents.html) task runner.
 For other, more mature alternatives, see [Luigi](https://github.com/spotify/luigi), and [SnakeMake](https://github.com/snakemake/snakemake)
 and, of course, [GNU Make](https://www.gnu.org/software/make/).
```

### Comparing `doot-0.7.0/README.md` & `doot-0.7.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ![doot](https://github.com/jgrey4296/doot/assets/5943270/170a5631-6175-4d92-8d66-e26aa2c2e472)
 # doot
-Version : 0.7.0  
+Version : 0.7.1  
 Author  : John Grey  
 Date    : 2022-12-09  
 
 ## Overview
 This started out as an opinionated rewrite of the [doit](https://pydoit.org/contents.html) task runner.
 For other, more mature alternatives, see [Luigi](https://github.com/spotify/luigi), and [SnakeMake](https://github.com/snakemake/snakemake)
 and, of course, [GNU Make](https://www.gnu.org/software/make/).
```

### Comparing `doot-0.7.0/doot/__data/aliases.toml` & `doot-0.7.1/doot/__data/aliases.toml`

 * *Files 2% similar despite different names*

```diff
@@ -55,17 +55,18 @@
 "dir!"    =  "doot.actions.io:EnsureDirectory"
 "delete!" =  "doot.actions.io:DeleteAction"
 "break!"  =  "doot.actions.util:action_debugger"
 "type!"   =  "doot.actions.util:typecheck"
 
 [[doot.aliases.action]] # control flow
 # Map {alias} -> CodeRef String
-"exists?"       = "doot.actions.control_flow:SkipIfFileExists"
-"ext?"          = "doot.actions.control_flow:SkipUnlessSuffix"
-"pred?"         = "doot.actions.control_flow:CancelOnPredicateAction"
+"exists?"       = "doot.actions.control_flow:FileExistsCheck"
+"ext?"          = "doot.actions.control_flow:SuffixCheck"
+"relative?"     = "doot.actions.control_flow:RelativeCheck"
+"pred?"         = "doot.actions.control_flow:PredicateCheck"
 "installed?"    = "doot.actions.control_flow:AssertInstalled"
 "dir?"          = "doot.actions.io:EnsureDirectory"
 "wait"          = "doot.actions.control_flow:WaitAction"
 
 [[doot.aliases.action]] # compressions
 # Map {alias} -> CodeRef String
 "json.read"     =  "doot.actions.json:ReadJson"
```

### Comparing `doot-0.7.0/doot/__data/constants.toml` & `doot-0.7.1/doot/__data/constants.toml`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/__init__.py` & `doot-0.7.1/doot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 ##-- logging
 logging         = logmod.getLogger(__name__)
 printer         = logmod.getLogger("doot._printer")
 ##-- end logging
 
 # Global, single points of truth:
-__version__          : Final[str]         = "0.7.0"
+__version__          : Final[str]         = "0.7.1"
 
 CONSTANT_PREFIX      : Final[str]         = "doot.constants"
 ALIAS_PREFIX         : Final[str]         = "doot.aliases"
 TOOL_PREFIX          : Final[str]         = "tool.doot"
 
 config               : TG.TomlGuard       = TG.TomlGuard() # doot config
 constants            : TG.TomlGuard       = TG.TomlGuard.load(constants_file).remove_prefix(CONSTANT_PREFIX)
```

### Comparing `doot-0.7.0/doot/__main__.py` & `doot-0.7.1/doot/__main__.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/__templates/basic_toml` & `doot-0.7.1/doot/__templates/basic_toml`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/__templates/stub_task_py` & `doot-0.7.1/doot/__templates/stub_task_py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/__tests/test_basic.py` & `doot-0.7.1/doot/__tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/__tests/test_inits.py` & `doot-0.7.1/doot/__tests/test_inits.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_abstract/__init__.py` & `doot-0.7.1/doot/_abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_abstract/cmd.py` & `doot-0.7.1/doot/_abstract/cmd.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_abstract/control.py` & `doot-0.7.1/doot/_abstract/control.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_abstract/dbm.py` & `doot-0.7.1/doot/_abstract/dbm.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_abstract/loader.py` & `doot-0.7.1/doot/_abstract/loader.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_abstract/overlord.py` & `doot-0.7.1/doot/_abstract/overlord.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_abstract/parser.py` & `doot-0.7.1/doot/_abstract/parser.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_abstract/policy.py` & `doot-0.7.1/doot/_abstract/policy.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_abstract/reporter.py` & `doot-0.7.1/doot/_abstract/reporter.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_abstract/structs.py` & `doot-0.7.1/doot/_abstract/structs.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_abstract/task.py` & `doot-0.7.1/doot/_abstract/task.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_structs/__tests/test_action_spec.py` & `doot-0.7.1/doot/_structs/__tests/test_action_spec.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_structs/__tests/test_artifact.py` & `doot-0.7.1/doot/_structs/__tests/test_artifact.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,156 +11,133 @@
                     TypeVar, cast)
 import warnings
 
 import pytest
 
 logging = logmod.root
 
-##-- pytest reminder
-# caplog
-# mocker.patch | patch.object | patch.multiple | patch.dict | stopall | stop | spy | stub
-# pytest.mark.filterwarnings
-# pytest.parameterize
-# pytest.skip | skipif | xfail
-# with pytest.deprecated_call
-# with pytest.raises
-# with pytest.warns(warntype)
-
-##-- end pytest reminder
-
 import doot
 doot._test_setup()
 from doot._structs.artifact import DootTaskArtifact
 
 class TestTaskArtifact:
 
-    @pytest.fixture(scope="function")
-    def setup(self):
-        pass
-
-    @pytest.fixture(scope="function")
-    def cleanup(self):
-        pass
-
     def test_initial(self):
         basic = DootTaskArtifact.build(pl.Path("a/b/c"))
         assert(basic is not None)
 
     def test_self_eq(self):
         basic = DootTaskArtifact.build(pl.Path("a/b/c"))
         assert(basic is basic)
         assert(basic == basic)
 
-
     def test_eq(self):
         basic = DootTaskArtifact.build(pl.Path("a/b/c"))
         basic2 = DootTaskArtifact.build(pl.Path("a/b/c"))
         assert(basic is not basic2)
         assert(basic == basic2)
 
-
     def test_neq(self):
         basic = DootTaskArtifact.build(pl.Path("a/b/c"))
         basic2 = DootTaskArtifact.build(pl.Path("a/b/d"))
         assert(basic is not basic2)
         assert(basic != basic2)
 
+    def test_definite_to_indefinite_contains(self):
+
+        definite = DootTaskArtifact.build(pl.Path("a/b/c.py"))
+        indef    = DootTaskArtifact.build(pl.Path("a/b/*.py"))
+        assert(definite in indef)
+
+class TestDefiniteArtifact:
 
     def test_definite(self):
         basic = DootTaskArtifact.build(pl.Path("a/b/c"))
         assert(basic.is_definite)
         assert(basic._definite_stem)
         assert(basic._definite_suffix)
 
+class TestIndefiniteArtifact:
 
     def test_indefinite_stem(self):
         basic = DootTaskArtifact.build(pl.Path("a/b/*.py"))
         assert(not basic.is_definite)
         assert(not basic._definite_stem)
         assert(basic._definite_suffix)
 
-
     def test_indefinite_suffix(self):
         basic = DootTaskArtifact.build(pl.Path("a/b/c.*"))
         assert(not basic.is_definite)
         assert(basic._definite_stem)
         assert(not basic._definite_suffix)
 
-
     def test_indefinite_path(self):
         basic = DootTaskArtifact.build(pl.Path("a/*/c.py"))
         assert(not basic.is_definite)
         assert(basic._definite_stem)
         assert(basic._definite_suffix)
 
-
     def test_recursive_indefinite(self):
         basic = DootTaskArtifact.build(pl.Path("a/**/c.py"))
         assert(not basic.is_definite)
         assert(basic._definite_stem)
         assert(basic._definite_suffix)
 
+    def test_indef_suffix_contains(self):
 
-    def test_stem_contains(self):
-        definite = DootTaskArtifact.build(pl.Path("a/b/c.py"))
-        indef    = DootTaskArtifact.build(pl.Path("a/b/*.py"))
-        assert(definite in indef)
-
-
-    def test_not_contains_reverse(self):
-        definite = DootTaskArtifact.build(pl.Path("a/b/c.py"))
-        indef    = DootTaskArtifact.build(pl.Path("a/b/*.py"))
-        assert(indef not in definite)
-
-
-    def test_suffix_contains(self):
         definite = DootTaskArtifact.build(pl.Path("a/b/c.py"))
         indef    = DootTaskArtifact.build(pl.Path("a/b/c.*"))
         assert(definite in indef)
 
+    def test_indef_suffix_contain_fail(self):
 
-    def test_suffix_contain_fail(self):
         definite = DootTaskArtifact.build(pl.Path("a/b/d.py"))
         indef    = DootTaskArtifact.build(pl.Path("a/b/c.*"))
         assert(definite not in indef)
 
+    def test_indef_path_contains(self):
 
-    def test_path_contains(self):
         definite = DootTaskArtifact.build(pl.Path("a/b/c.py"))
         indef    = DootTaskArtifact.build(pl.Path("a/*/c.py"))
         assert(definite in indef)
 
+    def test_indef_path_contain_fail(self):
 
-    def test_path_contain_fail(self):
         definite = DootTaskArtifact.build(pl.Path("b/b/c.py"))
         indef    = DootTaskArtifact.build(pl.Path("a/*/c.py"))
         assert(definite not in indef)
 
+    def test_indefinite_to_definite_contains_fail(self):
+
+        definite = DootTaskArtifact.build(pl.Path("a/b/c.py"))
+        indef    = DootTaskArtifact.build(pl.Path("a/b/*.py"))
+        assert(indef not in definite)
+
+    def test_indef_recursive_contains(self):
 
-    def test_path_recursive_contains(self):
         definite = DootTaskArtifact.build(pl.Path("a/b/c.py"))
         indef    = DootTaskArtifact.build(pl.Path("a/**/c.py"))
         assert(definite in indef)
 
+    def test_indef_recursive_contain_fail(self):
 
-    def test_path_recursive_contain_fail(self):
         definite = DootTaskArtifact.build(pl.Path("b/b/c.py"))
         indef    = DootTaskArtifact.build(pl.Path("a/**/c.py"))
         assert(definite not in indef)
 
+    def test_indef_multi_recursive_contains(self):
 
-    def test_multi_depth_recursive_contains(self):
         definite = DootTaskArtifact.build(pl.Path("a/b/d/e/f/c.py"))
         indef    = DootTaskArtifact.build(pl.Path("a/**/c.py"))
         assert(definite in indef)
 
+    def test_indef_root_recursive_contains(self):
 
-    def test_root_recursive_contains(self):
         definite = DootTaskArtifact.build(pl.Path("a/b/d/e/f/c.py"))
         indef    = DootTaskArtifact.build(pl.Path("**/c.py"))
         assert(definite in indef)
 
+    def test_indef_multi_component_contains(self):
 
-    def test_multi_indef_component_contains(self):
         definite = DootTaskArtifact.build(pl.Path("a/b/d/e/f/c.py"))
         indef    = DootTaskArtifact.build(pl.Path("**/*.*"))
         assert(definite in indef)
```

### Comparing `doot-0.7.0/doot/_structs/__tests/test_code_ref.py` & `doot-0.7.1/doot/_structs/__tests/test_code_ref.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_structs/__tests/test_formatter.py` & `doot-0.7.1/doot/_structs/__tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_structs/__tests/test_key.py` & `doot-0.7.1/doot/_structs/__tests/test_key.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_structs/__tests/test_key_multi.py` & `doot-0.7.1/doot/_structs/__tests/test_key_multi.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_structs/__tests/test_key_path_expansion.py` & `doot-0.7.1/doot/_structs/__tests/test_key_path_expansion.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_structs/__tests/test_key_string_expansion.py` & `doot-0.7.1/doot/_structs/__tests/test_key_string_expansion.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_structs/__tests/test_key_type_expansion.py` & `doot-0.7.1/doot/_structs/__tests/test_key_type_expansion.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_structs/__tests/test_param_spec.py` & `doot-0.7.1/doot/_structs/__tests/test_param_spec.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_structs/__tests/test_stub.py` & `doot-0.7.1/doot/_structs/__tests/test_stub.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_structs/__tests/test_task_name.py` & `doot-0.7.1/doot/_structs/__tests/test_task_name.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_structs/__tests/test_task_spec.py` & `doot-0.7.1/doot/_structs/__tests/test_task_spec.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_structs/action_spec.py` & `doot-0.7.1/doot/_structs/action_spec.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_structs/artifact.py` & `doot-0.7.1/doot/_structs/artifact.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_structs/code_ref.py` & `doot-0.7.1/doot/_structs/code_ref.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_structs/key.py` & `doot-0.7.1/doot/_structs/key.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,32 +42,28 @@
 import string
 from tomlguard import TomlGuard
 import doot
 import doot.errors
 from doot._structs.code_ref import DootCodeReference
 from doot._abstract.structs import SpecStruct_p
 from doot.utils.chain_get import DootKeyGetter
-from doot.utils.decorators import DootDecorator
+from doot.utils.decorators import DootDecorator, DecorationUtils
 
 KEY_PATTERN                                = doot.constants.patterns.KEY_PATTERN
 MAX_KEY_EXPANSIONS                         = doot.constants.patterns.MAX_KEY_EXPANSIONS
 STATE_TASK_NAME_K                          = doot.constants.patterns.STATE_TASK_NAME_K
 
 PATTERN        : Final[re.Pattern]         = re.compile(KEY_PATTERN)
 FAIL_PATTERN   : Final[re.Pattern]         = re.compile("[^a-zA-Z_{}/0-9-]")
-KEYS_HANDLED   : Final[str]                = "_doot_keys_handler"
-ORIG_ARGS      : Final[str]                = "_doot_orig_args"
-KEY_ANNOTS     : Final[str]                = "_doot_keys"
 EXPANSION_HINT : Final[str]                = "_doot_expansion_hint"
 HELP_HINT      : Final[str]                = "_doot_help_hint"
-FUNC_WRAPPED   : Final[str]                = "__wrapped__"
 
-class KWrapper(DootDecorator):
+class KeyDecorator:
     """ Decorators for actions
-    Kwrapper is accessible as DootKey.kwrap
+    KeyDecorator is accessible as DootKey.kwrap
 
     It registers arguments on an action and extracts them from the spec and state automatically.
 
     provides: expands/paths/types/requires/returns/args/kwargs/redirects/redirects_many
 
     The kwarg 'hint' takes a dict and passes the contents to the relevant expansion method as kwargs
 
@@ -75,218 +71,84 @@
     the name of the expansion is expected to be the name of the action parameter,
     with a "_" prepended if the name would conflict with a keyword., or with "_ex" as a suffix
     eg: @DootKey.kwrap.paths("from") -> def __call__(self, spec, state, _from):...
     or: @DootKey.kwrap.paths("from") -> def __call__(self, spec, state, from_ex):...
     """
 
     @staticmethod
-    def _annotate_keys(f, keys:list) -> bool:
-        """ cache original args, and cache declared keys """
-        if hasattr(f, FUNC_WRAPPED): # Deal with the actual function, not any decorators
-            return KWrapper._annotate_keys(f.__wrapped__, keys)
-
-        if not hasattr(f, ORIG_ARGS): # store the original arguments for easy access
-            setattr(f, ORIG_ARGS, f.__code__.co_varnames[:f.__code__.co_argcount])
-
-        if not hasattr(f, KEY_ANNOTS): # ensure theres a place for annotations
-            setattr(f, KEY_ANNOTS, [])
-
-        # prepend annotations, so written decorator order is the same as written arg order:
-        # (ie: @wrap(x) @wrap(y) @wrap(z) def f (x, y, z), even though z's decorator is applied first
-        new_annotations = keys + getattr(f, KEY_ANNOTS)
-        setattr(f, KEY_ANNOTS, new_annotations)
-
-        # run the key check
-        if not KWrapper._check_keys(f, getattr(f, KEY_ANNOTS)):
-            raise doot.errors.DootKeyError("Annotations do not match signature", getattr(f, ORIG_ARGS, []), getattr(f, KEY_ANNOTS), f.__qualname__)
-
-        return True
-
-    @staticmethod
-    def _annotate_non_expansions(f, keys:list, type_="in") -> bool:
-        """
-        Annotate required inputs and output
-        """
-        if hasattr(f, FUNC_WRAPPED):
-            return KWrapper._annotate_non_expansions(f.__wrapped__, keys)
-
-    @staticmethod
-    def _check_keys(f, keys, offset=0) -> bool:
-        """ test declared args to a list of keys """
-        if hasattr(f, ORIG_ARGS):
-            code_args           = getattr(f, ORIG_ARGS)
-            code_argcount       = len(code_args)
-        else:
-            code_argcount           = f.__code__.co_argcount
-            code_args               = f.__code__.co_varnames[:code_argcount]
-
-        result                  = True
-        if code_args[0]         == "self":
-            code_args           = code_args[1:]
-
-        # First two params should always be spec and state
-        result &= code_args[:2] == ("spec", "state")
-
-        # The rest should match keys
-        for actual, expected in zip(code_args[:1+offset:-1], keys[::-1]):
-            match expected:
-                case DootMultiKey():
-                    pass
-                case DootSimpleKey() | str() if actual.startswith("_"):
-                    pass
-                case DootSimpleKey() | str():
-                    result &= ((actual == expected) or (actual == f"{expected}_ex"))
-
-        return result
-
-    @staticmethod
-    def _add_key_handler(f):
-        """ idempotent key handler so decorated functions dont add unnecessary stack frames """
-        if DootDecorator.has_annotations(f):
-            return f
-
-        DootDecorator.truncate_signature(f)
-
-        match getattr(f, ORIG_ARGS)[0]:
-            case "self": # The method form handler
-
-                @ftz.wraps(f)
-                def action_expands(self, spec, state, *call_args, **kwargs):
-                    try:
-                        expansions = [x(spec, state) for x in getattr(f, KEY_ANNOTS)]
-                    except KeyError as err:
-                        printer.warning("Action State Expansion Failure: %s", err)
-                        return False
-                    all_args = (*call_args, *expansions)
-                    return f(self, spec, state, *all_args, **kwargs)
-            case _: # The function form handler
-
-                @ftz.wraps(f)
-                def action_expands(spec, state, *call_args, **kwargs):
-                    try:
-                        expansions = [x(spec, state) for x in getattr(f, KEY_ANNOTS)]
-                    except KeyError as err:
-                        printer.warning("Action State Expansion Failure: %s", err)
-                        return False
-                    all_args = (*call_args, *expansions)
-                    return f(spec, state, *all_args, **kwargs)
-
-        DootDecorator.annotate(action_expands, {KEYS_HANDLED})
-        return action_expands
-
-
-    @staticmethod
-    def taskname(f):
-        KWrapper._annotate_keys(f, [DootKey.build(STATE_TASK_NAME_K, exp_hint="type")])
-        return KWrapper._add_key_handler(f)
+    def taskname(fn):
+        keys = [DootKey.build(STATE_TASK_NAME_K, exp_hint="type")]
+        return DecorationUtils.prepare_expansion(keys, fn)
 
     @staticmethod
     def expands(*args, hint:dict|None=None, **kwargs):
         """ mark an action as using expanded string keys """
         exp_hint = {"expansion": "str", "kwargs" : hint or {} }
-        keys = [DootKey.build(x, exp_hint=exp_hint, **kwargs) for x in args]
-
-        def expand_wrapper(f):
-            KWrapper._annotate_keys(f, keys)
-            return KWrapper._add_key_handler(f)
-
-        return expand_wrapper
+        keys     = [DootKey.build(x, exp_hint=exp_hint, **kwargs) for x in args]
+        return ftz.partial(DecorationUtils.prepare_expansion, keys)
 
     @staticmethod
     def paths(*args, hint:dict|None=None, **kwargs):
         """ mark an action as using expanded path keys """
         exp_hint = {"expansion": "path", "kwargs" : hint or {} }
         keys = [DootKey.build(x, exp_hint=exp_hint, **kwargs) for x in args]
-
-        def expand_wrapper(f):
-            KWrapper._annotate_keys(f, keys)
-            return KWrapper._add_key_handler(f)
-
-        return expand_wrapper
+        return ftz.partial(DecorationUtils.prepare_expansion, keys)
 
     @staticmethod
     def types(*args, hint:dict|None=None, **kwargs):
         """ mark an action as using raw type keys """
         exp_hint = {"expansion": "type", "kwargs" : hint or {} }
         keys = [DootKey.build(x, exp_hint=exp_hint, **kwargs) for x in args]
-
-        def expand_wrapper(f):
-            KWrapper._annotate_keys(f, keys)
-            return KWrapper._add_key_handler(f)
-
-        return expand_wrapper
+        return ftz.partial(DecorationUtils.prepare_expansion, keys)
 
     @staticmethod
-    def args(f):
+    def args(fn):
         """ mark an action as using spec.args """
         # TODO handle expansion hint for the args
-        KWrapper._annotate_keys(f, [DootArgsKey("args")])
-        return KWrapper._add_key_handler(f)
+        keys = [DootArgsKey("args")]
+        return DecorationUtils.prepare_expansion(keys, fn)
 
     @staticmethod
-    def kwargs(f):
+    def kwargs(fn):
         """ mark an action as using spec.args """
-        KWrapper._annotate_keys(f, [DootKwargsKey("kwargs")])
-        return KWrapper._add_key_handler(f)
+        keys = [DootKwargsKey("kwargs")]
+        return DecorationUtils.prepare_expansion(keys, fn)
 
     @staticmethod
     def redirects(*args):
         """ mark an action as using redirection keys """
         keys = [DootKey.build(x, exp_hint="redirect") for x in args]
-
-        def expand_wrapper(f):
-            KWrapper._annotate_keys(f, keys)
-            return KWrapper._add_key_handler(f)
-
-        return expand_wrapper
+        return ftz.partial(DecorationUtils.prepare_expansion, keys)
 
     @staticmethod
     def redirects_many(*args, **kwargs):
         """ mark an action as using redirection key lists """
         keys = [DootKey.build(x, exp_hint="redirect_multi") for x in args]
-
-        def expand_wrapper(f):
-            KWrapper._annotate_keys(f, keys)
-            return KWrapper._add_key_handler(f)
-
-        return expand_wrapper
+        return ftz.partial(DecorationUtils.prepare_expansion, keys)
 
     @staticmethod
     def requires(*args, **kwargs):
-        """ mark an action as requiring certain keys to be passed in """
+        """ TODO mark an action as requiring certain keys to be passed in """
         keys = [DootKey.build(x, **kwargs) for x in args]
-
-        def expand_wrapper(f):
-            KWrapper._annotate_non_expansions(f, keys)
-            return f
-
-        return expand_wrapper
+        # return ftz.partial(DecorationUtils.prepare_expansion, keys)
+        return lambda x: x
 
     @staticmethod
     def returns(*args, **kwargs):
         """ mark an action as needing to return certain keys """
         keys = [DootKey.build(x, **kwargs) for x in args]
-
-        def expand_wrapper(f):
-            KWrapper._annotate_non_expansions(f, keys)
-            return f
-
-        return expand_wrapper
+        # return ftz.partial(DecorationUtils.prepare_expansion, keys)
+        return lambda x: x
 
     @staticmethod
     def references(*args, **kwargs):
         """ mark keys to use as to_coderef imports """
         exp_hint = {"expansion": "coderef", "kwargs" : {} }
         keys = [DootKey.build(x, exp_hint=exp_hint, **kwargs) for x in args]
-
-        def expand_wrapper(f):
-            KWrapper._annotate_keys(f, keys)
-            return KWrapper._add_key_handler(f)
-
-        return expand_wrapper
+        return ftz.partial(DecorationUtils.prepare_expansion, keys)
 
 class DootFormatter(string.Formatter):
     """
       A Formatter for expanding arguments based on action spec kwargs, and task state, and cli args
     """
     _fmt                = None
 
@@ -367,16 +229,16 @@
 
       DootSimpleKeys are strings, wrapped in {} when used in toml.
       so DootKey.build("blah") -> DootSimpleKey("blah") -> DootSimpleKey('blah').form =="{blah}" -> [toml] aValue = "{blah}"
 
       DootMultiKeys are containers of a string `value`, and a list of SimpleKeys the value contains.
       So DootKey.build("{blah}/{bloo}") -> DootMultiKey("{blah}/{bloo}", [DootSimpleKey("blah", DootSimpleKey("bloo")]) -> .form == "{blah}/{bloo}"
     """
-    dec   = KWrapper
-    kwrap = KWrapper
+    dec   = KeyDecorator
+    kwrap = KeyDecorator
 
     @staticmethod
     def build(s:str|DootKey|pl.Path|dict, *, strict=False, explicit=False, exp_hint:str|dict=None, help=None) -> DootKey:
         """ Make an appropriate DootKey based on input value
           Can only create MultiKeys if strict = False,
           if explicit, only keys wrapped in {} are made, everything else is returned untouched
           if strict, then only simple keys can be returned
```

### Comparing `doot-0.7.0/doot/_structs/param_spec.py` & `doot-0.7.1/doot/_structs/param_spec.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_structs/sname.py` & `doot-0.7.1/doot/_structs/sname.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_structs/structured_name.py` & `doot-0.7.1/doot/_structs/structured_name.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_structs/stub.py` & `doot-0.7.1/doot/_structs/stub.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_structs/task_name.py` & `doot-0.7.1/doot/_structs/task_name.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,18 @@
         group = self.group
         tail = self.subseparator.join([str(x) if not isinstance(x, UUID) else "<UUID>" for x in self.tail])
         return "{}{}{}".format(group, self.separator, tail)
 
     def root(self) -> DootTaskName:
         return DootTaskName.build(f"{self.head_str()}{self.separator}{self.tail[0]}")
 
-    def task_head(self):
+    def task_head(self) -> DootTaskName:
+        if self.tail[-1] == doot.constants.patterns.SUBTASKED_HEAD:
+            return self
+
         return self.subtask(doot.constants.patterns.SUBTASKED_HEAD)
 
     def subtask(self, *subtasks, subgroups:list[str]|None=None) -> DootTaskName:
         args = self.args.copy() if self.args else None
         subs = []
         match [x for x in subtasks if x != None]:
             case [int() as i, DootTaskName() as x]:
```

### Comparing `doot-0.7.0/doot/_structs/task_spec.py` & `doot-0.7.1/doot/_structs/task_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,17 +62,14 @@
         match key:
             case "extra" if val is not None:
                 extra_data.update(dict(val))
             case "extra":
                 pass
             case "print_levels":
                 core_data["print_levels"] = TomlGuard(val)
-            case "active_when":
-                processed = _prepare_deps(val)
-                core_data["active_when"] = processed
             case "required_for":
                 processed = _prepare_deps(val)
                 core_data["required_for"] = processed
             case "depends_on":
                 processed = _prepare_deps(val)
                 core_data["depends_on"] = processed
             case "setup":
@@ -109,25 +106,24 @@
                 results.append(DootActionSpec.build(x))
             case { "loc": filename }:
                 results.append(DootTaskArtifact.build(x))
             case str() if x.startswith(doot.constants.patterns.FILE_DEP_PREFIX):
                 results.append(DootTaskArtifact.build(x))
             case str() if doot.constants.patterns.TASK_SEP in x:
                 results.append(DootTaskName.build(x))
-            case DootTaskName() | DootTaskArtifact():
+            case DootTaskName() | DootTaskArtifact() | DootActionSpec():
                 results.append(x)
             case _:
                 raise doot.errors.DootInvalidConfig(f"Unrecognised task pre/post dependency form. (Remember: files are prefixed with `{doot.constants.patterns.FILE_DEP_PREFIX}`, tasks are in the form group::name)", x, source)
 
     return results
 
 def _prepare_ctor(ctor, mixins) -> DootTaskName|DootCodeReference:
     match ctor:
         case None:
-
             default_alias = doot.constants.entrypoints.DEFAULT_TASK_CTOR_ALIAS
             coderef_str   = doot.aliases.task[default_alias]
             return DootCodeReference.build(coderef_str).add_mixins(*mixins)
         case EntryPoint():
             return DootCodeReference.build(ctor).add_mixins(*mixins)
         case DootTaskName() if bool(mixins):
             raise TypeError("Task name ctor can't take mixins")
@@ -169,15 +165,14 @@
     version                      : str                                                                     = field(default="0.1")
     # TODO version               : dict                                                                    = field(default_factory=dict)
     print_levels                 : TomlGuard                                                               = field(default_factory=TomlGuard)
     flags                        : TaskFlags                                                               = field(default=TaskFlags.TASK)
 
     extra                        : TomlGuard                                                               = field(default_factory=TomlGuard)
 
-    inject                       : list[str]                                                               = field(default_factory=list) # For jobs
     queue_behaviour              : TaskQueueMeta                                                 = field(default=TaskQueueMeta.default)
 
     @staticmethod
     def build(data:TomlGuard|dict|DootTaskName|str):
         match data:
             case TomlGuard() | dict():
                 return DootTaskSpec.from_dict(data)
@@ -235,16 +230,20 @@
                     specialized[field] = self.ctor
                 case "actions":
                     specialized[field] = self.actions + data.actions
                 case "depends_on":
                     specialized["depends_on"] = self.depends_on[:] + data.depends_on[:]
                 case "required_for":
                     specialized["required_for"] = self.required_for[:] + data.required_for[:]
-                case "inject":
-                    specialized["inject"] = self.inject[:] + data.inject[:]
+                case "cleanup":
+                    specialized["cleanup"] = self.cleanup[:] + data.cleanup[:]
+                case "on_fail":
+                    specialized["on_fail"] = self.on_fail[:] + data.on_fail[:]
+                case "setup":
+                    specialized["setup"] = self.setup[:] + data.setup[:]
                 case _:
                     # prefer the newest data, then the unspecialized data, then the default
                     field_data         = DootTaskSpec.__dataclass_fields__.get(field)
                     match getattr(data,field), field_data.default, field_data.default_factory:
                         case x, _MISSING_TYPE(), y if y == TomlGuard:
                             value = TomlGuard.merge(getattr(data,field), getattr(self, field), shadow=True)
                         case x, _MISSING_TYPE(), _MISSING_TYPE():
```

### Comparing `doot-0.7.0/doot/_structs/toml_loc.py` & `doot-0.7.1/doot/_structs/toml_loc.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/_structs/trace.py` & `doot-0.7.1/doot/_structs/trace.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/actions/__tests/test_base_action.py` & `doot-0.7.1/doot/actions/__tests/test_base_action.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/actions/__tests/test_control_flow.py` & `doot-0.7.1/doot/actions/__tests/test_control_flow.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/actions/__tests/test_io.py` & `doot-0.7.1/doot/actions/__tests/test_io.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/actions/__tests/test_job_actions.py` & `doot-0.7.1/doot/actions/__tests/test_job_actions.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/actions/__tests/test_job_expansion.py` & `doot-0.7.1/doot/actions/__tests/test_job_expansion.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,26 +55,25 @@
         result = obj(spec, state)
         assert(isinstance(result, dict))
         assert(isinstance(result[spec.kwargs['update_']], list))
         assert(len(result['specs']) == 3)
         for spec, expect in zip(result['specs'], args):
             assert(spec.extra.target == expect)
 
-
-    def test_action_base(self, spec, state):
-        state['base'] = "test::task"
+    def test_action_template(self, spec, state):
+        state['template'] = "test::task"
         obj = JobExpandAction()
         result = obj(spec, state)
         assert(isinstance(result, dict))
         assert(isinstance(result[spec.kwargs['update_']], list))
         assert(result['specs'][0].ctor == "test::task")
         assert(len(result['specs'][0].actions) == 0)
 
-    def test_taskname_base(self, spec, state):
-        state['base'] = [{"do":"aweg"}, {"do":"blah"}, {"do":"jioj"}]
+    def test_taskname_template(self, spec, state):
+        state['template'] = [{"do":"aweg"}, {"do":"blah"}, {"do":"jioj"}]
         obj = JobExpandAction()
         result = obj(spec, state)
         assert(isinstance(result, dict))
         assert(isinstance(result[spec.kwargs['update_']], list))
         assert(len(result['specs'][0].actions) == 3)
 
 class TestJobMatcher:
```

### Comparing `doot-0.7.0/doot/actions/__tests/test_job_injection.py` & `doot-0.7.1/doot/actions/__tests/test_job_injection.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/actions/__tests/test_job_queuing.py` & `doot-0.7.1/doot/actions/__tests/test_job_queuing.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/actions/__tests/test_postbox.py` & `doot-0.7.1/doot/actions/__tests/test_postbox.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/actions/__tests/test_shell.py` & `doot-0.7.1/doot/actions/__tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/actions/__tests/test_state.py` & `doot-0.7.1/doot/actions/__tests/test_state.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/actions/base_action.py` & `doot-0.7.1/doot/actions/base_action.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/actions/compression.py` & `doot-0.7.1/doot/actions/compression.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/actions/io.py` & `doot-0.7.1/doot/actions/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 import tomlguard as TG
 import doot
 from doot.errors import DootTaskError, DootTaskFailed
 from doot.enums import ActionResponseEnum
 from doot.mixins.path_manip import PathManip_m
 from doot.structs import DootKey
 from doot.actions.postbox import _DootPostBox
-from doot.utils.decorators import IOWriter
+from doot.utils.action_decorators import IOWriter
 
 # TODO using doot.config.settings.general.protect to disallow write/delete/backup/copy
 
 ##-- expansion keys
 TO_KEY             : Final[DootKey] = DootKey.build("to")
 FROM_KEY           : Final[DootKey] = DootKey.build("from")
 UPDATE             : Final[DootKey] = DootKey.build("update_")
@@ -78,14 +78,16 @@
                 if not arg:
                     continue
 
                 printer.info("Appending %s chars to %s", len(arg), loc)
                 f.write(sep)
                 f.write(arg)
 
+
+
 @IOWriter()
 class WriteAction(PathManip_m):
     """
       Writes data from the state to a file, accessed through the
       doot.locs object
     """
```

### Comparing `doot-0.7.0/doot/actions/job_actions.py` & `doot-0.7.1/doot/actions/job_actions.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/actions/job_expansion.py` & `doot-0.7.1/doot/actions/job_expansion.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,78 +33,80 @@
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 printer = logmod.getLogger("doot._printer")
 ##-- end logging
 
-
 import random
 from tomlguard import TomlGuard
 import doot
 import doot.errors
 from doot.structs import DootKey, DootTaskSpec, DootTaskName, DootCodeReference
 from doot.actions.base_action import DootBaseAction
 from doot.actions.job_injection import JobInjector
 
 class JobGenerate(DootBaseAction):
-    """ Run a custom function to generate task specs  """
+    """ Run a custom function to generate task specs
+      Function is in the form: fn(spec, state) -> list[DootTaskSpec]
+    """
 
     @DootKey.dec.references("fn")
     @DootKey.dec.redirects("update_")
     def __call__(self, spec, state, _fn_ref, _update):
         fn = _fn_ref.try_import()
         return { _update : list(fn(spec, state)) }
 
 class JobExpandAction(JobInjector):
     """
-      Takes a base action and builds one new subtask for each entry in a list
+      Takes a template taskname/list[actionspec] and builds one new subtask for each entry in a list
 
       'inject' provides an injection dict, with $arg$ being the entry from the source list
     """
 
-    @DootKey.dec.types("from", "inject", "base", "print_levels")
+    @DootKey.dec.types("from", "inject", "template", "print_levels")
     @DootKey.dec.expands("prefix")
     @DootKey.dec.redirects("update_")
     @DootKey.dec.taskname
-    def __call__(self, spec, state, _from, inject, base, _printL, prefix, _update, _basename):
+    def __call__(self, spec, state, _from, inject, template, _printL, prefix, _update, _basename):
         match prefix:
             case "{prefix}":
                 prefix = "{Anon}"
             case _:
                 pass
+
         result          = []
-        actions, base   = self._prep_base(base)
-        build_queue = []
+        build_queue     = []
+        base_head       = _basename.task_head()
+        actions, base   = self._prep_base(template)
         match _from:
             case int():
                 build_queue += range(_from)
             case list():
                 build_queue += _from
             case None:
                 build_queue += [1]
             case _:
                 printer.warning("Tried to expand a non-list of args")
-                return None
+                return self.ActRE.FAIL
 
         for i, arg in enumerate(build_queue):
                 injection = self.build_injection(spec, state, inject, replacement=arg)
                 new_spec  = DootTaskSpec.build(dict(name=_basename.subtask(prefix, i),
                                                     ctor=base,
                                                     actions = actions or [],
-                                                    required_for=[_basename.task_head()],
+                                                    required_for=[base_head],
                                                     extra=injection,
                                                     print_levels=_printL or {},
                                                     ))
                 result.append(new_spec)
 
-
         return { _update : result }
 
-    def _prep_base(self, base) -> tuple[list, DootTaskName|None]:
+    def _prep_base(self, base:DootTaskName|list[DootActionSpec]) -> tuple[list, DootTaskName|None]:
         """
           base can be the literal name of a task (base="group::task") to build off,
           or an indirect key to a list of actions (base_="sub_actions")
 
           This handles those possibilities and returns a list of actions and maybe a task name
 
         """
```

### Comparing `doot-0.7.0/doot/actions/job_injection.py` & `doot-0.7.1/doot/actions/job_injection.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/actions/json.py` & `doot-0.7.1/doot/actions/json.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/actions/postbox.py` & `doot-0.7.1/doot/actions/postbox.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/actions/shell.py` & `doot-0.7.1/doot/actions/shell.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/actions/speak.py` & `doot-0.7.1/doot/actions/speak.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/actions/state.py` & `doot-0.7.1/doot/actions/state.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/actions/templater.py` & `doot-0.7.1/doot/actions/templater.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/actions/util.py` & `doot-0.7.1/doot/actions/util.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/cmds/__tests/test_list_cmd.py` & `doot-0.7.1/doot/cmds/__tests/test_list_cmd.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/cmds/base_cmd.py` & `doot-0.7.1/doot/cmds/base_cmd.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/cmds/clean_cmd.py` & `doot-0.7.1/doot/cmds/clean_cmd.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/cmds/graph_cmd.py` & `doot-0.7.1/doot/cmds/graph_cmd.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/cmds/help_cmd.py` & `doot-0.7.1/doot/cmds/help_cmd.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/cmds/list_cmd.py` & `doot-0.7.1/doot/cmds/list_cmd.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/cmds/locs_cmd.py` & `doot-0.7.1/doot/cmds/locs_cmd.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/cmds/plugins_cmd.py` & `doot-0.7.1/doot/cmds/plugins_cmd.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/cmds/run_cmd.py` & `doot-0.7.1/doot/cmds/run_cmd.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/cmds/step_cmd.py` & `doot-0.7.1/doot/cmds/step_cmd.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/cmds/stub_cmd.py` & `doot-0.7.1/doot/cmds/stub_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,16 @@
 import doot.enums
 import doot.errors
 from doot.cmds.base_cmd import BaseCommand
 from doot._abstract import PluginLoader_p, Task_i
 from doot.structs import TaskStub, DootTaskName, DootCodeReference
 from doot.task.base_job import DootJob
 from doot.task.base_task import DootTask
-from doot._structs.key import KEY_ANNOTS, HELP_HINT
+from doot._structs.key import HELP_HINT
+from doot.utils.decorators import KEY_ANNOTS
 
 ##-- data
 data_path = files(doot.constants.paths.TEMPLATE_PATH).joinpath(doot.constants.paths.TOML_TEMPLATE)
 ##-- end data
 PRINT_LOCATIONS : Final[list[str]] = doot.constants.printer.PRINT_LOCATIONS
 
 class StubCmd(BaseCommand):
```

### Comparing `doot-0.7.0/doot/control/__tests/test_locations.py` & `doot-0.7.1/doot/control/__tests/test_locations.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/control/__tests/test_overlord.py` & `doot-0.7.1/doot/control/__tests/test_overlord.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/control/__tests/test_runner.py` & `doot-0.7.1/doot/control/__tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/control/__tests/test_tracker.py` & `doot-0.7.1/doot/control/__tests/test_tracker.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/control/base_runner.py` & `doot-0.7.1/doot/control/base_runner.py`

 * *Files 9% similar despite different names*

```diff
@@ -76,76 +76,90 @@
     def __enter__(self) -> Any:
         printer.info("- Validating Task Network, building remaining abstract tasks: %s", self.tracker.late_count)
         self.tracker.validate()
         printer.info(self._enter_msg, extra={"colour" : "green"})
         return
 
     def __exit__(self, exc_type, exc_value, exc_traceback) -> bool:
+        # TODO handle exc_types?
         printer.setLevel("INFO")
         printer.info("")
         printer.info(self._exit_msg, extra={"colour":"green"})
         self._finish()
         return
 
     def _finish(self):
-        """finish running tasks, summarizing results
+        """finish running tasks, summarizing results using the reporter
           separate from __exit__ to allow it to be overridden
         """
         logging.info("Task Running Completed")
         if self.step >= max_steps:
             printer.info("Runner Hit the Step Limit: %s", max_steps)
 
         printer.info("Final Summary: ")
         printer.info(str(self.reporter), extra={"colour":"magenta"})
         match self._signal_failure:
             case None:
                 return
             case doot.errors.DootError():
                 raise self._signal_failure
 
-    def _handle_task_success(self, task):
+    def _handle_task_success(self, task:None|Task_i|DootTaskArtifact):
+        """ The basic success handler. just informs the tracker of the success """
         if task:
             self.tracker.update_state(task, self.tracker.state_e.SUCCESS)
         return task
 
     def _handle_failure(self, task:None|Task_i, failure:Error) -> None:
+        """ The basic failure handler.
+          Triggers a breakpoint on DootTaskInterrupt,
+          otherwise informs the tracker of the failure.
+
+          Halts any failed or errored tasks, which propagates to any successors
+          Fails any DootErrors, TrackingErrors, and non-doot errors
+
+          the tracker handle's clearing itself and shutting down
+        """
         match failure:
             case doot.errors.DootTaskInterrupt():
                 breakpoint()
                 pass
             case doot.errors.DootTaskFailed() as err:
                 self._signal_failure = err
                 printer.warning("%s %s", fail_prefix, err)
-                self.tracker.update_state(err.task.name, self.tracker.state_e.FAILED)
+                self.tracker.update_state(err.task.name, self.tracker.state_e.HALTED)
             case doot.errors.DootTaskError() as err:
                 self._signal_failure = err
                 printer.warning("%s %s", fail_prefix, err)
-                self.tracker.update_state(err.task.name, self.tracker.state_e.FAILED)
+                self.tracker.update_state(err.task.name, self.tracker.state_e.HALTED)
             case doot.errors.DootError() as err:
                 self._signal_failure = err
                 printer.warning("%s %s", fail_prefix, err)
                 self.tracker.update_state(task, self.tracker.state_e.FAILED)
             case doot.errors.DootTaskTrackingError() as err:
                 self._signal_failure = err
                 printer.warning("%s %s", fail_prefix, err)
-                self.tracker.clear_queue()
+                self.tracker.update_state(task, self.tracker.state_e.FAILED)
             case _:
                 self._signal_failure = doot.errors.DootError("Unknown Failure")
                 printer.exception("%s Unknown failure occurred: %s", fail_prefix, failure)
-                self.tracker.clear_queue()
+                self.tracker.update_state(task, self.tracker.state_e.FAILED)
 
     def _sleep(self, task):
+        """
+          The runner's sleep method, which spaces out tasks
+        """
         match task:
             case None:
                 return
             case DootTaskArtifact():
                 return
 
         with logctx(task.spec.print_levels.on_fail(sleep_level).sleep()) as p:
             sleep_len = task.spec.extra.on_fail(default_SLEEP_LENGTH, int|float).sleep()
             p.info("[Sleeping (%s)...]", sleep_len, extra={"colour":"white"})
             time.sleep(sleep_len)
-            self.step += 1
 
     def _notify_artifact(self, art:DootTaskArtifact) -> None:
+        """ A No-op for when the tracker gives an artifact """
         printer.info("---- Artifact: %s", art)
-        self.reporter.trace(art, flags=ReportEnum.ARTIFACT)
+        self.reporter.add_trace(art, flags=ReportEnum.ARTIFACT)
```

### Comparing `doot-0.7.0/doot/control/base_tracker.py` & `doot-0.7.1/doot/control/base_tracker.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,28 +45,30 @@
 import doot.errors
 from doot.enums import TaskStateEnum, TaskQueueMeta
 from doot._abstract import Job_i, Task_i, FailPolicy_p
 from doot.structs import DootTaskArtifact, DootTaskSpec, DootTaskName, DootCodeReference, DootActionSpec
 from doot._abstract import TaskTracker_i, TaskRunner_i, Task_i
 from doot.task.base_task import DootTask
 
-ROOT             : Final[str]                  = "__root" # Root node of dependency graph
-STATE            : Final[str]                  = "state"  # Node attribute name
-PRIORITY         : Final[str]                  = "priority"
-COMPLETE_STATES  : Final[set[TaskStateEnum]]   = {TaskStateEnum.SUCCESS, TaskStateEnum.EXISTS}
-DECLARE_PRIORITY : Final[int]                  = 10
-MIN_PRIORITY     : Final[int]                  = -10
-
 class EDGE_E(enum.Enum):
     """ Enum describing the possible edges of the task tracker's task network """
     TASK               = enum.auto()
     ARTIFACT           = enum.auto()
     TASK_CROSS         = enum.auto() # Task to artifact
     ARTIFACT_CROSS     = enum.auto() # artifact to task
 
+ROOT             : Final[str]                  = "__root" # Root node of dependency graph
+STATE            : Final[str]                  = "state"  # Node attribute name
+PRIORITY         : Final[str]                  = "priority"
+REACTIVE_ADD     : Final[str]                  = "reactive-add"
+COMPLETE_STATES  : Final[set[TaskStateEnum]]   = {TaskStateEnum.SUCCESS, TaskStateEnum.EXISTS}
+ARTIFACT_EDGES   : Final[set[EDGE_E]]          = [EDGE_E.ARTIFACT, EDGE_E.TASK_CROSS]
+DECLARE_PRIORITY : Final[int]                  = 10
+MIN_PRIORITY     : Final[int]                  = -10
+
 class _InternalTrackerBase(TaskTracker_i):
     """ Standard implementation of private tracker methods and plumbing """
 
     state_e            = TaskStateEnum
     INITIAL_TASK_STATE = TaskStateEnum.DEFINED
 
     def __init__(self, shadowing:bool=False, *, policy=None):
@@ -154,14 +156,32 @@
                 self.task_graph.add_node(str(artifact), state=self.state_e.ARTIFACT, priority=self._declare_priority)
                 # connect to definites
                 for x in filter(lambda x: x in artifact, self.artifacts.values()):
                     self.task_graph.add_edge(str(x), str(artifact), type=EDGE_E.ARTIFACT)
 
         return str(artifact)
 
+    def _build_head(self, spec:DootTaskSpec) -> None|TaskSpec:
+        """
+          Build a head task for a job, taking the jobs cleanup actions
+          and using them as the head's main action.
+          Depends on the job, and its reactively queued.
+        """
+        # build $head$
+        head : DootTaskSpec = DootTaskSpec.build({
+            "name"            : spec.name.task_head(),
+            "source"          : spec.name,
+            "actions"         : spec.cleanup,
+            "print_levels"    : spec.print_levels,
+            "extra"           : spec.extra,
+            "queue_behaviour" : TaskQueueMeta.reactive,
+            "depends_on"      : [spec.name],
+            })
+        return head
+
     def _insert_cli_args_into_spec(self, spec:DootTaskSpec) -> DootTaskSpec:
         """ Takes a task spec, and inserts matching cli args into it if necessary """
         spec_extra : dict = dict(spec.extra.items() or [])
 
         for cli in spec.extra.on_fail([]).cli():
             if cli.name not in spec_extra:
                 spec_extra[cli.name] = cli.default
@@ -180,14 +200,15 @@
     def _insert_dependencies(self, task):
         """ insert a task's dependencies into the network, connecting them to the task """
         for pre in task.depends_on:
             logging.debug("Connecting Dependency: %s -> %s", pre, task.readable_name)
             match pre:
                 case DootActionSpec():
                     # Action spec dependencies are tested when running, not as part of the DAG
+                    # TODO use decorations to know about implicit depencies, eg: artifacts
                     pass
                 case DootTaskArtifact():
                     pre = self._add_artifact(pre)
                     self.task_graph.add_edge(pre, task.name, type=EDGE_E.ARTIFACT_CROSS)
                 case DootTaskName() if all([(in_graph:=str(pre) in self.task_graph),(has_args:=bool(pre.args))]):
                     base_spec                 = self.tasks[str(pre)].spec
                     name_spec                 = DootTaskSpec.build(pre)
@@ -257,31 +278,44 @@
             case TaskQueueMeta.default:
                 # Waits for explicit queue
                 pass
             case _:
                 raise doot.errors.DootTaskTrackingError("Unknown queue behaviour specified: %s", task.spec.queue_behaviour)
 
     def _task_dependencies(self, task) -> tuple[list[str], list[str]]:
-        # TODO detect 'read' actions as implicit dependencies
+        """ get predecessors of the task,
+          return [list[incomplete], list[all]]
+        """
         dependencies = list(self.task_graph.pred[task].keys())
         incomplete   = list(filter(lambda x: self.task_state(x) not in COMPLETE_STATES, dependencies))
         return incomplete, dependencies
 
     def _task_products(self, task) -> tuple[list[str], list[str]]:
         """
-          Get task 'required-for' files: [not-existing, total]
+          Get task 'required-for' files: [list[not-existing], list[total]]
         """
         # TODO detect 'write!' actions as implicit products
-        looking_for  = [EDGE_E.ARTIFACT, EDGE_E.TASK_CROSS]
-        artifacts    = list(map(lambda x: x[0], filter(lambda x: x[1].get('type', None) in looking_for, self.task_graph.succ[str(task)].items())))
+        artifacts    = list(map(lambda x: x[0], filter(lambda x: x[1].get('type', None) in ARTIFACT_EDGES, self.task_graph.succ[str(task)].items())))
         incomplete   = list(filter(lambda x: not bool(self.artifacts[x]), artifacts))
-
         return incomplete, artifacts
 
     def _task_dependents(self, task) -> tuple[list[str], list[str]]:
+        """ TODO get [list[incomplete], list[total]] successors for a task """
+        raise NotImplementedError()
+
+    def _reactive_queue(self, focus:str):
+        """ Queue any known task in the network that auto-reacts to a focus """
+        for adj in self.task_graph.adj[focus]:
+            if self.task_graph.nodes[adj].get(REACTIVE_ADD, False):
+                self.queue_task(adj, silent=True)
+
+    def _reactive_fail_queue(self, focus:str):
+        """ TODO: make reactive failure tasks that can be triggered from
+          a tasks 'on_fail' collection
+          """
         raise NotImplementedError()
 
 class BaseTracker(_InternalTrackerBase):
     """ The public part of the standard tracker implementation """
 
     @property
     def late_count(self):
```

### Comparing `doot-0.7.0/doot/control/locations.py` & `doot-0.7.1/doot/control/locations.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/control/overlord.py` & `doot-0.7.1/doot/control/overlord.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/control/runner.py` & `doot-0.7.1/doot/control/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,26 +97,27 @@
                         self._notify_artifact(task)
                     case Job_i() if self._test_conditions(task):
                         self._expand_job(task)
                     case Task_i() if self._test_conditions(task):
                         self._execute_task(task)
                     case Task_i():
                         # test_conditions failed, so skip
-                        printer.info("Skipping Task: %s", task.spec.name)
+                        printer.info("----| Task %s: %s Skipped.", self.step, task.spec.name)
                     case _:
                         pass
             except doot.errors.DootError as err:
                 self._handle_failure(task, err)
             except Exception as err:
                 printer.exception("Unknown, non-Doot failure occurred: %s", err)
                 self.tracker.clear_queue()
                 raise err
             else:
                 self._handle_task_success(task)
                 self._sleep(task)
+                self.step += 1
 
     def _expand_job(self, job:Job_i) -> None:
         """ turn a job into all of its tasks, including teardowns """
         build_log_level  = job.spec.print_levels.on_fail(build_level).build()
         head_log_level   = job.spec.print_levels.on_fail(head_level).head()
 
         try:
@@ -124,99 +125,108 @@
             with logctx(head_log_level) as p:     # Announce entry
                 p.info("---> Job %s: %s", self.step, job.name, extra={"colour":"magenta"})
                 # TODO queue $head$
 
             self.reporter.add_trace(job.spec, flags=ReportEnum.JOB | ReportEnum.INIT)
 
             with logctx(build_log_level) as p: # Run the actions
-                self._execute_action_group(job.spec.setup, job)
-                self._execute_action_group(job.spec.actions, job, allow_queue=True)
+                self._execute_action_group(job.spec.setup, job, group="setup")
+                self._execute_action_group(job.spec.actions, job, allow_queue=True, group="actions")
 
         except doot.errors.DootError as err:
-            self._execute_action_group(task.spec.on_fail, task)
+            self._execute_action_group(job.spec.on_fail, job, group="on_fail")
             raise err
         finally:
-            self._execute_action_group(job.spec.cleanup, job)
+            # cleanup actions are *not* run here, as they've been added to the auto-gen $head$ and queued
             job.state.clear()
 
             with logctx(head_log_level)  as p: # Announce Exit
                 self.reporter.add_trace(job.spec, flags=ReportEnum.JOB | ReportEnum.SUCCEED)
                 p.info("---< Job %s: %s", self.step, job.name, extra={"colour":"magenta"})
 
     def _execute_task(self, task:Task_i) -> None:
         """ execute a single task's actions """
         build_log_level  = task.spec.print_levels.on_fail(build_level).build()
         head_log_level   = task.spec.print_levels.on_fail(head_level).head()
 
         try:
             with logctx(head_log_level) as p: # Announce entry
                 p.info("----> Task %s :  %s", self.step, task.spec.name.readable, extra={"colour":"magenta"})
-                # TODO queue $head$
 
             self.reporter.add_trace(task.spec, flags=ReportEnum.TASK | ReportEnum.INIT)
 
             with logctx(build_log_level) as p: # Build then run actions
-                self._execute_action_group(task.spec.setup, task)
-                self._execute_action_group(task.spec.actions, task)
+                self._execute_action_group(task.spec.setup, task, group="setup")
+                self._execute_action_group(task.spec.actions, task, group="action")
                 self.reporter.add_trace(task.spec, flags=ReportEnum.TASK | ReportEnum.SUCCEED)
         except doot.errors.DootError as err:
-            self._execute_action_group(task.spec.on_fail, task)
+            self._execute_action_group(task.spec.on_fail, task, group="on_fail")
             raise err
         finally:
-            self._execute_action_group(task.spec.cleanup, task)
+            # Cleanup Actions *are* run here, because tasks don't have subtasks they setup for
+            self._execute_action_group(task.spec.cleanup, task, group="cleanup")
             task.state.clear()
 
             with logctx(head_log_level)  as p: # Cleanup and exit
                 p.debug("----< Task: %s", task.name, extra={"colour":"cyan"})
 
-    def _execute_action_group(self, actions:list, task:Task_i, allow_queue=False) -> tuple[int, ActRE]:
+    def _execute_action_group(self, actions:list, task:Task_i, allow_queue=False, group=None) -> tuple[int, ActRE]:
         """ Execute a group of actions, possibly queue any task specs they produced,
         and return a count of the actions run + the result
         """
-        group_result    = ActRE.SUCCESS
-        to_queue        = []
-        executed        = 0
+        logging.debug("Running Action Group %s (%s) for : %s", group, len(actions), task.spec.name)
+        group_result     = ActRE.SUCCESS
+        to_queue         = []
+        executed_count   = 0
 
         for action in actions:
             result = None
             match action:
                 case DootActionSpec():
-                    result = self._execute_action(executed, action, task)
+                    result = self._execute_action(executed_count, action, task)
                 case DootTaskArtifact():
                     pass
                 case DootTaskName():
                     pass
                 case _:
                     self.reporter.add_trace(task.spec, flags=ReportEnum.FAIL | ReportEnum.TASK)
                     raise doot.errors.DootTaskError("Task %s Failed: Produced a bad action: %s", task.name, action, task=task.spec)
 
             match result:
                 case None:
                     continue
                 case list():
                     to_queue += result
                 case ActRE.SKIP:
-                    p.warning("------ Remaining Task Actions skipped by Action Instruction")
+                    printer.warning("------ Remaining Task Actions skipped by Action Result")
                     group_result = ActRE.SKIP
                     break
 
-            executed += 1
+            executed_count += 1
 
         else: # runs only if no 'break'
-            if not allow_queue:
-                    return executed, group_result
-
-            for spec in to_queue:
-                self.tracker.add_task(spec, no_root_connection=True)
+            match to_queue:
+                case []:
+                    pass
+                case [*xs] if not allow_queue:
+                    printer.warning("---- !!!! Tried to Queue additional tasks from a bad action group: %s", task)
+                    group_result = ActRE.FAIL
+                case [*xs]:
+                    for spec in xs:
+                        self.tracker.add_task(spec, no_root_connection=True)
+                    printer.info("Queued %s Subtasks for %s", len(xs), task.spec.name)
 
-        return executed, group_result
+        return executed_count, group_result
 
     def _execute_action(self, count, action, task) -> ActRE|list:
         """ Run the given action of a specific task.
 
+          returns either a list of specs to (potentially) queue,
+          or an ActRE describing the action result.
+
         """
         result                     = None
         action_log_level           = task.spec.print_levels.on_fail(action_level).action()
         execute_log_level          = task.spec.print_levels.on_fail(execute_level).execute()
         task.state['_action_step'] = count
         self.reporter.add_trace(action, flags=ReportEnum.ACTION | ReportEnum.INIT)
         logmod.debug("-----> Action Execution: %s for %s", action, task.name)
@@ -255,13 +265,13 @@
         with logctx(action_log_level) as p: # Prep the action
             p.debug("-----< Action Execution Complete: %s for %s", action, task.name)
 
         self.reporter.add_trace(action, flags=ReportEnum.ACTION | ReportEnum.SUCCEED)
         return result
 
     def _test_conditions(self, task:Task_i) -> bool:
-        """ run action specs that test if the task can be started """
-        match self._execute_action_group(task.spec.depends_on, task):
-            case _, ActRE.SKIP:
+        """ run a task's depends_on group, coercing to a bool """
+        match self._execute_action_group(task.spec.depends_on, task, group="depends_on"):
+            case _, ActRE.SKIP | ActRE.FAIL:
                 return False
             case _, _:
                 return True
```

### Comparing `doot-0.7.0/doot/control/step_runner.py` & `doot-0.7.1/doot/control/step_runner.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/control/tracker.py` & `doot-0.7.1/doot/control/tracker.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 from doot.enums import TaskStateEnum
 from doot._abstract import Job_i, Task_i, FailPolicy_p
 from doot.structs import DootTaskArtifact, DootTaskSpec, DootTaskName, DootCodeReference
 from doot._abstract import TaskTracker_i, TaskRunner_i, Task_i
 from doot.task.base_task import DootTask
 from doot.control.base_tracker import BaseTracker, ROOT, STATE, PRIORITY, EDGE_E, MIN_PRIORITY
 
-REACTIVE_ADD     : Final[str]                  = "reactive-add"
 
 @doot.check_protocol
 class DootTracker(BaseTracker, TaskTracker_i):
     """
     track dependencies in a networkx digraph,
     predecessors of a node are its dependencies.
       ie: SubDependency -> Dependency -> Task -> ROOT
@@ -53,15 +52,15 @@
 
     the `task_graph` stores nodes as full names of tasks
     """
     state_e            = TaskStateEnum
     INITIAL_TASK_STATE = TaskStateEnum.DEFINED
 
     def __init__(self, shadowing:bool=False, *, policy=None):
-        super().__init__(shadowing=shadowing, policy=policy) # self.tasks
+        super().__init__(shadowing=shadowing, policy=policy) # -> self.tasks
 
     def add_task(self, task:DootTaskSpec|Task_i, *, no_root_connection=False) -> None:
         """ add a task description into the tracker, but don't queue it
         connecting it with its dependencies and tasks that depend on it
         """
         task : Task_i = self._prep_task(task)
         assert(isinstance(task, Task_i))
@@ -76,14 +75,23 @@
         if not no_root_connection and task.name:
             self.task_graph.add_edge(task.name, ROOT)
 
         self._insert_dependencies(task)
         self._insert_dependents(task)
         self._maybe_implicit_queue(task)
 
+        # To Stop heads having heads
+        if task.spec.name == task.spec.name.task_head():
+            return
+        if not isinstance(task, Job_i):
+            return
+
+        head_spec = self._build_head(task.spec)
+        self.add_task(head_spec, no_root_connection=True)
+
     def update_state(self, task:str|Task_i|DootTaskArtifact, state:self.state_e):
         """ update the state of a task in the dependency graph """
         logging.debug("Updating State: %s -> %s", task, state)
         match task, state:
             case str(), self.state_e() if task in self.task_graph:
                 self.task_graph.nodes[task][STATE] = state
             case DootTaskName(), self.state_e() if task in self.task_graph:
@@ -108,50 +116,53 @@
             if focus in self.task_graph and self.task_graph.nodes[focus][PRIORITY] < self._min_priority:
                 logging.warning("Task halted due to reaching minimum priority while tracking: %s", focus)
                 self.update_state(focus, self.state_e.HALTED)
 
             match self.task_state(focus):
                 case self.state_e.SUCCESS:
                     self.deque_task()
-                    # Queue any task that auto-reacts to this task
-                    for adj in self.task_graph.adj[focus]:
-                        if self.task_graph.nodes[adj].get(REACTIVE_ADD, False):
-                            self.queue_task(adj)
-                case self.state_e.EXISTS: # remove task on completion
+                    self._reactive_queue(focus)
+                case self.state_e.EXISTS: # remove artifact if exists
                     for pred in self.task_graph.pred[focus].keys():
                         logging.debug("Propagating Artifact existence to disable: %s", pred)
                         self.update_state(pred, self.state_e.SUCCESS)
                     self.deque_task()
                     return self.artifacts[focus]
                 case self.state_e.HALTED:  # remove and propagate halted status
                     # anything that depends on a halted task in turn gets halted
                     halting = list(self.task_graph.succ[focus].keys())
                     printer.warning("Propagating Halt from: %s to: %s", focus, halting)
                     for pred in halting:
                         self.update_state(pred, self.state_e.HALTED)
                     # And remove the halted task from the active_set
                     self.deque_task()
                 case self.state_e.FAILED:  # stop when a task fails, and clear any queued tasks
+                    # TODO
                     self.clear_queue()
                     return None
+                case self.state_e.RUNNING:
+                    raise doot.errors.DootTaskTrackingError("running state shouldn't be possible")
                 case self.state_e.READY if focus in self.execution_path: # error on running the same task twice
                     raise doot.errors.DootTaskTrackingError("Task Attempted to run twice: %s", focus)
                 case self.state_e.READY:   # return the task if its ready
                     self.execution_path.append(focus)
+                    # TODO check this, it might not affect the priority queue
+                    self.task_graph.nodes[focus][PRIORITY] -= 1
                     return self.tasks.get(focus, None)
                 case self.state_e.ARTIFACT if bool(self.artifacts[focus]): # if an artifact exists, mark it so and remove it
                     logging.info("Artifact Exists: %s", focus)
                     self.update_state(focus, self.state_e.EXISTS)
                 case self.state_e.ARTIFACT: # Add dependencies of an artifact to the stack
                     incomplete, all_deps = self._task_dependencies(focus)
                     if bool(incomplete):
                         logging.info("Artifact Blocking Check: %s", focus)
                         self.deque_task()
                         self.queue_task(focus, *incomplete, silent=True)
                     elif bool(all_deps):
+                        # Only unblock if something produces thsi artifact
                         logging.debug("Artifact Unblocked: %s", focus)
                         self.update_state(focus, self.state_e.EXISTS)
                     else:
                         self.deque_task()
                         self.queue_task(focus)
 
                 case self.state_e.WAIT | self.state_e.DEFINED: # Add dependencies of a task to the stack
```

### Comparing `doot-0.7.0/doot/enums.py` & `doot-0.7.1/doot/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     HALTED          = enum.auto()
     WAIT            = enum.auto()
     READY           = enum.auto()
     RUNNING         = enum.auto()
     EXISTS          = enum.auto()
     INIT            = enum.auto()
 
+    SKIPPED         = enum.auto()
     DEFINED         = enum.auto()
     DECLARED        = enum.auto()
     ARTIFACT        = enum.auto()
 
 class TaskFlags(FlagsBuilder_m, enum.Flag):
     """
       Flags describing properties of a task,
@@ -103,27 +104,31 @@
     yes     = enum.auto()
     noBut   = enum.auto()
     no      = enum.auto()
 
 class LocationMeta(FlagsBuilder_m, enum.Flag):
     """ Available metadata attachable to a location """
 
-    default      = enum.auto()
-    file         = enum.auto()
+    location     = enum.auto()
+    artifact     = enum.auto()
     protected    = enum.auto()
     indefinite   = enum.auto()
     cleanable    = enum.auto()
     normOnLoad   = enum.auto()
 
+    file         = artifact
+    default      = location
+
 class TaskQueueMeta(EnumBuilder_m, enum.Enum):
     """ available ways a task can be activated for running
       onRegister/auto     : activates automatically when added to the task network
       reactive            : activates if an adjacent node completes
 
       default             : activates only if uses queues the task, or its a dependency
 
     """
 
-    default    = enum.auto()
-    onRegister = enum.auto()
-    reactive   = enum.auto()
-    auto       = onRegister
+    default      = enum.auto()
+    onRegister   = enum.auto()
+    reactive     = enum.auto()
+    reactiveFail = enum.auto()
+    auto         = onRegister
```

### Comparing `doot-0.7.0/doot/errors.py` & `doot-0.7.1/doot/errors.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/loaders/__tests/test_cmd_loader.py` & `doot-0.7.1/doot/loaders/__tests/test_cmd_loader.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/loaders/__tests/test_plugin_loader.py` & `doot-0.7.1/doot/loaders/__tests/test_plugin_loader.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/loaders/__tests/test_task_loader.py` & `doot-0.7.1/doot/loaders/__tests/test_task_loader.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/loaders/cmd_loader.py` & `doot-0.7.1/doot/loaders/cmd_loader.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/loaders/plugin_loader.py` & `doot-0.7.1/doot/loaders/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/loaders/task_loader.py` & `doot-0.7.1/doot/loaders/task_loader.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/mixins/enums.py` & `doot-0.7.1/doot/mixins/enums.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/mixins/fail_handler.py` & `doot-0.7.1/doot/mixins/fail_handler.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/mixins/human_numbers.py` & `doot-0.7.1/doot/mixins/human_numbers.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/mixins/importer.py` & `doot-0.7.1/doot/mixins/importer.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/mixins/param_spec.py` & `doot-0.7.1/doot/mixins/param_spec.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/mixins/path_manip.py` & `doot-0.7.1/doot/mixins/path_manip.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/mixins/zipper.py` & `doot-0.7.1/doot/mixins/zipper.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/parsers/__tests/test_flexible.py` & `doot-0.7.1/doot/parsers/__tests/test_flexible.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/parsers/flexible.py` & `doot-0.7.1/doot/parsers/flexible.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/reporters/__tests/test_stack_manager.py` & `doot-0.7.1/doot/reporters/__tests/test_stack_manager.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/reporters/__tests/test_summary_manager.py` & `doot-0.7.1/doot/reporters/__tests/test_summary_manager.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/reporters/basic_reporters.py` & `doot-0.7.1/doot/reporters/basic_reporters.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/reporters/stack_manager.py` & `doot-0.7.1/doot/reporters/stack_manager.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/reporters/summary_manager.py` & `doot-0.7.1/doot/reporters/summary_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,17 +47,17 @@
     """
 
     def __init__(self, reporters:list=None):
         super().__init__(reporters)
 
     def __str__(self):
         result = {
-            "tasks"     : {"success": 0, "fail": 0, "total": 0},
+            "tasks"     : {"success": 0, "fail": 0, "skip": 0, "total": 0},
+            "jobs"      : {"success": 0, "fail": 0, "skip": 0, "total": 0},
             "actions"   : {"success": 0, "fail": 0, "total": 0},
-            "jobs"      : {"success": 0, "fail": 0, "total": 0},
             "artifacts" : 0
             }
 
         for trace in self._full_trace:
             if ReportEnum.ARTIFACT in trace.flags:
                 result['artifacts'] += 1
                 continue
@@ -72,23 +72,25 @@
             elif ReportEnum.TASK in trace.flags:
                 category = "tasks"
 
             if ReportEnum.FAIL in trace.flags:
                 ended = "fail"
             elif ReportEnum.SUCCEED in trace.flags:
                 ended = "success"
+            elif ReportEnum.SKIP in trace.flags:
+                ended = "skip"
 
             if category is None or ended is None:
                 continue
 
             result[category][ended] += 1
             result[category]["total"] += 1
 
         output = [
             "    - Totals : Jobs: {}, Tasks: {}, Actions: {}".format(result['jobs']['total'], result['tasks']['total'], result['actions']['total']),
-            "    - Success/Failures:",
-            "    -- Jobs      : {}/{}".format(result['jobs']['success'],result['jobs']['fail']),
-            "    -- Tasks     : {}/{}".format(result['tasks']['success'], result['tasks']['fail']),
+            "    - Success/Failures/Skips:",
+            "    -- Jobs      : {}/{}/{}".format(result['jobs']['success'],result['jobs']['fail'], result['jobs']['skip']),
+            "    -- Tasks     : {}/{}/{}".format(result['tasks']['success'], result['tasks']['fail'], result['tasks']['skip']),
             "    -- Actions   : {}/{}".format(result['actions']['success'], result['actions']['fail']),
             "    -- Artifacts : {}".format(result['artifacts']),
         ]
         return "\n".join(output)
```

### Comparing `doot-0.7.0/doot/structs.py` & `doot-0.7.1/doot/structs.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/task/__tests/test_base_job.py` & `doot-0.7.1/doot/task/__tests/test_base_job.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/task/__tests/test_base_task.py` & `doot-0.7.1/doot/task/__tests/test_base_task.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/task/__tests/test_check_locs.py` & `doot-0.7.1/doot/task/__tests/test_check_locs.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/task/base_job.py` & `doot-0.7.1/doot/task/base_job.py`

 * *Files 14% similar despite different names*

```diff
@@ -108,24 +108,7 @@
 
         params = cls.param_specs
         if bool([x for x in params if not x.invisible]):
             help_lines += ["", "Params:"]
             help_lines += [str(x) for x in cls.param_specs if not x.invisible]
 
         return "\n".join(help_lines)
-
-    def _build_head(self, **kwargs) -> None|DootTaskSpec:
-        logging.debug("Building Head Task for: %s", self.name)
-        inject_keys = set(self.spec.inject)
-        inject_dict = {k: self.spec.extra[k] for k in inject_keys if k in self.spec.extra}
-        extra       = {}
-        extra.update(kwargs)
-        extra.update(inject_dict)
-        task_spec                 = self.default_task(None, TomlGuard(extra))
-        task_spec.queue_behaviour = "auto"
-        task_spec.print_levels    = self.spec.print_levels
-
-        task_ref                  = self.spec.extra.on_fail((None,), None|str).head_task()
-        if task_ref is not None:
-            task_spec.ctor = DootStructuredName.build(task_ref)
-
-        return task_spec
```

### Comparing `doot-0.7.0/doot/task/base_task.py` & `doot-0.7.1/doot/task/base_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 printer = logmod.getLogger("doot._printer")
 
 import doot
 import doot.errors
 import tomlguard
 from doot._abstract import Task_i, Job_i, Action_p, PluginLoader_p
 from doot.enums import TaskFlags, TaskStateEnum
-from doot.structs import TaskStub, TaskStubPart, DootActionSpec, DootCodeReference, DootTaskName
+from doot.structs import TaskStub, TaskStubPart, DootActionSpec, DootCodeReference, DootTaskName, DootTaskArtifact
 from doot.actions.base_action import DootBaseAction
 from doot.errors import DootTaskLoadError, DootTaskError
 
 from doot.mixins.param_spec import ParamSpecMaker_m
 from doot.mixins.importer import Importer_m
 
 TASK_ALISES     = doot.aliases.task
@@ -216,18 +216,18 @@
         """ if the task/action spec requires particular action ctors, load them.
           if the action spec doesn't have a ctor, use the task's action_ctor
         """
         logging.info("Preparing Actions: %s", self.name)
         for group in self.spec.action_groups:
             for action_spec in group:
                 match action_spec:
-                    case DootTaskName():
+                    case DootTaskName() | DootTaskArtifact():
                         pass
                     case DootActionSpec() if action_spec.fun is not None:
                         pass
                     case DootActionSpec() if action_spec.do is not None:
                         action_ref = self.import_callable(action_spec.do)
                         action_spec.set_function(action_ref)
                     case DootActionSpec():
                         action_spec.set_function(self.action_ctor)
                     case _:
-                        raise doot.errors.DootTaskError("Unknown element in action group: ", action_spec)
+                        raise doot.errors.DootTaskError("Unknown element in action group: ", action_spec, self.spec.name)
```

### Comparing `doot-0.7.0/doot/task/check_locs.py` & `doot-0.7.1/doot/task/check_locs.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 ##-- end std imports
 
 from tomlguard import TomlGuard
 import doot
 import doot.errors
 from doot.structs import DootTaskSpec
 from doot._abstract import Job_i
-from doot.task.base_job import DootJob
 from doot.task.base_task import DootTask
 from doot.enums import LocationMeta
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 printer = logmod.getLogger("doot._printer")
 ##-- end logging
@@ -43,15 +42,15 @@
             "name"         : CheckLocsTask.task_name,
             "actions"      : locations,
             "print_levels" : print_levels,
             "priority"     : 100,
                                            })
         super().__init__(spec, action_ctor=self.checklocs)
 
-    def checklocs(self, spec, task_state_copy):
+    def checklocs(self, spec, state):
         exists_p = spec.args[0].exists()
         if exists_p:
             printer.info("Base Location Exists : %s", spec.args[0])
         else:
             printer.warning("Base Location Missing: %s", spec.args[0])
             if make_missing:
                 printer.info("Making Directory: %s", spec.args[0])
```

### Comparing `doot-0.7.0/doot/task/specialised_jobs.py` & `doot-0.7.1/doot/task/specialised_jobs.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/utils/__tests/test_decorators.py` & `doot-0.7.1/doot/utils/__tests/test_action_decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 import warnings
 
 import pytest
 import doot
 doot._test_setup()
 from doot.structs import DootKey
 from doot.utils.testing_fixtures import wrap_locs
-from doot.utils import decorators as decs
+from doot.utils import action_decorators as decs
+from doot.utils.decorators import DecorationUtils as DU
 
 logging = logmod.root
 
 DD = decs.DootDecorator
 
 class TestDecorators:
 
@@ -35,137 +36,137 @@
     def test_initial(self):
         """ check a simple annotation and wrap """
 
         @decs.DryRunSwitch()
         def simple(spec:dict, state:dict) -> str:
             return "blah"
 
-        assert(DD.has_annotations(simple, doot.constants.decorations.RUN_DRY_SWITCH))
+        assert(DU.has_annotations(simple, doot.constants.decorations.RUN_DRY_SWITCH))
         assert(simple({}, {}) == "blah")
 
     def test_override_dry_run(self):
         """ check the wrapper works """
 
         @decs.DryRunSwitch(override=True)
         def simple(spec:dict, state:dict) -> str:
             return "blah"
 
-        assert(DD.has_annotations(simple, doot.constants.decorations.RUN_DRY_SWITCH))
+        assert(DU.has_annotations(simple, doot.constants.decorations.RUN_DRY_SWITCH))
         assert(simple({}, {}) is None)
 
     def test_wrap_method(self):
 
         @decs.DryRunSwitch()
         class SimpleClass:
 
             def __call__(self, spec, state):
                 return "blah"
 
         # class is annotated
-        assert(DD.has_annotations(SimpleClass, doot.constants.decorations.RUN_DRY_SWITCH))
+        assert(DU.has_annotations(SimpleClass, doot.constants.decorations.RUN_DRY_SWITCH))
         # Instance is annotated
-        assert(DD.has_annotations(SimpleClass(), doot.constants.decorations.RUN_DRY_SWITCH))
+        assert(DU.has_annotations(SimpleClass(), doot.constants.decorations.RUN_DRY_SWITCH))
         assert(SimpleClass()({}, {}) == "blah")
 
     def test_wrap_method_override_dry(self):
 
         @decs.DryRunSwitch(override=True)
         class SimpleClass:
 
             def __call__(self, spec, state):
                 return "blah"
 
         # class is annotated
-        assert(DD.has_annotations(SimpleClass, doot.constants.decorations.RUN_DRY_SWITCH))
+        assert(DU.has_annotations(SimpleClass, doot.constants.decorations.RUN_DRY_SWITCH))
         # Instance is annotated
-        assert(DD.has_annotations(SimpleClass(), doot.constants.decorations.RUN_DRY_SWITCH))
+        assert(DU.has_annotations(SimpleClass(), doot.constants.decorations.RUN_DRY_SWITCH))
         assert(SimpleClass()({}, {}) is None)
 
     def test_annotate_fn(self):
 
         @decs.RunsDry()
         def simple(spec:dict, state:dict) -> str:
             return "blah"
 
-        assert(DD.has_annotations(simple, doot.constants.decorations.RUN_DRY))
+        assert(DU.has_annotations(simple, doot.constants.decorations.RUN_DRY))
 
     def test_annotate_method(self):
 
         @decs.RunsDry()
         class SimpleClass:
 
             def __call__(self, spec:dict, state:dict) -> str:
                 return "blah"
 
-        assert(DD.has_annotations(SimpleClass, doot.constants.decorations.RUN_DRY))
-        assert(DD.has_annotations(SimpleClass(), doot.constants.decorations.RUN_DRY))
+        assert(DU.has_annotations(SimpleClass, doot.constants.decorations.RUN_DRY))
+        assert(DU.has_annotations(SimpleClass(), doot.constants.decorations.RUN_DRY))
 
     def test_annotation_survives_subclassing(self):
 
         @decs.RunsDry()
         class SimpleSuper:
             pass
 
         class SimpleChild(SimpleSuper):
             pass
 
-        assert(DD.has_annotations(SimpleSuper,   decs.RUN_DRY))
-        assert(DD.has_annotations(SimpleSuper(), decs.RUN_DRY))
-        assert(DD.has_annotations(SimpleChild,   decs.RUN_DRY))
-        assert(DD.has_annotations(SimpleChild(), decs.RUN_DRY))
+        assert(DU.has_annotations(SimpleSuper,   decs.RUN_DRY))
+        assert(DU.has_annotations(SimpleSuper(), decs.RUN_DRY))
+        assert(DU.has_annotations(SimpleChild,   decs.RUN_DRY))
+        assert(DU.has_annotations(SimpleChild(), decs.RUN_DRY))
 
 
     def test_key_decoration_survives_annotation(self):
 
         @decs.RunsDry()
         @DootKey.dec.expands("blah")
         def simple(spec, state, blah):
             return blah
 
-        assert(DD.has_annotations(simple,   decs.RUN_DRY))
+        assert(DU.has_annotations(simple,   decs.RUN_DRY))
         assert(simple(None, {"blah":"bloo"}) == "bloo")
 
 
     def test_wrapper_survives_key_decoration(self):
 
         @decs.DryRunSwitch(override=True)
         @DootKey.dec.expands("blah")
         def simple(spec:dict, state:dict, blah:str) -> str:
             """ a simple test func """
             return blah
 
-        assert(DD.has_annotations(simple,   decs.RUN_DRY_SWITCH))
+        assert(DU.has_annotations(simple,   decs.RUN_DRY_SWITCH))
         assert(simple(None, {"blah": "bloo"}) is None)
 
 
     def test_wrapper_survives_method_key_decoration(self):
 
         @decs.DryRunSwitch(override=True)
         class SimpleAction:
 
             @DootKey.dec.expands("blah")
             def __call__(self, spec:dict, state:dict, blah:str) -> str:
                 """ a simple test func """
                 return blah
 
-        assert(DD.has_annotations(SimpleAction,   decs.RUN_DRY_SWITCH))
+        assert(DU.has_annotations(SimpleAction,   decs.RUN_DRY_SWITCH))
         assert(SimpleAction()({}, {"blah": "bloo"}) is None)
 
 
     def test_setting_dryswitch_on_method(self):
 
         class SimpleAction:
 
             @decs.DryRunSwitch(override=True)
             @DootKey.dec.expands("blah")
             def __call__(self, spec:dict, state:dict, blah:str) -> str:
                 """ a simple test func """
                 return blah
 
-        assert(DD.has_annotations(SimpleAction.__call__,   decs.RUN_DRY_SWITCH))
+        assert(DU.has_annotations(SimpleAction.__call__,   decs.RUN_DRY_SWITCH))
         assert(SimpleAction()({}, {"blah": "bloo"}) is None)
 
     def test_wrapping_overriden_by_subclassing(self):
 
         @decs.DryRunSwitch(override=True)
         class SimpleSuper:
 
@@ -182,46 +183,46 @@
 
     def test_gens_tasks(self):
 
         @decs.GeneratesTasks()
         def simple(spec, state):
             return []
 
-        assert(DD.has_annotations(simple, decs.GEN_TASKS))
+        assert(DU.has_annotations(simple, decs.GEN_TASKS))
         assert(isinstance(simple({},{}), list))
 
 
     def test_gens_tasks_raises_error(self):
 
         @decs.GeneratesTasks()
         def simple(spec, state):
             return "blah"
 
-        assert(DD.has_annotations(simple, decs.GEN_TASKS))
+        assert(DU.has_annotations(simple, decs.GEN_TASKS))
         with pytest.raises(doot.errors.DootActionError):
             simple({},{})
 
 
     def test_io_writer_check(self, wrap_locs):
         doot.locs.update({"blah" : dict(loc="blah", protected=True) })
 
         @decs.IOWriter()
         @DootKey.dec.paths("to")
         def simple(spec, state, to):
             return "blah"
 
-        assert(DD.has_annotations(simple, decs.IO_ACT))
+        assert(DU.has_annotations(simple, decs.IO_ACT))
         with pytest.raises(doot.errors.DootTaskError):
             simple(None, {"to": "{blah}"})
 
 
     def test_io_writer_pas(self, wrap_locs):
         doot.locs.update({"blah" : dict(loc="blah", protected=False) })
 
         @decs.IOWriter()
         @DootKey.dec.paths("to")
         def simple(spec, state, to):
             "a simple docstring "
             return "blah"
 
-        assert(DD.has_annotations(simple, decs.IO_ACT))
+        assert(DU.has_annotations(simple, decs.IO_ACT))
         assert(simple(None, {"to": "{blah}"}) == "blah")
```

### Comparing `doot-0.7.0/doot/utils/chain_get.py` & `doot-0.7.1/doot/utils/chain_get.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/utils/check_protocol.py` & `doot-0.7.1/doot/utils/check_protocol.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/utils/log_colour.py` & `doot-0.7.1/doot/utils/log_colour.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/utils/log_config.py` & `doot-0.7.1/doot/utils/log_config.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/utils/log_context.py` & `doot-0.7.1/doot/utils/log_context.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/utils/mock_gen.py` & `doot-0.7.1/doot/utils/mock_gen.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/utils/plugin_selector.py` & `doot-0.7.1/doot/utils/plugin_selector.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/utils/retrievers.py` & `doot-0.7.1/doot/utils/retrievers.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/utils/signal_handler.py` & `doot-0.7.1/doot/utils/signal_handler.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/utils/testing_fixtures.py` & `doot-0.7.1/doot/utils/testing_fixtures.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/utils/trace_helper.py` & `doot-0.7.1/doot/utils/trace_helper.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot/utils/url_expand.py` & `doot-0.7.1/doot/utils/url_expand.py`

 * *Files identical despite different names*

### Comparing `doot-0.7.0/doot.egg-info/PKG-INFO` & `doot-0.7.1/doot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doot
-Version: 0.7.0
+Version: 0.7.1
 Summary: An opinionated, TOML based task runner
 Author-email: jgrey <jgrey.n.plus.one@gmail.com>
 License:  ACAB License © 2022-12-09 John Grey
         
         
         To the maximum extent applicable by law, and any licenses of components of this work:
         
@@ -67,15 +67,15 @@
 Requires-Dist: pytest-mock; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pipreqs; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 
 ![doot](https://github.com/jgrey4296/doot/assets/5943270/170a5631-6175-4d92-8d66-e26aa2c2e472)
 # doot
-Version : 0.7.0  
+Version : 0.7.1  
 Author  : John Grey  
 Date    : 2022-12-09  
 
 ## Overview
 This started out as an opinionated rewrite of the [doit](https://pydoit.org/contents.html) task runner.
 For other, more mature alternatives, see [Luigi](https://github.com/spotify/luigi), and [SnakeMake](https://github.com/snakemake/snakemake)
 and, of course, [GNU Make](https://www.gnu.org/software/make/).
```

### Comparing `doot-0.7.0/doot.egg-info/SOURCES.txt` & `doot-0.7.1/doot.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 doot/_abstract/structs.py
 doot/_abstract/task.py
 doot/_structs/__init__.py
 doot/_structs/action_spec.py
 doot/_structs/artifact.py
 doot/_structs/code_ref.py
 doot/_structs/key.py
-doot/_structs/log.doot
 doot/_structs/param_spec.py
 doot/_structs/sname.py
 doot/_structs/structured_name.py
 doot/_structs/stub.py
 doot/_structs/task_name.py
 doot/_structs/task_spec.py
 doot/_structs/toml_loc.py
@@ -96,15 +95,14 @@
 doot/cmds/step_cmd.py
 doot/cmds/stub_cmd.py
 doot/cmds/__tests/test_list_cmd.py
 doot/control/__init__.py
 doot/control/base_runner.py
 doot/control/base_tracker.py
 doot/control/locations.py
-doot/control/log.doot
 doot/control/overlord.py
 doot/control/runner.py
 doot/control/step_runner.py
 doot/control/tracker.py
 doot/control/__tests/test_locations.py
 doot/control/__tests/test_overlord.py
 doot/control/__tests/test_runner.py
@@ -138,21 +136,22 @@
 doot/task/base_task.py
 doot/task/check_locs.py
 doot/task/specialised_jobs.py
 doot/task/__tests/test_base_job.py
 doot/task/__tests/test_base_task.py
 doot/task/__tests/test_check_locs.py
 doot/utils/__init__.py
+doot/utils/action_decorators.py
 doot/utils/chain_get.py
 doot/utils/check_protocol.py
 doot/utils/decorators.py
 doot/utils/log_colour.py
 doot/utils/log_config.py
 doot/utils/log_context.py
 doot/utils/mock_gen.py
 doot/utils/plugin_selector.py
 doot/utils/retrievers.py
 doot/utils/signal_handler.py
 doot/utils/testing_fixtures.py
 doot/utils/trace_helper.py
 doot/utils/url_expand.py
-doot/utils/__tests/test_decorators.py
+doot/utils/__tests/test_action_decorators.py
```

### Comparing `doot-0.7.0/pyproject.toml` & `doot-0.7.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name            = "doot"
-version         = "0.7.0"
+version         = "0.7.1"
 description     = "An opinionated, TOML based task runner"
 readme          = "README.md"
 requires-python = ">=3.11"
 license         = {file = "LICENSE"}
 keywords        = ["toml","taskrunner"]
 authors         = [
   {email = "jgrey.n.plus.one@gmail.com", name  = "jgrey"}
@@ -86,21 +86,21 @@
 log_cli_level = "INFO"
 log_format    = "%(levelname)s %(name)s : %(message)s"
 
 ##-- end pytest
 
 ##-- bumpver
 [tool.bumpver]
-current_version    = "0.7.0"
+current_version    = "0.7.1"
 version_pattern    = "MAJOR.MINOR.PATCH"
 commit_message     = "[bump]: version {old_version} -> {new_version}"
 tag_message        = "{new_version}"
 tag_scope          = "default"
 commit             = true
-tag                = true
+# tag                = true
 # push             = true
 # pre_commit_hook  = ""
 # post_commit_hook = ""
 
 [tool.bumpver.file_patterns]
 "pyproject.toml"   = [
                    '^version\s+=\s+"{version}"',
```

