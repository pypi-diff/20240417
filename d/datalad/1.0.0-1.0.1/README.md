# Comparing `tmp/datalad-1.0.0.tar.gz` & `tmp/datalad-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalad-1.0.0.tar", last modified: Sat Apr  6 16:46:28 2024, max compression
+gzip compressed data, was "datalad-1.0.1.tar", last modified: Wed Apr 17 04:25:22 2024, max compression
```

## Comparing `datalad-1.0.0.tar` & `datalad-1.0.1.tar`

### file list

```diff
@@ -1,585 +1,585 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.382451 datalad-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-06 16:45:49.000000 datalad-1.0.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)   305112 2024-04-06 16:46:20.000000 datalad-1.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    31594 2024-04-06 16:45:49.000000 datalad-1.0.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-06 16:45:49.000000 datalad-1.0.0/CONTRIBUTORS
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-06 16:45:49.000000 datalad-1.0.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-06 16:45:49.000000 datalad-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-06 16:45:49.000000 datalad-1.0.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    37754 2024-04-06 16:46:28.382451 datalad-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27149 2024-04-06 16:45:49.000000 datalad-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.286450 datalad-1.0.0/_datalad_build_support/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-06 16:45:49.000000 datalad-1.0.0/_datalad_build_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10971 2024-04-06 16:45:49.000000 datalad-1.0.0/_datalad_build_support/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)    13311 2024-04-06 16:45:49.000000 datalad-1.0.0/_datalad_build_support/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-06 16:45:49.000000 datalad-1.0.0/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.286450 datalad-1.0.0/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 16:45:49.000000 datalad-1.0.0/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-06 16:45:49.000000 datalad-1.0.0/benchmarks/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-06 16:45:49.000000 datalad-1.0.0/benchmarks/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-06 16:45:49.000000 datalad-1.0.0/benchmarks/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-06 16:45:49.000000 datalad-1.0.0/benchmarks/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.286450 datalad-1.0.0/benchmarks/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:45:49.000000 datalad-1.0.0/benchmarks/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-06 16:45:49.000000 datalad-1.0.0/benchmarks/plugins/addurls.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-06 16:45:49.000000 datalad-1.0.0/benchmarks/repo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.286450 datalad-1.0.0/benchmarks/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      223 2024-04-06 16:45:49.000000 datalad-1.0.0/benchmarks/scripts/heavyout
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.286450 datalad-1.0.0/benchmarks/support/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:45:49.000000 datalad-1.0.0/benchmarks/support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-06 16:45:49.000000 datalad-1.0.0/benchmarks/support/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-06 16:45:49.000000 datalad-1.0.0/benchmarks/usecases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.386451 datalad-1.0.0/datalad/
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-06 16:46:28.386451 datalad-1.0.0/datalad/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.294450 datalad-1.0.0/datalad/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/cli/common_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/cli/exec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10321 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/cli/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/cli/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    24331 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/cli/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.294450 datalad-1.0.0/datalad/cli/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/cli/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/cli/tests/test_exec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/cli/tests/test_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/cli/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/cli/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    15683 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/cli/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/cli/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/cli/tests/test_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/cli/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22299 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.294450 datalad-1.0.0/datalad/cmdline/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/cmdline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/cmdline/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/cmdline/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    44706 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.294450 datalad-1.0.0/datalad/core/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.294450 datalad-1.0.0/datalad/core/distributed/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/core/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36141 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/core/distributed/clone.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/core/distributed/clone_ephemeral.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/core/distributed/clone_ria.py
--rw-r--r--   0 runner    (1001) docker     (127)    36247 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/core/distributed/clone_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    36859 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/core/distributed/push.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.294450 datalad-1.0.0/datalad/core/distributed/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/core/distributed/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    66865 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/core/distributed/tests/test_clone.py
--rw-r--r--   0 runner    (1001) docker     (127)    40767 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/core/distributed/tests/test_push.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.298451 datalad-1.0.0/datalad/core/local/
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/core/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22200 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/core/local/create.py
--rw-r--r--   0 runner    (1001) docker     (127)    16916 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/core/local/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/core/local/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7711 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/core/local/resulthooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    42741 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/core/local/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    17029 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/core/local/save.py
--rw-r--r--   0 runner    (1001) docker     (127)    27762 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/core/local/status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.298451 datalad-1.0.0/datalad/core/local/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/core/local/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18286 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/core/local/tests/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    20775 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/core/local/tests/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/core/local/tests/test_resulthooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/core/local/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    28900 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/core/local/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    40272 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/core/local/tests/test_save.py
--rw-r--r--   0 runner    (1001) docker     (127)    16350 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/core/local/tests/test_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/coreapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.298451 datalad-1.0.0/datalad/customremotes/
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/customremotes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19135 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/customremotes/archives.py
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/customremotes/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/customremotes/datalad.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/customremotes/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/customremotes/ria_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/customremotes/ria_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.302451 datalad-1.0.0/datalad/customremotes/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/customremotes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10912 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/customremotes/tests/test_archives.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/customremotes/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/customremotes/tests/test_datalad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/customremotes/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/customremotes/tests/test_ria_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.302451 datalad-1.0.0/datalad/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28903 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/dataset/gitrepo.py
--rw-r--r--   0 runner    (1001) docker     (127)    11777 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/dataset/repo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.302451 datalad-1.0.0/datalad/dataset/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/dataset/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/dataset/tests/test_gitrepo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.302451 datalad-1.0.0/datalad/distributed/
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24668 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/create_sibling_ghlike.py
--rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/create_sibling_gin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/create_sibling_gitea.py
--rw-r--r--   0 runner    (1001) docker     (127)    12166 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/create_sibling_github.py
--rw-r--r--   0 runner    (1001) docker     (127)    27785 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/create_sibling_gitlab.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/create_sibling_gogs.py
--rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/create_sibling_ria.py
--rw-r--r--   0 runner    (1001) docker     (127)    31971 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/drop.py
--rw-r--r--   0 runner    (1001) docker     (127)     9709 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/export_archive_ora.py
--rw-r--r--   0 runner    (1001) docker     (127)    15010 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/export_to_figshare.py
--rw-r--r--   0 runner    (1001) docker     (127)    64838 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/ora_remote.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.306450 datalad-1.0.0/datalad/distributed/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/tests/ria_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/tests/test_create_sibling_ghlike.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/tests/test_create_sibling_gin.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/tests/test_create_sibling_gitea.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/tests/test_create_sibling_github.py
--rw-r--r--   0 runner    (1001) docker     (127)    17937 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/tests/test_create_sibling_gitlab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/tests/test_create_sibling_gogs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14789 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/tests/test_create_sibling_ria.py
--rw-r--r--   0 runner    (1001) docker     (127)    22502 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/tests/test_drop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/tests/test_export_to_figshare.py
--rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/tests/test_ora_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/tests/test_ria.py
--rw-r--r--   0 runner    (1001) docker     (127)    27819 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/tests/test_ria_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14542 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distributed/tests/test_ria_git_remote.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.310451 datalad-1.0.0/datalad/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42187 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/create_sibling.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/create_sibling_github.py
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/create_test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    29636 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/drop.py
--rw-r--r--   0 runner    (1001) docker     (127)    41294 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/get.py
--rw-r--r--   0 runner    (1001) docker     (127)    18719 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/install.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/remove.py
--rw-r--r--   0 runner    (1001) docker     (127)    35111 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/siblings.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/subdatasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.310451 datalad-1.0.0/datalad/distribution/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36685 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/tests/test_create_sibling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/tests/test_create_test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    21165 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/tests/test_dataset_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/tests/test_dataset_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/tests/test_drop.py
--rw-r--r--   0 runner    (1001) docker     (127)    30776 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/tests/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)    39348 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/tests/test_install.py
--rw-r--r--   0 runner    (1001) docker     (127)    21275 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/tests/test_siblings.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/tests/test_uninstall.py
--rw-r--r--   0 runner    (1001) docker     (127)    44945 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.310451 datalad-1.0.0/datalad/distribution/tests/vcr_cassettes/
--rw-r--r--   0 runner    (1001) docker     (127)    38684 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/tests/vcr_cassettes/github_datalad_tester_org.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    26085 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/tests/vcr_cassettes/github_yarikoptic.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/uninstall.py
--rw-r--r--   0 runner    (1001) docker     (127)    24518 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/distribution/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9648 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/dochelpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.314451 datalad-1.0.0/datalad/downloaders/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29242 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.314451 datalad-1.0.0/datalad/downloaders/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/configs/crawdad.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/configs/crcns.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/configs/dockerio.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/configs/figshare.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/configs/hcp.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/configs/indi.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/configs/kaggle.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/configs/loris.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/configs/nda.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/configs/nitrc.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/configs/nsidc.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/configs/openfmri.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/configs/providers.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    19843 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    28532 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/http.py
--rw-r--r--   0 runner    (1001) docker     (127)    24331 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)    16270 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/shub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.318451 datalad-1.0.0/datalad/downloaders/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11204 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/tests/test_docker_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    31188 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/tests/test_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     9287 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/tests/test_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12649 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/tests/test_shub.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/downloaders/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.318451 datalad-1.0.0/datalad/interface/
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/interface/add_archive_content.py
--rw-r--r--   0 runner    (1001) docker     (127)    34196 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/interface/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/interface/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)    30528 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/interface/common_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)    15858 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/interface/common_opts.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/interface/download_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/interface/rerun.py
--rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/interface/results.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/interface/run_procedure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/interface/shell_completion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.318451 datalad-1.0.0/datalad/interface/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/interface/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/interface/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/interface/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/interface/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/interface/tests/test_shell_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19645 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/interface/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/interface/unlock.py
--rw-r--r--   0 runner    (1001) docker     (127)    17915 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/interface/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.322450 datalad-1.0.0/datalad/local/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30822 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/add_archive_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     9681 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/add_readme.py
--rw-r--r--   0 runner    (1001) docker     (127)    60394 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/addurls.py
--rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/check_dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    30262 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/copy_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/download_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/export_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)    18739 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/foreach_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/gitcredential.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/gitcredential_datalad.py
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/no_annex.py
--rw-r--r--   0 runner    (1001) docker     (127)    11056 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/remove.py
--rw-r--r--   0 runner    (1001) docker     (127)    27294 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/rerun.py
--rw-r--r--   0 runner    (1001) docker     (127)    21317 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/run_procedure.py
--rw-r--r--   0 runner    (1001) docker     (127)    17769 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/subdatasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.326451 datalad-1.0.0/datalad/local/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25061 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/tests/test_add_archive_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/tests/test_add_readme.py
--rw-r--r--   0 runner    (1001) docker     (127)    37452 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/tests/test_addurls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/tests/test_check_dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/tests/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/tests/test_copy_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     8929 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/tests/test_download_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/tests/test_export_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/tests/test_foreach_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7218 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/tests/test_gitcredential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/tests/test_no_annex.py
--rw-r--r--   0 runner    (1001) docker     (127)    10057 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/tests/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)    34225 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/tests/test_rerun.py
--rw-r--r--   0 runner    (1001) docker     (127)    22961 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/tests/test_rerun_merges.py
--rw-r--r--   0 runner    (1001) docker     (127)    15920 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/tests/test_run_procedure.py
--rw-r--r--   0 runner    (1001) docker     (127)    12436 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/tests/test_subdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/tests/test_unlock.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/tests/test_wtf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/unlock.py
--rw-r--r--   0 runner    (1001) docker     (127)    21259 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/local/wtf.py
--rw-r--r--   0 runner    (1001) docker     (127)    25582 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.330451 datalad-1.0.0/datalad/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/plugin/add_readme.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/plugin/addurls.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/plugin/check_dates.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/plugin/export_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/plugin/export_to_figshare.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/plugin/no_annex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.330451 datalad-1.0.0/datalad/plugin/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/plugin/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/plugin/wtf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.278450 datalad-1.0.0/datalad/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.330451 datalad-1.0.0/datalad/resources/procedures/
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/resources/procedures/cfg_noannex.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/resources/procedures/cfg_text2git.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/resources/procedures/cfg_yoda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.330451 datalad-1.0.0/datalad/resources/procedures/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/resources/procedures/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/resources/procedures/tests/test_noannex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.330451 datalad-1.0.0/datalad/runner/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/runner/coreprotocols.py
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/runner/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    12377 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/runner/gitrunner.py
--rw-r--r--   0 runner    (1001) docker     (127)    30114 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/runner/nonasyncrunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/runner/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     9995 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/runner/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7567 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/runner/runnerthreads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.334451 datalad-1.0.0/datalad/runner/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/runner/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/runner/tests/test_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/runner/tests/test_generatormixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/runner/tests/test_gitrunner.py
--rw-r--r--   0 runner    (1001) docker     (127)    24452 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/runner/tests/test_nonasyncrunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/runner/tests/test_threadsafety.py
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/runner/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14360 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/runner/tests/test_witless_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/runner/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.338451 datalad-1.0.0/datalad/support/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/annex_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   159444 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/annexrepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/ansi_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/archive_utils_7z.py
--rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/archive_utils_patool.py
--rw-r--r--   0 runner    (1001) docker     (127)    16198 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/archives.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    14584 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/digests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/due.py
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/due_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (127)    18826 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14985 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/external_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)   156510 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/gitrepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/globbedpaths.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/itertools.py
--rw-r--r--   0 runner    (1001) docker     (127)     6224 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/json_py.py
--rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/keyring_.py
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/locking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/nda_.py
--rw-r--r--   0 runner    (1001) docker     (127)    40503 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    25153 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/param.py
--rw-r--r--   0 runner    (1001) docker     (127)    10699 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/path.py
--rw-r--r--   0 runner    (1001) docker     (127)    10635 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/repodates.py
--rw-r--r--   0 runner    (1001) docker     (127)    19803 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)    31564 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/sshconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/sshrun.py
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.342451 datalad-1.0.0/datalad/support/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    99030 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/tests/test_annexrepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/tests/test_ansi_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/tests/test_captured_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/tests/test_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/tests/test_digests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/tests/test_due_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/tests/test_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/tests/test_external_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15124 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/tests/test_fileinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    55678 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/tests/test_gitrepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8142 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/tests/test_globbedpaths.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/tests/test_json_py.py
--rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/tests/test_locking.py
--rw-r--r--   0 runner    (1001) docker     (127)    26036 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/tests/test_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/tests/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/tests/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/tests/test_repo_save.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/tests/test_repodates.py
--rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/tests/test_sshconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/tests/test_sshrun.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/tests/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/tests/test_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/tests/test_vcr_.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.342451 datalad-1.0.0/datalad/support/third/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/third/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/third/loris_token_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/third/nda_aws_token_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/support/vcr_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.346451 datalad-1.0.0/datalad/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.350451 datalad-1.0.0/datalad/tests/ca/
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/ca/README
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/ca/ca-key.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/ca/ca-root.pem
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/ca/ca-root.srl
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/ca/ca_bundle.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/ca/certificate-key.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/ca/certificate-pub.pem
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/ca/certificate.csr
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/heavyoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/test__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/test_archives.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/test_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    31290 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/test_direct_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/test_dochelpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/test_installed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/test_strings.py
--rw-r--r--   0 runner    (1001) docker     (127)    21530 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/test_tests_utils_pytest.py
--rw-r--r--   0 runner    (1001) docker     (127)    46028 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12336 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/test_utils_cached_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/test_utils_testrepos.py
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9968 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/utils_cached_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    68204 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/utils_pytest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/utils_testdatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7262 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/tests/utils_testrepos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.350451 datalad-1.0.0/datalad/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/ui/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    14079 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/ui/dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    12376 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/ui/progressbars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.350451 datalad-1.0.0/datalad/ui/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/ui/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/ui/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/ui/tests/test_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/ui/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    96337 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-06 16:45:49.000000 datalad-1.0.0/datalad/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.366451 datalad-1.0.0/datalad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    37754 2024-04-06 16:46:28.000000 datalad-1.0.0/datalad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17010 2024-04-06 16:46:28.000000 datalad-1.0.0/datalad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 16:46:28.000000 datalad-1.0.0/datalad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-06 16:46:28.000000 datalad-1.0.0/datalad.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-06 16:46:28.000000 datalad-1.0.0/datalad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 16:46:28.000000 datalad-1.0.0/datalad.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.350451 datalad-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.350451 datalad-1.0.0/docs/casts/
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/casts/basic_search.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/casts/boxcom.sh
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/casts/cmdline_basic_usage.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/casts/datalad_convenience_vs_git.sh
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/casts/heudiconv_dicom_to_bids.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/casts/publish_on_github.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/casts/reproducible_analysis.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/casts/seamless_nested_repos.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/casts/simple_provenance_tracking.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/casts/track_data_from_webpage.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/config-format.rst
--rw-r--r--   0 runner    (1001) docker     (127)    21354 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/design.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.354451 datalad-1.0.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.354451 datalad-1.0.0/docs/source/_extras/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/_extras/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.354451 datalad-1.0.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/_static/datalad_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/_static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.278450 datalad-1.0.0/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.354451 datalad-1.0.0/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/acknowledgements.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/background.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/basics.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/basics_cmdline.rst.in
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/basics_nesteddatasets.rst.in
--rw-r--r--   0 runner    (1001) docker     (127)   348581 2024-04-06 16:46:21.000000 datalad-1.0.0/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/cmdline.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12514 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/config.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/credentials.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/customization.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.358451 datalad-1.0.0/docs/source/design/
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/design/application_vs_library_mode.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/design/batched_command.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/design/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/design/credentials.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/design/dataset_argument.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/design/docstrings.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/design/drop.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/design/exception_handling.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/design/file_url_handling.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/design/github_actions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/design/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/design/log_levels.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/design/miscpatterns.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/design/pos_vs_kw_parameters.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/design/progress_reporting.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/design/provenance_capture.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/design/python_imports.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/design/result_records.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/design/standard_parameters.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/design/testing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/design/threaded_runner.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/design/url_substitution.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/design/user_messaging.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/modref.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/publications.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/source/related.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.358451 datalad-1.0.0/docs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-06 16:45:49.000000 datalad-1.0.0/docs/utils/pygments_ansi_color.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-06 16:45:49.000000 datalad-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-06 16:45:49.000000 datalad-1.0.0/requirements-devel.txt
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-06 16:45:49.000000 datalad-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-06 16:46:28.386451 datalad-1.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     6122 2024-04-06 16:45:49.000000 datalad-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.362451 datalad-1.0.0/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/Dockerfile.fullmaster
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/Singularity
--rwxr-xr-x   0 runner    (1001) docker     (127)     1211 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/adhoc-httpd
--rwxr-xr-x   0 runner    (1001) docker     (127)      932 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/bisect-git-annex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.362451 datalad-1.0.0/tools/bisect-git-annex.scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      241 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/bisect-git-annex.scripts/bisect-git-annex-doublepasswd.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      197 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/bisect-git-annex.scripts/bisect-git-annex-lock.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      884 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/changelog-todo
--rwxr-xr-x   0 runner    (1001) docker     (127)     2177 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/checkpwd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.366451 datalad-1.0.0/tools/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/ci/appveyor_enable_windevmode.ps1
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/ci/appveyor_env_setup.bat
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/ci/appveyor_install_git-annex.bat
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/ci/appveyor_ssh2localhost.bat
--rwxr-xr-x   0 runner    (1001) docker     (127)      120 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/ci/appveyor_ssh2localhost.sh
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/ci/appveyor_ssh_config
--rwxr-xr-x   0 runner    (1001) docker     (127)      826 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/ci/benchmark-travis-pr.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2943 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/ci/bisect-python.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      300 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/ci/debians_disable_outdated_ssl_cert
--rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/ci/deploy_datalad-rootca
--rwxr-xr-x   0 runner    (1001) docker     (127)     2481 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/ci/download-latest-artifact
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/ci/gpg-90F7E9EB.pub
--rwxr-xr-x   0 runner    (1001) docker     (127)     8846 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/ci/install-annex.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      379 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/ci/install-minimum-git.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      531 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/ci/install-singularity.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      220 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/ci/install-upstream-git.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      715 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/ci/prep-travis-devel-annex.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1048 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/ci/prep-travis-forssh.sh
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/cmdline-completion
--rwxr-xr-x   0 runner    (1001) docker     (127)      880 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/convert-git-annex-layout
--rwxr-xr-x   0 runner    (1001) docker     (127)     2352 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/copy_urls_from_datalad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.366451 datalad-1.0.0/tools/coverage-bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      858 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/coverage-bin/datalad
--rwxr-xr-x   0 runner    (1001) docker     (127)      858 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/coverage-bin/git-annex-remote-datalad
--rwxr-xr-x   0 runner    (1001) docker     (127)      858 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/coverage-bin/git-annex-remote-datalad-archives
--rwxr-xr-x   0 runner    (1001) docker     (127)      858 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/coverage-bin/git-annex-remote-ora
--rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/coverage-bin/sitecustomize.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1007 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/describegitannex
--rwxr-xr-x   0 runner    (1001) docker     (127)     1791 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/downgrade-annex
--rwxr-xr-x   0 runner    (1001) docker     (127)     1536 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/dtime
--rwxr-xr-x   0 runner    (1001) docker     (127)      943 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/eval_under_nfs
--rwxr-xr-x   0 runner    (1001) docker     (127)      801 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/eval_under_testloopfs
--rwxr-xr-x   0 runner    (1001) docker     (127)      876 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/find-hanged-tests
--rwxr-xr-x   0 runner    (1001) docker     (127)     2127 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/git-web-submodules.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      447 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/link_issues_CHANGELOG
--rwxr-xr-x   0 runner    (1001) docker     (127)     3010 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/mimic_merges
--rwxr-xr-x   0 runner    (1001) docker     (127)     4567 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/mimic_repo
--rwxr-xr-x   0 runner    (1001) docker     (127)      419 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/mkcontrib
--rwxr-xr-x   0 runner    (1001) docker     (127)     2802 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/monitor-interrupts.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2298 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/profile_python
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.366451 datalad-1.0.0/tools/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/testing/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.282451 datalad-1.0.0/tools/testing/bad_internals/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.366451 datalad-1.0.0/tools/testing/bad_internals/_scrapy/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/testing/bad_internals/_scrapy/scrapy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.366451 datalad-1.0.0/tools/testing/conf/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/testing/conf/apache-ssh-supervisor.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.282451 datalad-1.0.0/tools/testing/conf/etc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.282451 datalad-1.0.0/tools/testing/conf/etc/apt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:46:28.366451 datalad-1.0.0/tools/testing/conf/etc/apt/apt.conf.d/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/testing/conf/etc/apt/apt.conf.d/99apt-cacher
--rwxr-xr-x   0 runner    (1001) docker     (127)     3461 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/testing/make_test_repo
--rwxr-xr-x   0 runner    (1001) docker     (127)      938 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/testing/make_test_repos
--rwxr-xr-x   0 runner    (1001) docker     (127)     4134 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/testing/start_website_in_docker
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/testing/start_website_in_docker-Dockerfile.in
--rwxr-xr-x   0 runner    (1001) docker     (127)     1932 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/testing/test_README_in_docker
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/testing/test_README_in_docker-Dockerfile.in
--rwxr-xr-x   0 runner    (1001) docker     (127)      481 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/testing/travis_ifdown_nonlo.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      593 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/upgrade-annex-osx.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     3570 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/urlinfo
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-06 16:45:49.000000 datalad-1.0.0/tools/which.py
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-06 16:45:49.000000 datalad-1.0.0/tox.ini
--rw-r--r--   0 runner    (1001) docker     (127)    81087 2024-04-06 16:45:49.000000 datalad-1.0.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.118665 datalad-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-17 04:24:43.000000 datalad-1.0.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)   305429 2024-04-17 04:25:14.000000 datalad-1.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    31594 2024-04-17 04:24:43.000000 datalad-1.0.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-17 04:24:43.000000 datalad-1.0.1/CONTRIBUTORS
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-17 04:24:43.000000 datalad-1.0.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-17 04:24:43.000000 datalad-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-17 04:24:43.000000 datalad-1.0.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    37754 2024-04-17 04:25:22.114665 datalad-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27149 2024-04-17 04:24:43.000000 datalad-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.010665 datalad-1.0.1/_datalad_build_support/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-17 04:24:43.000000 datalad-1.0.1/_datalad_build_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10971 2024-04-17 04:24:43.000000 datalad-1.0.1/_datalad_build_support/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13311 2024-04-17 04:24:43.000000 datalad-1.0.1/_datalad_build_support/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-17 04:24:43.000000 datalad-1.0.1/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.014665 datalad-1.0.1/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 04:24:43.000000 datalad-1.0.1/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-17 04:24:43.000000 datalad-1.0.1/benchmarks/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-17 04:24:43.000000 datalad-1.0.1/benchmarks/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-17 04:24:43.000000 datalad-1.0.1/benchmarks/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-17 04:24:43.000000 datalad-1.0.1/benchmarks/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.014665 datalad-1.0.1/benchmarks/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 04:24:43.000000 datalad-1.0.1/benchmarks/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-17 04:24:43.000000 datalad-1.0.1/benchmarks/plugins/addurls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-17 04:24:43.000000 datalad-1.0.1/benchmarks/repo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.014665 datalad-1.0.1/benchmarks/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      223 2024-04-17 04:24:43.000000 datalad-1.0.1/benchmarks/scripts/heavyout
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.014665 datalad-1.0.1/benchmarks/support/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 04:24:43.000000 datalad-1.0.1/benchmarks/support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-17 04:24:43.000000 datalad-1.0.1/benchmarks/support/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-17 04:24:43.000000 datalad-1.0.1/benchmarks/usecases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.118665 datalad-1.0.1/datalad/
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-17 04:25:22.118665 datalad-1.0.1/datalad/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.018665 datalad-1.0.1/datalad/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/cli/common_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/cli/exec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10321 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/cli/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/cli/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24331 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/cli/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.022665 datalad-1.0.1/datalad/cli/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/cli/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/cli/tests/test_exec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/cli/tests/test_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/cli/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/cli/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15683 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/cli/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/cli/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/cli/tests/test_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/cli/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22299 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.022665 datalad-1.0.1/datalad/cmdline/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/cmdline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/cmdline/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/cmdline/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44706 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.022665 datalad-1.0.1/datalad/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.022665 datalad-1.0.1/datalad/core/distributed/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/core/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36141 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/core/distributed/clone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/core/distributed/clone_ephemeral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/core/distributed/clone_ria.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36247 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/core/distributed/clone_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36859 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/core/distributed/push.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.022665 datalad-1.0.1/datalad/core/distributed/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/core/distributed/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66865 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/core/distributed/tests/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40767 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/core/distributed/tests/test_push.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.026665 datalad-1.0.1/datalad/core/local/
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/core/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22200 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/core/local/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16916 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/core/local/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/core/local/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7711 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/core/local/resulthooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42741 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/core/local/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17029 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/core/local/save.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27762 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/core/local/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.026665 datalad-1.0.1/datalad/core/local/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/core/local/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18286 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/core/local/tests/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20775 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/core/local/tests/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/core/local/tests/test_resulthooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/core/local/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28900 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/core/local/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40272 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/core/local/tests/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16350 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/core/local/tests/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/coreapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.026665 datalad-1.0.1/datalad/customremotes/
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/customremotes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19135 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/customremotes/archives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/customremotes/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/customremotes/datalad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/customremotes/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/customremotes/ria_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/customremotes/ria_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.030665 datalad-1.0.1/datalad/customremotes/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/customremotes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10912 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/customremotes/tests/test_archives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/customremotes/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/customremotes/tests/test_datalad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/customremotes/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/customremotes/tests/test_ria_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.030665 datalad-1.0.1/datalad/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28903 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/dataset/gitrepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11777 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/dataset/repo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.030665 datalad-1.0.1/datalad/dataset/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/dataset/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/dataset/tests/test_gitrepo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.030665 datalad-1.0.1/datalad/distributed/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24668 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/create_sibling_ghlike.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/create_sibling_gin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/create_sibling_gitea.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12166 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/create_sibling_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27785 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/create_sibling_gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/create_sibling_gogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/create_sibling_ria.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31971 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/drop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9709 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/export_archive_ora.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15010 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/export_to_figshare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64838 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/ora_remote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.034665 datalad-1.0.1/datalad/distributed/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/tests/ria_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/tests/test_create_sibling_ghlike.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/tests/test_create_sibling_gin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/tests/test_create_sibling_gitea.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/tests/test_create_sibling_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17937 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/tests/test_create_sibling_gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/tests/test_create_sibling_gogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14789 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/tests/test_create_sibling_ria.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22502 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/tests/test_drop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/tests/test_export_to_figshare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/tests/test_ora_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/tests/test_ria.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27819 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/tests/test_ria_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14542 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distributed/tests/test_ria_git_remote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.038665 datalad-1.0.1/datalad/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42187 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/create_sibling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/create_sibling_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/create_test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29636 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/drop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41294 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18719 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35111 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/siblings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/subdatasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.038665 datalad-1.0.1/datalad/distribution/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36685 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/tests/test_create_sibling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/tests/test_create_test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21165 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/tests/test_dataset_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/tests/test_dataset_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/tests/test_drop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30776 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/tests/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39348 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/tests/test_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21275 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/tests/test_siblings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/tests/test_uninstall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44945 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.038665 datalad-1.0.1/datalad/distribution/tests/vcr_cassettes/
+-rw-r--r--   0 runner    (1001) docker     (127)    38684 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/tests/vcr_cassettes/github_datalad_tester_org.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    26085 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/tests/vcr_cassettes/github_yarikoptic.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/uninstall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24518 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/distribution/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9648 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/dochelpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.042665 datalad-1.0.1/datalad/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29242 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.042665 datalad-1.0.1/datalad/downloaders/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/configs/crawdad.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/configs/crcns.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/configs/dockerio.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/configs/figshare.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/configs/hcp.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/configs/indi.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/configs/kaggle.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/configs/loris.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/configs/nda.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/configs/nitrc.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/configs/nsidc.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/configs/openfmri.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/configs/providers.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    19843 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28532 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24331 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16270 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/shub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.046665 datalad-1.0.1/datalad/downloaders/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11204 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/tests/test_docker_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31188 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9287 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/tests/test_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12649 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/tests/test_shub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/downloaders/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.046665 datalad-1.0.1/datalad/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/interface/add_archive_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34196 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/interface/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/interface/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30528 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/interface/common_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15858 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/interface/common_opts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/interface/download_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/interface/rerun.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/interface/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/interface/run_procedure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/interface/shell_completion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.046665 datalad-1.0.1/datalad/interface/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/interface/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/interface/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/interface/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/interface/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/interface/tests/test_shell_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19645 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/interface/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/interface/unlock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17915 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/interface/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.050665 datalad-1.0.1/datalad/local/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30822 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/add_archive_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9681 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/add_readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60394 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/addurls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/check_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30262 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/copy_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/download_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/export_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18739 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/foreach_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/gitcredential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/gitcredential_datalad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/no_annex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11056 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27294 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/rerun.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21317 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/run_procedure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17769 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/subdatasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.054665 datalad-1.0.1/datalad/local/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25061 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/tests/test_add_archive_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/tests/test_add_readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37452 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/tests/test_addurls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/tests/test_check_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/tests/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/tests/test_copy_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8929 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/tests/test_download_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/tests/test_export_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/tests/test_foreach_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7218 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/tests/test_gitcredential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/tests/test_no_annex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10057 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/tests/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34225 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/tests/test_rerun.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22961 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/tests/test_rerun_merges.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15920 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/tests/test_run_procedure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12436 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/tests/test_subdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/tests/test_unlock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/tests/test_wtf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/unlock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21259 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/local/wtf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25582 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.058665 datalad-1.0.1/datalad/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/plugin/add_readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/plugin/addurls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/plugin/check_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/plugin/export_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/plugin/export_to_figshare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/plugin/no_annex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.058665 datalad-1.0.1/datalad/plugin/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/plugin/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/plugin/wtf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.006665 datalad-1.0.1/datalad/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.058665 datalad-1.0.1/datalad/resources/procedures/
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/resources/procedures/cfg_noannex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/resources/procedures/cfg_text2git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/resources/procedures/cfg_yoda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.058665 datalad-1.0.1/datalad/resources/procedures/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/resources/procedures/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/resources/procedures/tests/test_noannex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.058665 datalad-1.0.1/datalad/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/runner/coreprotocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/runner/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12377 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/runner/gitrunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30114 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/runner/nonasyncrunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/runner/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9995 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/runner/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7567 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/runner/runnerthreads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.062665 datalad-1.0.1/datalad/runner/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/runner/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/runner/tests/test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/runner/tests/test_generatormixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/runner/tests/test_gitrunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24452 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/runner/tests/test_nonasyncrunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/runner/tests/test_threadsafety.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/runner/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14360 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/runner/tests/test_witless_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/runner/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.066665 datalad-1.0.1/datalad/support/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/annex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   159444 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/annexrepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/ansi_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/archive_utils_7z.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/archive_utils_patool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16198 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/archives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14584 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/digests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/due.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/due_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18826 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14985 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/external_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)   156510 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/gitrepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/globbedpaths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/itertools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6224 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/json_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/keyring_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/locking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/nda_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40503 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25153 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/param.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10699 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10635 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/repodates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19803 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31564 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/sshconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/sshrun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.074665 datalad-1.0.1/datalad/support/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99030 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/tests/test_annexrepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/tests/test_ansi_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/tests/test_captured_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/tests/test_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/tests/test_digests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/tests/test_due_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/tests/test_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/tests/test_external_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15124 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/tests/test_fileinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55678 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/tests/test_gitrepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8142 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/tests/test_globbedpaths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/tests/test_json_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/tests/test_locking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26036 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/tests/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/tests/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/tests/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/tests/test_repo_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/tests/test_repodates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/tests/test_sshconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/tests/test_sshrun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/tests/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/tests/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/tests/test_vcr_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.074665 datalad-1.0.1/datalad/support/third/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/third/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/third/loris_token_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/third/nda_aws_token_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/support/vcr_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.078665 datalad-1.0.1/datalad/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.078665 datalad-1.0.1/datalad/tests/ca/
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/ca/README
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/ca/ca-key.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/ca/ca-root.pem
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/ca/ca-root.srl
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/ca/ca_bundle.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/ca/certificate-key.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/ca/certificate-pub.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/ca/certificate.csr
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/heavyoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/test__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/test_archives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/test_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31290 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/test_direct_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/test_dochelpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/test_installed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/test_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21530 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/test_tests_utils_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46028 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12336 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/test_utils_cached_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/test_utils_testrepos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9968 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/utils_cached_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68204 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/utils_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/utils_testdatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7262 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/tests/utils_testrepos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.078665 datalad-1.0.1/datalad/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/ui/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14079 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/ui/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12376 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/ui/progressbars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.078665 datalad-1.0.1/datalad/ui/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/ui/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/ui/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/ui/tests/test_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/ui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96337 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-17 04:24:43.000000 datalad-1.0.1/datalad/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.102665 datalad-1.0.1/datalad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    37754 2024-04-17 04:25:21.000000 datalad-1.0.1/datalad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17010 2024-04-17 04:25:21.000000 datalad-1.0.1/datalad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 04:25:21.000000 datalad-1.0.1/datalad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-17 04:25:21.000000 datalad-1.0.1/datalad.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-17 04:25:21.000000 datalad-1.0.1/datalad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 04:25:21.000000 datalad-1.0.1/datalad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.082665 datalad-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.082665 datalad-1.0.1/docs/casts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/casts/basic_search.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/casts/boxcom.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/casts/cmdline_basic_usage.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/casts/datalad_convenience_vs_git.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/casts/heudiconv_dicom_to_bids.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/casts/publish_on_github.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/casts/reproducible_analysis.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/casts/seamless_nested_repos.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/casts/simple_provenance_tracking.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/casts/track_data_from_webpage.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/config-format.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    21354 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/design.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.086665 datalad-1.0.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.086665 datalad-1.0.1/docs/source/_extras/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/_extras/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.086665 datalad-1.0.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/_static/datalad_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/_static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.006665 datalad-1.0.1/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.086665 datalad-1.0.1/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/acknowledgements.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/background.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/basics_cmdline.rst.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/basics_nesteddatasets.rst.in
+-rw-r--r--   0 runner    (1001) docker     (127)   348929 2024-04-17 04:25:16.000000 datalad-1.0.1/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/cmdline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12514 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/credentials.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/customization.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.090665 datalad-1.0.1/docs/source/design/
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/design/application_vs_library_mode.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/design/batched_command.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/design/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/design/credentials.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/design/dataset_argument.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/design/docstrings.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/design/drop.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/design/exception_handling.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/design/file_url_handling.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/design/github_actions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/design/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/design/log_levels.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/design/miscpatterns.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/design/pos_vs_kw_parameters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/design/progress_reporting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/design/provenance_capture.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/design/python_imports.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/design/result_records.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/design/standard_parameters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/design/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/design/threaded_runner.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/design/url_substitution.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/design/user_messaging.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/modref.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/publications.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/source/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.090665 datalad-1.0.1/docs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-17 04:24:43.000000 datalad-1.0.1/docs/utils/pygments_ansi_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-17 04:24:43.000000 datalad-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-17 04:24:43.000000 datalad-1.0.1/requirements-devel.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-17 04:24:43.000000 datalad-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-17 04:25:22.118665 datalad-1.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6122 2024-04-17 04:24:43.000000 datalad-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.094665 datalad-1.0.1/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/Dockerfile.fullmaster
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/Singularity
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1211 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/adhoc-httpd
+-rwxr-xr-x   0 runner    (1001) docker     (127)      932 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/bisect-git-annex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.094665 datalad-1.0.1/tools/bisect-git-annex.scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      241 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/bisect-git-annex.scripts/bisect-git-annex-doublepasswd.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      197 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/bisect-git-annex.scripts/bisect-git-annex-lock.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      884 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/changelog-todo
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2177 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/checkpwd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.098665 datalad-1.0.1/tools/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/ci/appveyor_enable_windevmode.ps1
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/ci/appveyor_env_setup.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/ci/appveyor_install_git-annex.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/ci/appveyor_ssh2localhost.bat
+-rwxr-xr-x   0 runner    (1001) docker     (127)      120 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/ci/appveyor_ssh2localhost.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/ci/appveyor_ssh_config
+-rwxr-xr-x   0 runner    (1001) docker     (127)      826 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/ci/benchmark-travis-pr.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2943 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/ci/bisect-python.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      300 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/ci/debians_disable_outdated_ssl_cert
+-rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/ci/deploy_datalad-rootca
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2481 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/ci/download-latest-artifact
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/ci/gpg-90F7E9EB.pub
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8846 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/ci/install-annex.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      379 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/ci/install-minimum-git.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      531 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/ci/install-singularity.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      220 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/ci/install-upstream-git.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      715 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/ci/prep-travis-devel-annex.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1048 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/ci/prep-travis-forssh.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/cmdline-completion
+-rwxr-xr-x   0 runner    (1001) docker     (127)      880 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/convert-git-annex-layout
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2352 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/copy_urls_from_datalad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.098665 datalad-1.0.1/tools/coverage-bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      858 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/coverage-bin/datalad
+-rwxr-xr-x   0 runner    (1001) docker     (127)      858 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/coverage-bin/git-annex-remote-datalad
+-rwxr-xr-x   0 runner    (1001) docker     (127)      858 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/coverage-bin/git-annex-remote-datalad-archives
+-rwxr-xr-x   0 runner    (1001) docker     (127)      858 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/coverage-bin/git-annex-remote-ora
+-rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/coverage-bin/sitecustomize.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1007 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/describegitannex
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1791 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/downgrade-annex
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1536 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/dtime
+-rwxr-xr-x   0 runner    (1001) docker     (127)      943 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/eval_under_nfs
+-rwxr-xr-x   0 runner    (1001) docker     (127)      801 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/eval_under_testloopfs
+-rwxr-xr-x   0 runner    (1001) docker     (127)      876 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/find-hanged-tests
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2127 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/git-web-submodules.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      447 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/link_issues_CHANGELOG
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3010 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/mimic_merges
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4567 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/mimic_repo
+-rwxr-xr-x   0 runner    (1001) docker     (127)      419 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/mkcontrib
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2802 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/monitor-interrupts.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2298 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/profile_python
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.098665 datalad-1.0.1/tools/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/testing/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.006665 datalad-1.0.1/tools/testing/bad_internals/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.098665 datalad-1.0.1/tools/testing/bad_internals/_scrapy/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/testing/bad_internals/_scrapy/scrapy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.102665 datalad-1.0.1/tools/testing/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/testing/conf/apache-ssh-supervisor.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.010665 datalad-1.0.1/tools/testing/conf/etc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.010665 datalad-1.0.1/tools/testing/conf/etc/apt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:25:22.102665 datalad-1.0.1/tools/testing/conf/etc/apt/apt.conf.d/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/testing/conf/etc/apt/apt.conf.d/99apt-cacher
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3461 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/testing/make_test_repo
+-rwxr-xr-x   0 runner    (1001) docker     (127)      938 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/testing/make_test_repos
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4134 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/testing/start_website_in_docker
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/testing/start_website_in_docker-Dockerfile.in
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1932 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/testing/test_README_in_docker
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/testing/test_README_in_docker-Dockerfile.in
+-rwxr-xr-x   0 runner    (1001) docker     (127)      481 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/testing/travis_ifdown_nonlo.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      593 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/upgrade-annex-osx.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3570 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/urlinfo
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-17 04:24:43.000000 datalad-1.0.1/tools/which.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-17 04:24:43.000000 datalad-1.0.1/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    81087 2024-04-17 04:24:43.000000 datalad-1.0.1/versioneer.py
```

### Comparing `datalad-1.0.0/CHANGELOG.md` & `datalad-1.0.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,18 @@
 
