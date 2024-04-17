# Comparing `tmp/duckietown-shell-6.0.2.tar.gz` & `tmp/duckietown-shell-6.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckietown-shell-6.0.2.tar", last modified: Wed Mar 20 14:56:50 2024, max compression
+gzip compressed data, was "duckietown-shell-6.0.3.tar", last modified: Wed Apr 17 19:25:38 2024, max compression
```

## Comparing `duckietown-shell-6.0.2.tar` & `duckietown-shell-6.0.3.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.977597 duckietown-shell-6.0.2/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    75933 2023-03-22 21:05:31.000000 duckietown-shell-6.0.2/LICENSE.pdf
--rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      599 2024-03-20 14:56:50.977597 duckietown-shell-6.0.2/PKG-INFO
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.977597 duckietown-shell-6.0.2/duckietown_shell.egg-info/
--rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      599 2024-03-20 14:56:50.000000 duckietown-shell-6.0.2/duckietown_shell.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3347 2024-03-20 14:56:50.000000 duckietown-shell-6.0.2/duckietown_shell.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2024-03-20 14:56:50.000000 duckietown-shell-6.0.2/duckietown_shell.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       45 2024-03-20 14:56:50.000000 duckietown-shell-6.0.2/duckietown_shell.egg-info/entry_points.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2024-03-20 14:56:50.000000 duckietown-shell-6.0.2/duckietown_shell.egg-info/not-zip-safe
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      259 2024-03-20 14:56:50.000000 duckietown-shell-6.0.2/duckietown_shell.egg-info/requires.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2024-03-20 14:56:50.000000 duckietown-shell-6.0.2/duckietown_shell.egg-info/top_level.txt
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.965597 duckietown-shell-6.0.2/lib/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.969597 duckietown-shell-6.0.2/lib/dt_shell/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1143 2024-03-20 14:56:46.000000 duckietown-shell-6.0.2/lib/dt_shell/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.969597 duckietown-shell-6.0.2/lib/dt_shell/assets/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      145 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/assets/dts-completion.bash
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)  2605506 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/assets/get-pip.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      241 2024-03-20 14:56:50.000000 duckietown-shell-6.0.2/lib/dt_shell/assets/requirements.txt
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.969597 duckietown-shell-6.0.2/lib/dt_shell/checks/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/checks/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2731 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/checks/environment.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2431 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/checks/packages.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4081 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/checks/version.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.973597 duckietown-shell-6.0.2/lib/dt_shell/commands/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      314 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/commands/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1744 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/commands/autocomplete.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    22097 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/commands/commands.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6891 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/commands/importer.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3832 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/commands/repository.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.973597 duckietown-shell-6.0.2/lib/dt_shell/compatibility/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1703 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/compatibility/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      253 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/compatibility/commands_.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1394 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/compatibility/config.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      120 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/compatibility/duckietown_tokens.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      753 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/compatibility/env_checks.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.973597 duckietown-shell-6.0.2/lib/dt_shell/compatibility/migrations/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       26 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/compatibility/migrations/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4545 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/compatibility/migrations/migrations.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      820 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/compatibility/tokens_cli.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      179 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/compatibility/version_check.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3559 2024-03-20 14:43:29.000000 duckietown-shell-6.0.2/lib/dt_shell/constants.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.973597 duckietown-shell-6.0.2/lib/dt_shell/database/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/database/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7316 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/database/database.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2046 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/database/utils.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.965597 duckietown-shell-6.0.2/lib/dt_shell/embedded/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.973597 duckietown-shell-6.0.2/lib/dt_shell/embedded/__command_set__/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1241 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/__command_set__/configuration.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       21 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/__command_set__/init.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/__command_set__/requirements.txt
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.973597 duckietown-shell-6.0.2/lib/dt_shell/embedded/commands/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      519 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/commands/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      875 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/commands/command.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.973597 duckietown-shell-6.0.2/lib/dt_shell/embedded/exit/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/exit/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      211 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/exit/command.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      553 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/exit/configuration.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.973597 duckietown-shell-6.0.2/lib/dt_shell/embedded/install/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/install/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      387 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/install/command.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.973597 duckietown-shell-6.0.2/lib/dt_shell/embedded/profile/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/profile/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.973597 duckietown-shell-6.0.2/lib/dt_shell/embedded/profile/dependencies/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/profile/dependencies/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.973597 duckietown-shell-6.0.2/lib/dt_shell/embedded/profile/dependencies/reinstall/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/profile/dependencies/reinstall/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1027 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/profile/dependencies/reinstall/command.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      336 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/profile/dependencies/reinstall/configuration.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.973597 duckietown-shell-6.0.2/lib/dt_shell/embedded/profile/list/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/profile/list/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1492 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/profile/list/command.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      431 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/profile/list/configuration.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.973597 duckietown-shell-6.0.2/lib/dt_shell/embedded/profile/new/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/profile/new/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3331 2024-03-20 14:43:29.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/profile/new/command.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      639 2024-03-20 14:43:29.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/profile/new/configuration.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.973597 duckietown-shell-6.0.2/lib/dt_shell/embedded/profile/switch/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/profile/switch/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2207 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/profile/switch/command.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      532 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/profile/switch/configuration.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.973597 duckietown-shell-6.0.2/lib/dt_shell/embedded/tok/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/tok/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      218 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/tok/configuration.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.973597 duckietown-shell-6.0.2/lib/dt_shell/embedded/tok/set/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/tok/set/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2006 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/tok/set/command.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.973597 duckietown-shell-6.0.2/lib/dt_shell/embedded/tok/status/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/tok/status/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      409 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/tok/status/command.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.973597 duckietown-shell-6.0.2/lib/dt_shell/embedded/tok/verify/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/tok/verify/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1028 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/tok/verify/command.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.973597 duckietown-shell-6.0.2/lib/dt_shell/embedded/uninstall/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/uninstall/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      383 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/uninstall/command.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.977597 duckietown-shell-6.0.2/lib/dt_shell/embedded/update/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/update/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      393 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/update/command.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.977597 duckietown-shell-6.0.2/lib/dt_shell/embedded/version/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       69 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/version/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1174 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/embedded/version/command.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7557 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/environments.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2662 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/exceptions.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2487 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/hub.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1756 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/logging.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    17337 2024-03-20 14:43:29.000000 duckietown-shell-6.0.2/lib/dt_shell/profile.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    34612 2024-03-20 14:43:29.000000 duckietown-shell-6.0.2/lib/dt_shell/shell.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1976 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/statistics.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6765 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/tasks.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      194 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell/typing.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    10749 2024-03-20 14:56:28.000000 duckietown-shell-6.0.2/lib/dt_shell/utils.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-20 14:56:50.977597 duckietown-shell-6.0.2/lib/dt_shell_cli/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      218 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell_cli/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     8501 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell_cli/dts.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1971 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/lib/dt_shell_cli/main.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2024-03-20 14:56:50.977597 duckietown-shell-6.0.2/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3017 2024-03-13 05:31:54.000000 duckietown-shell-6.0.2/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.814544 duckietown-shell-6.0.3/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    75933 2023-03-22 21:05:31.000000 duckietown-shell-6.0.3/LICENSE.pdf
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      599 2024-04-17 19:25:38.814544 duckietown-shell-6.0.3/PKG-INFO
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.814544 duckietown-shell-6.0.3/duckietown_shell.egg-info/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      599 2024-04-17 19:25:38.000000 duckietown-shell-6.0.3/duckietown_shell.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3347 2024-04-17 19:25:38.000000 duckietown-shell-6.0.3/duckietown_shell.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2024-04-17 19:25:38.000000 duckietown-shell-6.0.3/duckietown_shell.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       45 2024-04-17 19:25:38.000000 duckietown-shell-6.0.3/duckietown_shell.egg-info/entry_points.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2024-03-20 14:56:50.000000 duckietown-shell-6.0.3/duckietown_shell.egg-info/not-zip-safe
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      259 2024-04-17 19:25:38.000000 duckietown-shell-6.0.3/duckietown_shell.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2024-04-17 19:25:38.000000 duckietown-shell-6.0.3/duckietown_shell.egg-info/top_level.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.806544 duckietown-shell-6.0.3/lib/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.806544 duckietown-shell-6.0.3/lib/dt_shell/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1143 2024-04-17 19:25:31.000000 duckietown-shell-6.0.3/lib/dt_shell/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.806544 duckietown-shell-6.0.3/lib/dt_shell/assets/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      145 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/assets/dts-completion.bash
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)  2605506 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/assets/get-pip.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      241 2024-04-17 19:25:38.000000 duckietown-shell-6.0.3/lib/dt_shell/assets/requirements.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.810544 duckietown-shell-6.0.3/lib/dt_shell/checks/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/checks/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2731 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/checks/environment.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2431 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/checks/packages.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4081 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/checks/version.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.810544 duckietown-shell-6.0.3/lib/dt_shell/commands/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      314 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/commands/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1744 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/commands/autocomplete.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    22097 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/commands/commands.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6891 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/commands/importer.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3832 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/commands/repository.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.810544 duckietown-shell-6.0.3/lib/dt_shell/compatibility/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1703 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/compatibility/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      253 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/compatibility/commands_.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1394 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/compatibility/config.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      120 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/compatibility/duckietown_tokens.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      753 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/compatibility/env_checks.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.810544 duckietown-shell-6.0.3/lib/dt_shell/compatibility/migrations/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       26 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/compatibility/migrations/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4545 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/compatibility/migrations/migrations.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      820 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/compatibility/tokens_cli.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      179 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/compatibility/version_check.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3559 2024-03-20 14:43:29.000000 duckietown-shell-6.0.3/lib/dt_shell/constants.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.810544 duckietown-shell-6.0.3/lib/dt_shell/database/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/database/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7316 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/database/database.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2046 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/database/utils.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.806544 duckietown-shell-6.0.3/lib/dt_shell/embedded/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.810544 duckietown-shell-6.0.3/lib/dt_shell/embedded/__command_set__/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1241 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/__command_set__/configuration.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       21 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/__command_set__/init.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/__command_set__/requirements.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.810544 duckietown-shell-6.0.3/lib/dt_shell/embedded/commands/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      519 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/commands/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      875 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/commands/command.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.810544 duckietown-shell-6.0.3/lib/dt_shell/embedded/exit/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/exit/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      211 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/exit/command.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      553 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/exit/configuration.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.810544 duckietown-shell-6.0.3/lib/dt_shell/embedded/install/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/install/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      387 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/install/command.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.810544 duckietown-shell-6.0.3/lib/dt_shell/embedded/profile/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/profile/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.810544 duckietown-shell-6.0.3/lib/dt_shell/embedded/profile/dependencies/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/profile/dependencies/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.810544 duckietown-shell-6.0.3/lib/dt_shell/embedded/profile/dependencies/reinstall/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/profile/dependencies/reinstall/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1027 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/profile/dependencies/reinstall/command.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      336 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/profile/dependencies/reinstall/configuration.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.810544 duckietown-shell-6.0.3/lib/dt_shell/embedded/profile/list/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/profile/list/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1492 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/profile/list/command.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      431 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/profile/list/configuration.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.810544 duckietown-shell-6.0.3/lib/dt_shell/embedded/profile/new/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/profile/new/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3331 2024-03-20 14:43:29.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/profile/new/command.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      639 2024-03-20 14:43:29.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/profile/new/configuration.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.810544 duckietown-shell-6.0.3/lib/dt_shell/embedded/profile/switch/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/profile/switch/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2207 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/profile/switch/command.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      532 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/profile/switch/configuration.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.810544 duckietown-shell-6.0.3/lib/dt_shell/embedded/tok/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/tok/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      218 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/tok/configuration.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.810544 duckietown-shell-6.0.3/lib/dt_shell/embedded/tok/set/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/tok/set/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2006 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/tok/set/command.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.810544 duckietown-shell-6.0.3/lib/dt_shell/embedded/tok/status/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/tok/status/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      409 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/tok/status/command.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.814544 duckietown-shell-6.0.3/lib/dt_shell/embedded/tok/verify/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/tok/verify/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1028 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/tok/verify/command.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.814544 duckietown-shell-6.0.3/lib/dt_shell/embedded/uninstall/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/uninstall/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      383 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/uninstall/command.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.814544 duckietown-shell-6.0.3/lib/dt_shell/embedded/update/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/update/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      393 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/update/command.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.814544 duckietown-shell-6.0.3/lib/dt_shell/embedded/version/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       69 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/version/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1174 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/embedded/version/command.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7557 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/environments.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2662 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/exceptions.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2487 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/hub.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1756 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/logging.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    17337 2024-03-20 14:43:29.000000 duckietown-shell-6.0.3/lib/dt_shell/profile.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    34688 2024-04-17 19:24:14.000000 duckietown-shell-6.0.3/lib/dt_shell/shell.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1976 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/statistics.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6765 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/tasks.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      194 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell/typing.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    10749 2024-03-20 14:56:28.000000 duckietown-shell-6.0.3/lib/dt_shell/utils.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-17 19:25:38.814544 duckietown-shell-6.0.3/lib/dt_shell_cli/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      218 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell_cli/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     8501 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell_cli/dts.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1971 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/lib/dt_shell_cli/main.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2024-04-17 19:25:38.814544 duckietown-shell-6.0.3/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3017 2024-03-13 05:31:54.000000 duckietown-shell-6.0.3/setup.py
```

### Comparing `duckietown-shell-6.0.2/LICENSE.pdf` & `duckietown-shell-6.0.3/LICENSE.pdf`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/PKG-INFO` & `duckietown-shell-6.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: duckietown-shell
-Version: 6.0.2
-Download-URL: http://github.com/duckietown/duckietown-shell/tarball/6.0.2
+Version: 6.0.3
+Download-URL: http://github.com/duckietown/duckietown-shell/tarball/6.0.3
 License-File: LICENSE.pdf
 Requires-Dist: termcolor<3,>=2.3.0
 Requires-Dist: requests<3,>=2.31.0
 Requires-Dist: pyyaml!=5.4.0,!=5.4.1,!=6.0.0,<7
 Requires-Dist: pyfiglet<1,>=0.8.0
 Requires-Dist: questionary<3,>=2.0.1
 Requires-Dist: argcomplete<4,>=3.1.4
```

