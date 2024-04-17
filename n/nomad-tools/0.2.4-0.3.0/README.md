# Comparing `tmp/nomad-tools-0.2.4.tar.gz` & `tmp/nomad_tools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomad-tools-0.2.4.tar", last modified: Tue Feb 13 19:45:46 2024, max compression
+gzip compressed data, was "nomad_tools-0.3.0.tar", last modified: Wed Apr 17 20:35:21 2024, max compression
```

## Comparing `nomad-tools-0.2.4.tar` & `nomad_tools-0.3.0.tar`

### file list

```diff
@@ -1,49 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 19:45:46.707852 nomad-tools-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35083 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9938 2024-02-13 19:45:46.707852 nomad-tools-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9101 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 19:45:46.707852 nomad-tools-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 19:45:46.699852 nomad-tools-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 19:45:46.703852 nomad-tools-0.2.4/src/nomad_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/common_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/common_click.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/common_nomad.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/exit_on_thread_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/flagdebug.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23256 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/nomad_cp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/nomad_dockers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/nomad_downloadrelease.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 19:45:46.703852 nomad-tools-0.2.4/src/nomad_tools/nomad_gitlab_runner/
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/nomad_gitlab_runner/script.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1789 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/nomad_gitlab_runner/waiter.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)    28355 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/nomad_gitlab_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/nomad_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/nomad_smart_start_job.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18558 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/nomad_vardir.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    66425 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/nomad_watch.py
--rw-r--r--   0 runner    (1001) docker     (127)    15304 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/nomaddbjob.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 19:45:46.703852 nomad-tools-0.2.4/src/nomad_tools/nomadlib/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/nomadlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/nomadlib/_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8126 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/nomadlib/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/nomadlib/datadict.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/nomadlib/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    19575 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/nomadlib/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/nomadt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/nomadt_completion.sh
--rw-r--r--   0 runner    (1001) docker     (127)    14021 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/src/nomad_tools/taskexec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 19:45:46.703852 nomad-tools-0.2.4/src/nomad_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9938 2024-02-13 19:45:46.000000 nomad-tools-0.2.4/src/nomad_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-02-13 19:45:46.000000 nomad-tools-0.2.4/src/nomad_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 19:45:46.000000 nomad-tools-0.2.4/src/nomad_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-02-13 19:45:46.000000 nomad-tools-0.2.4/src/nomad_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-13 19:45:46.000000 nomad-tools-0.2.4/src/nomad_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-13 19:45:46.000000 nomad-tools-0.2.4/src/nomad_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 19:45:46.703852 nomad-tools-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8118 2024-02-13 19:45:39.000000 nomad-tools-0.2.4/tests/testlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:35:21.747339 nomad_tools-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35083 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11774 2024-04-17 20:35:21.747339 nomad_tools-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10759 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 20:35:21.747339 nomad_tools-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:35:21.735339 nomad_tools-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:35:21.743339 nomad_tools-0.3.0/src/nomad_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/common_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/common_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/common_nomad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/entry_constrainteval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21243 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/entry_go.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/exit_on_thread_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/flagdebug.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28872 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomad_cp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomad_dockers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomad_downloadrelease.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:35:21.743339 nomad_tools-0.3.0/src/nomad_tools/nomad_gitlab_runner/
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomad_gitlab_runner/script.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1789 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomad_gitlab_runner/waiter.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28600 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomad_gitlab_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomad_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomad_smart_start_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomad_taskexec.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18624 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomad_vardir.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    77612 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomad_watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15126 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomaddbjob.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:35:21.743339 nomad_tools-0.3.0/src/nomad_tools/nomadlib/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomadlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomadlib/_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomadlib/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomadlib/datadict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomadlib/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19655 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomadlib/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/nomadt_completion.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    16619 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/taskexec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/src/nomad_tools/transferstats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:35:21.743339 nomad_tools-0.3.0/src/nomad_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11774 2024-04-17 20:35:21.000000 nomad_tools-0.3.0/src/nomad_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-17 20:35:21.000000 nomad_tools-0.3.0/src/nomad_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:35:21.000000 nomad_tools-0.3.0/src/nomad_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-17 20:35:21.000000 nomad_tools-0.3.0/src/nomad_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-17 20:35:21.000000 nomad_tools-0.3.0/src/nomad_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 20:35:21.000000 nomad_tools-0.3.0/src/nomad_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:35:21.743339 nomad_tools-0.3.0/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      561 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/tests/test_nomad_cp_complete.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3302 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/tests/test_taskexec_transfer_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7999 2024-04-17 20:35:14.000000 nomad_tools-0.3.0/tests/testlib.py
```

### Comparing `nomad-tools-0.2.4/LICENSE` & `nomad_tools-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nomad-tools-0.2.4/PKG-INFO` & `nomad_tools-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,28 @@
-Metadata-Version: 2.1
-Name: nomad-tools
-Version: 0.2.4
-Summary: Set of tools and utilities to ease interacting with Hashicorp Nomad scheduling solution.
-Author: Kamil Cukrowski
-License: GPL-3.0-or-later
-Project-URL: homepage, https://github.com/Kamilcuk/nomad-tools
-Project-URL: repository, https://github.com/Kamilcuk/nomad-tools
-Project-URL: documentation, https://github.com/Kamilcuk/nomad-tools
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: click
-Requires-Dist: requests
-Requires-Dist: setuptools
-Requires-Dist: pyyaml
-Requires-Dist: python-dateutil
-Requires-Dist: typing-extensions
-Requires-Dist: websocket-client
-Provides-Extra: test
-Requires-Dist: tomli; extra == "test"
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-xdist; extra == "test"
-Requires-Dist: pytest-cov; extra == "test"
-
-# nomad-tools
+# nomadtools
 
 Set of tools and utilities to ease interacting with HashiCorp Nomad scheduling solution.
 
 ## Table of Contents
 
 <!-- vim-markdown-toc GFM -->
 
 * [Installation](#installation)
     * [Shell completion](#shell-completion)
 * [Usage](#usage)
-    * [nomadt](#nomadt)
-    * [nomad-watch](#nomad-watch)
-    * [nomad-port](#nomad-port)
-    * [nomad-vardir](#nomad-vardir)
-    * [nomad-cp](#nomad-cp)
-    * [nomad-gitlab-runner](#nomad-gitlab-runner)
+    * [watch](#watch)
+    * [go](#go)
+    * [port](#port)
+    * [vardir](#vardir)
+    * [cp](#cp)
+    * [gitlab-runner](#gitlab-runner)
     * [nomad-dockers](#nomad-dockers)
-    * [nomad-downloadrelease](#nomad-downloadrelease)
+    * [downloadrelease](#downloadrelease)
     * [import nomad_tools](#import-nomad_tools)
+* [History](#history)
 * [Contributing](#contributing)
     * [Running tests](#running-tests)
 * [License](#license)
 
 <!-- vim-markdown-toc -->
 
 # Installation
@@ -53,210 +30,245 @@
 This is a bundle of executables packages together in a PyPY package. Install
 using `pipx` project.
 
 ```
 pipx install nomad-tools
 ```
 
+After installation the executable `nomadtools` should be available.
+
+```
+nomadtools --help
+```
+
 ## Shell completion
 
-After installation, see `nomad-watch --autocomplete-info` for shell
+After installation, see `nomadtools watch --autocomplete-info` for shell
 completion installation instruction.
 
 # Usage
 
-This module install several command line tools:
-
-## nomadt
-
-`nomadt` is a wrapper around `nomad` commands and `nomad-anything`
-command. If a `nomad` sub-command exists, `nomad` will be run. Otherwise
-an executable `nomad-subcommand` will be executed for a given sub-command.
-
-The intention is that you can do `alias nomad=nomadt` and use it seamlessly.
+This module installs command line tool `nomadtools` with several modes of
+operation:
 
-```
-nomadt job run example.nomad.hcl    # will execute nomad job run example.nomad.hcl
-nomadt watch run example.nomad.hcl  # will execute nomad-watch run example.nomad.hcl
-```
+## watch
 
-## nomad-watch
-
-Nomad-watch is meant to watch over a job change that you type in
+`nomadtools watch` is meant to watch over a job change that you type in
 terminal. It prints all relevant messages - messages about allocation,
 evaluation, deployment and stdout and stderr logs from all the
 processes. Depending on the mode of operation, the tool waits until an
 action is finished.
 
-I primarily use nomad-watch to deploy new versions of services. I was always
+I primarily use `watch` to deploy new versions of services. I was always
 frustrated that I start something from terminal and then I have to check the
 logs of the service in multiple tabs in the Nomad web interface. For example,
-you can use `nomad-watch start ./postgres.nomad.hcl` to update postgres
+you can use `watch start ./postgres.nomad.hcl` to update PostgreSQL
 container and watch it's logs in your terminal.
 
 An example terminal session deploying a HTTP server job with canary and health
 check. Note that while the new version is deployed, the old one still prints
 the logs.
 
-![gif showing example usage of nomad-watch start](./assets/imgs/nomad-watch-start-listen.gif)
+![gif showing example usage of watch start](./assets/imgs/nomad-watch-start-listen.gif)
 
 Another usage of the job is to run an one-shot batch jobs to do something and
 wait until they are finished and collect the exit status and logs, for example
 as an airflow or cron job. In this case `run` mode will wait for the job to be
-finished. For example `nomad-watch --purge run ./compute.nomad.hcl` will run
+finished. For example `watch --purge run ./compute.nomad.hcl` will run
 a calculation job, purge after it is done and exit with calculate job exit
 status (if there is one task).
 
-![gif showing example usage of nomad-watch run](./assets/imgs/nomad-watch-run-compute.gif)
+![gif showing example usage of watch run](./assets/imgs/nomad-watch-run-compute.gif)
+
+Internally, watch uses Nomad event stream to get the events in real time.
 
-Internally, nomad-watch uses Nomad event stream to get the events in real time.
+## go
 
-## nomad-port
+Mimics operation of `docker run`, it is built on top of `watch` mode to
+execute a single Nomad job created dynamically from command line arguments.
+It creates a Nomad job specification from command line arguments and then
+"watches" over the execution of the job.
+
+```
+$ nomadtools go --rm alpine apk add bash
+INFO:nomad_tools.nomad_watch:Watching job nomad_tools_go_5305da8f-b376-4c35-9a05-71027aadd587@default until it is finished
+Allocation 70c4ac9d-0e03-53d7-6e34-9c86cf8ee768 started on leonidas
+Received Task received by client
+Task Setup Building Task Directory
+Driver Downloading image
+Started Task started by client
+INFO:nomad_tools.nomad_watch:Job nomad_tools_go_5305da8f-b376-4c35-9a05-71027aadd587#0@default started allocations 70c4ac running group 'nomad_tools_go_5305da8f-b376-4c35-9a05-71027aadd587' with 1 main tasks.
+fetch https://dl-cdn.alpinelinux.org/alpine/v3.19/main/x86_64/APKINDEX.tar.gz
+fetch https://dl-cdn.alpinelinux.org/alpine/v3.19/community/x86_64/APKINDEX.tar.gz
+(1/4) Installing ncurses-terminfo-base (6.4_p20231125-r0)
+(2/4) Installing libncursesw (6.4_p20231125-r0)
+(3/4) Installing readline (8.2.1-r2)
+(4/4) Installing bash (5.2.21-r0)
+Terminated Exit Code: 0
+Allocation 70c4ac9d-0e03-53d7-6e34-9c86cf8ee768 finished
+Executing bash-5.2.21-r0.post-install
+Executing busybox-1.36.1-r15.trigger
+OK: 10 MiB in 19 packages
+INFO:nomad_tools.nomad_watch:Purging job nomad_tools_go_5305da8f-b376-4c35-9a05-71027aadd587
+INFO:nomad_tools.nomad_watch:Job nomad_tools_go_5305da8f-b376-4c35-9a05-71027aadd587#0@default purged with no active allocations, evaluations nor deployments. Exiting.
+INFO:nomad_tools.nomad_watch:Single task exited with 0 exit status. Exit code is 0.
+```
+
+## port
 
 Prints out the ports allocated for a particular Nomad job or
 allocation. It is meant to mimic `docker port` command.
 
 ```
-$ nomad-port httpd
+$ nomadtools port httpd
 192.168.0.5:31076
-$ nomad-port -l httpd
+$ nomadtools port -l httpd
 192.168.0.5 31076 http httpd.listen[0] d409e855-bf13-a342-fe7a-6fb579d2de85
-$ nomad-port --alloc d409e855
+$ nomadtools port --alloc d409e855
 192.168.0.5:31076
 ```
 
 Further argument allows to filter for port label.
 
 ```
-$ nomad-port httpd http
+$ nomadtools port httpd http
 192.168.0.5:31076
 ```
 
-## nomad-vardir
+## vardir
 
 I was frustrated with how Nomad variables look like. It is really hard to
 incrementally modify Nomad variables. The API is at one go. You either update
 all variables or nothing. Most often I wanted to update a single key
 from a Nomad variable at a time and the variable value was usually a file content.
 
 Example execution of putting a `passwordfile.txt` into `nomad/jobs/nginx`
 Nomad variable:
 
 ```
-$ nomad-vardir -j nginx put ./passwordfile.txt 
+$ nomadtools vardir -j nginx put ./passwordfile.txt 
 nomad_vardir: Putting var nomad/jobs/nginx@default with keys: passwordfile.txt
-$ nomad-vardir -j nginx cat passwordfile.txt 
+$ nomadtools vardir -j nginx cat passwordfile.txt 
 secretpassword
-$ nomad-vardir -j nginx ls
+$ nomadtools vardir -j nginx ls
 nomad_vardir: Listing Nomad variable at nomad/jobs/nginx@default
 key              size
 passwordfile.txt 15
 ```
 
 You can then remove the `passwordfile.txt` key from the Nomad variable:
 
 ```
-$ nomad-vardir -j nginx rm passwordfile.txt 
+$ nomadtools vardir -j nginx rm passwordfile.txt 
 nomad_vardir: Removing passwordfile.txt
 nomad_vardir: Removing empty var nomad/jobs/nginx@default
-$ nomad-vardir -j nginx ls
+$ nomadtools vardir -j nginx ls
 nomad_vardir: Nomad variable not found at nomad/jobs/nginx@default
 ```
 
-## nomad-cp
+## cp
 
 This is a copy of the `docker cp` command. The syntax is meant to be the
 same with docker. The rules of copying a file vs directory are meant to be
 in-line with `docker cp` documentation.
 
-`nomad-cp` uses some special syntax for specifying from which allocation/task
+`nomadtools cp` uses some special syntax for specifying from which allocation/task
 exactly do you want to copy by using colon `:`. The number of colons in the
 arguments determines the format. The colon can be escaped with slash `\` in
 the path if needed.
 
 Both `SRC` and `DST` addresses can be specified as follows:
 
 ```
+# Search a task matching specific URL query:
+task://JOB[@NAMESPACE]/PATH[?group=GROUP][&alloc=ALLOC][&task=TASK][&hostname=HOSTNAME][&node=NODE]
+# or
 :ALLOCATION:PATH                  copy path from this allocation having one job
-:ALLOCATION:TASK:PATH             copy path from this task inside allocation
+:ALLOCATION::TASK:PATH            copy path from this task inside allocation
 :ALLOCATION:GROUP:TASK:PATH       like above, but filter by group name
 JOB:PATH                          copy path from one task inside specified job
-JOB:TASK:PATH                     copy path from the task inside this job
+JOB::TASK:PATH                    copy path from the task inside this job
 JOB:GROUP:TASK:PATH               like above, but filter also by group name
 PATH                              copy local path
 -                                 copy stdin or stdout TAR stream
 ```
 
-`nomad-cp` depends on `sh` and `tar` command line utility to be available
+`cp` depends on `sh` and `tar` command line utility to be available
 inside the allocation it is coping to/from. It has to be available there.
 
 Example:
 
 ```
-$ nomad-cp -v nginx:/etc/nginx/nginx.conf ./nginx.conf
+$ nomadtools cp -v nginx:/etc/nginx/nginx.conf ./nginx.conf
 INFO nomad_cp.py:copy_mode:487: File :d409e855-bf13-a342-fe7a-6fb579d2de85:listen:/etc/nginx/nginx.conf -> ./nginx.conf
-$ nomad-cp -v alpine:/etc/. ./etc/
+$ nomadtools cp -v alpine:/etc/. ./etc/
 INFO nomad_cp.py:copy_mode:512: New mkdir :d409e855-bf13-a342-fe7a-6fb579d2de85:listen:/etc/. -> /home/kamil/tmp/etc2/
 ```
 
 Nomad does not have the capability of accessing any file inside the
 allocation file system. Instead, `nomad-cp` executes several `nomad exec`
 calls to execute a `tar` pipe to stream the data from or to the allocation
 context to or from the local host using stdout and stdin forwarded by
 `nomad exec`.
 
-## nomad-gitlab-runner
+## gitlab-runner
 
 An implementation of custom Gitlab executor driver that runs Gitlab CI/CD jobs
 using Nomad.
 
 This program does _not_ run the `gitlab-runner` itself in Nomad. Rather, the
 `gitlab-runner` is running on (any) one host. That `gitlab-runner` will then
 schedule Nomad jobs to execute using the script as an executor. These jobs will
 execute the CI/CD from Gitlab inside Nomad cluster.
 
-More on it can be read on [github wiki](https://github.com/Kamilcuk/nomad-tools/wiki/nomad%E2%80%90gitlab%E2%80%90runner).
+More on it can be read on [github wiki](https://github.com/Kamilcuk/nomadtools/wiki/gitlab%E2%80%90runner).
 
 ## nomad-dockers
 
 Lists docker images referenced in Nomad job file or a running Nomad job.
 
 ```
-$ nomad-dockers ./httpd.nomad.hcl
+$ nomadtools dockers ./httpd.nomad.hcl
 busybox:stable
-$ nomad-dockers --job httpd
+$ nomadtools dockers --job httpd
 busybox:stable
 ```
 
-## nomad-downloadrelease
+## downloadrelease
 
 Program for downloading specific Nomad release binary from their release page.
 I use it for testing and checking new Nomad versions.
 
 ```
-$ nomad-downloadrelease nomad
+$ nomadtools downloadrelease nomad
 INFO:nomad_tools.nomad_downloadrelease:Downloading https://releases.hashicorp.com/nomad/1.7.3/nomad_1.7.3_linux_amd64.zip to nomad
 INFO:nomad_tools.nomad_downloadrelease:https://releases.hashicorp.com/nomad/1.7.3/nomad_1.7.3_linux_amd64.zip -> -rwxr-xr-x 105.7MB nomad
-$ nomad-downloadrelease consul
+$ nomadtools downloadrelease consul
 INFO:nomad_tools.nomad_downloadrelease:Downloading https://releases.hashicorp.com/consul/1.9.9/consul_1.9.9_linux_amd64.zip to consul
 INFO:nomad_tools.nomad_downloadrelease:https://releases.hashicorp.com/consul/1.9.9/consul_1.9.9_linux_amd64.zip -> -rwxr-xr-x 105.8MB consul
-$ nomad-downloadrelease -p 1.6.3 nomad ./nomad1.6.3
+$ nomadtools downloadrelease -p 1.6.3 nomad ./nomad1.6.3
 INFO:nomad_tools.nomad_downloadrelease:Downloading https://releases.hashicorp.com/nomad/1.6.3/nomad_1.6.3_linux_amd64.zip to nomad1.6.3
 INFO:nomad_tools.nomad_downloadrelease:https://releases.hashicorp.com/nomad/1.6.3/nomad_1.6.3_linux_amd64.zip -> -rwxr-xr-x 101.8MB nomad1.6.3
 
 ```
 
 ## import nomad_tools
 
 This project is licensed under GPL. The internal API of this project can be
 used, however it is not stable at all and is an implementation detail.
 
 Internally, `nomad_tools.nomadlib` is a Python class definitions which
 represents models for Nomad API data documentation.
 
+# History
+
+This module once installed bunch of separate tools, like `nomad-watch` or
+`nomad-gitlab-runner`. That became unmaintainable. It is one `nomadtools`
+executable with several sub-commands.
+
 # Contributing
 
 Kindly make a issue or pull request on GitHub.
 I should be fast to respond and contributions are super welcome.
 
 ## Running tests
```

### Comparing `nomad-tools-0.2.4/README.md` & `nomad_tools-0.3.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,55 @@
-# nomad-tools
+Metadata-Version: 2.1
+Name: nomad-tools
+Version: 0.3.0
+Summary: Set of tools and utilities to ease interacting with Hashicorp Nomad scheduling solution.
+Author: Kamil Cukrowski
+License: GPL-3.0-or-later
+Project-URL: homepage, https://github.com/Kamilcuk/nomad-tools
+Project-URL: repository, https://github.com/Kamilcuk/nomad-tools
+Project-URL: documentation, https://github.com/Kamilcuk/nomad-tools
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: click==8.1.7
+Requires-Dist: python-dateutil==2.8.2
+Requires-Dist: PyYAML==6.0.1
+Requires-Dist: requests==2.31.0
+Requires-Dist: typing_extensions==4.7.1
+Requires-Dist: websocket-client==1.6.1
+Requires-Dist: clickdc==0.0.5
+Requires-Dist: clickforward==0.0.1
+Requires-Dist: python-dotenv==0.21.1
+Requires-Dist: packaging>=16.1
+Provides-Extra: test
+Requires-Dist: tomli==2.0.1; extra == "test"
+Requires-Dist: pytest==7.4.4; extra == "test"
+Requires-Dist: pytest-xdist==3.5.0; extra == "test"
+Requires-Dist: pytest-cov==4.1.0; extra == "test"
+
+# nomadtools
 
 Set of tools and utilities to ease interacting with HashiCorp Nomad scheduling solution.
 
 ## Table of Contents
 
 <!-- vim-markdown-toc GFM -->
 
 * [Installation](#installation)
     * [Shell completion](#shell-completion)
 * [Usage](#usage)
-    * [nomadt](#nomadt)
-    * [nomad-watch](#nomad-watch)
-    * [nomad-port](#nomad-port)
-    * [nomad-vardir](#nomad-vardir)
-    * [nomad-cp](#nomad-cp)
-    * [nomad-gitlab-runner](#nomad-gitlab-runner)
+    * [watch](#watch)
+    * [go](#go)
+    * [port](#port)
+    * [vardir](#vardir)
+    * [cp](#cp)
+    * [gitlab-runner](#gitlab-runner)
     * [nomad-dockers](#nomad-dockers)
-    * [nomad-downloadrelease](#nomad-downloadrelease)
+    * [downloadrelease](#downloadrelease)
     * [import nomad_tools](#import-nomad_tools)
+* [History](#history)
 * [Contributing](#contributing)
     * [Running tests](#running-tests)
 * [License](#license)
 
 <!-- vim-markdown-toc -->
 
 # Installation
@@ -29,210 +57,245 @@
 This is a bundle of executables packages together in a PyPY package. Install
 using `pipx` project.
 
 ```
 pipx install nomad-tools
 ```
 
+After installation the executable `nomadtools` should be available.
+
+```
+nomadtools --help
+```
+
 ## Shell completion
 
-After installation, see `nomad-watch --autocomplete-info` for shell
+After installation, see `nomadtools watch --autocomplete-info` for shell
 completion installation instruction.
 
 # Usage
 
-This module install several command line tools:
-
-## nomadt
-
-`nomadt` is a wrapper around `nomad` commands and `nomad-anything`
-command. If a `nomad` sub-command exists, `nomad` will be run. Otherwise
-an executable `nomad-subcommand` will be executed for a given sub-command.
-
-The intention is that you can do `alias nomad=nomadt` and use it seamlessly.
+This module installs command line tool `nomadtools` with several modes of
+operation:
 
-```
-nomadt job run example.nomad.hcl    # will execute nomad job run example.nomad.hcl
-nomadt watch run example.nomad.hcl  # will execute nomad-watch run example.nomad.hcl
-```
+## watch
 
-## nomad-watch
-
-Nomad-watch is meant to watch over a job change that you type in
+`nomadtools watch` is meant to watch over a job change that you type in
 terminal. It prints all relevant messages - messages about allocation,
 evaluation, deployment and stdout and stderr logs from all the
 processes. Depending on the mode of operation, the tool waits until an
 action is finished.
 
-I primarily use nomad-watch to deploy new versions of services. I was always
+I primarily use `watch` to deploy new versions of services. I was always
 frustrated that I start something from terminal and then I have to check the
 logs of the service in multiple tabs in the Nomad web interface. For example,
-you can use `nomad-watch start ./postgres.nomad.hcl` to update postgres
+you can use `watch start ./postgres.nomad.hcl` to update PostgreSQL
 container and watch it's logs in your terminal.
 
 An example terminal session deploying a HTTP server job with canary and health
 check. Note that while the new version is deployed, the old one still prints
 the logs.
 
-![gif showing example usage of nomad-watch start](./assets/imgs/nomad-watch-start-listen.gif)
+![gif showing example usage of watch start](./assets/imgs/nomad-watch-start-listen.gif)
 
 Another usage of the job is to run an one-shot batch jobs to do something and
 wait until they are finished and collect the exit status and logs, for example
 as an airflow or cron job. In this case `run` mode will wait for the job to be
-finished. For example `nomad-watch --purge run ./compute.nomad.hcl` will run
+finished. For example `watch --purge run ./compute.nomad.hcl` will run
 a calculation job, purge after it is done and exit with calculate job exit
 status (if there is one task).
 
-![gif showing example usage of nomad-watch run](./assets/imgs/nomad-watch-run-compute.gif)
+![gif showing example usage of watch run](./assets/imgs/nomad-watch-run-compute.gif)
+
+Internally, watch uses Nomad event stream to get the events in real time.
 
-Internally, nomad-watch uses Nomad event stream to get the events in real time.
+## go
 
-## nomad-port
+Mimics operation of `docker run`, it is built on top of `watch` mode to
+execute a single Nomad job created dynamically from command line arguments.
+It creates a Nomad job specification from command line arguments and then
+"watches" over the execution of the job.
+
+```
+$ nomadtools go --rm alpine apk add bash
+INFO:nomad_tools.nomad_watch:Watching job nomad_tools_go_5305da8f-b376-4c35-9a05-71027aadd587@default until it is finished
+Allocation 70c4ac9d-0e03-53d7-6e34-9c86cf8ee768 started on leonidas
+Received Task received by client
+Task Setup Building Task Directory
+Driver Downloading image
+Started Task started by client
+INFO:nomad_tools.nomad_watch:Job nomad_tools_go_5305da8f-b376-4c35-9a05-71027aadd587#0@default started allocations 70c4ac running group 'nomad_tools_go_5305da8f-b376-4c35-9a05-71027aadd587' with 1 main tasks.
+fetch https://dl-cdn.alpinelinux.org/alpine/v3.19/main/x86_64/APKINDEX.tar.gz
+fetch https://dl-cdn.alpinelinux.org/alpine/v3.19/community/x86_64/APKINDEX.tar.gz
+(1/4) Installing ncurses-terminfo-base (6.4_p20231125-r0)
+(2/4) Installing libncursesw (6.4_p20231125-r0)
+(3/4) Installing readline (8.2.1-r2)
+(4/4) Installing bash (5.2.21-r0)
+Terminated Exit Code: 0
+Allocation 70c4ac9d-0e03-53d7-6e34-9c86cf8ee768 finished
+Executing bash-5.2.21-r0.post-install
+Executing busybox-1.36.1-r15.trigger
+OK: 10 MiB in 19 packages
+INFO:nomad_tools.nomad_watch:Purging job nomad_tools_go_5305da8f-b376-4c35-9a05-71027aadd587
+INFO:nomad_tools.nomad_watch:Job nomad_tools_go_5305da8f-b376-4c35-9a05-71027aadd587#0@default purged with no active allocations, evaluations nor deployments. Exiting.
+INFO:nomad_tools.nomad_watch:Single task exited with 0 exit status. Exit code is 0.
+```
+
+## port
 
 Prints out the ports allocated for a particular Nomad job or
 allocation. It is meant to mimic `docker port` command.
 
 ```
-$ nomad-port httpd
+$ nomadtools port httpd
 192.168.0.5:31076
-$ nomad-port -l httpd
+$ nomadtools port -l httpd
 192.168.0.5 31076 http httpd.listen[0] d409e855-bf13-a342-fe7a-6fb579d2de85
-$ nomad-port --alloc d409e855
+$ nomadtools port --alloc d409e855
 192.168.0.5:31076
 ```
 
 Further argument allows to filter for port label.
 
 ```
-$ nomad-port httpd http
+$ nomadtools port httpd http
 192.168.0.5:31076
 ```
 
-## nomad-vardir
+## vardir
 
 I was frustrated with how Nomad variables look like. It is really hard to
 incrementally modify Nomad variables. The API is at one go. You either update
 all variables or nothing. Most often I wanted to update a single key
 from a Nomad variable at a time and the variable value was usually a file content.
 
 Example execution of putting a `passwordfile.txt` into `nomad/jobs/nginx`
 Nomad variable:
 
 ```
-$ nomad-vardir -j nginx put ./passwordfile.txt 
+$ nomadtools vardir -j nginx put ./passwordfile.txt 
 nomad_vardir: Putting var nomad/jobs/nginx@default with keys: passwordfile.txt
-$ nomad-vardir -j nginx cat passwordfile.txt 
+$ nomadtools vardir -j nginx cat passwordfile.txt 
 secretpassword
-$ nomad-vardir -j nginx ls
+$ nomadtools vardir -j nginx ls
 nomad_vardir: Listing Nomad variable at nomad/jobs/nginx@default
 key              size
 passwordfile.txt 15
 ```
 
 You can then remove the `passwordfile.txt` key from the Nomad variable:
 
 ```
-$ nomad-vardir -j nginx rm passwordfile.txt 
+$ nomadtools vardir -j nginx rm passwordfile.txt 
 nomad_vardir: Removing passwordfile.txt
 nomad_vardir: Removing empty var nomad/jobs/nginx@default
-$ nomad-vardir -j nginx ls
+$ nomadtools vardir -j nginx ls
 nomad_vardir: Nomad variable not found at nomad/jobs/nginx@default
 ```
 
-## nomad-cp
+## cp
 
 This is a copy of the `docker cp` command. The syntax is meant to be the
 same with docker. The rules of copying a file vs directory are meant to be
 in-line with `docker cp` documentation.
 
-`nomad-cp` uses some special syntax for specifying from which allocation/task
+`nomadtools cp` uses some special syntax for specifying from which allocation/task
 exactly do you want to copy by using colon `:`. The number of colons in the
 arguments determines the format. The colon can be escaped with slash `\` in
 the path if needed.
 
 Both `SRC` and `DST` addresses can be specified as follows:
 
 ```
+# Search a task matching specific URL query:
+task://JOB[@NAMESPACE]/PATH[?group=GROUP][&alloc=ALLOC][&task=TASK][&hostname=HOSTNAME][&node=NODE]
+# or
 :ALLOCATION:PATH                  copy path from this allocation having one job
-:ALLOCATION:TASK:PATH             copy path from this task inside allocation
+:ALLOCATION::TASK:PATH            copy path from this task inside allocation
 :ALLOCATION:GROUP:TASK:PATH       like above, but filter by group name
 JOB:PATH                          copy path from one task inside specified job
-JOB:TASK:PATH                     copy path from the task inside this job
+JOB::TASK:PATH                    copy path from the task inside this job
 JOB:GROUP:TASK:PATH               like above, but filter also by group name
 PATH                              copy local path
 -                                 copy stdin or stdout TAR stream
 ```
 
-`nomad-cp` depends on `sh` and `tar` command line utility to be available
+`cp` depends on `sh` and `tar` command line utility to be available
 inside the allocation it is coping to/from. It has to be available there.
 
 Example:
 
 ```
-$ nomad-cp -v nginx:/etc/nginx/nginx.conf ./nginx.conf
+$ nomadtools cp -v nginx:/etc/nginx/nginx.conf ./nginx.conf
 INFO nomad_cp.py:copy_mode:487: File :d409e855-bf13-a342-fe7a-6fb579d2de85:listen:/etc/nginx/nginx.conf -> ./nginx.conf
-$ nomad-cp -v alpine:/etc/. ./etc/
+$ nomadtools cp -v alpine:/etc/. ./etc/
 INFO nomad_cp.py:copy_mode:512: New mkdir :d409e855-bf13-a342-fe7a-6fb579d2de85:listen:/etc/. -> /home/kamil/tmp/etc2/
 ```
 
 Nomad does not have the capability of accessing any file inside the
 allocation file system. Instead, `nomad-cp` executes several `nomad exec`
 calls to execute a `tar` pipe to stream the data from or to the allocation
 context to or from the local host using stdout and stdin forwarded by
 `nomad exec`.
 
-## nomad-gitlab-runner
+## gitlab-runner
 
 An implementation of custom Gitlab executor driver that runs Gitlab CI/CD jobs
 using Nomad.
 
 This program does _not_ run the `gitlab-runner` itself in Nomad. Rather, the
 `gitlab-runner` is running on (any) one host. That `gitlab-runner` will then
 schedule Nomad jobs to execute using the script as an executor. These jobs will
 execute the CI/CD from Gitlab inside Nomad cluster.
 
-More on it can be read on [github wiki](https://github.com/Kamilcuk/nomad-tools/wiki/nomad%E2%80%90gitlab%E2%80%90runner).
+More on it can be read on [github wiki](https://github.com/Kamilcuk/nomadtools/wiki/gitlab%E2%80%90runner).
 
 ## nomad-dockers
 
 Lists docker images referenced in Nomad job file or a running Nomad job.
 
 ```
-$ nomad-dockers ./httpd.nomad.hcl
+$ nomadtools dockers ./httpd.nomad.hcl
 busybox:stable
-$ nomad-dockers --job httpd
+$ nomadtools dockers --job httpd
 busybox:stable
 ```
 
-## nomad-downloadrelease
+## downloadrelease
 
 Program for downloading specific Nomad release binary from their release page.
 I use it for testing and checking new Nomad versions.
 
 ```
-$ nomad-downloadrelease nomad
+$ nomadtools downloadrelease nomad
 INFO:nomad_tools.nomad_downloadrelease:Downloading https://releases.hashicorp.com/nomad/1.7.3/nomad_1.7.3_linux_amd64.zip to nomad
 INFO:nomad_tools.nomad_downloadrelease:https://releases.hashicorp.com/nomad/1.7.3/nomad_1.7.3_linux_amd64.zip -> -rwxr-xr-x 105.7MB nomad
-$ nomad-downloadrelease consul
+$ nomadtools downloadrelease consul
 INFO:nomad_tools.nomad_downloadrelease:Downloading https://releases.hashicorp.com/consul/1.9.9/consul_1.9.9_linux_amd64.zip to consul
 INFO:nomad_tools.nomad_downloadrelease:https://releases.hashicorp.com/consul/1.9.9/consul_1.9.9_linux_amd64.zip -> -rwxr-xr-x 105.8MB consul
-$ nomad-downloadrelease -p 1.6.3 nomad ./nomad1.6.3
+$ nomadtools downloadrelease -p 1.6.3 nomad ./nomad1.6.3
 INFO:nomad_tools.nomad_downloadrelease:Downloading https://releases.hashicorp.com/nomad/1.6.3/nomad_1.6.3_linux_amd64.zip to nomad1.6.3
 INFO:nomad_tools.nomad_downloadrelease:https://releases.hashicorp.com/nomad/1.6.3/nomad_1.6.3_linux_amd64.zip -> -rwxr-xr-x 101.8MB nomad1.6.3
 
 ```
 
 ## import nomad_tools
 
 This project is licensed under GPL. The internal API of this project can be
 used, however it is not stable at all and is an implementation detail.
 
 Internally, `nomad_tools.nomadlib` is a Python class definitions which
 represents models for Nomad API data documentation.
 
+# History
+
+This module once installed bunch of separate tools, like `nomad-watch` or
+`nomad-gitlab-runner`. That became unmaintainable. It is one `nomadtools`
+executable with several sub-commands.
+
 # Contributing
 
 Kindly make a issue or pull request on GitHub.
 I should be fast to respond and contributions are super welcome.
 
 ## Running tests
```

### Comparing `nomad-tools-0.2.4/src/nomad_tools/colors.py` & `nomad_tools-0.3.0/src/nomad_tools/colors.py`

 * *Files identical despite different names*

### Comparing `nomad-tools-0.2.4/src/nomad_tools/common_click.py` & `nomad_tools-0.3.0/src/nomad_tools/common_click.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 from typing import Any, Callable, Dict, Iterable, List, Optional
 
 import click
 
-from .common_base import NOMAD_NAMESPACE, composed, print_version, shell_completion
+from .common_base import composed, print_version, shell_completion
 
 
 def complete_set_namespace(ctx: click.Context):
     namespace = ctx.params.get("namespace")
     if namespace:
-        os.environ[NOMAD_NAMESPACE] = namespace
+        os.environ["NOMAD_NAMESPACE"] = namespace
 
 
 def completor(
     cb: Callable[[], Iterable[str]]
 ) -> Callable[[click.Context, str, str], Optional[List[str]]]:
     def completor_cb(
         ctx: click.Context, param: str, incomplete: str
@@ -35,17 +35,16 @@
             return
         cb()
         ctx.exit()
 
     return wrap
 
 
-def common_options():
+def main_options():
     return composed(
-        click.help_option("-h", "--help"),
         click.option(
             "--version",
             is_flag=True,
             callback=click_callback_wrap_exit(print_version),
             expose_value=False,
             is_eager=True,
             help="Print program version then exit.",
@@ -65,14 +64,20 @@
             expose_value=False,
             is_eager=True,
             help="Install shell completion.",
         ),
     )
 
 
+def common_options():
+    return composed(
+        click.help_option("-h", "--help"),
+    )
+
+
 def __alias_option_callback(
     aliased: Dict[str, Any],
     ctx: click.Context,
     param: click.Parameter,
     value: Any,
 ):
     """Callback called from alias_option option."""
```

### Comparing `nomad-tools-0.2.4/src/nomad_tools/exit_on_thread_exception.py` & `nomad_tools-0.3.0/src/nomad_tools/exit_on_thread_exception.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 def patched_init(self, *args, **kwargs):
     original_init(self, *args, **kwargs)
     original_run = self.run
 
     def patched_run(*args, **kw):
         try:
             original_run(*args, **kw)
+        except SystemExit:
+            os._exit(1)
         except BaseException:
             traceback.print_exc()
             os._exit(1)
 
     self.run = patched_run
```

### Comparing `nomad-tools-0.2.4/src/nomad_tools/nomad_cp.py` & `nomad_tools-0.3.0/src/nomad_tools/nomad_cp.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,60 @@
 #!/usr/bin/env python3
 
 from __future__ import annotations
 
-import argparse
+import collections
+import contextlib
 import enum
 import logging
 import os
 import re
 import shlex
-import shutil
+import string
 import subprocess
 import sys
 import textwrap
+import traceback
 from abc import ABC
 from dataclasses import dataclass
 from pathlib import Path
 from shlex import quote, split
-from typing import Any, List, Optional
+from typing import IO, Any, Dict, Iterator, List, Optional
+from urllib.parse import parse_qs, urlparse
 
 import click
-from click.shell_completion import BashComplete, CompletionItem
-from typing_extensions import override
+import clickdc
+from click.shell_completion import CompletionItem
+from typing_extensions import Protocol, override
 
 from . import nomadlib, taskexec
 from .common import (
     cached_property,
     common_options,
     mynomad,
     namespace_option,
     nomad_find_job,
 )
 from .common_base import quotearr
+from .transferstats import transfer_stats
 
 log = logging.getLogger(Path(__file__).name)
+ARGS: "Args"
+
+###############################################################################
+
+
+def popen_raise_for_returncode(pp: subprocess.Popen):
+    if pp.returncode:
+        raise subprocess.CalledProcessError(pp.returncode, pp.args)
+
+
+class MyPopen(Protocol):
+    stdin: Optional[IO[bytes]]
+    stdout: Optional[IO[bytes]]
 
 
 ###############################################################################
 
 
 @dataclass
 class Mypath(ABC):
@@ -44,27 +62,29 @@
 
     path: str
     """
     This is string represented of the path.
     This has to be a string to properly handle /. suffixes in strings given by user.
     """
 
-    def run(self, cmd: str):
-        log.debug(f"+ {cmd}")
-        subprocess.run(split(cmd), check=True)
-
     def check_output(self, cmd: str) -> str:
         log.debug(f"+ {cmd}")
         return subprocess.check_output(split(cmd), text=True)
 
+    @contextlib.contextmanager
     def popen(
-        self, cmd: str, stdout: Optional[int] = None, stdin: Optional[int] = None
-    ) -> Any:
+        self,
+        cmd: str,
+        stdin: int = subprocess.DEVNULL,
+        stdout: int = subprocess.DEVNULL,
+    ) -> Iterator[MyPopen]:
         log.debug(f"+ {cmd}")
-        return subprocess.Popen(split(cmd), stdout=stdout, stdin=stdin)
+        with subprocess.Popen(split(cmd), stdin=stdin, stdout=stdout) as pp:
+            yield pp
+        popen_raise_for_returncode(pp)
 
     def isstdin(self) -> bool:
         return str(self.path) == "-"
 
     def isnomad(self) -> bool:
         return False
 
@@ -88,429 +108,521 @@
         return str(self.path)
 
     def __itruediv__(self, name: str):
         self.path = os.path.join(self.path, name)
         return self
 
     def quoteparent(self):
-        return quote(os.path.dirname(self.path))
+        # Dirname may return an empty string. Return dot in such case.
+        return quote(os.path.dirname(self.path) or ".")
 
     def quotename(self):
-        return quote(os.path.basename(self.path))
+        return quote(os.path.basename(self.path) or ".")
 
     def quotepath(self):
         return quote(self.path)
 
 
 class FileType(enum.Enum):
     file = enum.auto()
     dir = enum.auto()
-    none = enum.auto()
+    notexists = enum.auto()
+    other = enum.auto()
 
 
 @dataclass
 class NomadMypath(Mypath):
     """Represents a path inside a specific Nomad task"""
 
     allocation: str
     task: str
 
     @override
-    def run(self, cmd: str):
-        log.debug(f"+ {self.allocation} {self.task} {cmd}")
-        taskexec.run(self.allocation, self.task, split(cmd))
-
-    @override
     def check_output(self, cmd: str) -> str:
-        log.debug(f"+ {self.allocation} {self.task} {cmd}")
-        return taskexec.check_output(self.allocation, self.task, split(cmd), text=True)
+        log.debug(f"+ {self.allocation}/{self.task} {cmd}")
+        with taskexec.TaskExec(self.allocation, self.task, split(cmd)) as pp:
+            pp.close_stdin()
+            buf: bytes = pp.read()
+        pp.raise_for_returncode(buf)
+        return buf.decode(errors="replace")
 
     @override
+    @contextlib.contextmanager
     def popen(
-        self, cmd: str, stdout: Optional[int] = None, stdin: Optional[int] = None
-    ) -> Any:
-        log.debug(f"+ {self.allocation} {self.task} {cmd}")
-        return taskexec.NomadPopen(
-            self.allocation, self.task, split(cmd), stdout=stdout, stdin=stdin
-        )
+        self,
+        cmd: str,
+        stdin: int = subprocess.DEVNULL,
+        stdout: int = subprocess.DEVNULL,
+    ) -> Iterator[MyPopen]:
+        log.debug(f"+ {self.allocation}/{self.task} {cmd}")
+        i = str(bool(stdin != subprocess.DEVNULL)).lower()
+        cmdarr: List[str] = [
+            *f"nomad alloc exec -i={quote(i)} -t=false -task={quote(self.task)}".split(),
+            self.allocation,
+            *split(cmd),
+        ]
+        log.debug(f"+ {quotearr(cmdarr)}")
+        with subprocess.Popen(cmdarr, stdin=stdin, stdout=stdout) as pp:
+            yield pp
+        popen_raise_for_returncode(pp)
 
     @override
     def isstdin(self) -> bool:
         return False
 
     @override
     def isnomad(self) -> bool:
         return True
 
     def _nomadrunsh(self, script: str, *args: str) -> str:
-        cmd = [
-            "sh",
-            "-c",
-            script,
-            *args,
-        ]
+        cmd = ["sh", "-c", script, *args]
         cmdstr = quotearr(cmd)
         log.debug(f"+ {cmdstr}")
         return self.check_output(cmdstr).strip()
 
     @cached_property
     def _nomadstat(self) -> FileType:
         assert self.isnomad()
         # Execute a script inside the container to determine the type of the file.
-        script = 'if [ -f "$1" ]; then echo file; elif [ -d "$1" ]; then echo dir; else echo none; fi'
-        stat = self._nomadrunsh(script, "--", self.path)
+        script = (
+            'if [ -f "$1" ]; then echo file;'
+            ' elif [ -d "$1" ]; then echo dir;'
+            ' elif ! [ -e "$1" ]; then echo notexists;'
+            " else echo other; fi"
+        )
+        stat = self._nomadrunsh(script, "sh", self.path)
         log.debug(f"stat = {stat}")
         return FileType[stat]
 
     @override
     def exists(self) -> bool:
-        return self._nomadstat != FileType.none
+        return self._nomadstat != FileType.notexists
 
     @override
     def is_file(self) -> bool:
         return self._nomadstat == FileType.file
 
     @override
     def is_dir(self) -> bool:
         return self._nomadstat == FileType.dir
 
     @override
     def mkdir(self):
-        v = "v" if args.verbose else ""
+        v = "v" if ARGS.verbose else ""
         self._nomadrunsh(f"mkdir -{v}p {quote(self.path)}")
 
     @staticmethod
     def __colon(arg: str):
-        """Replaces single colon by esacped for printing"""
+        """Replaces single colon by escaped for printing"""
         return arg.replace(":", r"\:")
 
     @override
     def __str__(self):
         return f":{self.__colon(self.allocation)}:{self.__colon(self.task)}:{quote(self.__colon(str(self.path)))}"
 
+    def compgen(self) -> List[str]:
+        """Given incomplete line, generate compgen of files inside a running allocation if possible"""
+        # This is some magic to handle find arguments.
+        path: str = self.path
+        parts: List[str] = path[::-1].split("/", 1)
+        noslash: bool = len(parts) == 1
+        searchdir: str = "." if noslash else (parts[1][::-1] + "/")
+        searchname: str = parts[0][::-1]
+        searchnamenoglob: str = (
+            searchname.replace("\\", "\\\\")
+            .replace(r"*", r"\*")
+            .replace(r"?", r"\?")
+            .replace(r"[", r"\[")  # ]]
+        )
+        # Repetition in output means it is a directory.
+        # Technically, maxdepth and mindepth are not POSIX.
+        cmd: str = (
+            f'find {quote(searchdir)} -maxdepth 1 -mindepth 1 -name {quote(searchnamenoglob)}"*"'
+            f' "(" -type f  -print ")" -o "(" -type d -print -print ")"'
+        )
+        output = self.check_output(cmd)
+        # Add trailing / to directories.
+        ret: List[str] = [
+            k if v == 1 else (k + "/")
+            for k, v in collections.Counter(output.split("\n")).items()
+            if k
+        ]
+        # In case of noslash is given, the initial part is going to be './'. Strip it.
+        ret = [x[2 if noslash else 0 :] for x in ret]
+        return ret
+
 
 ###############################################################################
 
 
-class NomadOrHostMyPath(click.ParamType):
+@dataclass
+class ArgPath:
+    """Represents splitted up parts of the input"""
+
     _description = textwrap.dedent(
         """\
-        :ALLOCATION:PATH
-        :ALLOCATION:TASK:PATH
-        :ALLOCATION:GROUP:TASK:PATH
-        JOB:PATH
-        JOB:TASK:PATH
-        JOB:GROUP:TASK:PATH
+        :ALLOCATION[:TASK]:[PATH]
+        JOB[:[GROUP][:TASK]]:[PATH]
+        task://JOB[@NAMESPACE]/PATH[?group=GROUP][&alloc=ALLOC][&task=TASK][&hostname=HOSTNAME][&node=NODE]
         PATH
         -
         """
     )
 
-    name = "path"
-
-    @dataclass
-    class Elem:
-        """Represents splitted up parts of the input"""
-
-        path: str
-        isalloc: bool = False
-        id: Optional[str] = None
-        group: Optional[str] = None
-        task: Optional[str] = None
+    arg: str
+    path: str
+    arr: Optional[List[str]] = None
+    alloc: Optional[str] = None
+    job: Optional[str] = None
+    group: Optional[str] = None
+    task: Optional[str] = None
+    namespace: Optional[str] = None
+    hostname: Optional[str] = None
+    node: Optional[str] = None
 
     @staticmethod
-    def __split_on_colon(arg: str) -> List[str]:
-        """Splits string on un-escaped colon, and then replaced secaped colons by colons"""
-        return [x.replace(r"\:", ":") for x in re.split(r"(?<!\\):", arg)]
-
-    @classmethod
-    def __split_arg(cls, arg: str) -> NomadOrHostMyPath.Elem:
+    def mk(arg: str) -> ArgPath:
         """Converts the argument into it's parts represented with object"""
-        arr = cls.__split_on_colon(arg)
-        el = cls.Elem(arr[-1])
-        if len(arr) > 1:
-            if arr[0] == "":
-                el.isalloc = True
-                el.id = arr[1]
-                arr = arr[1:]
-            else:
-                el.isalloc = False
-                el.id = arr[0]
-            el.group = arr[1] if len(arr) > 3 else None
-            el.task = arr[2] if len(arr) > 3 else arr[1] if len(arr) > 2 else None
-            assert len(arr) <= 5, f"Could not parse argument, too many colons: {arg}"
-        return el
+        if not arg.startswith("task://"):
+            # Split string on un-escaped colon, and then replaced secaped colons by colons
+            arr: List[str] = [x.replace(r"\:", ":") for x in re.split(r"(?<!\\):", arg)]
+            assert len(arr) <= 4, f"Could not parse argument: too many colons: {arg!r}"
+            path: str = arr[-1]
+            if len(arr) > 1:
+                if arr[0] == "":
+                    return ArgPath(
+                        arg=arg,
+                        arr=arr,
+                        path=path,
+                        alloc=arr[1],
+                        task=arr[2] if len(arr) > 3 else None,
+                    )
+                else:
+                    return ArgPath(
+                        arg=arg,
+                        arr=arr,
+                        path=path,
+                        job=arr[0],
+                        group=arr[1] if len(arr) > 2 else None,
+                        task=arr[2] if len(arr) > 3 else None,
+                    )
+            return ArgPath(arg=arg, arr=arr, path=path)
+        o = urlparse(arg)
+        assert o.scheme == "task", "Internal error"
+        assert o.port is None, f"Port in URL doesn't make sense: {arg!r}"
+        qsl: Dict[str, List[str]] = parse_qs(o.query)
+        qs: Dict[str, str] = {k: v[-1] for k, v in qsl.items()}
+        fields = "alloc task group hostname node".split()
+        for k in qs.keys():
+            assert k in fields, f"Unknown URL parameter {k}: {arg!r}"
+        return ArgPath(
+            arg=arg,
+            path=o.path[1:] if o.path and o.path[0] == "/" else o.path,
+            job=o.username if o.username else o.hostname,
+            namespace=o.hostname if o.username else None,
+            arr=None,
+            **qs,
+        )
 
-    @classmethod
-    def __parse_arg(cls, arg: str) -> Mypath:
+    def __post_init__(self):
+        assert (
+            (not self.alloc and not self.job)
+            or (self.alloc and not self.job)
+            or (not self.alloc and self.job)
+        ), f"Internal error: initialized in both alloc and job mode: {self.arg!r} {self.alloc} {self.job}"
+        if self.alloc:
+            alloweddigits = string.hexdigits + "-"
+            assert all(
+                c in alloweddigits for c in self.alloc
+            ), f"Allocation ID can only be one of {alloweddigits!r}: {self.alloc}"
+
+    @cached_property
+    def __find_jobid(self):
+        assert self.job
+        return nomad_find_job(self.job)
+
+    @cached_property
+    def __allocations(self):
+        """Return running allocations with ID starting with self.alloc"""
+        assert self.alloc is not None
+        # It is only possible to prefix using even length. Query uneven length using filter expression.
+        alloc = "".join(c for c in self.alloc if c in string.hexdigits)
+        params = dict(
+            prefix=alloc[: len(alloc) // 2 * 2],
+            filter=f'ID matches "^{self.alloc}"' if len(alloc) % 2 != 0 else None,
+        )
+        allocations: List[nomadlib.Alloc] = [
+            nomadlib.Alloc(x) for x in mynomad.get("allocations", params=params)
+        ]
+        return self.__filter_alocations(allocations)
+
+    def __filter_alocations(
+        self, allocations: List[nomadlib.Alloc]
+    ) -> List[nomadlib.Alloc]:
+        return [
+            alloc
+            for alloc in allocations
+            if alloc.is_running()
+            and len(alloc.get_taskstates()) != 0
+            and (not self.alloc or alloc.ID.startswith(self.alloc))
+            and (not self.task or self.task in alloc.get_tasknames())
+            and (not self.group or alloc.TaskGroup == self.group)
+            and (not self.hostname or alloc.NodeName == self.hostname)
+            and (not self.node or alloc.NodeID == self.node)
+        ]
+
+    @cached_property
+    def __allocation(self):
+        """Return the single running allocation with ID starting with self.alloc"""
+        assert self.alloc
+        allocs = self.__allocations
+        assert len(allocs) > 0, f"Found no running allocations matching {self.arg!r}"
+        assert (
+            len(allocs) == 1
+        ), f"Found multiple running allocations matching {self.arg!r}"
+        return allocs[0]
+
+    def to_mypath(self) -> Mypath:
         """Converts the argument into NomadMypath or Mypath object"""
-        el = cls.__split_arg(arg)
-        if not el.id:
-            return Mypath(el.path)
         # The job here is to find the allocation associated with specified parameters.
-        if el.isalloc:
-            allocations = [
-                nomadlib.Alloc(x)
-                for x in mynomad.get("allocations", params=dict(prefix=el.id))
-            ]
-            allocations = [x for x in allocations if x["ID"].startswith(el.id)]
-            assert len(allocations) >= 1, f"No allocation starts with {el.id}"
-            assert len(allocations) == 1, f"Multiple allocations start with {el.id}"
-            allocation = allocations[0]
-            assert allocation.is_running(), f"Allocation {allocation.ID} is not running"
-            assert (
-                len(allocation.get_taskstates()) != 0
-            ), f"Allocation {allocation.ID} has no running tasks"
-            allocations = [allocation]
-        else:
-            jobid = nomad_find_job(el.id)
+        if self.alloc:
+            allocations = [self.__allocation]
+        elif self.job:
+            jobid = self.__find_jobid
             allocations = [
                 nomadlib.Alloc(x) for x in mynomad.get(f"job/{jobid}/allocations")
             ]
             allocations = [x for x in allocations if x.is_running()]
             assert len(allocations) >= 1, f"Job {jobid} has no running allocations"
-        if el.group:
-            allocations = [x for x in allocations if x.TaskGroup == el.group]
-            assert len(allocations) >= 1, f"No allocations matching group {el.group}"
-        if el.task:
-            allocations = [x for x in allocations if el.task in x.get_tasknames()]
-            assert len(allocations) >= 1, f"No allocations running task {el.task}"
+        else:
+            # It is a local filesystem path, just return.
+            return Mypath(self.path)
+        # Filter using group.
+        if self.group:
+            allocations = [x for x in allocations if x.TaskGroup == self.group]
+            assert (
+                len(allocations) >= 1
+            ), f"No running allocations after matching group: {self.arg!r}"
+        # Filter on the task.
+        if self.task:
+            allocations = [x for x in allocations if self.task in x.get_tasknames()]
+            assert (
+                len(allocations) >= 1
+            ), f"No running allocations after matching task: {self.arg!r}"
         assert (
             len(allocations) == 1
-        ), f"Found multiple allocations mathing {arg!r}: {' '.join(x.ID for x in allocations)}"
+        ), f"Found multiple running allocations mathing {self.arg!r}: {' '.join(x.ID for x in allocations)}"
         allocation = allocations[0]
-        task = el.task if el.task else allocation.get_tasknames()[0]
-        return NomadMypath(el.path, allocation.ID, task)
-
-    def convert(
-        self, value: Any, param: Optional[click.Parameter], ctx: Optional[click.Context]
-    ) -> Mypath:
-        """Entrypoint for click option conversion"""
-        return value if isinstance(value, Mypath) else self.__parse_arg(value)
+        if self.task:
+            task = self.task
+        else:
+            # Get running tasks of specific allocation.
+            runningtasks: List[str] = [
+                task
+                for task, state in allocation.get_taskstates().items()
+                if state.FinishedAt is None
+            ]
+            assert (
+                len(runningtasks) != 0
+            ), f"No running tasks found in allocation {allocation.ID} matching {self.arg!r}"
+            assert len(runningtasks) == 1, (
+                f"Multiple running tasks found in allocation {allocation.ID}"
+                f" matching {self.arg!r}: {' '.join(runningtasks)}"
+            )
+            task = runningtasks[0]
+        return NomadMypath(self.path, allocation.ID, task)
 
     @staticmethod
     def __filter(
-        arr: List[str], prefix: str, suffix: str = ":"
+        arr: List[str], prefix: str, suffix: str = ":", addnospace: bool = True
     ) -> List[CompletionItem]:
         """Filter list of string by prefix and convert to CompletionItem. Also remove duplicates"""
-        return [
+        nospace = CompletionItem("", type="nospace")
+        ret = [
             CompletionItem(shlex.quote(f"{x}{suffix}"))
             for x in sorted(list(set(x for x in arr if x.startswith(prefix))))
         ]
+        if ret and addnospace:
+            ret = [nospace] + ret
+        return ret
 
     @staticmethod
     def debug(msg: str):
         if os.environ.get("COMP_DEBUG"):
-            print(msg, file=sys.stderr)
+            print(f"\n{msg}\n", file=sys.stderr)
 
     @classmethod
-    def __compgen(cls, incomplete: str) -> List[CompletionItem]:
+    def debugexception(cls, e: Exception):
+        cls.debug(f"{traceback.format_exc()} Exception: {e}")
+
+    def __compgen(self) -> List[CompletionItem]:
         """Given incomplete line, generate compgen of files inside a running allocation if possible"""
-        try:
-            mypath = cls.__parse_arg(incomplete)
-        except AssertionError:
-            return []
+        assert self.alloc or self.job
+        mypath = self.to_mypath()
         assert mypath.isnomad()
-        # This is some magic to handle find arguments.
-        path: str = mypath.path
-        parts: List[str] = path[::-1].split("/", 1)
-        noslash: bool = len(parts) == 1
-        searchdir: str = "." if noslash else parts[1][::-1] + "/"
-        searchname: str = parts[0][::-1]
-        searchnamenoglob = (
-            searchname.replace("\\", "\\\\")
-            .replace(r"*", r"\*")
-            .replace(r"?", r"\?")
-            .replace(r"[", r"\[")  # ]]
-        )
-        cmd = [
-            "sh",
-            "-c",
-            textwrap.dedent(
-                """\
-                find "$1" -maxdepth 1 -mindepth 1 -type f -name "$2*"
-                find "$1" -maxdepth 1 -mindepth 1 -type d -name "$2*" |
-                    while IFS= read -r line; do echo "$line/"; done
-                """
-            ),
-            "--",
-            searchdir,
-            searchnamenoglob,
+        assert isinstance(mypath, NomadMypath)
+        ret: List[str] = mypath.compgen()
+        addnospace: bool = len(ret) > 1 or any(x[-1] == "/" for x in ret)
+        return self.__filter(ret, self.path, suffix="", addnospace=addnospace)
+
+    def __complete_job_name(self, last: str, suffix: str = ":"):
+        jobs = [nomadlib.Job(x) for x in mynomad.get("jobs", params=dict(prefix=last))]
+        jobs = [
+            x
+            for x in jobs
+            if not x.is_dead()
+            and (not self.group or self.group in [g.Name for g in x.TaskGroups])
+            and (
+                not self.task
+                or self.task in [t.Name for g in x.TaskGroups for t in g.Tasks]
+            )
         ]
-        cmdstr = quotearr(cmd)
-        cls.debug(f"+ {cmdstr}")
-        try:
-            output = mypath.check_output(cmdstr)
-        except subprocess.CalledProcessError:
-            return []
-        # In case of noslash is given, the initial part is going to be './'. Strip it.
-        ret = [x[2 if noslash else 0 :] for x in output.splitlines()]
-        nospace = (
-            [CompletionItem("", type="nospace")]
-            if len(ret) > 1 or any(x[-1] == "/" for x in ret)
-            else []
-        )
-        return nospace + cls.__filter(ret, path, suffix="")
+        return self.__filter([x.ID for x in jobs], last, suffix=suffix)
 
-    @classmethod
-    def gen_shell_complete(cls, incomplete: str) -> List[CompletionItem]:
-        """Generate completion given value"""
-        arr = cls.__split_on_colon(incomplete)
-        files = [CompletionItem(incomplete, type="file")]
+    def __gen_shell_complete_arr(self) -> List[CompletionItem]:
+        """Generate completion for JOB:GROUP:TASK:PATH or :ALLOCATION:TASK:PATH"""
+        arr = self.arr
+        assert arr
+        add: List[CompletionItem] = []
+        last = self.path
         if len(arr) == 1:
-            # JOB...
             # PATH...
-            jobs = [x["ID"] for x in mynomad.get("jobs", params=dict(prefix=arr[0]))]
-            return (
-                files
-                + [CompletionItem("", type="nospace")]
-                + cls.__filter(jobs, arr[0])
-            )
-        elif arr[0] == "":
-            if len(arr) == 2:
-                # :ALLOCATION...
-                allocidprefix = arr[1]
-                allocations = [
-                    x["ID"]
-                    for x in mynomad.get("allocations", params=dict(prefix=arr[1]))
-                    if x["ID"].startswith(allocidprefix)
-                ]
-                return [CompletionItem("", type="nospace")] + cls.__filter(
-                    allocations, arr[1]
-                )
-            elif len(arr) in [3, 4, 5]:
-                # :ALLOCATION:PATH...
-                # :ALLOCATION:GROUP...
-                # :ALLOCATION:GROUP:PATH...
-                # :ALLOCATION:GROUP:TASK...
-                # :ALLOCATION:GROUP:TASK:PATH...
-                add = []
-                if "/" not in arr[-1]:
-                    allocidprefix = arr[1]
-                    allocations = [
-                        nomadlib.Alloc(x)
-                        for x in mynomad.get(
-                            "allocations", params=dict(prefix=allocidprefix)
-                        )
-                        if x["ID"].startswith(allocidprefix)
-                    ]
-                    assert (
-                        len(allocations) == 1
-                    ), f"Found multiple or none allocation matching prefix {allocidprefix}"
-                    allocation = allocations[0]
-                    if len(arr) <= 4:
-                        add = [CompletionItem("", type="nospace")] + cls.__filter(
-                            allocation.get_tasknames(), arr[-1]
-                        )
-                return add + cls.__compgen(incomplete)
-        elif len(arr) in [2, 3, 4]:
+            if "/" not in arr[0]:
+                # JOB...
+                add = self.__complete_job_name(last)
+            files = CompletionItem(self.arg, type="file")
+            return [files] + add
+        elif arr[0] == "" and len(arr) == 2:
+            # :ALLOCATION...
+            assert (
+                self.alloc is not None
+            ), f"Internal error: self.alloc is None on allocation path: {self}"
+            return self.__filter([x.ID for x in self.__allocations], self.alloc)
+        # If there is only a single matching allocation:task pair, just use it.
+        try:
+            # :ALLOCATION:PATH...
+            # :ALLOCATION:TASK:PATH...
             # JOB:PATH...
-            # JOB:GROUP...
             # JOB:GROUP:PATH...
-            # JOB:GROUP:TASK...
             # JOB:GROUP:TASK:PATH...
-            add = []
-            if "/" not in arr[-1]:
-                jobid = nomad_find_job(arr[0])
-                job = nomadlib.Job(mynomad.get(f"job/{jobid}"))
+            return self.__compgen()
+        except Exception as e:
+            ArgPath.debugexception(e)
+        # Otherwise show completions for the task or group names.
+        if arr[0] == "":
+            if len(arr) == 3:
+                # :ALLOCATION:TASK:...
+                return self.__filter(self.__allocation.get_tasknames(), last)
+        elif len(arr) in [2, 3]:
+            jobid = self.__find_jobid
+            job = nomadlib.Job(mynomad.get(f"job/{jobid}"))
+            if len(arr) == 2:
+                # JOB:GROUP...
+                groups = [g.Name for g in job.TaskGroups]
+                return self.__filter(groups, last)
+            elif len(arr) == 3:
+                # JOB:GROUP:TASK:...
                 tasks = [
                     t.Name
-                    for tg in job.TaskGroups
-                    if len(arr) < 3 or tg.Name == arr[2]
-                    for t in tg.Tasks
+                    for g in job.TaskGroups
+                    if (not self.group or g.Name == self.group)
+                    for t in g.Tasks
                 ]
-                add = [CompletionItem("", type="nospace")] + cls.__filter(
-                    tasks, arr[-1]
-                )
-            return add + cls.__compgen(incomplete)
+                return self.__filter(tasks, last)
         return []
 
-    def shell_complete(
-        self, ctx: click.Context, param: click.Parameter, incomplete: str
-    ) -> List[CompletionItem]:
+    def __gen_shell_complete_url(self) -> List[CompletionItem]:
+        self.debug(f"{self}")
+        if self.arg.count("/") == 2:
+            if "@" not in self.arg:
+                return self.__complete_job_name(self.job or "", suffix="/")
+            nss = mynomad.get("namespaces", params={"prefix": self.namespace or ""})
+            return self.__filter(
+                [x["Name"] for x in nss], self.namespace or "", suffix="/"
+            )
+        # If there is only a single matching allocation:task pair, just use it.
         try:
-            return self.gen_shell_complete(incomplete)
-        except Exception:
-            pass
+            return self.__compgen()
+        except Exception as e:
+            ArgPath.debugexception(e)
         return []
 
+    def gen_shell_complete(self) -> List[CompletionItem]:
+        """Generate completion given value"""
+        if self.arr:
+            return self.__gen_shell_complete_arr()
+        else:
+            return self.__gen_shell_complete_url()
 
-# Fix bash splitting completion on colon.
-# Use __reassemble_comp_words_by_ref from bash-completion.
-BashComplete.source_template = """\
-    %(complete_func)s() {
-        if [[ $(type -t __reassemble_comp_words_by_ref) != function ]]; then
-            return -1
-        fi
-        local cword words=()
-        __reassemble_comp_words_by_ref ":" words cword
-        local IFS=$'\\n'
-        response=$(env COMP_WORDS="${words[*]}" COMP_CWORD="$cword" %(complete_var)s=bash_complete $1)
-        for completion in $response; do
-            IFS=',' read type value <<< "$completion"
-            case $type in
-            dir) COMPREPLY=(); compopt -o dirnames; ;;
-            file) COMPREPLY=(); compopt -o default; ;;
-            plain) COMPREPLY+=($value); ;;
-            nospace) compopt -o nospace; ;;
-            esac
-        done
-    }
-    %(complete_func)s_setup() {
-        complete -o nosort -F %(complete_func)s %(prog_name)s
-    }
-    %(complete_func)s_setup;
-"""
 
+class NomadOrHostMyPath(click.ParamType):
+    """Click parameter representing Nomad or host path"""
 
-###############################################################################
+    name = "path"
 
+    def convert(
+        self, value: Any, param: Optional[click.Parameter], ctx: Optional[click.Context]
+    ) -> Mypath:
+        """Entrypoint for click option conversion"""
+        return value if isinstance(value, Mypath) else ArgPath.mk(value).to_mypath()
 
-def pipe(cmda: str, cmdb: str):
-    """Run a pipe of cmda | cmdb"""
-    arra = shlex.split(cmda)
-    arrb = shlex.split(cmdb)
-    log.debug(f"+ {quotearr(arra)} | {quotearr(arrb)}")
-    with subprocess.Popen(arrb, stdin=subprocess.PIPE) as ps:
-        subprocess.check_call(arra, stdin=subprocess.PIPE, stdout=ps.stdin)
-    if ps.returncode:
-        raise subprocess.CalledProcessError(ps.returncode, ps.args)
+    def shell_complete(
+        self, ctx: click.Context, param: click.Parameter, incomplete: str
+    ) -> List[CompletionItem]:
+        try:
+            return ArgPath.mk(incomplete).gen_shell_complete()
+        except Exception as e:
+            ArgPath.debugexception(e)
+        return []
 
 
-def run(cmd: str):
-    """Run a command"""
-    log.debug(f"+ {cmd}")
-    subprocess.check_call(shlex.split(cmd), stdin=subprocess.DEVNULL)
+###############################################################################
 
 
 def nomadpipe(src: Mypath, dst: Mypath, srccmd: str, dstcmd: str):
-    with src.popen(srccmd, stdout=subprocess.PIPE) as srcp:
-        with dst.popen(dstcmd, stdin=subprocess.PIPE) as dstp:
-            shutil.copyfileobj(srcp.stdout, dstp.stdin)
-    for p in [srcp, dstp]:
-        if p.returncode:
-            raise subprocess.CalledProcessError(p.returncode, p.cmd)
+    stats: bool = (ARGS.stats is None and sys.stderr.isatty()) or ARGS.stats is True
+    with dst.popen(dstcmd, stdin=subprocess.PIPE) as pdst:
+        assert pdst.stdin
+        if stats:
+            with src.popen(srccmd, stdout=subprocess.PIPE) as psrc:
+                assert psrc.stdout
+                transfer_stats(psrc.stdout.fileno(), pdst.stdin.fileno(), ARGS.pv)
+        else:
+            with src.popen(srccmd, stdout=pdst.stdin.fileno()) as psrc:
+                pass
+
+
+def tar_out_opt() -> str:
+    return (
+        ("z" if ARGS.gzip else "")
+        + ("j" if ARGS.bzip2 else "")
+        + ("J" if ARGS.xz else "")
+    )
 
 
-def get_tar_x_opt():
+def tar_in_opt() -> str:
     return (
+        tar_out_opt()
         # If dryrun, pass vt to print to stdout.
-        ("vt" if args.dryrun else "x")
-        + ("v" if args.verbose else "")
+        + ("vt" if ARGS.dryrun else "x")
+        + ("v" if ARGS.verbose else "")
         # If archive, pass p to preserve permissions when not root.
         # If not archive, pass o to do not preserve permissions even as root.
         # See tar docs.
-        + ("p" if args.archive else "o")
+        + ("p" if ARGS.archive else "o")
     )
 
 
 def nomadtarpipe(src: Mypath, dst: Mypath, tar_c: str, tar_x: str):
-    global args
-    x = get_tar_x_opt()
-    nomadpipe(src, dst, f"tar -cf - {tar_c}", f"tar -{x}f - {tar_x}")
+    nomadpipe(
+        src,
+        dst,
+        f"tar -c{tar_out_opt()}f - {tar_c}",
+        f"tar -{tar_in_opt()}f - {tar_x}",
+    )
 
 
 def copy_mode(src: Mypath, dst: Mypath):
     # logic from https://docs.docker.com/engine/reference/commandline/cp/
     # SRC_PATH specifies a file
     if src.is_file():
         # DEST_PATH does not exist and ends with /
@@ -526,37 +638,48 @@
             not dst.exists()
             # DEST_PATH exists and is a file
             # the destination is overwritten with the source file’s contents
             or dst.is_file()
         ):
             # Copy one file.
             log.info(f"File {src} -> {dst}")
+            prog: Optional[str] = (
+                "gzip"
+                if ARGS.gzip
+                else "xz"
+                if ARGS.xz
+                else "bzip2"
+                if ARGS.bzip2
+                else None
+            )
+            srcscript: str = f"{prog} -c" if prog else "cat"
+            dstscript: str = f"{prog} -d" if prog else "cat"
             nomadpipe(
                 src,
                 dst,
-                f"cat {src.quotepath()}",
-                f"sh -c 'cat >\"$1\"' sh {dst.quotepath()}"
-                if not args.dryrun
-                else f"true -- {dst.quotepath()}",
+                f"{srcscript} {src.quotepath()}",
+                "sh -c " + quote(f"{dstscript} >{dst.quotepath()}")
+                if not ARGS.dryrun
+                else f"true -- {quote(dstscript)} {dst.quotepath()}",
             )
         else:
             exit(f"Not a file or directory: {dst}")
     # SRC_PATH specifies a directory
     elif src.is_dir():
         # DEST_PATH does not exist
         if not dst.exists():
             # DEST_PATH is created as a directory and the contents of the source directory are copied into this directory
             log.info(f"New mkdir {src} -> {dst}")
-            if not args.dryrun:
-                log.debug(f"mkdir {dst}")
+            log.debug(f"mkdir {dst}")
+            if not ARGS.dryrun:
                 dst.mkdir()
             tar_c = f"-C {src.quotepath()} ."
             # And unpack to parent directory.
-            components: int = str(src.path).count("/")
-            tar_x = f"-C {dst.quoteparent()} --strip-components={components}"
+            components: int = src.path.count("/")
+            tar_x = f"-C {dst.quotepath()} --strip-components={components}"
             nomadtarpipe(src, dst, tar_c, tar_x)
         # DEST_PATH exists and is a file
         elif dst.is_file():
             exit("Error condition: cannot copy a directory to a file")
         # DEST_PATH exists and is a directory
         elif dst.is_dir():
             # SRC_PATH does not end with /. (that is: slash followed by dot)
@@ -579,126 +702,132 @@
         exit(f"Not a file or directory: {src}")
 
 
 def stream_mode(src: Mypath, dst: Mypath):
     # One of source or dest is a -
     if src.isstdin():
         log.info(f"Stream stdin -> {dst}")
-        assert dst.isstdin(), "Both operands are '-'"
-        x = get_tar_x_opt()
-        dst.run(f"tar -{x}f - -C {dst.quotepath()}")
+        assert not dst.isstdin(), f"Both operands are '-': {src} {dst}"
+        with dst.popen(
+            f"tar -{tar_in_opt()}f - -C {dst.quotepath()}",
+            stdin=sys.stdin.fileno(),
+        ):
+            pass
     elif dst.isstdin():
         log.info(f"Stream {src} -> stdout")
-        src.run(f"tar -cf - -C {src.quoteparent()} -- {src.quotename()}")
+        with src.popen(
+            f"tar -c{tar_out_opt()}f - -C {src.quoteparent()} -- {src.quotename()}",
+            stdout=sys.stdout.fileno(),
+        ):
+            pass
     else:
         assert 0, "Internal error - neither source nor dest is equal to -"
 
 
-def test(ctx, param, value):
-    if not value or ctx.resilient_parsing:
-        return
-    script = """
-        set -xeuo pipefail
-        cmd="$1"
-        cmd() { python -m nomad_tools.nomad_cp -vv "$@"; }
-        tmpd=$(mktemp -d)
-        trap 'rm -vrf "$tmpd"' EXIT
-        mkdir "$tmpd/src" "$tmpd/dst"
-        echo 123 > "$tmpd/src/1"
-
-        echo "testing file copy without destination"
-        cmd "$tmpd/src/1" "$tmpd/dst"
-        test -e "$tmpd/dst/1"
-        rm -v "$tmpd/dst/1"
-
-        echo "tesing file copy to a different file"
-        cmd "$tmpd/src/1" "$tmpd/dst/2"
-        test -e "$tmpd/dst/2"
-        rm -v "$tmpd/dst/2"
-
-        echo "testing dir copy to a dir"
-        cmd "$tmpd/src" "$tmpd/dst"
-        test -e "$tmpd/dst/src/1"
-        rm -vr "$tmpd/dst/src"
-
-        echo "testing content of a dir copy to a dir"
-        cmd "$tmpd/src/." "$tmpd/dst"
-        test -e "$tmpd/dst/1"
-        rm -v "$tmpd/dst/1"
-        """
-    subprocess.check_call(
-        [
-            "bash",
-            "-c",
-            script,
-            "--",
-            sys.argv[0],
-        ]
-    )
-    ctx.exit()
+def rsync_mode(src: Mypath, dst: Mypath):
+    assert not src.isstdin()
+    assert not dst.isstdin()
+    if isinstance(src, NomadMypath):
+        srcn = True
+        npath = src
+    elif isinstance(dst, NomadMypath):
+        srcn = False
+        npath = dst
+    else:
+        assert False, "One of SOURCE and DEST can be Nomad path"
+    rsh = f"nomad alloc exec -t=false -i=true -task={quote(npath.task)} {quote(npath.allocation)}"
+    srcp = (":" if srcn else "") + src.quotepath().replace(":", r"\:")
+    dstp = ("" if srcn else ":") + dst.quotepath().replace(":", r"\:")
+    cmd = f"rsync {ARGS.rsyncargs} --rsh={quote(rsh)} {srcp} {dstp}"
+    log.debug(f"+ {quotearr(split(cmd))}")
+    if not ARGS.dryrun:
+        subprocess.check_call(split(cmd))
 
 
 ###############################################################################
 
 
+@dataclass
+class Args:
+    gzip: bool = clickdc.option("-z", help="Pass -z to tar")
+    xz: bool = clickdc.option("-J", help="Pass -J to tar")
+    bzip2: bool = clickdc.option("-j", help="Pass -j to tar")
+    archive: bool = clickdc.option(
+        "-a",
+        help="Archive mode (copy all uid/gid information)",
+    )
+    #
+    rsync: bool = clickdc.option(help="Rsync two paths")
+    rsyncargs: str = clickdc.option(help="Shell quoted rsync options", default="")
+    #
+    pv: Optional[bool] = clickdc.option(
+        "--pv/--no-pv",
+        help="Use pv to show statistics. By default, if pv is available, it will be used.",
+        default=None,
+    )
+    stats: Optional[bool] = clickdc.option(
+        "--stats/--no-stats",
+        help="Display statistics. By default, if stderr is a terminal, stats will be shown.",
+        default=None,
+    )
+    #
+    dryrun: bool = clickdc.option(
+        "-n",
+        help="Do tar -vt for unpacking. Usefull for listing files for debugging.",
+    )
+    verbose: int = clickdc.option("-v", "--verbose", count=True)
+    quiet: int = clickdc.option("-q", "--quiet", count=True)
+    source: Mypath = clickdc.argument(type=NomadOrHostMyPath())
+    dest: Mypath = clickdc.argument(type=NomadOrHostMyPath())
+
+
 @click.command(
+    "cp",
     help=f"""
 Copy files/folders between a nomad allocation and the local filesystem.
 Use '-' as the source to read a tar archive from stdin
 and extract it to a directory destination in a container.
 Use '-' as the destination to stream a tar archive of a
 container source to stdout.
 The logic mimics docker cp.
 
 \b
 Both source and dest take one of the forms:
-{textwrap.indent(NomadOrHostMyPath._description, '   ')}
+{textwrap.indent(ArgPath._description, '   ')}
 
 To use colon in any part of the path, escape it with backslash.
 
 \b
 Examples:
-    nomad-cp -n :9190d781:/tmp ~/tmp
-    nomad-cp -vn -Nservices promtail:/. ~/tmp
+    nomad-tools cp -n :9190d781:/tmp ~/tmp
+    nomad-tools cp -vn -Nservices promtail:/. ~/tmp
 """,
     epilog="""
 Written by Kamil Cukrowski 2023. Licensed under GNU GPL version or later.
 """,
 )
-@click.option(
-    "-n",
-    "--dryrun",
-    is_flag=True,
-    help="Do tar -vt for unpacking. Usefull for listing files for debugging.",
-)
-@click.option("-v", "--verbose", count=True)
-@namespace_option()
-@click.option(
-    "-a",
-    "--archive",
-    is_flag=True,
-    help="Archive mode (copy all uid/gid information)",
-)
-@click.option("--test", is_flag=True, help="Run tests", is_eager=True, callback=test)
-@click.argument("source", type=NomadOrHostMyPath())
-@click.argument("dest", type=NomadOrHostMyPath())
 @namespace_option()
 @common_options()
-def cli(source: Mypath, dest: Mypath, **kwargs):
-    global args
-    args = argparse.Namespace(**kwargs)
+@clickdc.adddc("args", Args)
+def cli(args: Args):
+    global ARGS
+    ARGS = args
+    verbose = 1 + ARGS.verbose - ARGS.quiet
     logging.basicConfig(
         level=logging.DEBUG
-        if args.verbose > 1
+        if verbose > 1
         else logging.INFO
-        if args.verbose > 0
+        if verbose > 0
         else logging.WARNING,
         format="%(levelname)s %(name)s:%(funcName)s:%(lineno)d: %(message)s",
     )
-    if source.isstdin() or dest.isstdin():
-        stream_mode(source, dest)
+    log.debug(f"ARGS={ARGS}")
+    if ARGS.rsync:
+        rsync_mode(ARGS.source, ARGS.dest)
+    elif ARGS.source.isstdin() or ARGS.dest.isstdin():
+        stream_mode(ARGS.source, ARGS.dest)
     else:
-        copy_mode(source, dest)
+        copy_mode(ARGS.source, ARGS.dest)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `nomad-tools-0.2.4/src/nomad_tools/nomad_dockers.py` & `nomad_tools-0.3.0/src/nomad_tools/nomad_dockers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import json
 import logging
 import shlex
 import subprocess
 import sys
-from typing import IO, Any, Dict, List
+from dataclasses import dataclass
+from typing import IO, Any, Dict, List, Tuple
 
 import click.shell_completion
+import clickdc
 
 from . import common, nomadlib
-from .common_click import alias_option
 
 log = logging.getLogger(__name__)
 
 
 def complete_job(
     ctx: click.Context, param: click.Parameter, incomplete: str
 ) -> List[click.shell_completion.CompletionItem]:
@@ -42,83 +43,83 @@
             cmd = "nomad job run -output -"
             log.debug(f"+ {cmd}")
             content = subprocess.check_output(cmd.split(), input=content, text=True)
         jobdata = json.loads(content)
     return nomadlib.Job(jobdata.get("Job", jobdata))
 
 
+@dataclass
+class Args:
+    verbose: int = clickdc.option("-v", count=True, help="Be verbose")
+    format: str = clickdc.option(
+        "-f",
+        help="Passed to python .format()",
+        show_default=True,
+        default="{image}",
+    )
+    long: Any = clickdc.alias_option(
+        "-l",
+        aliased=dict(format="{groupName} {taskName} {image}"),
+    )
+    job: Tuple[str, ...] = clickdc.option(
+        "-j",
+        multiple=True,
+        help="List images referenced by a Nomad job name",
+    )
+    all: Tuple[str, ...] = clickdc.option(
+        "-a",
+        multiple=True,
+        help="NextList docker images referenced by all job versions",
+    )
+    files: Tuple[IO, ...] = clickdc.argument("files", nargs=-1, type=click.File("r"))
+
+
 @click.command(
+    "dockers",
     help="""
     List all docker images referenced by a Nomad job.
     Typically used to download or test the images like
-    nomad-dockers ./file.nomad.hcl | xargs docker pull.
-    """
+    `nomadtools dockers ./file.nomad.hcl | xargs docker pull`.
+    """,
 )
 @common.common_options()
-@click.option("-v", "--verbose", count=True, help="Be verbose")
-@click.option(
-    "-f",
-    "--format",
-    help="Passed to python .format()",
-    show_default=True,
-    default="{image}",
-)
-@alias_option(
-    "-l",
-    "--long",
-    aliased=dict(format="{groupName} {taskName} {image}"),
-)
-@click.option(
-    "-j",
-    "--job",
-    multiple=True,
-    help="List images referenced by a Nomad job name",
-)
-@click.option(
-    "-a",
-    "--all",
-    multiple=True,
-    help="NextList docker images referenced by all job versions",
-)
-@click.argument("files", nargs=-1, type=click.File("r"))
-def cli(
-    all: List[str], files: List[IO], job: List[str], format: str, verbose: int, **kwargs
-):
-    logging.basicConfig(level=logging.DEBUG if verbose else logging.INFO)
-    if not (all or files or job):
+@clickdc.adddc("args", Args)
+def cli(args: Args):
+    logging.basicConfig(level=logging.DEBUG if args.verbose else logging.INFO)
+    if not (args.all or args.files or args.job):
         raise click.ClickException(
             "One of --all --job or positional arguments have to given"
         )
     njobs: List[nomadlib.Job] = []
     njobs += [
         nomadlib.Job(njobversion)
-        for job in all
+        for job in args.all
         for njobversion in common.mynomad.get(
             f"job/{common.nomad_find_job(job)}/versions"
         )["Versions"]
     ]
     njobs += [
         nomadlib.Job(common.mynomad.get(f"job/{common.nomad_find_job(job)}"))
-        for job in job
+        for job in args.job
     ]
-    njobs += [load_job_file(file) for file in files]
+    njobs += [load_job_file(file) for file in args.files]
     for njob in njobs:
         out: List[str] = []
         for group in njob.TaskGroups or []:
             for task in group.Tasks or []:
                 image = task.Config.get("image")
                 if image and task.Driver == "docker":
                     params: Dict[str, Any] = dict(
                         groupName=group.Name,
                         taskName=task.Name,
                         jobVersion=njob.Version,
                         image=image,
                     )
                     log.debug(f"{format!r} {params}")
-                    out.append(format.format(**params))
+                    out.append(args.format.format(**params))
         out = sorted(list(set(out)))
         for line in out:
             print(line)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `nomad-tools-0.2.4/src/nomad_tools/nomad_downloadrelease.py` & `nomad_tools-0.3.0/src/nomad_tools/nomad_downloadrelease.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,21 +33,22 @@
 def get_arch() -> str:
     if platform.machine() in ["AMD64", "x86_64"]:
         return "amd64"
     return ""
 
 
 @click.command(
+    "downloadrelease",
     help="""
 \b
 Download specific binary from releases.hashicorp
 Examples:
     %(prog) -p 1.7.2 nomad ./bin/nomad
     %(prog) consul ./bin/consul
-"""
+""",
 )
 @click.option("--verbose", is_flag=True)
 @click.option(
     "-p", "--pinversion", help="Use this version instead of autodetecting latest"
 )
 @click.option(
     "--os",
```

### Comparing `nomad-tools-0.2.4/src/nomad_tools/nomad_gitlab_runner/script.sh` & `nomad_tools-0.3.0/src/nomad_tools/nomad_gitlab_runner/script.sh`

 * *Files identical despite different names*

### Comparing `nomad-tools-0.2.4/src/nomad_tools/nomad_gitlab_runner/waiter.sh` & `nomad_tools-0.3.0/src/nomad_tools/nomad_gitlab_runner/waiter.sh`

 * *Files identical despite different names*

### Comparing `nomad-tools-0.2.4/src/nomad_tools/nomad_gitlab_runner.py` & `nomad_tools-0.3.0/src/nomad_tools/nomad_gitlab_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import string
 import sys
 import tempfile
 from collections import defaultdict
 from pathlib import Path
 from shlex import quote, split
 from textwrap import dedent
-from typing import Dict, List, Optional, Union
+from typing import Callable, Dict, List, Optional, Union
 
 import click
 import yaml
 
 from . import nomad_watch, nomadlib, taskexec
 from .common import (
     cached_property,
@@ -138,33 +138,33 @@
     builds_dir: str = "/alloc/builds"
     cache_dir: str = "/alloc/cache"
     builds_dir_is_shared: Optional[bool] = False
     image: str = "alpine:latest"
     """The image to run jobs with."""
     volumes: List[str] = []
     """https://developer.hashicorp.com/nomad/docs/drivers/docker#volumes
-    The default mounts /certs to ../alloc to have it available for docker dind sevice just like in gitlab-runner."""
+    The default mounts ${NOMAD_ALLOD_DIR} to /certs to have it available for docker dind sevice just like in gitlab-runner."""
     wait_for_services_timeout: int = 30
     """How long to wait for Docker services. Set to -1 to disable. Default is 30."""
     privileged: bool = False
     """Make the container run in privileged mode. Insecure."""
     services_privileged: Optional[bool] = None
     """Allow services to run in privileged mode. If unset (default) privileged value is used instead.
     Use with the Docker executor. Insecure."""
     force_pull: bool = True
     """https://developer.hashicorp.com/nomad/docs/drivers/docker#force_pull"""
-    waiter_image: str = "docker:24.0.6-cli"
+    waiter_image: str = "docker:25.0.3-cli"
     """A image with POSIX sh and docker that waits for services to have open ports"""
-    helper_image: str = "gitlab/gitlab-runner:alpine-v16.3.1"
+    helper_image: str = "gitlab/gitlab-runner:alpine-v16.9.1"
     """(Advanced) The default helper image used to clone repositories and upload artifacts."""
     auto_fix_docker_dind: bool = True
     """
     If there is a service aliased "docker" and DOCKER_TLS_CERTDIR is set to exactly "/certs"
     and DOCKER_CERT_PATH, DOCKER_HOST nor DOCKER_TLS_VERIFY are not set, then:
-    automatically mount volume "../alloc:/certs"
+    automatically mount volume "${NOMAD_ALLOC_DIR}:/certs"
     and add following environment variables:
         DOCKER_CERT_PATH="/certs/client"
         DOCKER_HOST=tcp://docker:2376
         DOCKER_TLS_CERTDIR=/certs
         DOCKER_TLS_VERIFY=1
     This automatically properly handles the environment variables with docker like in plain gitlab-runner.
     See also https://docs.gitlab.com/ee/ci/docker/using_docker_build.html#docker-in-docker-with-tls-enabled-in-kubernetes
@@ -247,15 +247,14 @@
             {
                 "Name": s.alias,
                 "Driver": "docker",
                 "Config": {
                     "image": s.name,
                     **({"entrypoint": s.entrypoint} if s.entrypoint else {}),
                     **({"args": s.command} if s.command else {}),
-                    "network_aliases": [s.alias],
                     "privileged": (
                         self.services_privileged
                         if self.services_privileged is not None
                         else self.privileged
                     ),
                 },
                 "Env": get_CUSTOM_ENV(),
@@ -315,22 +314,23 @@
                         {
                             "DOCKER_CERT_PATH": "/certs/client",
                             "DOCKER_HOST": "tcp://docker:2376",
                             "DOCKER_TLS_VERIFY": "1",
                         }
                     )
             # Volumes handled below.
-            self.volumes += ["../alloc:/certs"]
+            self.volumes += ["${NOMAD_ALLOC_DIR}:/certs"]
         for task in taskgroup.Tasks:
             taskconfig = task["Config"]
             # Apply cpuset_cpus
             if config.cpuset_cpus:
                 taskconfig["cpuset_cpus"] = config.cpuset_cpus
             # Apply volumes.
-            taskconfig.setdefault("volumes", []).extend(self.volumes)
+            if self.volumes:
+                taskconfig.setdefault("volumes", []).extend(self.volumes)
 
     def get_task_for_stage(self, stage: str) -> str:
         return (
             main_task_name
             if stage.startswith("step_") or stage.startswith("build_")
             else self.get_helper_task().Name
         )
@@ -545,15 +545,15 @@
     except SystemExit as e:
         if not (e.code is None or e.code == 0):
             raise
 
 
 def purge_previous_nomad_job(jobname: str):
     try:
-        jobdata = mynomad.get("job/{jobname}")
+        jobdata = mynomad.get(f"job/{jobname}")
     except nomadlib.JobNotFound:
         return
     job = Job(jobdata["Job"])
     assert (
         job.Stop is True or job.Status == "dead"
     ), f"Job {job.description()} already exists and is not stopped or not dead. Bailing out"
     run_nomad_watch(f"--purge -xn0 stop {quote(jobname)}")
@@ -652,14 +652,15 @@
     """Raising this exception makes the code exit with BUILD_FAILURE_EXIT_CODE"""
 
     code: int = 76
     """Special chosen exit status returned by script.sh that the build script has failed."""
 
 
 @click.group(
+    "gitlab-runner",
     help=""" Custom gitlab-runner executor to run gitlab-ci jobs in Nomad. """,
     epilog="Written by Kamil Cukrowski 2023. Licensed under GNU GPL version or later.",
 )
 @click.option("-v", "--verbose", count=True)
 @click.option(
     "-c",
     "--config",
@@ -701,17 +702,35 @@
     log.debug(f"+ {sys.argv}")
     #
     dc = config.get_driverconfig
     if dc.get("image"):
         os.environ.setdefault("CUSTOM_ENV_CI_JOB_IMAGE", dc["image"])
 
 
+def executor_exit(f: Callable) -> Callable:
+    """Custom executor should always exit with specific exit codes"""
+
+    def executor_exiting(*args, **kvargs):
+        try:
+            f(*args, **kvargs)
+        except BuildFailure:
+            log.debug("build failure")
+            exit(int(os.environ.get("BUILD_FAILURE_EXIT_CODE", BuildFailure.code)))
+        except Exception as e:
+            log.exception(e)
+            exit(int(os.environ.get("SYSTEM_FAILURE_EXIT_CODE", 111)))
+        return 0
+
+    return executor_exiting
+
+
 @cli.command(
     "config", help="https://docs.gitlab.com/runner/executors/custom.html#config"
 )
+@executor_exit
 def mode_config():
     dc = config.get_driverconfig
     driver_config = {
         "builds_dir": dc.builds_dir,
         "cache_dir": dc.cache_dir,
         "builds_dir_is_shared": dc.builds_dir_is_shared,
         "hostname": socket.gethostname(),
@@ -726,28 +745,31 @@
     log.debug(f"driver_config={driver_config_json}")
     click.echo(driver_config_json)
 
 
 @cli.command(
     "prepare", help="https://docs.gitlab.com/runner/executors/custom.html#prepare"
 )
+@executor_exit
 def mode_prepare():
     # print_env()
     je = Jobenv()
     purge_previous_nomad_job(je.jobname)
     jobjson = json.dumps({"Job": je.job.asdict()})
+    log.debug(f"JOBJSON: {jobjson}")
     with tempfile.NamedTemporaryFile("w+") as f:
         f.write(jobjson)
         f.flush()
-        run_nomad_watch(f"start -json {f.name}")
+        run_nomad_watch(f"--json start {f.name}")
 
 
 @cli.command("run", help="https://docs.gitlab.com/runner/executors/custom.html#run")
 @click.argument("script")
 @click.argument("stage")
+@executor_exit
 def mode_run(script: str, stage: str):
     je = Jobenv()
     set_x = "-x" if config.verbose > 1 else ""
     # Execute all except step_ and build_ in that special gitlab docker container.
     taskname = config.get_driverconfig.get_task_for_stage(stage)
     # Find our running allocation.
     allocid = taskexec.find_job_alloc(je.jobname, taskname)
@@ -768,14 +790,15 @@
     else:
         rr.check_returncode()
 
 
 @cli.command(
     "cleanup", help="https://docs.gitlab.com/runner/executors/custom.html#cleanup"
 )
+@executor_exit
 def mode_cleanup():
     je = Jobenv()
     run_nomad_watch(
         f" {'--purge' if config.purge else ''}"
         f" {'--purge-successful' if config.purge_successful and config.purge is None else ''}"
         f" -x -n0 stop {quote(je.jobname)}"
     )
@@ -803,23 +826,9 @@
     print()
     print("--- program configuration: ---")
     print(yaml.dump(config.asdict()))
 
 
 ###############################################################################
 
-
-def main(*args, **kvargs) -> int:
-    """Custom executor should always exit with specific exit codes"""
-    try:
-        cli.main(*args, **kvargs)
-    except BuildFailure:
-        log.debug("build failure")
-        return int(os.environ.get("BUILD_FAILURE_EXIT_CODE", BuildFailure.code))
-    except Exception as e:
-        log.exception(e)
-        return int(os.environ.get("SYSTEM_FAILURE_EXIT_CODE", 111))
-    return 0
-
-
 if __name__ == "__main__":
-    exit(main())
+    cli()
```

### Comparing `nomad-tools-0.2.4/src/nomad_tools/nomad_port.py` & `nomad_tools-0.3.0/src/nomad_tools/nomad_port.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 
 
 default_format = "{host}:{port}"
 long_format = "{host} {port} {label} {Name} {ID}"
 
 
 @click.command(
+    "port",
     help="""
 Print dynamic ports allocated by Nomad for a specific job or allocation.
 If no ports are found, exit with 2 exit status.
 If label argument is given, outputs only redirects which label is equal to given label.
 
 \b
 The following variables are available for --format option:
@@ -95,15 +96,15 @@
 And any other key from Nomad allocation API definition which value is a string or a number.
 
 \b
 Exits with the following exit status:
   0  if at least one redirection was found,
   1  on python exception, missing job,
   2  if no redirections were found.
-"""
+""",
 )
 @click.option(
     "-f",
     "--format",
     default=default_format,
     help=f"The template used to format output. Templated with python .format() function. [default: {default_format!r}]",
 )
```

### Comparing `nomad-tools-0.2.4/src/nomad_tools/nomad_smart_start_job.py` & `nomad_tools-0.3.0/src/nomad_tools/nomad_smart_start_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import subprocess
 import sys
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Optional, TextIO, Tuple, Union
 
 from .common import mynomad
+from .nomadlib.connection import JobSubmission
 
 log = logging.getLogger(__name__)
 
 ###############################################################################
 
 
 def nomad_job_run(
@@ -67,18 +68,18 @@
 
 
 ###############################################################################
 
 
 @dataclasses.dataclass
 class Detail(ABC):
-    # The actual inputed string from the user.
     input: str
-    # This is true, we know that content is a JSON.
+    """The actual inputed string from the user."""
     forcejson: bool
+    """This is true, we know that content is a JSON."""
 
     @abstractmethod
     def seekable_read(self) -> Optional[str]:
         """Read the content of the file only if it is seekable."""
         raise NotImplementedError()
 
     def read(self) -> str:
@@ -118,29 +119,33 @@
         return nomad_job_run(
             file=file,
             isjson=self.seekable_isjson(),
             stdin=stdin,
             input=input,
         )
 
-    def read_dict(self) -> Tuple[str, dict]:
+    def read_dict(self) -> Tuple[str, str, dict]:
         content = self.read()
         # Assume input is a string with valid job specification.
         try:
             # try json
             data = json.loads(content)
+            format = "json"
         except json.JSONDecodeError:
             if self.forcejson:
                 raise
             data = json.loads(mynomad.jobhcl2json(content))
-        return content, data
+            format = "hcl2"
+        return content, format, data
 
     def api_start(self):
-        content, data = self.read_dict()
-        evalid = mynomad.start_job(data, content)["EvalID"]
+        content, format, data = self.read_dict()
+        evalid = mynomad.start_job(data, JobSubmission(Source=content, Format=format))[
+            "EvalID"
+        ]
         return evalid
 
     def run(self) -> str:
         return self.nomad_start() if shutil.which("nomad") else self.api_start()
 
 
 @dataclasses.dataclass
```

### Comparing `nomad-tools-0.2.4/src/nomad_tools/nomad_vardir.py` & `nomad_tools-0.3.0/src/nomad_tools/nomad_vardir.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,19 @@
         #
         if newitems == olditems:
             log.info(f"No changes in {VAR.desc()}")
         else:
             cas: Optional[int] = (
                 check_index
                 if check_index is not None
-                else None if force else oldvar.ModifyIndex if oldvar else 0
+                else None
+                if force
+                else oldvar.ModifyIndex
+                if oldvar
+                else 0
             )
             if newitems:
                 log.info(
                     f"Putting var {VAR.desc()} with keys: {dict_keys_str(newitems)}"
                 )
                 try:
                     VAR.put(newitems, cas)
@@ -368,14 +372,15 @@
 def click_vardir_paths(required: bool = False):
     return click_vardir_keys(
         required=required, name="paths", type=click.Path(path_type=Path, exists=False)
     )
 
 
 @click.group(
+    "vardir",
     help="""
 This is a solution for managing Nomad variables as directories and files.
 Single Nomad variable can be represented as a directory.
 Each file inside the directory represent a JSON key inside the Nomad variable.
 This tool can update and edit the keys in Nomad variables as files.
 
 \b
@@ -384,15 +389,15 @@
    - for example an `nginx.conf` configuration,
 - write a makefile that will generate the `nginx.conf` from the template using consul-template,
 - use this script on the directory containing generated `nginx.conf` to upload it to Nomad variables.
 """,
     epilog="""
 \b
 Examples:
-    nomad-vardir nomad/jobs/nginx@nginx get nginx.conf
+     nomad/jobs/nginx@nginx get nginx.conf
     nomad-vardir -j nginx@nginx ls
     nomad-vardir -j nginx@nginx put ./nginx.conf
     nomad-vardir -j nginx@nginx cat ./nginx.conf
     nomad-vardir -j nginx@nginx get ./nginx.conf
     nomad-vardir -j nginx@nginx diff
     nomad-vardir -j nginx@nginx rm ./nginx.conf
```

### Comparing `nomad-tools-0.2.4/src/nomad_tools/nomad_watch.py` & `nomad_tools-0.3.0/src/nomad_tools/nomad_watch.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 from __future__ import annotations
 
 import argparse
 import base64
+import contextlib
 import datetime
 import enum
 import inspect
 import itertools
 import json
 import logging
 import os
@@ -18,36 +19,37 @@
 import subprocess
 import sys
 import threading
 import time
 import traceback
 from abc import ABC, abstractmethod
 from dataclasses import asdict, dataclass, field
-from http import client as http_client
 from typing import (
     Any,
+    Callable,
     ClassVar,
     Dict,
     Iterator,
     List,
     Optional,
     Pattern,
     Set,
     Tuple,
     TypeVar,
 )
 
 import click
+import clickdc
 import requests
 from click.shell_completion import CompletionItem
 from typing_extensions import override
 
 from . import colors, exit_on_thread_exception, flagdebug, nomaddbjob, nomadlib
 from .common_base import andjoin, cached_property, composed, eprint
-from .common_click import alias_option, common_options, complete_set_namespace
+from .common_click import common_options, complete_set_namespace
 from .common_nomad import (
     NoJobFound,
     complete_job,
     completor,
     mynomad,
     namespace_option,
     nomad_find_job,
@@ -59,15 +61,15 @@
 log = logging.getLogger(__name__)
 
 ###############################################################################
 
 ARGS = argparse.Namespace()
 """Arguments passed to this program"""
 
-START_NS: int = 0
+START_S: float = 0
 """This program start time, assigned from cli()"""
 
 COLORS = colors.init()
 
 DB: NomadDbJob
 """Database listening to Nomad stream"""
 
@@ -188,247 +190,389 @@
 class LOGFORMAT:
     """Logging output format specification templates using f-string. Very poor mans templating langauge."""
 
     pre = "{color}{now.strftime(args.log_time_format) + '>' if ARGS.log_time else ''}"
     mark = "{mark}>"
     post = "{message}{reset}"
     task = "{task + '>' if task else ''}"
+
     DEFAULT = (
         pre + mark + "{id:.{args.log_id_len}}>v{str(jobversion)}>" + task + " " + post
     )
     """
     Default log format. The log is templated with f-string using eval() below.
         O>45fbbd>v0>group1>task1> hello world
     """
+
     ONE = pre + mark + task + " " + post
     """
     Log format with -1 option.
         O>task1> hello world
     """
+
+    ONLYMARK = pre + mark + post
+    """ O>hello world """
+
     ZERO = pre + post
     """
     Log format with -0 option.
         hello world
     """
+
     LOGGING = (
         COLORS.brightblue
         + "{'%(asctime)s>' if ARGS.log_time else ''}"
-        + "{'nomad-watch' if ARGS.verbose <= 0 else '%(module)s'}>"
+        + "{'watch' if ARGS.verbose <= 0 else '%(module)s'}>"
         + "%(lineno)03d>"
         + " %(levelname)s %(message)s"
         + COLORS.reset
     )
     """Logging format, first templated with f-string, then by logging."""
-    colors: Dict[LogWhat, str] = {
+
+    colors: Dict[str, str] = {
         LogWhat.deploy: COLORS.brightmagenta,
         LogWhat.eval: COLORS.magenta,
         LogWhat.alloc: COLORS.cyan,
         LogWhat.stderr: COLORS.orange,
         LogWhat.stdout: "",
     }
     """Logs colors"""
-    marks: Dict[LogWhat, str] = {
+
+    marks: Dict[str, str] = {
         LogWhat.deploy: "deploy",
         LogWhat.eval: "eval",
         LogWhat.alloc: "A",
         LogWhat.stderr: "E",
         LogWhat.stdout: "O",
     }
     """Logs marks"""
 
     @staticmethod
     def render(fmt: str, **kwargs) -> str:
         locals().update(kwargs)
         return eval(f"f{fmt!r}")
 
 
-def click_log_options():
-    """All logging options"""
-    return composed(
-        click.option(
-            "-T",
-            "--log-time",
-            is_flag=True,
-            help="""
-                Additionally add timestamp to the logs.
-                The timestamp of stdout and stderr streams is when the log was received,
-                as Nomad does not store timestamp of task logs.
-                """,
-        ),
-        click.option(
-            "--log-time-format",
-            default="%Y-%m-%dT%H:%M:%S%z",
-            show_default=True,
-            help="Format time with specific format. Passed to python datetime.strftime.",
-        ),
-        alias_option(
-            "-H",
-            "--log-time-hour",
-            aliased=dict(
-                log_time_format="%H:%M:%S",
-                log_time=True,
-            ),
-        ),
-        click.option(
-            "--log-format",
-            default=LOGFORMAT.DEFAULT,
-            show_default=True,
-            help="The format to use when printing job logs",
-        ),
-        click.option(
-            "--log-id-len",
-            default=6,
-            help="The length of id to log. UUIDv4 has 36 characters.",
-        ),
-        alias_option(
-            "-l",
-            "--log-id-long",
-            aliased=dict(log_id_len=36),
-        ),
-        alias_option(
-            "-1",
-            "--log-only-task",
-            aliased=dict(log_format=LOGFORMAT.ONE),
-        ),
-        alias_option(
-            "-0",
-            "--log-none",
-            aliased=dict(log_format=LOGFORMAT.ZERO),
+@dataclass
+class LogOptions:
+    log_time: bool = clickdc.option(
+        "-T",
+        is_flag=True,
+        help="""
+            Additionally add timestamp to the logs.
+            The timestamp of stdout and stderr streams is when the log was received,
+            as Nomad does not store timestamp of task logs.
+            """,
+    )
+    log_time_format: str = clickdc.option(
+        default="%Y-%m-%dT%H:%M:%S%z",
+        show_default=True,
+        help="Format time with specific format. Passed to python datetime.strftime.",
+    )
+    log_time_hour: Any = clickdc.alias_option(
+        "-H",
+        aliased=dict(
+            log_time_format="%H:%M:%S",
+            log_time=True,
         ),
-        click.option(
-            "-o",
-            "--out",
-            type=CommaList("all alloc stdout stderr eval deploy none".split()),
-            default=["all"],
-            show_default=True,
-            help="""
-                Comma separated list of streams of messages to print:
-                deployment, evaluation, allocation, stdout and stderr logs of tasks.
-                """,
+    )
+    log_time_us: Any = clickdc.alias_option(
+        "-U",
+        aliased=dict(
+            log_time_format="%H:%M:%S.%f",
+            log_time=True,
         ),
     )
+    log_format: str = clickdc.option(
+        default=LOGFORMAT.DEFAULT,
+        show_default=True,
+        help="The format to use when printing job logs",
+    )
+    log_id_len: int = clickdc.option(
+        default=6,
+        type=int,
+        help="The length of id to log. UUIDv4 has 36 characters.",
+    )
+    log_id_long: Any = clickdc.alias_option("-l", aliased=dict(log_id_len=36))
+    log_only_task: Any = clickdc.alias_option(
+        "-1", aliased=dict(log_format=LOGFORMAT.ONE)
+    )
+    log_only_mark: Any = clickdc.alias_option(
+        aliased=dict(log_format=LOGFORMAT.ONLYMARK)
+    )
+    log_none: Any = clickdc.alias_option("-0", aliased=dict(log_format=LOGFORMAT.ZERO))
+    out: List[str] = clickdc.option(
+        "-o",
+        type=CommaList("all alloc stdout stderr eval deploy nolog none".split()),
+        default=["all"],
+        show_default=True,
+        help="""
+            Comma separated list of streams of messages to print:
+            deployment, evaluation, allocation, stdout and stderr logs of tasks.
+            """,
+    )
 
 
 def init_logging():
-    LOGENABLED.deploy = any(s in "all deploy".split() for s in ARGS.out)
-    LOGENABLED.eval = any(s in "all eval".split() for s in ARGS.out)
-    LOGENABLED.alloc = any(s in "all alloc".split() for s in ARGS.out)
+    LOGENABLED.deploy = any(s in "all deploy nolog".split() for s in ARGS.out)
+    LOGENABLED.eval = any(s in "all eval nolog".split() for s in ARGS.out)
+    LOGENABLED.alloc = any(s in "all alloc nolog".split() for s in ARGS.out)
     LOGENABLED.stderr = any(s in "all stderr".split() for s in ARGS.out)
     LOGENABLED.stdout = any(s in "all stdout".split() for s in ARGS.out)
     #
     ARGS.verbose -= ARGS.quiet
     if ARGS.verbose > 1:
+        from http import client as http_client
+
         http_client.HTTPConnection.debuglevel = 1
     logging.basicConfig(
         format=LOGFORMAT.render(LOGFORMAT.LOGGING),
         datefmt=ARGS.log_time_format,
         level=(
             logging.DEBUG
             if ARGS.verbose > 0
-            else (
-                logging.INFO
-                if ARGS.verbose == 0
-                else logging.WARN
-                if ARGS.verbose == 1
-                else logging.ERROR
-            )
+            else logging.INFO
+            if ARGS.verbose == 0
+            else logging.WARN
+            if ARGS.verbose == 1
+            else logging.ERROR
         ),
     )
 
 
-@dataclass(frozen=True)
-class Mylogger:
-    """Used to log from the various streams we want to log from"""
+@dataclass(frozen=True, order=True)
+class MyloggerLine:
+    """Represents a single line to log out"""
 
+    # Now has to be first for sorting order
+    now: datetime.datetime
     id: str
     message: str
     what: str
-    now: datetime.datetime = field(default_factory=datetime.datetime.now)
+    ModifyIndex: int
     nodename: Optional[str] = None
     jobversion: Optional[str] = None
     group: Optional[str] = None
     task: Optional[str] = None
 
-    def fmt(self):
+    def __post_init__(self):
         assert self.what in [
             e.value for e in LogWhat
         ], f"{self.what} value is not a valid what"
+
+    @property
+    def known_time(self):
+        """Is the time of the message known or guessed?"""
+        return self.what not in [LogWhat.stdout, LogWhat.stderr]
+
+    def __fmt(self):
         mark: str = LOGFORMAT.marks[self.what]
         color: str = LOGFORMAT.colors[self.what]
         reset: str = COLORS.reset if color else ""
         return LOGFORMAT.render(
             ARGS.log_format,
             **asdict(self),
             mark=mark,
             color=color,
             reset=reset,
             args=ARGS,
         )
 
-    @staticmethod
-    def __log(what: str, **kwargs):
-        mylogger = Mylogger(what=what, **kwargs)
+    def output(self):
         try:
-            out = mylogger.fmt()
+            out = self.__fmt()
         except KeyError:
-            log.exception(f"fmt={ARGS.log_format!r} params={ARGS}")
+            log.exception(
+                f"Could not format logging line. fmt={ARGS.log_format!r} params={ARGS}"
+            )
             raise
         try:
             print(out, flush=True)
         except BrokenPipeError:
             # Python flushes standard streams on exit; redirect remaining output
             # to devnull to avoid another BrokenPipeError at shutdown
             devnull = os.open(os.devnull, os.O_WRONLY)
             os.dup2(devnull, sys.stdout.fileno())
             sys.exit(1)  # Python exits with error code 1 on EPIPE
 
+
+class MyloggerDelayer:
+    """Delay outputting of logs for lines_timeout seconds"""
+
+    @dataclass(frozen=True, order=True)
+    class Key:
+        """The key used in cache as an object"""
+
+        known_time: bool
+
+    def __init__(self):
+        self.old_ModifyIndex: Optional[int] = None
+        """There are new events and old events. Filter out old events"""
+        self.cache: Dict[MyloggerDelayer.Key, List[MyloggerLine]] = {}
+        """Cache of lines to output"""
+        self.newcache: List[MyloggerLine] = []
+        """Cache of lines to output which are newer than old_ModifyIndex"""
+        self.thread = threading.Thread(
+            name=self.__class__.__name__, target=self.__run, daemon=False
+        )
+        """Thread that after lines_timeout outputs log lines"""
+        self.lock = threading.Lock()
+        """Synchronize thread with log producer"""
+        self.finished: bool = False
+        """Set to true when thread is finished for speed"""
+
+    def __run(self):
+        assert ARGS.lines >= 0
+        assert ARGS.lines_timeout >= 0
+        log.debug(f"{self.thread.name} sleeping")
+        time.sleep(ARGS.lines_timeout)
+        log.debug(f"{self.thread.name} starting")
+        with self.lock:
+            try:
+                if ARGS.lines == 0 or len(self.cache) == 0:
+                    return
+                #
+                lines = ARGS.lines
+                knowntimelines = sorted(self.cache.get(self.Key(True), []))[-lines:]
+                for line in knowntimelines:
+                    line.output()
+                lines -= len(knowntimelines)
+                if lines:
+                    unknowntimelines = self.cache.get(self.Key(False), [])[-lines:]
+                    for line in unknowntimelines:
+                        line.output()
+                #
+                self.newcache.sort()
+                for line in self.newcache:
+                    line.output()
+            finally:
+                cachetxt = [
+                    len(self.cache.get(self.Key(True), "")),
+                    len(self.cache.get(self.Key(False), "")),
+                ]
+                log.debug(
+                    f"{self.thread.name} finished"
+                    f" len(newcache)={len(self.newcache)} len(cache)={cachetxt} -n={ARGS.lines}"
+                )
+                self.newcache.clear()
+                self.cache.clear()
+                self.finished = True
+
+    def start(self, ModifyIndex: Optional[int]):
+        """Start the thread"""
+        self.old_ModifyIndex = ModifyIndex
+        if ARGS.lines < 0:
+            # If args is lower than 0, we set finished right away.
+            self.finished = True
+        else:
+            self.thread.start()
+
+    def join(self):
+        """The only possible way the thread can get stuck is if print() output
+        is stuck, as if writing to a pipe."""
+        if ARGS.lines >= 0:
+            self.thread.join()
+
+    def log(self, line: MyloggerLine):
+        """Try to log the line. The line is either logged streight or added to cache"""
+        if self.finished:
+            line.output()
+            return
+        with self.lock:
+            if self.finished:
+                line.output()
+                return
+            if (
+                self.old_ModifyIndex is not None
+                and line.ModifyIndex > self.old_ModifyIndex
+            ):
+                self.newcache.append(line)
+            else:
+                self.cache.setdefault(self.Key(line.known_time), []).append(line)
+
+
+myloggerdelayer = MyloggerDelayer()
+
+
+class Mylogger:
+    """Used to log from the various streams we want to log from"""
+
+    @staticmethod
+    def __log(**kwargs):
+        line = MyloggerLine(**kwargs)
+        myloggerdelayer.log(line)
+
+    ###############################################################################
+
     @classmethod
     def log_eval(cls, eval: nomadlib.Eval, message: str):
         return cls.__log(
-            LogWhat.eval,
+            what=LogWhat.eval,
             id=eval.ID,
-            jobversion=DB.find_jobversion_from_modifyindex(eval.ModifyIndex),
             now=ns2dt(eval.ModifyTime),
+            jobversion=DB.find_jobversion_from_modifyindex(eval.ModifyIndex),
             message=message,
+            ModifyIndex=eval.ModifyIndex,
         )
 
     @classmethod
     def log_deploy(cls, deploy: nomadlib.Deploy, message: str):
         job = DB.jobversions.get(deploy.JobVersion)
         return cls.__log(
-            LogWhat.deploy,
+            what=LogWhat.deploy,
             id=deploy.ID,
-            jobversion=deploy.JobVersion,
             now=ns2dt(job.SubmitTime) if job else datetime.datetime.now(),
+            jobversion=deploy.JobVersion,
             message=message,
+            ModifyIndex=deploy.ModifyIndex,
+        )
+
+    @staticmethod
+    def __add_allocdata(allocid: str) -> dict:
+        """Given an allocid, extracts ModifyIndex and finds job version"""
+        alloc = DB.allocations.get(allocid)
+        return dict(
+            ModifyIndex=alloc.ModifyIndex if alloc else None,
+            nodename=alloc.NodeName if alloc else None,
+            group=alloc.TaskGroup if alloc else None,
+            jobversion=None if not alloc else DB.get_allocation_jobversion(alloc),
         )
 
     @classmethod
     def log_alloc(cls, allocid: str, **kwargs):
-        return cls.__log(LogWhat.alloc, id=allocid, **kwargs)
+        return cls.__log(
+            what=LogWhat.alloc,
+            id=allocid,
+            **cls.__add_allocdata(allocid),
+            **kwargs,
+        )
 
     @classmethod
     def log_std(cls, stderr: bool, allocid: str, **kwargs):
         return cls.__log(
-            LogWhat.stderr if stderr else LogWhat.stdout, id=allocid, **kwargs
+            what=LogWhat.stderr if stderr else LogWhat.stdout,
+            id=allocid,
+            **cls.__add_allocdata(allocid),
+            **kwargs,
         )
 
 
 @dataclass(frozen=True)
 class TaskKey:
-    """Represent data to unique identify a task"""
+    """
+    Represent data to uniquely identify a task.
+    TaskKey stores allocation ID. Altough we have to do a search later,
+    the allocation data itself change often and in parallel to this object.
+    """
 
     allocid: str
-    jobversion: str
-    nodename: str
-    group: str
     task: str
 
     def __str__(self):
-        return f"{self.allocid:.6}:v{self.jobversion}:{self.group}:{self.task}"
+        return f"{self.allocid:.6}:{self.task}"
 
     def asdict(self):
         return asdict(self)
 
     def log_alloc(self, now: datetime.datetime, message: str):
         Mylogger.log_alloc(now=now, message=message, **self.asdict())
 
@@ -449,142 +593,130 @@
 
     def __init__(self, tk: TaskKey, stderr: bool):
         super().__init__(name=f"{tk}:{'stderr' if stderr else 'stdout'}")
         self.tk = tk
         """task key"""
         self.stderr: bool = stderr
         """is this stderr or stdout logger"""
-        #
-        self.startevent = threading.Event()
-        """This is an event which is sent after --shutdown-timeout time after log listening starts"""
-        self.starttimer = threading.Timer(ARGS.shutdown_timeout, self.__set_startevent)
-        """A timer that will set startevent"""
-        self.exitevent = threading.Event()
-        """User should set this event to stop logging the task logs"""
-        self.ignoredlines: List[str] = []
-        """In the case of --lines argument, this is a buffer of spare lines to output"""
-        self.first_line: bool = True
-        """Ignore input lines if printing only trailing lines."""
-        self.ignoretime_ns: int = START_NS + int(ARGS.lines_timeout * 1e9)
-        """If ignore time is in the past, it is no longer relevant anyway."""
-        #
-        if ARGS.lines < 0 or self.ignoretime_ns < time.time_ns():
-            self.ignoretime_ns = 0
-
-    def __set_startevent(self):
-        self.startevent.set()
-        DB.send_empty_event()
+        self.exitreqtime: Optional[float] = None
+        """stop() was called"""
+        self.started: bool = False
+        """This logger is assumed to have started and printed logs"""
+        self.startedtime: Optional[float] = None
+        """A timer that will set self.stated"""
+        self.stopped: bool = False
 
     @staticmethod
-    def read_json_stream(stream: requests.Response):
+    def read_json_txt(stream: requests.Response) -> Iterator[str]:
         txt: str = ""
         for dataorbytes in stream.iter_content(decode_unicode=True):
             try:
                 data: str = dataorbytes.decode()
             except (UnicodeDecodeError, AttributeError):
                 data: str = dataorbytes
             for c in data:
                 txt += c
                 # Nomad happens to be consistent, the jsons are flat.
                 if c == "}":
-                    try:
-                        ret = json.loads(txt)
-                        # log.debug(f"RECV: {ret}")
-                        yield ret
-                    except json.JSONDecodeError as e:
-                        log.warn(f"error decoding json: {txt} {e}")
+                    yield txt
                     txt = ""
+        if txt:
+            yield txt
 
-    def taskout(self, lines: List[str]):
-        """Output the lines"""
-        # If ignoring and this is first received line or the ignoring time is still happenning.
-        if self.ignoretime_ns and (
-            self.first_line or time.time_ns() < self.ignoretime_ns
-        ):
-            # Accumulate args.lines into ignoredlines array.
-            self.first_line = False
-            self.ignoredlines = lines
-            self.ignoredlines = self.ignoredlines[: ARGS.lines]
-        else:
-            if self.ignoretime_ns:
-                # If not ignoring lines, flush the accumulated lines.
-                lines = self.ignoredlines + lines
-                self.ignoredlines.clear()
-                # Disable further accumulation of ignored lines.
-                self.ignoretime_ns = 0
-            # Print the log lines.
-            for line in lines:
-                line = line.rstrip()
-                self.tk.log_task(self.stderr, line)
+    @classmethod
+    def read_json_stream(cls, stream: requests.Response) -> Iterator[Dict[str, Any]]:
+        for txt in cls.read_json_txt(stream):
+            try:
+                ret = json.loads(txt)
+                # log.debug(f"RECV: {ret}")
+                yield ret
+            except json.JSONDecodeError as e:
+                if not re.match(
+                    "failed to list entries:.*no such file or directory", txt
+                ):
+                    log.warn(f"error decoding json: {txt} {e}")
 
     def __typestr(self):
         return "stderr" if self.stderr else "stdout"
 
     def __run_in(self):
+        usestart = ARGS.lines < 0 or START_S + ARGS.lines_timeout < time.time()
         with mynomad.stream(
             f"client/fs/logs/{self.tk.allocid}",
             params={
                 "task": self.tk.task,
                 "type": self.__typestr(),
                 "follow": True,
-                "origin": "end" if self.ignoretime_ns else "start",
-                "offset": 50000 if self.ignoretime_ns else 0,
+                "origin": "start" if usestart else "end",
+                "offset": 0 if usestart else 50000,
             },
         ) as stream:
-            self.starttimer.start()
             for event in self.read_json_stream(stream):
                 if event:
                     line64: Optional[str] = event.get("Data")
                     if line64:
-                        lines = (
-                            base64.b64decode(line64.encode())
-                            .decode(errors="replace")
-                            .splitlines()
-                        )
-                        self.taskout(lines)
-                else:
-                    # Nomad json stream periodically sends empty {}.
-                    self.taskout([])
-                if self.exitevent.is_set():
-                    break
+                        linebytes = base64.b64decode(line64.encode())
+                        lines = linebytes.decode(errors="replace").splitlines()
+                        for line in lines:
+                            self.tk.log_task(self.stderr, line.strip())
+                    fileevent: Optional[str] = event.get("FileEvent")
+                    if fileevent == "file deleted":
+                        # Deleted means end of stream.
+                        break
+                # Nomad json stream every second sends empty {}.
+                # If requested to exit, then exit.
+                if self.exitreqtime is not None:
+                    if self.exitreqtime <= time.time():
+                        break
+        stream.raise_for_status()
 
     def run(self):
         """Listen to Nomad log stream and print the logs"""
         try:
-            self.__run_in()
+            # Try getting the logs for 2 seconds, then give up.
+            tries: int = int(ARGS.shutdown_timeout + 1)
+            for tryno in range(tries):
+                try:
+                    self.__run_in()
+                    break
+                except nomadlib.LogNotFound:
+                    time.sleep(1)
+            else:
+                self.__run_in()
         except nomadlib.LogNotFound as e:
             # Gracefully handle missing logs errors from Nomad.
             # Logs are removed by garbage collector and when purging the job.
             code = e.response.status_code if e.response is not None else None
             text = e.response.text if e.response is not None else None
             self.tk.log_alloc(
                 datetime.datetime.now(),
                 f"Error getting {self.__typestr()} logs: {code} {text!r}",
             )
-        except requests.HTTPError:
-            raise
         finally:
-            self.__set_startevent()
+            log.debug(f"{self} stopped")
+            self.stopped = True
+            DB.send_empty_event()
 
-    def stop(self):
-        self.exitevent.set()
-        self.starttimer.cancel()
-        self.__set_startevent()
+    def stop(self, delay: bool):
+        if self.exitreqtime is None or (
+            delay is True and self.exitreqtime > time.time()
+        ):
+            log.debug(f"{self} stoppping delay={delay}")
+            self.exitreqtime = time.time() + delay * ARGS.shutdown_timeout
 
 
 @dataclass
 class TaskHandler:
     """A handler for one task. Creates loggers, writes out task events, handle exit conditions"""
 
     loggers: Optional[List[TaskLogger]] = None
     """Array of loggers that log allocation logs."""
     messages: Set[int] = field(default_factory=set)
     """A set of message timestamp to know what has been printed."""
     exitcode: Optional[int] = None
-    stoptimer: Optional[threading.Timer] = None
 
     @staticmethod
     def _create_loggers(tk: TaskKey):
         ths: List[TaskLogger] = []
         if LOGENABLED.stdout:
             ths.append(TaskLogger(tk, False))
         if LOGENABLED.stderr:
@@ -600,63 +732,55 @@
             for e in taskstate.Events or []:
                 msgtime_ns = e.Time
                 # Ignore message before ignore times.
                 if (
                     msgtime_ns
                     and (
                         ARGS.lines < 0
-                        or msgtime_ns >= START_NS
+                        or msgtime_ns >= int(START_S * 10**9)
                         or len(self.messages) < ARGS.lines
                     )
                     and set_not_in_add(self.messages, msgtime_ns)
                 ):
                     for line in e.DisplayMessage.splitlines():
                         if line:
                             tk.log_alloc(ns2dt(msgtime_ns), f"{e.Type} {line}")
         if (
             self.loggers is None
             and taskstate.State in ["running", "dead"]
             and taskstate.was_started()
         ):
             self.loggers = self._create_loggers(tk)
-        if self.stoptimer is None and self.loggers and taskstate.State == "dead":
-            # If the task is already finished, give myself max 3 seconds to query all the logs.
-            # This is to reduce the number of connections.
-            self.stoptimer = threading.Timer(3, self.stop)
-            self.stoptimer.start()
+        if taskstate.State == "dead":
+            # log.debug(f"Task {tk} dead")
+            self.stop(True)
         if self.exitcode is None and taskstate.State == "dead":
             terminatedevent = taskstate.find_event("Terminated")
             if terminatedevent:
                 self.exitcode = terminatedevent.ExitCode
 
-    def stop(self):
-        if self.stoptimer:
-            self.stoptimer.cancel()
+    def stop(self, delay: bool = False):
         for ll in self.loggers or []:
-            ll.stop()
+            ll.stop(delay)
 
 
 @dataclass
 class AllocWorker:
     """Represents a worker that prints out and manages state related to one allocation"""
 
     taskhandlers: Dict[TaskKey, TaskHandler] = field(default_factory=dict)
 
     def notify(self, alloc: nomadlib.Alloc):
         """Update the state with alloc"""
         for taskname, task in alloc.get_taskstates().items():
             if ARGS.task and not ARGS.task.search(taskname):
                 continue
-            tk = TaskKey(
-                alloc.ID,
-                str(DB.get_allocation_jobversion(alloc, "?")),
-                alloc.NodeName,
-                alloc.TaskGroup,
-                taskname,
-            )
+            if ARGS.node and not ARGS.node.search(alloc.NodeName):
+                continue
+            tk = TaskKey(allocid=alloc.ID, task=taskname)
             self.taskhandlers.setdefault(tk, TaskHandler()).notify(tk, task)
 
 
 class ExitCode:
     success = 0
     exception = 1
     interrupted = 2
@@ -773,71 +897,73 @@
         return [
             logger
             for w in self.workers.values()
             for th in w.taskhandlers.values()
             for logger in th.loggers or []
         ]
 
+    def all_threads_stopped(self) -> bool:
+        return all(th.stopped for th in self.get_threads())
+
     def join(self):
         threads = self.get_threads()
         # Logs stream outputs empty {} which allows to handle timeouts.
         thcnt = sum(len(w.taskhandlers) for w in self.workers.values())
         log.debug(
             f"Joining {len(self.workers)} allocations with {thcnt} taskhandlers and {len(threads)} loggers"
         )
+        myloggerdelayer.join()
         timeend = time.time() + ARGS.shutdown_timeout
         timeout = None
         for thread in threads:
             timeout = timeend - time.time()
             if timeout > 0:
                 log.debug(f"joining worker {thread.name} timeout={timeout}")
-                thread.startevent.wait(timeout)
+                thread.join(timeout)
             else:
                 break
         log.debug(f"{len(threads)} threads joined with {timeout} timeout to spare")
 
     def __exitcode(self) -> ExitcodeRet:
         tasks_exitcodes: List[Optional[int]] = [
             th.exitcode for w in self.workers.values() for th in w.taskhandlers.values()
         ]
         if flagdebug.debug("exitcode"):
             for allocid, w in self.workers.items():
                 for taskkey, taskhandler in w.taskhandlers.items():
-                    eprint(
-                        f"EXITCODE: {allocid[:6]} {taskkey.group}/{taskkey.task} {taskhandler.exitcode}"
-                    )
+                    eprint(f"EXITCODE: {taskkey} {taskhandler.exitcode}")
         if len(tasks_exitcodes) == 0:
             return ExitcodeRet(ExitCode.no_allocations, "there were no allocations")
         unfinished_tasks = [v for v in tasks_exitcodes if v is None]
         if unfinished_tasks:
             return ExitcodeRet(
                 ExitCode.any_unfinished_tasks,
-                f"there were {len(unfinished_tasks)} unfinished tasks",
+                f"There were {len(unfinished_tasks)} unfinished tasks",
             )
         only_one_task = len(tasks_exitcodes) == 1
         if only_one_task:
             assert tasks_exitcodes[0] is not None
             return ExitcodeRet(
                 tasks_exitcodes[0],
-                f"single task exited with {tasks_exitcodes[0]} exit status",
+                f"Single task exited with {tasks_exitcodes[0]} exit status",
             )
         failed_tasks = [v for v in tasks_exitcodes if v != 0]
         if len(failed_tasks) == len(tasks_exitcodes):
             return ExitcodeRet(
                 ExitCode.all_failed_tasks,
-                f"all {len(tasks_exitcodes)} tasks exited with nonzero exit status",
+                f"All {len(tasks_exitcodes)} tasks exited with nonzero exit status",
             )
         if failed_tasks:
             return ExitcodeRet(
                 ExitCode.any_failed_tasks,
                 f"{len(failed_tasks)} tasks exited with nonzero exit status",
             )
         return ExitcodeRet(
             ExitCode.success,
-            f"all {len(tasks_exitcodes)} tasks exited with zero exit status",
+            f"All {len(tasks_exitcodes)} tasks exited with zero exit status",
         )
 
     def exitcode(self) -> int:
         er: ExitcodeRet = self.__exitcode()
         log.info(f"{er.reason.capitalize()}. Exit code is {er.code}.")
         return er.code
 
@@ -846,15 +972,15 @@
 
 
 def __nomad_job_run(args: List[str]) -> str:
     """Call nomad job run to start a Nomad job using nomad job run call with specified arguments"""
     cmd: List[str] = "nomad job run -detach -verbose".split() + args
     log.info(f"+ {' '.join(shlex.quote(x) for x in cmd)}")
     try:
-        output = subprocess.check_output(cmd, text=True)
+        output = subprocess.check_output(cmd, text=True, stdin=sys.stdin)
     except subprocess.CalledProcessError as e:
         # nomad will print its error, we can just exit
         exit(e.returncode)
     # Extract evaluation id from Nomad output.
     for line in output.splitlines():
         log.info(line)
     founduuids = re.findall(
@@ -871,15 +997,36 @@
     )
     evalid = founduuids[0]
     return evalid
 
 
 def nomad_start_job(opts: List[str]) -> nomadlib.Eval:
     """Start a nomad job using nomad job run parameters. Return evluation from running the job"""
-    evalid = __nomad_job_run(opts)
+    assert opts
+    evalid: Optional[str] = None
+    if ARGS.json or (len(opts) == 2 and opts[0] == "-json"):
+        # If the input file is a json and we have no arguments, we can use the API ourselves.
+        file = opts[-1]
+        stream = contextlib.closing(sys.stdin) if file == "-" else open(file)
+        with stream as f:
+            data: str = f.read()
+        job: dict = json.loads(data)
+        if "Job" in job:
+            job = job["Job"]
+        format: str = "json"
+        resp = mynomad.start_job(job, nomadlib.JobSubmission(data, format))
+        evalid = resp["EvalID"]
+        warnings = resp.get("Warnings")
+        if warnings:
+            log.warning(f"{warnings}")
+    else:
+        # Otherwise, call nomad executable to schedule the job.
+        if ARGS.json:
+            opts = ["-json"] + opts
+        evalid = __nomad_job_run(opts)
     evaluation = nomadlib.Eval(mynomad.get(f"evaluation/{evalid}"))
     mynomad.namespace = evaluation.Namespace
     return evaluation
 
 
 ###############################################################################
 
@@ -910,38 +1057,44 @@
             ],
             select_event_cb=self.__db_select_event_job,
             init_cb=self.__db_init_cb,
             force_polling=True if ARGS.polling else None,
         )
         self.notifier = NotifierWorker()
         """Notification worker dispatching Nomad stream events"""
-        self.no_follow_timeend: float = time.time() + ARGS.no_follow_timeout
-        """If in --no-follow mode, exit after this time"""
+        self.no_follow_end: bool = False
+        """Flag that is set once no_follow timeout passes"""
+        if ARGS.no_follow:
+            th = threading.Timer(ARGS.no_follow_timeout, self.__no_follow_timer)
+            th.setDaemon(True)
+            th.start()
         #
         DB.start()
         InterruptTwice.install()
+        myloggerdelayer.start(self.eval.ModifyIndex if self.eval else None)
+
+    def __no_follow_timer(self):
+        self.no_follow_end = True
+        DB.send_empty_event()
 
     def __db_init_cb(self) -> List[Event]:
         """Db initialization callback"""
         try:
             job: dict = mynomad.get(f"job/{self.jobid}")
             jobversions: dict = mynomad.get(f"job/{self.jobid}/versions")["Versions"]
             deployments: List[dict] = mynomad.get(f"job/{self.jobid}/deployments")
             evaluations: List[dict] = mynomad.get(f"job/{self.jobid}/evaluations")
             allocations: List[dict] = mynomad.get(f"job/{self.jobid}/allocations")
-        except nomadlib.JobNotFound:
+        except nomadlib.JobNotFound as e:
             # This is fine to fail if it was purged, potentially.
-            if DB.seen_job() and self.job:
-                # If the job was purged, generate one event so that listener can catch it.
-                return [
-                    Event(
-                        -1, EventTopic.Job, EventType.JobDeregistered, self.job.asdict()
-                    )
-                ]
-            raise
+            # If the job was purged, generate one event so that listener can catch it.
+            # In the follow mode, just ignore missing job.
+            log.debug(f"JobNotFound exception: {e}")
+            DB.job_deregistered_ModifyIndex = DB.job.ModifyIndex + 1 if DB.job else 0
+            return []
         # Set the job if not set for the first time.
         if not self.job:
             self.job = nomadlib.Job(job)
             log.debug(
                 f"Found job {self.job.description()} from {self.eval.ID if self.eval else None}"
                 f" with {len(allocations)} allocations"
             )
@@ -1056,45 +1209,38 @@
                 seenJob=self.job and DB.seen_job(),
                 activeEvals=self.has_active_evaluations(),
                 activeAllocs=self.has_active_allocations(),
                 activeDeploys=self.has_active_deployments(),
                 isPurged=DB.job_purged(),
                 jobDead=self.job.is_dead() if self.job else None,
                 notifiers=[
-                    f"{th.name}={int(th.startevent.is_set())}"
-                    for th in self.notifier.get_threads()
+                    f"{th.name}={th.started}" for th in self.notifier.get_threads()
                 ],
             )
             eprint(f"LOOP: {strdict(info)}")
 
     def loop(self) -> Iterator[None]:
         """Thread entrypoint that handles events from Nomad event stream database"""
         untilstr = (
             "forever"
-            if ARGS.all
-            else (
-                f"for {ARGS.no_follow_timeout} seconds"
-                if ARGS.no_follow
-                else f"until it is {self.endstatusstr}"
-            )
+            if ARGS.follow
+            else f"for {ARGS.no_follow_timeout} seconds"
+            if ARGS.no_follow
+            else f"until it is {self.endstatusstr}"
         )
         log.info(f"Watching job {self.jobid}@{mynomad.namespace} {untilstr}")
         for events in DB.events():
             for event in events:
                 self.__handle_event(event)
             self.__loop_debug(events)
-            if (
-                # If we started with an evaluation, it has to be finished.
-                # Otherwise the events may be related to a previous job version.
-                (self.eval is None or not self.eval.is_pending_or_blocked())
-                # Make sure all the threads have finished outputting logs.
-                and all(th.startevent.is_set() for th in self.notifier.get_threads())
-            ):
+            # If we started with an evaluation, it has to be finished.
+            # Otherwise the events may be related to a previous job version.
+            if self.eval is None or not self.eval.is_pending_or_blocked():
                 yield
-            if ARGS.no_follow and time.time() > self.no_follow_timeend:
+            if self.no_follow_end:
                 break
         log.debug(f"Watching job {self.jobid}@{mynomad.namespace} exiting")
 
     def has_active_deployments(self):
         for deployment in DB.deployments.values():
             if not deployment.is_finished():
                 if flagdebug.debug("active"):
@@ -1125,59 +1271,250 @@
         return (
             not self.has_active_allocations()
             and not self.has_active_evaluations()
             and not self.has_active_deployments()
         )
 
 
-class NomadJobWatcher(_NomadJobWatcherDetail):
+class NotifyEvent(MyStrEnum):
+    started = enum.auto()
+    purging = enum.auto()
+    stopping = enum.auto()
+    exit = enum.auto()
+
+    @classmethod
+    def txt(cls) -> str:
+        return andjoin((repr(x + "") for x in cls), fin=" or ")
+
+
+class _NomadJobWatcherEvents(_NomadJobWatcherDetail):
     @override
     def __init__(self, jobid: Optional[str], eval: Optional[nomadlib.Eval] = None):
         super().__init__(jobid, eval)
         self.purged_eval: Optional[str] = None
         """Return true if we sent a request to purge the job"""
         self.stopped_eval: Optional[str] = None
         """Return true if we sent a request to stop the job"""
+        self.job_started: bool = False
+        """If set to True, means that the job has started all main tasks"""
+        self.notifyfd = sorted(list(set(ARGS.notifyfd)))
+        self.notifyfdstarted = sorted(list(set(ARGS.notifyfdstarted)))
+
+    def __notifyfd(self, arg: List[str], fdlist: List[int]):
+        if fdlist:
+            for fd in list(fdlist):
+                line: str = json.dumps(arg)
+                assert line.count("\n") == 0
+                linebytes: bytes = f"{line}\n".encode()
+                flagdebug.logdebug("notify", f"notifyfd {fd} {line!r}")
+                try:
+                    os.write(fd, linebytes)
+                except (BrokenPipeError, IOError) as e:
+                    flagdebug.logdebug("notify", f"{e}")
+                    try:
+                        os.close(fd)
+                    except Exception:
+                        pass
+                    fdlist.remove(fd)
+
+    def __notifyuser(self, event: NotifyEvent):
+        flagdebug.logdebug("notify", f"notify {event}")
+        arg: List[str] = [self.jobid, event]
+        for exe in ARGS.notifyexe:
+            cmd = shlex.split(exe) + arg
+            flagdebug.logdebug("notify", f"notifyexe {cmd}")
+            subprocess.check_call(cmd)
+        self.__notifyfd(arg, self.notifyfd)
+        if event == NotifyEvent.started:
+            for exe in ARGS.notifyexestarted:
+                cmd = shlex.split(exe)
+                flagdebug.logdebug("notify", f"notifyexestarted {cmd}")
+                subprocess.check_call(cmd)
+            self.__notifyfd(arg, self.notifyfdstarted)
+            for fd in self.notifyfdstarted:
+                os.close(fd)
 
-    @abstractmethod
-    def _get_exitcode_cb(self) -> int:
-        raise NotImplementedError()
-
-    @abstractmethod
-    def _loop_end_cb(self):
-        raise NotImplementedError()
+    @override
+    def loop(self) -> Iterator[None]:
+        try:
+            for i in super().loop():
+                if not self.job_started:
+                    if self.__job_has_finished_starting():
+                        self.__notifyuser(NotifyEvent.started)
+                        self.job_started = True
+                yield i
+        finally:
+            self.__notifyuser(NotifyEvent.exit)
 
     def stop_job(self, purge: bool = False):
         assert DB.initialized.is_set()
         if purge:
             if self.purged_eval:
                 return
+            self.__notifyuser(NotifyEvent.purging)
             log.info(f"Purging job {self.jobid}")
         else:
             if self.stopped_eval:
                 return
             log.info(f"Stopping job {self.jobid}")
+            self.__notifyuser(NotifyEvent.stopping)
         evalid = mynomad.stop_job(self.jobid, purge)["EvalID"]
         self.stopped_eval = evalid
         if purge:
             self.purged_eval = evalid
 
-    def stop_threads(self):
-        log.debug(f"stopping {self.__class__.__name__}")
-        self.notifier.stop()
-        DB.stop()
-        self.notifier.join()
-        DB.join()
-        mynomad.session.close()
-
-    def get_exitcode(self) -> int:
-        assert DB.stopevent.is_set(), f"{self.stop_threads.__name__} not called"
-        if InterruptTwice.received:
-            return ExitCode.interrupted
-        return self._get_exitcode_cb()
+    @staticmethod
+    def __nomad_job_group_main_tasks(group: nomadlib.JobTaskGroup):
+        """Get a set of names of Nomad job group main tasks"""
+        # Main tasks are tasks that:
+        # - do not have lifecycle
+        # - have lifecycle prestart with sidecar = true
+        # - have lifecycle poststart
+        # All these tasks have to be started.
+        maintasks = set(
+            t.Name
+            for t in group.Tasks
+            if "Lifecycle" not in t
+            or t.Lifecycle is None
+            or (
+                t.Lifecycle.Hook == nomadlib.LifecycleHook.prestart
+                and t.Lifecycle.get_sidecar() is True
+            )
+            or t.Lifecycle.Hook == nomadlib.LifecycleHook.poststart
+        )
+        assert len(maintasks) > 0, f"Internal error when getting main tasks of {group}"
+        return maintasks
+
+    def __job_has_finished_starting(self) -> bool:
+        """
+        Return True if the job is not starting anymore.
+        self.started will be set to True, if the job was successfully started.
+        """
+        # log.debug(f"has_active_deployments={self.has_active_deployments()} has_active_evaluations={self.has_active_evaluations()} allocations={len(DB.allocations)}")  # noqa
+        if (
+            not self.job
+            or self.has_active_deployments()
+            or self.has_active_evaluations()
+        ):
+            flagdebug.logdebug(
+                "started",
+                "The job is still doing something. Wait for it. "
+                f" job={self.job} deployments={self.has_active_deployments()} evals={self.has_active_evaluations()}",
+            )
+            return False
+        allocations = DB.allocations.values()
+        if (
+            not allocations
+            or any(alloc.is_pending() for alloc in allocations)
+            or any(alloc.TaskStates is None for alloc in allocations)
+        ):
+            flagdebug.logdebug(
+                "started",
+                "There are still allocations which Tasks have not started yet. Wait for them."
+                f" allocations={not not allocations}"
+                f" pendings={sum(alloc.is_pending() for alloc in allocations)}"
+                f" taskstates={sum(alloc.TaskStates is None for alloc in allocations)}",
+            )
+            return False
+        # Check if there are tasks running for all Groups.
+        groupmsgs: List[str] = []
+        for group in self.job.TaskGroups:
+            previousrunningallocs: List[nomadlib.Alloc] = [
+                alloc
+                for alloc in allocations
+                if alloc.TaskGroup == group.Name
+                and alloc.is_pending_or_running()
+                and (
+                    DB.get_allocation_jobmodifyindex(alloc, -1) < self.minjobmodifyindex
+                    or DB.get_allocation_jobversion(alloc, -1) < self.job.Version
+                )
+            ]
+            # Allocations related to previous job version have to be stopped.
+            if previousrunningallocs:
+                flagdebug.logdebug(
+                    "started",
+                    f"There are still allocations running for previous job version: {previousrunningallocs}",
+                )
+                return False
+            #
+            groupallocs: List[nomadlib.Alloc] = [
+                alloc
+                for alloc in allocations
+                if alloc.TaskGroup == group.Name
+                and DB.get_allocation_jobmodifyindex(alloc, -1)
+                >= self.minjobmodifyindex
+                and DB.get_allocation_jobversion(alloc, -1) == self.job.Version
+            ]
+            # There have to be at exactly group.Count allocations of this group for it to be deployed.
+            # The allocation not necessarily have to be running - they may have finished.
+            if len(groupallocs) != group.Count:
+                # This group has no active evaluation and deployments (checked above).
+                flagdebug.logdebug(
+                    "started",
+                    f"groupallocs={[x.ID for x in groupallocs]}"
+                    f" {[DB.get_allocation_jobmodifyindex(alloc, -1) for alloc in groupallocs]}"
+                    f" {[DB.get_allocation_jobversion(alloc, -1) for alloc in groupallocs]}",
+                )
+                log.error(
+                    f"Job {self.job.description()} group {group.Name!r} started"
+                    f" {len(groupallocs)} allocation out of {group.Count}."
+                )
+                return True
+            maintasks: Set[str] = self.__nomad_job_group_main_tasks(group)
+            for alloc in groupallocs:
+                # List of started tasks.
+                startedtasks: Set[str] = set(
+                    name
+                    for name, taskstate in alloc.get_taskstates().items()
+                    if taskstate.was_started()
+                )
+                notrunningmaintasks = maintasks.difference(startedtasks)
+                if notrunningmaintasks:
+                    # There are main tasks that are not running.
+                    if alloc.TaskStates is None or alloc.is_pending_or_running():
+                        flagdebug.logdebug(
+                            "started",
+                            f"TaskStates={alloc.TaskStates} is_pending_or_running={alloc.is_pending_or_running()}",
+                        )
+                        # Wait for them.
+                        return False
+                    else:
+                        # The allocation has finished - the tasks will never start.
+                        log.error(
+                            f"Job {self.job.description()} failed to start group"
+                            f" {group.Name!r} tasks {' '.join(notrunningmaintasks)}"
+                        )
+                        return True
+            groupallocsidsstr = andjoin(alloc.ID[:6] for alloc in groupallocs)
+            groupmsgs.append(
+                f"allocations {groupallocsidsstr} running group {group.Name!r} with {len(maintasks)} main tasks"
+            )
+        self.started = True
+        msg = f"Job {self.job.description()} started " + andjoin(groupmsgs)
+        # If we are running in eval mode, we can check the associated deployment for failure.
+        if self.eval and self.eval.DeploymentID:
+            deploy = DB.deployments.get(self.eval.DeploymentID)
+            if deploy and deploy.Status in [
+                nomadlib.DeploymentStatus.cancelled,
+                nomadlib.DeploymentStatus.failed,
+            ]:
+                msg += f", but deployment failed: {deploy.StatusDescription!r}"
+                self.started = False
+        log.info(msg + ".")
+        return True
+
+
+class NomadJobWatcher(_NomadJobWatcherEvents):
+    @abstractmethod
+    def _get_exitcode_cb(self) -> int:
+        raise NotImplementedError()
+
+    @abstractmethod
+    def _loop_end_cb(self):
+        raise NotImplementedError()
 
     def run_and_exit(self, stopit: bool = False):
         try:
             for _ in self.loop():
                 # If the job is purged, stop watching.
                 if (
                     not ARGS.follow
@@ -1204,16 +1541,23 @@
                     if ARGS.attach:
                         self.stop_job()
                     else:
                         exit(ExitCode.interrupted)
                 if not ARGS.follow and self._loop_end_cb():
                     break
         finally:
-            self.stop_threads()
-        exit(self.get_exitcode())
+            log.debug(f"stopping {self.__class__.__name__}")
+            self.notifier.stop()
+            DB.stop()
+            if not isinstance(sys.exc_info()[1], SystemExit):
+                self.notifier.join()
+                DB.join()
+        exit(
+            ExitCode.interrupted if InterruptTwice.received else self._get_exitcode_cb()
+        )
 
     def job_is_finished(self):
         return (
             DB.seen_job()
             and self.job
             and self.job.is_dead()
             and self.has_no_active_allocations_nor_evaluations_nor_deployments()
@@ -1253,15 +1597,16 @@
             # Wait for beeing purged in the main loop.
             return False
         if self.job_is_finished():
             if not self.purged_eval and (
                 ARGS.purge
                 or (ARGS.purge_successful and self.job_finished_successfully())
             ):
-                self.stop_job(True)
+                if self.notifier.all_threads_stopped():
+                    self.stop_job(True)
             else:
                 log.info(self.job_dead_message())
                 return True
         return False
 
     @override
     def _get_exitcode_cb(self) -> int:
@@ -1281,124 +1626,27 @@
     def __init__(self, jobid: Optional[str], eval: Optional[nomadlib.Eval] = None):
         super().__init__(jobid, eval)
         self.started: bool = False
         """Will be set to True if the job was _successfully_ started"""
 
     @override
     def _loop_end_cb(self) -> bool:
-        if self.job_has_finished_starting():
+        if self.job_started:
             return True
         if self.job_is_finished():
             log.info(self.job_dead_message())
             return True
         return False
 
     @override
     def _get_exitcode_cb(self) -> int:
         exitcode = ExitCode.success if self.started else ExitCode.failed
         log.debug(f"started={self.started} exitcode={exitcode}")
         return exitcode
 
-    @staticmethod
-    def nomad_job_group_main_tasks(group: nomadlib.JobTaskGroup):
-        """Get a set of names of Nomad job group main tasks"""
-        # Main tasks are tasks that:
-        # - do not have lifecycle
-        # - have lifecycle prestart with sidecar = true
-        # - have lifecycle poststart
-        # All these tasks have to be started.
-        maintasks = set(
-            t.Name
-            for t in group.Tasks
-            if "Lifecycle" not in t
-            or t.Lifecycle is None
-            or (
-                t.Lifecycle.Hook == nomadlib.LifecycleHook.prestart
-                and t.Lifecycle.get_sidecar() is True
-            )
-            or t.Lifecycle.Hook == nomadlib.LifecycleHook.poststart
-        )
-        assert len(maintasks) > 0, f"Internal error when getting main tasks of {group}"
-        return maintasks
-
-    def job_has_finished_starting(self) -> bool:
-        """
-        Return True if the job is not starting anymore.
-        self.started will be set to True, if the job was successfully started.
-        """
-        # log.debug(f"has_active_deployments={self.has_active_deployments()} has_active_evaluations={self.has_active_evaluations()} allocations={len(DB.allocations)}")  # noqa
-        if (
-            not self.job
-            or self.has_active_deployments()
-            or self.has_active_evaluations()
-        ):
-            # The job is still doing something. Wait for it.
-            return False
-        allocations = DB.allocations.values()
-        if (
-            not allocations
-            or any(alloc.is_pending() for alloc in allocations)
-            or any(alloc.TaskStates is None for alloc in allocations)
-        ):
-            # There are still allocations which Tasks have not started yet. Wait for them.
-            return False
-        #
-        groupmsgs: List[str] = []
-        for group in self.job.TaskGroups:
-            groupallocs: List[nomadlib.Alloc] = [
-                alloc
-                for alloc in allocations
-                if alloc.TaskGroup == group.Name
-                and DB.get_allocation_jobmodifyindex(alloc, -1)
-                >= self.minjobmodifyindex
-                and DB.get_allocation_jobversion(alloc, -1) == self.job.Version
-            ]
-            # There have to be at exactly group.Count allocations of this group for it to be deployed.
-            # The allocation not necessarily have to be running - they may have finished.
-            if len(groupallocs) != group.Count:
-                # This group has no active evaluation and deployments (checked above).
-                log.debug(
-                    f"groupallocs={[x.ID for x in groupallocs]}"
-                    f" {[DB.get_allocation_jobmodifyindex(alloc, -1) for alloc in groupallocs]}"
-                    f" {[DB.get_allocation_jobversion(alloc, -1) for alloc in groupallocs]}"
-                )
-                log.error(
-                    f"Job {self.job.description()} group {group.Name!r} started"
-                    f" {len(groupallocs)} allocation out of {group.Count}."
-                )
-                return True
-            maintasks: Set[str] = self.nomad_job_group_main_tasks(group)
-            for alloc in groupallocs:
-                # List of started tasks.
-                startedtasks: Set[str] = set(
-                    name
-                    for name, taskstate in alloc.get_taskstates().items()
-                    if taskstate.was_started()
-                )
-                notrunningmaintasks = maintasks.difference(startedtasks)
-                if notrunningmaintasks:
-                    # There are main tasks that are not running.
-                    if alloc.TaskStates is None or alloc.is_pending_or_running():
-                        # Wait for them.
-                        return False
-                    else:
-                        # The allocation has finished - the tasks will never start.
-                        log.error(
-                            f"Job {self.job.description()} failed to start group"
-                            f" {group.Name!r} tasks {' '.join(notrunningmaintasks)}"
-                        )
-                        return True
-            groupallocsidsstr = andjoin(alloc.ID[:6] for alloc in groupallocs)
-            groupmsgs.append(
-                f"allocations {groupallocsidsstr} running group {group.Name!r} with {len(maintasks)} main tasks"
-            )
-        log.info(f"Job {self.job.description()} started " + andjoin(groupmsgs) + ".")
-        self.started = True
-        return True
-
 
 ###############################################################################
 
 
 @dataclass
 class NomadAllocationWatcher:
     """Watch an allocation until it is finished"""
@@ -1506,15 +1754,144 @@
                 complete = [f"{tg.Name}@{t}" for tg in job.TaskGroups for t in tg.Tasks]
             complete = [f"{arg[0]}@{x}" for x in complete]
         else:
             return []
         return [x for x in complete if x.startswith(incomplete)]
 
 
+@dataclass
+class NotifyOptions:
+    notifyexe: Tuple[str, ...] = clickdc.option(
+        help=f"""
+             When state changes execute this shlex.split command with two arguments:
+             the watched jobid and one of {NotifyEvent.txt()}.
+             """,
+        multiple=True,
+    )
+    notifyfd: Tuple[int, ...] = clickdc.option(
+        type=int,
+        help=f"""
+             When state changes write to this file descriptor a JSON array with two elements:
+             the watched jobid and one of {NotifyEvent.txt()}.
+             """,
+        multiple=True,
+    )
+    notifyexestarted: Tuple[str, ...] = clickdc.option(
+        help="Execute this shlex.split command once the job is started.",
+        multiple=True,
+    )
+    notifyfdstarted: Tuple[int, ...] = clickdc.option(
+        type=int,
+        help="Send a single line message to this fiole descriptor when the job is started.",
+        multiple=True,
+    )
+
+
+def click_validate(check: Callable[[Any], bool], msg: str):
+    def validator(ctx, param, value):
+        if not check(value):
+            raise click.BadParameter(msg)
+        return value
+
+    return validator
+
+
+@dataclass
+class Args(LogOptions, NotifyOptions):
+    all: bool = clickdc.option(
+        "-a",
+        is_flag=True,
+        help="Print logs from all allocations, including previous versions of the job.",
+    )
+    verbose: int = clickdc.option("-v", count=True, help="Be more verbose.")
+    quiet: int = clickdc.option("-q", count=True, help="Be less verbose.")
+    attach: bool = clickdc.option(
+        "-A",
+        is_flag=True,
+        help="""
+             Stop the job on receiving an SIGINT or SIGTERM signal.
+             Exit immediately after receiving a signal the second time.
+             """,
+    )
+    purge: bool = clickdc.option(
+        is_flag=True,
+        help="""
+             After the job is stopped, purge the job and wait until the job is purged.
+             Relevant in job, run, stop and stopped modes.
+             """,
+    )
+    purge_successful: bool = clickdc.option(
+        is_flag=True,
+        help="""
+             After the job is stopped and is successfull, purge the job and wait until it is purged.
+             Job is successfull if all job summary metrics are zero except nonzero complete metric.
+             Relevant in job, run, stop and stopped modes.
+             """,
+    )
+    json: bool = clickdc.option(
+        help="The job file is in JSON format",
+    )
+    lines: int = clickdc.option(
+        "-n",
+        default=30,
+        show_default=True,
+        help="""
+             Sets the tail location in best-efforted number of lines relative to the end of logs.
+             Negative value prints all available log lines.
+             """,
+    )
+    lines_timeout: float = clickdc.option(
+        default=2,
+        show_default=True,
+        help="When using --lines the number of lines is best-efforted by ignoring lines for this specific time",
+        callback=click_validate(lambda x: x >= 0, "timeout must be greater than 0"),
+    )
+    shutdown_timeout: float = clickdc.option(
+        default=2,
+        show_default=True,
+        help="The time to wait to make sure task loggers received all logs when exiting.",
+        callback=click_validate(lambda x: x >= 0, "timeout must be greater than 0"),
+    )
+    follow: bool = clickdc.option(
+        help="Never exit",
+    )
+    no_follow: bool = clickdc.option(
+        help="Just run once, get the logs in a best-effort style and exit.",
+    )
+    no_follow_timeout: float = clickdc.option(
+        default=3,
+        show_default=True,
+        help="The time to run in --no-follow mode.",
+        callback=click_validate(lambda x: x >= 0, "timeout must be greater than 0"),
+    )
+    task: Optional[re.Pattern] = clickdc.option(
+        "-t",
+        type=re.compile,
+        help="Only watch tasks names matching this regex.",
+    )
+    group: Optional[re.Pattern] = clickdc.option(
+        "-g",
+        type=re.compile,
+        help="Only watch group names matching this regex.",
+    )
+    node: Optional[re.Pattern] = clickdc.option(
+        type=re.compile,
+        help="Only watch tasks running on nodes whose names match this regex.",
+    )
+    polling: bool = clickdc.option(
+        help="Instead of listening to Nomad event stream, periodically poll for events.",
+    )
+    no_preserve_status: bool = clickdc.option(
+        "-x",
+        help="Do not preserve tasks exit statuses.",
+    )
+
+
 @click.group(
+    "watch",
     help="""
 Depending on the command, run or stop a Nomad job. Watch over the job and
 print all job allocation events and tasks stdouts and tasks stderrs
 logs. Depending on command, wait for a specific event to happen to finish
 watching. This program is intended to help debugging issues with running
 jobs in Nomad and for synchronizing with execution of batch jobs in Nomad.
 
@@ -1522,142 +1899,36 @@
 The mark in the log lines is equal to: 'deploy' for messages printed as
 a result of deployment, 'eval' for messages printed from evaluations,
 'A' from allocation, 'E' for stderr logs of a task and 'O' from stdout
 logs of a task.
 
 \b
 Examples:
-    nomad-watch run ./some-job.nomad.hcl
-    nomad-watch job some-job
-    nomad-watch alloc af94b2
-    nomad-watch -N services --task redis -1f job redis
+    watch run ./some-job.nomad.hcl
+    watch job some-job
+    watch alloc af94b2
+    watch -N services --task redis -1f job redis
 """,
     epilog="""
     Written by Kamil Cukrowski 2023. Licensed under GNU GPL version 3 or later.
     """,
 )
-@namespace_option()
-@click.option(
-    "-a",
-    "--all",
-    is_flag=True,
-    help="Print logs from all allocations, including previous versions of the job.",
-)
-@click.option("-v", "--verbose", count=True, help="Be more verbose.")
-@click.option("-q", "--quiet", count=True, help="Be less verbose.")
 @flagdebug.click_debug_option("NOMAD_WATCH_DEBUG")
-@click.option(
-    "-A",
-    "--attach",
-    is_flag=True,
-    help="""
-        Stop the job on receiving an SIGINT or SIGTERM signal.
-        Exit immediately after receiving a signal the second time.
-        """,
-)
-@click.option(
-    "--purge",
-    is_flag=True,
-    help="""
-        After the job is stopped, purge the job and wait until the job is purged.
-        Relevant in job, run, stop and stopped modes.
-        """,
-)
-@click.option(
-    "--purge-successful",
-    "purge_successful",
-    is_flag=True,
-    help="""
-        After the job is stopped and is successfull, purge the job and wait until it is purged.
-        Job is successfull if all job summary metrics are zero except nonzero complete metric.
-        Relevant in job, run, stop and stopped modes.
-        """,
-)
-@click.option(
-    "-n",
-    "--lines",
-    default=10,
-    show_default=True,
-    type=int,
-    help="""
-        Sets the tail location in best-efforted number of lines relative to the end of logs.
-        Negative value prints all available log lines.
-        """,
-)
-@click.option(
-    "--lines-timeout",
-    "lines_timeout",
-    default=0.5,
-    show_default=True,
-    type=float,
-    help="When using --lines the number of lines is best-efforted by ignoring lines for this specific time",
-)
-@click.option(
-    "--shutdown-timeout",
-    "shutdown_timeout",
-    default=1,
-    show_default=True,
-    type=float,
-    help="The time to wait to make sure task loggers received all logs when exiting.",
-)
-@click.option(
-    "-f",
-    "--follow",
-    is_flag=True,
-    help="Never exit",
-)
-@click.option(
-    "--no-follow",
-    "no_follow",
-    is_flag=True,
-    help="Just run once, get the logs in a best-effort style and exit.",
-)
-@click.option(
-    "--no-follow-timeout",
-    "no_follow_timeout",
-    default=3,
-    show_default=True,
-    type=float,
-    help="The time to run in --no-follow mode.",
-)
-@click.option(
-    "-t",
-    "--task",
-    type=re.compile,
-    help="Only watch tasks names matching this regex.",
-)
-@click.option(
-    "-g",
-    "--group",
-    type=re.compile,
-    help="Only watch group names matching this regex.",
-)
-@click.option(
-    "--polling",
-    is_flag=True,
-    help="Instead of listening to Nomad event stream, periodically poll for events.",
-)
-@click.option(
-    "-x",
-    "--no-preserve-status",
-    "no_preserve_status",
-    is_flag=True,
-    help="Do not preserve tasks exit statuses.",
-)
-@click_log_options()
+@clickdc.adddc("args", Args)
+@namespace_option()
 @common_options()
-def cli(**kwargs):
+def cli(args: Args):
     signal.signal(signal.SIGUSR1, print_all_threads_stacktrace)
     exit_on_thread_exception.install()
     global ARGS
-    ARGS = argparse.Namespace(**kwargs)
+    ARGS = args
     assert not (ARGS.follow and ARGS.no_follow), "--follow and --no-follow conflict"
     #
-    global START_NS
-    START_NS = time.time_ns()
+    global START_S
+    START_S = time.time()
     init_logging()
 
 
 cli_jobid = click.argument(
     "jobid",
     shell_complete=complete_job(),
 )
@@ -1813,15 +2084,21 @@
 
 @cli.command(
     "stop",
     help="Stop a Nomad job and then act like stopped command.",
 )
 @cli_jobid
 def mode_stop(jobid: str):
-    jobid = nomad_find_job(jobid)
+    try:
+        jobid = nomad_find_job(jobid)
+    except NoJobFound:
+        if ARGS.no_preserve_status and (ARGS.purge or ARGS.purge_successful):
+            return
+        else:
+            raise
     NomadJobWatcherUntilFinished(jobid).run_and_exit(True)
 
 
 @cli.command(
     "purge",
     help=f"""
 Alias to `--purge stop`, with the following difference in exit status.
@@ -1874,11 +2151,8 @@
     jobid = nomad_find_job(jobid)
     NomadJobWatcherUntilFinished(jobid).run_and_exit()
 
 
 ###############################################################################
 
 if __name__ == "__main__":
-    try:
-        cli.main()
-    finally:
-        mynomad.session.close()
+    cli.main()
```

### Comparing `nomad-tools-0.2.4/src/nomad_tools/nomaddbjob.py` & `nomad_tools-0.3.0/src/nomad_tools/nomaddbjob.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import logging
 import queue
 import threading
 from typing import Callable, Dict, Iterable, List, Optional, TypeVar, Union
 
 import requests
 
-from nomad_tools.nomadlib.types import JobStatus
-
 from . import flagdebug, nomadlib
 from .common import eprint, json_loads, mynomad
 from .nomadlib import Event, EventTopic, EventType
+from .nomadlib.types import JobStatus
 
 log = logging.getLogger(__name__)
 T = TypeVar("T")
 
 
 class NomadDbJob:
     """Represents relevant state cache from Nomad database of a single job"""
@@ -189,18 +188,15 @@
                 # and not eval.DeploymentID
             ):
                 self.job_deregistered_ModifyIndex = eval.ModifyIndex
                 actionstr = "JobDeregister because eval "
             actionstr += f"{eval}"
             self.evaluations[e.data["ID"]] = eval
         elif e.topic == EventTopic.Allocation:
-            # Events from event stream are missing JobVersion. Try to preserve it here by preserving keys.
-            self.allocations[e.data["ID"]] = nomadlib.Alloc(
-                {**self.allocations.get(e.data["ID"], {}), **e.data}
-            )
+            self.allocations[e.data["ID"]] = e.alloc()
         elif e.topic == EventTopic.Deployment:
             self.deployments[e.data["ID"]] = e.deployment()
         return actionstr
 
     def handle_event(self, e: Event) -> bool:
         if self._select_new_event(e):
             if self.select_is_in_db(e) or self.select_event_cb(e):
@@ -301,33 +297,41 @@
                 return evaluation.JobModifyIndex
             if evaluation.DeploymentID is not None:
                 deployment = self.deployments.get(evaluation.DeploymentID)
                 if deployment:
                     return deployment.JobModifyIndex
         return default
 
+    def get_evaluation_jobversion(
+        self, eval: nomadlib.Eval, default: T = None
+    ) -> Union[T, int]:
+        # If we can find Job from JobModifyIndex, lets find it.
+        if eval.JobModifyIndex is not None:
+            version = self.find_jobversion_from_modifyindex(eval.JobModifyIndex)
+            if version is not None:
+                return version
+        # Otherwise we may find deployment that may have jobversion.
+        if eval.DeploymentID is not None:
+            deployment = self.deployments.get(eval.DeploymentID)
+            if deployment:
+                return deployment.JobVersion
+        return default
+
     def get_allocation_jobversion(
         self, alloc: nomadlib.Alloc, default: T = None
     ) -> Union[T, int]:
         """Given an allocation return the job version associated with that allocation"""
-        # If alloc JobVersion is missing, try to set it.
-        if alloc.JobVersion is None:
-            evaluation = self.evaluations.get(alloc.EvalID)
-            if evaluation:
-                # If we can find Job from JobModifyIndex, lets find it.
-                if evaluation.JobModifyIndex is not None:
-                    job = self.find_job_from_modifyindex(evaluation.JobModifyIndex)
-                    if job is not None:
-                        alloc.JobVersion = job.Version
-                # Otherwise we may find deployment that may have jobversion.
-                if alloc.JobVersion is None and evaluation.DeploymentID is not None:
-                    deployment = self.deployments.get(evaluation.DeploymentID)
-                    if deployment:
-                        alloc.JobVersion = deployment.JobVersion
-        return alloc.JobVersion if alloc.JobVersion is not None else default
+        if False:
+            # This is unreliable.
+            if alloc.JobVersion:
+                return alloc.JobVersion
+        evaluation = self.evaluations.get(alloc.EvalID)
+        if evaluation:
+            return self.get_evaluation_jobversion(evaluation, default)
+        return default
 
     def find_job_from_modifyindex(self, jobmodifyindex: int) -> Optional[nomadlib.Job]:
         # Note that job versions may not be in JobModifyIndex order.
         # Job versions of previous job (after purge and start) may be here.
         # Sort explicitly over JobModifyIndex
         for job in sorted(
             self.jobversions.values(), key=lambda job: job.JobModifyIndex, reverse=True
```

### Comparing `nomad-tools-0.2.4/src/nomad_tools/nomadlib/_generator.py` & `nomad_tools-0.3.0/src/nomad_tools/nomadlib/_generator.py`

 * *Files identical despite different names*

### Comparing `nomad-tools-0.2.4/src/nomad_tools/nomadlib/connection.py` & `nomad_tools-0.3.0/src/nomad_tools/nomadlib/connection.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import atexit
 import base64
 import dataclasses
 import logging
 import os
 import ssl
 from abc import ABC, abstractmethod
 from typing import Any, Dict, Optional
@@ -11,14 +12,22 @@
 import websocket
 
 from ..common_base import cached_property
 from . import types
 
 log = logging.getLogger(__name__)
 
+NOMAD_NAMESPACE = "NOMAD_NAMESPACE"
+NOMAD_TOKEN = "NOMAD_TOKEN"
+NOMAD_HTTP_AUTH = "NOMAD_HTTP_AUTH"
+NOMAD_SKIP_VERIFY = "NOMAD_SKIP_VERIFY"
+NOMAD_CACERT = "NOMAD_CACERT"
+NOMAD_CLIENT_CERT = "NOMAD_CLIENT_CERT"
+NOMAD_CLIENT_KEY = "NOMAD_CLIENT_KEY"
+
 
 def _default_session():
     s = requests.Session()
     # Increase the number of connections.
     a = requests.adapters.HTTPAdapter(
         pool_connections=1000,
         pool_maxsize=1000,
@@ -26,17 +35,17 @@
     )
     s.mount("http://", a)
     s.mount("https://", a)
     return s
 
 
 class APIException(requests.HTTPError):
-    def __init__(self, e: requests.HTTPError):
+    def __init__(self, e: requests.HTTPError, msg: str = ""):
         """Just construct from other requests.HTTPError"""
-        super().__init__(request=e.request, response=e.response)
+        super().__init__(msg, request=e.request, response=e.response)
 
 
 class PermissionDenied(APIException):
     pass
 
 
 class JobNotFound(APIException):
@@ -115,21 +124,30 @@
     def delete(self, var_path: str, cas: Optional[int] = None):
         # request does not read DELETE response, so there is no JSON. Call requests, instead of wrapper above.
         self.r.request(
             "DELETE", var_path, params={cas: cas} if cas is not None else None
         )
 
 
+@dataclasses.dataclass
+class JobSubmission:
+    Source: str
+    Format: str
+    VariableFlags: Dict[str, str] = dataclasses.field(default_factory=dict)
+    Variables: str = ""
+
+
 class NomadConn(Requestor):
     """Represents connection to Nomad"""
 
     def __init__(self, namespace: str = "", session: Optional[requests.Session] = None):
         self.namespace = namespace
         self.session: requests.Session = session or _default_session()
         self.variables = VariableConn(self, "var")
+        atexit.register(self.session.close)
 
     @cached_property
     def nomad_version(self) -> str:
         agent = self.get("agent/self")
         version = agent["config"]["Version"]
         if isinstance(version, str):
             return version
@@ -145,70 +163,72 @@
         url: str,
         params: Optional[dict] = None,
         *args,
         **kvargs,
     ):
         params = dict(params or {})
         params.setdefault(
-            "namespace", self.namespace or os.environ.get("NOMAD_NAMESPACE", "*")
+            "namespace", self.namespace or os.environ.get(NOMAD_NAMESPACE, "*")
         )
         req = self.session.request(
             method,
             self.addr() + "/v1/" + url,
             *args,
             auth=(
-                requests.auth.HTTPBasicAuth(*os.environ["NOMAD_HTTP_AUTH"].split(":"))
-                if "NOMAD_HTTP_AUTH" in os.environ
+                requests.auth.HTTPBasicAuth(*os.environ[NOMAD_HTTP_AUTH].split(":", 2))
+                if NOMAD_HTTP_AUTH in os.environ
                 else None
             ),
             headers=(
-                {"X-Nomad-Token": os.environ["NOMAD_TOKEN"]}
-                if "NOMAD_TOKEN" in os.environ
+                {"X-Nomad-Token": os.environ[NOMAD_TOKEN]}
+                if NOMAD_TOKEN in os.environ
                 else None
             ),
             params=params,
-            verify=False
-            if "NOMAD_SKIP_VERIFY" in os.environ
-            else os.environ.get("NOMAD_CACERT"),
+            verify=(
+                False
+                if NOMAD_SKIP_VERIFY in os.environ
+                else os.environ[NOMAD_CACERT]
+                if NOMAD_CACERT in os.environ
+                else True
+            ),
             cert=(
-                (os.environ["NOMAD_CLIENT_CERT"], os.environ["NOMAD_CLIENT_KEY"])
-                if "NOMAD_CLIENT_CERT" in os.environ
-                and "NOMAD_CLIENT_KEY" in os.environ
+                (os.environ[NOMAD_CLIENT_CERT], os.environ[NOMAD_CLIENT_KEY])
+                if NOMAD_CLIENT_CERT in os.environ and NOMAD_CLIENT_KEY in os.environ
                 else None
             ),
             **kvargs,
         )
         try:
             req.raise_for_status()
         except requests.HTTPError as e:
             code = req.status_code
             text = req.text.lower()
             url = req.url
             if code == 500 and text == "permission denied":
                 raise PermissionDenied(e) from e
-            elif code == 404 and text == "job not found":
+            elif code == 404 and text in ["job not found", "job versions not found"]:
                 raise JobNotFound(e) from e
             elif "/v1/var/" in url and code == 404 and text == "variable not found":
                 raise VariableNotFound(e) from e
-            elif (
-                "/v1/client/fs/logs/" in url
-                and code in (404, 500)
-                and "no such file or directory" in text
-            ):
+            elif "/v1/client/fs/logs/" in url and code in (404, 500):
                 raise LogNotFound(e) from e
             else:
                 log.exception(f"{code} {text!r}")
             raise
         return req
 
     def jobhcl2json(self, hcl: str):
         return self.post("jobs/parse", json={"JobHCL": hcl})
 
-    def start_job(self, jobjson: dict, submission: Optional[str] = None):
-        return self.post("jobs", json={"Job": jobjson, "Submission": submission})
+    def start_job(self, jobjson: dict, submission: Optional[JobSubmission] = None):
+        data = {"Job": jobjson}
+        if submission:
+            data["Submission"] = dataclasses.asdict(submission)
+        return self.post("jobs", json=data)
 
     def stop_job(self, jobid: str, purge: bool = False):
         assert self.namespace
         resp: dict = self.delete(f"job/{jobid}", params={"purge": purge})
         assert resp["EvalID"], f"Stopping {jobid} did not trigger evaluation: {resp}"
         return resp
 
@@ -229,29 +249,29 @@
     # Replace http in address to ws
     addr: str = NomadConn.addr()
     if addr.startswith("http"):
         addr = "ws" + addr[4:]
     url: str = f"{addr}/{path}"
     # Build headers with authorization and token.
     headers: Dict[str, str] = {}
-    token = os.environ.get("NOMAD_TOKEN")
+    token = os.environ.get(NOMAD_TOKEN)
     if token:
         headers["X-Nomad-Token"] = token
-    auth = os.environ.get("NOMAD_HTTP_AUTH")
+    auth = os.environ.get(NOMAD_HTTP_AUTH)
     if auth:
         headers["Authorization"] = "Basic " + base64.b64encode(auth.encode()).decode()
     # Build SSL options from environment variables.
     sslopt: Dict[str, Any] = {}
-    skip_verify = os.environ.get("NOMAD_SKIP_VERIFY")
+    skip_verify = os.environ.get(NOMAD_SKIP_VERIFY)
     if skip_verify:
         sslopt["cert_reqs"] = ssl.CERT_NONE
         sslopt["check_hostname"] = False
-    cacert = os.environ.get("NOMAD_CACERT")
+    cacert = os.environ.get(NOMAD_CACERT)
     if cacert:
         sslopt["ca_cert_path"] = cacert
-    cert = os.environ.get("NOMAD_CLIENT_CERT")
-    key = os.environ.get("NOMAD_CLIENT_KEY")
+    cert = os.environ.get(NOMAD_CLIENT_CERT)
+    key = os.environ.get(NOMAD_CLIENT_KEY)
     if cert and key:
         sslopt["certfile"] = cert
         sslopt["keyfile"] = key
     # Make the connection.
     return websocket.create_connection(url, header=headers, sslopt=sslopt)
```

### Comparing `nomad-tools-0.2.4/src/nomad_tools/nomadlib/datadict.py` & `nomad_tools-0.3.0/src/nomad_tools/nomadlib/datadict.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,62 +1,68 @@
 from __future__ import annotations
 
 import copy
 import enum
+import logging
 from typing import Any, ChainMap, Type, Union, get_type_hints
 
+from typing_extensions import get_args, get_origin
+
+log = logging.getLogger(__name__)
+strict: bool = False
+
 
 def all_annotations(cls) -> ChainMap[str, Type]:
     """
     Returns a dictionary-like ChainMap that includes annotations for all
     attributes defined in cls or inherited from superclasses.
     Also resolve runtime type hints - https://peps.python.org/pep-0563/
     """
     return ChainMap(*(get_type_hints(c) for c in cls.__mro__))
 
 
 def _init_value(classname: str, dstname: str, dsttype: Any, srcval: Any):
     # print(f"Constructing {aname} with type {atype} from {val}")
-    dstorigin = getattr(dsttype, "__origin__", None)
+    dstorigin = get_origin(dsttype)
 
     def msg() -> str:
         return (
             f"Error when constructing class {classname!r} expected type {dsttype!r} with origin {dstorigin!r}"
             f" for field {dstname!r}, but received {type(srcval)} with value: {srcval!r}"
         )
 
     try:
         if dstorigin == list:
             assert type(srcval) is dstorigin, msg()
             return [
-                _init_value(classname, dstname, dsttype.__args__[0], x) for x in srcval
+                _init_value(classname, dstname, get_args(dsttype)[0], x) for x in srcval
             ]
         elif dstorigin == dict:
             assert type(srcval) is dstorigin, msg()
             return {
-                _init_value(classname, dstname, dsttype.__args__[0], k): _init_value(
-                    classname, dstname, dsttype.__args__[1], v
+                _init_value(classname, dstname, get_args(dsttype)[0], k): _init_value(
+                    classname, dstname, get_args(dsttype)[1], v
                 )
                 for k, v in srcval.items()
             }
         elif dstorigin == Union:
             if type(srcval) in dsttype.__args__:
                 return srcval
-            return _init_value(classname, dstname, dsttype.__args__[0], srcval)
+            return _init_value(classname, dstname, get_args(dsttype)[0], srcval)
         elif dsttype == Any:
             return srcval
         elif issubclass(dsttype, DataDict):
             return dsttype(srcval)
         elif issubclass(dsttype, enum.Enum):
             return dsttype(srcval)
-        return srcval
-    except AssertionError:
-        raise
     except Exception:
-        raise Exception(msg())
+        log.exception(f"DATADICT:ERROR: {msg()}")
+        if strict:
+            raise
+    return srcval
 
 
 def _asdict_value(fname: str, val: Any):
     if isinstance(val, list):
         return [_asdict_value(fname, x) for x in val]
     elif isinstance(val, dict):
         return {
```

### Comparing `nomad-tools-0.2.4/src/nomad_tools/nomadlib/tools.py` & `nomad_tools-0.3.0/src/nomad_tools/nomadlib/tools.py`

 * *Files identical despite different names*

### Comparing `nomad-tools-0.2.4/src/nomad_tools/nomadlib/types.py` & `nomad_tools-0.3.0/src/nomad_tools/nomadlib/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,19 +38,19 @@
     readonly: bool
 
 
 class JobTaskConfig(DataDict):
     image: str
     command: str
     args: List[str]
-    network_mode: str
-    network_aliases: List[str]
     volumes: List[str]
     mounts: List[DockerMounts]
     extra_hosts: List[str]
+    network_mode: str
+    init: bool
 
 
 class LifecycleHook(MyStrEnum):
     prestart = "prestart"
     poststart = "poststart"
     poststop = "poststop"
 
@@ -70,18 +70,18 @@
 
 
 class JobTask(DataDict):
     Name: str
     Driver: str
     User: str
     Config: Union[dict, JobTaskConfig]
-    Lifecycle: Optional[JobTaskLifecycle] = None
+    Lifecycle: Optional[JobTaskLifecycle]
     Env: Optional[Dict[str, str]]
     Services: Optional[List[Any]]
-    Templates: Optional[List[JobTaskTemplate]] = None
+    Templates: Optional[List[JobTaskTemplate]]
 
 
 class JobTaskGroup(DataDict):
     Name: str
     Count: int
     Tasks: List[JobTask]
     Services: Optional[List[Any]]
@@ -127,42 +127,43 @@
                     out += task.Services
         return out
 
 
 class JobsJob(DataDict):
     """Returned aby jobs API. DO NOT mix with Job"""
 
+    Namespace: Optional[str]
     ID: str
 
 
 class NodeScoreMeta(DataDict):
     NodeID: str
     Scores: Dict[str, float]
     NormScore: float
 
 
 class AllocationMetric(DataDict):
     NodesEvaluated: int
     NodesFiltered: int
-    NodesAvailable: Dict[str, int]
+    NodesExhausted: int
+    NodesAvailable: Optional[Dict[str, int]] = None
     ClassFiltered: Optional[Dict[str, int]] = None
     ConstraintFiltered: Optional[Dict[str, int]] = None
-    NodesExhausted: int
     QuotaExhausted: Optional[Dict[str, int]] = None
     ScoreMetaData: Optional[List[NodeScoreMeta]] = None
     ClassExhausted: Optional[Dict[str, int]] = None
     Scores: Optional[Dict[str, float]] = None
     DimensionExhausted: Optional[Dict[str, int]] = None
 
     def format(self, scores: bool = False, prefix: str = "") -> str:
         """https://github.com/hashicorp/nomad/blob/484f91b893c6f054e9339f8db6bd157429c2ef20/command/monitor.go#L345"""
         out = []
         if self.NodesEvaluated == 0:
             out += ["No nodes were eligible for evaluation"]
-        for dc, available in self.NodesAvailable.items():
+        for dc, available in (self.NodesAvailable or {}).items():
             if available == 0:
                 out += [f"No nodes are available in datacenter {dc}"]
         for cls, num in (self.ClassFiltered or {}).items():
             out += [f"Class {cls}: {num} nodes excluded by filter"]
         for cs, num in (self.ConstraintFiltered or {}).items():
             out += [f"Constraint {cs}: {num} nodes excluded by filter"]
         ne = self.NodesExhausted
@@ -206,24 +207,24 @@
 def fromisoformat(txt: str) -> datetime.datetime:
     return dateutil.parser.isoparse(txt)
 
 
 class Eval(DataDict):
     ID: str
     Namespace: str
-    DeploymentID: Optional[str] = None
-    """May be missing when evaluation started by user starting the job"""
     JobID: str
-    JobModifyIndex: Optional[int] = None
-    """May be missing. No idea when"""
     ModifyIndex: int
     ModifyTime: int
     Status: str
     WaitUntil: str
     FailedTGAllocs: Dict[str, AllocationMetric]
+    DeploymentID: Optional[str] = None
+    """May be missing when evaluation started by user starting the job"""
+    JobModifyIndex: Optional[int] = None
+    """May be missing. No idea when"""
     TriggeredBy: Optional[str] = None
 
     def is_pending_or_blocked(self):
         return self.Status in [EvalStatus.pending, EvalStatus.blocked]
 
     def is_blocked(self):
         return self.Status == EvalStatus.blocked
@@ -346,14 +347,15 @@
     unknown = enum.auto()
 
 
 class Alloc(DataDict):
     ID: str
     Name: str
     NodeName: str
+    NodeID: str
     JobID: str
     EvalID: str
     ClientStatus: str
     DesiredStatus: str
     CreateTime: int
     Namespace: str
     ModifyIndex: int
@@ -426,19 +428,19 @@
 class DeploymentTaskGroup(DataDict):
     AutoPromote: bool
     AutoRevert: bool
     DesiredCanaries: int
     DesiredTotal: int
     HealthyAllocs: int
     PlacedAllocs: int
-    PlacedCanaries: Optional[List[str]] = None
     ProgressDeadline: int
     Promoted: bool
     RequireProgressBy: Optional[str]
     UnhealthyAllocs: int
+    PlacedCanaries: Optional[List[str]] = None
 
 
 class Deploy(DataDict):
     ID: str
     ModifyIndex: int
     JobCreateIndex: int
     JobModifyIndex: int
@@ -610,18 +612,18 @@
         for k in set(self.asdict()) | set(o.asdict()):
             self[k] = self.get(k, 0) + o.get(k, 0)
         return self
 
 
 class JobSummary(DataDict):
     JobID: str
-    Summary: Dict[str, JobSummarySummary]
-    Children: JobSummaryChildren
     CreateIndex: int
     ModifyIndex: int
+    Summary: Optional[Dict[str, JobSummarySummary]] = None
+    Children: Optional[JobSummaryChildren] = None
 
     def get_sum_summary(self) -> JobSummarySummary:
         """Sum all summaries into one"""
-        ret = JobSummarySummary({})
-        for s in self.Summary.values():
+        ret = JobSummarySummary()
+        for s in (self.Summary or {}).values():
             ret += s
         return ret
```

### Comparing `nomad-tools-0.2.4/src/nomad_tools/nomadt_completion.sh` & `nomad_tools-0.3.0/src/nomad_tools/nomadt_completion.sh`

 * *Files identical despite different names*

### Comparing `nomad-tools-0.2.4/src/nomad_tools/taskexec.py` & `nomad_tools-0.3.0/src/nomad_tools/taskexec.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,47 @@
 from __future__ import annotations
 
 import base64
-import dataclasses
+import functools
 import io
 import json
 import logging
+import os
 import subprocess
-import sys
+import threading
 import urllib.parse
 from typing import (
     IO,
     Any,
     BinaryIO,
+    Dict,
     Generic,
     Iterator,
     List,
     Optional,
     Set,
+    TextIO,
     Tuple,
     TypeVar,
     Union,
     cast,
-    overload,
 )
 
 import websocket
-from typing_extensions import Literal, override
+from typing_extensions import Literal, overload
 
 from . import nomadlib
 from .common_base import eprint
-from .common_nomad import mynomad, nomad_find_job
+from .common_nomad import mynomad
+from .nomadlib.datadict import DataDict
 from .nomadlib.types import Alloc
 
 log = logging.getLogger(__name__)
 log.setLevel(level=logging.INFO)
 
-DEVNULL = subprocess.DEVNULL
-PIPE = subprocess.PIPE
-CompletedProcess = subprocess.CompletedProcess
-_DESTFILE = Union[int, IO[Any]]
-_FILE = Optional[_DESTFILE]
-_StrAny = Union[bytes, str]
-_InputString = Optional[_StrAny]
-
 
 def find_alloc_task(
     allocid: Optional[str], task: Optional[str] = None, job: Optional[str] = None
 ) -> Tuple[str, str]:
     """Find allocation and task name given the search parameters."""
     allocation: Optional[Alloc] = None
     if allocid:
@@ -85,14 +80,148 @@
     Given a job, return its running allocation id and task.
     There has to be exactly one running allocation of that job.
     That allocation has to have exactly one task.
     """
     return find_alloc_task(None, None, job)
 
 
+###############################################################################
+
+
+class FrameData(DataDict):
+    data: Optional[str] = None
+    close: Optional[bool] = None
+
+
+class FrameResult(DataDict):
+    exit_code: int = 0
+
+
+class ExecStreamingOutput(DataDict):
+    stderr: Optional[FrameData] = None
+    stdout: Optional[FrameData] = None
+    exited: Optional[bool] = None
+    result: Optional[FrameResult] = None
+
+
+class TaskExec:
+    """Abstraction over Nomad websocket API for running argument in task"""
+
+    def __init__(self, allocid: str, task: str, args: List[str]):
+        assert allocid
+        assert task
+        assert args
+        self.name: str = f"{self.__class__.__name__}({allocid}/{task},{args})"
+        self.__closed: Set[str] = set()
+        """Protect against double closing"""
+        self.returncode: Optional[int] = None
+        # Connect to the remote side.
+        path = f"v1/client/allocation/{allocid}/exec?" + urllib.parse.urlencode(
+            dict(task=task, command=json.dumps(args))
+        )
+        log.debug(f"CONNECT {path!r}")
+        self.ws: websocket.WebSocket = nomadlib.create_websocket_connection(path)
+        self.__readergen = self.__reader()
+        assert self.ws.connected
+
+    def __reader(self) -> Iterator[bytes]:
+        while self.ws.connected:
+            line = self.ws.recv()
+            log.debug(f"R: {line}")
+            if not line:
+                break
+            frame = ExecStreamingOutput(json.loads(line))
+            if frame.stderr:
+                if frame.stderr.data:
+                    txt: str = base64.b64decode(frame.stderr.data.encode()).decode(
+                        errors="replace"
+                    )
+                    eprint(txt, end="")
+            if frame.stdout:
+                if frame.stdout.data:
+                    yield base64.b64decode(frame.stdout.data.encode())
+            if frame.exited and frame.result:
+                self.returncode = frame.result.exit_code
+                break
+        self.terminate()
+
+    def __send(self, msg: str):
+        try:
+            self.ws.send(msg)
+        except BrokenPipeError:
+            self.ws.close()
+            raise
+
+    def __close_stream(self, stream: str):
+        """Send message to Nomad to close specific stream"""
+        if not self.ws.connected:
+            return
+        if stream in self.__closed:
+            return
+        self.__closed.add(stream)
+        msg = json.dumps({stream: {"close": True}})
+        log.debug(f"W {msg}")
+        self.__send(msg)
+
+    def close_stdin(self):
+        # Only stdin is handled in Nomad
+        # https://github.com/hashicorp/nomad/blob/695bb7ffcf90fc9455152dadd2a504bc4499e3b3/plugins/drivers/execstreaming.go#L41
+        return self.__close_stream("stdin")
+
+    def terminate(self):
+        if self.ws.connected:
+            log.debug("closing ws")
+            self.ws.close()
+
+    def wait(self):
+        if not self.ws.connected:
+            return
+        self.close_stdin()
+        self.read()
+
+    def read(self) -> bytes:
+        return functools.reduce(bytes.__add__, self.read1(), b"")
+
+    def read1(self) -> Iterator[bytes]:
+        return self.__readergen
+
+    def write(self, s: bytes):
+        msg = json.dumps({"stdin": {"data": base64.b64encode(s).decode()}})
+        log.debug(f"W stdin:data:{s!r}")
+        self.__send(msg)
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.terminate()
+
+    def raise_for_returncode(self, output: Optional[Union[str, bytes]] = None):
+        if self.returncode is None:
+            raise Exception(
+                f"when executing {self.name}"
+                "the websocket was closed by Nomad server without sending the exit code of the process."
+            )
+        if self.returncode:
+            raise subprocess.CalledProcessError(self.returncode, self.name, output)
+
+
+###############################################################################
+
+
+DEVNULL = subprocess.DEVNULL
+PIPE = subprocess.PIPE
+CompletedProcess = subprocess.CompletedProcess
+_IoAny = Union[IO[bytes], IO[str]]
+_DESTFILE = Union[int, _IoAny]
+_FILE = Optional[_DESTFILE]
+_StrAny = Union[bytes, str]
+_InputString = Optional[_StrAny]
+
+
 T = TypeVar("T", bytes, str)
 
 
 class NomadPopen(Generic[T]):
     """
     An implementation of subprocess.Popen on top of Nomad Exec Alocation API.
     https://developer.hashicorp.com/nomad/api-docs/allocations#exec-allocation
@@ -101,256 +230,177 @@
 
     @overload
     def __init__(
         self: NomadPopen[bytes],
         allocid: str,
         task: str,
         args: List[str],
-        job: Optional[str] = ...,
         stdin: _FILE = ...,
         stdout: _FILE = ...,
         text: Literal[False] = ...,
     ) -> None:
         ...
 
     @overload
     def __init__(
         self: NomadPopen[str],
         allocid: str,
         task: str,
         args: List[str],
-        job: Optional[str] = ...,
         stdin: _FILE = ...,
         stdout: _FILE = ...,
         text: Literal[True] = ...,
     ) -> None:
         ...
 
     @overload
     def __init__(
         self: NomadPopen[bytes],
         allocid: str,
         task: str,
         args: List[str],
-        job: Optional[str] = ...,
         stdin: _FILE = ...,
         stdout: _FILE = ...,
         text: bool = ...,
     ) -> None:
         ...
 
     def __init__(
         self,
         allocid: str,
         task: str,
         args: List[str],
-        job: Optional[str] = None,
         stdin: _FILE = None,
         stdout: _FILE = None,
         text: bool = False,
     ):
-        assert allocid
-        assert task
-        assert args
-        assert stdin is None or stdin == PIPE
-        self.cmd = [allocid, task] + args
-        self.__stdin_arg: _DESTFILE = DEVNULL if stdin is None else stdin
-        self.__stdout_arg: _DESTFILE = sys.stdout if stdout is None else stdout
-        #
-        self.__closed: Set[str] = set()
-        """Protect against double closing"""
-        self.__returncode: Optional[int] = None
-        self._reader = self.__readergen()
+        self.np = TaskExec(allocid, task, args)
         self.text = text
-        # Connect to the remote side.
-        path = f"v1/client/allocation/{allocid}/exec?" + urllib.parse.urlencode(
-            dict(task=task, command=json.dumps(args))
-        )
-        log.debug(f"CONNECT {path!r} text={text}")
-        self.ws: Optional[websocket.WebSocket] = nomadlib.create_websocket_connection(
-            path
-        )
-        # Initialize self.stdin
+        self.__initialize_stdin(self.__stdin_to_fd(stdin))
+        self.__initialize_stdout(self.__stdout_to_fd(stdout))
+
+    def __stdin_to_fd(self, stdin: _FILE) -> Optional[IO[bytes]]:
         self.stdin: Optional[IO[T]] = None
-        if self.__stdin_arg == DEVNULL:
-            self._close_stream("stdin")
-        elif self.__stdin_arg == PIPE:
-            stream = self.Stdin(self)
-            if self.text:
-                stream = io.TextIOWrapper(stream)
-            self.stdin = cast(IO[T], stream)
+        if stdin == DEVNULL or stdin is None:
+            return None
+        elif isinstance(stdin, BinaryIO):
+            return stdin
+        elif isinstance(stdin, TextIO):
+            return stdin.buffer
+        elif stdin == PIPE:
+            pipe = os.pipe()
+            self.stdin = os.fdopen(pipe[1], "w" if self.text else "wb")
+            return os.fdopen(pipe[0], "rb")
+        elif isinstance(stdin, int) and stdin >= 0:
+            return os.fdopen(stdin, "rb")
         else:
-            assert 0, f"Unhandled stdin={self.__stdin_arg}"
-        # Initialize self.stdout
+            assert 0, f"Unhandled stdin={stdin}"
+
+    def __stdout_to_fd(self, stdout: _FILE) -> IO[bytes]:
         self.stdout: Optional[IO[T]] = None
-        if self.__stdout_arg == DEVNULL:
-            self._close_stream("stdout")
-        elif self.__stdout_arg is sys.stdout:
+        if stdout == DEVNULL or stdout is None:
             pass
-        elif self.__stdout_arg == PIPE:
-            stream = self.Stdout(self)
-            if self.text:
-                stream = io.TextIOWrapper(stream)
-            self.stdout = cast(IO[T], stream)
+        elif isinstance(stdout, BinaryIO):
+            return stdout
+        elif isinstance(stdout, TextIO):
+            return stdout.buffer
+        elif stdout == PIPE:
+            pipe = os.pipe()
+            self.stdout = os.fdopen(pipe[0], "r" if self.text else "rb")
+            return os.fdopen(pipe[1], "wb")
+        elif isinstance(stdout, int) and stdout >= 0:
+            return os.fdopen(stdout, "wb")
         else:
-            assert 0, f"Unhandled stdout={self.__stdout_arg}"
+            assert 0, f"Unhandled stdout={self.stdout}"
+        return open(os.devnull, "wb")
+
+    def __initialize_stdin(self, fd: Optional[IO[bytes]]):
+        if fd is not None:
 
-    def __output(self, buf: bytes) -> Iterator[int]:
-        log.debug(f"RRAW len={len(buf)} {self.__stdout_arg}")
-        if self.__stdout_arg is sys.stdout:
-            sys.stdout.buffer.write(buf)
-        elif self.__stdout_arg == PIPE:
-            for c in buf:
-                yield c
+            def writer():
+                try:
+                    with fd as f:
+                        # Use read1 if available.
+                        for buf in (
+                            iter(f.read1, b"")
+                            if isinstance(f, io.BufferedIOBase)
+                            else f
+                        ):
+                            self.np.write(buf)
+                except BrokenPipeError:
+                    pass
+                except Exception as e:
+                    log.exception(e)
+                finally:
+                    self.np.close_stdin()
+
+            threading.Thread(
+                name=f"{self.np.name}WRITER", target=writer, daemon=True
+            ).start()
         else:
-            assert 0, f"Unhandled stdout={self.__stdout_arg}"
+            self.np.close_stdin()
 
-    def __readergen(self) -> Iterator[int]:
-        while self.ws:
-            line = self.ws.recv()
-            if not line:
-                break
-            frame: dict = json.loads(line)
-            fstderr: Optional[dict] = frame.get("stderr")
-            if fstderr:
-                data: Optional[str] = fstderr.get("data")
-                if data:
-                    txt: str = base64.b64decode(data.encode()).decode(errors="replace")
-                    eprint(txt, end="")
-            fstdout: Optional[dict] = frame.get("stdout")
-            if fstdout:
-                data: Optional[str] = fstdout.get("data")
-                if data:
-                    buf = base64.b64decode(data.encode())
-                    for c in self.__output(buf):
-                        yield c
-            fexited = frame.get("exited")
-            if fexited:
-                self.__returncode = frame["result"].get("exit_code", 0)
-                break
+    def __initialize_stdout(self, fd: IO[bytes]):
+        def reader():
+            try:
+                with fd as f:
+                    for buf in self.np.read1():
+                        f.write(buf)
+            except BrokenPipeError:
+                pass
+            except Exception as e:
+                log.exception(e)
+
+        self.readthread = threading.Thread(
+            name=f"{self.np.name}READER", target=reader, daemon=True
+        )
+        self.readthread.start()
+
+    ###############################################################################
+
+    @property
+    def name(self):
+        return self.np.name
 
     def __enter__(self):
         return self
 
     def communicate(
         self, input: Optional[Union[str, bytes]] = None
     ) -> Tuple[Optional[Union[str, bytes]], None]:
         if input:
-            assert self.__stdin_arg == PIPE
             assert self.stdin
-            assert isinstance(input, str) if self.text else isinstance(input, bytes)
+            assert isinstance(input, str if self.text else bytes)
             self.stdin.write(cast(T, input))
+        if self.stdin:
             self.stdin.close()
         output: Optional[T] = None
-        if self.__stdout_arg == PIPE:
-            assert self.stdout
+        if self.stdout:
             output = self.stdout.read()
-            assert isinstance(output, str) if self.text else isinstance(output, bytes)
+            assert isinstance(output, str if self.text else bytes)
         return output, None
 
     @property
-    def returncode(self):
-        assert (
-            self.__returncode is not None
-        ), f"nomad alloc exec {self.cmd} not finished"
-        return self.__returncode
+    def returncode(self) -> Optional[int]:
+        return self.np.returncode
 
-    def wait(self):
-        assert self.ws
-        self._close_stream("stdin")
-        for _ in self._reader:
-            pass
-        if self.__returncode is None:
-            raise Exception(
-                f"when executing nomad alloc exec {self.cmd}"
-                "the websocket was closed by Nomad server without sending the exit code of the process."
-            )
-        log.debug("closing")
-        self.ws.close()
-        self.ws = None
+    def wait(self, timeout: Optional[float] = None):
+        self.readthread.join(timeout)
+
+    def terminate(self):
+        self.np.terminate()
 
     def __exit__(self, exc_type, exc_val, exc_tb):
+        if exc_type:
+            self.terminate()
         self.wait()
 
-    def _close_stream(self, stream: str):
-        """Send message to Nomad to close specific stream"""
-        assert self.ws
-        if stream in self.__closed:
-            return
-        self.__closed.add(stream)
-        msg = json.dumps({stream: {"close": True}})
-        log.debug(f"W {msg}")
-        try:
-            self.ws.send(msg)
-        except BrokenPipeError:
-            self.ws.close()
-            self.ws = None
-            raise
-
-    def write(self, s: bytes) -> int:
-        assert isinstance(s, bytes)
-        assert self.ws
-        msg = json.dumps({"stdin": {"data": base64.b64encode(s).decode()}})
-        log.debug(f"W stdin:data:{s!r}")
-        return self.ws.send(msg)
-
-    def read(self, size: int = -1) -> bytes:
-        acc: bytearray = bytearray()
-        for c in self._reader:
-            acc.append(c)
-            if size != -1 and len(acc) == size:
-                break
-        accbytes = bytes(acc)
-        log.debug(f"R({size}) {accbytes!r}")
-        return accbytes
-
-    @dataclasses.dataclass
-    class Stdin(BinaryIO):
-        p: NomadPopen
-
-        @override
-        def fileno(self) -> int:
-            return -1
-
-        @override
-        def writable(self) -> bool:
-            return True
-
-        @override
-        def write(self, s) -> int:
-            assert isinstance(s, bytes)
-            return self.p.write(s)
-
-        @override
-        def close(self):
-            self.p._close_stream("stdin")
-
-    @dataclasses.dataclass
-    class Stdout(BinaryIO):
-        p: NomadPopen
-
-        @override
-        def fileno(self) -> int:
-            return -1
-
-        @override
-        def readable(self) -> bool:
-            return True
-
-        @override
-        def read(self, size: int = -1) -> bytes:
-            return self.p.read(size)
-
-        @override
-        def close(self):
-            self.p._close_stream("stdout")
-
     def raise_for_returncode(self, output: Optional[Union[str, bytes]] = None):
-        if self.returncode:
-            raise subprocess.CalledProcessError(self.returncode, self.cmd, output, None)
+        self.readthread.join()
+        self.np.raise_for_returncode()
 
 
 ###############################################################################
 
 
 @overload
 def run(
@@ -415,15 +465,17 @@
         stdin=PIPE if input else stdin,
         stdout=stdout,
         text=text,
     ) as p:
         output = p.communicate(input)[0]
     if check:
         p.raise_for_returncode(output)
-    return CompletedProcess(cmd, p.returncode, output, None)
+    return CompletedProcess(
+        cmd, p.returncode if p.returncode is not None else 400, output, None
+    )
 
 
 ###############################################################################
 
 
 @overload
 def check_output(
@@ -488,37 +540,65 @@
 ###############################################################################
 
 if __name__ == "__main__":
     import argparse
 
     logging.basicConfig(level=logging.DEBUG)
     parser = argparse.ArgumentParser()
-    parser.add_argument("--input")
+    parser.add_argument("-i", "--input")
     parser.add_argument("--trace", action="store_true")
-    parser.add_argument("--debug", action="store_true")
-    parser.add_argument("--text", action="store_false")
+    parser.add_argument("-d", "--debug", action="store_true")
+    parser.add_argument("-t", "--text", action="store_true")
     parser.add_argument(
+        "-m",
         "--mode",
-        choices="check_output run".split(),
+        choices="check_output run popen".split(),
         default="check_output",
     )
+    parser.add_argument("--stdin", "--in", default=str(subprocess.PIPE))
+    parser.add_argument("--stdout", "--out", default=str(subprocess.PIPE))
     parser.add_argument("job")
     parser.add_argument("task")
     parser.add_argument("cmd", nargs="+")
     args = parser.parse_args()
     if args.trace:
         websocket.enableTrace(True)
     if args.debug:
         log.setLevel(level=logging.DEBUG)
-    print(args)
-    job = nomad_find_job(args.job)
+    print("ARGS", args)
+    # spec = find_job(args.job)
     allocid = find_job_alloc(args.job, args.task)
     if args.mode == "check_output":
         output = ""
         try:
             output = check_output(
                 allocid, args.task, args.cmd, input=args.input, text=args.text
             ).strip()
         finally:
             print(output)
     elif args.mode == "run":
         run(allocid, args.task, args.cmd, input=args.input, text=args.text)
+    elif args.mode == "popen":
+
+        def parse_stream(txt: str) -> int:
+            map = {"pipe": subprocess.PIPE, "null": subprocess.DEVNULL, "none": None}
+            return map[txt.lower()] if txt.lower() in map else int(txt)
+
+        ppargs: Dict[str, Any] = dict(
+            allocid=allocid,
+            task=args.task,
+            args=args.cmd,
+            stdin=parse_stream(args.stdin),
+            stdout=parse_stream(args.stdout),
+            text=args.text,
+        )
+        print(f"PIPE={subprocess.PIPE} DEVNULL={subprocess.DEVNULL}")
+        print(f"NomadPopen({ppargs})")
+        with NomadPopen(**ppargs) as pp:
+            out = pp.communicate(
+                None
+                if args.input is None
+                else args.input
+                if args.text
+                else args.input.encode()
+            )
+            print(f"{out[0]!r}")
```

### Comparing `nomad-tools-0.2.4/src/nomad_tools.egg-info/PKG-INFO` & `nomad_tools-0.3.0/src/nomad_tools.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 Metadata-Version: 2.1
 Name: nomad-tools
-Version: 0.2.4
+Version: 0.3.0
 Summary: Set of tools and utilities to ease interacting with Hashicorp Nomad scheduling solution.
 Author: Kamil Cukrowski
 License: GPL-3.0-or-later
 Project-URL: homepage, https://github.com/Kamilcuk/nomad-tools
 Project-URL: repository, https://github.com/Kamilcuk/nomad-tools
 Project-URL: documentation, https://github.com/Kamilcuk/nomad-tools
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: click
-Requires-Dist: requests
-Requires-Dist: setuptools
-Requires-Dist: pyyaml
-Requires-Dist: python-dateutil
-Requires-Dist: typing-extensions
-Requires-Dist: websocket-client
+Requires-Dist: click==8.1.7
+Requires-Dist: python-dateutil==2.8.2
+Requires-Dist: PyYAML==6.0.1
+Requires-Dist: requests==2.31.0
+Requires-Dist: typing_extensions==4.7.1
+Requires-Dist: websocket-client==1.6.1
+Requires-Dist: clickdc==0.0.5
+Requires-Dist: clickforward==0.0.1
+Requires-Dist: python-dotenv==0.21.1
+Requires-Dist: packaging>=16.1
 Provides-Extra: test
-Requires-Dist: tomli; extra == "test"
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-xdist; extra == "test"
-Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: tomli==2.0.1; extra == "test"
+Requires-Dist: pytest==7.4.4; extra == "test"
+Requires-Dist: pytest-xdist==3.5.0; extra == "test"
+Requires-Dist: pytest-cov==4.1.0; extra == "test"
 
-# nomad-tools
+# nomadtools
 
 Set of tools and utilities to ease interacting with HashiCorp Nomad scheduling solution.
 
 ## Table of Contents
 
 <!-- vim-markdown-toc GFM -->
 
 * [Installation](#installation)
     * [Shell completion](#shell-completion)
 * [Usage](#usage)
-    * [nomadt](#nomadt)
-    * [nomad-watch](#nomad-watch)
-    * [nomad-port](#nomad-port)
-    * [nomad-vardir](#nomad-vardir)
-    * [nomad-cp](#nomad-cp)
-    * [nomad-gitlab-runner](#nomad-gitlab-runner)
+    * [watch](#watch)
+    * [go](#go)
+    * [port](#port)
+    * [vardir](#vardir)
+    * [cp](#cp)
+    * [gitlab-runner](#gitlab-runner)
     * [nomad-dockers](#nomad-dockers)
-    * [nomad-downloadrelease](#nomad-downloadrelease)
+    * [downloadrelease](#downloadrelease)
     * [import nomad_tools](#import-nomad_tools)
+* [History](#history)
 * [Contributing](#contributing)
     * [Running tests](#running-tests)
 * [License](#license)
 
 <!-- vim-markdown-toc -->
 
 # Installation
@@ -53,210 +57,245 @@
 This is a bundle of executables packages together in a PyPY package. Install
 using `pipx` project.
 
 ```
 pipx install nomad-tools
 ```
 
+After installation the executable `nomadtools` should be available.
+
+```
+nomadtools --help
+```
+
 ## Shell completion
 
-After installation, see `nomad-watch --autocomplete-info` for shell
+After installation, see `nomadtools watch --autocomplete-info` for shell
 completion installation instruction.
 
 # Usage
 
-This module install several command line tools:
+This module installs command line tool `nomadtools` with several modes of
+operation:
 
-## nomadt
+## watch
 
-`nomadt` is a wrapper around `nomad` commands and `nomad-anything`
-command. If a `nomad` sub-command exists, `nomad` will be run. Otherwise
-an executable `nomad-subcommand` will be executed for a given sub-command.
-
-The intention is that you can do `alias nomad=nomadt` and use it seamlessly.
-
-```
-nomadt job run example.nomad.hcl    # will execute nomad job run example.nomad.hcl
-nomadt watch run example.nomad.hcl  # will execute nomad-watch run example.nomad.hcl
-```
-
-## nomad-watch
-
-Nomad-watch is meant to watch over a job change that you type in
+`nomadtools watch` is meant to watch over a job change that you type in
 terminal. It prints all relevant messages - messages about allocation,
 evaluation, deployment and stdout and stderr logs from all the
 processes. Depending on the mode of operation, the tool waits until an
 action is finished.
 
-I primarily use nomad-watch to deploy new versions of services. I was always
+I primarily use `watch` to deploy new versions of services. I was always
 frustrated that I start something from terminal and then I have to check the
 logs of the service in multiple tabs in the Nomad web interface. For example,
-you can use `nomad-watch start ./postgres.nomad.hcl` to update postgres
+you can use `watch start ./postgres.nomad.hcl` to update PostgreSQL
 container and watch it's logs in your terminal.
 
 An example terminal session deploying a HTTP server job with canary and health
 check. Note that while the new version is deployed, the old one still prints
 the logs.
 
-![gif showing example usage of nomad-watch start](./assets/imgs/nomad-watch-start-listen.gif)
+![gif showing example usage of watch start](./assets/imgs/nomad-watch-start-listen.gif)
 
 Another usage of the job is to run an one-shot batch jobs to do something and
 wait until they are finished and collect the exit status and logs, for example
 as an airflow or cron job. In this case `run` mode will wait for the job to be
-finished. For example `nomad-watch --purge run ./compute.nomad.hcl` will run
+finished. For example `watch --purge run ./compute.nomad.hcl` will run
 a calculation job, purge after it is done and exit with calculate job exit
 status (if there is one task).
 
-![gif showing example usage of nomad-watch run](./assets/imgs/nomad-watch-run-compute.gif)
+![gif showing example usage of watch run](./assets/imgs/nomad-watch-run-compute.gif)
 
-Internally, nomad-watch uses Nomad event stream to get the events in real time.
+Internally, watch uses Nomad event stream to get the events in real time.
 
-## nomad-port
+## go
+
+Mimics operation of `docker run`, it is built on top of `watch` mode to
+execute a single Nomad job created dynamically from command line arguments.
+It creates a Nomad job specification from command line arguments and then
+"watches" over the execution of the job.
+
+```
+$ nomadtools go --rm alpine apk add bash
+INFO:nomad_tools.nomad_watch:Watching job nomad_tools_go_5305da8f-b376-4c35-9a05-71027aadd587@default until it is finished
+Allocation 70c4ac9d-0e03-53d7-6e34-9c86cf8ee768 started on leonidas
+Received Task received by client
+Task Setup Building Task Directory
+Driver Downloading image
+Started Task started by client
+INFO:nomad_tools.nomad_watch:Job nomad_tools_go_5305da8f-b376-4c35-9a05-71027aadd587#0@default started allocations 70c4ac running group 'nomad_tools_go_5305da8f-b376-4c35-9a05-71027aadd587' with 1 main tasks.
+fetch https://dl-cdn.alpinelinux.org/alpine/v3.19/main/x86_64/APKINDEX.tar.gz
+fetch https://dl-cdn.alpinelinux.org/alpine/v3.19/community/x86_64/APKINDEX.tar.gz
+(1/4) Installing ncurses-terminfo-base (6.4_p20231125-r0)
+(2/4) Installing libncursesw (6.4_p20231125-r0)
+(3/4) Installing readline (8.2.1-r2)
+(4/4) Installing bash (5.2.21-r0)
+Terminated Exit Code: 0
+Allocation 70c4ac9d-0e03-53d7-6e34-9c86cf8ee768 finished
+Executing bash-5.2.21-r0.post-install
+Executing busybox-1.36.1-r15.trigger
+OK: 10 MiB in 19 packages
+INFO:nomad_tools.nomad_watch:Purging job nomad_tools_go_5305da8f-b376-4c35-9a05-71027aadd587
+INFO:nomad_tools.nomad_watch:Job nomad_tools_go_5305da8f-b376-4c35-9a05-71027aadd587#0@default purged with no active allocations, evaluations nor deployments. Exiting.
+INFO:nomad_tools.nomad_watch:Single task exited with 0 exit status. Exit code is 0.
+```
+
+## port
 
 Prints out the ports allocated for a particular Nomad job or
 allocation. It is meant to mimic `docker port` command.
 
 ```
-$ nomad-port httpd
+$ nomadtools port httpd
 192.168.0.5:31076
-$ nomad-port -l httpd
+$ nomadtools port -l httpd
 192.168.0.5 31076 http httpd.listen[0] d409e855-bf13-a342-fe7a-6fb579d2de85
-$ nomad-port --alloc d409e855
+$ nomadtools port --alloc d409e855
 192.168.0.5:31076
 ```
 
 Further argument allows to filter for port label.
 
 ```
-$ nomad-port httpd http
+$ nomadtools port httpd http
 192.168.0.5:31076
 ```
 
-## nomad-vardir
+## vardir
 
 I was frustrated with how Nomad variables look like. It is really hard to
 incrementally modify Nomad variables. The API is at one go. You either update
 all variables or nothing. Most often I wanted to update a single key
 from a Nomad variable at a time and the variable value was usually a file content.
 
 Example execution of putting a `passwordfile.txt` into `nomad/jobs/nginx`
 Nomad variable:
 
 ```
-$ nomad-vardir -j nginx put ./passwordfile.txt 
+$ nomadtools vardir -j nginx put ./passwordfile.txt 
 nomad_vardir: Putting var nomad/jobs/nginx@default with keys: passwordfile.txt
-$ nomad-vardir -j nginx cat passwordfile.txt 
+$ nomadtools vardir -j nginx cat passwordfile.txt 
 secretpassword
-$ nomad-vardir -j nginx ls
+$ nomadtools vardir -j nginx ls
 nomad_vardir: Listing Nomad variable at nomad/jobs/nginx@default
 key              size
 passwordfile.txt 15
 ```
 
 You can then remove the `passwordfile.txt` key from the Nomad variable:
 
 ```
-$ nomad-vardir -j nginx rm passwordfile.txt 
+$ nomadtools vardir -j nginx rm passwordfile.txt 
 nomad_vardir: Removing passwordfile.txt
 nomad_vardir: Removing empty var nomad/jobs/nginx@default
-$ nomad-vardir -j nginx ls
+$ nomadtools vardir -j nginx ls
 nomad_vardir: Nomad variable not found at nomad/jobs/nginx@default
 ```
 
-## nomad-cp
+## cp
 
 This is a copy of the `docker cp` command. The syntax is meant to be the
 same with docker. The rules of copying a file vs directory are meant to be
 in-line with `docker cp` documentation.
 
-`nomad-cp` uses some special syntax for specifying from which allocation/task
+`nomadtools cp` uses some special syntax for specifying from which allocation/task
 exactly do you want to copy by using colon `:`. The number of colons in the
 arguments determines the format. The colon can be escaped with slash `\` in
 the path if needed.
 
 Both `SRC` and `DST` addresses can be specified as follows:
 
 ```
+# Search a task matching specific URL query:
+task://JOB[@NAMESPACE]/PATH[?group=GROUP][&alloc=ALLOC][&task=TASK][&hostname=HOSTNAME][&node=NODE]
+# or
 :ALLOCATION:PATH                  copy path from this allocation having one job
-:ALLOCATION:TASK:PATH             copy path from this task inside allocation
+:ALLOCATION::TASK:PATH            copy path from this task inside allocation
 :ALLOCATION:GROUP:TASK:PATH       like above, but filter by group name
 JOB:PATH                          copy path from one task inside specified job
-JOB:TASK:PATH                     copy path from the task inside this job
+JOB::TASK:PATH                    copy path from the task inside this job
 JOB:GROUP:TASK:PATH               like above, but filter also by group name
 PATH                              copy local path
 -                                 copy stdin or stdout TAR stream
 ```
 
-`nomad-cp` depends on `sh` and `tar` command line utility to be available
+`cp` depends on `sh` and `tar` command line utility to be available
 inside the allocation it is coping to/from. It has to be available there.
 
 Example:
 
 ```
-$ nomad-cp -v nginx:/etc/nginx/nginx.conf ./nginx.conf
+$ nomadtools cp -v nginx:/etc/nginx/nginx.conf ./nginx.conf
 INFO nomad_cp.py:copy_mode:487: File :d409e855-bf13-a342-fe7a-6fb579d2de85:listen:/etc/nginx/nginx.conf -> ./nginx.conf
-$ nomad-cp -v alpine:/etc/. ./etc/
+$ nomadtools cp -v alpine:/etc/. ./etc/
 INFO nomad_cp.py:copy_mode:512: New mkdir :d409e855-bf13-a342-fe7a-6fb579d2de85:listen:/etc/. -> /home/kamil/tmp/etc2/
 ```
 
 Nomad does not have the capability of accessing any file inside the
 allocation file system. Instead, `nomad-cp` executes several `nomad exec`
 calls to execute a `tar` pipe to stream the data from or to the allocation
 context to or from the local host using stdout and stdin forwarded by
 `nomad exec`.
 
-## nomad-gitlab-runner
+## gitlab-runner
 
 An implementation of custom Gitlab executor driver that runs Gitlab CI/CD jobs
 using Nomad.
 
 This program does _not_ run the `gitlab-runner` itself in Nomad. Rather, the
 `gitlab-runner` is running on (any) one host. That `gitlab-runner` will then
 schedule Nomad jobs to execute using the script as an executor. These jobs will
 execute the CI/CD from Gitlab inside Nomad cluster.
 
-More on it can be read on [github wiki](https://github.com/Kamilcuk/nomad-tools/wiki/nomad%E2%80%90gitlab%E2%80%90runner).
+More on it can be read on [github wiki](https://github.com/Kamilcuk/nomadtools/wiki/gitlab%E2%80%90runner).
 
 ## nomad-dockers
 
 Lists docker images referenced in Nomad job file or a running Nomad job.
 
 ```
-$ nomad-dockers ./httpd.nomad.hcl
+$ nomadtools dockers ./httpd.nomad.hcl
 busybox:stable
-$ nomad-dockers --job httpd
+$ nomadtools dockers --job httpd
 busybox:stable
 ```
 
-## nomad-downloadrelease
+## downloadrelease
 
 Program for downloading specific Nomad release binary from their release page.
 I use it for testing and checking new Nomad versions.
 
 ```
-$ nomad-downloadrelease nomad
+$ nomadtools downloadrelease nomad
 INFO:nomad_tools.nomad_downloadrelease:Downloading https://releases.hashicorp.com/nomad/1.7.3/nomad_1.7.3_linux_amd64.zip to nomad
 INFO:nomad_tools.nomad_downloadrelease:https://releases.hashicorp.com/nomad/1.7.3/nomad_1.7.3_linux_amd64.zip -> -rwxr-xr-x 105.7MB nomad
-$ nomad-downloadrelease consul
+$ nomadtools downloadrelease consul
 INFO:nomad_tools.nomad_downloadrelease:Downloading https://releases.hashicorp.com/consul/1.9.9/consul_1.9.9_linux_amd64.zip to consul
 INFO:nomad_tools.nomad_downloadrelease:https://releases.hashicorp.com/consul/1.9.9/consul_1.9.9_linux_amd64.zip -> -rwxr-xr-x 105.8MB consul
-$ nomad-downloadrelease -p 1.6.3 nomad ./nomad1.6.3
+$ nomadtools downloadrelease -p 1.6.3 nomad ./nomad1.6.3
 INFO:nomad_tools.nomad_downloadrelease:Downloading https://releases.hashicorp.com/nomad/1.6.3/nomad_1.6.3_linux_amd64.zip to nomad1.6.3
 INFO:nomad_tools.nomad_downloadrelease:https://releases.hashicorp.com/nomad/1.6.3/nomad_1.6.3_linux_amd64.zip -> -rwxr-xr-x 101.8MB nomad1.6.3
 
 ```
 
 ## import nomad_tools
 
 This project is licensed under GPL. The internal API of this project can be
 used, however it is not stable at all and is an implementation detail.
 
 Internally, `nomad_tools.nomadlib` is a Python class definitions which
 represents models for Nomad API data documentation.
 
+# History
+
+This module once installed bunch of separate tools, like `nomad-watch` or
+`nomad-gitlab-runner`. That became unmaintainable. It is one `nomadtools`
+executable with several sub-commands.
+
 # Contributing
 
 Kindly make a issue or pull request on GitHub.
 I should be fast to respond and contributions are super welcome.
 
 ## Running tests
```

### Comparing `nomad-tools-0.2.4/src/nomad_tools.egg-info/SOURCES.txt` & `nomad_tools-0.3.0/src/nomad_tools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,36 +5,42 @@
 requirements.txt
 src/nomad_tools/__init__.py
 src/nomad_tools/colors.py
 src/nomad_tools/common.py
 src/nomad_tools/common_base.py
 src/nomad_tools/common_click.py
 src/nomad_tools/common_nomad.py
+src/nomad_tools/entry_constrainteval.py
+src/nomad_tools/entry_go.py
+src/nomad_tools/entrypoint.py
 src/nomad_tools/exit_on_thread_exception.py
 src/nomad_tools/flagdebug.py
 src/nomad_tools/nomad_cp.py
 src/nomad_tools/nomad_dockers.py
 src/nomad_tools/nomad_downloadrelease.py
 src/nomad_tools/nomad_gitlab_runner.py
 src/nomad_tools/nomad_port.py
 src/nomad_tools/nomad_smart_start_job.py
+src/nomad_tools/nomad_taskexec.py
 src/nomad_tools/nomad_vardir.py
 src/nomad_tools/nomad_watch.py
 src/nomad_tools/nomaddbjob.py
-src/nomad_tools/nomadt.py
 src/nomad_tools/nomadt_completion.sh
 src/nomad_tools/taskexec.py
+src/nomad_tools/transferstats.py
 src/nomad_tools.egg-info/PKG-INFO
 src/nomad_tools.egg-info/SOURCES.txt
 src/nomad_tools.egg-info/dependency_links.txt
 src/nomad_tools.egg-info/entry_points.txt
 src/nomad_tools.egg-info/requires.txt
 src/nomad_tools.egg-info/top_level.txt
 src/nomad_tools/nomad_gitlab_runner/script.sh
 src/nomad_tools/nomad_gitlab_runner/waiter.sh
 src/nomad_tools/nomadlib/__init__.py
 src/nomad_tools/nomadlib/_generator.py
 src/nomad_tools/nomadlib/connection.py
 src/nomad_tools/nomadlib/datadict.py
 src/nomad_tools/nomadlib/tools.py
 src/nomad_tools/nomadlib/types.py
+tests/test_nomad_cp_complete.py
+tests/test_taskexec_transfer_stats.py
 tests/testlib.py
```

### Comparing `nomad-tools-0.2.4/tests/testlib.py` & `nomad_tools-0.3.0/tests/testlib.py`

 * *Files 8% similar despite different names*

```diff
@@ -152,20 +152,15 @@
     :param check: if null, don't perform any checks, if true, exit status has to be zero, if false, exit status
     :param text: passed to subprocess.run
     :param input: pass input to subprocess.run
     :param output: an array of strings or patterns to check output of command against
     :param stdout: capture stdout. tru if output is given
     """
     cmd = f"timeout {timeout} {cmd}"
-    cmda: List[str] = []
-    for i in shlex.split(cmd):
-        if i in "nomad-cp nomad-watch nomad-port".split():
-            cmda.extend(f"python3 -m nomad_tools.{i.replace('-', '_')} -v".split())
-        else:
-            cmda.append(i)
+    cmda: List[str] = shlex.split(cmd)
     print(" ", file=sys.stderr, flush=True)
     print(f"+ {quotearr(cmda)}", file=sys.stderr, flush=True)
     stdout = stdout or bool(output)
     # Run subprocess.Popen, input stdin and output stdout.
     with subprocess.Popen(
         cmda,
         text=text,
@@ -222,20 +217,24 @@
     @functools.wraps(run)
     def inner(cmd: str, *args, **kwargs):
         return run(f"{prefix} {cmd}", *args, **kwargs)
 
     return inner
 
 
-run_nomad_cp = prefixed_run("python3 -m nomad_tools.nomad_cp -vv")
-run_nomad_watch = prefixed_run("python3 -m nomad_tools.nomad_watch -v")
-run_nomad_vardir = prefixed_run("python3 -m nomad_tools.nomad_vardir -v")
-run_nomad_dockers = prefixed_run("python3 -m nomad_tools.nomad_dockers -v")
-run_downloadrelease = prefixed_run("python3 -m nomad_tools.nomad_downloadrelease")
-run_nomadt = prefixed_run("python3 -m nomad_tools.nomadt --verbose")
+run_nomad_cp = prefixed_run(
+    "python3 -m nomad_tools.entrypoint cp -vv --no-stats --no-pv"
+)
+run_nomad_watch = prefixed_run(
+    "python3 -m nomad_tools.entrypoint watch -v --lines -1 --shutdown-timeout 5"
+)
+run_nomad_vardir = prefixed_run("python3 -m nomad_tools.entrypoint vardir -v")
+run_nomad_dockers = prefixed_run("python3 -m nomad_tools.entrypoint dockers -v")
+run_downloadrelease = prefixed_run("python3 -m nomad_tools.entrypoint downloadrelease")
+run_nomadt = prefixed_run("python3 -m nomad_tools.entrypoint")
 
 
 def run_bash(script: str, **kwargs):
     return run(f"bash -o pipefail -euxc {shlex.quote(script)}", **kwargs)
 
 
 ###############################################################################
```