+<a id='changelog-1.0.1'></a>
+# 1.0.1 (2024-04-17)
+
+## 🏠 Internal
+
+- The main entrypoint for annex remotes now also runs the standard extension
+  load hook. This enables extensions to alter annex remote implementation
+  behavior in the same way than other DataLad components.
+  (by [@mih](https://github.com/mih))
+
 <a id='changelog-1.0.0'></a>
 # 1.0.0 (2024-04-06)
 
 ## 💥 Breaking Changes
 
 - Merging maint to make the first major release.  [PR #7577](https://github.com/datalad/datalad/pull/7577) (by [@yarikoptic](https://github.com/yarikoptic))
```

### Comparing `datalad-1.0.0/CONTRIBUTING.md` & `datalad-1.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/CONTRIBUTORS` & `datalad-1.0.1/CONTRIBUTORS`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/COPYING` & `datalad-1.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/MANIFEST.in` & `datalad-1.0.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/Makefile` & `datalad-1.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/PKG-INFO` & `datalad-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad
-Version: 1.0.0
+Version: 1.0.1
 Summary: data distribution geared toward scientific datasets
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
 Project-URL: Homepage, https://www.datalad.org
 Project-URL: Developer docs, https://docs.datalad.org/en/stable
 Project-URL: User handbook, https://handbook.datalad.org
 Project-URL: Source, https://github.com/datalad/datalad
```

### Comparing `datalad-1.0.0/README.md` & `datalad-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/_datalad_build_support/__init__.py` & `datalad-1.0.1/_datalad_build_support/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/_datalad_build_support/formatters.py` & `datalad-1.0.1/_datalad_build_support/formatters.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/_datalad_build_support/setup.py` & `datalad-1.0.1/_datalad_build_support/setup.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/asv.conf.json` & `datalad-1.0.1/asv.conf.json`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/benchmarks/api.py` & `datalad-1.0.1/benchmarks/api.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/benchmarks/cli.py` & `datalad-1.0.1/benchmarks/cli.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/benchmarks/common.py` & `datalad-1.0.1/benchmarks/common.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/benchmarks/core.py` & `datalad-1.0.1/benchmarks/core.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/benchmarks/plugins/addurls.py` & `datalad-1.0.1/benchmarks/plugins/addurls.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/benchmarks/repo.py` & `datalad-1.0.1/benchmarks/repo.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/benchmarks/support/path.py` & `datalad-1.0.1/benchmarks/support/path.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/benchmarks/usecases.py` & `datalad-1.0.1/benchmarks/usecases.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/__init__.py` & `datalad-1.0.1/datalad/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/__main__.py` & `datalad-1.0.1/datalad/__main__.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/api.py` & `datalad-1.0.1/datalad/api.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/cli/common_args.py` & `datalad-1.0.1/datalad/cli/common_args.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/cli/exec.py` & `datalad-1.0.1/datalad/cli/exec.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/cli/helpers.py` & `datalad-1.0.1/datalad/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/cli/interface.py` & `datalad-1.0.1/datalad/cli/interface.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/cli/main.py` & `datalad-1.0.1/datalad/cli/main.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/cli/parser.py` & `datalad-1.0.1/datalad/cli/parser.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/cli/renderer.py` & `datalad-1.0.1/datalad/cli/renderer.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/cli/tests/test_exec.py` & `datalad-1.0.1/datalad/cli/tests/test_exec.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/cli/tests/test_formatters.py` & `datalad-1.0.1/datalad/cli/tests/test_formatters.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/cli/tests/test_helpers.py` & `datalad-1.0.1/datalad/cli/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/cli/tests/test_interface.py` & `datalad-1.0.1/datalad/cli/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/cli/tests/test_main.py` & `datalad-1.0.1/datalad/cli/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/cli/tests/test_parser.py` & `datalad-1.0.1/datalad/cli/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/cli/tests/test_utils.py` & `datalad-1.0.1/datalad/cli/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/cli/utils.py` & `datalad-1.0.1/datalad/cli/utils.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/cmd.py` & `datalad-1.0.1/datalad/cmd.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/cmdline/__init__.py` & `datalad-1.0.1/datalad/cmdline/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/cmdline/helpers.py` & `datalad-1.0.1/datalad/cmdline/helpers.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/cmdline/main.py` & `datalad-1.0.1/datalad/cmdline/main.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/config.py` & `datalad-1.0.1/datalad/config.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/conftest.py` & `datalad-1.0.1/datalad/conftest.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/consts.py` & `datalad-1.0.1/datalad/consts.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/core/__init__.py` & `datalad-1.0.1/datalad/core/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/core/distributed/clone.py` & `datalad-1.0.1/datalad/core/distributed/clone.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/core/distributed/clone_ephemeral.py` & `datalad-1.0.1/datalad/core/distributed/clone_ephemeral.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/core/distributed/clone_ria.py` & `datalad-1.0.1/datalad/core/distributed/clone_ria.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/core/distributed/clone_utils.py` & `datalad-1.0.1/datalad/core/distributed/clone_utils.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/core/distributed/push.py` & `datalad-1.0.1/datalad/core/distributed/push.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/core/distributed/tests/test_clone.py` & `datalad-1.0.1/datalad/core/distributed/tests/test_clone.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/core/distributed/tests/test_push.py` & `datalad-1.0.1/datalad/core/distributed/tests/test_push.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/core/local/__init__.py` & `datalad-1.0.1/datalad/core/local/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/core/local/create.py` & `datalad-1.0.1/datalad/core/local/create.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/core/local/diff.py` & `datalad-1.0.1/datalad/core/local/diff.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/core/local/repo.py` & `datalad-1.0.1/datalad/core/local/repo.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/core/local/resulthooks.py` & `datalad-1.0.1/datalad/core/local/resulthooks.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/core/local/run.py` & `datalad-1.0.1/datalad/core/local/run.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/core/local/save.py` & `datalad-1.0.1/datalad/core/local/save.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/core/local/status.py` & `datalad-1.0.1/datalad/core/local/status.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/core/local/tests/test_create.py` & `datalad-1.0.1/datalad/core/local/tests/test_create.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/core/local/tests/test_diff.py` & `datalad-1.0.1/datalad/core/local/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/core/local/tests/test_resulthooks.py` & `datalad-1.0.1/datalad/core/local/tests/test_resulthooks.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/core/local/tests/test_results.py` & `datalad-1.0.1/datalad/core/local/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/core/local/tests/test_run.py` & `datalad-1.0.1/datalad/core/local/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/core/local/tests/test_save.py` & `datalad-1.0.1/datalad/core/local/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/core/local/tests/test_status.py` & `datalad-1.0.1/datalad/core/local/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/coreapi.py` & `datalad-1.0.1/datalad/coreapi.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/customremotes/__init__.py` & `datalad-1.0.1/datalad/customremotes/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/customremotes/archives.py` & `datalad-1.0.1/datalad/customremotes/archives.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/customremotes/base.py` & `datalad-1.0.1/datalad/customremotes/base.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/customremotes/datalad.py` & `datalad-1.0.1/datalad/customremotes/datalad.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/customremotes/main.py` & `datalad-1.0.1/datalad/customremotes/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,14 +56,21 @@
     # cleanup
     if hasattr(remote, 'stop'):
         remote.stop()
 
 
 def main(args=None, cls=None, remote_name=None, description=None):
     import sys
+    from datalad.support.entrypoints import load_extensions
+    # load extensions requested by configuration
+    # analog to what coreapi is doing for a Python session
+    # importantly, load them prior to parser construction, such
+    # that CLI tuning is also within reach for extensions
+    load_extensions()
+
     parser = setup_parser(remote_name, description)
     # parse cmd args
     args = parser.parse_args(args)
 
     # stdin/stdout will be used for interactions with annex
     ui.set_backend('annex')
```

### Comparing `datalad-1.0.0/datalad/customremotes/ria_remote.py` & `datalad-1.0.1/datalad/customremotes/ria_remote.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/customremotes/ria_utils.py` & `datalad-1.0.1/datalad/customremotes/ria_utils.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/customremotes/tests/test_archives.py` & `datalad-1.0.1/datalad/customremotes/tests/test_archives.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/customremotes/tests/test_base.py` & `datalad-1.0.1/datalad/customremotes/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/customremotes/tests/test_datalad.py` & `datalad-1.0.1/datalad/customremotes/tests/test_datalad.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/customremotes/tests/test_main.py` & `datalad-1.0.1/datalad/customremotes/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/customremotes/tests/test_ria_utils.py` & `datalad-1.0.1/datalad/customremotes/tests/test_ria_utils.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/dataset/gitrepo.py` & `datalad-1.0.1/datalad/dataset/gitrepo.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/dataset/repo.py` & `datalad-1.0.1/datalad/dataset/repo.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/dataset/tests/test_gitrepo.py` & `datalad-1.0.1/datalad/dataset/tests/test_gitrepo.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distributed/__init__.py` & `datalad-1.0.1/datalad/distributed/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distributed/create_sibling_ghlike.py` & `datalad-1.0.1/datalad/distributed/create_sibling_ghlike.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distributed/create_sibling_gin.py` & `datalad-1.0.1/datalad/distributed/create_sibling_gin.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distributed/create_sibling_gitea.py` & `datalad-1.0.1/datalad/distributed/create_sibling_gitea.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distributed/create_sibling_github.py` & `datalad-1.0.1/datalad/distributed/create_sibling_github.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distributed/create_sibling_gitlab.py` & `datalad-1.0.1/datalad/distributed/create_sibling_gitlab.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distributed/create_sibling_gogs.py` & `datalad-1.0.1/datalad/distributed/create_sibling_gogs.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distributed/create_sibling_ria.py` & `datalad-1.0.1/datalad/distributed/create_sibling_ria.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distributed/drop.py` & `datalad-1.0.1/datalad/distributed/drop.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distributed/export_archive_ora.py` & `datalad-1.0.1/datalad/distributed/export_archive_ora.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distributed/export_to_figshare.py` & `datalad-1.0.1/datalad/distributed/export_to_figshare.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distributed/ora_remote.py` & `datalad-1.0.1/datalad/distributed/ora_remote.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distributed/tests/ria_utils.py` & `datalad-1.0.1/datalad/distributed/tests/ria_utils.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distributed/tests/test_create_sibling_ghlike.py` & `datalad-1.0.1/datalad/distributed/tests/test_create_sibling_ghlike.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distributed/tests/test_create_sibling_gin.py` & `datalad-1.0.1/datalad/distributed/tests/test_create_sibling_gin.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distributed/tests/test_create_sibling_gitea.py` & `datalad-1.0.1/datalad/distributed/tests/test_create_sibling_gitea.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distributed/tests/test_create_sibling_github.py` & `datalad-1.0.1/datalad/distributed/tests/test_create_sibling_github.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distributed/tests/test_create_sibling_gitlab.py` & `datalad-1.0.1/datalad/distributed/tests/test_create_sibling_gitlab.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distributed/tests/test_create_sibling_gogs.py` & `datalad-1.0.1/datalad/distributed/tests/test_create_sibling_gogs.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distributed/tests/test_create_sibling_ria.py` & `datalad-1.0.1/datalad/distributed/tests/test_create_sibling_ria.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distributed/tests/test_drop.py` & `datalad-1.0.1/datalad/distributed/tests/test_drop.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distributed/tests/test_export_to_figshare.py` & `datalad-1.0.1/datalad/distributed/tests/test_export_to_figshare.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distributed/tests/test_ora_http.py` & `datalad-1.0.1/datalad/distributed/tests/test_ora_http.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distributed/tests/test_ria.py` & `datalad-1.0.1/datalad/distributed/tests/test_ria.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distributed/tests/test_ria_basics.py` & `datalad-1.0.1/datalad/distributed/tests/test_ria_basics.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distributed/tests/test_ria_git_remote.py` & `datalad-1.0.1/datalad/distributed/tests/test_ria_git_remote.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/create_sibling.py` & `datalad-1.0.1/datalad/distribution/create_sibling.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/create_sibling_github.py` & `datalad-1.0.1/datalad/distribution/create_sibling_github.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/create_test_dataset.py` & `datalad-1.0.1/datalad/distribution/create_test_dataset.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/dataset.py` & `datalad-1.0.1/datalad/distribution/dataset.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/drop.py` & `datalad-1.0.1/datalad/distribution/drop.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/get.py` & `datalad-1.0.1/datalad/distribution/get.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/install.py` & `datalad-1.0.1/datalad/distribution/install.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/remove.py` & `datalad-1.0.1/datalad/distribution/remove.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/siblings.py` & `datalad-1.0.1/datalad/distribution/siblings.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/subdatasets.py` & `datalad-1.0.1/datalad/distribution/subdatasets.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/tests/test_create_sibling.py` & `datalad-1.0.1/datalad/distribution/tests/test_create_sibling.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/tests/test_create_test_dataset.py` & `datalad-1.0.1/datalad/distribution/tests/test_create_test_dataset.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/tests/test_dataset.py` & `datalad-1.0.1/datalad/distribution/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/tests/test_dataset_api.py` & `datalad-1.0.1/datalad/distribution/tests/test_dataset_api.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/tests/test_dataset_binding.py` & `datalad-1.0.1/datalad/distribution/tests/test_dataset_binding.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/tests/test_drop.py` & `datalad-1.0.1/datalad/distribution/tests/test_drop.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/tests/test_get.py` & `datalad-1.0.1/datalad/distribution/tests/test_get.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/tests/test_install.py` & `datalad-1.0.1/datalad/distribution/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/tests/test_siblings.py` & `datalad-1.0.1/datalad/distribution/tests/test_siblings.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/tests/test_uninstall.py` & `datalad-1.0.1/datalad/distribution/tests/test_uninstall.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/tests/test_update.py` & `datalad-1.0.1/datalad/distribution/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/tests/test_utils.py` & `datalad-1.0.1/datalad/distribution/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/tests/vcr_cassettes/github_datalad_tester_org.yaml` & `datalad-1.0.1/datalad/distribution/tests/vcr_cassettes/github_datalad_tester_org.yaml`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/tests/vcr_cassettes/github_yarikoptic.yaml` & `datalad-1.0.1/datalad/distribution/tests/vcr_cassettes/github_yarikoptic.yaml`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/uninstall.py` & `datalad-1.0.1/datalad/distribution/uninstall.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/update.py` & `datalad-1.0.1/datalad/distribution/update.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/distribution/utils.py` & `datalad-1.0.1/datalad/distribution/utils.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/dochelpers.py` & `datalad-1.0.1/datalad/dochelpers.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/downloaders/__init__.py` & `datalad-1.0.1/datalad/downloaders/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/downloaders/base.py` & `datalad-1.0.1/datalad/downloaders/base.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/downloaders/configs/crcns.cfg` & `datalad-1.0.1/datalad/downloaders/configs/crcns.cfg`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/downloaders/configs/hcp.cfg` & `datalad-1.0.1/datalad/downloaders/configs/hcp.cfg`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/downloaders/configs/kaggle.cfg` & `datalad-1.0.1/datalad/downloaders/configs/kaggle.cfg`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/downloaders/configs/nda.cfg` & `datalad-1.0.1/datalad/downloaders/configs/nda.cfg`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/downloaders/configs/nitrc.cfg` & `datalad-1.0.1/datalad/downloaders/configs/nitrc.cfg`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/downloaders/credentials.py` & `datalad-1.0.1/datalad/downloaders/credentials.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/downloaders/http.py` & `datalad-1.0.1/datalad/downloaders/http.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/downloaders/providers.py` & `datalad-1.0.1/datalad/downloaders/providers.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/downloaders/s3.py` & `datalad-1.0.1/datalad/downloaders/s3.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/downloaders/shub.py` & `datalad-1.0.1/datalad/downloaders/shub.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/downloaders/tests/test_credentials.py` & `datalad-1.0.1/datalad/downloaders/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/downloaders/tests/test_docker_registry.py` & `datalad-1.0.1/datalad/downloaders/tests/test_docker_registry.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/downloaders/tests/test_http.py` & `datalad-1.0.1/datalad/downloaders/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/downloaders/tests/test_providers.py` & `datalad-1.0.1/datalad/downloaders/tests/test_providers.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/downloaders/tests/test_s3.py` & `datalad-1.0.1/datalad/downloaders/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/downloaders/tests/test_shub.py` & `datalad-1.0.1/datalad/downloaders/tests/test_shub.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/downloaders/tests/utils.py` & `datalad-1.0.1/datalad/downloaders/tests/utils.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/interface/__init__.py` & `datalad-1.0.1/datalad/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/interface/add_archive_content.py` & `datalad-1.0.1/datalad/interface/add_archive_content.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/interface/base.py` & `datalad-1.0.1/datalad/interface/base.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/interface/clean.py` & `datalad-1.0.1/datalad/interface/clean.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/interface/common_cfg.py` & `datalad-1.0.1/datalad/interface/common_cfg.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/interface/common_opts.py` & `datalad-1.0.1/datalad/interface/common_opts.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/interface/download_url.py` & `datalad-1.0.1/datalad/interface/download_url.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/interface/rerun.py` & `datalad-1.0.1/datalad/interface/rerun.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/interface/results.py` & `datalad-1.0.1/datalad/interface/results.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/interface/run_procedure.py` & `datalad-1.0.1/datalad/interface/run_procedure.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/interface/shell_completion.py` & `datalad-1.0.1/datalad/interface/shell_completion.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/interface/tests/test_base.py` & `datalad-1.0.1/datalad/interface/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/interface/tests/test_docs.py` & `datalad-1.0.1/datalad/interface/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/interface/tests/test_results.py` & `datalad-1.0.1/datalad/interface/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/interface/tests/test_shell_completion.py` & `datalad-1.0.1/datalad/interface/tests/test_shell_completion.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/interface/tests/test_utils.py` & `datalad-1.0.1/datalad/interface/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/interface/unlock.py` & `datalad-1.0.1/datalad/interface/unlock.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/interface/utils.py` & `datalad-1.0.1/datalad/interface/utils.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/__init__.py` & `datalad-1.0.1/datalad/local/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/add_archive_content.py` & `datalad-1.0.1/datalad/local/add_archive_content.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/add_readme.py` & `datalad-1.0.1/datalad/local/add_readme.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/addurls.py` & `datalad-1.0.1/datalad/local/addurls.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/check_dates.py` & `datalad-1.0.1/datalad/local/check_dates.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/clean.py` & `datalad-1.0.1/datalad/local/clean.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/configuration.py` & `datalad-1.0.1/datalad/local/configuration.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/copy_file.py` & `datalad-1.0.1/datalad/local/copy_file.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/download_url.py` & `datalad-1.0.1/datalad/local/download_url.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/export_archive.py` & `datalad-1.0.1/datalad/local/export_archive.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/foreach_dataset.py` & `datalad-1.0.1/datalad/local/foreach_dataset.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/gitcredential.py` & `datalad-1.0.1/datalad/local/gitcredential.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/gitcredential_datalad.py` & `datalad-1.0.1/datalad/local/gitcredential_datalad.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/no_annex.py` & `datalad-1.0.1/datalad/local/no_annex.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/remove.py` & `datalad-1.0.1/datalad/local/remove.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/rerun.py` & `datalad-1.0.1/datalad/local/rerun.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/run_procedure.py` & `datalad-1.0.1/datalad/local/run_procedure.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/subdatasets.py` & `datalad-1.0.1/datalad/local/subdatasets.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/tests/test_add_archive_content.py` & `datalad-1.0.1/datalad/local/tests/test_add_archive_content.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/tests/test_add_readme.py` & `datalad-1.0.1/datalad/local/tests/test_add_readme.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/tests/test_addurls.py` & `datalad-1.0.1/datalad/local/tests/test_addurls.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/tests/test_check_dates.py` & `datalad-1.0.1/datalad/local/tests/test_check_dates.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/tests/test_clean.py` & `datalad-1.0.1/datalad/local/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/tests/test_configuration.py` & `datalad-1.0.1/datalad/local/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/tests/test_copy_file.py` & `datalad-1.0.1/datalad/local/tests/test_copy_file.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/tests/test_download_url.py` & `datalad-1.0.1/datalad/local/tests/test_download_url.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/tests/test_export_archive.py` & `datalad-1.0.1/datalad/local/tests/test_export_archive.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/tests/test_foreach_dataset.py` & `datalad-1.0.1/datalad/local/tests/test_foreach_dataset.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/tests/test_gitcredential.py` & `datalad-1.0.1/datalad/local/tests/test_gitcredential.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/tests/test_no_annex.py` & `datalad-1.0.1/datalad/local/tests/test_no_annex.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/tests/test_remove.py` & `datalad-1.0.1/datalad/local/tests/test_remove.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/tests/test_rerun.py` & `datalad-1.0.1/datalad/local/tests/test_rerun.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/tests/test_rerun_merges.py` & `datalad-1.0.1/datalad/local/tests/test_rerun_merges.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/tests/test_run_procedure.py` & `datalad-1.0.1/datalad/local/tests/test_run_procedure.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/tests/test_subdataset.py` & `datalad-1.0.1/datalad/local/tests/test_subdataset.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/tests/test_unlock.py` & `datalad-1.0.1/datalad/local/tests/test_unlock.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/tests/test_wtf.py` & `datalad-1.0.1/datalad/local/tests/test_wtf.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/unlock.py` & `datalad-1.0.1/datalad/local/unlock.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/local/wtf.py` & `datalad-1.0.1/datalad/local/wtf.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/log.py` & `datalad-1.0.1/datalad/log.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/resources/procedures/cfg_noannex.py` & `datalad-1.0.1/datalad/resources/procedures/cfg_noannex.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/resources/procedures/cfg_text2git.py` & `datalad-1.0.1/datalad/resources/procedures/cfg_text2git.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/resources/procedures/cfg_yoda.py` & `datalad-1.0.1/datalad/resources/procedures/cfg_yoda.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/resources/procedures/tests/test_noannex.py` & `datalad-1.0.1/datalad/resources/procedures/tests/test_noannex.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/runner/__init__.py` & `datalad-1.0.1/datalad/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/runner/coreprotocols.py` & `datalad-1.0.1/datalad/runner/coreprotocols.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/runner/exception.py` & `datalad-1.0.1/datalad/runner/exception.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/runner/gitrunner.py` & `datalad-1.0.1/datalad/runner/gitrunner.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/runner/nonasyncrunner.py` & `datalad-1.0.1/datalad/runner/nonasyncrunner.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/runner/protocol.py` & `datalad-1.0.1/datalad/runner/protocol.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/runner/runner.py` & `datalad-1.0.1/datalad/runner/runner.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/runner/runnerthreads.py` & `datalad-1.0.1/datalad/runner/runnerthreads.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/runner/tests/test_exception.py` & `datalad-1.0.1/datalad/runner/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/runner/tests/test_generatormixin.py` & `datalad-1.0.1/datalad/runner/tests/test_generatormixin.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/runner/tests/test_gitrunner.py` & `datalad-1.0.1/datalad/runner/tests/test_gitrunner.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/runner/tests/test_nonasyncrunner.py` & `datalad-1.0.1/datalad/runner/tests/test_nonasyncrunner.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/runner/tests/test_threadsafety.py` & `datalad-1.0.1/datalad/runner/tests/test_threadsafety.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/runner/tests/test_utils.py` & `datalad-1.0.1/datalad/runner/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/runner/tests/test_witless_runner.py` & `datalad-1.0.1/datalad/runner/tests/test_witless_runner.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/runner/utils.py` & `datalad-1.0.1/datalad/runner/utils.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/annex_utils.py` & `datalad-1.0.1/datalad/support/annex_utils.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/annexrepo.py` & `datalad-1.0.1/datalad/support/annexrepo.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/ansi_colors.py` & `datalad-1.0.1/datalad/support/ansi_colors.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/archive_utils_7z.py` & `datalad-1.0.1/datalad/support/archive_utils_7z.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/archive_utils_patool.py` & `datalad-1.0.1/datalad/support/archive_utils_patool.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/archives.py` & `datalad-1.0.1/datalad/support/archives.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/cache.py` & `datalad-1.0.1/datalad/support/cache.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/collections.py` & `datalad-1.0.1/datalad/support/collections.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/constraints.py` & `datalad-1.0.1/datalad/support/constraints.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/cookies.py` & `datalad-1.0.1/datalad/support/cookies.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/digests.py` & `datalad-1.0.1/datalad/support/digests.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/due.py` & `datalad-1.0.1/datalad/support/due.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/due_utils.py` & `datalad-1.0.1/datalad/support/due_utils.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/entrypoints.py` & `datalad-1.0.1/datalad/support/entrypoints.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/exceptions.py` & `datalad-1.0.1/datalad/support/exceptions.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/extensions.py` & `datalad-1.0.1/datalad/support/extensions.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/external_versions.py` & `datalad-1.0.1/datalad/support/external_versions.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/gitrepo.py` & `datalad-1.0.1/datalad/support/gitrepo.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/globbedpaths.py` & `datalad-1.0.1/datalad/support/globbedpaths.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/itertools.py` & `datalad-1.0.1/datalad/support/itertools.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/json_py.py` & `datalad-1.0.1/datalad/support/json_py.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/keyring_.py` & `datalad-1.0.1/datalad/support/keyring_.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/locking.py` & `datalad-1.0.1/datalad/support/locking.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/nda_.py` & `datalad-1.0.1/datalad/support/nda_.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/network.py` & `datalad-1.0.1/datalad/support/network.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/parallel.py` & `datalad-1.0.1/datalad/support/parallel.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/param.py` & `datalad-1.0.1/datalad/support/param.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/path.py` & `datalad-1.0.1/datalad/support/path.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/repodates.py` & `datalad-1.0.1/datalad/support/repodates.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/s3.py` & `datalad-1.0.1/datalad/support/s3.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/sshconnector.py` & `datalad-1.0.1/datalad/support/sshconnector.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/sshrun.py` & `datalad-1.0.1/datalad/support/sshrun.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/stats.py` & `datalad-1.0.1/datalad/support/stats.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/status.py` & `datalad-1.0.1/datalad/support/status.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/strings.py` & `datalad-1.0.1/datalad/support/strings.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/tests/test_annexrepo.py` & `datalad-1.0.1/datalad/support/tests/test_annexrepo.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/tests/test_ansi_colors.py` & `datalad-1.0.1/datalad/support/tests/test_ansi_colors.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/tests/test_cache.py` & `datalad-1.0.1/datalad/support/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/tests/test_captured_exception.py` & `datalad-1.0.1/datalad/support/tests/test_captured_exception.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/tests/test_cookies.py` & `datalad-1.0.1/datalad/support/tests/test_cookies.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/tests/test_digests.py` & `datalad-1.0.1/datalad/support/tests/test_digests.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/tests/test_due_utils.py` & `datalad-1.0.1/datalad/support/tests/test_due_utils.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/tests/test_extensions.py` & `datalad-1.0.1/datalad/support/tests/test_extensions.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/tests/test_external_versions.py` & `datalad-1.0.1/datalad/support/tests/test_external_versions.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/tests/test_fileinfo.py` & `datalad-1.0.1/datalad/support/tests/test_fileinfo.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/tests/test_gitrepo.py` & `datalad-1.0.1/datalad/support/tests/test_gitrepo.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/tests/test_globbedpaths.py` & `datalad-1.0.1/datalad/support/tests/test_globbedpaths.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/tests/test_json_py.py` & `datalad-1.0.1/datalad/support/tests/test_json_py.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/tests/test_locking.py` & `datalad-1.0.1/datalad/support/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/tests/test_network.py` & `datalad-1.0.1/datalad/support/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/tests/test_parallel.py` & `datalad-1.0.1/datalad/support/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/tests/test_path.py` & `datalad-1.0.1/datalad/support/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/tests/test_repo_save.py` & `datalad-1.0.1/datalad/support/tests/test_repo_save.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/tests/test_repodates.py` & `datalad-1.0.1/datalad/support/tests/test_repodates.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/tests/test_sshconnector.py` & `datalad-1.0.1/datalad/support/tests/test_sshconnector.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/tests/test_sshrun.py` & `datalad-1.0.1/datalad/support/tests/test_sshrun.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/tests/test_stats.py` & `datalad-1.0.1/datalad/support/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/tests/test_status.py` & `datalad-1.0.1/datalad/support/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/tests/test_vcr_.py` & `datalad-1.0.1/datalad/support/tests/test_vcr_.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/third/loris_token_generator.py` & `datalad-1.0.1/datalad/support/third/loris_token_generator.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/third/nda_aws_token_generator.py` & `datalad-1.0.1/datalad/support/third/nda_aws_token_generator.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/support/vcr_.py` & `datalad-1.0.1/datalad/support/vcr_.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/__init__.py` & `datalad-1.0.1/datalad/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/ca/README` & `datalad-1.0.1/datalad/tests/ca/README`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/ca/ca-key.pem` & `datalad-1.0.1/datalad/tests/ca/ca-key.pem`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/ca/ca-root.pem` & `datalad-1.0.1/datalad/tests/ca/ca-root.pem`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/ca/ca_bundle.pem` & `datalad-1.0.1/datalad/tests/ca/ca_bundle.pem`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/ca/certificate-key.pem` & `datalad-1.0.1/datalad/tests/ca/certificate-key.pem`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/ca/certificate-pub.pem` & `datalad-1.0.1/datalad/tests/ca/certificate-pub.pem`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/ca/certificate.csr` & `datalad-1.0.1/datalad/tests/ca/certificate.csr`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/test__main__.py` & `datalad-1.0.1/datalad/tests/test__main__.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/test_api.py` & `datalad-1.0.1/datalad/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/test_archives.py` & `datalad-1.0.1/datalad/tests/test_archives.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/test_base.py` & `datalad-1.0.1/datalad/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/test_cmd.py` & `datalad-1.0.1/datalad/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/test_config.py` & `datalad-1.0.1/datalad/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/test_constraints.py` & `datalad-1.0.1/datalad/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/test_direct_mode.py` & `datalad-1.0.1/datalad/tests/test_direct_mode.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/test_dochelpers.py` & `datalad-1.0.1/datalad/tests/test_dochelpers.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/test_installed.py` & `datalad-1.0.1/datalad/tests/test_installed.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/test_interface.py` & `datalad-1.0.1/datalad/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/test_log.py` & `datalad-1.0.1/datalad/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/test_misc.py` & `datalad-1.0.1/datalad/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/test_s3.py` & `datalad-1.0.1/datalad/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/test_strings.py` & `datalad-1.0.1/datalad/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/test_tests_utils_pytest.py` & `datalad-1.0.1/datalad/tests/test_tests_utils_pytest.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/test_utils.py` & `datalad-1.0.1/datalad/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/test_utils_cached_dataset.py` & `datalad-1.0.1/datalad/tests/test_utils_cached_dataset.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/test_utils_testrepos.py` & `datalad-1.0.1/datalad/tests/test_utils_testrepos.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/test_version.py` & `datalad-1.0.1/datalad/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/utils_cached_dataset.py` & `datalad-1.0.1/datalad/tests/utils_cached_dataset.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/utils_pytest.py` & `datalad-1.0.1/datalad/tests/utils_pytest.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/utils_testdatasets.py` & `datalad-1.0.1/datalad/tests/utils_testdatasets.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/tests/utils_testrepos.py` & `datalad-1.0.1/datalad/tests/utils_testrepos.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/typing.py` & `datalad-1.0.1/datalad/typing.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/ui/__init__.py` & `datalad-1.0.1/datalad/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/ui/base.py` & `datalad-1.0.1/datalad/ui/base.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/ui/dialog.py` & `datalad-1.0.1/datalad/ui/dialog.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/ui/progressbars.py` & `datalad-1.0.1/datalad/ui/progressbars.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/ui/tests/test_base.py` & `datalad-1.0.1/datalad/ui/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/ui/tests/test_dialog.py` & `datalad-1.0.1/datalad/ui/tests/test_dialog.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/ui/utils.py` & `datalad-1.0.1/datalad/ui/utils.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/utils.py` & `datalad-1.0.1/datalad/utils.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad/version.py` & `datalad-1.0.1/datalad/version.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad.egg-info/PKG-INFO` & `datalad-1.0.1/datalad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad
-Version: 1.0.0
+Version: 1.0.1
 Summary: data distribution geared toward scientific datasets
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
 Project-URL: Homepage, https://www.datalad.org
 Project-URL: Developer docs, https://docs.datalad.org/en/stable
 Project-URL: User handbook, https://handbook.datalad.org
 Project-URL: Source, https://github.com/datalad/datalad
```

### Comparing `datalad-1.0.0/datalad.egg-info/SOURCES.txt` & `datalad-1.0.1/datalad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/datalad.egg-info/requires.txt` & `datalad-1.0.1/datalad.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/Makefile` & `datalad-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/casts/basic_search.sh` & `datalad-1.0.1/docs/casts/basic_search.sh`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/casts/boxcom.sh` & `datalad-1.0.1/docs/casts/boxcom.sh`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/casts/cmdline_basic_usage.sh` & `datalad-1.0.1/docs/casts/cmdline_basic_usage.sh`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/casts/datalad_convenience_vs_git.sh` & `datalad-1.0.1/docs/casts/datalad_convenience_vs_git.sh`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/casts/heudiconv_dicom_to_bids.sh` & `datalad-1.0.1/docs/casts/heudiconv_dicom_to_bids.sh`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/casts/publish_on_github.sh` & `datalad-1.0.1/docs/casts/publish_on_github.sh`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/casts/reproducible_analysis.sh` & `datalad-1.0.1/docs/casts/reproducible_analysis.sh`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/casts/seamless_nested_repos.sh` & `datalad-1.0.1/docs/casts/seamless_nested_repos.sh`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/casts/simple_provenance_tracking.sh` & `datalad-1.0.1/docs/casts/simple_provenance_tracking.sh`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/casts/track_data_from_webpage.sh` & `datalad-1.0.1/docs/casts/track_data_from_webpage.sh`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/config-format.rst` & `datalad-1.0.1/docs/config-format.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/design.rst` & `datalad-1.0.1/docs/design.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/_static/datalad_logo.png` & `datalad-1.0.1/docs/source/_static/datalad_logo.png`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/_static/favicon.ico` & `datalad-1.0.1/docs/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/acknowledgements.rst` & `datalad-1.0.1/docs/source/acknowledgements.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/background.rst` & `datalad-1.0.1/docs/source/background.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/basics.rst` & `datalad-1.0.1/docs/source/basics.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/basics_cmdline.rst.in` & `datalad-1.0.1/docs/source/basics_cmdline.rst.in`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/basics_nesteddatasets.rst.in` & `datalad-1.0.1/docs/source/basics_nesteddatasets.rst.in`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/changelog.rst` & `datalad-1.0.1/docs/source/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 .. This file is auto-converted from CHANGELOG.md (make update-changelog) -- do not edit
 
 Change log
 **********
+1.0.1 (2024-04-17)
+==================
+
+Internal
+--------
+
+-  The main entrypoint for annex remotes now also runs the standard
+   extension load hook. This enables extensions to alter annex remote
+   implementation behavior in the same way than other DataLad
+   components. (by `@mih <https://github.com/mih>`__)
+
+.. _section-1:
+
 1.0.0 (2024-04-06)
 ==================
 
 Breaking Changes
 ----------------
 
 -  Merging maint to make the first major release. `PR
@@ -16,55 +29,57 @@
 -----------------------------
 
 -  Increase minimal Git version to 2.25. Fixes
    `#7389 <https://github.com/datalad/datalad/issues/7389>`__ via `PR
    #7431 <https://github.com/datalad/datalad/pull/7431>`__ (by
    `@adswa <https://github.com/adswa>`__)
 
-.. _section-1:
+.. _section-2:
 
 0.19.6 (2024-02-02)
 ===================
 
 .. _enhancements-and-new-features-1:
 
 Enhancements and New Features
 -----------------------------
 
 -  Add the “http_token” authentication mechanism which provides
    ‘Authentication: Token {TOKEN}’ header. `PR
    #7551 <https://github.com/datalad/datalad/pull/7551>`__ (by
    `@yarikoptic <https://github.com/yarikoptic>`__)
 
+.. _internal-1:
+
 Internal
 --------
 
 -  Update ``pytest_ignore_collect()`` for pytest 8.0. `PR
    #7546 <https://github.com/datalad/datalad/pull/7546>`__ (by
    `@jwodder <https://github.com/jwodder>`__)
 
 -  Add manual triggering support/documentation for release workflow. `PR
    #7553 <https://github.com/datalad/datalad/pull/7553>`__ (by
    `@yarikoptic <https://github.com/yarikoptic>`__)
 
-.. _section-2:
+.. _section-3:
 
 0.19.5 (2023-12-28)
 ===================
 
 Tests
 -----
 
 -  Fix text to account for a recent change in git-annex dropping
    sub-second clock precision. As a result we might not report push of
    git-annex branch since there would be none. `PR
    #7544 <https://github.com/datalad/datalad/pull/7544>`__ (by
    `@yarikoptic <https://github.com/yarikoptic>`__)
 
-.. _section-3:
+.. _section-4:
 
 0.19.4 (2023-12-13)
 ===================
 
 Bug Fixes
 ---------
 
@@ -82,15 +97,15 @@
 -------------
 
 -  Improve threaded-runner documentation. Fixes
    `#7498 <https://github.com/datalad/datalad/issues/7498>`__ via `PR
    #7500 <https://github.com/datalad/datalad/pull/7500>`__ (by
    `@christian-monch <https://github.com/christian-monch>`__)
 
-.. _internal-1:
+.. _internal-2:
 
 Internal
 --------
 
 -  add RRID to package metadata. `PR
    #7495 <https://github.com/datalad/datalad/pull/7495>`__ (by
    `@adswa <https://github.com/adswa>`__)
@@ -124,15 +139,15 @@
    `@yarikoptic <https://github.com/yarikoptic>`__)
 
 -  BF(TST): Relax matching of git-annex error message about unsafe drop,
    which was changed in 10.20231129-18-gfd0b510573. `PR
    #7541 <https://github.com/datalad/datalad/pull/7541>`__ (by
    `@yarikoptic <https://github.com/yarikoptic>`__)
 
-.. _section-4:
+.. _section-5:
 
 0.19.3 (2023-08-10)
 ===================
 
 .. _bug-fixes-1:
 
 Bug Fixes
@@ -168,15 +183,15 @@
 
 -  Fix a property name and default costs described in “getting
    subdatasets” section of ``get`` documentation. Fixes
    `#7458 <https://github.com/datalad/datalad/issues/7458>`__ via `PR
    #7460 <https://github.com/datalad/datalad/pull/7460>`__ (by
    `@mslw <https://github.com/mslw>`__)
 
-.. _internal-2:
+.. _internal-3:
 
 Internal
 --------
 
 -  Copy an adjusted environment only if requested to do so. `PR
    #7399 <https://github.com/datalad/datalad/pull/7399>`__ (by
    `@christian-monch <https://github.com/christian-monch>`__)
@@ -191,15 +206,15 @@
 Tests
 -----
 
 -  Disable some S3 tests of their VCR taping where they fail for known
    issues. `PR #7467 <https://github.com/datalad/datalad/pull/7467>`__
    (by `@yarikoptic <https://github.com/yarikoptic>`__)
 
-.. _section-5:
+.. _section-6:
 
 0.19.2 (2023-07-03)
 ===================
 
 .. _bug-fixes-2:
 
 Bug Fixes
@@ -217,20 +232,20 @@
 -------------
 
 -  DOC: clarify description of the “install” interface to reflect its
    convoluted behavior. `PR
    #7445 <https://github.com/datalad/datalad/pull/7445>`__ (by
    `@yarikoptic <https://github.com/yarikoptic>`__)
 
-.. _section-6:
+.. _section-7:
 
 0.19.1 (2023-06-26)
 ===================
 
-.. _internal-3:
+.. _internal-4:
 
 Internal
 --------
 
 -  Make compatible with upcoming release of git-annex (next after
    10.20230407) and pass explicit core.quotepath=false to all git calls.
    Also added ``tools/find-hanged-tests`` helper. `PR
@@ -243,15 +258,15 @@
 -----
 
 -  Adjust tests for upcoming release of git-annex (next after
    10.20230407) and ignore DeprecationWarning for pkg_resources for now.
    `PR #7372 <https://github.com/datalad/datalad/pull/7372>`__ (by
    `@yarikoptic <https://github.com/yarikoptic>`__)
 