### Comparing `duckietown-shell-6.0.2/duckietown_shell.egg-info/PKG-INFO` & `duckietown-shell-6.0.3/duckietown_shell.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: duckietown-shell
-Version: 6.0.2
-Download-URL: http://github.com/duckietown/duckietown-shell/tarball/6.0.2
+Version: 6.0.3
+Download-URL: http://github.com/duckietown/duckietown-shell/tarball/6.0.3
 License-File: LICENSE.pdf
 Requires-Dist: termcolor<3,>=2.3.0
 Requires-Dist: requests<3,>=2.31.0
 Requires-Dist: pyyaml!=5.4.0,!=5.4.1,!=6.0.0,<7
 Requires-Dist: pyfiglet<1,>=0.8.0
 Requires-Dist: questionary<3,>=2.0.1
 Requires-Dist: argcomplete<4,>=3.1.4
```

### Comparing `duckietown-shell-6.0.2/duckietown_shell.egg-info/SOURCES.txt` & `duckietown-shell-6.0.3/duckietown_shell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/__init__.py` & `duckietown-shell-6.0.3/lib/dt_shell/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from dt_shell_cli import logger
 
 # logger dedicated to the commands
 dtslogger = logging.getLogger("dts")
 dtslogger.setLevel(logging.INFO)
 
