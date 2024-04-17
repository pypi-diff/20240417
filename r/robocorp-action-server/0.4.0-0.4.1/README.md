# Comparing `tmp/robocorp_action_server-0.4.0.tar.gz` & `tmp/robocorp_action_server-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_action_server-0.4.0.tar", max compression
+gzip compressed data, was "robocorp_action_server-0.4.1.tar", max compression
```

## Comparing `robocorp_action_server-0.4.0.tar` & `robocorp_action_server-0.4.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0     4055 2024-04-16 20:07:26.948676 robocorp_action_server-0.4.0/README.md
--rw-r--r--   0        0        0     2100 2024-04-16 20:07:26.948676 robocorp_action_server-0.4.0/build.py
--rw-r--r--   0        0        0     1576 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      894 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/README.md
--rw-r--r--   0        0        0      128 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/__init__.py
--rw-r--r--   0        0        0      284 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/__main__.py
--rw-r--r--   0        0        0    18157 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_actions_import.py
--rw-r--r--   0        0        0    20512 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_actions_process_pool.py
--rw-r--r--   0        0        0    11351 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_actions_run.py
--rw-r--r--   0        0        0     1266 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_actions_run_helpers.py
--rw-r--r--   0        0        0     1239 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_api_action_package.py
--rw-r--r--   0        0        0     7726 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_api_run.py
--rw-r--r--   0        0        0     2623 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_app.py
--rw-r--r--   0        0        0      775 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_cli_helpers.py
--rw-r--r--   0        0        0    21166 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_database.py
--rw-r--r--   0        0        0     1875 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_download_rcc.py
--rw-r--r--   0        0        0     3764 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_errors.py
--rw-r--r--   0        0        0      113 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_errors_action_server.py
--rw-r--r--   0        0        0      642 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_gen_ids.py
--rw-r--r--   0        0        0     5215 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_models.py
--rw-r--r--   0        0        0     2764 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_new_project.py
--rw-r--r--   0        0        0        0 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_preload_actions/__init__.py
--rw-r--r--   0        0        0      714 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_preload_actions/preload_actions.py
--rw-r--r--   0        0        0     9519 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_preload_actions/preload_actions_server_main.py
--rw-r--r--   0        0        0     7869 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_preload_actions/preload_actions_streams.py
--rw-r--r--   0        0        0      587 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_preload_actions/preload_actions_teardown.py
--rw-r--r--   0        0        0     4322 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_protocols.py
--rw-r--r--   0        0        0    10444 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_rcc.py
--rw-r--r--   0        0        0      426 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_robo_utils/auth.py
--rw-r--r--   0        0        0     1526 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_robo_utils/callback.py
--rw-r--r--   0        0        0     1282 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_robo_utils/constants.py
--rw-r--r--   0        0        0     1027 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_robo_utils/log_custom_handler.py
--rw-r--r--   0        0        0     1397 2024-04-16 20:07:26.956676 robocorp_action_server-0.4.0/src/robocorp/action_server/_robo_utils/log_formatter.py
--rw-r--r--   0        0        0    19023 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/_robo_utils/process.py
--rw-r--r--   0        0        0      692 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/_robo_utils/run_in_thread.py
--rw-r--r--   0        0        0    13510 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/_robo_utils/system_mutex.py
--rw-r--r--   0        0        0     4031 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/_runs_state_cache.py
--rw-r--r--   0        0        0    15845 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/_selftest.py
--rw-r--r--   0        0        0    11168 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/_server.py
--rw-r--r--   0        0        0    16735 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/_server_expose.py
--rw-r--r--   0        0        0    10278 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/_server_websockets.py
--rw-r--r--   0        0        0     4746 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/_settings.py
--rw-r--r--   0        0        0     1662 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/_slugify.py
--rw-r--r--   0        0        0   880128 2024-04-16 20:08:12.912454 robocorp_action_server-0.4.0/src/robocorp/action_server/_static_contents.py
--rw-r--r--   0        0        0     2403 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/_whitelist.py
--rw-r--r--   0        0        0        6 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/bin/.gitignore
--rw-r--r--   0        0        0    25098 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/cli.py
--rw-r--r--   0        0        0     4730 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/migrations/__init__.py
--rw-r--r--   0        0        0      411 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/migrations/migration_add_action_enabled.py
--rw-r--r--   0        0        0      378 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/migrations/migration_add_action_managed_params.py
--rw-r--r--   0        0        0      375 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/migrations/migration_add_is_consequential.py
--rw-r--r--   0        0        0      260 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/migrations/migration_initial.py
--rw-r--r--   0        0        0        0 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/package/__init__.py
--rw-r--r--   0        0        0      468 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/package/_ask_user.py
--rw-r--r--   0        0        0     7884 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/package/_package_build.py
--rw-r--r--   0        0        0     7666 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/package/_package_build_cli.py
--rw-r--r--   0        0        0     3298 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/package/_package_metadata.py
--rw-r--r--   0        0        0        0 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/py.typed
--rw-r--r--   0        0        0      349 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/README.md
--rw-r--r--   0        0        0        0 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/__init__.py
--rw-r--r--   0        0        0    14886 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/action_package_handling/__init__.py
--rw-r--r--   0        0        0      157 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/action_package_handling/cli_errors.py
--rw-r--r--   0        0        0        0 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/__init__.py
--rw-r--r--   0        0        0     1812 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/_conda_deps.py
--rw-r--r--   0        0        0     6112 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/_deps_protocols.py
--rw-r--r--   0        0        0     1405 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/_package_deps.py
--rw-r--r--   0        0        0     2331 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/_pip_deps.py
--rw-r--r--   0        0        0    23317 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/analyzer.py
--rw-r--r--   0        0        0    23813 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/conda_cloud.py
--rw-r--r--   0        0        0        0 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/__init__.py
--rw-r--r--   0        0        0      849 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_channel.py
--rw-r--r--   0        0        0    11440 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_match_spec.py
--rw-r--r--   0        0        0     9084 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_path.py
--rw-r--r--   0        0        0    13400 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_url.py
--rw-r--r--   0        0        0    25543 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_version.py
--rw-r--r--   0        0        0        0 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/__init__.py
--rw-r--r--   0        0        0     8976 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/pip_distlib_util.py
--rw-r--r--   0        0        0     1431 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_structure.py
--rw-r--r--   0        0        0    14693 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_version.py
--rw-r--r--   0        0        0     7245 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/pypi_cloud.py
--rw-r--r--   0        0        0      319 2024-04-16 20:07:26.960676 robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/termcolors/__init__.py
--rw-r--r--   0        0        0     5949 1970-01-01 00:00:00.000000 robocorp_action_server-0.4.0/setup.py
--rw-r--r--   0        0        0     5245 1970-01-01 00:00:00.000000 robocorp_action_server-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     4055 2024-04-17 18:22:32.005219 robocorp_action_server-0.4.1/README.md
+-rw-r--r--   0        0        0     2100 2024-04-17 18:22:32.005219 robocorp_action_server-0.4.1/build.py
+-rw-r--r--   0        0        0     1576 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      894 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/README.md
+-rw-r--r--   0        0        0      128 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/__init__.py
+-rw-r--r--   0        0        0      284 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/__main__.py
+-rw-r--r--   0        0        0    18829 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_actions_import.py
+-rw-r--r--   0        0        0    20512 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_actions_process_pool.py
+-rw-r--r--   0        0        0    11351 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_actions_run.py
+-rw-r--r--   0        0        0     1266 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_actions_run_helpers.py
+-rw-r--r--   0        0        0     1239 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_api_action_package.py
+-rw-r--r--   0        0        0     7726 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_api_run.py
+-rw-r--r--   0        0        0     2623 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_app.py
+-rw-r--r--   0        0        0      775 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_cli_helpers.py
+-rw-r--r--   0        0        0    21166 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_database.py
+-rw-r--r--   0        0        0     1875 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_download_rcc.py
+-rw-r--r--   0        0        0     3764 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_errors.py
+-rw-r--r--   0        0        0      113 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_errors_action_server.py
+-rw-r--r--   0        0        0      642 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_gen_ids.py
+-rw-r--r--   0        0        0     5215 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_models.py
+-rw-r--r--   0        0        0     2764 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_new_project.py
+-rw-r--r--   0        0        0        0 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_preload_actions/__init__.py
+-rw-r--r--   0        0        0      714 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_preload_actions/preload_actions.py
+-rw-r--r--   0        0        0     9519 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_preload_actions/preload_actions_server_main.py
+-rw-r--r--   0        0        0     7869 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_preload_actions/preload_actions_streams.py
+-rw-r--r--   0        0        0      587 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_preload_actions/preload_actions_teardown.py
+-rw-r--r--   0        0        0     4322 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_protocols.py
+-rw-r--r--   0        0        0    10444 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_rcc.py
+-rw-r--r--   0        0        0      426 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_robo_utils/auth.py
+-rw-r--r--   0        0        0     1526 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_robo_utils/callback.py
+-rw-r--r--   0        0        0     1282 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_robo_utils/constants.py
+-rw-r--r--   0        0        0     1027 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_robo_utils/log_custom_handler.py
+-rw-r--r--   0        0        0     1397 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_robo_utils/log_formatter.py
+-rw-r--r--   0        0        0    19023 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_robo_utils/process.py
+-rw-r--r--   0        0        0      692 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_robo_utils/run_in_thread.py
+-rw-r--r--   0        0        0    13510 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_robo_utils/system_mutex.py
+-rw-r--r--   0        0        0     4031 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_runs_state_cache.py
+-rw-r--r--   0        0        0    15845 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_selftest.py
+-rw-r--r--   0        0        0    11168 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_server.py
+-rw-r--r--   0        0        0    16735 2024-04-17 18:22:32.013219 robocorp_action_server-0.4.1/src/robocorp/action_server/_server_expose.py
+-rw-r--r--   0        0        0    10278 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/_server_websockets.py
+-rw-r--r--   0        0        0     4746 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/_settings.py
+-rw-r--r--   0        0        0     1662 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/_slugify.py
+-rw-r--r--   0        0        0   880128 2024-04-17 18:23:19.293278 robocorp_action_server-0.4.1/src/robocorp/action_server/_static_contents.py
+-rw-r--r--   0        0        0     2403 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/_whitelist.py
+-rw-r--r--   0        0        0        6 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/bin/.gitignore
+-rw-r--r--   0        0        0    25098 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/cli.py
+-rw-r--r--   0        0        0     4730 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/migrations/__init__.py
+-rw-r--r--   0        0        0      411 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/migrations/migration_add_action_enabled.py
+-rw-r--r--   0        0        0      378 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/migrations/migration_add_action_managed_params.py
+-rw-r--r--   0        0        0      375 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/migrations/migration_add_is_consequential.py
+-rw-r--r--   0        0        0      260 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/migrations/migration_initial.py
+-rw-r--r--   0        0        0        0 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/package/__init__.py
+-rw-r--r--   0        0        0      468 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/package/_ask_user.py
+-rw-r--r--   0        0        0     7884 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/package/_package_build.py
+-rw-r--r--   0        0        0     7666 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/package/_package_build_cli.py
+-rw-r--r--   0        0        0     3298 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/package/_package_metadata.py
+-rw-r--r--   0        0        0        0 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/py.typed
+-rw-r--r--   0        0        0      349 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/__init__.py
+-rw-r--r--   0        0        0    14886 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/action_package_handling/__init__.py
+-rw-r--r--   0        0        0      157 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/action_package_handling/cli_errors.py
+-rw-r--r--   0        0        0        0 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/__init__.py
+-rw-r--r--   0        0        0     1812 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/_conda_deps.py
+-rw-r--r--   0        0        0     6112 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/_deps_protocols.py
+-rw-r--r--   0        0        0     1405 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/_package_deps.py
+-rw-r--r--   0        0        0     2331 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/_pip_deps.py
+-rw-r--r--   0        0        0    23317 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/analyzer.py
+-rw-r--r--   0        0        0    23813 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/conda_cloud.py
+-rw-r--r--   0        0        0        0 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/__init__.py
+-rw-r--r--   0        0        0      849 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_channel.py
+-rw-r--r--   0        0        0    11440 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_match_spec.py
+-rw-r--r--   0        0        0     9084 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_path.py
+-rw-r--r--   0        0        0    13400 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_url.py
+-rw-r--r--   0        0        0    25543 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_version.py
+-rw-r--r--   0        0        0        0 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/__init__.py
+-rw-r--r--   0        0        0     8976 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/pip_distlib_util.py
+-rw-r--r--   0        0        0     1431 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_structure.py
+-rw-r--r--   0        0        0    14693 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_version.py
+-rw-r--r--   0        0        0     7245 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/pypi_cloud.py
+-rw-r--r--   0        0        0      319 2024-04-17 18:22:32.017219 robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/termcolors/__init__.py
+-rw-r--r--   0        0        0     5949 1970-01-01 00:00:00.000000 robocorp_action_server-0.4.1/setup.py
+-rw-r--r--   0        0        0     5245 1970-01-01 00:00:00.000000 robocorp_action_server-0.4.1/PKG-INFO
```

### Comparing `robocorp_action_server-0.4.0/README.md` & `robocorp_action_server-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/build.py` & `robocorp_action_server-0.4.1/build.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/pyproject.toml` & `robocorp_action_server-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-action-server"
-version = "0.4.0"
+version = "0.4.1"
 description = "Robocorp local task server"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robocorp/"
 license = "Apache-2.0"