-.. _section-7:
+.. _section-8:
 
 0.19.0 (2023-06-14)
 ===================
 
 .. _enhancements-and-new-features-2:
 
 Enhancements and New Features
@@ -306,15 +321,15 @@
 -----
 
 -  Remove nose-based testing utils and possibility to test extensions
    using nose. `PR
    #7261 <https://github.com/datalad/datalad/pull/7261>`__ (by
    `@yarikoptic <https://github.com/yarikoptic>`__)
 
-.. _section-8:
+.. _section-9:
 
 0.18.5 (2023-06-13)
 ===================
 
 .. _bug-fixes-4:
 
 Bug Fixes
@@ -344,15 +359,15 @@
 -------------
 
 -  Use ``sphinx_autodoc_typehints``. Fixes
    `#7404 <https://github.com/datalad/datalad/issues/7404>`__ via `PR
    #7412 <https://github.com/datalad/datalad/pull/7412>`__ (by
    `@jwodder <https://github.com/jwodder>`__)
 
-.. _internal-4:
+.. _internal-5:
 
 Internal
 --------
 
 -  Discontinue ConfigManager abuse for Git identity warning. `PR
    #7378 <https://github.com/datalad/datalad/pull/7378>`__ (by
    `@mih <https://github.com/mih>`__) and `PR
@@ -369,15 +384,15 @@
    `@yarikoptic <https://github.com/yarikoptic>`__)
 
 -  Skip test_system_ssh_version if no ssh found + split parsing into
    separate test. `PR
    #7422 <https://github.com/datalad/datalad/pull/7422>`__ (by
    `@yarikoptic <https://github.com/yarikoptic>`__)
 
