# Comparing `tmp/slack_cli_hooks-0.0.0.dev2.tar.gz` & `tmp/slack_cli_hooks-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack_cli_hooks-0.0.0.dev2.tar", last modified: Wed Jan 24 20:11:03 2024, max compression
+gzip compressed data, was "slack_cli_hooks-0.0.1.tar", last modified: Wed Apr 17 17:53:33 2024, max compression
```

## Comparing `slack_cli_hooks-0.0.0.dev2.tar` & `slack_cli_hooks-0.0.1.tar`

### file list

```diff
@@ -1,34 +1,32 @@
-drwxr-xr-x   0 wbergamin   (502) staff       (20)        0 2024-01-24 20:11:03.959276 slack_cli_hooks-0.0.0.dev2/
--rw-r--r--   0 wbergamin   (502) staff       (20)     1081 2023-12-04 16:07:50.000000 slack_cli_hooks-0.0.0.dev2/LICENSE
--rw-r--r--   0 wbergamin   (502) staff       (20)       51 2023-12-04 16:10:47.000000 slack_cli_hooks-0.0.0.dev2/MANIFEST.in
--rw-r--r--   0 wbergamin   (502) staff       (20)     4391 2024-01-24 20:11:03.958908 slack_cli_hooks-0.0.0.dev2/PKG-INFO
--rw-r--r--   0 wbergamin   (502) staff       (20)     3292 2024-01-23 18:33:05.000000 slack_cli_hooks-0.0.0.dev2/README.md
--rw-r--r--   0 wbergamin   (502) staff       (20)     1547 2024-01-24 20:00:46.000000 slack_cli_hooks-0.0.0.dev2/pyproject.toml
--rw-r--r--   0 wbergamin   (502) staff       (20)       22 2023-12-04 16:07:50.000000 slack_cli_hooks-0.0.0.dev2/requirements.txt
--rw-r--r--   0 wbergamin   (502) staff       (20)       38 2024-01-24 20:11:03.959355 slack_cli_hooks-0.0.0.dev2/setup.cfg
-drwxr-xr-x   0 wbergamin   (502) staff       (20)        0 2024-01-24 20:11:03.947576 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/
--rw-r--r--   0 wbergamin   (502) staff       (20)      508 2023-12-13 15:31:21.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/__init__.py
-drwxr-xr-x   0 wbergamin   (502) staff       (20)        0 2024-01-24 20:11:03.949409 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/error/
--rw-r--r--   0 wbergamin   (502) staff       (20)      157 2024-01-05 17:06:46.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/error/__init__.py
-drwxr-xr-x   0 wbergamin   (502) staff       (20)        0 2024-01-24 20:11:03.953720 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/hooks/
--rw-r--r--   0 wbergamin   (502) staff       (20)       51 2023-12-13 15:31:21.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/hooks/__init__.py
--rw-r--r--   0 wbergamin   (502) staff       (20)     3458 2024-01-23 21:23:25.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/hooks/check_update.py
--rw-r--r--   0 wbergamin   (502) staff       (20)      787 2024-01-05 17:06:46.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/hooks/get_hooks.py
--rw-r--r--   0 wbergamin   (502) staff       (20)     1273 2023-12-20 17:57:58.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/hooks/get_manifest.py
--rw-r--r--   0 wbergamin   (502) staff       (20)     1824 2024-01-24 19:56:56.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/hooks/start.py
-drwxr-xr-x   0 wbergamin   (502) staff       (20)        0 2024-01-24 20:11:03.954770 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/hooks/utils/
--rw-r--r--   0 wbergamin   (502) staff       (20)       89 2023-12-19 20:50:29.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/hooks/utils/__init__.py
--rw-r--r--   0 wbergamin   (502) staff       (20)      684 2024-01-05 17:06:46.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/hooks/utils/managed_os_env_vars.py
-drwxr-xr-x   0 wbergamin   (502) staff       (20)        0 2024-01-24 20:11:03.957748 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/protocol/
--rw-r--r--   0 wbergamin   (502) staff       (20)      712 2023-12-13 15:31:21.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/protocol/__init__.py
--rw-r--r--   0 wbergamin   (502) staff       (20)      564 2023-12-13 15:31:21.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/protocol/default_protocol.py
--rw-r--r--   0 wbergamin   (502) staff       (20)      655 2023-12-13 15:31:21.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/protocol/message_boundary_protocol.py
--rw-r--r--   0 wbergamin   (502) staff       (20)     1395 2023-12-13 15:31:21.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/protocol/protocol.py
--rw-r--r--   0 wbergamin   (502) staff       (20)        0 2023-12-13 15:31:21.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/py.typed
--rw-r--r--   0 wbergamin   (502) staff       (20)      103 2024-01-24 20:01:31.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/version.py
-drwxr-xr-x   0 wbergamin   (502) staff       (20)        0 2024-01-24 20:11:03.958418 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks.egg-info/
--rw-r--r--   0 wbergamin   (502) staff       (20)     4391 2024-01-24 20:11:03.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks.egg-info/PKG-INFO
--rw-r--r--   0 wbergamin   (502) staff       (20)      809 2024-01-24 20:11:03.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks.egg-info/SOURCES.txt
--rw-r--r--   0 wbergamin   (502) staff       (20)        1 2024-01-24 20:11:03.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks.egg-info/dependency_links.txt
--rw-r--r--   0 wbergamin   (502) staff       (20)       22 2024-01-24 20:11:03.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks.egg-info/requires.txt
--rw-r--r--   0 wbergamin   (502) staff       (20)       16 2024-01-24 20:11:03.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:53:33.505679 slack_cli_hooks-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-17 17:53:23.000000 slack_cli_hooks-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-17 17:53:23.000000 slack_cli_hooks-0.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-04-17 17:53:33.505679 slack_cli_hooks-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-04-17 17:53:23.000000 slack_cli_hooks-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-17 17:53:23.000000 slack_cli_hooks-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-17 17:53:23.000000 slack_cli_hooks-0.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 17:53:33.505679 slack_cli_hooks-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:53:33.501679 slack_cli_hooks-0.0.1/slack_cli_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-17 17:53:23.000000 slack_cli_hooks-0.0.1/slack_cli_hooks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:53:33.505679 slack_cli_hooks-0.0.1/slack_cli_hooks/error/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-17 17:53:23.000000 slack_cli_hooks-0.0.1/slack_cli_hooks/error/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:53:33.505679 slack_cli_hooks-0.0.1/slack_cli_hooks/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-17 17:53:23.000000 slack_cli_hooks-0.0.1/slack_cli_hooks/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-17 17:53:23.000000 slack_cli_hooks-0.0.1/slack_cli_hooks/hooks/check_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-17 17:53:23.000000 slack_cli_hooks-0.0.1/slack_cli_hooks/hooks/doctor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-17 17:53:23.000000 slack_cli_hooks-0.0.1/slack_cli_hooks/hooks/get_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-17 17:53:23.000000 slack_cli_hooks-0.0.1/slack_cli_hooks/hooks/get_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-17 17:53:23.000000 slack_cli_hooks-0.0.1/slack_cli_hooks/hooks/start.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:53:33.505679 slack_cli_hooks-0.0.1/slack_cli_hooks/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-17 17:53:23.000000 slack_cli_hooks-0.0.1/slack_cli_hooks/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-17 17:53:23.000000 slack_cli_hooks-0.0.1/slack_cli_hooks/protocol/default_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-17 17:53:23.000000 slack_cli_hooks-0.0.1/slack_cli_hooks/protocol/message_boundary_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-17 17:53:23.000000 slack_cli_hooks-0.0.1/slack_cli_hooks/protocol/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:53:23.000000 slack_cli_hooks-0.0.1/slack_cli_hooks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-17 17:53:23.000000 slack_cli_hooks-0.0.1/slack_cli_hooks/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:53:33.505679 slack_cli_hooks-0.0.1/slack_cli_hooks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-04-17 17:53:33.000000 slack_cli_hooks-0.0.1/slack_cli_hooks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-17 17:53:33.000000 slack_cli_hooks-0.0.1/slack_cli_hooks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 17:53:33.000000 slack_cli_hooks-0.0.1/slack_cli_hooks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-17 17:53:33.000000 slack_cli_hooks-0.0.1/slack_cli_hooks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-17 17:53:33.000000 slack_cli_hooks-0.0.1/slack_cli_hooks.egg-info/top_level.txt
```

### Comparing `slack_cli_hooks-0.0.0.dev2/LICENSE` & `slack_cli_hooks-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `slack_cli_hooks-0.0.0.dev2/PKG-INFO` & `slack_cli_hooks-0.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack_cli_hooks
-Version: 0.0.0.dev2
+Version: 0.0.1
 Summary: The Slack CLI contract implementation for Bolt Python
 Author-email: "Slack Technologies, LLC" <opensource@slack.com>
 License: MIT
 Project-URL: Source Code, https://github.com/slackapi/python-slack-hooks
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -19,22 +19,25 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: slack_bolt<2,>=1.18.0
+Requires-Dist: packaging<25
 
 <h1 align="center">Python Slack Hooks</h1>
 
 <p align="center">
     <a href="https://pypi.org/project/slack-cli-hooks/">
         <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/slack-cli-hooks?style=flat-square"></a>
     <a href="https://pypi.org/project/slack-cli-hooks/">
         <img alt="Python Versions" src="https://img.shields.io/pypi/pyversions/slack-cli-hooks.svg?style=flat-square"></a>
+    <a href="https://codecov.io/gh/slackapi/python-slack-hooks">
+        <img alt="Codecov" src="https://img.shields.io/codecov/c/gh/slackapi/python-slack-hooks?style=flat-square"></a>
 </p>
 
 This library defines the contract between the
 [Slack CLI](https://api.slack.com/automation/cli/install) and
 [Bolt for Python](https://slack.dev/bolt-python/).
 
 ## Overview
@@ -53,19 +56,20 @@
 
 A Slack CLI-compatible Slack application includes a `./slack.json` file that contains hooks specific to that project. Each hook is associated with commands that are available in the Slack CLI. By default, `get-hooks` retrieves all of the [supported hooks](#supported-hooks) and their corresponding scripts as defined in this library.
 
 The CLI will always use the version of the `python-slack-hooks` that is specified in the project's `requirements.txt`.
 
 ### Supported Hooks
 
-The hooks currently supported for use within the Slack CLI include `check-update`, `get-hooks`, `get-manifest`, and `start`:
+The hooks currently supported for use within the Slack CLI include `check-update`, `doctor`, `get-hooks`, `get-manifest`, and `start`:
 
 | Hook Name  | CLI Command  | File  |  Description  |
 | --- | --- | --- | --- |
 | `check-update` | `slack update` | [check_update.py](./slack_cli_hooks/hooks/check_update.py) | Checks the project's Slack dependencies to determine whether or not any libraries need to be updated. |
+| `doctor` | `slack doctor` | [doctor.py](./slack_cli_hooks/hooks/doctor.py) | Returns runtime versions and other system dependencies required by the application. |
 | `get-hooks` | All | [get_hooks.py](./slack_cli_hooks/hooks/get_hooks.py) | Fetches the list of available hooks for the CLI from this repository. |
 | `get-manifest` | `slack manifest` | [get_manifest.py](./slack_cli_hooks/hooks/get_manifest.py) | Converts a `manifest.json` file into a valid manifest JSON payload. |
 | `start` | `slack run` | [start.py](./slack_cli_hooks/hooks/start.py) | While developing locally, the CLI manages a socket connection with Slack's backend and utilizes this hook for events received via this connection. |
 
 ### Overriding Hooks
 
 To customize the behavior of a hook, add the hook to your application's `/slack.json` file, and provide a corresponding script to be executed.
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: slack_cli_hooks Version: 0.0.0.dev2 Summary: The
-Slack CLI contract implementation for Bolt Python Author-email: "Slack
-Technologies, LLC"
+Metadata-Version: 2.1 Name: slack_cli_hooks Version: 0.0.1 Summary: The Slack
+CLI contract implementation for Bolt Python Author-email: "Slack Technologies,
+LLC"
 slack.com> License: MIT Project-URL: Source Code, https://github.com/slackapi/
 python-slack-hooks Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Environment :: Console Classifier: Intended Audience :: Developers Classifier:
 Topic :: Office/Business Classifier: Topic :: Software Development Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Programming Language ::
 Python :: Implementation :: CPython Classifier: Programming Language :: Python
 :: Implementation :: PyPy Requires-Python: >=3.9 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: slack_bolt<2,>=1.18.0
+Requires-Dist: packaging<25
                        ************ PPyytthhoonn SSllaacckk HHooookkss ************
-                       _[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]
+                  _[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_C_o_d_e_c_o_v_]
 This library defines the contract between the [Slack CLI](https://
 api.slack.com/automation/cli/install) and [Bolt for Python](https://slack.dev/
 bolt-python/). ## Overview This library enables inter-process communication
 between the [Slack CLI](https://api.slack.com/automation/cli/install) and
 applications built with Bolt for Python. When used together, the CLI delegates
 various tasks to the Bolt application by invoking processes ("hooks") and then
 making use of the responses provided by each hook's `stdout`. For a complete
@@ -27,29 +28,31 @@
 slack-bolt/) is recommended. ## Usage A Slack CLI-compatible Slack application
 includes a `./slack.json` file that contains hooks specific to that project.
 Each hook is associated with commands that are available in the Slack CLI. By
 default, `get-hooks` retrieves all of the [supported hooks](#supported-hooks)
 and their corresponding scripts as defined in this library. The CLI will always
 use the version of the `python-slack-hooks` that is specified in the project's
 `requirements.txt`. ### Supported Hooks The hooks currently supported for use
-within the Slack CLI include `check-update`, `get-hooks`, `get-manifest`, and
-`start`: | Hook Name | CLI Command | File | Description | | --- | --- | --- | -
--- | | `check-update` | `slack update` | [check_update.py](./slack_cli_hooks/
-hooks/check_update.py) | Checks the project's Slack dependencies to determine
-whether or not any libraries need to be updated. | | `get-hooks` | All |
-[get_hooks.py](./slack_cli_hooks/hooks/get_hooks.py) | Fetches the list of
-available hooks for the CLI from this repository. | | `get-manifest` | `slack
-manifest` | [get_manifest.py](./slack_cli_hooks/hooks/get_manifest.py) |
-Converts a `manifest.json` file into a valid manifest JSON payload. | | `start`
-| `slack run` | [start.py](./slack_cli_hooks/hooks/start.py) | While developing
-locally, the CLI manages a socket connection with Slack's backend and utilizes
-this hook for events received via this connection. | ### Overriding Hooks To
-customize the behavior of a hook, add the hook to your application's `/
-slack.json` file, and provide a corresponding script to be executed. When
-commands are run, the Slack CLI will look to the project's hook definitions and
-use those instead of what's defined in this library, if provided. Below is an
-example `/slack.json` file that overrides the default `start`: ```json
-{ "hooks": { "get-hooks": "python3 -m slack_cli_hooks.hooks.get_hooks",
-"start": "python3 app.py" } } ``` ## Contributing Contributions are always
-welcome! Please review the [contributing guidelines](https://github.com/
-slackapi/python-slack-hooks/blob/main/.github/CONTRIBUTING.md) for more
-information.
+within the Slack CLI include `check-update`, `doctor`, `get-hooks`, `get-
+manifest`, and `start`: | Hook Name | CLI Command | File | Description | | --
+- | --- | --- | --- | | `check-update` | `slack update` | [check_update.py](./
+slack_cli_hooks/hooks/check_update.py) | Checks the project's Slack
+dependencies to determine whether or not any libraries need to be updated. | |
+`doctor` | `slack doctor` | [doctor.py](./slack_cli_hooks/hooks/doctor.py) |
+Returns runtime versions and other system dependencies required by the
+application. | | `get-hooks` | All | [get_hooks.py](./slack_cli_hooks/hooks/
+get_hooks.py) | Fetches the list of available hooks for the CLI from this
+repository. | | `get-manifest` | `slack manifest` | [get_manifest.py](./
+slack_cli_hooks/hooks/get_manifest.py) | Converts a `manifest.json` file into a
+valid manifest JSON payload. | | `start` | `slack run` | [start.py](./
+slack_cli_hooks/hooks/start.py) | While developing locally, the CLI manages a
+socket connection with Slack's backend and utilizes this hook for events
+received via this connection. | ### Overriding Hooks To customize the behavior
+of a hook, add the hook to your application's `/slack.json` file, and provide a
+corresponding script to be executed. When commands are run, the Slack CLI will
+look to the project's hook definitions and use those instead of what's defined
+in this library, if provided. Below is an example `/slack.json` file that
+overrides the default `start`: ```json { "hooks": { "get-hooks": "python3 -
+m slack_cli_hooks.hooks.get_hooks", "start": "python3 app.py" } } ``` ##
+Contributing Contributions are always welcome! Please review the [contributing
+guidelines](https://github.com/slackapi/python-slack-hooks/blob/main/.github/
+CONTRIBUTING.md) for more information.
```

### Comparing `slack_cli_hooks-0.0.0.dev2/README.md` & `slack_cli_hooks-0.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 <h1 align="center">Python Slack Hooks</h1>
 
 <p align="center">
     <a href="https://pypi.org/project/slack-cli-hooks/">
         <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/slack-cli-hooks?style=flat-square"></a>
     <a href="https://pypi.org/project/slack-cli-hooks/">
         <img alt="Python Versions" src="https://img.shields.io/pypi/pyversions/slack-cli-hooks.svg?style=flat-square"></a>
+    <a href="https://codecov.io/gh/slackapi/python-slack-hooks">
+        <img alt="Codecov" src="https://img.shields.io/codecov/c/gh/slackapi/python-slack-hooks?style=flat-square"></a>
 </p>
 
 This library defines the contract between the
 [Slack CLI](https://api.slack.com/automation/cli/install) and
 [Bolt for Python](https://slack.dev/bolt-python/).
 
 ## Overview
@@ -27,19 +29,20 @@
 
 A Slack CLI-compatible Slack application includes a `./slack.json` file that contains hooks specific to that project. Each hook is associated with commands that are available in the Slack CLI. By default, `get-hooks` retrieves all of the [supported hooks](#supported-hooks) and their corresponding scripts as defined in this library.
 
 The CLI will always use the version of the `python-slack-hooks` that is specified in the project's `requirements.txt`.
 
 ### Supported Hooks
 
-The hooks currently supported for use within the Slack CLI include `check-update`, `get-hooks`, `get-manifest`, and `start`:
+The hooks currently supported for use within the Slack CLI include `check-update`, `doctor`, `get-hooks`, `get-manifest`, and `start`:
 
 | Hook Name  | CLI Command  | File  |  Description  |
 | --- | --- | --- | --- |
 | `check-update` | `slack update` | [check_update.py](./slack_cli_hooks/hooks/check_update.py) | Checks the project's Slack dependencies to determine whether or not any libraries need to be updated. |
+| `doctor` | `slack doctor` | [doctor.py](./slack_cli_hooks/hooks/doctor.py) | Returns runtime versions and other system dependencies required by the application. |
 | `get-hooks` | All | [get_hooks.py](./slack_cli_hooks/hooks/get_hooks.py) | Fetches the list of available hooks for the CLI from this repository. |
 | `get-manifest` | `slack manifest` | [get_manifest.py](./slack_cli_hooks/hooks/get_manifest.py) | Converts a `manifest.json` file into a valid manifest JSON payload. |
 | `start` | `slack run` | [start.py](./slack_cli_hooks/hooks/start.py) | While developing locally, the CLI manages a socket connection with Slack's backend and utilizes this hook for events received via this connection. |
 
 ### Overriding Hooks
 
 To customize the behavior of a hook, add the hook to your application's `/slack.json` file, and provide a corresponding script to be executed.
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
                        ************ PPyytthhoonn SSllaacckk HHooookkss ************
-                       _[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]
+                  _[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_C_o_d_e_c_o_v_]
 This library defines the contract between the [Slack CLI](https://
 api.slack.com/automation/cli/install) and [Bolt for Python](https://slack.dev/
 bolt-python/). ## Overview This library enables inter-process communication
 between the [Slack CLI](https://api.slack.com/automation/cli/install) and
 applications built with Bolt for Python. When used together, the CLI delegates
 various tasks to the Bolt application by invoking processes ("hooks") and then
 making use of the responses provided by each hook's `stdout`. For a complete
@@ -12,29 +12,31 @@
 slack-bolt/) is recommended. ## Usage A Slack CLI-compatible Slack application
 includes a `./slack.json` file that contains hooks specific to that project.
 Each hook is associated with commands that are available in the Slack CLI. By
 default, `get-hooks` retrieves all of the [supported hooks](#supported-hooks)
 and their corresponding scripts as defined in this library. The CLI will always
 use the version of the `python-slack-hooks` that is specified in the project's
 `requirements.txt`. ### Supported Hooks The hooks currently supported for use
-within the Slack CLI include `check-update`, `get-hooks`, `get-manifest`, and
-`start`: | Hook Name | CLI Command | File | Description | | --- | --- | --- | -
--- | | `check-update` | `slack update` | [check_update.py](./slack_cli_hooks/
-hooks/check_update.py) | Checks the project's Slack dependencies to determine
-whether or not any libraries need to be updated. | | `get-hooks` | All |
-[get_hooks.py](./slack_cli_hooks/hooks/get_hooks.py) | Fetches the list of
-available hooks for the CLI from this repository. | | `get-manifest` | `slack
-manifest` | [get_manifest.py](./slack_cli_hooks/hooks/get_manifest.py) |
-Converts a `manifest.json` file into a valid manifest JSON payload. | | `start`
-| `slack run` | [start.py](./slack_cli_hooks/hooks/start.py) | While developing
-locally, the CLI manages a socket connection with Slack's backend and utilizes
-this hook for events received via this connection. | ### Overriding Hooks To
-customize the behavior of a hook, add the hook to your application's `/
-slack.json` file, and provide a corresponding script to be executed. When
-commands are run, the Slack CLI will look to the project's hook definitions and
-use those instead of what's defined in this library, if provided. Below is an
-example `/slack.json` file that overrides the default `start`: ```json
-{ "hooks": { "get-hooks": "python3 -m slack_cli_hooks.hooks.get_hooks",
-"start": "python3 app.py" } } ``` ## Contributing Contributions are always
-welcome! Please review the [contributing guidelines](https://github.com/
-slackapi/python-slack-hooks/blob/main/.github/CONTRIBUTING.md) for more
-information.
+within the Slack CLI include `check-update`, `doctor`, `get-hooks`, `get-
+manifest`, and `start`: | Hook Name | CLI Command | File | Description | | --
+- | --- | --- | --- | | `check-update` | `slack update` | [check_update.py](./
+slack_cli_hooks/hooks/check_update.py) | Checks the project's Slack
+dependencies to determine whether or not any libraries need to be updated. | |
+`doctor` | `slack doctor` | [doctor.py](./slack_cli_hooks/hooks/doctor.py) |
+Returns runtime versions and other system dependencies required by the
+application. | | `get-hooks` | All | [get_hooks.py](./slack_cli_hooks/hooks/
+get_hooks.py) | Fetches the list of available hooks for the CLI from this
+repository. | | `get-manifest` | `slack manifest` | [get_manifest.py](./
+slack_cli_hooks/hooks/get_manifest.py) | Converts a `manifest.json` file into a
+valid manifest JSON payload. | | `start` | `slack run` | [start.py](./
+slack_cli_hooks/hooks/start.py) | While developing locally, the CLI manages a
+socket connection with Slack's backend and utilizes this hook for events
+received via this connection. | ### Overriding Hooks To customize the behavior
+of a hook, add the hook to your application's `/slack.json` file, and provide a
+corresponding script to be executed. When commands are run, the Slack CLI will
+look to the project's hook definitions and use those instead of what's defined
+in this library, if provided. Below is an example `/slack.json` file that
+overrides the default `start`: ```json { "hooks": { "get-hooks": "python3 -
+m slack_cli_hooks.hooks.get_hooks", "start": "python3 app.py" } } ``` ##
+Contributing Contributions are always welcome! Please review the [contributing
+guidelines](https://github.com/slackapi/python-slack-hooks/blob/main/.github/
+CONTRIBUTING.md) for more information.
```

### Comparing `slack_cli_hooks-0.0.0.dev2/pyproject.toml` & `slack_cli_hooks-0.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/hooks/check_update.py` & `slack_cli_hooks-0.0.1/slack_cli_hooks/hooks/check_update.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,18 +26,18 @@
         latest: Optional[Version] = None,
         message: Optional[str] = None,
         url: Optional[str] = None,
         error: Optional[Dict[str, str]] = None,
     ):
         self.name = name
         if current and latest:
-            self.current = current.base_version
-            self.latest = latest.base_version
+            self.current = str(current)
+            self.latest = str(latest)
             self.update = current < latest
-            self.breaking = (current.major - latest.major) != 0
+            self.breaking = (latest.major - current.major) > 0
         if error:
             self.error = error
         if message:
             self.message = message
         if url:
             self.url = url
```

### Comparing `slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/hooks/get_hooks.py` & `slack_cli_hooks-0.0.1/slack_cli_hooks/hooks/get_hooks.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,18 +12,20 @@
 
 
 hooks_payload = {
     "hooks": {
         "get-manifest": f"{EXEC} -m slack_cli_hooks.hooks.get_manifest",
         "start": f"{EXEC} -X dev -m slack_cli_hooks.hooks.start",
         "check-update": f"{EXEC} -m slack_cli_hooks.hooks.check_update",
+        "doctor": f"{EXEC} -m slack_cli_hooks.hooks.doctor",
     },
     "config": {
         "watch": {"filter-regex": "(^manifest\\.json$)", "paths": ["."]},
         "protocol-version": [MessageBoundaryProtocol.name, DefaultProtocol.name],
         "sdk-managed-connection-enabled": True,
     },
+    "runtime": "python",
 }
 
 if __name__ == "__main__":
     PROTOCOL = build_protocol()
     PROTOCOL.respond(json.dumps(hooks_payload))
```

### Comparing `slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/hooks/get_manifest.py` & `slack_cli_hooks-0.0.1/slack_cli_hooks/hooks/get_manifest.py`

 * *Files identical despite different names*

### Comparing `slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/protocol/__init__.py` & `slack_cli_hooks-0.0.1/slack_cli_hooks/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/protocol/default_protocol.py` & `slack_cli_hooks-0.0.1/slack_cli_hooks/protocol/default_protocol.py`

 * *Files identical despite different names*

### Comparing `slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/protocol/message_boundary_protocol.py` & `slack_cli_hooks-0.0.1/slack_cli_hooks/protocol/message_boundary_protocol.py`

 * *Files identical despite different names*

### Comparing `slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/protocol/protocol.py` & `slack_cli_hooks-0.0.1/slack_cli_hooks/protocol/protocol.py`

 * *Files identical despite different names*

### Comparing `slack_cli_hooks-0.0.0.dev2/slack_cli_hooks.egg-info/PKG-INFO` & `slack_cli_hooks-0.0.1/slack_cli_hooks.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack_cli_hooks
-Version: 0.0.0.dev2
+Version: 0.0.1
 Summary: The Slack CLI contract implementation for Bolt Python
 Author-email: "Slack Technologies, LLC" <opensource@slack.com>
 License: MIT
 Project-URL: Source Code, https://github.com/slackapi/python-slack-hooks
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -19,22 +19,25 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: slack_bolt<2,>=1.18.0
+Requires-Dist: packaging<25
 
 <h1 align="center">Python Slack Hooks</h1>
 
 <p align="center">
     <a href="https://pypi.org/project/slack-cli-hooks/">
         <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/slack-cli-hooks?style=flat-square"></a>
     <a href="https://pypi.org/project/slack-cli-hooks/">
         <img alt="Python Versions" src="https://img.shields.io/pypi/pyversions/slack-cli-hooks.svg?style=flat-square"></a>
+    <a href="https://codecov.io/gh/slackapi/python-slack-hooks">
+        <img alt="Codecov" src="https://img.shields.io/codecov/c/gh/slackapi/python-slack-hooks?style=flat-square"></a>
 </p>
 
 This library defines the contract between the
 [Slack CLI](https://api.slack.com/automation/cli/install) and
 [Bolt for Python](https://slack.dev/bolt-python/).
 
 ## Overview
@@ -53,19 +56,20 @@
 
 A Slack CLI-compatible Slack application includes a `./slack.json` file that contains hooks specific to that project. Each hook is associated with commands that are available in the Slack CLI. By default, `get-hooks` retrieves all of the [supported hooks](#supported-hooks) and their corresponding scripts as defined in this library.
 
 The CLI will always use the version of the `python-slack-hooks` that is specified in the project's `requirements.txt`.
 
 ### Supported Hooks
 
-The hooks currently supported for use within the Slack CLI include `check-update`, `get-hooks`, `get-manifest`, and `start`:
+The hooks currently supported for use within the Slack CLI include `check-update`, `doctor`, `get-hooks`, `get-manifest`, and `start`:
 
 | Hook Name  | CLI Command  | File  |  Description  |
 | --- | --- | --- | --- |
 | `check-update` | `slack update` | [check_update.py](./slack_cli_hooks/hooks/check_update.py) | Checks the project's Slack dependencies to determine whether or not any libraries need to be updated. |
+| `doctor` | `slack doctor` | [doctor.py](./slack_cli_hooks/hooks/doctor.py) | Returns runtime versions and other system dependencies required by the application. |
 | `get-hooks` | All | [get_hooks.py](./slack_cli_hooks/hooks/get_hooks.py) | Fetches the list of available hooks for the CLI from this repository. |
 | `get-manifest` | `slack manifest` | [get_manifest.py](./slack_cli_hooks/hooks/get_manifest.py) | Converts a `manifest.json` file into a valid manifest JSON payload. |
 | `start` | `slack run` | [start.py](./slack_cli_hooks/hooks/start.py) | While developing locally, the CLI manages a socket connection with Slack's backend and utilizes this hook for events received via this connection. |
 
 ### Overriding Hooks
 
 To customize the behavior of a hook, add the hook to your application's `/slack.json` file, and provide a corresponding script to be executed.
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: slack_cli_hooks Version: 0.0.0.dev2 Summary: The
-Slack CLI contract implementation for Bolt Python Author-email: "Slack
-Technologies, LLC"
+Metadata-Version: 2.1 Name: slack_cli_hooks Version: 0.0.1 Summary: The Slack
+CLI contract implementation for Bolt Python Author-email: "Slack Technologies,
+LLC"
 slack.com> License: MIT Project-URL: Source Code, https://github.com/slackapi/
 python-slack-hooks Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Environment :: Console Classifier: Intended Audience :: Developers Classifier:
 Topic :: Office/Business Classifier: Topic :: Software Development Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Programming Language ::
 Python :: Implementation :: CPython Classifier: Programming Language :: Python
 :: Implementation :: PyPy Requires-Python: >=3.9 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: slack_bolt<2,>=1.18.0
+Requires-Dist: packaging<25
                        ************ PPyytthhoonn SSllaacckk HHooookkss ************
-                       _[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]
+                  _[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_C_o_d_e_c_o_v_]
 This library defines the contract between the [Slack CLI](https://
 api.slack.com/automation/cli/install) and [Bolt for Python](https://slack.dev/
 bolt-python/). ## Overview This library enables inter-process communication
 between the [Slack CLI](https://api.slack.com/automation/cli/install) and
 applications built with Bolt for Python. When used together, the CLI delegates
 various tasks to the Bolt application by invoking processes ("hooks") and then
 making use of the responses provided by each hook's `stdout`. For a complete
@@ -27,29 +28,31 @@
 slack-bolt/) is recommended. ## Usage A Slack CLI-compatible Slack application
 includes a `./slack.json` file that contains hooks specific to that project.
 Each hook is associated with commands that are available in the Slack CLI. By
 default, `get-hooks` retrieves all of the [supported hooks](#supported-hooks)
 and their corresponding scripts as defined in this library. The CLI will always
 use the version of the `python-slack-hooks` that is specified in the project's
 `requirements.txt`. ### Supported Hooks The hooks currently supported for use
-within the Slack CLI include `check-update`, `get-hooks`, `get-manifest`, and
-`start`: | Hook Name | CLI Command | File | Description | | --- | --- | --- | -
--- | | `check-update` | `slack update` | [check_update.py](./slack_cli_hooks/
-hooks/check_update.py) | Checks the project's Slack dependencies to determine
-whether or not any libraries need to be updated. | | `get-hooks` | All |
-[get_hooks.py](./slack_cli_hooks/hooks/get_hooks.py) | Fetches the list of
-available hooks for the CLI from this repository. | | `get-manifest` | `slack
-manifest` | [get_manifest.py](./slack_cli_hooks/hooks/get_manifest.py) |
-Converts a `manifest.json` file into a valid manifest JSON payload. | | `start`
-| `slack run` | [start.py](./slack_cli_hooks/hooks/start.py) | While developing
-locally, the CLI manages a socket connection with Slack's backend and utilizes
-this hook for events received via this connection. | ### Overriding Hooks To
-customize the behavior of a hook, add the hook to your application's `/
-slack.json` file, and provide a corresponding script to be executed. When
-commands are run, the Slack CLI will look to the project's hook definitions and
-use those instead of what's defined in this library, if provided. Below is an
-example `/slack.json` file that overrides the default `start`: ```json
-{ "hooks": { "get-hooks": "python3 -m slack_cli_hooks.hooks.get_hooks",
-"start": "python3 app.py" } } ``` ## Contributing Contributions are always
-welcome! Please review the [contributing guidelines](https://github.com/
-slackapi/python-slack-hooks/blob/main/.github/CONTRIBUTING.md) for more
-information.
+within the Slack CLI include `check-update`, `doctor`, `get-hooks`, `get-
+manifest`, and `start`: | Hook Name | CLI Command | File | Description | | --
+- | --- | --- | --- | | `check-update` | `slack update` | [check_update.py](./
+slack_cli_hooks/hooks/check_update.py) | Checks the project's Slack
+dependencies to determine whether or not any libraries need to be updated. | |
+`doctor` | `slack doctor` | [doctor.py](./slack_cli_hooks/hooks/doctor.py) |
+Returns runtime versions and other system dependencies required by the
+application. | | `get-hooks` | All | [get_hooks.py](./slack_cli_hooks/hooks/
+get_hooks.py) | Fetches the list of available hooks for the CLI from this
+repository. | | `get-manifest` | `slack manifest` | [get_manifest.py](./
+slack_cli_hooks/hooks/get_manifest.py) | Converts a `manifest.json` file into a
+valid manifest JSON payload. | | `start` | `slack run` | [start.py](./
+slack_cli_hooks/hooks/start.py) | While developing locally, the CLI manages a
+socket connection with Slack's backend and utilizes this hook for events
+received via this connection. | ### Overriding Hooks To customize the behavior
+of a hook, add the hook to your application's `/slack.json` file, and provide a
+corresponding script to be executed. When commands are run, the Slack CLI will
+look to the project's hook definitions and use those instead of what's defined
+in this library, if provided. Below is an example `/slack.json` file that
+overrides the default `start`: ```json { "hooks": { "get-hooks": "python3 -
+m slack_cli_hooks.hooks.get_hooks", "start": "python3 app.py" } } ``` ##
+Contributing Contributions are always welcome! Please review the [contributing
+guidelines](https://github.com/slackapi/python-slack-hooks/blob/main/.github/
+CONTRIBUTING.md) for more information.
```

### Comparing `slack_cli_hooks-0.0.0.dev2/slack_cli_hooks.egg-info/SOURCES.txt` & `slack_cli_hooks-0.0.1/slack_cli_hooks.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 slack_cli_hooks.egg-info/SOURCES.txt
 slack_cli_hooks.egg-info/dependency_links.txt
 slack_cli_hooks.egg-info/requires.txt
 slack_cli_hooks.egg-info/top_level.txt
 slack_cli_hooks/error/__init__.py
 slack_cli_hooks/hooks/__init__.py
 slack_cli_hooks/hooks/check_update.py
+slack_cli_hooks/hooks/doctor.py
 slack_cli_hooks/hooks/get_hooks.py
 slack_cli_hooks/hooks/get_manifest.py
 slack_cli_hooks/hooks/start.py
-slack_cli_hooks/hooks/utils/__init__.py
-slack_cli_hooks/hooks/utils/managed_os_env_vars.py
 slack_cli_hooks/protocol/__init__.py
 slack_cli_hooks/protocol/default_protocol.py
 slack_cli_hooks/protocol/message_boundary_protocol.py
 slack_cli_hooks/protocol/protocol.py
```