```

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/README.md` & `robocorp_action_server-0.4.1/src/robocorp/action_server/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_actions_import.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_actions_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,14 +258,26 @@
         else:
             raise ActionServerValidationError(
                 f"Error, the `robocorp-actions` version is: {v_as_str}.\n"
                 f"Expected it to be {expected_version_str} or higher.\n"
                 f"Please update the `robocorp-actions` version in your python environment (python: {sys.executable})\n"
             )
 
+    min_version_for_encryption_with_auth_tag = (0, 2, 1)
+    if v < min_version_for_encryption_with_auth_tag:
+        v_as_str = ".".join(str(x) for x in v)
+        log.critical(
+            f"Warning: the `robocorp-actions` version is: {v_as_str}.\n"
+            f"To receive encrypted secrets, robocorp-actions 0.2.1 or newer is required.\n"
+            f"Please update the version in: {original_conda_yaml}\n"
+            "(proceeding with initalization but actions receiving encrypted secrets will\n"
+            "not work properly -- on future versions of the action server, support for \n"
+            "this version of robocorp-actions will be removed)."
+        )
+
     _add_actions_to_db(
         datadir,
         env,
         import_path,
         action_package,
         disable_not_imported=disable_not_imported,
         skip_lint=skip_lint,
```

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_actions_process_pool.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_actions_process_pool.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_actions_run.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_actions_run.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_actions_run_helpers.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_actions_run_helpers.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_api_action_package.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_api_action_package.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_api_run.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_api_run.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_app.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_app.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_cli_helpers.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_cli_helpers.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_database.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_database.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_download_rcc.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_download_rcc.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_errors.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_errors.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_gen_ids.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_gen_ids.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_models.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_models.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_new_project.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_new_project.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_preload_actions/preload_actions.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_preload_actions/preload_actions.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_preload_actions/preload_actions_server_main.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_preload_actions/preload_actions_server_main.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_preload_actions/preload_actions_streams.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_preload_actions/preload_actions_streams.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_preload_actions/preload_actions_teardown.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_preload_actions/preload_actions_teardown.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_protocols.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_protocols.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_rcc.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_rcc.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_robo_utils/callback.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_robo_utils/callback.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_robo_utils/constants.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_robo_utils/constants.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_robo_utils/log_custom_handler.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_robo_utils/log_custom_handler.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_robo_utils/log_formatter.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_robo_utils/log_formatter.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_robo_utils/process.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_robo_utils/process.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_robo_utils/run_in_thread.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_robo_utils/run_in_thread.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_robo_utils/system_mutex.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_robo_utils/system_mutex.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_runs_state_cache.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_runs_state_cache.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_selftest.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_selftest.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_server.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_server.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_server_expose.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_server_expose.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_server_websockets.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_server_websockets.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_settings.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_settings.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_slugify.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_slugify.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_static_contents.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_static_contents.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/_whitelist.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/_whitelist.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/cli.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/cli.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/migrations/__init__.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/package/_package_build.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/package/_package_build.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/package/_package_build_cli.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/package/_package_build_cli.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/package/_package_metadata.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/package/_package_metadata.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/action_package_handling/__init__.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/action_package_handling/__init__.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/_conda_deps.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/_conda_deps.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/_deps_protocols.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/_deps_protocols.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/_package_deps.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/_package_deps.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/_pip_deps.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/_pip_deps.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/analyzer.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/analyzer.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/conda_cloud.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/conda_cloud.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_channel.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_channel.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_match_spec.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_match_spec.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_path.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_path.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_url.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_url.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_version.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/conda_impl/conda_version.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/pip_distlib_util.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/pip_distlib_util.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_structure.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_structure.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_version.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_version.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/src/robocorp/action_server/vendored_deps/package_deps/pypi_cloud.py` & `robocorp_action_server-0.4.1/src/robocorp/action_server/vendored_deps/package_deps/pypi_cloud.py`

 * *Files identical despite different names*

### Comparing `robocorp_action_server-0.4.0/setup.py` & `robocorp_action_server-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
  'websockets>=12.0,<13.0']
 
 entry_points = \
 {'console_scripts': ['action-server = robocorp.action_server.cli:main']}
 
 setup_kwargs = {
     'name': 'robocorp-action-server',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': 'Robocorp local task server',
     'long_description': '# robocorp-action-server\n\n[Robocorp Action Server](https://github.com/robocorp/robocorp#readme) is a Python framework designed to simplify the deployment of actions (AI or otherwise).\n\nAn `action` in this case is defined as a Python function (which has inputs/outputs defined), which is served by the `Robocorp Action Server`.\n\nThe `Robocorp Action Server` automatically generates an OpenAPI spec for your Python code, enabling different AI/LLM Agents to understand and call your Action. It also manages the Action lifecycle and provides full traceability of what happened during runs.\n\n## 1. Install Action Server\n\nAction Server is available as a stand-alone fully signed executable and via `pip install robocorp-action-server`.\n> We recommend the executable to prevent confusion in case you have multiple/crowded Python environments, etc.\n\n#### For macOS\n\n```sh\n# Install Robocorp Action Server\nbrew update\nbrew install robocorp/tools/action-server \n```\n\n#### For Windows\n\n```sh\n# Download Robocorp Action Server\ncurl -o action-server.exe https://downloads.robocorp.com/action-server/releases/latest/windows64/action-server.exe\n\n# Add to PATH or move to a folder that is in PATH\nsetx PATH=%PATH%;%CD%\n```\n\n#### For Linux\n\n```sh\n# Download Robocorp Action Server\ncurl -o action-server https://downloads.robocorp.com/action-server/releases/latest/linux64/action-server\nchmod a+x action-server\n\n# Add to PATH or move to a folder that is in PATH\nsudo mv action-server /usr/local/bin/\n```\n\n## 2. Run your first Action\n\n```sh\n# Bootstrap a new project using this template.\n# You\'ll be prompted for the name of the project (directory):\naction-server new\n\n# Start Action Server \ncd my-project\naction-server start --expose\n```\n\n👉 You should now have an Action Server running locally at: [http://localhost:8080](http://localhost:8080), so open that in your browser and the web UI will guide you further.\n\n👉 Using the `--expose` -flag, you also get a public internet-facing URL (something like "https://twently-cuddly-dinosaurs.robocorp.link") and the related token. These are the details that you need to configure your AI Agent to have access to your Action\n\n## What do you need in your Action Package\n\nAn `Action Package` is currently defined as a local folder that contains at least one Python file containing an action entry point (a Python function marked with `@action` -decorator from `robocorp.actions`).\n\nThe `package.yaml` file is required for specifying the Python environment and dependencies for your Action ([RCC](https://github.com/robocorp/rcc/) will be used to automatically bootstrap it and keep it updated given the `package.yaml` contents).\n\n> Note: the `package.yaml` is optional if the action server is not being used as a standalone (i.e.: if it was pip-installed it can use the same python environment where it\'s installed).\n\n### Bootstrapping a new Action\n\nStart new projects with:\n\n`action-server new`\n\nNote: the `action-server` executable should be automatically added to your python installation after `pip install robocorp-action-server`, but if for some reason it wasn\'t pip-installed, it\'s also possible to use `python -m robocorp.action_server` instead of `action-server`.\n\nAfter creating the project, it\'s possible to serve the actions under the current directory with:\n\n`action-server start`\n\nFor example: When running `action-server start`, the action server will scan for existing actions under the current directory, and it\'ll start serving those.\n\nAfter it\'s started, it\'s possible to access the following URLs:\n\n- `/index.html`: UI for the Action Server.\n- `/openapi.json`: Provides the openapi spec for the action server.\n- `/docs`: Provides access to the APIs available in the server and a UI to test it.\n\n## Documentation\n\nExplore our [docs](https://github.com/robocorp/robocorp/tree/master/action_server/docs) for extensive documentation.\n\n## Changelog\n\nA list of releases and corresponding changes can be found in the [changelog](https://github.com/robocorp/robocorp/blob/master/action_server/docs/CHANGELOG.md).\n',
     'author': 'Fabio Z.',
     'author_email': 'fabio@robocorp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/robocorp/robocorp/',
```

### Comparing `robocorp_action_server-0.4.0/PKG-INFO` & `robocorp_action_server-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-action-server
-Version: 0.4.0
+Version: 0.4.1
 Summary: Robocorp local task server
 Home-page: https://github.com/robocorp/robocorp/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