-.. _section-9:
+.. _section-10:
 
 0.18.4 (2023-05-16)
 ===================
 
 .. _bug-fixes-5:
 
 Bug Fixes
@@ -396,15 +411,15 @@
 
 -  Added a workaround for an issue with documentation theme (search
    function not working on Read the Docs). Fixes
    `#7374 <https://github.com/datalad/datalad/issues/7374>`__ via `PR
    #7385 <https://github.com/datalad/datalad/pull/7385>`__ (by
    `@mslw <https://github.com/mslw>`__)
 
-.. _internal-5:
+.. _internal-6:
 
 Internal
 --------
 
 -  Type-annotate ``datalad/support/gitrepo.py``. `PR
    #7341 <https://github.com/datalad/datalad/pull/7341>`__ (by
    `@jwodder <https://github.com/jwodder>`__)
@@ -419,15 +434,15 @@
    `@yarikoptic <https://github.com/yarikoptic>`__)
 
    -  use sample S3 url DANDI archive,
    -  use our copy of old .deb from datasets.datalad.org instead of
       snapshots.d.o
    -  use specific miniconda installer for py 3.7.
 
-.. _section-10:
+.. _section-11:
 
 0.18.3 (2023-03-25)
 ===================
 
 .. _bug-fixes-6:
 
 Bug Fixes