-__version__ = "6.0.2"
+__version__ = "6.0.3"
 
 import sys
 
 if sys.version_info < (3, 6):
     msg = f"! duckietown-shell works with Python 3.6 and later !.\nDetected {sys.version}."
     logger.error(msg)
     sys.exit(2)
```

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/assets/get-pip.py` & `duckietown-shell-6.0.3/lib/dt_shell/assets/get-pip.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/checks/environment.py` & `duckietown-shell-6.0.3/lib/dt_shell/checks/environment.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/checks/packages.py` & `duckietown-shell-6.0.3/lib/dt_shell/checks/packages.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/checks/version.py` & `duckietown-shell-6.0.3/lib/dt_shell/checks/version.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/commands/autocomplete.py` & `duckietown-shell-6.0.3/lib/dt_shell/commands/autocomplete.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/commands/commands.py` & `duckietown-shell-6.0.3/lib/dt_shell/commands/commands.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/commands/importer.py` & `duckietown-shell-6.0.3/lib/dt_shell/commands/importer.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/commands/repository.py` & `duckietown-shell-6.0.3/lib/dt_shell/commands/repository.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/compatibility/__init__.py` & `duckietown-shell-6.0.3/lib/dt_shell/compatibility/__init__.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/compatibility/config.py` & `duckietown-shell-6.0.3/lib/dt_shell/compatibility/config.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/compatibility/env_checks.py` & `duckietown-shell-6.0.3/lib/dt_shell/compatibility/env_checks.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/compatibility/migrations/migrations.py` & `duckietown-shell-6.0.3/lib/dt_shell/compatibility/migrations/migrations.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/compatibility/tokens_cli.py` & `duckietown-shell-6.0.3/lib/dt_shell/compatibility/tokens_cli.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/constants.py` & `duckietown-shell-6.0.3/lib/dt_shell/constants.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/database/database.py` & `duckietown-shell-6.0.3/lib/dt_shell/database/database.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/database/utils.py` & `duckietown-shell-6.0.3/lib/dt_shell/database/utils.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/embedded/__command_set__/configuration.py` & `duckietown-shell-6.0.3/lib/dt_shell/embedded/__command_set__/configuration.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/embedded/commands/__init__.py` & `duckietown-shell-6.0.3/lib/dt_shell/embedded/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/embedded/commands/command.py` & `duckietown-shell-6.0.3/lib/dt_shell/embedded/commands/command.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/embedded/exit/configuration.py` & `duckietown-shell-6.0.3/lib/dt_shell/embedded/exit/configuration.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/embedded/profile/dependencies/reinstall/command.py` & `duckietown-shell-6.0.3/lib/dt_shell/embedded/profile/dependencies/reinstall/command.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/embedded/profile/list/command.py` & `duckietown-shell-6.0.3/lib/dt_shell/embedded/profile/list/command.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/embedded/profile/new/command.py` & `duckietown-shell-6.0.3/lib/dt_shell/embedded/profile/new/command.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/embedded/profile/new/configuration.py` & `duckietown-shell-6.0.3/lib/dt_shell/embedded/profile/new/configuration.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/embedded/profile/switch/command.py` & `duckietown-shell-6.0.3/lib/dt_shell/embedded/profile/switch/command.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/embedded/profile/switch/configuration.py` & `duckietown-shell-6.0.3/lib/dt_shell/embedded/profile/switch/configuration.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/embedded/tok/set/command.py` & `duckietown-shell-6.0.3/lib/dt_shell/embedded/tok/set/command.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/embedded/tok/verify/command.py` & `duckietown-shell-6.0.3/lib/dt_shell/embedded/tok/verify/command.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/embedded/version/command.py` & `duckietown-shell-6.0.3/lib/dt_shell/embedded/version/command.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/environments.py` & `duckietown-shell-6.0.3/lib/dt_shell/environments.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/exceptions.py` & `duckietown-shell-6.0.3/lib/dt_shell/exceptions.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/hub.py` & `duckietown-shell-6.0.3/lib/dt_shell/hub.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/logging.py` & `duckietown-shell-6.0.3/lib/dt_shell/logging.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/profile.py` & `duckietown-shell-6.0.3/lib/dt_shell/profile.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/shell.py` & `duckietown-shell-6.0.3/lib/dt_shell/shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 @dataclass
 class CLIOptions:
     debug: bool = env_option("DTSHELL_DEBUG", False)
     verbose: bool = env_option("DTSHELL_VERBOSE", False)
     quiet: bool = env_option("DTSHELL_QUIET", False)
     complete: bool = False
-    profile: Optional[str] = None
+    profile: Optional[str] = env_option("DTSHELL_PROFILE", None)
 
 
 def get_cli_options(args: List[str]) -> Tuple[CLIOptions, List[str]]:
     """Returns cli options plus other arguments for the commands."""
     default_opts: CLIOptions = CLIOptions()
 
     if args and not args[0].startswith("-"):
@@ -96,15 +96,15 @@
         action="store_true",
         default=default_opts.quiet,
         help="Quiet execution"
     )
     parser.add_argument(
         "--profile",
         type=str,
-        default=None,
+        default=default_opts.profile,
         help="Select specific profile just for this session"
     )
 
     if "--complete" in args[:i]:
         parser.add_argument(
             "--complete",
             action="store_true",
@@ -232,15 +232,15 @@
         self._db_profiles: DTShellDatabase = DTShellDatabase.open(DB_PROFILES, readonly=readonly)
         self._db_settings: ShellSettings = ShellSettings.open(DB_SETTINGS, readonly=readonly)
 
         # custom profile
         if profile is not None:
             if profile not in self._db_profiles.keys():
                 raise UserError(f"The profile '{profile}' does not exist.")
-            logger.info(f"Using profile '{profile}' as prescribed by the option --profile")
+            logger.info(f"Using profile '{profile}' as prescribed by --profile or environment variable DTSHELL_PROFILE")
             with self.settings.in_memory():
                 self.settings.profile = profile
 
         # load current profile
         self._profile: ShellProfile = ShellProfile(self.settings.profile, readonly=readonly) \
             if self.settings.profile else None
```

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/statistics.py` & `duckietown-shell-6.0.3/lib/dt_shell/statistics.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/tasks.py` & `duckietown-shell-6.0.3/lib/dt_shell/tasks.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell/utils.py` & `duckietown-shell-6.0.3/lib/dt_shell/utils.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell_cli/dts.py` & `duckietown-shell-6.0.3/lib/dt_shell_cli/dts.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/lib/dt_shell_cli/main.py` & `duckietown-shell-6.0.3/lib/dt_shell_cli/main.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.2/setup.py` & `duckietown-shell-6.0.3/setup.py`

 * *Files identical despite different names*