@@ -478,15 +493,15 @@
 -------------
 
 -  Include a few previously missing commands in html API docs. Fixes
    `#7288 <https://github.com/datalad/datalad/issues/7288>`__ via `PR
    #7289 <https://github.com/datalad/datalad/pull/7289>`__ (by
    `@mslw <https://github.com/mslw>`__)
 
-.. _internal-6:
+.. _internal-7:
 
 Internal
 --------
 
 -  Type-annotate almost all of ``datalad/utils.py``; add
    ``datalad/typing.py``. `PR
    #7317 <https://github.com/datalad/datalad/pull/7317>`__ (by
@@ -527,15 +542,15 @@
    `@bpoldrack <https://github.com/bpoldrack>`__)
 
 -  Fix testing assumption - do create pure GitRepo superdataset and test
    against it. `PR
    #7353 <https://github.com/datalad/datalad/pull/7353>`__ (by
    `@yarikoptic <https://github.com/yarikoptic>`__)
 
-.. _section-11:
+.. _section-12:
 
 0.18.2 (2023-02-27)
 ===================
 
 .. _bug-fixes-7:
 
 Bug Fixes
@@ -564,15 +579,15 @@
 Dependencies
 ------------
 
 -  Revert “Revert”Remove chardet version upper limit"". `PR
    #7263 <https://github.com/datalad/datalad/pull/7263>`__ (by
    `@yarikoptic <https://github.com/yarikoptic>`__)
 
-.. _internal-7:
+.. _internal-8:
 
 Internal
 --------
 
 -  Codespell more (CHANGELOGs etc) and remove custom CLI options from
    tox.ini. `PR #7271 <https://github.com/datalad/datalad/pull/7271>`__
    (by `@yarikoptic <https://github.com/yarikoptic>`__)
@@ -584,15 +599,15 @@
 
 -  Use older python 3.8 in testing nose utils in github-action
    test-nose. Fixes
    `#7259 <https://github.com/datalad/datalad/issues/7259>`__ via `PR
    #7260 <https://github.com/datalad/datalad/pull/7260>`__ (by
    `@yarikoptic <https://github.com/yarikoptic>`__)
 
-.. _section-12:
+.. _section-13:
 
 0.18.1 (2023-01-16)
 ===================
 
 .. _bug-fixes-8:
 
 Bug Fixes
@@ -619,15 +634,15 @@
 
 -  Integrate buffer size optimization from datalad-next, leading to
    significant performance improvement for status and diff. Fixes
    `#7190 <https://github.com/datalad/datalad/issues/7190>`__ via `PR
    #7250 <https://github.com/datalad/datalad/pull/7250>`__ (by
    `@bpoldrack <https://github.com/bpoldrack>`__)
 
-.. _section-13:
+.. _section-14:
 
 0.18.0 (2022-12-31)
 ===================
 
 .. _breaking-changes-1:
 
 Breaking Changes
@@ -743,15 +758,15 @@
    `@adswa <https://github.com/adswa>`__)
 
 -  CONTRIBUTING.md was extended with up-to-date information on CI
    logging, changelog and release procedures. `PR
    #7204 <https://github.com/datalad/datalad/pull/7204>`__ (by
    `@yarikoptic <https://github.com/yarikoptic>`__)
 
-.. _internal-8:
+.. _internal-9:
 
 Internal
 --------
 
 -  Allow EnsureDataset constraint to handle Path instances. Fixes
    `#7069 <https://github.com/datalad/datalad/issues/7069>`__ via `PR
    #7133 <https://github.com/datalad/datalad/pull/7133>`__ (by
@@ -827,15 +842,15 @@
    `@adswa <https://api.github.com/users/adswa>`__)
 
 -  Remove the ``with_testrepos`` decorator and associated tests for it
    Fixes `#6752 <https://github.com/datalad/datalad/issues/6752>`__ via
    `PR #7176 <https://github.com/datalad/datalad/pull/7176>`__ (by
    `@adswa <https://api.github.com/users/adswa>`__)
 
-.. _section-14:
+.. _section-15:
 
 0.17.10 (2022-12-14)
 ====================
 
 .. _enhancements-and-new-features-4:
 
 Enhancements and New Features
@@ -920,15 +935,15 @@
 
 -  Fix documentation of ``Runner.run()`` to not accept strings. Instead,
    encoding must be ensured by the caller. Fixes
    `#7145 <https://github.com/datalad/datalad/issues/7145>`__ via `PR
    #7155 <https://github.com/datalad/datalad/pull/7155>`__ (by
    `@bpoldrack <https://github.com/bpoldrack>`__)
 
-.. _internal-9:
+.. _internal-10:
 
 Internal
 --------
 
 -  Fix import of the ``ls`` command from datalad-deprecated for
    benchmarks. Fixes
    `#7149 <https://github.com/datalad/datalad/issues/7149>`__ via `PR
@@ -958,15 +973,15 @@
 -  Use Plaintext keyring backend in tests to avoid the need for
    (interactive) authentication to unlock the keyring during (CI-) test
    runs. Fixes
    `#6623 <https://github.com/datalad/datalad/issues/6623>`__ via `PR
    #7209 <https://github.com/datalad/datalad/pull/7209>`__ (by
    `@bpoldrack <https://github.com/bpoldrack>`__)
 
-.. _section-15:
+.. _section-16:
 
 0.17.9 (2022-11-07)
 ===================
 
 .. _bug-fixes-11:
 
 Bug Fixes
@@ -1003,15 +1018,15 @@
 
 -  Remove remaining references to ``nose`` and the implied requirement
    for building the documentation Fixes
    `#7100 <https://github.com/datalad/datalad/issues/7100>`__ via `PR
    #7136 <https://github.com/datalad/datalad/pull/7136>`__ (by
    `@bpoldrack <https://github.com/bpoldrack>`__)
 
-.. _internal-10:
+.. _internal-11:
 
 Internal
 --------
 
 -  Use datalad/release-action. Fixes
    `#7110 <https://github.com/datalad/datalad/issues/7110>`__. `PR
    #7111 <https://github.com/datalad/datalad/pull/7111>`__ (by
@@ -1039,15 +1054,15 @@
    #7126 <https://github.com/datalad/datalad/pull/7126>`__ (by
    `@yarikoptic <https://github.com/yarikoptic>`__)
 
 -  Configure Git to allow for “file” protocol in tests. `PR
    #7130 <https://github.com/datalad/datalad/pull/7130>`__ (by
    `@yarikoptic <https://github.com/yarikoptic>`__)
 
-.. _section-16:
+.. _section-17:
 
 0.17.8 (2022-10-24)
 ===================
 
 .. _bug-fixes-12:
 
 Bug Fixes
@@ -1086,15 +1101,15 @@
    ``create-sibling*`` commands (``-gin``, ``-gitea``, ``-github``,
    ``-gogs``). The result messages will now display names of the
    repositories which would be created (useful for recursive
    operations). `PR
    #7103 <https://github.com/datalad/datalad/pull/7103>`__ (by
    `@mslw <https://github.com/mslw>`__)
 
-.. _section-17:
+.. _section-18:
 
 0.17.7 (2022-10-14)
 ===================
 
 .. _bug-fixes-13:
 
 Bug Fixes
@@ -1110,15 +1125,15 @@
    via https://github.com/datalad/datalad/pull/7072 (by @bpoldrack)
 
 -  BF: lock across threads check/instantiation of Flyweight instances.
    Fixes `#6598 <https://github.com/datalad/datalad/issues/6598>`__ via
    `PR #7075 <https://github.com/datalad/datalad/pull/7075>`__ (by
    `@yarikoptic <https://github.com/yarikoptic>`__)
 
-.. _internal-11:
+.. _internal-12:
 
 Internal
 --------
 
 -  Do not use ``gen4``-metadata methods in ``datalad metadata``-command.
    `PR #7001 <https://github.com/datalad/datalad/pull/7001>`__ (by
    `@christian-monch <https://github.com/christian-monch>`__)
@@ -1147,15 +1162,15 @@
 Tests
 -----
 
 -  Fix broken test helpers for result record testing that would falsely
    pass. `PR #7002 <https://github.com/datalad/datalad/pull/7002>`__ (by
    `@bpoldrack <https://github.com/bpoldrack>`__)
 
-.. _section-18:
+.. _section-19:
 
 0.17.6 (2022-09-21)
 ===================
 
 .. _bug-fixes-14:
 
 Bug Fixes
@@ -1184,15 +1199,15 @@
    #7039 <https://github.com/datalad/datalad/pull/7039>`__ (by
    `@mih <https://github.com/mih>`__)
 
 -  push: Assume 0 bytes pushed if git-annex does not provide bytesize.
    `PR #7049 <https://github.com/datalad/datalad/pull/7049>`__ (by
    `@yarikoptic <https://github.com/yarikoptic>`__)
 
-.. _internal-12:
+.. _internal-13:
 
 Internal
 --------
 
 -  Use scriv for CHANGELOG generation in release workflow. `PR
    #7009 <https://github.com/datalad/datalad/pull/7009>`__ (by
    `@jwodder <https://github.com/jwodder>`__)
@@ -1629,15 +1644,15 @@
    `#6746 <https://github.com/datalad/datalad/pull/6746>`__ (by @mih)
 -  New design document on progress reporting.
    `#6734 <https://github.com/datalad/datalad/pull/6734>`__ (by @mih)
 -  Explain downstream consequences of using ``--fast`` option in
    ``addurls``. `#6684 <https://github.com/datalad/datalad/pull/6684>`__
    (by @jdkent)
 
-.. _internal-13:
+.. _internal-14:
 
 Internal
 --------
 
 -  Inline code of ``create-sibling-ria`` has been refactored to an
    internal helper to check for siblings with particular names across
    dataset hierarchies in ``datalad-next``, and is reintroduced into
@@ -2427,15 +2442,15 @@
    provide an overview of basic principles and customization
    possibilities
    `#6391 <https://github.com/datalad/datalad/pull/6391>`__ (by @mih)
 -  ``--since=^`` mode of operation of ``create-sibling`` is documented
    now `#6436 <https://github.com/datalad/datalad/pull/6436>`__ (by
    @yarikoptic)
 
-.. _internal-14:
+.. _internal-15:
 
 Internal
 --------
 
 -  The internal ``status()`` helper was equipped with docstrings and
    promotes “breadth-first” reporting with a new parameter
    ``reporting_order``
@@ -2857,15 +2872,15 @@
 
 Pushed to ``maint``
 -------------------
 
 -  CI: Enable new codecov uploader in Appveyor CI
    (`@adswa <https://github.com/adswa>`__)
 
-.. _internal-15:
+.. _internal-16:
 
 Internal
 --------
 
 -  UX: Log clone-candidate number and URLs
    `#6092 <https://github.com/datalad/datalad/pull/6092>`__
    (`@adswa <https://github.com/adswa>`__)
@@ -3013,15 +3028,15 @@
 
 Pushed to ``maint``
 -------------------
 
 -  Discontinue testing of hirni extension
    (`@mih <https://github.com/mih>`__)
 
-.. _internal-16:
+.. _internal-17:
 
 Internal
 --------
 
 -  Add debugging information to release step
    `#5980 <https://github.com/datalad/datalad/pull/5980>`__
    (`@jwodder <https://github.com/jwodder>`__)
@@ -3458,15 +3473,15 @@
 -------------------
 
 -  Merge branch ‘bf-http-headers-agent’ into maint
    (`@yarikoptic <https://github.com/yarikoptic>`__)
 -  RF(BF?)+DOC: provide User-Agent to entire session headers + use those
    if provided (`@yarikoptic <https://github.com/yarikoptic>`__)
 
-.. _internal-17:
+.. _internal-18:
 
 Internal
 --------
 
 -  Pass ``--no-changelog`` to ``auto shipit`` if changelog already has
    entry `#5952 <https://github.com/datalad/datalad/pull/5952>`__
    (`@jwodder <https://github.com/jwodder>`__)
@@ -3548,15 +3563,15 @@
    ERROR if argcomplete fails to import
    `#5781 <https://github.com/datalad/datalad/pull/5781>`__
    (`@yarikoptic <https://github.com/yarikoptic>`__)
 -  ENH (UX): add python-gitlab dependency
    `#5776 <https://github.com/datalad/datalad/pull/5776>`__
    (s.heunis@fz-juelich.de)
 
-.. _internal-18:
+.. _internal-19:
 
 Internal
 --------
 
 -  BF: Fix reported paths in ORA remote
    `#5821 <https://github.com/datalad/datalad/pull/5821>`__
    (`@adswa <https://github.com/adswa>`__)
@@ -3588,15 +3603,15 @@
 -  Yaroslav Halchenko (`@yarikoptic <https://github.com/yarikoptic>`__)
 
 --------------
 
 0.14.6 (Sun Jun 27 2021)
 ========================
 
-.. _internal-19:
+.. _internal-20:
 
 Internal
 --------
 
 -  BF: update changelog conversion from .md to .rst (for sphinx)
    `#5757 <https://github.com/datalad/datalad/pull/5757>`__
    (`@yarikoptic <https://github.com/yarikoptic>`__
@@ -3699,15 +3714,15 @@
 .. _pushed-to-maint-6:
 
 Pushed to ``maint``
 -------------------
 
 -  MNT: Post-release dance (`@kyleam <https://github.com/kyleam>`__)
 
-.. _internal-20:
+.. _internal-21:
 
 Internal
 --------
 
 -  Switch to versioneer and auto
    `#5669 <https://github.com/datalad/datalad/pull/5669>`__
    (`@jwodder <https://github.com/jwodder>`__
```

### Comparing `datalad-1.0.0/docs/source/cmdline.rst` & `datalad-1.0.1/docs/source/cmdline.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/conf.py` & `datalad-1.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/config.rst` & `datalad-1.0.1/docs/source/config.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/credentials.rst` & `datalad-1.0.1/docs/source/credentials.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/customization.rst` & `datalad-1.0.1/docs/source/customization.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/design/application_vs_library_mode.rst` & `datalad-1.0.1/docs/source/design/application_vs_library_mode.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/design/batched_command.rst` & `datalad-1.0.1/docs/source/design/batched_command.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/design/cli.rst` & `datalad-1.0.1/docs/source/design/cli.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/design/credentials.rst` & `datalad-1.0.1/docs/source/design/credentials.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/design/dataset_argument.rst` & `datalad-1.0.1/docs/source/design/dataset_argument.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/design/docstrings.rst` & `datalad-1.0.1/docs/source/design/docstrings.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/design/drop.rst` & `datalad-1.0.1/docs/source/design/drop.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/design/exception_handling.rst` & `datalad-1.0.1/docs/source/design/exception_handling.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/design/file_url_handling.rst` & `datalad-1.0.1/docs/source/design/file_url_handling.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/design/github_actions.rst` & `datalad-1.0.1/docs/source/design/github_actions.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/design/index.rst` & `datalad-1.0.1/docs/source/design/index.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/design/log_levels.rst` & `datalad-1.0.1/docs/source/design/log_levels.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/design/miscpatterns.rst` & `datalad-1.0.1/docs/source/design/miscpatterns.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/design/pos_vs_kw_parameters.rst` & `datalad-1.0.1/docs/source/design/pos_vs_kw_parameters.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/design/progress_reporting.rst` & `datalad-1.0.1/docs/source/design/progress_reporting.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/design/provenance_capture.rst` & `datalad-1.0.1/docs/source/design/provenance_capture.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/design/python_imports.rst` & `datalad-1.0.1/docs/source/design/python_imports.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/design/result_records.rst` & `datalad-1.0.1/docs/source/design/result_records.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/design/standard_parameters.rst` & `datalad-1.0.1/docs/source/design/standard_parameters.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/design/testing.rst` & `datalad-1.0.1/docs/source/design/testing.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/design/threaded_runner.rst` & `datalad-1.0.1/docs/source/design/threaded_runner.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/design/url_substitution.rst` & `datalad-1.0.1/docs/source/design/url_substitution.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/design/user_messaging.rst` & `datalad-1.0.1/docs/source/design/user_messaging.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/glossary.rst` & `datalad-1.0.1/docs/source/glossary.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/index.rst` & `datalad-1.0.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/modref.rst` & `datalad-1.0.1/docs/source/modref.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/publications.rst` & `datalad-1.0.1/docs/source/publications.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/source/related.rst` & `datalad-1.0.1/docs/source/related.rst`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/docs/utils/pygments_ansi_color.py` & `datalad-1.0.1/docs/utils/pygments_ansi_color.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/setup.py` & `datalad-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/Dockerfile.fullmaster` & `datalad-1.0.1/tools/Dockerfile.fullmaster`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/Singularity` & `datalad-1.0.1/tools/Singularity`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/adhoc-httpd` & `datalad-1.0.1/tools/adhoc-httpd`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/bisect-git-annex` & `datalad-1.0.1/tools/bisect-git-annex`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/changelog-todo` & `datalad-1.0.1/tools/changelog-todo`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/checkpwd.py` & `datalad-1.0.1/tools/checkpwd.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/ci/appveyor_ssh2localhost.bat` & `datalad-1.0.1/tools/ci/appveyor_ssh2localhost.bat`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/ci/benchmark-travis-pr.sh` & `datalad-1.0.1/tools/ci/benchmark-travis-pr.sh`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/ci/bisect-python.sh` & `datalad-1.0.1/tools/ci/bisect-python.sh`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/ci/download-latest-artifact` & `datalad-1.0.1/tools/ci/download-latest-artifact`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/ci/gpg-90F7E9EB.pub` & `datalad-1.0.1/tools/ci/gpg-90F7E9EB.pub`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/ci/install-annex.sh` & `datalad-1.0.1/tools/ci/install-annex.sh`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/ci/install-singularity.sh` & `datalad-1.0.1/tools/ci/install-singularity.sh`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/ci/prep-travis-devel-annex.sh` & `datalad-1.0.1/tools/ci/prep-travis-devel-annex.sh`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/ci/prep-travis-forssh.sh` & `datalad-1.0.1/tools/ci/prep-travis-forssh.sh`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/convert-git-annex-layout` & `datalad-1.0.1/tools/convert-git-annex-layout`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/copy_urls_from_datalad.py` & `datalad-1.0.1/tools/copy_urls_from_datalad.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/coverage-bin/datalad` & `datalad-1.0.1/tools/coverage-bin/datalad`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/coverage-bin/git-annex-remote-datalad` & `datalad-1.0.1/tools/coverage-bin/git-annex-remote-datalad`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/coverage-bin/git-annex-remote-datalad-archives` & `datalad-1.0.1/tools/coverage-bin/git-annex-remote-datalad-archives`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/coverage-bin/git-annex-remote-ora` & `datalad-1.0.1/tools/coverage-bin/git-annex-remote-ora`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/describegitannex` & `datalad-1.0.1/tools/describegitannex`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/downgrade-annex` & `datalad-1.0.1/tools/downgrade-annex`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/dtime` & `datalad-1.0.1/tools/dtime`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/eval_under_nfs` & `datalad-1.0.1/tools/eval_under_nfs`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/eval_under_testloopfs` & `datalad-1.0.1/tools/eval_under_testloopfs`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/find-hanged-tests` & `datalad-1.0.1/tools/find-hanged-tests`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/git-web-submodules.sh` & `datalad-1.0.1/tools/git-web-submodules.sh`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/mimic_merges` & `datalad-1.0.1/tools/mimic_merges`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/mimic_repo` & `datalad-1.0.1/tools/mimic_repo`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/monitor-interrupts.py` & `datalad-1.0.1/tools/monitor-interrupts.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/profile_python` & `datalad-1.0.1/tools/profile_python`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/testing/make_test_repo` & `datalad-1.0.1/tools/testing/make_test_repo`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/testing/make_test_repos` & `datalad-1.0.1/tools/testing/make_test_repos`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/testing/start_website_in_docker` & `datalad-1.0.1/tools/testing/start_website_in_docker`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/testing/start_website_in_docker-Dockerfile.in` & `datalad-1.0.1/tools/testing/start_website_in_docker-Dockerfile.in`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/testing/test_README_in_docker` & `datalad-1.0.1/tools/testing/test_README_in_docker`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/testing/test_README_in_docker-Dockerfile.in` & `datalad-1.0.1/tools/testing/test_README_in_docker-Dockerfile.in`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/upgrade-annex-osx.sh` & `datalad-1.0.1/tools/upgrade-annex-osx.sh`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/urlinfo` & `datalad-1.0.1/tools/urlinfo`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tools/which.py` & `datalad-1.0.1/tools/which.py`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/tox.ini` & `datalad-1.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `datalad-1.0.0/versioneer.py` & `datalad-1.0.1/versioneer.py`

 * *Files identical despite different names*

