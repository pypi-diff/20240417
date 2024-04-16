# Comparing `tmp/littlefs-python-0.9.1.tar.gz` & `tmp/littlefs-python-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "littlefs-python-0.9.1.tar", last modified: Mon Dec 11 00:29:28 2023, max compression
+gzip compressed data, was "littlefs-python-0.9.3.tar", last modified: Tue Jan 16 18:01:23 2024, max compression
```

## Comparing `littlefs-python-0.9.1.tar` & `littlefs-python-0.9.3.tar`

### file list

```diff
@@ -1,150 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 00:29:28.658191 littlefs-python-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 00:29:28.638191 littlefs-python-0.9.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 00:29:28.638191 littlefs-python-0.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      982 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      170 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)      381 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2023-12-11 00:29:28.658191 littlefs-python-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 00:29:28.638191 littlefs-python-0.9.1/ci/
--rwxr-xr-x   0 runner    (1001) docker     (127)      860 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/ci/build-wheels.sh
--rw-r--r--   0 runner    (1001) docker     (127)      845 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/ci/download_release_files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 00:29:28.642191 littlefs-python-0.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 00:29:28.642191 littlefs-python-0.9.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      156 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/docs/doc8.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 00:29:28.642191 littlefs-python-0.9.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/docs/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      353 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      795 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 00:29:28.642191 littlefs-python-0.9.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/examples/mkfsimg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/examples/walk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 00:29:28.642191 littlefs-python-0.9.1/littlefs/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/.git
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 00:29:28.634191 littlefs-python-0.9.1/littlefs/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 00:29:28.642191 littlefs-python-0.9.1/littlefs/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/.github/workflows/post-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9157 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/.github/workflows/status.yml
--rw-r--r--   0 runner    (1001) docker     (127)    28922 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      385 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    96233 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/DESIGN.md
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    14577 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    11259 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    33650 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/SPEC.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 00:29:28.646191 littlefs-python-0.9.1/littlefs/bd/
--rw-r--r--   0 runner    (1001) docker     (127)    19614 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/bd/lfs_emubd.c
--rw-r--r--   0 runner    (1001) docker     (127)     7363 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/bd/lfs_emubd.h
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/bd/lfs_filebd.c
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/bd/lfs_filebd.h
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/bd/lfs_rambd.c
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/bd/lfs_rambd.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 00:29:28.646191 littlefs-python-0.9.1/littlefs/benches/
--rw-r--r--   0 runner    (1001) docker     (127)     7107 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/benches/bench_dir.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/benches/bench_file.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/benches/bench_superblock.toml
--rw-r--r--   0 runner    (1001) docker     (127)   190300 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/lfs.c
--rw-r--r--   0 runner    (1001) docker     (127)    25577 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/lfs.h
--rw-r--r--   0 runner    (1001) docker     (127)      907 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/lfs_util.c
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/lfs_util.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 00:29:28.646191 littlefs-python-0.9.1/littlefs/runners/
--rw-r--r--   0 runner    (1001) docker     (127)    68019 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/runners/bench_runner.c
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/runners/bench_runner.h
--rw-r--r--   0 runner    (1001) docker     (127)    92762 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/runners/test_runner.c
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/runners/test_runner.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 00:29:28.650191 littlefs-python-0.9.1/littlefs/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)    52054 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/scripts/bench.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5401 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/scripts/changeprefix.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23095 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/scripts/code.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27397 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/scripts/cov.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22943 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/scripts/data.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    45193 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/scripts/perf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    44308 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/scripts/perfbd.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    54030 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/scripts/plot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    41869 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/scripts/plotmpl.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15011 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/scripts/prettyasserts.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      858 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/scripts/readblock.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12631 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/scripts/readmdir.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6357 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/scripts/readtree.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24367 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/scripts/stack.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21064 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/scripts/structs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    25393 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/scripts/summary.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5275 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/scripts/tailpipe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1993 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/scripts/teepipe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    54598 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/scripts/test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31069 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/scripts/tracebd.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8135 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/scripts/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 00:29:28.654191 littlefs-python-0.9.1/littlefs/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    23130 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/tests/test_alloc.toml
--rw-r--r--   0 runner    (1001) docker     (127)    12219 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/tests/test_attrs.toml
--rw-r--r--   0 runner    (1001) docker     (127)     7983 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/tests/test_badblocks.toml
--rw-r--r--   0 runner    (1001) docker     (127)     6811 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/tests/test_bd.toml
--rw-r--r--   0 runner    (1001) docker     (127)    42929 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/tests/test_compat.toml
--rw-r--r--   0 runner    (1001) docker     (127)    32864 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/tests/test_dirs.toml
--rw-r--r--   0 runner    (1001) docker     (127)    22546 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/tests/test_entries.toml
--rw-r--r--   0 runner    (1001) docker     (127)    10596 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/tests/test_evil.toml
--rw-r--r--   0 runner    (1001) docker     (127)    16965 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/tests/test_exhaustion.toml
--rw-r--r--   0 runner    (1001) docker     (127)    17120 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/tests/test_files.toml
--rw-r--r--   0 runner    (1001) docker     (127)     8346 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/tests/test_interspersed.toml
--rw-r--r--   0 runner    (1001) docker     (127)    70817 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/tests/test_move.toml
--rw-r--r--   0 runner    (1001) docker     (127)     8611 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/tests/test_orphans.toml
--rw-r--r--   0 runner    (1001) docker     (127)    10658 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/tests/test_paths.toml
--rw-r--r--   0 runner    (1001) docker     (127)     5842 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/tests/test_powerloss.toml
--rw-r--r--   0 runner    (1001) docker     (127)    12400 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/tests/test_relocations.toml
--rw-r--r--   0 runner    (1001) docker     (127)    13530 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/tests/test_seek.toml
--rw-r--r--   0 runner    (1001) docker     (127)    13920 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/tests/test_superblocks.toml
--rw-r--r--   0 runner    (1001) docker     (127)    17457 2023-12-11 00:29:16.000000 littlefs-python-0.9.1/littlefs/tests/test_truncate.toml
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-11 00:29:28.658191 littlefs-python-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 00:29:28.638191 littlefs-python-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 00:29:28.654191 littlefs-python-0.9.1/src/littlefs/
--rw-r--r--   0 runner    (1001) docker     (127)    15103 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/src/littlefs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6813 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/src/littlefs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5367 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/src/littlefs/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/src/littlefs/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)  1727800 2023-12-11 00:29:28.000000 littlefs-python-0.9.1/src/littlefs/lfs.c
--rw-r--r--   0 runner    (1001) docker     (127)     5647 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/src/littlefs/lfs.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/src/littlefs/lfs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14959 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/src/littlefs/lfs.pyx
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/src/littlefs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 00:29:28.658191 littlefs-python-0.9.1/src/littlefs_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2023-12-11 00:29:28.000000 littlefs-python-0.9.1/src/littlefs_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2023-12-11 00:29:28.000000 littlefs-python-0.9.1/src/littlefs_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 00:29:28.000000 littlefs-python-0.9.1/src/littlefs_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-12-11 00:29:28.000000 littlefs-python-0.9.1/src/littlefs_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 00:29:28.000000 littlefs-python-0.9.1/src/littlefs_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-12-11 00:29:28.000000 littlefs-python-0.9.1/src/littlefs_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-11 00:29:28.000000 littlefs-python-0.9.1/src/littlefs_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 00:29:28.658191 littlefs-python-0.9.1/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 00:29:28.658191 littlefs-python-0.9.1/test/lfs/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/test/lfs/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/test/lfs/test_dir_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/test/lfs/test_file_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/test/lfs/test_fs_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/test/test_attr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/test/test_block_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/test/test_directories.py
--rw-r--r--   0 runner    (1001) docker     (127)     5225 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/test/test_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/test/test_grow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/test/test_multiversion.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/test/test_name_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/test/test_remove_rename.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/test/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2023-12-11 00:29:15.000000 littlefs-python-0.9.1/test/test_walk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:01:23.320828 littlefs-python-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:01:23.296828 littlefs-python-0.9.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:01:23.296828 littlefs-python-0.9.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-01-16 18:01:23.320828 littlefs-python-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:01:23.296828 littlefs-python-0.9.3/ci/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      861 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/ci/build-wheels.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/ci/download_release_files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:01:23.296828 littlefs-python-0.9.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:01:23.296828 littlefs-python-0.9.3/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/docs/doc8.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:01:23.296828 littlefs-python-0.9.3/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/docs/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:01:23.300828 littlefs-python-0.9.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/examples/mkfsimg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/examples/walk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:01:23.300828 littlefs-python-0.9.3/littlefs/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/.git
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:01:23.292828 littlefs-python-0.9.3/littlefs/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:01:23.300828 littlefs-python-0.9.3/littlefs/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/.github/workflows/post-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     9158 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/.github/workflows/status.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    28922 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    96235 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/DESIGN.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    33650 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/SPEC.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:01:23.304828 littlefs-python-0.9.3/littlefs/bd/
+-rw-r--r--   0 runner    (1001) docker     (127)    19614 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/bd/lfs_emubd.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/bd/lfs_emubd.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/bd/lfs_filebd.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/bd/lfs_filebd.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/bd/lfs_rambd.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/bd/lfs_rambd.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:01:23.304828 littlefs-python-0.9.3/littlefs/benches/
+-rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/benches/bench_dir.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/benches/bench_file.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/benches/bench_superblock.toml
+-rw-r--r--   0 runner    (1001) docker     (127)   190403 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/lfs.c
+-rw-r--r--   0 runner    (1001) docker     (127)    25577 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/lfs.h
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/lfs_util.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/lfs_util.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:01:23.304828 littlefs-python-0.9.3/littlefs/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)    68019 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/runners/bench_runner.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/runners/bench_runner.h
+-rw-r--r--   0 runner    (1001) docker     (127)    92762 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/runners/test_runner.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/runners/test_runner.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:01:23.308828 littlefs-python-0.9.3/littlefs/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    52054 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/scripts/bench.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5401 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/scripts/changeprefix.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23095 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/scripts/code.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27397 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/scripts/cov.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22943 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/scripts/data.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    45193 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/scripts/perf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44308 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/scripts/perfbd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    54030 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/scripts/plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    41869 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/scripts/plotmpl.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15011 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/scripts/prettyasserts.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      858 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/scripts/readblock.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12631 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/scripts/readmdir.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6357 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/scripts/readtree.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24367 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/scripts/stack.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21064 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/scripts/structs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25393 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/scripts/summary.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5275 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/scripts/tailpipe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1993 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/scripts/teepipe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    54598 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/scripts/test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31069 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/scripts/tracebd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8135 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/scripts/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:01:23.312828 littlefs-python-0.9.3/littlefs/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    23130 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/tests/test_alloc.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    12219 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/tests/test_attrs.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/tests/test_badblocks.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/tests/test_bd.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    42929 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/tests/test_compat.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    32864 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/tests/test_dirs.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    22546 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/tests/test_entries.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    10596 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/tests/test_evil.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    16965 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/tests/test_exhaustion.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    17120 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/tests/test_files.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/tests/test_interspersed.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    70817 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/tests/test_move.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/tests/test_orphans.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    10658 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/tests/test_paths.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/tests/test_powerloss.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    12400 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/tests/test_relocations.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    13530 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/tests/test_seek.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/tests/test_superblocks.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    17457 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/littlefs/tests/test_truncate.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-16 18:01:23.320828 littlefs-python-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:01:23.292828 littlefs-python-0.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:01:23.316828 littlefs-python-0.9.3/src/littlefs/
+-rw-r--r--   0 runner    (1001) docker     (127)    14860 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/src/littlefs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/src/littlefs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/src/littlefs/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/src/littlefs/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1730105 2024-01-16 18:01:22.000000 littlefs-python-0.9.3/src/littlefs/lfs.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/src/littlefs/lfs.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/src/littlefs/lfs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15004 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/src/littlefs/lfs.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/src/littlefs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:01:23.320828 littlefs-python-0.9.3/src/littlefs_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-01-16 18:01:23.000000 littlefs-python-0.9.3/src/littlefs_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-01-16 18:01:23.000000 littlefs-python-0.9.3/src/littlefs_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 18:01:23.000000 littlefs-python-0.9.3/src/littlefs_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-16 18:01:23.000000 littlefs-python-0.9.3/src/littlefs_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 18:01:22.000000 littlefs-python-0.9.3/src/littlefs_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-01-16 18:01:23.000000 littlefs-python-0.9.3/src/littlefs_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-16 18:01:23.000000 littlefs-python-0.9.3/src/littlefs_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:01:23.320828 littlefs-python-0.9.3/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:01:23.320828 littlefs-python-0.9.3/test/lfs/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/test/lfs/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/test/lfs/test_dir_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/test/lfs/test_file_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/test/lfs/test_fs_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/test/test_attr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/test/test_block_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/test/test_directories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/test/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/test/test_grow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/test/test_multiversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/test/test_name_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/test/test_remove_rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/test/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-01-16 18:01:14.000000 littlefs-python-0.9.3/test/test_walk.py
```

### Comparing `littlefs-python-0.9.1/.github/workflows/deploy.yml` & `littlefs-python-0.9.3/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/.github/workflows/run-tests.yml` & `littlefs-python-0.9.3/.github/workflows/run-tests.yml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         python-version: [3.8, 3.9, "3.10", "3.11"]
 
     steps:
       - uses: actions/checkout@v4
         with:
           submodules: "recursive"
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -r requirements.txt
           pip install -e .
```

### Comparing `littlefs-python-0.9.1/LICENSE` & `littlefs-python-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/PKG-INFO` & `littlefs-python-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: littlefs-python
-Version: 0.9.1
+Version: 0.9.3
 Summary: A python wrapper for littlefs
 Home-page: https://github.com/jrast/littlefs-python
 Author: Jürg Rast
 Author-email: juergr@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `littlefs-python-0.9.1/README.rst` & `littlefs-python-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/ci/build-wheels.sh` & `littlefs-python-0.9.3/ci/build-wheels.sh`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -27,8 +27,8 @@
         continue
     fi
     if [[ "${PYBIN}" == *"cp34"* ]]; then
         continue
     fi
     "${PYBIN}/pip" install littlefs-python --no-index -f /io/wheels
     "${PYBIN}/py.test" /io/test
-done
+done
```

### Comparing `littlefs-python-0.9.1/ci/download_release_files.py` & `littlefs-python-0.9.3/ci/download_release_files.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import requests
 import os
 
 HERE = os.path.dirname(__file__)
-DIST_DIR = os.path.abspath(os.path.join(HERE, '..', 'dist'))
-REPO = 'jrast/littlefs-python'
+DIST_DIR = os.path.abspath(os.path.join(HERE, "..", "dist"))
+REPO = "jrast/littlefs-python"
 
 if not os.path.exists(DIST_DIR):
     os.mkdir(DIST_DIR)
 
-resp = requests.get('https://api.github.com/repos/%s/releases/latest' % REPO)
+resp = requests.get("https://api.github.com/repos/%s/releases/latest" % REPO)
 
 if resp.status_code != 200:
-    raise RuntimeError('Github API call failed!')
+    raise RuntimeError("Github API call failed!")
 
 data = resp.json()
 
-print('Release Tag:', data['tag_name'])
+print("Release Tag:", data["tag_name"])
 
-print('Assets:')
-num_assets = len(data['assets'])
-for nr, e in enumerate(data['assets'], 1):
-    print('(%2d/%2d) Downloading %s' % (nr, num_assets, e['name']))
-    r = requests.get(e['browser_download_url'], allow_redirects=True)
+print("Assets:")
+num_assets = len(data["assets"])
+for nr, e in enumerate(data["assets"], 1):
+    print("(%2d/%2d) Downloading %s" % (nr, num_assets, e["name"]))
+    r = requests.get(e["browser_download_url"], allow_redirects=True)
     if r.status_code != 200:
-        raise RuntimeError('Downloading %s failed!' % e['name'])
-    with open(os.path.join(DIST_DIR, e['name']), 'wb') as fh:
+        raise RuntimeError("Downloading %s failed!" % e["name"])
+    with open(os.path.join(DIST_DIR, e["name"]), "wb") as fh:
         fh.write(r.content)
-
```

### Comparing `littlefs-python-0.9.1/docs/Makefile` & `littlefs-python-0.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/docs/conf.py` & `littlefs-python-0.9.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/docs/examples/index.rst` & `littlefs-python-0.9.3/docs/examples/index.rst`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/docs/make.bat` & `littlefs-python-0.9.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/docs/usage.rst` & `littlefs-python-0.9.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/examples/mkfsimg.py` & `littlefs-python-0.9.3/examples/mkfsimg.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/examples/walk.py` & `littlefs-python-0.9.3/examples/walk.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/.github/workflows/post-release.yml` & `littlefs-python-0.9.3/littlefs/.github/workflows/post-release.yml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/.github/workflows/release.yml` & `littlefs-python-0.9.3/littlefs/.github/workflows/release.yml`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
           do
             # per-config results
             c_or_default=${c:-default}
             c_camel=${c_or_default^}
             table[$i,$j]=$c_camel
             ((j+=1))
 
-            for s in code stack struct
+            for s in code stack structs
             do
               f=sizes/thumb${c:+-$c}.$s.csv
               [ -e $f ] && table[$i,$j]=$( \
                 export PREV="$(jq -re '
                     select(.context == "'"sizes (thumb${c:+, $c}) / $s"'").description
                     | capture("(?<prev>[0-9∞]+)").prev' \
                   prev-status.json || echo 0)"
```

### Comparing `littlefs-python-0.9.1/littlefs/.github/workflows/status.yml` & `littlefs-python-0.9.3/littlefs/.github/workflows/status.yml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/.github/workflows/test.yml` & `littlefs-python-0.9.3/littlefs/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/DESIGN.md` & `littlefs-python-0.9.3/littlefs/DESIGN.md`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 1. **Bounded RAM/ROM** - If the above requirements weren't enough, these
    systems also have very limited amounts of memory. This prevents many
    existing filesystem designs, which can lean on relatively large amounts of
    RAM to temporarily store filesystem metadata.
 
    For ROM, this means we need to keep our design simple and reuse code paths
-   were possible. For RAM we have a stronger requirement, all RAM usage is
+   where possible. For RAM we have a stronger requirement, all RAM usage is
    bounded. This means RAM usage does not grow as the filesystem changes in
    size or number of files. This creates a unique challenge as even presumably
    simple operations, such as traversing the filesystem, become surprisingly
    difficult.
 
 ## Existing designs?
 
@@ -622,15 +622,15 @@
 The rules CTZ skip-lists follow are that for every _n_&zwj;th block where _n_
 is divisible by 2&zwj;_&#739;_, that block contains a pointer to block
 _n_-2&zwj;_&#739;_. This means that each block contains anywhere from 1 to
 log&#8322;_n_ pointers that skip to different preceding elements of the
 skip-list.
 
 The name comes from heavy use of the [CTZ instruction][wikipedia-ctz], which
-lets us calculate the power-of-two factors efficiently. For a give block _n_,
+lets us calculate the power-of-two factors efficiently. For a given block _n_,
 that block contains ctz(_n_)+1 pointers.
 
 ```
 A backwards CTZ skip-list
 .--------.  .--------.  .--------.  .--------.  .--------.  .--------.
 | data 0 |<-| data 1 |<-| data 2 |<-| data 3 |<-| data 4 |<-| data 5 |
 |        |<-|        |--|        |<-|        |--|        |  |        |
```

### Comparing `littlefs-python-0.9.1/littlefs/LICENSE.md` & `littlefs-python-0.9.3/littlefs/LICENSE.md`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/Makefile` & `littlefs-python-0.9.3/littlefs/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 BENCH_TRACE := $(BENCH_RUNNER:%=%.trace)
 BENCH_CSV   := $(BENCH_RUNNER:%=%.csv)
 
 CFLAGS += -fcallgraph-info=su
 CFLAGS += -g3
 CFLAGS += -I.
 CFLAGS += -std=c99 -Wall -Wextra -pedantic
+CFLAGS += -Wmissing-prototypes
 CFLAGS += -ftrack-macro-expansion=0
 ifdef DEBUG
 CFLAGS += -O0
 else
 CFLAGS += -Os
 endif
 ifdef TRACE
@@ -350,14 +351,15 @@
 			$(BUILDDIR)/lfs.data.csv \
 			$(BUILDDIR)/lfs.stack.csv \
 			$(BUILDDIR)/lfs.structs.csv \
 			-q $(SUMMARYFLAGS) -o-))
 
 ## Build the test-runner
 .PHONY: test-runner build-test
+test-runner build-test: CFLAGS+=-Wno-missing-prototypes
 ifndef NO_COV
 test-runner build-test: CFLAGS+=--coverage
 endif
 ifdef YES_PERF
 test-runner build-test: CFLAGS+=-fno-omit-frame-pointer
 endif
 ifdef YES_PERFBD
@@ -401,14 +403,15 @@
 	$(strip ./scripts/summary.py $^ \
 		-bsuite \
 		-fpassed=test_passed \
 		$(SUMMARYFLAGS) -d $(BUILDDIR)/lfs.test.csv)
 
 ## Build the bench-runner
 .PHONY: bench-runner build-bench
+bench-runner build-bench: CFLAGS+=-Wno-missing-prototypes
 ifdef YES_COV
 bench-runner build-bench: CFLAGS+=--coverage
 endif
 ifdef YES_PERF
 bench-runner build-bench: CFLAGS+=-fno-omit-frame-pointer
 endif
 ifndef NO_PERFBD
```

### Comparing `littlefs-python-0.9.1/littlefs/README.md` & `littlefs-python-0.9.3/littlefs/README.md`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/SPEC.md` & `littlefs-python-0.9.3/littlefs/SPEC.md`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/bd/lfs_emubd.c` & `littlefs-python-0.9.3/littlefs/bd/lfs_emubd.c`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/bd/lfs_emubd.h` & `littlefs-python-0.9.3/littlefs/bd/lfs_emubd.h`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/bd/lfs_filebd.c` & `littlefs-python-0.9.3/littlefs/bd/lfs_filebd.c`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/bd/lfs_filebd.h` & `littlefs-python-0.9.3/littlefs/bd/lfs_filebd.h`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/bd/lfs_rambd.c` & `littlefs-python-0.9.3/littlefs/bd/lfs_rambd.c`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/bd/lfs_rambd.h` & `littlefs-python-0.9.3/littlefs/bd/lfs_rambd.h`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/benches/bench_dir.toml` & `littlefs-python-0.9.3/littlefs/benches/bench_dir.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/benches/bench_file.toml` & `littlefs-python-0.9.3/littlefs/benches/bench_file.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/benches/bench_superblock.toml` & `littlefs-python-0.9.3/littlefs/benches/bench_superblock.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/lfs.c` & `littlefs-python-0.9.3/littlefs/lfs.c`

 * *Files 1% similar despite different names*

```diff
@@ -2147,17 +2147,19 @@
         // oh no! we're writing too much to the superblock,
         // should we expand?
         lfs_ssize_t size = lfs_fs_rawsize(lfs);
         if (size < 0) {
             return size;
         }
 
-        // do we have extra space? littlefs can't reclaim this space
-        // by itself, so expand cautiously
-        if ((lfs_size_t)size < lfs->block_count/2) {
+        // littlefs cannot reclaim expanded superblocks, so expand cautiously
+        //
+        // if our filesystem is more than ~88% full, don't expand, this is
+        // somewhat arbitrary
+        if (lfs->block_count - size > lfs->block_count/8) {
             LFS_DEBUG("Expanding superblock at rev %"PRIu32, dir->rev);
             int err = lfs_dir_split(lfs, dir, attrs, attrcount,
                     source, begin, end);
             if (err && err != LFS_ERR_NOSPC) {
                 return err;
             }
 
@@ -4995,15 +4997,15 @@
     }
 
     return 0;
 }
 #endif
 
 #ifndef LFS_READONLY
-int lfs_fs_rawmkconsistent(lfs_t *lfs) {
+static int lfs_fs_rawmkconsistent(lfs_t *lfs) {
     // lfs_fs_forceconsistency does most of the work here
     int err = lfs_fs_forceconsistency(lfs);
     if (err) {
         return err;
     }
 
     // do we have any pending gstate?
@@ -5042,15 +5044,15 @@
         return err;
     }
 
     return size;
 }
 
 #ifndef LFS_READONLY
-int lfs_fs_rawgrow(lfs_t *lfs, lfs_size_t block_count) {
+static int lfs_fs_rawgrow(lfs_t *lfs, lfs_size_t block_count) {
     // shrinking is not supported
     LFS_ASSERT(block_count >= lfs->block_count);
 
     if (block_count > lfs->block_count) {
         lfs->block_count = block_count;
 
         // fetch the root
```

### Comparing `littlefs-python-0.9.1/littlefs/lfs.h` & `littlefs-python-0.9.3/littlefs/lfs.h`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/lfs_util.c` & `littlefs-python-0.9.3/littlefs/lfs_util.c`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/lfs_util.h` & `littlefs-python-0.9.3/littlefs/lfs_util.h`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/runners/bench_runner.c` & `littlefs-python-0.9.3/littlefs/runners/bench_runner.c`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/runners/bench_runner.h` & `littlefs-python-0.9.3/littlefs/runners/bench_runner.h`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/runners/test_runner.c` & `littlefs-python-0.9.3/littlefs/runners/test_runner.c`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/runners/test_runner.h` & `littlefs-python-0.9.3/littlefs/runners/test_runner.h`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/scripts/bench.py` & `littlefs-python-0.9.3/littlefs/scripts/bench.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/scripts/changeprefix.py` & `littlefs-python-0.9.3/littlefs/scripts/changeprefix.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/scripts/code.py` & `littlefs-python-0.9.3/littlefs/scripts/code.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/scripts/cov.py` & `littlefs-python-0.9.3/littlefs/scripts/cov.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/scripts/data.py` & `littlefs-python-0.9.3/littlefs/scripts/data.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/scripts/perf.py` & `littlefs-python-0.9.3/littlefs/scripts/perf.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/scripts/perfbd.py` & `littlefs-python-0.9.3/littlefs/scripts/perfbd.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/scripts/plot.py` & `littlefs-python-0.9.3/littlefs/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/scripts/plotmpl.py` & `littlefs-python-0.9.3/littlefs/scripts/plotmpl.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/scripts/prettyasserts.py` & `littlefs-python-0.9.3/littlefs/scripts/prettyasserts.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/scripts/readblock.py` & `littlefs-python-0.9.3/littlefs/scripts/readblock.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/scripts/readmdir.py` & `littlefs-python-0.9.3/littlefs/scripts/readmdir.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/scripts/readtree.py` & `littlefs-python-0.9.3/littlefs/scripts/readtree.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/scripts/stack.py` & `littlefs-python-0.9.3/littlefs/scripts/stack.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/scripts/structs.py` & `littlefs-python-0.9.3/littlefs/scripts/structs.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/scripts/summary.py` & `littlefs-python-0.9.3/littlefs/scripts/summary.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/scripts/tailpipe.py` & `littlefs-python-0.9.3/littlefs/scripts/tailpipe.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/scripts/teepipe.py` & `littlefs-python-0.9.3/littlefs/scripts/teepipe.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/scripts/test.py` & `littlefs-python-0.9.3/littlefs/scripts/test.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/scripts/tracebd.py` & `littlefs-python-0.9.3/littlefs/scripts/tracebd.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/scripts/watch.py` & `littlefs-python-0.9.3/littlefs/scripts/watch.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/tests/test_alloc.toml` & `littlefs-python-0.9.3/littlefs/tests/test_alloc.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/tests/test_attrs.toml` & `littlefs-python-0.9.3/littlefs/tests/test_attrs.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/tests/test_badblocks.toml` & `littlefs-python-0.9.3/littlefs/tests/test_badblocks.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/tests/test_bd.toml` & `littlefs-python-0.9.3/littlefs/tests/test_bd.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/tests/test_compat.toml` & `littlefs-python-0.9.3/littlefs/tests/test_compat.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/tests/test_dirs.toml` & `littlefs-python-0.9.3/littlefs/tests/test_dirs.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/tests/test_entries.toml` & `littlefs-python-0.9.3/littlefs/tests/test_entries.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/tests/test_evil.toml` & `littlefs-python-0.9.3/littlefs/tests/test_evil.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/tests/test_exhaustion.toml` & `littlefs-python-0.9.3/littlefs/tests/test_exhaustion.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/tests/test_files.toml` & `littlefs-python-0.9.3/littlefs/tests/test_files.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/tests/test_interspersed.toml` & `littlefs-python-0.9.3/littlefs/tests/test_interspersed.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/tests/test_move.toml` & `littlefs-python-0.9.3/littlefs/tests/test_move.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/tests/test_orphans.toml` & `littlefs-python-0.9.3/littlefs/tests/test_orphans.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/tests/test_paths.toml` & `littlefs-python-0.9.3/littlefs/tests/test_paths.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/tests/test_powerloss.toml` & `littlefs-python-0.9.3/littlefs/tests/test_powerloss.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/tests/test_relocations.toml` & `littlefs-python-0.9.3/littlefs/tests/test_relocations.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/tests/test_seek.toml` & `littlefs-python-0.9.3/littlefs/tests/test_seek.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/tests/test_superblocks.toml` & `littlefs-python-0.9.3/littlefs/tests/test_superblocks.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/littlefs/tests/test_truncate.toml` & `littlefs-python-0.9.3/littlefs/tests/test_truncate.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/setup.py` & `littlefs-python-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.9.1/src/littlefs/__init__.py` & `littlefs-python-0.9.3/src/littlefs/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,18 +49,19 @@
     pass
 
 from .context import UserContext, UserContextWinDisk
 
 if TYPE_CHECKING:
     from .lfs import LFSStat
 
+
 class LittleFS:
     """Littlefs file system"""
 
-    def __init__(self, context:Optional['UserContext']=None, mount=True, **kwargs) -> None:
+    def __init__(self, context: Optional["UserContext"] = None, mount=True, **kwargs) -> None:
         self.cfg = lfs.LFSConfig(context=context, **kwargs)
         self.fs = lfs.LFSFilesystem()
 
         if mount:
             try:
                 self.mount()
             except errors.LittleFSError:
@@ -68,15 +69,15 @@
                 self.mount()
 
     @property
     def block_count(self) -> int:
         return self.fs.block_count
 
     @property
-    def context(self) -> 'UserContext':
+    def context(self) -> "UserContext":
         """User context of the file system"""
         return self.cfg.user_context
 
     def format(self) -> int:
         """Format the underlying buffer"""
         if self.cfg.block_count == 0:
             # ``lfs.format`` looks at cfg's block_count.
@@ -94,30 +95,24 @@
 
     def fs_mkconsistent(self) -> int:
         """Attempt to make the filesystem consistent and ready for writing"""
         return lfs.fs_mkconsistent(self.fs)
 
     def fs_grow(self, block_count: int) -> int:
         if block_count < self.block_count:
-            raise ValueError(f"Supplied {block_count=} cannot be smaller than current block_count {self.block_count}")
+            raise ValueError(f"Supplied block_count='{block_count}' cannot be smaller than current block_count {self.block_count}")
 
         return lfs.fs_grow(self.fs, block_count)
 
-    def fs_stat(self) -> 'LFSFSStat':
+    def fs_stat(self) -> "LFSFSStat":
         """Get the status of the filesystem"""
         return lfs.fs_stat(self.fs)
 
     def open(
-        self,
-        fname: str,
-        mode='r',
-        buffering: int = -1,
-        encoding: str = None,
-        errors: str = None,
-        newline: str = None
+        self, fname: str, mode="r", buffering: int = -1, encoding: str = None, errors: str = None, newline: str = None
     ) -> IO:
         """Open a file.
 
         :attr:`mode` is an optional string that specifies the mode in which
         the file is opened and is analogous to the built-in :func:`io.open`
         function. Files opened in text mode (default) will take and return
         `str` objects. Files opened in binary mode will take and return
@@ -170,33 +165,25 @@
 
         if text and binary:
             raise ValueError("can't have text and binary mode at once")
 
         exclusive_modes = (creating, reading, writing, appending)
 
         if sum(int(m) for m in exclusive_modes) > 1:
-            raise ValueError(
-                "must have exactly one of create/read/write/append mode"
-            )
+            raise ValueError("must have exactly one of create/read/write/append mode")
 
         if binary:
             if encoding is not None:
-                raise ValueError(
-                    "binary mode doesn't take an encoding argument"
-                )
+                raise ValueError("binary mode doesn't take an encoding argument")
 
             if errors is not None:
-                raise ValueError(
-                    "binary mode doesn't take an errors argument"
-                )
+                raise ValueError("binary mode doesn't take an errors argument")
 
             if newline is not None:
-                raise ValueError(
-                    "binary mode doesn't take a newline argument"
-                )
+                raise ValueError("binary mode doesn't take a newline argument")
 
             if buffering == 1:
                 msg = (
                     "line buffering (buffering=1) isn't supported in "
                     "binary mode, the default buffer size will be used"
                 )
                 warnings.warn(msg, RuntimeWarning)
@@ -240,21 +227,15 @@
             buffered = io.BufferedReader(raw, buffering)
         else:
             raise ValueError(f"Unknown mode: '{mode}'")
 
         if binary:
             return buffered
 
-        wrapped = io.TextIOWrapper(
-            buffered,
-            encoding,
-            errors,
-            newline,
-            line_buffering
-        )
+        wrapped = io.TextIOWrapper(buffered, encoding, errors, newline, line_buffering)
 
         return wrapped
 
     def getattr(self, path: str, typ: Union[str, bytes, int]) -> bytes:
         typ = _typ_to_uint8(typ)
         return lfs.getattr(self.fs, path, typ)
 
@@ -262,15 +243,15 @@
         typ = _typ_to_uint8(typ)
         lfs.setattr(self.fs, path, typ, data)
 
     def removeattr(self, path: str, typ: Union[str, bytes, int]) -> None:
         typ = _typ_to_uint8(typ)
         lfs.removeattr(self.fs, path, typ)
 
-    def listdir(self, path='.') -> List[str]:
+    def listdir(self, path=".") -> List[str]:
         """List directory content
 
         List the content of a directory. This function uses :meth:`scandir`
         internally. Using :meth:`scandir` might be better if you are
         searching for a specific file or need access to the :class:`littlefs.lfs.LFSStat`
         of the files.
         """
@@ -286,18 +267,18 @@
                     e.code, path
                 )
                 raise FileExistsError(msg) from e
             raise
 
     def makedirs(self, name: str, exist_ok=False):
         """Recursive directory creation function."""
-        parts = [p for p in name.split('/') if p]
-        current_name = ''
+        parts = [p for p in name.split("/") if p]
+        current_name = ""
         for nr, part in enumerate(parts):
-            current_name += '/%s' % part
+            current_name += "/%s" % part
             try:
                 self.mkdir(current_name)
             except FileExistsError as e:
                 is_last = nr == len(parts) - 1
                 if (not is_last) or (is_last and exist_ok):
                     continue
                 raise e
@@ -337,21 +318,21 @@
         """Remove directories recursively
 
         This works like :func:`remove` but if the leaf directory
         is empty after the successful removal of :attr:`name`, the
         function tries to recursively remove all parent directories
         which are also empty.
         """
-        parts = name.split('/')
+        parts = name.split("/")
         while parts:
             try:
-                name = '/'.join(parts)
+                name = "/".join(parts)
                 if not name:
                     break
-                self.remove('/'.join(parts))
+                self.remove("/".join(parts))
             except errors.LittleFSError as e:
                 if e.code == LittleFSError.Error.LFS_ERR_NOTEMPTY:
                     break
                 raise e
             parts.pop()
 
     def rename(self, src: str, dst: str) -> int:
@@ -361,25 +342,25 @@
     def rmdir(self, path: str) -> int:
         """Remove a directory
 
         This function is an alias for :func:`remove`
         """
         return self.remove(path)
 
-    def scandir(self, path='.') -> Iterator['LFSStat']:
+    def scandir(self, path=".") -> Iterator["LFSStat"]:
         """List directory content"""
         dh = lfs.dir_open(self.fs, path)
         info = lfs.dir_read(self.fs, dh)
         while info:
-            if info.name not in ['.', '..']:
+            if info.name not in [".", ".."]:
                 yield info
             info = lfs.dir_read(self.fs, dh)
         lfs.dir_close(self.fs, dh)
 
-    def stat(self, path: str) -> 'LFSStat':
+    def stat(self, path: str) -> "LFSStat":
         """Get the status of a file or directory"""
         return lfs.stat(self.fs, path)
 
     def unlink(self, path: str) -> int:
         """Remove a file or directory
 
         This function is an alias for :func:`remove`.
@@ -404,15 +385,15 @@
             if elem.type == 1:
                 files.append(elem.name)
             elif elem.type == 2:
                 dirs.append(elem.name)
 
         yield top, dirs, files
         for dirname in dirs:
-            newtop = '/'.join((top, dirname)).replace('//', '/')
+            newtop = "/".join((top, dirname)).replace("//", "/")
             yield from self.walk(newtop)
 
 
 class FileHandle(io.RawIOBase):
     def __init__(self, fs, fh):
         super().__init__()
 
@@ -483,17 +464,18 @@
 
         return lfs.file_read(self.fs, self.fh, size)
 
     def flush(self):
         super().flush()
         lfs.file_sync(self.fs, self.fh)
 
+
 def _typ_to_uint8(typ):
     try:
         out = ord(typ)
     except TypeError:
         out = int(typ)
 
-    if not(0 <= out <= 255):
+    if not (0 <= out <= 255):
         raise ValueError(f"type must be in range [0, 255]")
 
     return out
```

### Comparing `littlefs-python-0.9.1/src/littlefs/__main__.py` & `littlefs-python-0.9.3/src/littlefs/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 def _fs_from_args(args: argparse.Namespace) -> LittleFS:
     return LittleFS(
         block_size=args.block_size,
         block_count=args.block_count,
         name_max=args.name_max,
     )
 
+
 def size_parser(size_str):
     """Parse filesystem / block size in different formats"""
     size_str = str(size_str).lower()
 
     # Check if the string starts with '0x', which indicates a hexadecimal number
     if size_str.startswith("0x"):
         base = 16
@@ -150,30 +151,24 @@
             Create, extract and inspect LittleFS filesystem images. Use one of the
             commands listed below, the '-h' / '--help' option can be used on each
             command to learn more about the usage.
             """
         ),
         # formatter_class=argparse.RawTextHelpFormatter,
     )
-    parser.add_argument('--version', action='version', version=__version__)
+    parser.add_argument("--version", action="version", version=__version__)
 
     common_parser = argparse.ArgumentParser(add_help=False)
     common_parser.add_argument("-v", "--verbose", action="count", default=0)
-    common_parser.add_argument(
-        "--block-size", type=size_parser, required=True, help="LittleFS block size"
-    )
-    common_parser.add_argument(
-        "--name-max", type=size_parser, default=255, help="LittleFS max file path length."
-    )
+    common_parser.add_argument("--block-size", type=size_parser, required=True, help="LittleFS block size")
+    common_parser.add_argument("--name-max", type=size_parser, default=255, help="LittleFS max file path length.")
     group = common_parser.add_mutually_exclusive_group(required=True)
     group.add_argument("--block-count", type=int, help="LittleFS block count")
     group.add_argument("--fs-size", type=size_parser, help="LittleFS filesystem size")
-    common_parser.add_argument(
-        "--image", type=pathlib.Path, required=True, help="LittleFS filesystem image"
-    )
+    common_parser.add_argument("--image", type=pathlib.Path, required=True, help="LittleFS filesystem image")
 
     subparsers = parser.add_subparsers(required=True, title="Available Commands", dest="command")
 
     def add_command(handler, name="", help=""):
         subparser = subparsers.add_parser(
             name or handler.__name__, parents=[common_parser], help=help or handler.__doc__
         )
```

### Comparing `littlefs-python-0.9.1/src/littlefs/context.py` & `littlefs-python-0.9.3/src/littlefs/context.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,167 +1,171 @@
 import logging
 import typing
-import ctypes 
+import ctypes
 
 if typing.TYPE_CHECKING:
     from .lfs import LFSConfig
 
+
 class UserContext:
     """Basic User Context Implementation"""
 
     def __init__(self, buffsize: int) -> None:
         self.buffer = bytearray([0xFF] * buffsize)
 
-    def read(self, cfg: 'LFSConfig', block: int, off: int, size: int) -> bytearray:
+    def read(self, cfg: "LFSConfig", block: int, off: int, size: int) -> bytearray:
         """read data
 
         Parameters
         ----------
         cfg : ~littlefs.lfs.LFSConfig
             Filesystem configuration object
         block : int
             Block number to read
         off : int
             Offset from start of block
         size : int
             Number of bytes to read.
         """
-        logging.getLogger(__name__).debug('LFS Read : Block: %d, Offset: %d, Size=%d' % (block, off, size))
+        logging.getLogger(__name__).debug("LFS Read : Block: %d, Offset: %d, Size=%d" % (block, off, size))
         start = block * cfg.block_size + off
         end = start + size
         return self.buffer[start:end]
 
-    def prog(self, cfg: 'LFSConfig', block: int, off: int, data: bytes) -> int:
+    def prog(self, cfg: "LFSConfig", block: int, off: int, data: bytes) -> int:
         """program data
 
         Parameters
         ----------
         cfg : ~littlefs.lfs.LFSConfig
             Filesystem configuration object
         block : int
             Block number to program
         off : int
             Offset from start of block
         data : bytes
             Data to write
         """
-        logging.getLogger(__name__).debug('LFS Prog : Block: %d, Offset: %d, Data=%r' % (block, off, data))
+        logging.getLogger(__name__).debug("LFS Prog : Block: %d, Offset: %d, Data=%r" % (block, off, data))
         start = block * cfg.block_size + off
         end = start + len(data)
         self.buffer[start:end] = data
         return 0
 
-    def erase(self, cfg: 'LFSConfig', block: int) -> int:
+    def erase(self, cfg: "LFSConfig", block: int) -> int:
         """Erase a block
 
         Parameters
         ----------
         cfg : ~littlefs.lfs.LFSConfig
             Filesystem configuration object
         block : int
             Block number to read
         """
-        logging.getLogger(__name__).debug('LFS Erase: Block: %d' % block)
+        logging.getLogger(__name__).debug("LFS Erase: Block: %d" % block)
         start = block * cfg.block_size
         end = start + cfg.block_size
         self.buffer[start:end] = [0xFF] * cfg.block_size
         return 0
 
-    def sync(self, cfg: 'LFSConfig') -> int:
+    def sync(self, cfg: "LFSConfig") -> int:
         """Sync cached data
 
         Parameters
         ----------
         cfg : ~littlefs.lfs.LFSConfig
             Filesystem configuration object
         """
         return 0
 
 
-
-
-try:  
-    import win32file  
+try:
+    import win32file
 except ImportError:
     win32file = None
 
+
 class UserContextWinDisk(UserContext):
     """Windows disk/file context"""
 
-    def __init__(self, disk_path:str) -> None:
-        self.device = None # 
+    def __init__(self, disk_path: str) -> None:
+        self.device = None  #
         # if the user does not have the pywin
         if win32file == None:
-            raise ImportError("Unable to import 'win32file'. This module is required for Windows-specific functionality. Please ensure you are running on a Windows platform or install 'pywin32' using: 'pip install pywin32'.")
-        self.device = win32file.CreateFile(disk_path, win32file.GENERIC_READ, win32file.FILE_SHARE_READ, None, win32file.OPEN_EXISTING, 0, None)
+            raise ImportError(
+                "Unable to import 'win32file'. This module is required for Windows-specific functionality. Please ensure you are running on a Windows platform or install 'pywin32' using: 'pip install pywin32'."
+            )
+        self.device = win32file.CreateFile(
+            disk_path, win32file.GENERIC_READ, win32file.FILE_SHARE_READ, None, win32file.OPEN_EXISTING, 0, None
+        )
         if self.device == win32file.INVALID_HANDLE_VALUE:
             raise IOError("Could not open disk %s" % disk_path)
 
-    def read(self, cfg: 'LFSConfig', block: int, off: int, size: int) -> bytearray:
+    def read(self, cfg: "LFSConfig", block: int, off: int, size: int) -> bytearray:
         """read data
 
         Parameters
         ----------
         cfg : ~littlefs.lfs.LFSConfig
             Filesystem configuration object
         block : int
             Block number to read
         off : int
             Offset from start of block
         size : int
             Number of bytes to read.
         """
-        logging.getLogger(__name__).debug('LFS Read : Block: %d, Offset: %d, Size=%d' % (block, off, size))
+        logging.getLogger(__name__).debug("LFS Read : Block: %d, Offset: %d, Size=%d" % (block, off, size))
         start = block * cfg.block_size + off
-        
+
         win32file.SetFilePointer(self.device, start, win32file.FILE_BEGIN)
         buffer = ctypes.create_string_buffer(size)
         win32file.ReadFile(self.device, buffer)
         # store the data in the buffer and close the buffer
         data = buffer.raw
         return data
-    
-    def prog(self, cfg: 'LFSConfig', block: int, off: int, data: bytes) -> int:
+
+    def prog(self, cfg: "LFSConfig", block: int, off: int, data: bytes) -> int:
         """program data
 
         Parameters
         ----------
         cfg : ~littlefs.lfs.LFSConfig
             Filesystem configuration object
         block : int
             Block number to program
         off : int
             Offset from start of block
         data : bytes
             Data to write
         """
-        logging.getLogger(__name__).debug('LFS Prog : Block: %d, Offset: %d, Data=%r' % (block, off, data))
+        logging.getLogger(__name__).debug("LFS Prog : Block: %d, Offset: %d, Data=%r" % (block, off, data))
         start = block * cfg.block_size + off
-        
+
         win32file.SetFilePointer(self.device, start, win32file.FILE_BEGIN)
         win32file.WriteFile(self.device, data)
         return 0
-    
-    def erase(self, cfg: 'LFSConfig', block: int) -> int:
+
+    def erase(self, cfg: "LFSConfig", block: int) -> int:
         """Erase a block
 
         Parameters
         ----------
         cfg : ~littlefs.lfs.LFSConfig
             Filesystem configuration object
         block : int
             Block number to read
         """
-        logging.getLogger(__name__).debug('LFS Erase: Block: %d' % block)
+        logging.getLogger(__name__).debug("LFS Erase: Block: %d" % block)
         start = block * cfg.block_size
-        
+
         win32file.SetFilePointer(self.device, start, win32file.FILE_BEGIN)
         win32file.WriteFile(self.device, [0xFF] * cfg.block_size)
         return 0
-    
-    def sync(self, cfg: 'LFSConfig') -> int:
+
+    def sync(self, cfg: "LFSConfig") -> int:
         win32file.FlushFileBuffers(self.device)
         return 0
-    
+
     def __del__(self):
-        if self.device != None :
-            win32file.CloseHandle(self.device)
+        if self.device != None:
+            win32file.CloseHandle(self.device)
```

### Comparing `littlefs-python-0.9.1/src/littlefs/errors.py` & `littlefs-python-0.9.3/src/littlefs/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,17 +24,14 @@
         self.code = code
 
     @property
     def name(self) -> str:
         try:
             return self.Error(self.code).name
         except ValueError:
-            return 'ERR_UNKNOWN'
+            return "ERR_UNKNOWN"
 
     def __repr__(self) -> str:
-        return '<%s(%d)>' % (
-            self.__class__.__name__,
-            self.code
-        )
+        return "<%s(%d)>" % (self.__class__.__name__, self.code)
 
     def __str__(self) -> str:
-        return 'LittleFSError %d: %s' % (self.code, self.name)
+        return "LittleFSError %d: %s" % (self.code, self.name)
```

### Comparing `littlefs-python-0.9.1/src/littlefs/lfs.c` & `littlefs-python-0.9.3/src/littlefs/lfs.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.6 */
+/* Generated by Cython 3.0.8 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "LFS_NO_DEBUG",
@@ -66,18 +66,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_6" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030006F0
+#define CYTHON_HEX_VERSION 0x030008F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -611,22 +611,22 @@
     static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *exception_table = NULL;
         PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
         #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
-        PyObject *version_info; // borrowed
+        PyObject *version_info;
         PyObject *py_minor_version = NULL;
         #endif
         long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
-        minor_version = 11; // we don't yet need to distinguish between versions > 11
+        minor_version = 11;
         #else
         if (!(version_info = PySys_GetObject("version_info"))) goto end;
         if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
         minor_version = PyLong_AsLong(py_minor_version);
         Py_DECREF(py_minor_version);
         if (minor_version == -1 && PyErr_Occurred()) goto end;
         #endif
@@ -676,15 +676,15 @@
     #endif
 #elif PY_VERSION_HEX >= 0x030B0000
   static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
     PyCodeObject *result;
-    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);  // we don't have access to __pyx_empty_bytes here
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);
     if (!empty_bytes) return NULL;
     result =
       #if PY_VERSION_HEX >= 0x030C0000
         PyUnstable_Code_NewWithPosOnlyArgs
       #else
         PyCode_NewWithPosOnlyArgs
       #endif
@@ -1377,15 +1377,15 @@
     #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
-  #else  // Py < 3.12
+  #else
   #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
   #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
   #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
   #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
   #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
@@ -1656,68 +1656,68 @@
 struct __pyx_obj_8littlefs_3lfs_LFSDirectory;
 struct __pyx_obj_8littlefs_3lfs___pyx_scope_struct__genexpr;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "littlefs/lfs.pyx":78
+/* "littlefs/lfs.pyx":81
  * 
  * 
  * cdef class LFSConfig:             # <<<<<<<<<<<<<<
  * 
  *     cdef lfs_config _impl
  */
 struct __pyx_obj_8littlefs_3lfs_LFSConfig {
   PyObject_HEAD
   struct lfs_config _impl;
   PyObject *__dict__;
 };
 
 
-/* "littlefs/lfs.pyx":242
+/* "littlefs/lfs.pyx":245
  * 
  * 
  * cdef class LFSFilesystem:             # <<<<<<<<<<<<<<
  *     cdef lfs_t _impl
  * 
  */
 struct __pyx_obj_8littlefs_3lfs_LFSFilesystem {
   PyObject_HEAD
   lfs_t _impl;
 };
 
 
-/* "littlefs/lfs.pyx":250
+/* "littlefs/lfs.pyx":253
  * 
  * 
  * cdef class LFSFile:             # <<<<<<<<<<<<<<
  *     cdef lfs_file_t _impl
  * 
  */
 struct __pyx_obj_8littlefs_3lfs_LFSFile {
   PyObject_HEAD
   lfs_file_t _impl;
 };
 
 
-/* "littlefs/lfs.pyx":259
+/* "littlefs/lfs.pyx":262
  * 
  * 
  * cdef class LFSDirectory:             # <<<<<<<<<<<<<<
  *     cdef lfs_dir_t _impl
  * 
  */
 struct __pyx_obj_8littlefs_3lfs_LFSDirectory {
   PyObject_HEAD
   lfs_dir_t _impl;
 };
 
 
-/* "littlefs/lfs.pyx":390
+/* "littlefs/lfs.pyx":393
  *         exclusive_modes = (creating, reading, writing, appending)
  * 
  *         if sum(int(m) for m in exclusive_modes) > 1:             # <<<<<<<<<<<<<<
  *             raise ValueError(
  *                 "must have exactly one of create/read/write/append mode"
  */
 struct __pyx_obj_8littlefs_3lfs___pyx_scope_struct__genexpr {
@@ -2023,16 +2023,16 @@
 #else
     #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
 #endif
 #if CYTHON_AVOID_BORROWED_REFS
     #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
     #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
 #else
-    #define __Pyx_Arg_NewRef_VARARGS(arg) arg // no-op
-    #define __Pyx_Arg_XDECREF_VARARGS(arg) // no-op - arg is borrowed
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg
+    #define __Pyx_Arg_XDECREF_VARARGS(arg)
 #endif
 #define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
 #define __Pyx_KwValues_VARARGS(args, nargs) NULL
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
@@ -2040,16 +2040,17 @@
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
     CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
   #else
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
   #endif
-    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
-    #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg  /* no-op, __Pyx_Arg_FASTCALL is direct and this needs
+                                                   to have the same reference counting */
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
     #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
     #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
@@ -2650,15 +2651,15 @@
     PyObject *func_code;
     PyObject *func_closure;
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_classobj;
 #endif
     void *defaults;
     int defaults_pyobjects;
-    size_t defaults_size;  // used by FusedFunction for copying defaults
+    size_t defaults_size;
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
@@ -2821,14 +2822,17 @@
 #define __pyx_get_slice_count_pointer(memview) (&memview->acquisition_count)
 #define __PYX_INC_MEMVIEW(slice, have_gil) __Pyx_INC_MEMVIEW(slice, have_gil, __LINE__)
 #define __PYX_XCLEAR_MEMVIEW(slice, have_gil) __Pyx_XCLEAR_MEMVIEW(slice, have_gil, __LINE__)
 static CYTHON_INLINE void __Pyx_INC_MEMVIEW(__Pyx_memviewslice *, int, int);
 static CYTHON_INLINE void __Pyx_XCLEAR_MEMVIEW(__Pyx_memviewslice *, int, int);
 
 /* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__lfs_type(enum lfs_type value);
+
+/* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__lfs_open_flags(enum lfs_open_flags value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint32_t(uint32_t value);
@@ -3080,14 +3084,15 @@
 static const char __pyx_k_cfg[] = "cfg";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_got[] = " (got ";
 static const char __pyx_k_int[] = "int";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
 static const char __pyx_k_off[] = "off";
+static const char __pyx_k_str[] = "str";
 static const char __pyx_k_sum[] = "sum";
 static const char __pyx_k_sys[] = "sys";
 static const char __pyx_k_typ[] = "typ";
 static const char __pyx_k_xff[] = "\000xff";
 static const char __pyx_k_args[] = "args";
 static const char __pyx_k_base[] = "base";
 static const char __pyx_k_code[] = "code";
@@ -3151,14 +3156,15 @@
 static const char __pyx_k_rdonly[] = "rdonly";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_remove[] = "remove";
 static const char __pyx_k_rename[] = "rename";
 static const char __pyx_k_return[] = "return";
 static const char __pyx_k_retval[] = "retval";
 static const char __pyx_k_struct[] = "struct";
+static const char __pyx_k_typing[] = "typing";
 static const char __pyx_k_unpack[] = "unpack";
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_whence[] = "whence";
 static const char __pyx_k_wronly[] = "wronly";
 static const char __pyx_k_IntFlag[] = "IntFlag";
 static const char __pyx_k_LFSFile[] = "LFSFile";
 static const char __pyx_k_LFSStat[] = "LFSStat";
@@ -3177,14 +3183,16 @@
 static const char __pyx_k_prepare[] = "__prepare__";
 static const char __pyx_k_reading[] = "reading";
 static const char __pyx_k_setattr[] = "setattr";
 static const char __pyx_k_unmount[] = "unmount";
 static const char __pyx_k_writing[] = "writing";
 static const char __pyx_k_Ellipsis[] = "Ellipsis";
 static const char __pyx_k_Sequence[] = "Sequence";
+static const char __pyx_k_TYPE_DIR[] = "TYPE_DIR";
+static const char __pyx_k_TYPE_REG[] = "TYPE_REG";
 static const char __pyx_k_attr_max[] = "attr_max";
 static const char __pyx_k_buf_view[] = "buf_view";
 static const char __pyx_k_creating[] = "creating";
 static const char __pyx_k_dir_open[] = "dir_open";
 static const char __pyx_k_dir_read[] = "dir_read";
 static const char __pyx_k_dir_tell[] = "dir_tell";
 static const char __pyx_k_file_max[] = "file_max";
@@ -3215,32 +3223,33 @@
 static const char __pyx_k_isenabled[] = "isenabled";
 static const char __pyx_k_metaclass[] = "__metaclass__";
 static const char __pyx_k_prog_size[] = "prog_size";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_read_size[] = "read_size";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_IndexError[] = "IndexError";
+static const char __pyx_k_NamedTuple[] = "NamedTuple";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_attr_max_2[] = "attr_max=";
 static const char __pyx_k_block_size[] = "block_size";
 static const char __pyx_k_cache_size[] = "cache_size";
 static const char __pyx_k_dir_rewind[] = "dir_rewind";
 static const char __pyx_k_file_close[] = "file_close";
 static const char __pyx_k_file_max_2[] = "file_max=";
 static const char __pyx_k_file_write[] = "file_write";
 static const char __pyx_k_name_max_2[] = "name_max=";
-static const char __pyx_k_namedtuple[] = "namedtuple";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_removeattr[] = "removeattr";
 static const char __pyx_k_LFSFileFlag[] = "LFSFileFlag";
 static const char __pyx_k_LFS_VERSION[] = "__LFS_VERSION__";
 static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_UserContext[] = "UserContext";
+static const char __pyx_k_annotations[] = "__annotations__";
 static const char __pyx_k_block_count[] = "block_count";
 static const char __pyx_k_collections[] = "collections";
 static const char __pyx_k_file_rewind[] = "file_rewind";
 static const char __pyx_k_mro_entries[] = "__mro_entries__";
 static const char __pyx_k_prog_size_2[] = "prog_size=";
 static const char __pyx_k_read_size_2[] = "read_size=";
 static const char __pyx_k_LFSDirectory[] = "LFSDirectory";
@@ -3303,23 +3312,23 @@
 static const char __pyx_k_Littlefs_file_mode_flags[] = "Littlefs file mode flags";
 static const char __pyx_k_file_open_locals_genexpr[] = "file_open.<locals>.genexpr";
 static const char __pyx_k_Dimension_d_is_not_direct[] = "Dimension %d is not direct";
 static const char __pyx_k_LFSConfig___reduce_cython[] = "LFSConfig.__reduce_cython__";
 static const char __pyx_k_LFSFile___setstate_cython[] = "LFSFile.__setstate_cython__";
 static const char __pyx_k_Minimal_block_size_is_128[] = "Minimal block size is 128";
 static const char __pyx_k_Index_out_of_bounds_axis_d[] = "Index out of bounds (axis %d)";
-static const char __pyx_k_Littlefs_filesystem_status[] = "Littlefs filesystem status\n";
+static const char __pyx_k_Littlefs_filesystem_status[] = "Littlefs filesystem status.";
 static const char __pyx_k_LFSConfig___setstate_cython[] = "LFSConfig.__setstate_cython__";
 static const char __pyx_k_Step_may_not_be_zero_axis_d[] = "Step may not be zero (axis %d)";
 static const char __pyx_k_itemsize_0_for_cython_array[] = "itemsize <= 0 for cython.array";
 static const char __pyx_k_LFSDirectory___reduce_cython[] = "LFSDirectory.__reduce_cython__";
 static const char __pyx_k_LFSFilesystem___reduce_cython[] = "LFSFilesystem.__reduce_cython__";
 static const char __pyx_k_unable_to_allocate_array_data[] = "unable to allocate array data.";
 static const char __pyx_k_LFSDirectory___setstate_cython[] = "LFSDirectory.__setstate_cython__";
-static const char __pyx_k_Littlefs_File_Directory_status[] = "Littlefs File / Directory status\n";
+static const char __pyx_k_Littlefs_File_Directory_status[] = "Littlefs File / Directory status.";
 static const char __pyx_k_strided_and_direct_or_indirect[] = "<strided and direct or indirect>";
 static const char __pyx_k_LFSFilesystem___setstate_cython[] = "LFSFilesystem.__setstate_cython__";
 static const char __pyx_k_Pickling_of_struct_members_such[] = "Pickling of struct members such as self._impl must be explicitly requested with @auto_pickle(True)";
 static const char __pyx_k_must_have_exactly_one_of_create[] = "must have exactly one of create/read/write/append mode";
 static const char __pyx_k_All_dimensions_preceding_dimensi[] = "All dimensions preceding dimension %d must be indexed and not sliced";
 static const char __pyx_k_Buffer_view_does_not_expose_stri[] = "Buffer view does not expose strides";
 static const char __pyx_k_Can_only_create_a_buffer_that_is[] = "Can only create a buffer that is contiguous in memory.";
@@ -3518,44 +3527,45 @@
   PyObject *__pyx_n_s_LFSConfig;
   PyObject *__pyx_n_s_LFSConfig___reduce_cython;
   PyObject *__pyx_n_s_LFSConfig___setstate_cython;
   PyObject *__pyx_n_s_LFSDirectory;
   PyObject *__pyx_n_s_LFSDirectory___reduce_cython;
   PyObject *__pyx_n_s_LFSDirectory___setstate_cython;
   PyObject *__pyx_n_s_LFSFSStat;
-  PyObject *__pyx_n_u_LFSFSStat;
   PyObject *__pyx_n_s_LFSFile;
   PyObject *__pyx_n_s_LFSFileFlag;
   PyObject *__pyx_n_s_LFSFile___reduce_cython;
   PyObject *__pyx_n_s_LFSFile___setstate_cython;
   PyObject *__pyx_n_s_LFSFilesystem;
   PyObject *__pyx_n_s_LFSFilesystem___reduce_cython;
   PyObject *__pyx_n_s_LFSFilesystem___setstate_cython;
   PyObject *__pyx_n_s_LFSStat;
-  PyObject *__pyx_n_u_LFSStat;
   PyObject *__pyx_n_s_LFS_DISK_VERSION;
   PyObject *__pyx_n_s_LFS_VERSION;
   PyObject *__pyx_n_s_LittleFSError;
-  PyObject *__pyx_kp_u_Littlefs_File_Directory_status;
+  PyObject *__pyx_kp_s_Littlefs_File_Directory_status;
   PyObject *__pyx_kp_s_Littlefs_file_mode_flags;
-  PyObject *__pyx_kp_u_Littlefs_filesystem_status;
+  PyObject *__pyx_kp_s_Littlefs_filesystem_status;
   PyObject *__pyx_n_s_MemoryError;
   PyObject *__pyx_kp_s_MemoryView_of_r_at_0x_x;
   PyObject *__pyx_kp_s_MemoryView_of_r_object;
   PyObject *__pyx_kp_u_Minimal_block_size_is_128;
+  PyObject *__pyx_n_s_NamedTuple;
   PyObject *__pyx_n_s_NotImplementedError;
   PyObject *__pyx_kp_u_Not_all_data_written;
   PyObject *__pyx_n_b_O;
   PyObject *__pyx_kp_u_Out_of_bounds_on_buffer_access_a;
   PyObject *__pyx_n_s_PickleError;
   PyObject *__pyx_kp_s_Pickling_of_struct_members_such;
   PyObject *__pyx_n_s_RuntimeError;
   PyObject *__pyx_n_s_Sequence;
   PyObject *__pyx_kp_u_Size_must_be_0;
   PyObject *__pyx_kp_s_Step_may_not_be_zero_axis_d;
+  PyObject *__pyx_n_s_TYPE_DIR;
+  PyObject *__pyx_n_s_TYPE_REG;
   PyObject *__pyx_n_s_TypeError;
   PyObject *__pyx_kp_s_Unable_to_convert_item_to_object;
   PyObject *__pyx_n_s_UserContext;
   PyObject *__pyx_n_s_ValueError;
   PyObject *__pyx_n_s_View_MemoryView;
   PyObject *__pyx_kp_u__2;
   PyObject *__pyx_kp_u__23;
@@ -3565,32 +3575,30 @@
   PyObject *__pyx_kp_u__6;
   PyObject *__pyx_kp_u__7;
   PyObject *__pyx_n_s__99;
   PyObject *__pyx_n_u_a;
   PyObject *__pyx_n_s_abc;
   PyObject *__pyx_n_s_allocate_buffer;
   PyObject *__pyx_kp_u_and;
+  PyObject *__pyx_n_s_annotations;
   PyObject *__pyx_n_s_append;
   PyObject *__pyx_n_s_appending;
   PyObject *__pyx_n_s_args;
   PyObject *__pyx_n_u_ascii;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_attr_max;
-  PyObject *__pyx_n_u_attr_max;
   PyObject *__pyx_kp_u_attr_max_2;
   PyObject *__pyx_n_s_attr_size;
   PyObject *__pyx_n_u_b;
   PyObject *__pyx_n_s_base;
   PyObject *__pyx_n_s_block_count;
-  PyObject *__pyx_n_u_block_count;
   PyObject *__pyx_kp_u_block_count_2;
   PyObject *__pyx_n_s_block_cycles;
   PyObject *__pyx_kp_u_block_cycles_2;
   PyObject *__pyx_n_s_block_size;
-  PyObject *__pyx_n_u_block_size;
   PyObject *__pyx_kp_u_block_size_2;
   PyObject *__pyx_n_s_buf;
   PyObject *__pyx_n_s_buf_view;
   PyObject *__pyx_n_s_buffer;
   PyObject *__pyx_n_s_c;
   PyObject *__pyx_n_u_c;
   PyObject *__pyx_n_s_cache_size;
@@ -3619,15 +3627,14 @@
   PyObject *__pyx_n_s_dir_close;
   PyObject *__pyx_n_s_dir_open;
   PyObject *__pyx_n_s_dir_read;
   PyObject *__pyx_n_s_dir_rewind;
   PyObject *__pyx_n_s_dir_tell;
   PyObject *__pyx_kp_u_disable;
   PyObject *__pyx_n_s_disk_version;
-  PyObject *__pyx_n_u_disk_version;
   PyObject *__pyx_kp_u_disk_version_2;
   PyObject *__pyx_n_s_doc;
   PyObject *__pyx_n_s_dtype_is_object;
   PyObject *__pyx_kp_u_enable;
   PyObject *__pyx_n_s_encode;
   PyObject *__pyx_n_s_enum;
   PyObject *__pyx_n_s_enumerate;
@@ -3635,15 +3642,14 @@
   PyObject *__pyx_n_s_error;
   PyObject *__pyx_n_s_errors;
   PyObject *__pyx_n_s_excl;
   PyObject *__pyx_n_s_exclusive_modes;
   PyObject *__pyx_n_s_fh;
   PyObject *__pyx_n_s_file_close;
   PyObject *__pyx_n_s_file_max;
-  PyObject *__pyx_n_u_file_max;
   PyObject *__pyx_kp_u_file_max_2;
   PyObject *__pyx_n_s_file_open;
   PyObject *__pyx_n_s_file_open_cfg;
   PyObject *__pyx_n_s_file_open_locals_genexpr;
   PyObject *__pyx_n_s_file_read;
   PyObject *__pyx_n_s_file_rewind;
   PyObject *__pyx_n_s_file_seek;
@@ -3694,21 +3700,18 @@
   PyObject *__pyx_n_s_mkdir;
   PyObject *__pyx_n_s_mode;
   PyObject *__pyx_n_s_module;
   PyObject *__pyx_n_s_mount;
   PyObject *__pyx_n_s_mro_entries;
   PyObject *__pyx_kp_u_must_have_exactly_one_of_create;
   PyObject *__pyx_n_s_name;
-  PyObject *__pyx_n_u_name;
   PyObject *__pyx_n_s_name_2;
   PyObject *__pyx_n_s_name_max;
-  PyObject *__pyx_n_u_name_max;
   PyObject *__pyx_kp_u_name_max_2;
   PyObject *__pyx_kp_u_name_max_must_be_1022;
-  PyObject *__pyx_n_s_namedtuple;
   PyObject *__pyx_n_s_ndim;
   PyObject *__pyx_n_s_new;
   PyObject *__pyx_n_s_newpath;
   PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
   PyObject *__pyx_n_s_obj;
   PyObject *__pyx_n_s_off;
   PyObject *__pyx_n_s_oldpath;
@@ -3750,36 +3753,37 @@
   PyObject *__pyx_n_s_send;
   PyObject *__pyx_n_s_set_name;
   PyObject *__pyx_n_s_setattr;
   PyObject *__pyx_n_s_setstate;
   PyObject *__pyx_n_s_setstate_cython;
   PyObject *__pyx_n_s_shape;
   PyObject *__pyx_n_s_size;
-  PyObject *__pyx_n_u_size;
   PyObject *__pyx_n_s_spec;
   PyObject *__pyx_kp_s_src_littlefs_lfs_pyx;
   PyObject *__pyx_n_s_start;
   PyObject *__pyx_n_s_stat;
   PyObject *__pyx_n_s_step;
   PyObject *__pyx_n_s_stop;
+  PyObject *__pyx_n_s_str;
   PyObject *__pyx_kp_s_strided_and_direct;
   PyObject *__pyx_kp_s_strided_and_direct_or_indirect;
   PyObject *__pyx_kp_s_strided_and_indirect;
   PyObject *__pyx_kp_s_stringsource;
   PyObject *__pyx_n_s_struct;
   PyObject *__pyx_n_s_sum;
   PyObject *__pyx_n_s_super;
   PyObject *__pyx_n_s_sync;
   PyObject *__pyx_n_s_sys;
   PyObject *__pyx_n_u_t;
   PyObject *__pyx_n_s_test;
   PyObject *__pyx_n_s_throw;
   PyObject *__pyx_n_s_trunc;
   PyObject *__pyx_n_s_typ;
-  PyObject *__pyx_n_u_type;
+  PyObject *__pyx_n_s_type;
+  PyObject *__pyx_n_s_typing;
   PyObject *__pyx_kp_s_unable_to_allocate_array_data;
   PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
   PyObject *__pyx_n_s_unmount;
   PyObject *__pyx_n_s_unpack;
   PyObject *__pyx_n_s_update;
   PyObject *__pyx_n_s_updating;
   PyObject *__pyx_n_s_user_context;
@@ -3976,44 +3980,45 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_LFSConfig);
   Py_CLEAR(clear_module_state->__pyx_n_s_LFSConfig___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_LFSConfig___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_LFSDirectory);
   Py_CLEAR(clear_module_state->__pyx_n_s_LFSDirectory___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_LFSDirectory___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_LFSFSStat);
-  Py_CLEAR(clear_module_state->__pyx_n_u_LFSFSStat);
   Py_CLEAR(clear_module_state->__pyx_n_s_LFSFile);
   Py_CLEAR(clear_module_state->__pyx_n_s_LFSFileFlag);
   Py_CLEAR(clear_module_state->__pyx_n_s_LFSFile___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_LFSFile___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_LFSFilesystem);
   Py_CLEAR(clear_module_state->__pyx_n_s_LFSFilesystem___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_LFSFilesystem___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_LFSStat);
-  Py_CLEAR(clear_module_state->__pyx_n_u_LFSStat);
   Py_CLEAR(clear_module_state->__pyx_n_s_LFS_DISK_VERSION);
   Py_CLEAR(clear_module_state->__pyx_n_s_LFS_VERSION);
   Py_CLEAR(clear_module_state->__pyx_n_s_LittleFSError);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_Littlefs_File_Directory_status);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_Littlefs_File_Directory_status);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Littlefs_file_mode_flags);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_Littlefs_filesystem_status);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_Littlefs_filesystem_status);
   Py_CLEAR(clear_module_state->__pyx_n_s_MemoryError);
   Py_CLEAR(clear_module_state->__pyx_kp_s_MemoryView_of_r_at_0x_x);
   Py_CLEAR(clear_module_state->__pyx_kp_s_MemoryView_of_r_object);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Minimal_block_size_is_128);
+  Py_CLEAR(clear_module_state->__pyx_n_s_NamedTuple);
   Py_CLEAR(clear_module_state->__pyx_n_s_NotImplementedError);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Not_all_data_written);
   Py_CLEAR(clear_module_state->__pyx_n_b_O);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Out_of_bounds_on_buffer_access_a);
   Py_CLEAR(clear_module_state->__pyx_n_s_PickleError);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Pickling_of_struct_members_such);
   Py_CLEAR(clear_module_state->__pyx_n_s_RuntimeError);
   Py_CLEAR(clear_module_state->__pyx_n_s_Sequence);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Size_must_be_0);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Step_may_not_be_zero_axis_d);
+  Py_CLEAR(clear_module_state->__pyx_n_s_TYPE_DIR);
+  Py_CLEAR(clear_module_state->__pyx_n_s_TYPE_REG);
   Py_CLEAR(clear_module_state->__pyx_n_s_TypeError);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Unable_to_convert_item_to_object);
   Py_CLEAR(clear_module_state->__pyx_n_s_UserContext);
   Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
   Py_CLEAR(clear_module_state->__pyx_n_s_View_MemoryView);
   Py_CLEAR(clear_module_state->__pyx_kp_u__2);
   Py_CLEAR(clear_module_state->__pyx_kp_u__23);
@@ -4023,32 +4028,30 @@
   Py_CLEAR(clear_module_state->__pyx_kp_u__6);
   Py_CLEAR(clear_module_state->__pyx_kp_u__7);
   Py_CLEAR(clear_module_state->__pyx_n_s__99);
   Py_CLEAR(clear_module_state->__pyx_n_u_a);
   Py_CLEAR(clear_module_state->__pyx_n_s_abc);
   Py_CLEAR(clear_module_state->__pyx_n_s_allocate_buffer);
   Py_CLEAR(clear_module_state->__pyx_kp_u_and);
+  Py_CLEAR(clear_module_state->__pyx_n_s_annotations);
   Py_CLEAR(clear_module_state->__pyx_n_s_append);
   Py_CLEAR(clear_module_state->__pyx_n_s_appending);
   Py_CLEAR(clear_module_state->__pyx_n_s_args);
   Py_CLEAR(clear_module_state->__pyx_n_u_ascii);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_attr_max);
-  Py_CLEAR(clear_module_state->__pyx_n_u_attr_max);
   Py_CLEAR(clear_module_state->__pyx_kp_u_attr_max_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_attr_size);
   Py_CLEAR(clear_module_state->__pyx_n_u_b);
   Py_CLEAR(clear_module_state->__pyx_n_s_base);
   Py_CLEAR(clear_module_state->__pyx_n_s_block_count);
-  Py_CLEAR(clear_module_state->__pyx_n_u_block_count);
   Py_CLEAR(clear_module_state->__pyx_kp_u_block_count_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_block_cycles);
   Py_CLEAR(clear_module_state->__pyx_kp_u_block_cycles_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_block_size);
-  Py_CLEAR(clear_module_state->__pyx_n_u_block_size);
   Py_CLEAR(clear_module_state->__pyx_kp_u_block_size_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_buf);
   Py_CLEAR(clear_module_state->__pyx_n_s_buf_view);
   Py_CLEAR(clear_module_state->__pyx_n_s_buffer);
   Py_CLEAR(clear_module_state->__pyx_n_s_c);
   Py_CLEAR(clear_module_state->__pyx_n_u_c);
   Py_CLEAR(clear_module_state->__pyx_n_s_cache_size);
@@ -4077,15 +4080,14 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_dir_close);
   Py_CLEAR(clear_module_state->__pyx_n_s_dir_open);
   Py_CLEAR(clear_module_state->__pyx_n_s_dir_read);
   Py_CLEAR(clear_module_state->__pyx_n_s_dir_rewind);
   Py_CLEAR(clear_module_state->__pyx_n_s_dir_tell);
   Py_CLEAR(clear_module_state->__pyx_kp_u_disable);
   Py_CLEAR(clear_module_state->__pyx_n_s_disk_version);
-  Py_CLEAR(clear_module_state->__pyx_n_u_disk_version);
   Py_CLEAR(clear_module_state->__pyx_kp_u_disk_version_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_doc);
   Py_CLEAR(clear_module_state->__pyx_n_s_dtype_is_object);
   Py_CLEAR(clear_module_state->__pyx_kp_u_enable);
   Py_CLEAR(clear_module_state->__pyx_n_s_encode);
   Py_CLEAR(clear_module_state->__pyx_n_s_enum);
   Py_CLEAR(clear_module_state->__pyx_n_s_enumerate);
@@ -4093,15 +4095,14 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_error);
   Py_CLEAR(clear_module_state->__pyx_n_s_errors);
   Py_CLEAR(clear_module_state->__pyx_n_s_excl);
   Py_CLEAR(clear_module_state->__pyx_n_s_exclusive_modes);
   Py_CLEAR(clear_module_state->__pyx_n_s_fh);
   Py_CLEAR(clear_module_state->__pyx_n_s_file_close);
   Py_CLEAR(clear_module_state->__pyx_n_s_file_max);
-  Py_CLEAR(clear_module_state->__pyx_n_u_file_max);
   Py_CLEAR(clear_module_state->__pyx_kp_u_file_max_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_file_open);
   Py_CLEAR(clear_module_state->__pyx_n_s_file_open_cfg);
   Py_CLEAR(clear_module_state->__pyx_n_s_file_open_locals_genexpr);
   Py_CLEAR(clear_module_state->__pyx_n_s_file_read);
   Py_CLEAR(clear_module_state->__pyx_n_s_file_rewind);
   Py_CLEAR(clear_module_state->__pyx_n_s_file_seek);
@@ -4152,21 +4153,18 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_mkdir);
   Py_CLEAR(clear_module_state->__pyx_n_s_mode);
   Py_CLEAR(clear_module_state->__pyx_n_s_module);
   Py_CLEAR(clear_module_state->__pyx_n_s_mount);
   Py_CLEAR(clear_module_state->__pyx_n_s_mro_entries);
   Py_CLEAR(clear_module_state->__pyx_kp_u_must_have_exactly_one_of_create);
   Py_CLEAR(clear_module_state->__pyx_n_s_name);
-  Py_CLEAR(clear_module_state->__pyx_n_u_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_name_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_name_max);
-  Py_CLEAR(clear_module_state->__pyx_n_u_name_max);
   Py_CLEAR(clear_module_state->__pyx_kp_u_name_max_2);
   Py_CLEAR(clear_module_state->__pyx_kp_u_name_max_must_be_1022);
-  Py_CLEAR(clear_module_state->__pyx_n_s_namedtuple);
   Py_CLEAR(clear_module_state->__pyx_n_s_ndim);
   Py_CLEAR(clear_module_state->__pyx_n_s_new);
   Py_CLEAR(clear_module_state->__pyx_n_s_newpath);
   Py_CLEAR(clear_module_state->__pyx_kp_s_no_default___reduce___due_to_non);
   Py_CLEAR(clear_module_state->__pyx_n_s_obj);
   Py_CLEAR(clear_module_state->__pyx_n_s_off);
   Py_CLEAR(clear_module_state->__pyx_n_s_oldpath);
@@ -4208,36 +4206,37 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_send);
   Py_CLEAR(clear_module_state->__pyx_n_s_set_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_setattr);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_shape);
   Py_CLEAR(clear_module_state->__pyx_n_s_size);
-  Py_CLEAR(clear_module_state->__pyx_n_u_size);
   Py_CLEAR(clear_module_state->__pyx_n_s_spec);
   Py_CLEAR(clear_module_state->__pyx_kp_s_src_littlefs_lfs_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_start);
   Py_CLEAR(clear_module_state->__pyx_n_s_stat);
   Py_CLEAR(clear_module_state->__pyx_n_s_step);
   Py_CLEAR(clear_module_state->__pyx_n_s_stop);
+  Py_CLEAR(clear_module_state->__pyx_n_s_str);
   Py_CLEAR(clear_module_state->__pyx_kp_s_strided_and_direct);
   Py_CLEAR(clear_module_state->__pyx_kp_s_strided_and_direct_or_indirect);
   Py_CLEAR(clear_module_state->__pyx_kp_s_strided_and_indirect);
   Py_CLEAR(clear_module_state->__pyx_kp_s_stringsource);
   Py_CLEAR(clear_module_state->__pyx_n_s_struct);
   Py_CLEAR(clear_module_state->__pyx_n_s_sum);
   Py_CLEAR(clear_module_state->__pyx_n_s_super);
   Py_CLEAR(clear_module_state->__pyx_n_s_sync);
   Py_CLEAR(clear_module_state->__pyx_n_s_sys);
   Py_CLEAR(clear_module_state->__pyx_n_u_t);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
   Py_CLEAR(clear_module_state->__pyx_n_s_throw);
   Py_CLEAR(clear_module_state->__pyx_n_s_trunc);
   Py_CLEAR(clear_module_state->__pyx_n_s_typ);
-  Py_CLEAR(clear_module_state->__pyx_n_u_type);
+  Py_CLEAR(clear_module_state->__pyx_n_s_type);
+  Py_CLEAR(clear_module_state->__pyx_n_s_typing);
   Py_CLEAR(clear_module_state->__pyx_kp_s_unable_to_allocate_array_data);
   Py_CLEAR(clear_module_state->__pyx_kp_s_unable_to_allocate_shape_and_str);
   Py_CLEAR(clear_module_state->__pyx_n_s_unmount);
   Py_CLEAR(clear_module_state->__pyx_n_s_unpack);
   Py_CLEAR(clear_module_state->__pyx_n_s_update);
   Py_CLEAR(clear_module_state->__pyx_n_s_updating);
   Py_CLEAR(clear_module_state->__pyx_n_s_user_context);
@@ -4412,44 +4411,45 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_LFSConfig);
   Py_VISIT(traverse_module_state->__pyx_n_s_LFSConfig___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_LFSConfig___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_LFSDirectory);
   Py_VISIT(traverse_module_state->__pyx_n_s_LFSDirectory___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_LFSDirectory___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_LFSFSStat);
-  Py_VISIT(traverse_module_state->__pyx_n_u_LFSFSStat);
   Py_VISIT(traverse_module_state->__pyx_n_s_LFSFile);
   Py_VISIT(traverse_module_state->__pyx_n_s_LFSFileFlag);
   Py_VISIT(traverse_module_state->__pyx_n_s_LFSFile___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_LFSFile___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_LFSFilesystem);
   Py_VISIT(traverse_module_state->__pyx_n_s_LFSFilesystem___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_LFSFilesystem___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_LFSStat);
-  Py_VISIT(traverse_module_state->__pyx_n_u_LFSStat);
   Py_VISIT(traverse_module_state->__pyx_n_s_LFS_DISK_VERSION);
   Py_VISIT(traverse_module_state->__pyx_n_s_LFS_VERSION);
   Py_VISIT(traverse_module_state->__pyx_n_s_LittleFSError);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_Littlefs_File_Directory_status);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_Littlefs_File_Directory_status);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Littlefs_file_mode_flags);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_Littlefs_filesystem_status);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_Littlefs_filesystem_status);
   Py_VISIT(traverse_module_state->__pyx_n_s_MemoryError);
   Py_VISIT(traverse_module_state->__pyx_kp_s_MemoryView_of_r_at_0x_x);
   Py_VISIT(traverse_module_state->__pyx_kp_s_MemoryView_of_r_object);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Minimal_block_size_is_128);
+  Py_VISIT(traverse_module_state->__pyx_n_s_NamedTuple);
   Py_VISIT(traverse_module_state->__pyx_n_s_NotImplementedError);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Not_all_data_written);
   Py_VISIT(traverse_module_state->__pyx_n_b_O);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Out_of_bounds_on_buffer_access_a);
   Py_VISIT(traverse_module_state->__pyx_n_s_PickleError);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Pickling_of_struct_members_such);
   Py_VISIT(traverse_module_state->__pyx_n_s_RuntimeError);
   Py_VISIT(traverse_module_state->__pyx_n_s_Sequence);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Size_must_be_0);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Step_may_not_be_zero_axis_d);
+  Py_VISIT(traverse_module_state->__pyx_n_s_TYPE_DIR);
+  Py_VISIT(traverse_module_state->__pyx_n_s_TYPE_REG);
   Py_VISIT(traverse_module_state->__pyx_n_s_TypeError);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Unable_to_convert_item_to_object);
   Py_VISIT(traverse_module_state->__pyx_n_s_UserContext);
   Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
   Py_VISIT(traverse_module_state->__pyx_n_s_View_MemoryView);
   Py_VISIT(traverse_module_state->__pyx_kp_u__2);
   Py_VISIT(traverse_module_state->__pyx_kp_u__23);
@@ -4459,32 +4459,30 @@
   Py_VISIT(traverse_module_state->__pyx_kp_u__6);
   Py_VISIT(traverse_module_state->__pyx_kp_u__7);
   Py_VISIT(traverse_module_state->__pyx_n_s__99);
   Py_VISIT(traverse_module_state->__pyx_n_u_a);
   Py_VISIT(traverse_module_state->__pyx_n_s_abc);
   Py_VISIT(traverse_module_state->__pyx_n_s_allocate_buffer);
   Py_VISIT(traverse_module_state->__pyx_kp_u_and);
+  Py_VISIT(traverse_module_state->__pyx_n_s_annotations);
   Py_VISIT(traverse_module_state->__pyx_n_s_append);
   Py_VISIT(traverse_module_state->__pyx_n_s_appending);
   Py_VISIT(traverse_module_state->__pyx_n_s_args);
   Py_VISIT(traverse_module_state->__pyx_n_u_ascii);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_attr_max);
-  Py_VISIT(traverse_module_state->__pyx_n_u_attr_max);
   Py_VISIT(traverse_module_state->__pyx_kp_u_attr_max_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_attr_size);
   Py_VISIT(traverse_module_state->__pyx_n_u_b);
   Py_VISIT(traverse_module_state->__pyx_n_s_base);
   Py_VISIT(traverse_module_state->__pyx_n_s_block_count);
-  Py_VISIT(traverse_module_state->__pyx_n_u_block_count);
   Py_VISIT(traverse_module_state->__pyx_kp_u_block_count_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_block_cycles);
   Py_VISIT(traverse_module_state->__pyx_kp_u_block_cycles_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_block_size);
-  Py_VISIT(traverse_module_state->__pyx_n_u_block_size);
   Py_VISIT(traverse_module_state->__pyx_kp_u_block_size_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_buf);
   Py_VISIT(traverse_module_state->__pyx_n_s_buf_view);
   Py_VISIT(traverse_module_state->__pyx_n_s_buffer);
   Py_VISIT(traverse_module_state->__pyx_n_s_c);
   Py_VISIT(traverse_module_state->__pyx_n_u_c);
   Py_VISIT(traverse_module_state->__pyx_n_s_cache_size);
@@ -4513,15 +4511,14 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_dir_close);
   Py_VISIT(traverse_module_state->__pyx_n_s_dir_open);
   Py_VISIT(traverse_module_state->__pyx_n_s_dir_read);
   Py_VISIT(traverse_module_state->__pyx_n_s_dir_rewind);
   Py_VISIT(traverse_module_state->__pyx_n_s_dir_tell);
   Py_VISIT(traverse_module_state->__pyx_kp_u_disable);
   Py_VISIT(traverse_module_state->__pyx_n_s_disk_version);
-  Py_VISIT(traverse_module_state->__pyx_n_u_disk_version);
   Py_VISIT(traverse_module_state->__pyx_kp_u_disk_version_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_doc);
   Py_VISIT(traverse_module_state->__pyx_n_s_dtype_is_object);
   Py_VISIT(traverse_module_state->__pyx_kp_u_enable);
   Py_VISIT(traverse_module_state->__pyx_n_s_encode);
   Py_VISIT(traverse_module_state->__pyx_n_s_enum);
   Py_VISIT(traverse_module_state->__pyx_n_s_enumerate);
@@ -4529,15 +4526,14 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_error);
   Py_VISIT(traverse_module_state->__pyx_n_s_errors);
   Py_VISIT(traverse_module_state->__pyx_n_s_excl);
   Py_VISIT(traverse_module_state->__pyx_n_s_exclusive_modes);
   Py_VISIT(traverse_module_state->__pyx_n_s_fh);
   Py_VISIT(traverse_module_state->__pyx_n_s_file_close);
   Py_VISIT(traverse_module_state->__pyx_n_s_file_max);
-  Py_VISIT(traverse_module_state->__pyx_n_u_file_max);
   Py_VISIT(traverse_module_state->__pyx_kp_u_file_max_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_file_open);
   Py_VISIT(traverse_module_state->__pyx_n_s_file_open_cfg);
   Py_VISIT(traverse_module_state->__pyx_n_s_file_open_locals_genexpr);
   Py_VISIT(traverse_module_state->__pyx_n_s_file_read);
   Py_VISIT(traverse_module_state->__pyx_n_s_file_rewind);
   Py_VISIT(traverse_module_state->__pyx_n_s_file_seek);
@@ -4588,21 +4584,18 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_mkdir);
   Py_VISIT(traverse_module_state->__pyx_n_s_mode);
   Py_VISIT(traverse_module_state->__pyx_n_s_module);
   Py_VISIT(traverse_module_state->__pyx_n_s_mount);
   Py_VISIT(traverse_module_state->__pyx_n_s_mro_entries);
   Py_VISIT(traverse_module_state->__pyx_kp_u_must_have_exactly_one_of_create);
   Py_VISIT(traverse_module_state->__pyx_n_s_name);
-  Py_VISIT(traverse_module_state->__pyx_n_u_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_name_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_name_max);
-  Py_VISIT(traverse_module_state->__pyx_n_u_name_max);
   Py_VISIT(traverse_module_state->__pyx_kp_u_name_max_2);
   Py_VISIT(traverse_module_state->__pyx_kp_u_name_max_must_be_1022);
-  Py_VISIT(traverse_module_state->__pyx_n_s_namedtuple);
   Py_VISIT(traverse_module_state->__pyx_n_s_ndim);
   Py_VISIT(traverse_module_state->__pyx_n_s_new);
   Py_VISIT(traverse_module_state->__pyx_n_s_newpath);
   Py_VISIT(traverse_module_state->__pyx_kp_s_no_default___reduce___due_to_non);
   Py_VISIT(traverse_module_state->__pyx_n_s_obj);
   Py_VISIT(traverse_module_state->__pyx_n_s_off);
   Py_VISIT(traverse_module_state->__pyx_n_s_oldpath);
@@ -4644,36 +4637,37 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_send);
   Py_VISIT(traverse_module_state->__pyx_n_s_set_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_setattr);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_shape);
   Py_VISIT(traverse_module_state->__pyx_n_s_size);
-  Py_VISIT(traverse_module_state->__pyx_n_u_size);
   Py_VISIT(traverse_module_state->__pyx_n_s_spec);
   Py_VISIT(traverse_module_state->__pyx_kp_s_src_littlefs_lfs_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_start);
   Py_VISIT(traverse_module_state->__pyx_n_s_stat);
   Py_VISIT(traverse_module_state->__pyx_n_s_step);
   Py_VISIT(traverse_module_state->__pyx_n_s_stop);
+  Py_VISIT(traverse_module_state->__pyx_n_s_str);
   Py_VISIT(traverse_module_state->__pyx_kp_s_strided_and_direct);
   Py_VISIT(traverse_module_state->__pyx_kp_s_strided_and_direct_or_indirect);
   Py_VISIT(traverse_module_state->__pyx_kp_s_strided_and_indirect);
   Py_VISIT(traverse_module_state->__pyx_kp_s_stringsource);
   Py_VISIT(traverse_module_state->__pyx_n_s_struct);
   Py_VISIT(traverse_module_state->__pyx_n_s_sum);
   Py_VISIT(traverse_module_state->__pyx_n_s_super);
   Py_VISIT(traverse_module_state->__pyx_n_s_sync);
   Py_VISIT(traverse_module_state->__pyx_n_s_sys);
   Py_VISIT(traverse_module_state->__pyx_n_u_t);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
   Py_VISIT(traverse_module_state->__pyx_n_s_throw);
   Py_VISIT(traverse_module_state->__pyx_n_s_trunc);
   Py_VISIT(traverse_module_state->__pyx_n_s_typ);
-  Py_VISIT(traverse_module_state->__pyx_n_u_type);
+  Py_VISIT(traverse_module_state->__pyx_n_s_type);
+  Py_VISIT(traverse_module_state->__pyx_n_s_typing);
   Py_VISIT(traverse_module_state->__pyx_kp_s_unable_to_allocate_array_data);
   Py_VISIT(traverse_module_state->__pyx_kp_s_unable_to_allocate_shape_and_str);
   Py_VISIT(traverse_module_state->__pyx_n_s_unmount);
   Py_VISIT(traverse_module_state->__pyx_n_s_unpack);
   Py_VISIT(traverse_module_state->__pyx_n_s_update);
   Py_VISIT(traverse_module_state->__pyx_n_s_updating);
   Py_VISIT(traverse_module_state->__pyx_n_s_user_context);
@@ -4864,44 +4858,45 @@
 #define __pyx_n_s_LFSConfig __pyx_mstate_global->__pyx_n_s_LFSConfig
 #define __pyx_n_s_LFSConfig___reduce_cython __pyx_mstate_global->__pyx_n_s_LFSConfig___reduce_cython
 #define __pyx_n_s_LFSConfig___setstate_cython __pyx_mstate_global->__pyx_n_s_LFSConfig___setstate_cython
 #define __pyx_n_s_LFSDirectory __pyx_mstate_global->__pyx_n_s_LFSDirectory
 #define __pyx_n_s_LFSDirectory___reduce_cython __pyx_mstate_global->__pyx_n_s_LFSDirectory___reduce_cython
 #define __pyx_n_s_LFSDirectory___setstate_cython __pyx_mstate_global->__pyx_n_s_LFSDirectory___setstate_cython
 #define __pyx_n_s_LFSFSStat __pyx_mstate_global->__pyx_n_s_LFSFSStat
-#define __pyx_n_u_LFSFSStat __pyx_mstate_global->__pyx_n_u_LFSFSStat
 #define __pyx_n_s_LFSFile __pyx_mstate_global->__pyx_n_s_LFSFile
 #define __pyx_n_s_LFSFileFlag __pyx_mstate_global->__pyx_n_s_LFSFileFlag
 #define __pyx_n_s_LFSFile___reduce_cython __pyx_mstate_global->__pyx_n_s_LFSFile___reduce_cython
 #define __pyx_n_s_LFSFile___setstate_cython __pyx_mstate_global->__pyx_n_s_LFSFile___setstate_cython
 #define __pyx_n_s_LFSFilesystem __pyx_mstate_global->__pyx_n_s_LFSFilesystem
 #define __pyx_n_s_LFSFilesystem___reduce_cython __pyx_mstate_global->__pyx_n_s_LFSFilesystem___reduce_cython
 #define __pyx_n_s_LFSFilesystem___setstate_cython __pyx_mstate_global->__pyx_n_s_LFSFilesystem___setstate_cython
 #define __pyx_n_s_LFSStat __pyx_mstate_global->__pyx_n_s_LFSStat
-#define __pyx_n_u_LFSStat __pyx_mstate_global->__pyx_n_u_LFSStat
 #define __pyx_n_s_LFS_DISK_VERSION __pyx_mstate_global->__pyx_n_s_LFS_DISK_VERSION
 #define __pyx_n_s_LFS_VERSION __pyx_mstate_global->__pyx_n_s_LFS_VERSION
 #define __pyx_n_s_LittleFSError __pyx_mstate_global->__pyx_n_s_LittleFSError
-#define __pyx_kp_u_Littlefs_File_Directory_status __pyx_mstate_global->__pyx_kp_u_Littlefs_File_Directory_status
+#define __pyx_kp_s_Littlefs_File_Directory_status __pyx_mstate_global->__pyx_kp_s_Littlefs_File_Directory_status
 #define __pyx_kp_s_Littlefs_file_mode_flags __pyx_mstate_global->__pyx_kp_s_Littlefs_file_mode_flags
-#define __pyx_kp_u_Littlefs_filesystem_status __pyx_mstate_global->__pyx_kp_u_Littlefs_filesystem_status
+#define __pyx_kp_s_Littlefs_filesystem_status __pyx_mstate_global->__pyx_kp_s_Littlefs_filesystem_status
 #define __pyx_n_s_MemoryError __pyx_mstate_global->__pyx_n_s_MemoryError
 #define __pyx_kp_s_MemoryView_of_r_at_0x_x __pyx_mstate_global->__pyx_kp_s_MemoryView_of_r_at_0x_x
 #define __pyx_kp_s_MemoryView_of_r_object __pyx_mstate_global->__pyx_kp_s_MemoryView_of_r_object
 #define __pyx_kp_u_Minimal_block_size_is_128 __pyx_mstate_global->__pyx_kp_u_Minimal_block_size_is_128
+#define __pyx_n_s_NamedTuple __pyx_mstate_global->__pyx_n_s_NamedTuple
 #define __pyx_n_s_NotImplementedError __pyx_mstate_global->__pyx_n_s_NotImplementedError
 #define __pyx_kp_u_Not_all_data_written __pyx_mstate_global->__pyx_kp_u_Not_all_data_written
 #define __pyx_n_b_O __pyx_mstate_global->__pyx_n_b_O
 #define __pyx_kp_u_Out_of_bounds_on_buffer_access_a __pyx_mstate_global->__pyx_kp_u_Out_of_bounds_on_buffer_access_a
 #define __pyx_n_s_PickleError __pyx_mstate_global->__pyx_n_s_PickleError
 #define __pyx_kp_s_Pickling_of_struct_members_such __pyx_mstate_global->__pyx_kp_s_Pickling_of_struct_members_such
 #define __pyx_n_s_RuntimeError __pyx_mstate_global->__pyx_n_s_RuntimeError
 #define __pyx_n_s_Sequence __pyx_mstate_global->__pyx_n_s_Sequence
 #define __pyx_kp_u_Size_must_be_0 __pyx_mstate_global->__pyx_kp_u_Size_must_be_0
 #define __pyx_kp_s_Step_may_not_be_zero_axis_d __pyx_mstate_global->__pyx_kp_s_Step_may_not_be_zero_axis_d
+#define __pyx_n_s_TYPE_DIR __pyx_mstate_global->__pyx_n_s_TYPE_DIR
+#define __pyx_n_s_TYPE_REG __pyx_mstate_global->__pyx_n_s_TYPE_REG
 #define __pyx_n_s_TypeError __pyx_mstate_global->__pyx_n_s_TypeError
 #define __pyx_kp_s_Unable_to_convert_item_to_object __pyx_mstate_global->__pyx_kp_s_Unable_to_convert_item_to_object
 #define __pyx_n_s_UserContext __pyx_mstate_global->__pyx_n_s_UserContext
 #define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
 #define __pyx_n_s_View_MemoryView __pyx_mstate_global->__pyx_n_s_View_MemoryView
 #define __pyx_kp_u__2 __pyx_mstate_global->__pyx_kp_u__2
 #define __pyx_kp_u__23 __pyx_mstate_global->__pyx_kp_u__23
@@ -4911,32 +4906,30 @@
 #define __pyx_kp_u__6 __pyx_mstate_global->__pyx_kp_u__6
 #define __pyx_kp_u__7 __pyx_mstate_global->__pyx_kp_u__7
 #define __pyx_n_s__99 __pyx_mstate_global->__pyx_n_s__99
 #define __pyx_n_u_a __pyx_mstate_global->__pyx_n_u_a
 #define __pyx_n_s_abc __pyx_mstate_global->__pyx_n_s_abc
 #define __pyx_n_s_allocate_buffer __pyx_mstate_global->__pyx_n_s_allocate_buffer
 #define __pyx_kp_u_and __pyx_mstate_global->__pyx_kp_u_and
+#define __pyx_n_s_annotations __pyx_mstate_global->__pyx_n_s_annotations
 #define __pyx_n_s_append __pyx_mstate_global->__pyx_n_s_append
 #define __pyx_n_s_appending __pyx_mstate_global->__pyx_n_s_appending
 #define __pyx_n_s_args __pyx_mstate_global->__pyx_n_s_args
 #define __pyx_n_u_ascii __pyx_mstate_global->__pyx_n_u_ascii
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_attr_max __pyx_mstate_global->__pyx_n_s_attr_max
-#define __pyx_n_u_attr_max __pyx_mstate_global->__pyx_n_u_attr_max
 #define __pyx_kp_u_attr_max_2 __pyx_mstate_global->__pyx_kp_u_attr_max_2
 #define __pyx_n_s_attr_size __pyx_mstate_global->__pyx_n_s_attr_size
 #define __pyx_n_u_b __pyx_mstate_global->__pyx_n_u_b
 #define __pyx_n_s_base __pyx_mstate_global->__pyx_n_s_base
 #define __pyx_n_s_block_count __pyx_mstate_global->__pyx_n_s_block_count
-#define __pyx_n_u_block_count __pyx_mstate_global->__pyx_n_u_block_count
 #define __pyx_kp_u_block_count_2 __pyx_mstate_global->__pyx_kp_u_block_count_2
 #define __pyx_n_s_block_cycles __pyx_mstate_global->__pyx_n_s_block_cycles
 #define __pyx_kp_u_block_cycles_2 __pyx_mstate_global->__pyx_kp_u_block_cycles_2
 #define __pyx_n_s_block_size __pyx_mstate_global->__pyx_n_s_block_size
-#define __pyx_n_u_block_size __pyx_mstate_global->__pyx_n_u_block_size
 #define __pyx_kp_u_block_size_2 __pyx_mstate_global->__pyx_kp_u_block_size_2
 #define __pyx_n_s_buf __pyx_mstate_global->__pyx_n_s_buf
 #define __pyx_n_s_buf_view __pyx_mstate_global->__pyx_n_s_buf_view
 #define __pyx_n_s_buffer __pyx_mstate_global->__pyx_n_s_buffer
 #define __pyx_n_s_c __pyx_mstate_global->__pyx_n_s_c
 #define __pyx_n_u_c __pyx_mstate_global->__pyx_n_u_c
 #define __pyx_n_s_cache_size __pyx_mstate_global->__pyx_n_s_cache_size
@@ -4965,15 +4958,14 @@
 #define __pyx_n_s_dir_close __pyx_mstate_global->__pyx_n_s_dir_close
 #define __pyx_n_s_dir_open __pyx_mstate_global->__pyx_n_s_dir_open
 #define __pyx_n_s_dir_read __pyx_mstate_global->__pyx_n_s_dir_read
 #define __pyx_n_s_dir_rewind __pyx_mstate_global->__pyx_n_s_dir_rewind
 #define __pyx_n_s_dir_tell __pyx_mstate_global->__pyx_n_s_dir_tell
 #define __pyx_kp_u_disable __pyx_mstate_global->__pyx_kp_u_disable
 #define __pyx_n_s_disk_version __pyx_mstate_global->__pyx_n_s_disk_version
-#define __pyx_n_u_disk_version __pyx_mstate_global->__pyx_n_u_disk_version
 #define __pyx_kp_u_disk_version_2 __pyx_mstate_global->__pyx_kp_u_disk_version_2
 #define __pyx_n_s_doc __pyx_mstate_global->__pyx_n_s_doc
 #define __pyx_n_s_dtype_is_object __pyx_mstate_global->__pyx_n_s_dtype_is_object
 #define __pyx_kp_u_enable __pyx_mstate_global->__pyx_kp_u_enable
 #define __pyx_n_s_encode __pyx_mstate_global->__pyx_n_s_encode
 #define __pyx_n_s_enum __pyx_mstate_global->__pyx_n_s_enum
 #define __pyx_n_s_enumerate __pyx_mstate_global->__pyx_n_s_enumerate
@@ -4981,15 +4973,14 @@
 #define __pyx_n_s_error __pyx_mstate_global->__pyx_n_s_error
 #define __pyx_n_s_errors __pyx_mstate_global->__pyx_n_s_errors
 #define __pyx_n_s_excl __pyx_mstate_global->__pyx_n_s_excl
 #define __pyx_n_s_exclusive_modes __pyx_mstate_global->__pyx_n_s_exclusive_modes
 #define __pyx_n_s_fh __pyx_mstate_global->__pyx_n_s_fh
 #define __pyx_n_s_file_close __pyx_mstate_global->__pyx_n_s_file_close
 #define __pyx_n_s_file_max __pyx_mstate_global->__pyx_n_s_file_max
-#define __pyx_n_u_file_max __pyx_mstate_global->__pyx_n_u_file_max
 #define __pyx_kp_u_file_max_2 __pyx_mstate_global->__pyx_kp_u_file_max_2
 #define __pyx_n_s_file_open __pyx_mstate_global->__pyx_n_s_file_open
 #define __pyx_n_s_file_open_cfg __pyx_mstate_global->__pyx_n_s_file_open_cfg
 #define __pyx_n_s_file_open_locals_genexpr __pyx_mstate_global->__pyx_n_s_file_open_locals_genexpr
 #define __pyx_n_s_file_read __pyx_mstate_global->__pyx_n_s_file_read
 #define __pyx_n_s_file_rewind __pyx_mstate_global->__pyx_n_s_file_rewind
 #define __pyx_n_s_file_seek __pyx_mstate_global->__pyx_n_s_file_seek
@@ -5040,21 +5031,18 @@
 #define __pyx_n_s_mkdir __pyx_mstate_global->__pyx_n_s_mkdir
 #define __pyx_n_s_mode __pyx_mstate_global->__pyx_n_s_mode
 #define __pyx_n_s_module __pyx_mstate_global->__pyx_n_s_module
 #define __pyx_n_s_mount __pyx_mstate_global->__pyx_n_s_mount
 #define __pyx_n_s_mro_entries __pyx_mstate_global->__pyx_n_s_mro_entries
 #define __pyx_kp_u_must_have_exactly_one_of_create __pyx_mstate_global->__pyx_kp_u_must_have_exactly_one_of_create
 #define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
-#define __pyx_n_u_name __pyx_mstate_global->__pyx_n_u_name
 #define __pyx_n_s_name_2 __pyx_mstate_global->__pyx_n_s_name_2
 #define __pyx_n_s_name_max __pyx_mstate_global->__pyx_n_s_name_max
-#define __pyx_n_u_name_max __pyx_mstate_global->__pyx_n_u_name_max
 #define __pyx_kp_u_name_max_2 __pyx_mstate_global->__pyx_kp_u_name_max_2
 #define __pyx_kp_u_name_max_must_be_1022 __pyx_mstate_global->__pyx_kp_u_name_max_must_be_1022
-#define __pyx_n_s_namedtuple __pyx_mstate_global->__pyx_n_s_namedtuple
 #define __pyx_n_s_ndim __pyx_mstate_global->__pyx_n_s_ndim
 #define __pyx_n_s_new __pyx_mstate_global->__pyx_n_s_new
 #define __pyx_n_s_newpath __pyx_mstate_global->__pyx_n_s_newpath
 #define __pyx_kp_s_no_default___reduce___due_to_non __pyx_mstate_global->__pyx_kp_s_no_default___reduce___due_to_non
 #define __pyx_n_s_obj __pyx_mstate_global->__pyx_n_s_obj
 #define __pyx_n_s_off __pyx_mstate_global->__pyx_n_s_off
 #define __pyx_n_s_oldpath __pyx_mstate_global->__pyx_n_s_oldpath
@@ -5096,36 +5084,37 @@
 #define __pyx_n_s_send __pyx_mstate_global->__pyx_n_s_send
 #define __pyx_n_s_set_name __pyx_mstate_global->__pyx_n_s_set_name
 #define __pyx_n_s_setattr __pyx_mstate_global->__pyx_n_s_setattr
 #define __pyx_n_s_setstate __pyx_mstate_global->__pyx_n_s_setstate
 #define __pyx_n_s_setstate_cython __pyx_mstate_global->__pyx_n_s_setstate_cython
 #define __pyx_n_s_shape __pyx_mstate_global->__pyx_n_s_shape
 #define __pyx_n_s_size __pyx_mstate_global->__pyx_n_s_size
-#define __pyx_n_u_size __pyx_mstate_global->__pyx_n_u_size
 #define __pyx_n_s_spec __pyx_mstate_global->__pyx_n_s_spec
 #define __pyx_kp_s_src_littlefs_lfs_pyx __pyx_mstate_global->__pyx_kp_s_src_littlefs_lfs_pyx
 #define __pyx_n_s_start __pyx_mstate_global->__pyx_n_s_start
 #define __pyx_n_s_stat __pyx_mstate_global->__pyx_n_s_stat
 #define __pyx_n_s_step __pyx_mstate_global->__pyx_n_s_step
 #define __pyx_n_s_stop __pyx_mstate_global->__pyx_n_s_stop
+#define __pyx_n_s_str __pyx_mstate_global->__pyx_n_s_str
 #define __pyx_kp_s_strided_and_direct __pyx_mstate_global->__pyx_kp_s_strided_and_direct
 #define __pyx_kp_s_strided_and_direct_or_indirect __pyx_mstate_global->__pyx_kp_s_strided_and_direct_or_indirect
 #define __pyx_kp_s_strided_and_indirect __pyx_mstate_global->__pyx_kp_s_strided_and_indirect
 #define __pyx_kp_s_stringsource __pyx_mstate_global->__pyx_kp_s_stringsource
 #define __pyx_n_s_struct __pyx_mstate_global->__pyx_n_s_struct
 #define __pyx_n_s_sum __pyx_mstate_global->__pyx_n_s_sum
 #define __pyx_n_s_super __pyx_mstate_global->__pyx_n_s_super
 #define __pyx_n_s_sync __pyx_mstate_global->__pyx_n_s_sync
 #define __pyx_n_s_sys __pyx_mstate_global->__pyx_n_s_sys
 #define __pyx_n_u_t __pyx_mstate_global->__pyx_n_u_t
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
 #define __pyx_n_s_throw __pyx_mstate_global->__pyx_n_s_throw
 #define __pyx_n_s_trunc __pyx_mstate_global->__pyx_n_s_trunc
 #define __pyx_n_s_typ __pyx_mstate_global->__pyx_n_s_typ
-#define __pyx_n_u_type __pyx_mstate_global->__pyx_n_u_type
+#define __pyx_n_s_type __pyx_mstate_global->__pyx_n_s_type
+#define __pyx_n_s_typing __pyx_mstate_global->__pyx_n_s_typing
 #define __pyx_kp_s_unable_to_allocate_array_data __pyx_mstate_global->__pyx_kp_s_unable_to_allocate_array_data
 #define __pyx_kp_s_unable_to_allocate_shape_and_str __pyx_mstate_global->__pyx_kp_s_unable_to_allocate_shape_and_str
 #define __pyx_n_s_unmount __pyx_mstate_global->__pyx_n_s_unmount
 #define __pyx_n_s_unpack __pyx_mstate_global->__pyx_n_s_unpack
 #define __pyx_n_s_update __pyx_mstate_global->__pyx_n_s_update
 #define __pyx_n_s_updating __pyx_mstate_global->__pyx_n_s_updating
 #define __pyx_n_s_user_context __pyx_mstate_global->__pyx_n_s_user_context
@@ -18862,15 +18851,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":48
+/* "littlefs/lfs.pyx":51
  * 
  * 
  * cdef int _lfs_read(const lfs_config *c, lfs_block_t block, lfs_off_t off, void * buffer, lfs_size_t size) noexcept:             # <<<<<<<<<<<<<<
  *     ctx = <object>c.context
  *     data = ctx.user_context.read(ctx, block, off, size)
  */
 
@@ -18888,43 +18877,43 @@
   int __pyx_t_7;
   char *__pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_lfs_read", 1);
 
-  /* "littlefs/lfs.pyx":49
+  /* "littlefs/lfs.pyx":52
  * 
  * cdef int _lfs_read(const lfs_config *c, lfs_block_t block, lfs_off_t off, void * buffer, lfs_size_t size) noexcept:
  *     ctx = <object>c.context             # <<<<<<<<<<<<<<
  *     data = ctx.user_context.read(ctx, block, off, size)
  *     memcpy(buffer, <char *>data, size)
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_c->context);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_ctx = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "littlefs/lfs.pyx":50
+  /* "littlefs/lfs.pyx":53
  * cdef int _lfs_read(const lfs_config *c, lfs_block_t block, lfs_off_t off, void * buffer, lfs_size_t size) noexcept:
  *     ctx = <object>c.context
  *     data = ctx.user_context.read(ctx, block, off, size)             # <<<<<<<<<<<<<<
  *     memcpy(buffer, <char *>data, size)
  *     return 0
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_ctx, __pyx_n_s_user_context); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_ctx, __pyx_n_s_user_context); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_read); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_read); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_uint32_t(__pyx_v_block); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_uint32_t(__pyx_v_block); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyInt_From_uint32_t(__pyx_v_off); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_uint32_t(__pyx_v_off); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyInt_From_uint32_t(__pyx_v_size); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_uint32_t(__pyx_v_size); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_6)) {
@@ -18939,42 +18928,42 @@
   {
     PyObject *__pyx_callargs[5] = {__pyx_t_6, __pyx_v_ctx, __pyx_t_2, __pyx_t_4, __pyx_t_5};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_7, 4+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_data = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "littlefs/lfs.pyx":51
+  /* "littlefs/lfs.pyx":54
  *     ctx = <object>c.context
  *     data = ctx.user_context.read(ctx, block, off, size)
  *     memcpy(buffer, <char *>data, size)             # <<<<<<<<<<<<<<
  *     return 0
  * 
  */
-  __pyx_t_8 = __Pyx_PyObject_AsWritableString(__pyx_v_data); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsWritableString(__pyx_v_data); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 54, __pyx_L1_error)
   (void)(memcpy(__pyx_v_buffer, ((char *)__pyx_t_8), __pyx_v_size));
 
-  /* "littlefs/lfs.pyx":52
+  /* "littlefs/lfs.pyx":55
  *     data = ctx.user_context.read(ctx, block, off, size)
  *     memcpy(buffer, <char *>data, size)
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":48
+  /* "littlefs/lfs.pyx":51
  * 
  * 
  * cdef int _lfs_read(const lfs_config *c, lfs_block_t block, lfs_off_t off, void * buffer, lfs_size_t size) noexcept:             # <<<<<<<<<<<<<<
  *     ctx = <object>c.context
  *     data = ctx.user_context.read(ctx, block, off, size)
  */
 
@@ -18991,15 +18980,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_ctx);
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":55
+/* "littlefs/lfs.pyx":58
  * 
  * 
  * cdef int _lfs_prog(const lfs_config *c, lfs_block_t block, lfs_off_t off, const void * buffer, lfs_size_t size) noexcept:             # <<<<<<<<<<<<<<
  *     ctx = <object>c.context
  *     data = (<char*>buffer)[:size]
  */
 
@@ -19015,53 +19004,53 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_lfs_prog", 1);
 
-  /* "littlefs/lfs.pyx":56
+  /* "littlefs/lfs.pyx":59
  * 
  * cdef int _lfs_prog(const lfs_config *c, lfs_block_t block, lfs_off_t off, const void * buffer, lfs_size_t size) noexcept:
  *     ctx = <object>c.context             # <<<<<<<<<<<<<<
  *     data = (<char*>buffer)[:size]
  *     return ctx.user_context.prog(ctx, block, off, data)
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_c->context);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_ctx = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "littlefs/lfs.pyx":57
+  /* "littlefs/lfs.pyx":60
  * cdef int _lfs_prog(const lfs_config *c, lfs_block_t block, lfs_off_t off, const void * buffer, lfs_size_t size) noexcept:
  *     ctx = <object>c.context
  *     data = (<char*>buffer)[:size]             # <<<<<<<<<<<<<<
  *     return ctx.user_context.prog(ctx, block, off, data)
  * 
  */
-  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(((char *)__pyx_v_buffer) + 0, __pyx_v_size - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(((char *)__pyx_v_buffer) + 0, __pyx_v_size - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_data = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "littlefs/lfs.pyx":58
+  /* "littlefs/lfs.pyx":61
  *     ctx = <object>c.context
  *     data = (<char*>buffer)[:size]
  *     return ctx.user_context.prog(ctx, block, off, data)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_ctx, __pyx_n_s_user_context); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_ctx, __pyx_n_s_user_context); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 61, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_prog); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_prog); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 61, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_uint32_t(__pyx_v_block); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_uint32_t(__pyx_v_block); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 61, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyInt_From_uint32_t(__pyx_v_off); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_uint32_t(__pyx_v_off); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 61, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
@@ -19075,24 +19064,24 @@
   #endif
   {
     PyObject *__pyx_callargs[5] = {__pyx_t_5, __pyx_v_ctx, __pyx_t_2, __pyx_t_4, __pyx_v_data};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 4+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 61, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_6;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":55
+  /* "littlefs/lfs.pyx":58
  * 
  * 
  * cdef int _lfs_prog(const lfs_config *c, lfs_block_t block, lfs_off_t off, const void * buffer, lfs_size_t size) noexcept:             # <<<<<<<<<<<<<<
  *     ctx = <object>c.context
  *     data = (<char*>buffer)[:size]
  */
 
@@ -19108,15 +19097,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_ctx);
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":61
+/* "littlefs/lfs.pyx":64
  * 
  * 
  * cdef int _lfs_erase(const lfs_config *c, lfs_block_t block) noexcept:             # <<<<<<<<<<<<<<
  *     ctx = <object>c.context
  *     return ctx.user_context.erase(ctx, block)
  */
 
@@ -19130,39 +19119,39 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_lfs_erase", 1);
 
-  /* "littlefs/lfs.pyx":62
+  /* "littlefs/lfs.pyx":65
  * 
  * cdef int _lfs_erase(const lfs_config *c, lfs_block_t block) noexcept:
  *     ctx = <object>c.context             # <<<<<<<<<<<<<<
  *     return ctx.user_context.erase(ctx, block)
  * 
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_c->context);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_ctx = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "littlefs/lfs.pyx":63
+  /* "littlefs/lfs.pyx":66
  * cdef int _lfs_erase(const lfs_config *c, lfs_block_t block) noexcept:
  *     ctx = <object>c.context
  *     return ctx.user_context.erase(ctx, block)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_ctx, __pyx_n_s_user_context); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_ctx, __pyx_n_s_user_context); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_erase); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_erase); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_uint32_t(__pyx_v_block); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_uint32_t(__pyx_v_block); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
@@ -19175,24 +19164,24 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_4, __pyx_v_ctx, __pyx_t_2};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_5;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":61
+  /* "littlefs/lfs.pyx":64
  * 
  * 
  * cdef int _lfs_erase(const lfs_config *c, lfs_block_t block) noexcept:             # <<<<<<<<<<<<<<
  *     ctx = <object>c.context
  *     return ctx.user_context.erase(ctx, block)
  */
 
@@ -19206,15 +19195,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_ctx);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":66
+/* "littlefs/lfs.pyx":69
  * 
  * 
  * cdef int _lfs_sync(const lfs_config *c) noexcept:             # <<<<<<<<<<<<<<
  *     ctx = <object>c.context
  *     return ctx.user_context.sync(ctx)
  */
 
@@ -19227,36 +19216,36 @@
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_lfs_sync", 1);
 
-  /* "littlefs/lfs.pyx":67
+  /* "littlefs/lfs.pyx":70
  * 
  * cdef int _lfs_sync(const lfs_config *c) noexcept:
  *     ctx = <object>c.context             # <<<<<<<<<<<<<<
  *     return ctx.user_context.sync(ctx)
  * 
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_c->context);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_ctx = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "littlefs/lfs.pyx":68
+  /* "littlefs/lfs.pyx":71
  * cdef int _lfs_sync(const lfs_config *c) noexcept:
  *     ctx = <object>c.context
  *     return ctx.user_context.sync(ctx)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_ctx, __pyx_n_s_user_context); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_ctx, __pyx_n_s_user_context); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_sync); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_sync); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -19269,24 +19258,24 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_ctx};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_4;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":66
+  /* "littlefs/lfs.pyx":69
  * 
  * 
  * cdef int _lfs_sync(const lfs_config *c) noexcept:             # <<<<<<<<<<<<<<
  *     ctx = <object>c.context
  *     return ctx.user_context.sync(ctx)
  */
 
@@ -19299,15 +19288,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_ctx);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":71
+/* "littlefs/lfs.pyx":74
  * 
  * 
  * cdef int _raise_on_error(int code) except -1:             # <<<<<<<<<<<<<<
  *     if code < 0:
  *         raise errors.LittleFSError(code)
  */
 
@@ -19321,37 +19310,37 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_raise_on_error", 1);
 
-  /* "littlefs/lfs.pyx":72
+  /* "littlefs/lfs.pyx":75
  * 
  * cdef int _raise_on_error(int code) except -1:
  *     if code < 0:             # <<<<<<<<<<<<<<
  *         raise errors.LittleFSError(code)
  *     return code
  */
   __pyx_t_1 = (__pyx_v_code < 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "littlefs/lfs.pyx":73
+    /* "littlefs/lfs.pyx":76
  * cdef int _raise_on_error(int code) except -1:
  *     if code < 0:
  *         raise errors.LittleFSError(code)             # <<<<<<<<<<<<<<
  *     return code
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_errors); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_errors); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_LittleFSError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 73, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_LittleFSError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 76, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = NULL;
     __pyx_t_6 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
@@ -19364,42 +19353,42 @@
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_3};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 76, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 73, __pyx_L1_error)
+    __PYX_ERR(0, 76, __pyx_L1_error)
 
-    /* "littlefs/lfs.pyx":72
+    /* "littlefs/lfs.pyx":75
  * 
  * cdef int _raise_on_error(int code) except -1:
  *     if code < 0:             # <<<<<<<<<<<<<<
  *         raise errors.LittleFSError(code)
  *     return code
  */
   }
 
-  /* "littlefs/lfs.pyx":74
+  /* "littlefs/lfs.pyx":77
  *     if code < 0:
  *         raise errors.LittleFSError(code)
  *     return code             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_code;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":71
+  /* "littlefs/lfs.pyx":74
  * 
  * 
  * cdef int _raise_on_error(int code) except -1:             # <<<<<<<<<<<<<<
  *     if code < 0:
  *         raise errors.LittleFSError(code)
  */
 
@@ -19412,15 +19401,15 @@
   __Pyx_AddTraceback("littlefs.lfs._raise_on_error", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":83
+/* "littlefs/lfs.pyx":86
  *     cdef dict __dict__
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self._impl.read = &_lfs_read
  *         self._impl.prog = &_lfs_prog
  */
 
@@ -19447,64 +19436,64 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static int __pyx_pf_8littlefs_3lfs_9LFSConfig___cinit__(struct __pyx_obj_8littlefs_3lfs_LFSConfig *__pyx_v_self) {
   int __pyx_r;
 
-  /* "littlefs/lfs.pyx":84
+  /* "littlefs/lfs.pyx":87
  * 
  *     def __cinit__(self):
  *         self._impl.read = &_lfs_read             # <<<<<<<<<<<<<<
  *         self._impl.prog = &_lfs_prog
  *         self._impl.erase = &_lfs_erase
  */
   __pyx_v_self->_impl.read = (&__pyx_f_8littlefs_3lfs__lfs_read);
 
-  /* "littlefs/lfs.pyx":85
+  /* "littlefs/lfs.pyx":88
  *     def __cinit__(self):
  *         self._impl.read = &_lfs_read
  *         self._impl.prog = &_lfs_prog             # <<<<<<<<<<<<<<
  *         self._impl.erase = &_lfs_erase
  *         self._impl.sync = &_lfs_sync
  */
   __pyx_v_self->_impl.prog = (&__pyx_f_8littlefs_3lfs__lfs_prog);
 
-  /* "littlefs/lfs.pyx":86
+  /* "littlefs/lfs.pyx":89
  *         self._impl.read = &_lfs_read
  *         self._impl.prog = &_lfs_prog
  *         self._impl.erase = &_lfs_erase             # <<<<<<<<<<<<<<
  *         self._impl.sync = &_lfs_sync
  * 
  */
   __pyx_v_self->_impl.erase = (&__pyx_f_8littlefs_3lfs__lfs_erase);
 
-  /* "littlefs/lfs.pyx":87
+  /* "littlefs/lfs.pyx":90
  *         self._impl.prog = &_lfs_prog
  *         self._impl.erase = &_lfs_erase
  *         self._impl.sync = &_lfs_sync             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_v_self->_impl.sync = (&__pyx_f_8littlefs_3lfs__lfs_sync);
 
-  /* "littlefs/lfs.pyx":83
+  /* "littlefs/lfs.pyx":86
  *     cdef dict __dict__
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self._impl.read = &_lfs_read
  *         self._impl.prog = &_lfs_prog
  */
 
   /* function exit code */
   __pyx_r = 0;
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":90
+/* "littlefs/lfs.pyx":93
  * 
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  context=None,
  *                  *,
  */
 
@@ -19542,15 +19531,15 @@
   #else
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return -1;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_context,&__pyx_n_s_block_size,&__pyx_n_s_block_count,&__pyx_n_s_read_size,&__pyx_n_s_prog_size,&__pyx_n_s_block_cycles,&__pyx_n_s_cache_size,&__pyx_n_s_lookahead_size,&__pyx_n_s_name_max,&__pyx_n_s_file_max,&__pyx_n_s_attr_max,&__pyx_n_s_metadata_max,&__pyx_n_s_disk_version,0};
 
-    /* "littlefs/lfs.pyx":91
+    /* "littlefs/lfs.pyx":94
  * 
  *     def __init__(self,
  *                  context=None,             # <<<<<<<<<<<<<<
  *                  *,
  *                  block_size: int = 128,
  */
     values[0] = __Pyx_Arg_NewRef_VARARGS(((PyObject *)Py_None));
@@ -19576,28 +19565,28 @@
       }
       kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_context);
           if (value) { values[0] = __Pyx_Arg_NewRef_VARARGS(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 90, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 93, __pyx_L3_error)
         }
       }
       if (kw_args > 0 && likely(kw_args <= 12)) {
         Py_ssize_t index;
         for (index = 1; index < 13 && kw_args > 0; index++) {
           PyObject* value = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, *__pyx_pyargnames[index]);
           if (value) { values[index] = __Pyx_Arg_NewRef_VARARGS(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 90, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 93, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 90, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 93, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
@@ -19615,43 +19604,43 @@
     __pyx_v_file_max = ((PyObject*)values[9]);
     __pyx_v_attr_max = ((PyObject*)values[10]);
     __pyx_v_metadata_max = ((PyObject*)values[11]);
     __pyx_v_disk_version = ((PyObject*)values[12]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 90, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 93, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.LFSConfig.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_block_size), (&PyInt_Type), 0, "block_size", 1))) __PYX_ERR(0, 93, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_block_count), (&PyInt_Type), 0, "block_count", 1))) __PYX_ERR(0, 94, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_read_size), (&PyInt_Type), 0, "read_size", 1))) __PYX_ERR(0, 95, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_prog_size), (&PyInt_Type), 0, "prog_size", 1))) __PYX_ERR(0, 96, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_block_cycles), (&PyInt_Type), 0, "block_cycles", 1))) __PYX_ERR(0, 97, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_cache_size), (&PyInt_Type), 0, "cache_size", 1))) __PYX_ERR(0, 98, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_lookahead_size), (&PyInt_Type), 0, "lookahead_size", 1))) __PYX_ERR(0, 99, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_name_max), (&PyInt_Type), 0, "name_max", 1))) __PYX_ERR(0, 100, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_file_max), (&PyInt_Type), 0, "file_max", 1))) __PYX_ERR(0, 101, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_attr_max), (&PyInt_Type), 0, "attr_max", 1))) __PYX_ERR(0, 102, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_metadata_max), (&PyInt_Type), 0, "metadata_max", 1))) __PYX_ERR(0, 103, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_disk_version), (&PyInt_Type), 0, "disk_version", 1))) __PYX_ERR(0, 104, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_block_size), (&PyInt_Type), 0, "block_size", 1))) __PYX_ERR(0, 96, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_block_count), (&PyInt_Type), 0, "block_count", 1))) __PYX_ERR(0, 97, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_read_size), (&PyInt_Type), 0, "read_size", 1))) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_prog_size), (&PyInt_Type), 0, "prog_size", 1))) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_block_cycles), (&PyInt_Type), 0, "block_cycles", 1))) __PYX_ERR(0, 100, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_cache_size), (&PyInt_Type), 0, "cache_size", 1))) __PYX_ERR(0, 101, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_lookahead_size), (&PyInt_Type), 0, "lookahead_size", 1))) __PYX_ERR(0, 102, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_name_max), (&PyInt_Type), 0, "name_max", 1))) __PYX_ERR(0, 103, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_file_max), (&PyInt_Type), 0, "file_max", 1))) __PYX_ERR(0, 104, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_attr_max), (&PyInt_Type), 0, "attr_max", 1))) __PYX_ERR(0, 105, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_metadata_max), (&PyInt_Type), 0, "metadata_max", 1))) __PYX_ERR(0, 106, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_disk_version), (&PyInt_Type), 0, "disk_version", 1))) __PYX_ERR(0, 107, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_9LFSConfig_2__init__(((struct __pyx_obj_8littlefs_3lfs_LFSConfig *)__pyx_v_self), __pyx_v_context, __pyx_v_block_size, __pyx_v_block_count, __pyx_v_read_size, __pyx_v_prog_size, __pyx_v_block_cycles, __pyx_v_cache_size, __pyx_v_lookahead_size, __pyx_v_name_max, __pyx_v_file_max, __pyx_v_attr_max, __pyx_v_metadata_max, __pyx_v_disk_version);
 
-  /* "littlefs/lfs.pyx":90
+  /* "littlefs/lfs.pyx":93
  * 
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  context=None,
  *                  *,
  */
 
@@ -19688,250 +19677,250 @@
   int __pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
   __Pyx_INCREF(__pyx_v_context);
 
-  /* "littlefs/lfs.pyx":152
+  /* "littlefs/lfs.pyx":155
  *         """
  * 
  *         if block_size < 128:             # <<<<<<<<<<<<<<
  *             raise ValueError('Minimal block size is 128')
  * 
  */
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_block_size, __pyx_int_128, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 152, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_block_size, __pyx_int_128, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_t_2)) {
 
-    /* "littlefs/lfs.pyx":153
+    /* "littlefs/lfs.pyx":156
  * 
  *         if block_size < 128:
  *             raise ValueError('Minimal block size is 128')             # <<<<<<<<<<<<<<
  * 
  *         if name_max > 1022:  # LittleFS maximum name length limitation
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 153, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 156, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 153, __pyx_L1_error)
+    __PYX_ERR(0, 156, __pyx_L1_error)
 
-    /* "littlefs/lfs.pyx":152
+    /* "littlefs/lfs.pyx":155
  *         """
  * 
  *         if block_size < 128:             # <<<<<<<<<<<<<<
  *             raise ValueError('Minimal block size is 128')
  * 
  */
   }
 
-  /* "littlefs/lfs.pyx":155
+  /* "littlefs/lfs.pyx":158
  *             raise ValueError('Minimal block size is 128')
  * 
  *         if name_max > 1022:  # LittleFS maximum name length limitation             # <<<<<<<<<<<<<<
  *             raise ValueError(f"name_max must be <=1022.")
  * 
  */
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_name_max, __pyx_int_1022, Py_GT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 155, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 155, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_name_max, __pyx_int_1022, Py_GT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 158, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 158, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_t_2)) {
 
-    /* "littlefs/lfs.pyx":156
+    /* "littlefs/lfs.pyx":159
  * 
  *         if name_max > 1022:  # LittleFS maximum name length limitation
  *             raise ValueError(f"name_max must be <=1022.")             # <<<<<<<<<<<<<<
  * 
  *         self._impl.read_size = read_size if read_size else block_size
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 156, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 159, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 156, __pyx_L1_error)
+    __PYX_ERR(0, 159, __pyx_L1_error)
 
-    /* "littlefs/lfs.pyx":155
+    /* "littlefs/lfs.pyx":158
  *             raise ValueError('Minimal block size is 128')
  * 
  *         if name_max > 1022:  # LittleFS maximum name length limitation             # <<<<<<<<<<<<<<
  *             raise ValueError(f"name_max must be <=1022.")
  * 
  */
   }
 
-  /* "littlefs/lfs.pyx":158
+  /* "littlefs/lfs.pyx":161
  *             raise ValueError(f"name_max must be <=1022.")
  * 
  *         self._impl.read_size = read_size if read_size else block_size             # <<<<<<<<<<<<<<
  *         self._impl.prog_size = prog_size if prog_size else block_size
  *         self._impl.block_size = block_size
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_read_size); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 158, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_read_size); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 161, __pyx_L1_error)
   if (__pyx_t_2) {
-    __pyx_t_4 = __Pyx_PyInt_As_uint32_t(__pyx_v_read_size); if (unlikely((__pyx_t_4 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 158, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_As_uint32_t(__pyx_v_read_size); if (unlikely((__pyx_t_4 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 161, __pyx_L1_error)
     __pyx_t_3 = __pyx_t_4;
   } else {
-    __pyx_t_4 = __Pyx_PyInt_As_uint32_t(__pyx_v_block_size); if (unlikely((__pyx_t_4 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 158, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_As_uint32_t(__pyx_v_block_size); if (unlikely((__pyx_t_4 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 161, __pyx_L1_error)
     __pyx_t_3 = __pyx_t_4;
   }
   __pyx_v_self->_impl.read_size = __pyx_t_3;
 
-  /* "littlefs/lfs.pyx":159
+  /* "littlefs/lfs.pyx":162
  * 
  *         self._impl.read_size = read_size if read_size else block_size
  *         self._impl.prog_size = prog_size if prog_size else block_size             # <<<<<<<<<<<<<<
  *         self._impl.block_size = block_size
  *         self._impl.block_count = block_count
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_prog_size); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 159, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_prog_size); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 162, __pyx_L1_error)
   if (__pyx_t_2) {
-    __pyx_t_4 = __Pyx_PyInt_As_uint32_t(__pyx_v_prog_size); if (unlikely((__pyx_t_4 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 159, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_As_uint32_t(__pyx_v_prog_size); if (unlikely((__pyx_t_4 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 162, __pyx_L1_error)
     __pyx_t_3 = __pyx_t_4;
   } else {
-    __pyx_t_4 = __Pyx_PyInt_As_uint32_t(__pyx_v_block_size); if (unlikely((__pyx_t_4 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 159, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_As_uint32_t(__pyx_v_block_size); if (unlikely((__pyx_t_4 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 162, __pyx_L1_error)
     __pyx_t_3 = __pyx_t_4;
   }
   __pyx_v_self->_impl.prog_size = __pyx_t_3;
 
-  /* "littlefs/lfs.pyx":160
+  /* "littlefs/lfs.pyx":163
  *         self._impl.read_size = read_size if read_size else block_size
  *         self._impl.prog_size = prog_size if prog_size else block_size
  *         self._impl.block_size = block_size             # <<<<<<<<<<<<<<
  *         self._impl.block_count = block_count
  *         self._impl.block_cycles = block_cycles
  */
-  __pyx_t_3 = __Pyx_PyInt_As_uint32_t(__pyx_v_block_size); if (unlikely((__pyx_t_3 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 160, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_uint32_t(__pyx_v_block_size); if (unlikely((__pyx_t_3 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 163, __pyx_L1_error)
   __pyx_v_self->_impl.block_size = __pyx_t_3;
 
-  /* "littlefs/lfs.pyx":161
+  /* "littlefs/lfs.pyx":164
  *         self._impl.prog_size = prog_size if prog_size else block_size
  *         self._impl.block_size = block_size
  *         self._impl.block_count = block_count             # <<<<<<<<<<<<<<
  *         self._impl.block_cycles = block_cycles
  *         # Cache size, at least as big as read / prog size
  */
-  __pyx_t_3 = __Pyx_PyInt_As_uint32_t(__pyx_v_block_count); if (unlikely((__pyx_t_3 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_uint32_t(__pyx_v_block_count); if (unlikely((__pyx_t_3 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 164, __pyx_L1_error)
   __pyx_v_self->_impl.block_count = __pyx_t_3;
 
-  /* "littlefs/lfs.pyx":162
+  /* "littlefs/lfs.pyx":165
  *         self._impl.block_size = block_size
  *         self._impl.block_count = block_count
  *         self._impl.block_cycles = block_cycles             # <<<<<<<<<<<<<<
  *         # Cache size, at least as big as read / prog size
  *         self._impl.cache_size = cache_size if cache_size else max(self._impl.read_size, self._impl.prog_size)
  */
-  __pyx_t_5 = __Pyx_PyInt_As_int32_t(__pyx_v_block_cycles); if (unlikely((__pyx_t_5 == ((int32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 162, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_int32_t(__pyx_v_block_cycles); if (unlikely((__pyx_t_5 == ((int32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 165, __pyx_L1_error)
   __pyx_v_self->_impl.block_cycles = __pyx_t_5;
 
-  /* "littlefs/lfs.pyx":164
+  /* "littlefs/lfs.pyx":167
  *         self._impl.block_cycles = block_cycles
  *         # Cache size, at least as big as read / prog size
  *         self._impl.cache_size = cache_size if cache_size else max(self._impl.read_size, self._impl.prog_size)             # <<<<<<<<<<<<<<
  *         # Lookahead buffer size in bytes
  *         self._impl.lookahead_size = lookahead_size
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_cache_size); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 164, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_cache_size); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 167, __pyx_L1_error)
   if (__pyx_t_2) {
-    __pyx_t_4 = __Pyx_PyInt_As_uint32_t(__pyx_v_cache_size); if (unlikely((__pyx_t_4 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 164, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_As_uint32_t(__pyx_v_cache_size); if (unlikely((__pyx_t_4 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 167, __pyx_L1_error)
     __pyx_t_3 = __pyx_t_4;
   } else {
     __pyx_t_4 = __pyx_v_self->_impl.prog_size;
     __pyx_t_6 = __pyx_v_self->_impl.read_size;
     __pyx_t_8 = (__pyx_t_4 > __pyx_t_6);
     if (__pyx_t_8) {
       __pyx_t_7 = __pyx_t_4;
     } else {
       __pyx_t_7 = __pyx_t_6;
     }
     __pyx_t_3 = __pyx_t_7;
   }
   __pyx_v_self->_impl.cache_size = __pyx_t_3;
 
-  /* "littlefs/lfs.pyx":166
+  /* "littlefs/lfs.pyx":169
  *         self._impl.cache_size = cache_size if cache_size else max(self._impl.read_size, self._impl.prog_size)
  *         # Lookahead buffer size in bytes
  *         self._impl.lookahead_size = lookahead_size             # <<<<<<<<<<<<<<
  *         self._impl.name_max = name_max
  *         self._impl.file_max = file_max
  */
-  __pyx_t_3 = __Pyx_PyInt_As_uint32_t(__pyx_v_lookahead_size); if (unlikely((__pyx_t_3 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 166, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_uint32_t(__pyx_v_lookahead_size); if (unlikely((__pyx_t_3 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 169, __pyx_L1_error)
   __pyx_v_self->_impl.lookahead_size = __pyx_t_3;
 
-  /* "littlefs/lfs.pyx":167
+  /* "littlefs/lfs.pyx":170
  *         # Lookahead buffer size in bytes
  *         self._impl.lookahead_size = lookahead_size
  *         self._impl.name_max = name_max             # <<<<<<<<<<<<<<
  *         self._impl.file_max = file_max
  *         self._impl.attr_max = attr_max
  */
-  __pyx_t_3 = __Pyx_PyInt_As_uint32_t(__pyx_v_name_max); if (unlikely((__pyx_t_3 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 167, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_uint32_t(__pyx_v_name_max); if (unlikely((__pyx_t_3 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 170, __pyx_L1_error)
   __pyx_v_self->_impl.name_max = __pyx_t_3;
 
-  /* "littlefs/lfs.pyx":168
+  /* "littlefs/lfs.pyx":171
  *         self._impl.lookahead_size = lookahead_size
  *         self._impl.name_max = name_max
  *         self._impl.file_max = file_max             # <<<<<<<<<<<<<<
  *         self._impl.attr_max = attr_max
  *         self._impl.metadata_max = metadata_max
  */
-  __pyx_t_3 = __Pyx_PyInt_As_uint32_t(__pyx_v_file_max); if (unlikely((__pyx_t_3 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 168, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_uint32_t(__pyx_v_file_max); if (unlikely((__pyx_t_3 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 171, __pyx_L1_error)
   __pyx_v_self->_impl.file_max = __pyx_t_3;
 
-  /* "littlefs/lfs.pyx":169
+  /* "littlefs/lfs.pyx":172
  *         self._impl.name_max = name_max
  *         self._impl.file_max = file_max
  *         self._impl.attr_max = attr_max             # <<<<<<<<<<<<<<
  *         self._impl.metadata_max = metadata_max
  *         self._impl.disk_version = disk_version
  */
-  __pyx_t_3 = __Pyx_PyInt_As_uint32_t(__pyx_v_attr_max); if (unlikely((__pyx_t_3 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 169, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_uint32_t(__pyx_v_attr_max); if (unlikely((__pyx_t_3 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 172, __pyx_L1_error)
   __pyx_v_self->_impl.attr_max = __pyx_t_3;
 
-  /* "littlefs/lfs.pyx":170
+  /* "littlefs/lfs.pyx":173
  *         self._impl.file_max = file_max
  *         self._impl.attr_max = attr_max
  *         self._impl.metadata_max = metadata_max             # <<<<<<<<<<<<<<
  *         self._impl.disk_version = disk_version
  * 
  */
-  __pyx_t_3 = __Pyx_PyInt_As_uint32_t(__pyx_v_metadata_max); if (unlikely((__pyx_t_3 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 170, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_uint32_t(__pyx_v_metadata_max); if (unlikely((__pyx_t_3 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 173, __pyx_L1_error)
   __pyx_v_self->_impl.metadata_max = __pyx_t_3;
 
-  /* "littlefs/lfs.pyx":171
+  /* "littlefs/lfs.pyx":174
  *         self._impl.attr_max = attr_max
  *         self._impl.metadata_max = metadata_max
  *         self._impl.disk_version = disk_version             # <<<<<<<<<<<<<<
  * 
  *         if context is None:
  */
-  __pyx_t_9 = __Pyx_PyInt_As_uint32_t(__pyx_v_disk_version); if (unlikely((__pyx_t_9 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 171, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyInt_As_uint32_t(__pyx_v_disk_version); if (unlikely((__pyx_t_9 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 174, __pyx_L1_error)
   __pyx_v_self->_impl.disk_version = __pyx_t_9;
 
-  /* "littlefs/lfs.pyx":173
+  /* "littlefs/lfs.pyx":176
  *         self._impl.disk_version = disk_version
  * 
  *         if context is None:             # <<<<<<<<<<<<<<
  *             context = UserContext(self._impl.block_size * self._impl.block_count)
  * 
  */
   __pyx_t_2 = (__pyx_v_context == Py_None);
   if (__pyx_t_2) {
 
-    /* "littlefs/lfs.pyx":174
+    /* "littlefs/lfs.pyx":177
  * 
  *         if context is None:
  *             context = UserContext(self._impl.block_size * self._impl.block_count)             # <<<<<<<<<<<<<<
  * 
  *         self.user_context = context
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_UserContext); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 174, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_UserContext); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 177, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    __pyx_t_11 = __Pyx_PyInt_From_uint32_t((__pyx_v_self->_impl.block_size * __pyx_v_self->_impl.block_count)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 174, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyInt_From_uint32_t((__pyx_v_self->_impl.block_size * __pyx_v_self->_impl.block_count)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 177, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __pyx_t_12 = NULL;
     __pyx_t_13 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_10))) {
       __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_10);
       if (likely(__pyx_t_12)) {
@@ -19944,49 +19933,49 @@
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_12, __pyx_t_11};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_10, __pyx_callargs+1-__pyx_t_13, 1+__pyx_t_13);
       __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 174, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     }
     __Pyx_DECREF_SET(__pyx_v_context, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "littlefs/lfs.pyx":173
+    /* "littlefs/lfs.pyx":176
  *         self._impl.disk_version = disk_version
  * 
  *         if context is None:             # <<<<<<<<<<<<<<
  *             context = UserContext(self._impl.block_size * self._impl.block_count)
  * 
  */
   }
 
-  /* "littlefs/lfs.pyx":176
+  /* "littlefs/lfs.pyx":179
  *             context = UserContext(self._impl.block_size * self._impl.block_count)
  * 
  *         self.user_context = context             # <<<<<<<<<<<<<<
  *         self._impl.context = <void *>self
  * 
  */
-  if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_user_context, __pyx_v_context) < 0) __PYX_ERR(0, 176, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_user_context, __pyx_v_context) < 0) __PYX_ERR(0, 179, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":177
+  /* "littlefs/lfs.pyx":180
  * 
  *         self.user_context = context
  *         self._impl.context = <void *>self             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
   __pyx_v_self->_impl.context = ((void *)__pyx_v_self);
 
-  /* "littlefs/lfs.pyx":90
+  /* "littlefs/lfs.pyx":93
  * 
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  context=None,
  *                  *,
  */
 
@@ -20002,15 +19991,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_context);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":179
+/* "littlefs/lfs.pyx":182
  *         self._impl.context = <void *>self
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         args = (
  *             f"context={self.user_context!r}",
  */
 
@@ -20050,257 +20039,257 @@
   Py_ssize_t __pyx_t_15;
   Py_UCS4 __pyx_t_16;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 1);
 
-  /* "littlefs/lfs.pyx":181
+  /* "littlefs/lfs.pyx":184
  *     def __repr__(self):
  *         args = (
  *             f"context={self.user_context!r}",             # <<<<<<<<<<<<<<
  *             f"block_size={self._impl.block_size}",
  *             f"block_count={self._impl.block_count}",
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_user_context); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_user_context); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Repr(__pyx_t_1), __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Repr(__pyx_t_1), __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 184, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyUnicode_Concat(__pyx_kp_u_context_2, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyUnicode_Concat(__pyx_kp_u_context_2, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "littlefs/lfs.pyx":182
+  /* "littlefs/lfs.pyx":185
  *         args = (
  *             f"context={self.user_context!r}",
  *             f"block_size={self._impl.block_size}",             # <<<<<<<<<<<<<<
  *             f"block_count={self._impl.block_count}",
  *             f"read_size={self._impl.read_size}",
  */
-  __pyx_t_2 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.block_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.block_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_FormatSimple(__pyx_t_2, __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 182, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_FormatSimple(__pyx_t_2, __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_block_size_2, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_block_size_2, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "littlefs/lfs.pyx":183
+  /* "littlefs/lfs.pyx":186
  *             f"context={self.user_context!r}",
  *             f"block_size={self._impl.block_size}",
  *             f"block_count={self._impl.block_count}",             # <<<<<<<<<<<<<<
  *             f"read_size={self._impl.read_size}",
  *             f"prog_size={self._impl.prog_size}",
  */
-  __pyx_t_3 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.block_count); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 183, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.block_count); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 186, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_t_3, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 183, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_t_3, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 186, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_kp_u_block_count_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 183, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_kp_u_block_count_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 186, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "littlefs/lfs.pyx":184
+  /* "littlefs/lfs.pyx":187
  *             f"block_size={self._impl.block_size}",
  *             f"block_count={self._impl.block_count}",
  *             f"read_size={self._impl.read_size}",             # <<<<<<<<<<<<<<
  *             f"prog_size={self._impl.prog_size}",
  *             f"block_cycles={self._impl.block_cycles}",
  */
-  __pyx_t_4 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.read_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.read_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_kp_u_read_size_2, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_kp_u_read_size_2, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "littlefs/lfs.pyx":185
+  /* "littlefs/lfs.pyx":188
  *             f"block_count={self._impl.block_count}",
  *             f"read_size={self._impl.read_size}",
  *             f"prog_size={self._impl.prog_size}",             # <<<<<<<<<<<<<<
  *             f"block_cycles={self._impl.block_cycles}",
  *             f"cache_size={self._impl.cache_size}",
  */
-  __pyx_t_5 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.prog_size); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.prog_size); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_t_5, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_t_5, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyUnicode_Concat(__pyx_kp_u_prog_size_2, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyUnicode_Concat(__pyx_kp_u_prog_size_2, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "littlefs/lfs.pyx":186
+  /* "littlefs/lfs.pyx":189
  *             f"read_size={self._impl.read_size}",
  *             f"prog_size={self._impl.prog_size}",
  *             f"block_cycles={self._impl.block_cycles}",             # <<<<<<<<<<<<<<
  *             f"cache_size={self._impl.cache_size}",
  *             f"lookahead_size={self._impl.lookahead_size}",
  */
-  __pyx_t_6 = __Pyx_PyInt_From_int32_t(__pyx_v_self->_impl.block_cycles); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_int32_t(__pyx_v_self->_impl.block_cycles); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_t_6, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_t_6, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyUnicode_Concat(__pyx_kp_u_block_cycles_2, __pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyUnicode_Concat(__pyx_kp_u_block_cycles_2, __pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "littlefs/lfs.pyx":187
+  /* "littlefs/lfs.pyx":190
  *             f"prog_size={self._impl.prog_size}",
  *             f"block_cycles={self._impl.block_cycles}",
  *             f"cache_size={self._impl.cache_size}",             # <<<<<<<<<<<<<<
  *             f"lookahead_size={self._impl.lookahead_size}",
  *             f"name_max={self._impl.name_max}",
  */
-  __pyx_t_7 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.cache_size); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 187, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.cache_size); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 190, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_t_7, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 187, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_t_7, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 190, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyUnicode_Concat(__pyx_kp_u_cache_size_2, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 187, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyUnicode_Concat(__pyx_kp_u_cache_size_2, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 190, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "littlefs/lfs.pyx":188
+  /* "littlefs/lfs.pyx":191
  *             f"block_cycles={self._impl.block_cycles}",
  *             f"cache_size={self._impl.cache_size}",
  *             f"lookahead_size={self._impl.lookahead_size}",             # <<<<<<<<<<<<<<
  *             f"name_max={self._impl.name_max}",
  *             f"file_max={self._impl.file_max}",
  */
-  __pyx_t_8 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.lookahead_size); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.lookahead_size); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_9 = __Pyx_PyObject_FormatSimple(__pyx_t_8, __pyx_empty_unicode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_FormatSimple(__pyx_t_8, __pyx_empty_unicode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyUnicode_Concat(__pyx_kp_u_lookahead_size_2, __pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyUnicode_Concat(__pyx_kp_u_lookahead_size_2, __pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-  /* "littlefs/lfs.pyx":189
+  /* "littlefs/lfs.pyx":192
  *             f"cache_size={self._impl.cache_size}",
  *             f"lookahead_size={self._impl.lookahead_size}",
  *             f"name_max={self._impl.name_max}",             # <<<<<<<<<<<<<<
  *             f"file_max={self._impl.file_max}",
  *             f"attr_max={self._impl.attr_max}",
  */
-  __pyx_t_9 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.name_max); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 189, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.name_max); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 192, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_10 = __Pyx_PyObject_FormatSimple(__pyx_t_9, __pyx_empty_unicode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 189, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_FormatSimple(__pyx_t_9, __pyx_empty_unicode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 192, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __pyx_t_9 = __Pyx_PyUnicode_Concat(__pyx_kp_u_name_max_2, __pyx_t_10); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 189, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyUnicode_Concat(__pyx_kp_u_name_max_2, __pyx_t_10); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 192, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-  /* "littlefs/lfs.pyx":190
+  /* "littlefs/lfs.pyx":193
  *             f"lookahead_size={self._impl.lookahead_size}",
  *             f"name_max={self._impl.name_max}",
  *             f"file_max={self._impl.file_max}",             # <<<<<<<<<<<<<<
  *             f"attr_max={self._impl.attr_max}",
  *             f"metadata_max={self._impl.metadata_max}",
  */
-  __pyx_t_10 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.file_max); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 190, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.file_max); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 193, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_11 = __Pyx_PyObject_FormatSimple(__pyx_t_10, __pyx_empty_unicode); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 190, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_FormatSimple(__pyx_t_10, __pyx_empty_unicode); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 193, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_t_10 = __Pyx_PyUnicode_Concat(__pyx_kp_u_file_max_2, __pyx_t_11); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 190, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyUnicode_Concat(__pyx_kp_u_file_max_2, __pyx_t_11); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 193, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-  /* "littlefs/lfs.pyx":191
+  /* "littlefs/lfs.pyx":194
  *             f"name_max={self._impl.name_max}",
  *             f"file_max={self._impl.file_max}",
  *             f"attr_max={self._impl.attr_max}",             # <<<<<<<<<<<<<<
  *             f"metadata_max={self._impl.metadata_max}",
  *             f"disk_version={self._impl.disk_version}"
  */
-  __pyx_t_11 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.attr_max); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 191, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.attr_max); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
-  __pyx_t_12 = __Pyx_PyObject_FormatSimple(__pyx_t_11, __pyx_empty_unicode); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 191, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_FormatSimple(__pyx_t_11, __pyx_empty_unicode); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-  __pyx_t_11 = __Pyx_PyUnicode_Concat(__pyx_kp_u_attr_max_2, __pyx_t_12); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 191, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyUnicode_Concat(__pyx_kp_u_attr_max_2, __pyx_t_12); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
 
-  /* "littlefs/lfs.pyx":192
+  /* "littlefs/lfs.pyx":195
  *             f"file_max={self._impl.file_max}",
  *             f"attr_max={self._impl.attr_max}",
  *             f"metadata_max={self._impl.metadata_max}",             # <<<<<<<<<<<<<<
  *             f"disk_version={self._impl.disk_version}"
  *         )
  */
-  __pyx_t_12 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.metadata_max); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.metadata_max); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 195, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_13 = __Pyx_PyObject_FormatSimple(__pyx_t_12, __pyx_empty_unicode); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyObject_FormatSimple(__pyx_t_12, __pyx_empty_unicode); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 195, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  __pyx_t_12 = __Pyx_PyUnicode_Concat(__pyx_kp_u_metadata_max_2, __pyx_t_13); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyUnicode_Concat(__pyx_kp_u_metadata_max_2, __pyx_t_13); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 195, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
 
-  /* "littlefs/lfs.pyx":193
+  /* "littlefs/lfs.pyx":196
  *             f"attr_max={self._impl.attr_max}",
  *             f"metadata_max={self._impl.metadata_max}",
  *             f"disk_version={self._impl.disk_version}"             # <<<<<<<<<<<<<<
  *         )
  *         return f"{self.__class__.__name__}({', '.join(args)})"
  */
-  __pyx_t_13 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.disk_version); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.disk_version); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
-  __pyx_t_14 = __Pyx_PyObject_FormatSimple(__pyx_t_13, __pyx_empty_unicode); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyObject_FormatSimple(__pyx_t_13, __pyx_empty_unicode); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-  __pyx_t_13 = __Pyx_PyUnicode_Concat(__pyx_kp_u_disk_version_2, __pyx_t_14); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyUnicode_Concat(__pyx_kp_u_disk_version_2, __pyx_t_14); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
 
-  /* "littlefs/lfs.pyx":181
+  /* "littlefs/lfs.pyx":184
  *     def __repr__(self):
  *         args = (
  *             f"context={self.user_context!r}",             # <<<<<<<<<<<<<<
  *             f"block_size={self._impl.block_size}",
  *             f"block_count={self._impl.block_count}",
  */
-  __pyx_t_14 = PyTuple_New(13); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_14 = PyTuple_New(13); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 184, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_t_2)) __PYX_ERR(0, 181, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_t_2)) __PYX_ERR(0, 184, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 2, __pyx_t_3)) __PYX_ERR(0, 181, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 2, __pyx_t_3)) __PYX_ERR(0, 184, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 3, __pyx_t_4)) __PYX_ERR(0, 181, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 3, __pyx_t_4)) __PYX_ERR(0, 184, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_5);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 4, __pyx_t_5)) __PYX_ERR(0, 181, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 4, __pyx_t_5)) __PYX_ERR(0, 184, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_6);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 5, __pyx_t_6)) __PYX_ERR(0, 181, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 5, __pyx_t_6)) __PYX_ERR(0, 184, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_7);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 6, __pyx_t_7)) __PYX_ERR(0, 181, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 6, __pyx_t_7)) __PYX_ERR(0, 184, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_8);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 7, __pyx_t_8)) __PYX_ERR(0, 181, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 7, __pyx_t_8)) __PYX_ERR(0, 184, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_9);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 8, __pyx_t_9)) __PYX_ERR(0, 181, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 8, __pyx_t_9)) __PYX_ERR(0, 184, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_10);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 9, __pyx_t_10)) __PYX_ERR(0, 181, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 9, __pyx_t_10)) __PYX_ERR(0, 184, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_11);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 10, __pyx_t_11)) __PYX_ERR(0, 181, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 10, __pyx_t_11)) __PYX_ERR(0, 184, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_12);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 11, __pyx_t_12)) __PYX_ERR(0, 181, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 11, __pyx_t_12)) __PYX_ERR(0, 184, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_13);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 12, __pyx_t_13)) __PYX_ERR(0, 181, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 12, __pyx_t_13)) __PYX_ERR(0, 184, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
   __pyx_t_5 = 0;
   __pyx_t_6 = 0;
   __pyx_t_7 = 0;
@@ -20309,62 +20298,62 @@
   __pyx_t_10 = 0;
   __pyx_t_11 = 0;
   __pyx_t_12 = 0;
   __pyx_t_13 = 0;
   __pyx_v_args = ((PyObject*)__pyx_t_14);
   __pyx_t_14 = 0;
 
-  /* "littlefs/lfs.pyx":195
+  /* "littlefs/lfs.pyx":198
  *             f"disk_version={self._impl.disk_version}"
  *         )
  *         return f"{self.__class__.__name__}({', '.join(args)})"             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_14 = PyTuple_New(4); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 195, __pyx_L1_error)
+  __pyx_t_14 = PyTuple_New(4); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 198, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __pyx_t_15 = 0;
   __pyx_t_16 = 127;
-  __pyx_t_13 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 195, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 198, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
-  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_13, __pyx_n_s_name_2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 195, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_13, __pyx_n_s_name_2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 198, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-  __pyx_t_13 = __Pyx_PyObject_FormatSimple(__pyx_t_12, __pyx_empty_unicode); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 195, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyObject_FormatSimple(__pyx_t_12, __pyx_empty_unicode); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 198, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   __pyx_t_16 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_13) > __pyx_t_16) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_13) : __pyx_t_16;
   __pyx_t_15 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_13);
   __Pyx_GIVEREF(__pyx_t_13);
   PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_13);
   __pyx_t_13 = 0;
   __Pyx_INCREF(__pyx_kp_u__23);
   __pyx_t_15 += 1;
   __Pyx_GIVEREF(__pyx_kp_u__23);
   PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_kp_u__23);
-  __pyx_t_13 = PyUnicode_Join(__pyx_kp_u__24, __pyx_v_args); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 195, __pyx_L1_error)
+  __pyx_t_13 = PyUnicode_Join(__pyx_kp_u__24, __pyx_v_args); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 198, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __pyx_t_16 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_13) > __pyx_t_16) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_13) : __pyx_t_16;
   __pyx_t_15 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_13);
   __Pyx_GIVEREF(__pyx_t_13);
   PyTuple_SET_ITEM(__pyx_t_14, 2, __pyx_t_13);
   __pyx_t_13 = 0;
   __Pyx_INCREF(__pyx_kp_u__7);
   __pyx_t_15 += 1;
   __Pyx_GIVEREF(__pyx_kp_u__7);
   PyTuple_SET_ITEM(__pyx_t_14, 3, __pyx_kp_u__7);
-  __pyx_t_13 = __Pyx_PyUnicode_Join(__pyx_t_14, 4, __pyx_t_15, __pyx_t_16); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 195, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyUnicode_Join(__pyx_t_14, 4, __pyx_t_15, __pyx_t_16); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 198, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
   __pyx_r = __pyx_t_13;
   __pyx_t_13 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":179
+  /* "littlefs/lfs.pyx":182
  *         self._impl.context = <void *>self
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         args = (
  *             f"context={self.user_context!r}",
  */
 
@@ -20389,15 +20378,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_args);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":197
+/* "littlefs/lfs.pyx":200
  *         return f"{self.__class__.__name__}({', '.join(args)})"
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def read_size(self):
  *         return self._impl.read_size
  */
 
@@ -20421,29 +20410,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
 
-  /* "littlefs/lfs.pyx":199
+  /* "littlefs/lfs.pyx":202
  *     @property
  *     def read_size(self):
  *         return self._impl.read_size             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.read_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.read_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":197
+  /* "littlefs/lfs.pyx":200
  *         return f"{self.__class__.__name__}({', '.join(args)})"
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def read_size(self):
  *         return self._impl.read_size
  */
 
@@ -20454,15 +20443,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":201
+/* "littlefs/lfs.pyx":204
  *         return self._impl.read_size
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def prog_size(self):
  *         return self._impl.prog_size
  */
 
@@ -20486,29 +20475,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
 
-  /* "littlefs/lfs.pyx":203
+  /* "littlefs/lfs.pyx":206
  *     @property
  *     def prog_size(self):
  *         return self._impl.prog_size             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.prog_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.prog_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":201
+  /* "littlefs/lfs.pyx":204
  *         return self._impl.read_size
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def prog_size(self):
  *         return self._impl.prog_size
  */
 
@@ -20519,15 +20508,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":205
+/* "littlefs/lfs.pyx":208
  *         return self._impl.prog_size
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def block_size(self):
  *         return self._impl.block_size
  */
 
@@ -20551,29 +20540,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
 
-  /* "littlefs/lfs.pyx":207
+  /* "littlefs/lfs.pyx":210
  *     @property
  *     def block_size(self):
  *         return self._impl.block_size             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.block_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.block_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":205
+  /* "littlefs/lfs.pyx":208
  *         return self._impl.prog_size
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def block_size(self):
  *         return self._impl.block_size
  */
 
@@ -20584,15 +20573,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":209
+/* "littlefs/lfs.pyx":212
  *         return self._impl.block_size
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def block_count(self):
  *         return self._impl.block_count
  */
 
@@ -20616,29 +20605,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
 
-  /* "littlefs/lfs.pyx":211
+  /* "littlefs/lfs.pyx":214
  *     @property
  *     def block_count(self):
  *         return self._impl.block_count             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.block_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 211, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.block_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 214, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":209
+  /* "littlefs/lfs.pyx":212
  *         return self._impl.block_size
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def block_count(self):
  *         return self._impl.block_count
  */
 
@@ -20649,15 +20638,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":213
+/* "littlefs/lfs.pyx":216
  *         return self._impl.block_count
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def cache_size(self):
  *         return self._impl.cache_size
  */
 
@@ -20681,29 +20670,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
 
-  /* "littlefs/lfs.pyx":215
+  /* "littlefs/lfs.pyx":218
  *     @property
  *     def cache_size(self):
  *         return self._impl.cache_size             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.cache_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 215, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.cache_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 218, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":213
+  /* "littlefs/lfs.pyx":216
  *         return self._impl.block_count
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def cache_size(self):
  *         return self._impl.cache_size
  */
 
@@ -20714,15 +20703,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":217
+/* "littlefs/lfs.pyx":220
  *         return self._impl.cache_size
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def lookahead_size(self):
  *         return self._impl.lookahead_size
  */
 
@@ -20746,29 +20735,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
 
-  /* "littlefs/lfs.pyx":219
+  /* "littlefs/lfs.pyx":222
  *     @property
  *     def lookahead_size(self):
  *         return self._impl.lookahead_size             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.lookahead_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.lookahead_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":217
+  /* "littlefs/lfs.pyx":220
  *         return self._impl.cache_size
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def lookahead_size(self):
  *         return self._impl.lookahead_size
  */
 
@@ -20779,15 +20768,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":221
+/* "littlefs/lfs.pyx":224
  *         return self._impl.lookahead_size
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def name_max(self):
  *         return self._impl.name_max
  */
 
@@ -20811,29 +20800,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
 
-  /* "littlefs/lfs.pyx":223
+  /* "littlefs/lfs.pyx":226
  *     @property
  *     def name_max(self):
  *         return self._impl.name_max             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.name_max); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.name_max); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":221
+  /* "littlefs/lfs.pyx":224
  *         return self._impl.lookahead_size
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def name_max(self):
  *         return self._impl.name_max
  */
 
@@ -20844,15 +20833,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":225
+/* "littlefs/lfs.pyx":228
  *         return self._impl.name_max
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def file_max(self):
  *         return self._impl.file_max
  */
 
@@ -20876,29 +20865,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
 
-  /* "littlefs/lfs.pyx":227
+  /* "littlefs/lfs.pyx":230
  *     @property
  *     def file_max(self):
  *         return self._impl.file_max             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.file_max); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.file_max); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 230, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":225
+  /* "littlefs/lfs.pyx":228
  *         return self._impl.name_max
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def file_max(self):
  *         return self._impl.file_max
  */
 
@@ -20909,15 +20898,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":229
+/* "littlefs/lfs.pyx":232
  *         return self._impl.file_max
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def attr_max(self):
  *         return self._impl.attr_max
  */
 
@@ -20941,29 +20930,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
 
-  /* "littlefs/lfs.pyx":231
+  /* "littlefs/lfs.pyx":234
  *     @property
  *     def attr_max(self):
  *         return self._impl.attr_max             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.attr_max); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 231, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.attr_max); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 234, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":229
+  /* "littlefs/lfs.pyx":232
  *         return self._impl.file_max
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def attr_max(self):
  *         return self._impl.attr_max
  */
 
@@ -20974,15 +20963,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":233
+/* "littlefs/lfs.pyx":236
  *         return self._impl.attr_max
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def metadata_max(self):
  *         return self._impl.metadata_max
  */
 
@@ -21006,29 +20995,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
 
-  /* "littlefs/lfs.pyx":235
+  /* "littlefs/lfs.pyx":238
  *     @property
  *     def metadata_max(self):
  *         return self._impl.metadata_max             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.metadata_max); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.metadata_max); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":233
+  /* "littlefs/lfs.pyx":236
  *         return self._impl.attr_max
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def metadata_max(self):
  *         return self._impl.metadata_max
  */
 
@@ -21039,15 +21028,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":237
+/* "littlefs/lfs.pyx":240
  *         return self._impl.metadata_max
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def disk_version(self):
  *         return self._impl.disk_version
  */
 
@@ -21071,29 +21060,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
 
-  /* "littlefs/lfs.pyx":239
+  /* "littlefs/lfs.pyx":242
  *     @property
  *     def disk_version(self):
  *         return self._impl.disk_version             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.disk_version); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.disk_version); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":237
+  /* "littlefs/lfs.pyx":240
  *         return self._impl.metadata_max
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def disk_version(self):
  *         return self._impl.disk_version
  */
 
@@ -21320,15 +21309,15 @@
   __Pyx_AddTraceback("littlefs.lfs.LFSConfig.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":245
+/* "littlefs/lfs.pyx":248
  *     cdef lfs_t _impl
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def block_count(self) -> lfs_size_t:
  *         return self._impl.block_count
  */
 
@@ -21352,29 +21341,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
 
-  /* "littlefs/lfs.pyx":247
+  /* "littlefs/lfs.pyx":250
  *     @property
  *     def block_count(self) -> lfs_size_t:
  *         return self._impl.block_count             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.block_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.block_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":245
+  /* "littlefs/lfs.pyx":248
  *     cdef lfs_t _impl
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def block_count(self) -> lfs_size_t:
  *         return self._impl.block_count
  */
 
@@ -21601,15 +21590,15 @@
   __Pyx_AddTraceback("littlefs.lfs.LFSFilesystem.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":253
+/* "littlefs/lfs.pyx":256
  *     cdef lfs_file_t _impl
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def flags(self) -> LFSFileFlag:
  *         """Mode flags of an open file"""
  */
 
@@ -21637,25 +21626,25 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
 
-  /* "littlefs/lfs.pyx":256
+  /* "littlefs/lfs.pyx":259
  *     def flags(self) -> LFSFileFlag:
  *         """Mode flags of an open file"""
  *         return LFSFileFlag(self._impl.flags)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LFSFileFlag); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 256, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LFSFileFlag); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.flags); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 256, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_impl.flags); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
@@ -21668,23 +21657,23 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_3};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 256, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":253
+  /* "littlefs/lfs.pyx":256
  *     cdef lfs_file_t _impl
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def flags(self) -> LFSFileFlag:
  *         """Mode flags of an open file"""
  */
 
@@ -22130,15 +22119,15 @@
   __Pyx_AddTraceback("littlefs.lfs.LFSDirectory.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":263
+/* "littlefs/lfs.pyx":266
  * 
  * 
  * def fs_stat(LFSFilesystem fs):             # <<<<<<<<<<<<<<
  *     """Get filesystem status"""
  *     cdef lfs_fsinfo * info = <lfs_fsinfo *>malloc(sizeof(lfs_fsinfo))
  */
 
@@ -22192,45 +22181,45 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 263, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 266, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "fs_stat") < 0)) __PYX_ERR(0, 263, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "fs_stat") < 0)) __PYX_ERR(0, 266, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("fs_stat", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 263, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("fs_stat", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 266, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.fs_stat", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 263, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 266, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_fs_stat(__pyx_self, __pyx_v_fs);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -22267,110 +22256,110 @@
   PyObject *__pyx_t_17 = NULL;
   PyObject *__pyx_t_18 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("fs_stat", 1);
 
-  /* "littlefs/lfs.pyx":265
+  /* "littlefs/lfs.pyx":268
  * def fs_stat(LFSFilesystem fs):
  *     """Get filesystem status"""
  *     cdef lfs_fsinfo * info = <lfs_fsinfo *>malloc(sizeof(lfs_fsinfo))             # <<<<<<<<<<<<<<
  *     try:
  *         _raise_on_error(lfs_fs_stat(&fs._impl, info))
  */
   __pyx_v_info = ((struct lfs_fsinfo *)malloc((sizeof(struct lfs_fsinfo))));
 
-  /* "littlefs/lfs.pyx":266
+  /* "littlefs/lfs.pyx":269
  *     """Get filesystem status"""
  *     cdef lfs_fsinfo * info = <lfs_fsinfo *>malloc(sizeof(lfs_fsinfo))
  *     try:             # <<<<<<<<<<<<<<
  *         _raise_on_error(lfs_fs_stat(&fs._impl, info))
  *         return LFSFSStat(
  */
   /*try:*/ {
 
-    /* "littlefs/lfs.pyx":267
+    /* "littlefs/lfs.pyx":270
  *     cdef lfs_fsinfo * info = <lfs_fsinfo *>malloc(sizeof(lfs_fsinfo))
  *     try:
  *         _raise_on_error(lfs_fs_stat(&fs._impl, info))             # <<<<<<<<<<<<<<
  *         return LFSFSStat(
  *             info.disk_version,
  */
-    __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_fs_stat((&__pyx_v_fs->_impl), __pyx_v_info)); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 267, __pyx_L4_error)
+    __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_fs_stat((&__pyx_v_fs->_impl), __pyx_v_info)); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 270, __pyx_L4_error)
 
-    /* "littlefs/lfs.pyx":268
+    /* "littlefs/lfs.pyx":271
  *     try:
  *         _raise_on_error(lfs_fs_stat(&fs._impl, info))
  *         return LFSFSStat(             # <<<<<<<<<<<<<<
  *             info.disk_version,
  *             info.name_max,
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LFSFSStat); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 268, __pyx_L4_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LFSFSStat); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 271, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_3);
 
-    /* "littlefs/lfs.pyx":269
+    /* "littlefs/lfs.pyx":272
  *         _raise_on_error(lfs_fs_stat(&fs._impl, info))
  *         return LFSFSStat(
  *             info.disk_version,             # <<<<<<<<<<<<<<
  *             info.name_max,
  *             info.file_max,
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint32_t(__pyx_v_info->disk_version); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 269, __pyx_L4_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint32_t(__pyx_v_info->disk_version); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 272, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_4);
 
-    /* "littlefs/lfs.pyx":270
+    /* "littlefs/lfs.pyx":273
  *         return LFSFSStat(
  *             info.disk_version,
  *             info.name_max,             # <<<<<<<<<<<<<<
  *             info.file_max,
  *             info.attr_max,
  */
-    __pyx_t_5 = __Pyx_PyInt_From_uint32_t(__pyx_v_info->name_max); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 270, __pyx_L4_error)
+    __pyx_t_5 = __Pyx_PyInt_From_uint32_t(__pyx_v_info->name_max); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 273, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_5);
 
-    /* "littlefs/lfs.pyx":271
+    /* "littlefs/lfs.pyx":274
  *             info.disk_version,
  *             info.name_max,
  *             info.file_max,             # <<<<<<<<<<<<<<
  *             info.attr_max,
  *             info.block_count,
  */
-    __pyx_t_6 = __Pyx_PyInt_From_uint32_t(__pyx_v_info->file_max); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 271, __pyx_L4_error)
+    __pyx_t_6 = __Pyx_PyInt_From_uint32_t(__pyx_v_info->file_max); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 274, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_6);
 
-    /* "littlefs/lfs.pyx":272
+    /* "littlefs/lfs.pyx":275
  *             info.name_max,
  *             info.file_max,
  *             info.attr_max,             # <<<<<<<<<<<<<<
  *             info.block_count,
  *             info.block_size,
  */
-    __pyx_t_7 = __Pyx_PyInt_From_uint32_t(__pyx_v_info->attr_max); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 272, __pyx_L4_error)
+    __pyx_t_7 = __Pyx_PyInt_From_uint32_t(__pyx_v_info->attr_max); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 275, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_7);
 
-    /* "littlefs/lfs.pyx":273
+    /* "littlefs/lfs.pyx":276
  *             info.file_max,
  *             info.attr_max,
  *             info.block_count,             # <<<<<<<<<<<<<<
  *             info.block_size,
  *         )
  */
-    __pyx_t_8 = __Pyx_PyInt_From_uint32_t(__pyx_v_info->block_count); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 273, __pyx_L4_error)
+    __pyx_t_8 = __Pyx_PyInt_From_uint32_t(__pyx_v_info->block_count); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 276, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_8);
 
-    /* "littlefs/lfs.pyx":274
+    /* "littlefs/lfs.pyx":277
  *             info.attr_max,
  *             info.block_count,
  *             info.block_size,             # <<<<<<<<<<<<<<
  *         )
  *     finally:
  */
-    __pyx_t_9 = __Pyx_PyInt_From_uint32_t(__pyx_v_info->block_size); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 274, __pyx_L4_error)
+    __pyx_t_9 = __Pyx_PyInt_From_uint32_t(__pyx_v_info->block_size); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 277, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_10 = NULL;
     __pyx_t_1 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_10)) {
@@ -22388,24 +22377,24 @@
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 268, __pyx_L4_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 271, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L3_return;
   }
 
-  /* "littlefs/lfs.pyx":277
+  /* "littlefs/lfs.pyx":280
  *         )
  *     finally:
  *         free(info)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*finally:*/ {
@@ -22455,15 +22444,15 @@
       free(__pyx_v_info);
       __pyx_r = __pyx_t_18;
       __pyx_t_18 = 0;
       goto __pyx_L0;
     }
   }
 
-  /* "littlefs/lfs.pyx":263
+  /* "littlefs/lfs.pyx":266
  * 
  * 
  * def fs_stat(LFSFilesystem fs):             # <<<<<<<<<<<<<<
  *     """Get filesystem status"""
  *     cdef lfs_fsinfo * info = <lfs_fsinfo *>malloc(sizeof(lfs_fsinfo))
  */
 
@@ -22482,15 +22471,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":280
+/* "littlefs/lfs.pyx":283
  * 
  * 
  * def fs_size(LFSFilesystem fs):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_fs_size(&fs._impl))
  * 
  */
 
@@ -22544,45 +22533,45 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 280, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 283, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "fs_size") < 0)) __PYX_ERR(0, 280, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "fs_size") < 0)) __PYX_ERR(0, 283, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("fs_size", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 280, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("fs_size", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 283, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.fs_size", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 280, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 283, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_2fs_size(__pyx_self, __pyx_v_fs);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -22602,30 +22591,30 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("fs_size", 1);
 
-  /* "littlefs/lfs.pyx":281
+  /* "littlefs/lfs.pyx":284
  * 
  * def fs_size(LFSFilesystem fs):
  *     return _raise_on_error(lfs_fs_size(&fs._impl))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_fs_size((&__pyx_v_fs->_impl))); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 281, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 281, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_fs_size((&__pyx_v_fs->_impl))); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 284, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":280
+  /* "littlefs/lfs.pyx":283
  * 
  * 
  * def fs_size(LFSFilesystem fs):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_fs_size(&fs._impl))
  * 
  */
 
@@ -22636,15 +22625,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":284
+/* "littlefs/lfs.pyx":287
  * 
  * 
  * def format(LFSFilesystem fs, LFSConfig cfg):             # <<<<<<<<<<<<<<
  *     """Format the filesystem"""
  *     return _raise_on_error(lfs_format(&fs._impl, &cfg._impl))
  */
 
@@ -22701,58 +22690,58 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 284, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 287, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_cfg)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 284, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 287, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("format", 1, 2, 2, 1); __PYX_ERR(0, 284, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("format", 1, 2, 2, 1); __PYX_ERR(0, 287, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "format") < 0)) __PYX_ERR(0, 284, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "format") < 0)) __PYX_ERR(0, 287, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
     __pyx_v_cfg = ((struct __pyx_obj_8littlefs_3lfs_LFSConfig *)values[1]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("format", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 284, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("format", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 287, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.format", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 284, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_cfg), __pyx_ptype_8littlefs_3lfs_LFSConfig, 1, "cfg", 0))) __PYX_ERR(0, 284, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 287, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_cfg), __pyx_ptype_8littlefs_3lfs_LFSConfig, 1, "cfg", 0))) __PYX_ERR(0, 287, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_4format(__pyx_self, __pyx_v_fs, __pyx_v_cfg);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -22772,30 +22761,30 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("format", 1);
 
-  /* "littlefs/lfs.pyx":286
+  /* "littlefs/lfs.pyx":289
  * def format(LFSFilesystem fs, LFSConfig cfg):
  *     """Format the filesystem"""
  *     return _raise_on_error(lfs_format(&fs._impl, &cfg._impl))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_format((&__pyx_v_fs->_impl), (&__pyx_v_cfg->_impl))); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 286, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 286, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_format((&__pyx_v_fs->_impl), (&__pyx_v_cfg->_impl))); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 289, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":284
+  /* "littlefs/lfs.pyx":287
  * 
  * 
  * def format(LFSFilesystem fs, LFSConfig cfg):             # <<<<<<<<<<<<<<
  *     """Format the filesystem"""
  *     return _raise_on_error(lfs_format(&fs._impl, &cfg._impl))
  */
 
@@ -22806,15 +22795,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":289
+/* "littlefs/lfs.pyx":292
  * 
  * 
  * def mount(LFSFilesystem fs, LFSConfig cfg):             # <<<<<<<<<<<<<<
  *     """Mount the filesystem"""
  *     return _raise_on_error(lfs_mount(&fs._impl, &cfg._impl))
  */
 
@@ -22871,58 +22860,58 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 289, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 292, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_cfg)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 289, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 292, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("mount", 1, 2, 2, 1); __PYX_ERR(0, 289, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("mount", 1, 2, 2, 1); __PYX_ERR(0, 292, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "mount") < 0)) __PYX_ERR(0, 289, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "mount") < 0)) __PYX_ERR(0, 292, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
     __pyx_v_cfg = ((struct __pyx_obj_8littlefs_3lfs_LFSConfig *)values[1]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("mount", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 289, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("mount", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 292, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.mount", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 289, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_cfg), __pyx_ptype_8littlefs_3lfs_LFSConfig, 1, "cfg", 0))) __PYX_ERR(0, 289, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 292, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_cfg), __pyx_ptype_8littlefs_3lfs_LFSConfig, 1, "cfg", 0))) __PYX_ERR(0, 292, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_6mount(__pyx_self, __pyx_v_fs, __pyx_v_cfg);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -22942,30 +22931,30 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("mount", 1);
 
-  /* "littlefs/lfs.pyx":291
+  /* "littlefs/lfs.pyx":294
  * def mount(LFSFilesystem fs, LFSConfig cfg):
  *     """Mount the filesystem"""
  *     return _raise_on_error(lfs_mount(&fs._impl, &cfg._impl))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_mount((&__pyx_v_fs->_impl), (&__pyx_v_cfg->_impl))); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 291, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 291, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_mount((&__pyx_v_fs->_impl), (&__pyx_v_cfg->_impl))); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 294, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 294, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":289
+  /* "littlefs/lfs.pyx":292
  * 
  * 
  * def mount(LFSFilesystem fs, LFSConfig cfg):             # <<<<<<<<<<<<<<
  *     """Mount the filesystem"""
  *     return _raise_on_error(lfs_mount(&fs._impl, &cfg._impl))
  */
 
@@ -22976,15 +22965,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":294
+/* "littlefs/lfs.pyx":297
  * 
  * 
  * def unmount(LFSFilesystem fs):             # <<<<<<<<<<<<<<
  *     """Unmount the filesystem
  * 
  */
 
@@ -23038,45 +23027,45 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 294, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 297, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "unmount") < 0)) __PYX_ERR(0, 294, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "unmount") < 0)) __PYX_ERR(0, 297, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("unmount", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 294, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("unmount", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 297, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.unmount", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 294, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 297, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_8unmount(__pyx_self, __pyx_v_fs);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -23096,30 +23085,30 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("unmount", 1);
 
-  /* "littlefs/lfs.pyx":299
+  /* "littlefs/lfs.pyx":302
  *     This does nothing beside releasing any allocated resources
  *     """
  *     return _raise_on_error(lfs_unmount(&fs._impl))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_unmount((&__pyx_v_fs->_impl))); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 299, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 299, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_unmount((&__pyx_v_fs->_impl))); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 302, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 302, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":294
+  /* "littlefs/lfs.pyx":297
  * 
  * 
  * def unmount(LFSFilesystem fs):             # <<<<<<<<<<<<<<
  *     """Unmount the filesystem
  * 
  */
 
@@ -23130,15 +23119,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":302
+/* "littlefs/lfs.pyx":305
  * 
  * 
  * def fs_mkconsistent(LFSFilesystem fs):             # <<<<<<<<<<<<<<
  *     """Attempt to make the filesystem consistent and ready for writing"""
  *     return _raise_on_error(lfs_fs_mkconsistent(&fs._impl))
  */
 
@@ -23192,45 +23181,45 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 302, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 305, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "fs_mkconsistent") < 0)) __PYX_ERR(0, 302, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "fs_mkconsistent") < 0)) __PYX_ERR(0, 305, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("fs_mkconsistent", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 302, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("fs_mkconsistent", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 305, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.fs_mkconsistent", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 302, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 305, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_10fs_mkconsistent(__pyx_self, __pyx_v_fs);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -23250,30 +23239,30 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("fs_mkconsistent", 1);
 
-  /* "littlefs/lfs.pyx":304
+  /* "littlefs/lfs.pyx":307
  * def fs_mkconsistent(LFSFilesystem fs):
  *     """Attempt to make the filesystem consistent and ready for writing"""
  *     return _raise_on_error(lfs_fs_mkconsistent(&fs._impl))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_fs_mkconsistent((&__pyx_v_fs->_impl))); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 304, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 304, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_fs_mkconsistent((&__pyx_v_fs->_impl))); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 307, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 307, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":302
+  /* "littlefs/lfs.pyx":305
  * 
  * 
  * def fs_mkconsistent(LFSFilesystem fs):             # <<<<<<<<<<<<<<
  *     """Attempt to make the filesystem consistent and ready for writing"""
  *     return _raise_on_error(lfs_fs_mkconsistent(&fs._impl))
  */
 
@@ -23284,15 +23273,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":307
+/* "littlefs/lfs.pyx":310
  * 
  * 
  * def fs_grow(LFSFilesystem fs, block_count) -> int:             # <<<<<<<<<<<<<<
  *     """Irreversibly grows the filesystem to a new size.
  * 
  */
 
@@ -23349,57 +23338,57 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 307, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 310, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_block_count)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 307, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 310, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("fs_grow", 1, 2, 2, 1); __PYX_ERR(0, 307, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("fs_grow", 1, 2, 2, 1); __PYX_ERR(0, 310, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "fs_grow") < 0)) __PYX_ERR(0, 307, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "fs_grow") < 0)) __PYX_ERR(0, 310, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
     __pyx_v_block_count = values[1];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("fs_grow", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 307, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("fs_grow", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 310, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.fs_grow", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 307, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 310, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_12fs_grow(__pyx_self, __pyx_v_fs, __pyx_v_block_count);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -23420,32 +23409,32 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("fs_grow", 1);
 
-  /* "littlefs/lfs.pyx":316
+  /* "littlefs/lfs.pyx":319
  *         Number of blocks in the new filesystem.
  *     """
  *     return _raise_on_error(lfs_fs_grow(&fs._impl, block_count))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_uint32_t(__pyx_v_block_count); if (unlikely((__pyx_t_1 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 316, __pyx_L1_error)
-  __pyx_t_2 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_fs_grow((&__pyx_v_fs->_impl), __pyx_t_1)); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 316, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 316, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint32_t(__pyx_v_block_count); if (unlikely((__pyx_t_1 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 319, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_fs_grow((&__pyx_v_fs->_impl), __pyx_t_1)); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 319, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 319, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_3)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_3))) __PYX_ERR(0, 316, __pyx_L1_error)
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_3)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_3))) __PYX_ERR(0, 319, __pyx_L1_error)
   __pyx_r = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":307
+  /* "littlefs/lfs.pyx":310
  * 
  * 
  * def fs_grow(LFSFilesystem fs, block_count) -> int:             # <<<<<<<<<<<<<<
  *     """Irreversibly grows the filesystem to a new size.
  * 
  */
 
@@ -23456,15 +23445,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":319
+/* "littlefs/lfs.pyx":322
  * 
  * 
  * def remove(LFSFilesystem fs, path):             # <<<<<<<<<<<<<<
  *     """Remove a file or directory
  * 
  */
 
@@ -23521,57 +23510,57 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 319, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 322, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_path)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 319, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 322, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("remove", 1, 2, 2, 1); __PYX_ERR(0, 319, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("remove", 1, 2, 2, 1); __PYX_ERR(0, 322, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "remove") < 0)) __PYX_ERR(0, 319, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "remove") < 0)) __PYX_ERR(0, 322, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
     __pyx_v_path = values[1];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("remove", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 319, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("remove", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 322, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.remove", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 319, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 322, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_14remove(__pyx_self, __pyx_v_fs, __pyx_v_path);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -23595,25 +23584,25 @@
   int __pyx_t_5;
   char const *__pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("remove", 1);
 
-  /* "littlefs/lfs.pyx":324
+  /* "littlefs/lfs.pyx":327
  *     If removing a directory, the directory must be empty.
  *     """
  *     return _raise_on_error(lfs_remove(&fs._impl, path.encode(FILENAME_ENCODING)))             # <<<<<<<<<<<<<<
  * 
  * def rename(LFSFilesystem fs, oldpath, newpath):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_path, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 324, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_path, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 327, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FILENAME_ENCODING); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 324, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FILENAME_ENCODING); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 327, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
@@ -23626,28 +23615,28 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_3};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 324, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 327, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_t_6 = __Pyx_PyObject_AsString(__pyx_t_1); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 324, __pyx_L1_error)
-  __pyx_t_5 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_remove((&__pyx_v_fs->_impl), __pyx_t_6)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 324, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_AsString(__pyx_t_1); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 327, __pyx_L1_error)
+  __pyx_t_5 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_remove((&__pyx_v_fs->_impl), __pyx_t_6)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 327, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 324, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 327, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":319
+  /* "littlefs/lfs.pyx":322
  * 
  * 
  * def remove(LFSFilesystem fs, path):             # <<<<<<<<<<<<<<
  *     """Remove a file or directory
  * 
  */
 
@@ -23661,15 +23650,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":326
+/* "littlefs/lfs.pyx":329
  *     return _raise_on_error(lfs_remove(&fs._impl, path.encode(FILENAME_ENCODING)))
  * 
  * def rename(LFSFilesystem fs, oldpath, newpath):             # <<<<<<<<<<<<<<
  *     """Rename or move a file or directory
  * 
  */
 
@@ -23729,69 +23718,69 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 326, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 329, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_oldpath)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 326, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 329, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("rename", 1, 3, 3, 1); __PYX_ERR(0, 326, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("rename", 1, 3, 3, 1); __PYX_ERR(0, 329, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_newpath)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 326, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 329, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("rename", 1, 3, 3, 2); __PYX_ERR(0, 326, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("rename", 1, 3, 3, 2); __PYX_ERR(0, 329, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "rename") < 0)) __PYX_ERR(0, 326, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "rename") < 0)) __PYX_ERR(0, 329, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
     __pyx_v_oldpath = values[1];
     __pyx_v_newpath = values[2];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("rename", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 326, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("rename", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 329, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.rename", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 326, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 329, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_16rename(__pyx_self, __pyx_v_fs, __pyx_v_oldpath, __pyx_v_newpath);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -23817,25 +23806,25 @@
   PyObject *__pyx_t_7 = NULL;
   char const *__pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("rename", 1);
 
-  /* "littlefs/lfs.pyx":332
+  /* "littlefs/lfs.pyx":335
  *     If the destination is a directory, the directory must be empty.
  *     """
  *     return _raise_on_error(lfs_rename(&fs._impl, oldpath.encode(FILENAME_ENCODING),             # <<<<<<<<<<<<<<
  *                                         newpath.encode(FILENAME_ENCODING)))
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_oldpath, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 332, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_oldpath, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 335, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FILENAME_ENCODING); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 332, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FILENAME_ENCODING); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 335, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
@@ -23848,30 +23837,30 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_3};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 332, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 335, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_t_6 = __Pyx_PyObject_AsString(__pyx_t_1); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 332, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_AsString(__pyx_t_1); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 335, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":333
+  /* "littlefs/lfs.pyx":336
  *     """
  *     return _raise_on_error(lfs_rename(&fs._impl, oldpath.encode(FILENAME_ENCODING),
  *                                         newpath.encode(FILENAME_ENCODING)))             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_newpath, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 333, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_newpath, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 336, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FILENAME_ENCODING); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 333, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FILENAME_ENCODING); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 336, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_7 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_7)) {
@@ -23884,37 +23873,37 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_4};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 333, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 336, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_t_2); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 333, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_t_2); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 336, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":332
+  /* "littlefs/lfs.pyx":335
  *     If the destination is a directory, the directory must be empty.
  *     """
  *     return _raise_on_error(lfs_rename(&fs._impl, oldpath.encode(FILENAME_ENCODING),             # <<<<<<<<<<<<<<
  *                                         newpath.encode(FILENAME_ENCODING)))
  * 
  */
-  __pyx_t_5 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_rename((&__pyx_v_fs->_impl), __pyx_t_6, __pyx_t_8)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 332, __pyx_L1_error)
+  __pyx_t_5 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_rename((&__pyx_v_fs->_impl), __pyx_t_6, __pyx_t_8)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 335, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 332, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 335, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":326
+  /* "littlefs/lfs.pyx":329
  *     return _raise_on_error(lfs_remove(&fs._impl, path.encode(FILENAME_ENCODING)))
  * 
  * def rename(LFSFilesystem fs, oldpath, newpath):             # <<<<<<<<<<<<<<
  *     """Rename or move a file or directory
  * 
  */
 
@@ -23929,15 +23918,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":336
+/* "littlefs/lfs.pyx":339
  * 
  * 
  * def stat(LFSFilesystem fs, path):             # <<<<<<<<<<<<<<
  *     """Find info about a file or directory"""
  *     cdef lfs_info * info = <lfs_info *>malloc(sizeof(lfs_info))
  */
 
@@ -23994,57 +23983,57 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 336, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 339, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_path)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 336, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 339, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("stat", 1, 2, 2, 1); __PYX_ERR(0, 336, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("stat", 1, 2, 2, 1); __PYX_ERR(0, 339, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "stat") < 0)) __PYX_ERR(0, 336, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "stat") < 0)) __PYX_ERR(0, 339, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
     __pyx_v_path = values[1];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("stat", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 336, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("stat", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 339, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.stat", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 336, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 339, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_18stat(__pyx_self, __pyx_v_fs, __pyx_v_path);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -24081,42 +24070,42 @@
   PyObject *__pyx_t_17 = NULL;
   PyObject *__pyx_t_18 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("stat", 1);
 
-  /* "littlefs/lfs.pyx":338
+  /* "littlefs/lfs.pyx":341
  * def stat(LFSFilesystem fs, path):
  *     """Find info about a file or directory"""
  *     cdef lfs_info * info = <lfs_info *>malloc(sizeof(lfs_info))             # <<<<<<<<<<<<<<
  *     try:
  *         _raise_on_error(lfs_stat(&fs._impl, path.encode(FILENAME_ENCODING), info))
  */
   __pyx_v_info = ((struct lfs_info *)malloc((sizeof(struct lfs_info))));
 
-  /* "littlefs/lfs.pyx":339
+  /* "littlefs/lfs.pyx":342
  *     """Find info about a file or directory"""
  *     cdef lfs_info * info = <lfs_info *>malloc(sizeof(lfs_info))
  *     try:             # <<<<<<<<<<<<<<
  *         _raise_on_error(lfs_stat(&fs._impl, path.encode(FILENAME_ENCODING), info))
  *         return LFSStat(info.type, info.size, info.name.decode(FILENAME_ENCODING))
  */
   /*try:*/ {
 
-    /* "littlefs/lfs.pyx":340
+    /* "littlefs/lfs.pyx":343
  *     cdef lfs_info * info = <lfs_info *>malloc(sizeof(lfs_info))
  *     try:
  *         _raise_on_error(lfs_stat(&fs._impl, path.encode(FILENAME_ENCODING), info))             # <<<<<<<<<<<<<<
  *         return LFSStat(info.type, info.size, info.name.decode(FILENAME_ENCODING))
  *     finally:
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_path, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 340, __pyx_L4_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_path, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 343, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FILENAME_ENCODING); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 340, __pyx_L4_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FILENAME_ENCODING); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 343, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
@@ -24129,42 +24118,42 @@
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_3};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 340, __pyx_L4_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 343, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
-    __pyx_t_6 = __Pyx_PyObject_AsString(__pyx_t_1); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 340, __pyx_L4_error)
-    __pyx_t_5 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_stat((&__pyx_v_fs->_impl), __pyx_t_6, __pyx_v_info)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 340, __pyx_L4_error)
+    __pyx_t_6 = __Pyx_PyObject_AsString(__pyx_t_1); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 343, __pyx_L4_error)
+    __pyx_t_5 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_stat((&__pyx_v_fs->_impl), __pyx_t_6, __pyx_v_info)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 343, __pyx_L4_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "littlefs/lfs.pyx":341
+    /* "littlefs/lfs.pyx":344
  *     try:
  *         _raise_on_error(lfs_stat(&fs._impl, path.encode(FILENAME_ENCODING), info))
  *         return LFSStat(info.type, info.size, info.name.decode(FILENAME_ENCODING))             # <<<<<<<<<<<<<<
  *     finally:
  *         free(info)
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LFSStat); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 341, __pyx_L4_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LFSStat); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 344, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyInt_From_uint8_t(__pyx_v_info->type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 341, __pyx_L4_error)
+    __pyx_t_3 = __Pyx_PyInt_From_uint8_t(__pyx_v_info->type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 344, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyInt_From_uint32_t(__pyx_v_info->size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 341, __pyx_L4_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint32_t(__pyx_v_info->size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 344, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_8 = __Pyx_PyObject_FromString(__pyx_v_info->name); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 341, __pyx_L4_error)
+    __pyx_t_8 = __Pyx_PyObject_FromString(__pyx_v_info->name); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 344, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_decode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 341, __pyx_L4_error)
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_decode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 344, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_FILENAME_ENCODING); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 341, __pyx_L4_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_FILENAME_ENCODING); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 344, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_10 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_9))) {
       __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
       if (likely(__pyx_t_10)) {
@@ -24177,15 +24166,15 @@
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_10, __pyx_t_8};
       __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 341, __pyx_L4_error)
+      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 344, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     }
     __pyx_t_9 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_2))) {
@@ -24202,24 +24191,24 @@
     {
       PyObject *__pyx_callargs[4] = {__pyx_t_9, __pyx_t_3, __pyx_t_4, __pyx_t_7};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 3+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 341, __pyx_L4_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 344, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L3_return;
   }
 
-  /* "littlefs/lfs.pyx":343
+  /* "littlefs/lfs.pyx":346
  *         return LFSStat(info.type, info.size, info.name.decode(FILENAME_ENCODING))
  *     finally:
  *         free(info)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*finally:*/ {
@@ -24268,15 +24257,15 @@
       free(__pyx_v_info);
       __pyx_r = __pyx_t_18;
       __pyx_t_18 = 0;
       goto __pyx_L0;
     }
   }
 
-  /* "littlefs/lfs.pyx":336
+  /* "littlefs/lfs.pyx":339
  * 
  * 
  * def stat(LFSFilesystem fs, path):             # <<<<<<<<<<<<<<
  *     """Find info about a file or directory"""
  *     cdef lfs_info * info = <lfs_info *>malloc(sizeof(lfs_info))
  */
 
@@ -24294,15 +24283,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":346
+/* "littlefs/lfs.pyx":349
  * 
  * 
  * def getattr(LFSFilesystem fs, path, typ):             # <<<<<<<<<<<<<<
  *     buf = bytearray(LFS_ATTR_MAX)
  *     cdef unsigned char[::1] buf_view = buf
  */
 
@@ -24362,69 +24351,69 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 346, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 349, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_path)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 346, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 349, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("getattr", 1, 3, 3, 1); __PYX_ERR(0, 346, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("getattr", 1, 3, 3, 1); __PYX_ERR(0, 349, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_typ)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 346, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 349, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("getattr", 1, 3, 3, 2); __PYX_ERR(0, 346, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("getattr", 1, 3, 3, 2); __PYX_ERR(0, 349, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "getattr") < 0)) __PYX_ERR(0, 346, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "getattr") < 0)) __PYX_ERR(0, 349, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
     __pyx_v_path = values[1];
     __pyx_v_typ = values[2];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("getattr", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 346, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("getattr", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 349, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.getattr", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 346, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 349, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_20getattr(__pyx_self, __pyx_v_fs, __pyx_v_path, __pyx_v_typ);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -24454,51 +24443,51 @@
   uint8_t __pyx_t_8;
   Py_ssize_t __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("getattr", 1);
 
-  /* "littlefs/lfs.pyx":347
+  /* "littlefs/lfs.pyx":350
  * 
  * def getattr(LFSFilesystem fs, path, typ):
  *     buf = bytearray(LFS_ATTR_MAX)             # <<<<<<<<<<<<<<
  *     cdef unsigned char[::1] buf_view = buf
  *     attr_size = _raise_on_error(lfs_getattr(&fs._impl, path.encode(FILENAME_ENCODING), typ, &buf_view[0], LFS_ATTR_MAX))
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(LFS_ATTR_MAX); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 347, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(LFS_ATTR_MAX); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 350, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 347, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 350, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_buf = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "littlefs/lfs.pyx":348
+  /* "littlefs/lfs.pyx":351
  * def getattr(LFSFilesystem fs, path, typ):
  *     buf = bytearray(LFS_ATTR_MAX)
  *     cdef unsigned char[::1] buf_view = buf             # <<<<<<<<<<<<<<
  *     attr_size = _raise_on_error(lfs_getattr(&fs._impl, path.encode(FILENAME_ENCODING), typ, &buf_view[0], LFS_ATTR_MAX))
  *     return bytes(buf[:attr_size])
  */
-  __pyx_t_3 = __Pyx_PyObject_to_MemoryviewSlice_dc_unsigned_char(__pyx_v_buf, PyBUF_WRITABLE); if (unlikely(!__pyx_t_3.memview)) __PYX_ERR(0, 348, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_to_MemoryviewSlice_dc_unsigned_char(__pyx_v_buf, PyBUF_WRITABLE); if (unlikely(!__pyx_t_3.memview)) __PYX_ERR(0, 351, __pyx_L1_error)
   __pyx_v_buf_view = __pyx_t_3;
   __pyx_t_3.memview = NULL;
   __pyx_t_3.data = NULL;
 
-  /* "littlefs/lfs.pyx":349
+  /* "littlefs/lfs.pyx":352
  *     buf = bytearray(LFS_ATTR_MAX)
  *     cdef unsigned char[::1] buf_view = buf
  *     attr_size = _raise_on_error(lfs_getattr(&fs._impl, path.encode(FILENAME_ENCODING), typ, &buf_view[0], LFS_ATTR_MAX))             # <<<<<<<<<<<<<<
  *     return bytes(buf[:attr_size])
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_path, __pyx_n_s_encode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 349, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_path, __pyx_n_s_encode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 352, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FILENAME_ENCODING); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 349, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FILENAME_ENCODING); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 352, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_5)) {
@@ -24511,52 +24500,52 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_4};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 349, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 352, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
-  __pyx_t_7 = __Pyx_PyObject_AsString(__pyx_t_2); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 349, __pyx_L1_error)
-  __pyx_t_8 = __Pyx_PyInt_As_uint8_t(__pyx_v_typ); if (unlikely((__pyx_t_8 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 349, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_AsString(__pyx_t_2); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 352, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_As_uint8_t(__pyx_v_typ); if (unlikely((__pyx_t_8 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 352, __pyx_L1_error)
   __pyx_t_9 = 0;
   __pyx_t_6 = -1;
   if (__pyx_t_9 < 0) {
     __pyx_t_9 += __pyx_v_buf_view.shape[0];
     if (unlikely(__pyx_t_9 < 0)) __pyx_t_6 = 0;
   } else if (unlikely(__pyx_t_9 >= __pyx_v_buf_view.shape[0])) __pyx_t_6 = 0;
   if (unlikely(__pyx_t_6 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_6);
-    __PYX_ERR(0, 349, __pyx_L1_error)
+    __PYX_ERR(0, 352, __pyx_L1_error)
   }
-  __pyx_t_6 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_getattr((&__pyx_v_fs->_impl), __pyx_t_7, __pyx_t_8, (&(*((unsigned char *) ( /* dim=0 */ ((char *) (((unsigned char *) __pyx_v_buf_view.data) + __pyx_t_9)) )))), LFS_ATTR_MAX)); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 349, __pyx_L1_error)
+  __pyx_t_6 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_getattr((&__pyx_v_fs->_impl), __pyx_t_7, __pyx_t_8, (&(*((unsigned char *) ( /* dim=0 */ ((char *) (((unsigned char *) __pyx_v_buf_view.data) + __pyx_t_9)) )))), LFS_ATTR_MAX)); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 352, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_attr_size = __pyx_t_6;
 
-  /* "littlefs/lfs.pyx":350
+  /* "littlefs/lfs.pyx":353
  *     cdef unsigned char[::1] buf_view = buf
  *     attr_size = _raise_on_error(lfs_getattr(&fs._impl, path.encode(FILENAME_ENCODING), typ, &buf_view[0], LFS_ATTR_MAX))
  *     return bytes(buf[:attr_size])             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PySequence_GetSlice(__pyx_v_buf, 0, __pyx_v_attr_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 350, __pyx_L1_error)
+  __pyx_t_2 = PySequence_GetSlice(__pyx_v_buf, 0, __pyx_v_attr_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 353, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 350, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 353, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":346
+  /* "littlefs/lfs.pyx":349
  * 
  * 
  * def getattr(LFSFilesystem fs, path, typ):             # <<<<<<<<<<<<<<
  *     buf = bytearray(LFS_ATTR_MAX)
  *     cdef unsigned char[::1] buf_view = buf
  */
 
@@ -24573,15 +24562,15 @@
   __Pyx_XDECREF(__pyx_v_buf);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_buf_view, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":353
+/* "littlefs/lfs.pyx":356
  * 
  * 
  * def setattr(LFSFilesystem fs, path, typ, data):             # <<<<<<<<<<<<<<
  *     cdef const unsigned char[::1] buf_view = data
  *     _raise_on_error(lfs_setattr(&fs._impl, path.encode(FILENAME_ENCODING), typ, &buf_view[0], len(data)))
  */
 
@@ -24644,50 +24633,50 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 353, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 356, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_path)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 353, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 356, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("setattr", 1, 4, 4, 1); __PYX_ERR(0, 353, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("setattr", 1, 4, 4, 1); __PYX_ERR(0, 356, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_typ)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 353, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 356, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("setattr", 1, 4, 4, 2); __PYX_ERR(0, 353, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("setattr", 1, 4, 4, 2); __PYX_ERR(0, 356, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_data)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 353, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 356, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("setattr", 1, 4, 4, 3); __PYX_ERR(0, 353, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("setattr", 1, 4, 4, 3); __PYX_ERR(0, 356, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "setattr") < 0)) __PYX_ERR(0, 353, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "setattr") < 0)) __PYX_ERR(0, 356, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 4)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
@@ -24696,29 +24685,29 @@
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
     __pyx_v_path = values[1];
     __pyx_v_typ = values[2];
     __pyx_v_data = values[3];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("setattr", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 353, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("setattr", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 356, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.setattr", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 353, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 356, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_22setattr(__pyx_self, __pyx_v_fs, __pyx_v_path, __pyx_v_typ, __pyx_v_data);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -24747,36 +24736,36 @@
   Py_ssize_t __pyx_t_9;
   Py_ssize_t __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("setattr", 1);
 
-  /* "littlefs/lfs.pyx":354
+  /* "littlefs/lfs.pyx":357
  * 
  * def setattr(LFSFilesystem fs, path, typ, data):
  *     cdef const unsigned char[::1] buf_view = data             # <<<<<<<<<<<<<<
  *     _raise_on_error(lfs_setattr(&fs._impl, path.encode(FILENAME_ENCODING), typ, &buf_view[0], len(data)))
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_to_MemoryviewSlice_dc_unsigned_char__const__(__pyx_v_data, 0); if (unlikely(!__pyx_t_1.memview)) __PYX_ERR(0, 354, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_to_MemoryviewSlice_dc_unsigned_char__const__(__pyx_v_data, 0); if (unlikely(!__pyx_t_1.memview)) __PYX_ERR(0, 357, __pyx_L1_error)
   __pyx_v_buf_view = __pyx_t_1;
   __pyx_t_1.memview = NULL;
   __pyx_t_1.data = NULL;
 
-  /* "littlefs/lfs.pyx":355
+  /* "littlefs/lfs.pyx":358
  * def setattr(LFSFilesystem fs, path, typ, data):
  *     cdef const unsigned char[::1] buf_view = data
  *     _raise_on_error(lfs_setattr(&fs._impl, path.encode(FILENAME_ENCODING), typ, &buf_view[0], len(data)))             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_path, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_path, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 358, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FILENAME_ENCODING); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 355, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FILENAME_ENCODING); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 358, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
@@ -24789,35 +24778,35 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_4};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 355, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 358, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_t_7 = __Pyx_PyObject_AsString(__pyx_t_2); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 355, __pyx_L1_error)
-  __pyx_t_8 = __Pyx_PyInt_As_uint8_t(__pyx_v_typ); if (unlikely((__pyx_t_8 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_AsString(__pyx_t_2); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 358, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_As_uint8_t(__pyx_v_typ); if (unlikely((__pyx_t_8 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 358, __pyx_L1_error)
   __pyx_t_9 = 0;
   __pyx_t_6 = -1;
   if (__pyx_t_9 < 0) {
     __pyx_t_9 += __pyx_v_buf_view.shape[0];
     if (unlikely(__pyx_t_9 < 0)) __pyx_t_6 = 0;
   } else if (unlikely(__pyx_t_9 >= __pyx_v_buf_view.shape[0])) __pyx_t_6 = 0;
   if (unlikely(__pyx_t_6 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_6);
-    __PYX_ERR(0, 355, __pyx_L1_error)
+    __PYX_ERR(0, 358, __pyx_L1_error)
   }
-  __pyx_t_10 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1))) __PYX_ERR(0, 355, __pyx_L1_error)
-  __pyx_t_6 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_setattr((&__pyx_v_fs->_impl), __pyx_t_7, __pyx_t_8, (&(*((unsigned char const  *) ( /* dim=0 */ ((char *) (((unsigned char const  *) __pyx_v_buf_view.data) + __pyx_t_9)) )))), __pyx_t_10)); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_t_10 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1))) __PYX_ERR(0, 358, __pyx_L1_error)
+  __pyx_t_6 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_setattr((&__pyx_v_fs->_impl), __pyx_t_7, __pyx_t_8, (&(*((unsigned char const  *) ( /* dim=0 */ ((char *) (((unsigned char const  *) __pyx_v_buf_view.data) + __pyx_t_9)) )))), __pyx_t_10)); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 358, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "littlefs/lfs.pyx":353
+  /* "littlefs/lfs.pyx":356
  * 
  * 
  * def setattr(LFSFilesystem fs, path, typ, data):             # <<<<<<<<<<<<<<
  *     cdef const unsigned char[::1] buf_view = data
  *     _raise_on_error(lfs_setattr(&fs._impl, path.encode(FILENAME_ENCODING), typ, &buf_view[0], len(data)))
  */
 
@@ -24835,15 +24824,15 @@
   __pyx_L0:;
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_buf_view, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":358
+/* "littlefs/lfs.pyx":361
  * 
  * 
  * def removeattr(LFSFilesystem fs, path, typ):             # <<<<<<<<<<<<<<
  *     _raise_on_error(lfs_removeattr(&fs._impl, path.encode(FILENAME_ENCODING), typ))
  * 
  */
 
@@ -24903,69 +24892,69 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 358, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 361, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_path)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 358, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 361, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("removeattr", 1, 3, 3, 1); __PYX_ERR(0, 358, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("removeattr", 1, 3, 3, 1); __PYX_ERR(0, 361, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_typ)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 358, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 361, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("removeattr", 1, 3, 3, 2); __PYX_ERR(0, 358, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("removeattr", 1, 3, 3, 2); __PYX_ERR(0, 361, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "removeattr") < 0)) __PYX_ERR(0, 358, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "removeattr") < 0)) __PYX_ERR(0, 361, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
     __pyx_v_path = values[1];
     __pyx_v_typ = values[2];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("removeattr", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 358, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("removeattr", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 361, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.removeattr", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 358, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 361, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_24removeattr(__pyx_self, __pyx_v_fs, __pyx_v_path, __pyx_v_typ);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -24990,24 +24979,24 @@
   char const *__pyx_t_6;
   uint8_t __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("removeattr", 1);
 
-  /* "littlefs/lfs.pyx":359
+  /* "littlefs/lfs.pyx":362
  * 
  * def removeattr(LFSFilesystem fs, path, typ):
  *     _raise_on_error(lfs_removeattr(&fs._impl, path.encode(FILENAME_ENCODING), typ))             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_path, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 359, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_path, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 362, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FILENAME_ENCODING); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 359, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FILENAME_ENCODING); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 362, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
@@ -25020,24 +25009,24 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_3};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 359, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 362, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_t_6 = __Pyx_PyObject_AsString(__pyx_t_1); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 359, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyInt_As_uint8_t(__pyx_v_typ); if (unlikely((__pyx_t_7 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 359, __pyx_L1_error)
-  __pyx_t_5 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_removeattr((&__pyx_v_fs->_impl), __pyx_t_6, __pyx_t_7)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 359, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_AsString(__pyx_t_1); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 362, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_As_uint8_t(__pyx_v_typ); if (unlikely((__pyx_t_7 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 362, __pyx_L1_error)
+  __pyx_t_5 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_removeattr((&__pyx_v_fs->_impl), __pyx_t_6, __pyx_t_7)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 362, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "littlefs/lfs.pyx":358
+  /* "littlefs/lfs.pyx":361
  * 
  * 
  * def removeattr(LFSFilesystem fs, path, typ):             # <<<<<<<<<<<<<<
  *     _raise_on_error(lfs_removeattr(&fs._impl, path.encode(FILENAME_ENCODING), typ))
  * 
  */
 
@@ -25053,15 +25042,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":362
+/* "littlefs/lfs.pyx":365
  * 
  * 
  * def file_open(LFSFilesystem fs, path, flags):             # <<<<<<<<<<<<<<
  *     if isinstance(flags, str):
  *         creating = False
  */
 
@@ -25121,69 +25110,69 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 362, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 365, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_path)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 362, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 365, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("file_open", 1, 3, 3, 1); __PYX_ERR(0, 362, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("file_open", 1, 3, 3, 1); __PYX_ERR(0, 365, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_flags)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 362, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 365, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("file_open", 1, 3, 3, 2); __PYX_ERR(0, 362, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("file_open", 1, 3, 3, 2); __PYX_ERR(0, 365, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "file_open") < 0)) __PYX_ERR(0, 362, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "file_open") < 0)) __PYX_ERR(0, 365, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
     __pyx_v_path = values[1];
     __pyx_v_flags = values[2];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("file_open", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 362, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("file_open", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 365, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.file_open", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 362, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 365, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_26file_open(__pyx_self, __pyx_v_fs, __pyx_v_path, __pyx_v_flags);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -25194,15 +25183,15 @@
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_8littlefs_3lfs_9file_open_2generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "littlefs/lfs.pyx":390
+/* "littlefs/lfs.pyx":393
  *         exclusive_modes = (creating, reading, writing, appending)
  * 
  *         if sum(int(m) for m in exclusive_modes) > 1:             # <<<<<<<<<<<<<<
  *             raise ValueError(
  *                 "must have exactly one of create/read/write/append mode"
  */
 
@@ -25214,23 +25203,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_8littlefs_3lfs___pyx_scope_struct__genexpr *)__pyx_tp_new_8littlefs_3lfs___pyx_scope_struct__genexpr(__pyx_ptype_8littlefs_3lfs___pyx_scope_struct__genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_8littlefs_3lfs___pyx_scope_struct__genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 390, __pyx_L1_error)
+    __PYX_ERR(0, 393, __pyx_L1_error)
   } else {
     __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_genexpr_arg_0 = __pyx_genexpr_arg_0;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_8littlefs_3lfs_9file_open_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_file_open_locals_genexpr, __pyx_n_s_littlefs_lfs); if (unlikely(!gen)) __PYX_ERR(0, 390, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_8littlefs_3lfs_9file_open_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_file_open_locals_genexpr, __pyx_n_s_littlefs_lfs); if (unlikely(!gen)) __PYX_ERR(0, 393, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -25259,73 +25248,73 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L6_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 390, __pyx_L1_error)
-  if (unlikely(!__pyx_cur_scope->__pyx_genexpr_arg_0)) { __Pyx_RaiseUnboundLocalError(".0"); __PYX_ERR(0, 390, __pyx_L1_error) }
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 393, __pyx_L1_error)
+  if (unlikely(!__pyx_cur_scope->__pyx_genexpr_arg_0)) { __Pyx_RaiseUnboundLocalError(".0"); __PYX_ERR(0, 393, __pyx_L1_error) }
   if (likely(PyList_CheckExact(__pyx_cur_scope->__pyx_genexpr_arg_0)) || PyTuple_CheckExact(__pyx_cur_scope->__pyx_genexpr_arg_0)) {
     __pyx_t_1 = __pyx_cur_scope->__pyx_genexpr_arg_0; __Pyx_INCREF(__pyx_t_1);
     __pyx_t_2 = 0;
     __pyx_t_3 = NULL;
   } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_genexpr_arg_0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 390, __pyx_L1_error)
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_genexpr_arg_0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 390, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 393, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_3)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 390, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 393, __pyx_L1_error)
           #endif
           if (__pyx_t_2 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 390, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 393, __pyx_L1_error)
         #else
-        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 390, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 393, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_1);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 390, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 393, __pyx_L1_error)
           #endif
           if (__pyx_t_2 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 390, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 393, __pyx_L1_error)
         #else
-        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 390, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 393, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_3(__pyx_t_1);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 390, __pyx_L1_error)
+          else __PYX_ERR(0, 393, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_m);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_m, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_cur_scope->__pyx_v_m); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 390, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_cur_scope->__pyx_v_m); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 393, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     __Pyx_XGIVEREF(__pyx_t_1);
     __pyx_cur_scope->__pyx_t_0 = __pyx_t_1;
     __pyx_cur_scope->__pyx_t_1 = __pyx_t_2;
     __pyx_cur_scope->__pyx_t_2 = __pyx_t_3;
@@ -25337,15 +25326,15 @@
     return __pyx_r;
     __pyx_L6_resume_from_yield:;
     __pyx_t_1 = __pyx_cur_scope->__pyx_t_0;
     __pyx_cur_scope->__pyx_t_0 = 0;
     __Pyx_XGOTREF(__pyx_t_1);
     __pyx_t_2 = __pyx_cur_scope->__pyx_t_1;
     __pyx_t_3 = __pyx_cur_scope->__pyx_t_2;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 390, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 393, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* function exit code */
   PyErr_SetNone(PyExc_StopIteration);
   goto __pyx_L0;
@@ -25361,15 +25350,15 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":362
+/* "littlefs/lfs.pyx":365
  * 
  * 
  * def file_open(LFSFilesystem fs, path, flags):             # <<<<<<<<<<<<<<
  *     if isinstance(flags, str):
  *         creating = False
  */
 
@@ -25401,681 +25390,681 @@
   int __pyx_t_14;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("file_open", 0);
   __Pyx_INCREF(__pyx_v_flags);
 
-  /* "littlefs/lfs.pyx":363
+  /* "littlefs/lfs.pyx":366
  * 
  * def file_open(LFSFilesystem fs, path, flags):
  *     if isinstance(flags, str):             # <<<<<<<<<<<<<<
  *         creating = False
  *         reading = False
  */
   __pyx_t_1 = PyUnicode_Check(__pyx_v_flags); 
   if (__pyx_t_1) {
 
-    /* "littlefs/lfs.pyx":364
+    /* "littlefs/lfs.pyx":367
  * def file_open(LFSFilesystem fs, path, flags):
  *     if isinstance(flags, str):
  *         creating = False             # <<<<<<<<<<<<<<
  *         reading = False
  *         writing = False
  */
     __pyx_v_creating = 0;
 
-    /* "littlefs/lfs.pyx":365
+    /* "littlefs/lfs.pyx":368
  *     if isinstance(flags, str):
  *         creating = False
  *         reading = False             # <<<<<<<<<<<<<<
  *         writing = False
  *         appending = False
  */
     __pyx_v_reading = 0;
 
-    /* "littlefs/lfs.pyx":366
+    /* "littlefs/lfs.pyx":369
  *         creating = False
  *         reading = False
  *         writing = False             # <<<<<<<<<<<<<<
  *         appending = False
  *         updating = False
  */
     __pyx_v_writing = 0;
 
-    /* "littlefs/lfs.pyx":367
+    /* "littlefs/lfs.pyx":370
  *         reading = False
  *         writing = False
  *         appending = False             # <<<<<<<<<<<<<<
  *         updating = False
  * 
  */
     __pyx_v_appending = 0;
 
-    /* "littlefs/lfs.pyx":368
+    /* "littlefs/lfs.pyx":371
  *         writing = False
  *         appending = False
  *         updating = False             # <<<<<<<<<<<<<<
  * 
  *         for ch in flags:
  */
     __pyx_v_updating = 0;
 
-    /* "littlefs/lfs.pyx":370
+    /* "littlefs/lfs.pyx":373
  *         updating = False
  * 
  *         for ch in flags:             # <<<<<<<<<<<<<<
  *             if ch == "x":
  *                 creating = True
  */
     if (likely(PyList_CheckExact(__pyx_v_flags)) || PyTuple_CheckExact(__pyx_v_flags)) {
       __pyx_t_2 = __pyx_v_flags; __Pyx_INCREF(__pyx_t_2);
       __pyx_t_3 = 0;
       __pyx_t_4 = NULL;
     } else {
-      __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_flags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 370, __pyx_L1_error)
+      __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_flags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 373, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 370, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 373, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_4)) {
         if (likely(PyList_CheckExact(__pyx_t_2))) {
           {
             Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 370, __pyx_L1_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 373, __pyx_L1_error)
             #endif
             if (__pyx_t_3 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 370, __pyx_L1_error)
+          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 373, __pyx_L1_error)
           #else
-          __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 370, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 373, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         } else {
           {
             Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 370, __pyx_L1_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 373, __pyx_L1_error)
             #endif
             if (__pyx_t_3 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 370, __pyx_L1_error)
+          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 373, __pyx_L1_error)
           #else
-          __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 370, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 373, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         }
       } else {
         __pyx_t_5 = __pyx_t_4(__pyx_t_2);
         if (unlikely(!__pyx_t_5)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 370, __pyx_L1_error)
+            else __PYX_ERR(0, 373, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_5);
       }
       __Pyx_XDECREF_SET(__pyx_v_ch, __pyx_t_5);
       __pyx_t_5 = 0;
 
-      /* "littlefs/lfs.pyx":371
+      /* "littlefs/lfs.pyx":374
  * 
  *         for ch in flags:
  *             if ch == "x":             # <<<<<<<<<<<<<<
  *                 creating = True
  *             elif ch == "r":
  */
-      __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_ch, __pyx_n_u_x, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 371, __pyx_L1_error)
+      __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_ch, __pyx_n_u_x, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 374, __pyx_L1_error)
       if (__pyx_t_1) {
 
-        /* "littlefs/lfs.pyx":372
+        /* "littlefs/lfs.pyx":375
  *         for ch in flags:
  *             if ch == "x":
  *                 creating = True             # <<<<<<<<<<<<<<
  *             elif ch == "r":
  *                 reading = True
  */
         __pyx_v_creating = 1;
 
-        /* "littlefs/lfs.pyx":371
+        /* "littlefs/lfs.pyx":374
  * 
  *         for ch in flags:
  *             if ch == "x":             # <<<<<<<<<<<<<<
  *                 creating = True
  *             elif ch == "r":
  */
         goto __pyx_L6;
       }
 
-      /* "littlefs/lfs.pyx":373
+      /* "littlefs/lfs.pyx":376
  *             if ch == "x":
  *                 creating = True
  *             elif ch == "r":             # <<<<<<<<<<<<<<
  *                 reading = True
  *             elif ch == "w":
  */
-      __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_ch, __pyx_n_u_r, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 373, __pyx_L1_error)
+      __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_ch, __pyx_n_u_r, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 376, __pyx_L1_error)
       if (__pyx_t_1) {
 
-        /* "littlefs/lfs.pyx":374
+        /* "littlefs/lfs.pyx":377
  *                 creating = True
  *             elif ch == "r":
  *                 reading = True             # <<<<<<<<<<<<<<
  *             elif ch == "w":
  *                 writing = True
  */
         __pyx_v_reading = 1;
 
-        /* "littlefs/lfs.pyx":373
+        /* "littlefs/lfs.pyx":376
  *             if ch == "x":
  *                 creating = True
  *             elif ch == "r":             # <<<<<<<<<<<<<<
  *                 reading = True
  *             elif ch == "w":
  */
         goto __pyx_L6;
       }
 
-      /* "littlefs/lfs.pyx":375
+      /* "littlefs/lfs.pyx":378
  *             elif ch == "r":
  *                 reading = True
  *             elif ch == "w":             # <<<<<<<<<<<<<<
  *                 writing = True
  *             elif ch == "a":
  */
-      __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_ch, __pyx_n_u_w, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 375, __pyx_L1_error)
+      __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_ch, __pyx_n_u_w, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 378, __pyx_L1_error)
       if (__pyx_t_1) {
 
-        /* "littlefs/lfs.pyx":376
+        /* "littlefs/lfs.pyx":379
  *                 reading = True
  *             elif ch == "w":
  *                 writing = True             # <<<<<<<<<<<<<<
  *             elif ch == "a":
  *                 appending = True
  */
         __pyx_v_writing = 1;
 
-        /* "littlefs/lfs.pyx":375
+        /* "littlefs/lfs.pyx":378
  *             elif ch == "r":
  *                 reading = True
  *             elif ch == "w":             # <<<<<<<<<<<<<<
  *                 writing = True
  *             elif ch == "a":
  */
         goto __pyx_L6;
       }
 
-      /* "littlefs/lfs.pyx":377
+      /* "littlefs/lfs.pyx":380
  *             elif ch == "w":
  *                 writing = True
  *             elif ch == "a":             # <<<<<<<<<<<<<<
  *                 appending = True
  *             elif ch == "+":
  */
-      __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_ch, __pyx_n_u_a, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 377, __pyx_L1_error)
+      __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_ch, __pyx_n_u_a, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 380, __pyx_L1_error)
       if (__pyx_t_1) {
 
-        /* "littlefs/lfs.pyx":378
+        /* "littlefs/lfs.pyx":381
  *                 writing = True
  *             elif ch == "a":
  *                 appending = True             # <<<<<<<<<<<<<<
  *             elif ch == "+":
  *                 updating = True
  */
         __pyx_v_appending = 1;
 
-        /* "littlefs/lfs.pyx":377
+        /* "littlefs/lfs.pyx":380
  *             elif ch == "w":
  *                 writing = True
  *             elif ch == "a":             # <<<<<<<<<<<<<<
  *                 appending = True
  *             elif ch == "+":
  */
         goto __pyx_L6;
       }
 
-      /* "littlefs/lfs.pyx":379
+      /* "littlefs/lfs.pyx":382
  *             elif ch == "a":
  *                 appending = True
  *             elif ch == "+":             # <<<<<<<<<<<<<<
  *                 updating = True
  *             elif ch in ("t", "b"):
  */
-      __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_ch, __pyx_kp_u__25, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 379, __pyx_L1_error)
+      __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_ch, __pyx_kp_u__25, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 382, __pyx_L1_error)
       if (__pyx_t_1) {
 
-        /* "littlefs/lfs.pyx":380
+        /* "littlefs/lfs.pyx":383
  *                 appending = True
  *             elif ch == "+":
  *                 updating = True             # <<<<<<<<<<<<<<
  *             elif ch in ("t", "b"):
  *                 # lfs_file_open() always opens files in binary mode.
  */
         __pyx_v_updating = 1;
 
-        /* "littlefs/lfs.pyx":379
+        /* "littlefs/lfs.pyx":382
  *             elif ch == "a":
  *                 appending = True
  *             elif ch == "+":             # <<<<<<<<<<<<<<
  *                 updating = True
  *             elif ch in ("t", "b"):
  */
         goto __pyx_L6;
       }
 
-      /* "littlefs/lfs.pyx":381
+      /* "littlefs/lfs.pyx":384
  *             elif ch == "+":
  *                 updating = True
  *             elif ch in ("t", "b"):             # <<<<<<<<<<<<<<
  *                 # lfs_file_open() always opens files in binary mode.
  *                 # Text decoding is done at a higher level.
  */
       __Pyx_INCREF(__pyx_v_ch);
       __pyx_t_5 = __pyx_v_ch;
-      __pyx_t_6 = (__Pyx_PyUnicode_Equals(__pyx_t_5, __pyx_n_u_t, Py_EQ)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 381, __pyx_L1_error)
+      __pyx_t_6 = (__Pyx_PyUnicode_Equals(__pyx_t_5, __pyx_n_u_t, Py_EQ)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 384, __pyx_L1_error)
       if (!__pyx_t_6) {
       } else {
         __pyx_t_1 = __pyx_t_6;
         goto __pyx_L7_bool_binop_done;
       }
-      __pyx_t_6 = (__Pyx_PyUnicode_Equals(__pyx_t_5, __pyx_n_u_b, Py_EQ)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 381, __pyx_L1_error)
+      __pyx_t_6 = (__Pyx_PyUnicode_Equals(__pyx_t_5, __pyx_n_u_b, Py_EQ)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 384, __pyx_L1_error)
       __pyx_t_1 = __pyx_t_6;
       __pyx_L7_bool_binop_done:;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_6 = __pyx_t_1;
       if (likely(__pyx_t_6)) {
         goto __pyx_L6;
       }
 
-      /* "littlefs/lfs.pyx":386
+      /* "littlefs/lfs.pyx":389
  *                 pass
  *             else:
  *                 raise ValueError(f"invalid mode: '{flags}'")             # <<<<<<<<<<<<<<
  * 
  *         exclusive_modes = (creating, reading, writing, appending)
  */
       /*else*/ {
-        __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 386, __pyx_L1_error)
+        __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 389, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __pyx_t_7 = 0;
         __pyx_t_8 = 127;
         __Pyx_INCREF(__pyx_kp_u_invalid_mode);
         __pyx_t_7 += 15;
         __Pyx_GIVEREF(__pyx_kp_u_invalid_mode);
         PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_kp_u_invalid_mode);
-        __pyx_t_9 = __Pyx_PyObject_FormatSimple(__pyx_v_flags, __pyx_empty_unicode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 386, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyObject_FormatSimple(__pyx_v_flags, __pyx_empty_unicode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 389, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         __pyx_t_8 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_9) > __pyx_t_8) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_9) : __pyx_t_8;
         __pyx_t_7 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_9);
         __Pyx_GIVEREF(__pyx_t_9);
         PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_9);
         __pyx_t_9 = 0;
         __Pyx_INCREF(__pyx_kp_u__6);
         __pyx_t_7 += 1;
         __Pyx_GIVEREF(__pyx_kp_u__6);
         PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_kp_u__6);
-        __pyx_t_9 = __Pyx_PyUnicode_Join(__pyx_t_5, 3, __pyx_t_7, __pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 386, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyUnicode_Join(__pyx_t_5, 3, __pyx_t_7, __pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 389, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 386, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 389, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_Raise(__pyx_t_5, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __PYX_ERR(0, 386, __pyx_L1_error)
+        __PYX_ERR(0, 389, __pyx_L1_error)
       }
       __pyx_L6:;
 
-      /* "littlefs/lfs.pyx":370
+      /* "littlefs/lfs.pyx":373
  *         updating = False
  * 
  *         for ch in flags:             # <<<<<<<<<<<<<<
  *             if ch == "x":
  *                 creating = True
  */
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "littlefs/lfs.pyx":388
+    /* "littlefs/lfs.pyx":391
  *                 raise ValueError(f"invalid mode: '{flags}'")
  * 
  *         exclusive_modes = (creating, reading, writing, appending)             # <<<<<<<<<<<<<<
  * 
  *         if sum(int(m) for m in exclusive_modes) > 1:
  */
-    __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_creating); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 388, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_creating); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 391, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_5 = __Pyx_PyBool_FromLong(__pyx_v_reading); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 388, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyBool_FromLong(__pyx_v_reading); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 391, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_9 = __Pyx_PyBool_FromLong(__pyx_v_writing); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 388, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyBool_FromLong(__pyx_v_writing); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 391, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_10 = __Pyx_PyBool_FromLong(__pyx_v_appending); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 388, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyBool_FromLong(__pyx_v_appending); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 391, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    __pyx_t_11 = PyTuple_New(4); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 388, __pyx_L1_error)
+    __pyx_t_11 = PyTuple_New(4); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 391, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __Pyx_GIVEREF(__pyx_t_2);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_2)) __PYX_ERR(0, 388, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_2)) __PYX_ERR(0, 391, __pyx_L1_error);
     __Pyx_GIVEREF(__pyx_t_5);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_t_5)) __PYX_ERR(0, 388, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_t_5)) __PYX_ERR(0, 391, __pyx_L1_error);
     __Pyx_GIVEREF(__pyx_t_9);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 2, __pyx_t_9)) __PYX_ERR(0, 388, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 2, __pyx_t_9)) __PYX_ERR(0, 391, __pyx_L1_error);
     __Pyx_GIVEREF(__pyx_t_10);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 3, __pyx_t_10)) __PYX_ERR(0, 388, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 3, __pyx_t_10)) __PYX_ERR(0, 391, __pyx_L1_error);
     __pyx_t_2 = 0;
     __pyx_t_5 = 0;
     __pyx_t_9 = 0;
     __pyx_t_10 = 0;
     __pyx_v_exclusive_modes = __pyx_t_11;
     __pyx_t_11 = 0;
 
-    /* "littlefs/lfs.pyx":390
+    /* "littlefs/lfs.pyx":393
  *         exclusive_modes = (creating, reading, writing, appending)
  * 
  *         if sum(int(m) for m in exclusive_modes) > 1:             # <<<<<<<<<<<<<<
  *             raise ValueError(
  *                 "must have exactly one of create/read/write/append mode"
  */
-    __pyx_t_11 = __pyx_pf_8littlefs_3lfs_9file_open_genexpr(NULL, __pyx_v_exclusive_modes); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 390, __pyx_L1_error)
+    __pyx_t_11 = __pyx_pf_8littlefs_3lfs_9file_open_genexpr(NULL, __pyx_v_exclusive_modes); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 393, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
-    __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_builtin_sum, __pyx_t_11); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 390, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_builtin_sum, __pyx_t_11); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 393, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-    __pyx_t_11 = PyObject_RichCompare(__pyx_t_10, __pyx_int_1, Py_GT); __Pyx_XGOTREF(__pyx_t_11); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 390, __pyx_L1_error)
+    __pyx_t_11 = PyObject_RichCompare(__pyx_t_10, __pyx_int_1, Py_GT); __Pyx_XGOTREF(__pyx_t_11); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 393, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_11); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 390, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_11); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 393, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     if (unlikely(__pyx_t_6)) {
 
-      /* "littlefs/lfs.pyx":391
+      /* "littlefs/lfs.pyx":394
  * 
  *         if sum(int(m) for m in exclusive_modes) > 1:
  *             raise ValueError(             # <<<<<<<<<<<<<<
  *                 "must have exactly one of create/read/write/append mode"
  *             )
  */
-      __pyx_t_11 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 391, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 394, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_Raise(__pyx_t_11, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      __PYX_ERR(0, 391, __pyx_L1_error)
+      __PYX_ERR(0, 394, __pyx_L1_error)
 
-      /* "littlefs/lfs.pyx":390
+      /* "littlefs/lfs.pyx":393
  *         exclusive_modes = (creating, reading, writing, appending)
  * 
  *         if sum(int(m) for m in exclusive_modes) > 1:             # <<<<<<<<<<<<<<
  *             raise ValueError(
  *                 "must have exactly one of create/read/write/append mode"
  */
     }
 
-    /* "littlefs/lfs.pyx":395
+    /* "littlefs/lfs.pyx":398
  *             )
  * 
  *         if creating:             # <<<<<<<<<<<<<<
  *             flags = LFSFileFlag.creat | LFSFileFlag.excl | LFSFileFlag.wronly
  *         elif reading:
  */
     if (__pyx_v_creating) {
 
-      /* "littlefs/lfs.pyx":396
+      /* "littlefs/lfs.pyx":399
  * 
  *         if creating:
  *             flags = LFSFileFlag.creat | LFSFileFlag.excl | LFSFileFlag.wronly             # <<<<<<<<<<<<<<
  *         elif reading:
  *             flags = LFSFileFlag.rdonly
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_LFSFileFlag); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 396, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_LFSFileFlag); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 399, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
-      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_creat); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 396, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_creat); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 399, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_LFSFileFlag); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 396, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_LFSFileFlag); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 399, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_excl); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 396, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_excl); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 399, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      __pyx_t_11 = PyNumber_Or(__pyx_t_10, __pyx_t_9); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 396, __pyx_L1_error)
+      __pyx_t_11 = PyNumber_Or(__pyx_t_10, __pyx_t_9); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 399, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_LFSFileFlag); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 396, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_LFSFileFlag); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 399, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_wronly); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 396, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_wronly); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 399, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      __pyx_t_9 = PyNumber_Or(__pyx_t_11, __pyx_t_10); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 396, __pyx_L1_error)
+      __pyx_t_9 = PyNumber_Or(__pyx_t_11, __pyx_t_10); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 399, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_DECREF_SET(__pyx_v_flags, __pyx_t_9);
       __pyx_t_9 = 0;
 
-      /* "littlefs/lfs.pyx":395
+      /* "littlefs/lfs.pyx":398
  *             )
  * 
  *         if creating:             # <<<<<<<<<<<<<<
  *             flags = LFSFileFlag.creat | LFSFileFlag.excl | LFSFileFlag.wronly
  *         elif reading:
  */
       goto __pyx_L11;
     }
 
-    /* "littlefs/lfs.pyx":397
+    /* "littlefs/lfs.pyx":400
  *         if creating:
  *             flags = LFSFileFlag.creat | LFSFileFlag.excl | LFSFileFlag.wronly
  *         elif reading:             # <<<<<<<<<<<<<<
  *             flags = LFSFileFlag.rdonly
  *         elif writing:
  */
     if (__pyx_v_reading) {
 
-      /* "littlefs/lfs.pyx":398
+      /* "littlefs/lfs.pyx":401
  *             flags = LFSFileFlag.creat | LFSFileFlag.excl | LFSFileFlag.wronly
  *         elif reading:
  *             flags = LFSFileFlag.rdonly             # <<<<<<<<<<<<<<
  *         elif writing:
  *             flags = LFSFileFlag.creat | LFSFileFlag.wronly | LFSFileFlag.trunc
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_LFSFileFlag); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 398, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_LFSFileFlag); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 401, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_rdonly); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 398, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_rdonly); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 401, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF_SET(__pyx_v_flags, __pyx_t_10);
       __pyx_t_10 = 0;
 
-      /* "littlefs/lfs.pyx":397
+      /* "littlefs/lfs.pyx":400
  *         if creating:
  *             flags = LFSFileFlag.creat | LFSFileFlag.excl | LFSFileFlag.wronly
  *         elif reading:             # <<<<<<<<<<<<<<
  *             flags = LFSFileFlag.rdonly
  *         elif writing:
  */
       goto __pyx_L11;
     }
 
-    /* "littlefs/lfs.pyx":399
+    /* "littlefs/lfs.pyx":402
  *         elif reading:
  *             flags = LFSFileFlag.rdonly
  *         elif writing:             # <<<<<<<<<<<<<<
  *             flags = LFSFileFlag.creat | LFSFileFlag.wronly | LFSFileFlag.trunc
  *         elif appending:
  */
     if (__pyx_v_writing) {
 
-      /* "littlefs/lfs.pyx":400
+      /* "littlefs/lfs.pyx":403
  *             flags = LFSFileFlag.rdonly
  *         elif writing:
  *             flags = LFSFileFlag.creat | LFSFileFlag.wronly | LFSFileFlag.trunc             # <<<<<<<<<<<<<<
  *         elif appending:
  *             flags = LFSFileFlag.wronly | LFSFileFlag.append
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_LFSFileFlag); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 400, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_LFSFileFlag); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 403, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_creat); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 400, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_creat); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 403, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_LFSFileFlag); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 400, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_LFSFileFlag); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 403, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
-      __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_wronly); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 400, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_wronly); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 403, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __pyx_t_10 = PyNumber_Or(__pyx_t_9, __pyx_t_11); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 400, __pyx_L1_error)
+      __pyx_t_10 = PyNumber_Or(__pyx_t_9, __pyx_t_11); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 403, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_LFSFileFlag); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 400, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_LFSFileFlag); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 403, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_trunc); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 400, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_trunc); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 403, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      __pyx_t_11 = PyNumber_Or(__pyx_t_10, __pyx_t_9); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 400, __pyx_L1_error)
+      __pyx_t_11 = PyNumber_Or(__pyx_t_10, __pyx_t_9); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 403, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF_SET(__pyx_v_flags, __pyx_t_11);
       __pyx_t_11 = 0;
 
-      /* "littlefs/lfs.pyx":399
+      /* "littlefs/lfs.pyx":402
  *         elif reading:
  *             flags = LFSFileFlag.rdonly
  *         elif writing:             # <<<<<<<<<<<<<<
  *             flags = LFSFileFlag.creat | LFSFileFlag.wronly | LFSFileFlag.trunc
  *         elif appending:
  */
       goto __pyx_L11;
     }
 
-    /* "littlefs/lfs.pyx":401
+    /* "littlefs/lfs.pyx":404
  *         elif writing:
  *             flags = LFSFileFlag.creat | LFSFileFlag.wronly | LFSFileFlag.trunc
  *         elif appending:             # <<<<<<<<<<<<<<
  *             flags = LFSFileFlag.wronly | LFSFileFlag.append
  * 
  */
     if (__pyx_v_appending) {
 
-      /* "littlefs/lfs.pyx":402
+      /* "littlefs/lfs.pyx":405
  *             flags = LFSFileFlag.creat | LFSFileFlag.wronly | LFSFileFlag.trunc
  *         elif appending:
  *             flags = LFSFileFlag.wronly | LFSFileFlag.append             # <<<<<<<<<<<<<<
  * 
  *         if updating:
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_LFSFileFlag); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 402, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_LFSFileFlag); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 405, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_wronly); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 402, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_wronly); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 405, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_LFSFileFlag); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 402, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_LFSFileFlag); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 405, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
-      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_append); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 402, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_append); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 405, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      __pyx_t_11 = PyNumber_Or(__pyx_t_9, __pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 402, __pyx_L1_error)
+      __pyx_t_11 = PyNumber_Or(__pyx_t_9, __pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 405, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_DECREF_SET(__pyx_v_flags, __pyx_t_11);
       __pyx_t_11 = 0;
 
-      /* "littlefs/lfs.pyx":401
+      /* "littlefs/lfs.pyx":404
  *         elif writing:
  *             flags = LFSFileFlag.creat | LFSFileFlag.wronly | LFSFileFlag.trunc
  *         elif appending:             # <<<<<<<<<<<<<<
  *             flags = LFSFileFlag.wronly | LFSFileFlag.append
  * 
  */
     }
     __pyx_L11:;
 
-    /* "littlefs/lfs.pyx":404
+    /* "littlefs/lfs.pyx":407
  *             flags = LFSFileFlag.wronly | LFSFileFlag.append
  * 
  *         if updating:             # <<<<<<<<<<<<<<
  *             flags |= LFSFileFlag.rdwr
  * 
  */
     if (__pyx_v_updating) {
 
-      /* "littlefs/lfs.pyx":405
+      /* "littlefs/lfs.pyx":408
  * 
  *         if updating:
  *             flags |= LFSFileFlag.rdwr             # <<<<<<<<<<<<<<
  * 
  *     flags = int(flags)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_LFSFileFlag); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 405, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_LFSFileFlag); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 408, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
-      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_rdwr); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 405, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_rdwr); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 408, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      __pyx_t_11 = PyNumber_InPlaceOr(__pyx_v_flags, __pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 405, __pyx_L1_error)
+      __pyx_t_11 = PyNumber_InPlaceOr(__pyx_v_flags, __pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 408, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_DECREF_SET(__pyx_v_flags, __pyx_t_11);
       __pyx_t_11 = 0;
 
-      /* "littlefs/lfs.pyx":404
+      /* "littlefs/lfs.pyx":407
  *             flags = LFSFileFlag.wronly | LFSFileFlag.append
  * 
  *         if updating:             # <<<<<<<<<<<<<<
  *             flags |= LFSFileFlag.rdwr
  * 
  */
     }
 
-    /* "littlefs/lfs.pyx":363
+    /* "littlefs/lfs.pyx":366
  * 
  * def file_open(LFSFilesystem fs, path, flags):
  *     if isinstance(flags, str):             # <<<<<<<<<<<<<<
  *         creating = False
  *         reading = False
  */
   }
 
-  /* "littlefs/lfs.pyx":407
+  /* "littlefs/lfs.pyx":410
  *             flags |= LFSFileFlag.rdwr
  * 
  *     flags = int(flags)             # <<<<<<<<<<<<<<
  *     fh = LFSFile()
  *     _raise_on_error(lfs_file_open(&fs._impl, &fh._impl, path.encode(FILENAME_ENCODING), flags))
  */
-  __pyx_t_11 = __Pyx_PyNumber_Int(__pyx_v_flags); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyNumber_Int(__pyx_v_flags); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 410, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF_SET(__pyx_v_flags, __pyx_t_11);
   __pyx_t_11 = 0;
 
-  /* "littlefs/lfs.pyx":408
+  /* "littlefs/lfs.pyx":411
  * 
  *     flags = int(flags)
  *     fh = LFSFile()             # <<<<<<<<<<<<<<
  *     _raise_on_error(lfs_file_open(&fs._impl, &fh._impl, path.encode(FILENAME_ENCODING), flags))
  *     return fh
  */
-  __pyx_t_11 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8littlefs_3lfs_LFSFile)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 408, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8littlefs_3lfs_LFSFile)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __pyx_v_fh = ((struct __pyx_obj_8littlefs_3lfs_LFSFile *)__pyx_t_11);
   __pyx_t_11 = 0;
 
-  /* "littlefs/lfs.pyx":409
+  /* "littlefs/lfs.pyx":412
  *     flags = int(flags)
  *     fh = LFSFile()
  *     _raise_on_error(lfs_file_open(&fs._impl, &fh._impl, path.encode(FILENAME_ENCODING), flags))             # <<<<<<<<<<<<<<
  *     return fh
  * 
  */
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_path, __pyx_n_s_encode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 409, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_path, __pyx_n_s_encode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 412, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_FILENAME_ENCODING); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 409, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_FILENAME_ENCODING); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 412, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __pyx_t_5 = NULL;
   __pyx_t_12 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_10))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_10);
     if (likely(__pyx_t_5)) {
@@ -26088,36 +26077,36 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_9};
     __pyx_t_11 = __Pyx_PyObject_FastCall(__pyx_t_10, __pyx_callargs+1-__pyx_t_12, 1+__pyx_t_12);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 409, __pyx_L1_error)
+    if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 412, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   }
-  __pyx_t_13 = __Pyx_PyObject_AsString(__pyx_t_11); if (unlikely((!__pyx_t_13) && PyErr_Occurred())) __PYX_ERR(0, 409, __pyx_L1_error)
-  __pyx_t_12 = __Pyx_PyInt_As_int(__pyx_v_flags); if (unlikely((__pyx_t_12 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 409, __pyx_L1_error)
-  __pyx_t_14 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_file_open((&__pyx_v_fs->_impl), (&__pyx_v_fh->_impl), __pyx_t_13, __pyx_t_12)); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 409, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyObject_AsString(__pyx_t_11); if (unlikely((!__pyx_t_13) && PyErr_Occurred())) __PYX_ERR(0, 412, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyInt_As_int(__pyx_v_flags); if (unlikely((__pyx_t_12 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 412, __pyx_L1_error)
+  __pyx_t_14 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_file_open((&__pyx_v_fs->_impl), (&__pyx_v_fh->_impl), __pyx_t_13, __pyx_t_12)); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 412, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-  /* "littlefs/lfs.pyx":410
+  /* "littlefs/lfs.pyx":413
  *     fh = LFSFile()
  *     _raise_on_error(lfs_file_open(&fs._impl, &fh._impl, path.encode(FILENAME_ENCODING), flags))
  *     return fh             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF((PyObject *)__pyx_v_fh);
   __pyx_r = ((PyObject *)__pyx_v_fh);
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":362
+  /* "littlefs/lfs.pyx":365
  * 
  * 
  * def file_open(LFSFilesystem fs, path, flags):             # <<<<<<<<<<<<<<
  *     if isinstance(flags, str):
  *         creating = False
  */
 
@@ -26137,15 +26126,15 @@
   __Pyx_XDECREF(__pyx_gb_8littlefs_3lfs_9file_open_2generator);
   __Pyx_XDECREF(__pyx_v_flags);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":413
+/* "littlefs/lfs.pyx":416
  * 
  * 
  * def file_open_cfg(self, path, flags, config):             # <<<<<<<<<<<<<<
  *     raise NotImplementedError
  * 
  */
 
@@ -26208,50 +26197,50 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 413, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 416, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_path)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 413, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 416, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("file_open_cfg", 1, 4, 4, 1); __PYX_ERR(0, 413, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("file_open_cfg", 1, 4, 4, 1); __PYX_ERR(0, 416, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_flags)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 413, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 416, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("file_open_cfg", 1, 4, 4, 2); __PYX_ERR(0, 413, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("file_open_cfg", 1, 4, 4, 2); __PYX_ERR(0, 416, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_config)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 413, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 416, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("file_open_cfg", 1, 4, 4, 3); __PYX_ERR(0, 413, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("file_open_cfg", 1, 4, 4, 3); __PYX_ERR(0, 416, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "file_open_cfg") < 0)) __PYX_ERR(0, 413, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "file_open_cfg") < 0)) __PYX_ERR(0, 416, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 4)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
@@ -26260,15 +26249,15 @@
     __pyx_v_self = values[0];
     __pyx_v_path = values[1];
     __pyx_v_flags = values[2];
     __pyx_v_config = values[3];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("file_open_cfg", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 413, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("file_open_cfg", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 416, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -26295,25 +26284,25 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("file_open_cfg", 1);
 
-  /* "littlefs/lfs.pyx":414
+  /* "littlefs/lfs.pyx":417
  * 
  * def file_open_cfg(self, path, flags, config):
  *     raise NotImplementedError             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_Raise(__pyx_builtin_NotImplementedError, 0, 0, 0);
-  __PYX_ERR(0, 414, __pyx_L1_error)
+  __PYX_ERR(0, 417, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":413
+  /* "littlefs/lfs.pyx":416
  * 
  * 
  * def file_open_cfg(self, path, flags, config):             # <<<<<<<<<<<<<<
  *     raise NotImplementedError
  * 
  */
 
@@ -26322,15 +26311,15 @@
   __Pyx_AddTraceback("littlefs.lfs.file_open_cfg", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":417
+/* "littlefs/lfs.pyx":420
  * 
  * 
  * def file_close(LFSFilesystem fs, LFSFile fh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_file_close(&fs._impl, &fh._impl))
  * 
  */
 
@@ -26387,58 +26376,58 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 417, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 420, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fh)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 417, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 420, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("file_close", 1, 2, 2, 1); __PYX_ERR(0, 417, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("file_close", 1, 2, 2, 1); __PYX_ERR(0, 420, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "file_close") < 0)) __PYX_ERR(0, 417, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "file_close") < 0)) __PYX_ERR(0, 420, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
     __pyx_v_fh = ((struct __pyx_obj_8littlefs_3lfs_LFSFile *)values[1]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("file_close", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 417, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("file_close", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 420, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.file_close", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 417, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fh), __pyx_ptype_8littlefs_3lfs_LFSFile, 1, "fh", 0))) __PYX_ERR(0, 417, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 420, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fh), __pyx_ptype_8littlefs_3lfs_LFSFile, 1, "fh", 0))) __PYX_ERR(0, 420, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_30file_close(__pyx_self, __pyx_v_fs, __pyx_v_fh);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -26458,30 +26447,30 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("file_close", 1);
 
-  /* "littlefs/lfs.pyx":418
+  /* "littlefs/lfs.pyx":421
  * 
  * def file_close(LFSFilesystem fs, LFSFile fh):
  *     return _raise_on_error(lfs_file_close(&fs._impl, &fh._impl))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_file_close((&__pyx_v_fs->_impl), (&__pyx_v_fh->_impl))); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 418, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 418, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_file_close((&__pyx_v_fs->_impl), (&__pyx_v_fh->_impl))); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 421, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 421, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":417
+  /* "littlefs/lfs.pyx":420
  * 
  * 
  * def file_close(LFSFilesystem fs, LFSFile fh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_file_close(&fs._impl, &fh._impl))
  * 
  */
 
@@ -26492,15 +26481,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":421
+/* "littlefs/lfs.pyx":424
  * 
  * 
  * def file_sync(LFSFilesystem fs, LFSFile fh):             # <<<<<<<<<<<<<<
  *     _raise_on_error(lfs_file_sync(&fs._impl, &fh._impl))
  * 
  */
 
@@ -26557,58 +26546,58 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 421, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 424, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fh)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 421, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 424, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("file_sync", 1, 2, 2, 1); __PYX_ERR(0, 421, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("file_sync", 1, 2, 2, 1); __PYX_ERR(0, 424, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "file_sync") < 0)) __PYX_ERR(0, 421, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "file_sync") < 0)) __PYX_ERR(0, 424, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
     __pyx_v_fh = ((struct __pyx_obj_8littlefs_3lfs_LFSFile *)values[1]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("file_sync", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 421, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("file_sync", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 424, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.file_sync", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 421, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fh), __pyx_ptype_8littlefs_3lfs_LFSFile, 1, "fh", 0))) __PYX_ERR(0, 421, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 424, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fh), __pyx_ptype_8littlefs_3lfs_LFSFile, 1, "fh", 0))) __PYX_ERR(0, 424, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_32file_sync(__pyx_self, __pyx_v_fs, __pyx_v_fh);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -26627,24 +26616,24 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("file_sync", 1);
 
-  /* "littlefs/lfs.pyx":422
+  /* "littlefs/lfs.pyx":425
  * 
  * def file_sync(LFSFilesystem fs, LFSFile fh):
  *     _raise_on_error(lfs_file_sync(&fs._impl, &fh._impl))             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_file_sync((&__pyx_v_fs->_impl), (&__pyx_v_fh->_impl))); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 422, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_file_sync((&__pyx_v_fs->_impl), (&__pyx_v_fh->_impl))); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 425, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":421
+  /* "littlefs/lfs.pyx":424
  * 
  * 
  * def file_sync(LFSFilesystem fs, LFSFile fh):             # <<<<<<<<<<<<<<
  *     _raise_on_error(lfs_file_sync(&fs._impl, &fh._impl))
  * 
  */
 
@@ -26656,15 +26645,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":425
+/* "littlefs/lfs.pyx":428
  * 
  * 
  * def file_read(LFSFilesystem fs, LFSFile fh, size):             # <<<<<<<<<<<<<<
  *     assert size >= 0, 'Size must be >= 0'
  *     buffer = b'\0xff' * size
  */
 
@@ -26724,70 +26713,70 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 425, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 428, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fh)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 425, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 428, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("file_read", 1, 3, 3, 1); __PYX_ERR(0, 425, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("file_read", 1, 3, 3, 1); __PYX_ERR(0, 428, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_size)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 425, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 428, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("file_read", 1, 3, 3, 2); __PYX_ERR(0, 425, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("file_read", 1, 3, 3, 2); __PYX_ERR(0, 428, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "file_read") < 0)) __PYX_ERR(0, 425, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "file_read") < 0)) __PYX_ERR(0, 428, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
     __pyx_v_fh = ((struct __pyx_obj_8littlefs_3lfs_LFSFile *)values[1]);
     __pyx_v_size = values[2];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("file_read", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 425, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("file_read", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 428, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.file_read", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 425, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fh), __pyx_ptype_8littlefs_3lfs_LFSFile, 1, "fh", 0))) __PYX_ERR(0, 425, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 428, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fh), __pyx_ptype_8littlefs_3lfs_LFSFile, 1, "fh", 0))) __PYX_ERR(0, 428, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_34file_read(__pyx_self, __pyx_v_fs, __pyx_v_fh, __pyx_v_size);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -26812,74 +26801,74 @@
   lfs_size_t __pyx_t_4;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("file_read", 1);
 
-  /* "littlefs/lfs.pyx":426
+  /* "littlefs/lfs.pyx":429
  * 
  * def file_read(LFSFilesystem fs, LFSFile fh, size):
  *     assert size >= 0, 'Size must be >= 0'             # <<<<<<<<<<<<<<
  *     buffer = b'\0xff' * size
  *     rsize = _raise_on_error(lfs_file_read(&fs._impl, &fh._impl, <char *>buffer, size))
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
-    __pyx_t_1 = PyObject_RichCompare(__pyx_v_size, __pyx_int_0, Py_GE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 426, __pyx_L1_error)
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 426, __pyx_L1_error)
+    __pyx_t_1 = PyObject_RichCompare(__pyx_v_size, __pyx_int_0, Py_GE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 429, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 429, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (unlikely(!__pyx_t_2)) {
       __Pyx_Raise(__pyx_builtin_AssertionError, __pyx_kp_u_Size_must_be_0, 0, 0);
-      __PYX_ERR(0, 426, __pyx_L1_error)
+      __PYX_ERR(0, 429, __pyx_L1_error)
     }
   }
   #else
-  if ((1)); else __PYX_ERR(0, 426, __pyx_L1_error)
+  if ((1)); else __PYX_ERR(0, 429, __pyx_L1_error)
   #endif
 
-  /* "littlefs/lfs.pyx":427
+  /* "littlefs/lfs.pyx":430
  * def file_read(LFSFilesystem fs, LFSFile fh, size):
  *     assert size >= 0, 'Size must be >= 0'
  *     buffer = b'\0xff' * size             # <<<<<<<<<<<<<<
  *     rsize = _raise_on_error(lfs_file_read(&fs._impl, &fh._impl, <char *>buffer, size))
  *     return buffer[:rsize]
  */
-  __pyx_t_1 = PyNumber_Multiply(__pyx_kp_b_xff, __pyx_v_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Multiply(__pyx_kp_b_xff, __pyx_v_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 430, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_buffer = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "littlefs/lfs.pyx":428
+  /* "littlefs/lfs.pyx":431
  *     assert size >= 0, 'Size must be >= 0'
  *     buffer = b'\0xff' * size
  *     rsize = _raise_on_error(lfs_file_read(&fs._impl, &fh._impl, <char *>buffer, size))             # <<<<<<<<<<<<<<
  *     return buffer[:rsize]
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_AsWritableString(__pyx_v_buffer); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 428, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyInt_As_uint32_t(__pyx_v_size); if (unlikely((__pyx_t_4 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 428, __pyx_L1_error)
-  __pyx_t_5 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_file_read((&__pyx_v_fs->_impl), (&__pyx_v_fh->_impl), ((char *)__pyx_t_3), __pyx_t_4)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_AsWritableString(__pyx_v_buffer); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 431, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_uint32_t(__pyx_v_size); if (unlikely((__pyx_t_4 == ((lfs_size_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 431, __pyx_L1_error)
+  __pyx_t_5 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_file_read((&__pyx_v_fs->_impl), (&__pyx_v_fh->_impl), ((char *)__pyx_t_3), __pyx_t_4)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 431, __pyx_L1_error)
   __pyx_v_rsize = __pyx_t_5;
 
-  /* "littlefs/lfs.pyx":429
+  /* "littlefs/lfs.pyx":432
  *     buffer = b'\0xff' * size
  *     rsize = _raise_on_error(lfs_file_read(&fs._impl, &fh._impl, <char *>buffer, size))
  *     return buffer[:rsize]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_buffer, 0, __pyx_v_rsize, NULL, NULL, NULL, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 429, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_buffer, 0, __pyx_v_rsize, NULL, NULL, NULL, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 432, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":425
+  /* "littlefs/lfs.pyx":428
  * 
  * 
  * def file_read(LFSFilesystem fs, LFSFile fh, size):             # <<<<<<<<<<<<<<
  *     assert size >= 0, 'Size must be >= 0'
  *     buffer = b'\0xff' * size
  */
 
@@ -26891,15 +26880,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_buffer);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":432
+/* "littlefs/lfs.pyx":435
  * 
  * 
  * def file_write(LFSFilesystem fs, LFSFile fh, data):             # <<<<<<<<<<<<<<
  *     assert isinstance(data, (bytes, bytearray))
  *     pdata = <char *>data
  */
 
@@ -26959,70 +26948,70 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 432, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 435, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fh)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 432, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 435, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("file_write", 1, 3, 3, 1); __PYX_ERR(0, 432, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("file_write", 1, 3, 3, 1); __PYX_ERR(0, 435, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_data)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 432, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 435, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("file_write", 1, 3, 3, 2); __PYX_ERR(0, 432, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("file_write", 1, 3, 3, 2); __PYX_ERR(0, 435, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "file_write") < 0)) __PYX_ERR(0, 432, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "file_write") < 0)) __PYX_ERR(0, 435, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
     __pyx_v_fh = ((struct __pyx_obj_8littlefs_3lfs_LFSFile *)values[1]);
     __pyx_v_data = values[2];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("file_write", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 432, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("file_write", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 435, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.file_write", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 432, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fh), __pyx_ptype_8littlefs_3lfs_LFSFile, 1, "fh", 0))) __PYX_ERR(0, 432, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 435, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fh), __pyx_ptype_8littlefs_3lfs_LFSFile, 1, "fh", 0))) __PYX_ERR(0, 435, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_36file_write(__pyx_self, __pyx_v_fs, __pyx_v_fh, __pyx_v_data);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -27048,15 +27037,15 @@
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("file_write", 1);
 
-  /* "littlefs/lfs.pyx":433
+  /* "littlefs/lfs.pyx":436
  * 
  * def file_write(LFSFilesystem fs, LFSFile fh, data):
  *     assert isinstance(data, (bytes, bytearray))             # <<<<<<<<<<<<<<
  *     pdata = <char *>data
  *     code =_raise_on_error(lfs_file_write(&fs._impl, &fh._impl, <char *>data, len(data)))
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
@@ -27068,91 +27057,91 @@
       goto __pyx_L3_bool_binop_done;
     }
     __pyx_t_2 = PyByteArray_Check(__pyx_v_data); 
     __pyx_t_1 = __pyx_t_2;
     __pyx_L3_bool_binop_done:;
     if (unlikely(!__pyx_t_1)) {
       __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
-      __PYX_ERR(0, 433, __pyx_L1_error)
+      __PYX_ERR(0, 436, __pyx_L1_error)
     }
   }
   #else
-  if ((1)); else __PYX_ERR(0, 433, __pyx_L1_error)
+  if ((1)); else __PYX_ERR(0, 436, __pyx_L1_error)
   #endif
 
-  /* "littlefs/lfs.pyx":434
+  /* "littlefs/lfs.pyx":437
  * def file_write(LFSFilesystem fs, LFSFile fh, data):
  *     assert isinstance(data, (bytes, bytearray))
  *     pdata = <char *>data             # <<<<<<<<<<<<<<
  *     code =_raise_on_error(lfs_file_write(&fs._impl, &fh._impl, <char *>data, len(data)))
  *     if code != len(data):
  */
-  __pyx_t_3 = __Pyx_PyObject_AsWritableString(__pyx_v_data); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 434, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_AsWritableString(__pyx_v_data); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 437, __pyx_L1_error)
   __pyx_v_pdata = ((char *)__pyx_t_3);
 
-  /* "littlefs/lfs.pyx":435
+  /* "littlefs/lfs.pyx":438
  *     assert isinstance(data, (bytes, bytearray))
  *     pdata = <char *>data
  *     code =_raise_on_error(lfs_file_write(&fs._impl, &fh._impl, <char *>data, len(data)))             # <<<<<<<<<<<<<<
  *     if code != len(data):
  *         raise RuntimeError("Not all data written")
  */
-  __pyx_t_3 = __Pyx_PyObject_AsWritableString(__pyx_v_data); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 435, __pyx_L1_error)
-  __pyx_t_4 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 435, __pyx_L1_error)
-  __pyx_t_5 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_file_write((&__pyx_v_fs->_impl), (&__pyx_v_fh->_impl), ((char *)__pyx_t_3), __pyx_t_4)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 435, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_AsWritableString(__pyx_v_data); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 438, __pyx_L1_error)
+  __pyx_t_4 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 438, __pyx_L1_error)
+  __pyx_t_5 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_file_write((&__pyx_v_fs->_impl), (&__pyx_v_fh->_impl), ((char *)__pyx_t_3), __pyx_t_4)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 438, __pyx_L1_error)
   __pyx_v_code = __pyx_t_5;
 
-  /* "littlefs/lfs.pyx":436
+  /* "littlefs/lfs.pyx":439
  *     pdata = <char *>data
  *     code =_raise_on_error(lfs_file_write(&fs._impl, &fh._impl, <char *>data, len(data)))
  *     if code != len(data):             # <<<<<<<<<<<<<<
  *         raise RuntimeError("Not all data written")
  *     return code
  */
-  __pyx_t_4 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 436, __pyx_L1_error)
+  __pyx_t_4 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 439, __pyx_L1_error)
   __pyx_t_1 = (__pyx_v_code != __pyx_t_4);
   if (unlikely(__pyx_t_1)) {
 
-    /* "littlefs/lfs.pyx":437
+    /* "littlefs/lfs.pyx":440
  *     code =_raise_on_error(lfs_file_write(&fs._impl, &fh._impl, <char *>data, len(data)))
  *     if code != len(data):
  *         raise RuntimeError("Not all data written")             # <<<<<<<<<<<<<<
  *     return code
  * 
  */
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 437, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 440, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 437, __pyx_L1_error)
+    __PYX_ERR(0, 440, __pyx_L1_error)
 
-    /* "littlefs/lfs.pyx":436
+    /* "littlefs/lfs.pyx":439
  *     pdata = <char *>data
  *     code =_raise_on_error(lfs_file_write(&fs._impl, &fh._impl, <char *>data, len(data)))
  *     if code != len(data):             # <<<<<<<<<<<<<<
  *         raise RuntimeError("Not all data written")
  *     return code
  */
   }
 
-  /* "littlefs/lfs.pyx":438
+  /* "littlefs/lfs.pyx":441
  *     if code != len(data):
  *         raise RuntimeError("Not all data written")
  *     return code             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_code); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 438, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_code); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 441, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":432
+  /* "littlefs/lfs.pyx":435
  * 
  * 
  * def file_write(LFSFilesystem fs, LFSFile fh, data):             # <<<<<<<<<<<<<<
  *     assert isinstance(data, (bytes, bytearray))
  *     pdata = <char *>data
  */
 
@@ -27163,15 +27152,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":441
+/* "littlefs/lfs.pyx":444
  * 
  * 
  * def file_seek(LFSFilesystem fs, LFSFile fh, off, whence):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_file_seek(&fs._impl, &fh._impl, off, whence))
  * 
  */
 
@@ -27234,50 +27223,50 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 441, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 444, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fh)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 441, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 444, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("file_seek", 1, 4, 4, 1); __PYX_ERR(0, 441, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("file_seek", 1, 4, 4, 1); __PYX_ERR(0, 444, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_off)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 441, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 444, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("file_seek", 1, 4, 4, 2); __PYX_ERR(0, 441, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("file_seek", 1, 4, 4, 2); __PYX_ERR(0, 444, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_whence)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 441, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 444, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("file_seek", 1, 4, 4, 3); __PYX_ERR(0, 441, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("file_seek", 1, 4, 4, 3); __PYX_ERR(0, 444, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "file_seek") < 0)) __PYX_ERR(0, 441, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "file_seek") < 0)) __PYX_ERR(0, 444, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 4)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
@@ -27286,30 +27275,30 @@
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
     __pyx_v_fh = ((struct __pyx_obj_8littlefs_3lfs_LFSFile *)values[1]);
     __pyx_v_off = values[2];
     __pyx_v_whence = values[3];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("file_seek", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 441, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("file_seek", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 444, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.file_seek", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 441, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fh), __pyx_ptype_8littlefs_3lfs_LFSFile, 1, "fh", 0))) __PYX_ERR(0, 441, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 444, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fh), __pyx_ptype_8littlefs_3lfs_LFSFile, 1, "fh", 0))) __PYX_ERR(0, 444, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_38file_seek(__pyx_self, __pyx_v_fs, __pyx_v_fh, __pyx_v_off, __pyx_v_whence);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -27331,32 +27320,32 @@
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("file_seek", 1);
 
-  /* "littlefs/lfs.pyx":442
+  /* "littlefs/lfs.pyx":445
  * 
  * def file_seek(LFSFilesystem fs, LFSFile fh, off, whence):
  *     return _raise_on_error(lfs_file_seek(&fs._impl, &fh._impl, off, whence))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_int32_t(__pyx_v_off); if (unlikely((__pyx_t_1 == ((lfs_soff_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 442, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_whence); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 442, __pyx_L1_error)
-  __pyx_t_3 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_file_seek((&__pyx_v_fs->_impl), (&__pyx_v_fh->_impl), __pyx_t_1, __pyx_t_2)); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 442, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 442, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int32_t(__pyx_v_off); if (unlikely((__pyx_t_1 == ((lfs_soff_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 445, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_whence); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 445, __pyx_L1_error)
+  __pyx_t_3 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_file_seek((&__pyx_v_fs->_impl), (&__pyx_v_fh->_impl), __pyx_t_1, __pyx_t_2)); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 445, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 445, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":441
+  /* "littlefs/lfs.pyx":444
  * 
  * 
  * def file_seek(LFSFilesystem fs, LFSFile fh, off, whence):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_file_seek(&fs._impl, &fh._impl, off, whence))
  * 
  */
 
@@ -27367,15 +27356,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":445
+/* "littlefs/lfs.pyx":448
  * 
  * 
  * def file_truncate(LFSFilesystem fs, LFSFile fh, size):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_file_truncate(&fs._impl, &fh._impl, size))
  * 
  */
 
@@ -27435,70 +27424,70 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 445, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 448, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fh)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 445, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 448, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("file_truncate", 1, 3, 3, 1); __PYX_ERR(0, 445, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("file_truncate", 1, 3, 3, 1); __PYX_ERR(0, 448, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_size)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 445, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 448, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("file_truncate", 1, 3, 3, 2); __PYX_ERR(0, 445, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("file_truncate", 1, 3, 3, 2); __PYX_ERR(0, 448, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "file_truncate") < 0)) __PYX_ERR(0, 445, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "file_truncate") < 0)) __PYX_ERR(0, 448, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
     __pyx_v_fh = ((struct __pyx_obj_8littlefs_3lfs_LFSFile *)values[1]);
     __pyx_v_size = values[2];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("file_truncate", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 445, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("file_truncate", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 448, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.file_truncate", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 445, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fh), __pyx_ptype_8littlefs_3lfs_LFSFile, 1, "fh", 0))) __PYX_ERR(0, 445, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 448, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fh), __pyx_ptype_8littlefs_3lfs_LFSFile, 1, "fh", 0))) __PYX_ERR(0, 448, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_40file_truncate(__pyx_self, __pyx_v_fs, __pyx_v_fh, __pyx_v_size);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -27519,31 +27508,31 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("file_truncate", 1);
 
-  /* "littlefs/lfs.pyx":446
+  /* "littlefs/lfs.pyx":449
  * 
  * def file_truncate(LFSFilesystem fs, LFSFile fh, size):
  *     return _raise_on_error(lfs_file_truncate(&fs._impl, &fh._impl, size))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_uint32_t(__pyx_v_size); if (unlikely((__pyx_t_1 == ((lfs_off_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 446, __pyx_L1_error)
-  __pyx_t_2 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_file_truncate((&__pyx_v_fs->_impl), (&__pyx_v_fh->_impl), __pyx_t_1)); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 446, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 446, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint32_t(__pyx_v_size); if (unlikely((__pyx_t_1 == ((lfs_off_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 449, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_file_truncate((&__pyx_v_fs->_impl), (&__pyx_v_fh->_impl), __pyx_t_1)); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 449, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 449, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":445
+  /* "littlefs/lfs.pyx":448
  * 
  * 
  * def file_truncate(LFSFilesystem fs, LFSFile fh, size):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_file_truncate(&fs._impl, &fh._impl, size))
  * 
  */
 
@@ -27554,15 +27543,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":449
+/* "littlefs/lfs.pyx":452
  * 
  * 
  * def file_tell(LFSFilesystem fs, LFSFile fh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_file_tell(&fs._impl, &fh._impl))
  * 
  */
 
@@ -27619,58 +27608,58 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 449, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 452, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fh)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 449, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 452, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("file_tell", 1, 2, 2, 1); __PYX_ERR(0, 449, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("file_tell", 1, 2, 2, 1); __PYX_ERR(0, 452, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "file_tell") < 0)) __PYX_ERR(0, 449, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "file_tell") < 0)) __PYX_ERR(0, 452, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
     __pyx_v_fh = ((struct __pyx_obj_8littlefs_3lfs_LFSFile *)values[1]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("file_tell", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 449, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("file_tell", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 452, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.file_tell", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 449, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fh), __pyx_ptype_8littlefs_3lfs_LFSFile, 1, "fh", 0))) __PYX_ERR(0, 449, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 452, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fh), __pyx_ptype_8littlefs_3lfs_LFSFile, 1, "fh", 0))) __PYX_ERR(0, 452, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_42file_tell(__pyx_self, __pyx_v_fs, __pyx_v_fh);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -27690,30 +27679,30 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("file_tell", 1);
 
-  /* "littlefs/lfs.pyx":450
+  /* "littlefs/lfs.pyx":453
  * 
  * def file_tell(LFSFilesystem fs, LFSFile fh):
  *     return _raise_on_error(lfs_file_tell(&fs._impl, &fh._impl))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_file_tell((&__pyx_v_fs->_impl), (&__pyx_v_fh->_impl))); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 450, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 450, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_file_tell((&__pyx_v_fs->_impl), (&__pyx_v_fh->_impl))); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 453, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":449
+  /* "littlefs/lfs.pyx":452
  * 
  * 
  * def file_tell(LFSFilesystem fs, LFSFile fh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_file_tell(&fs._impl, &fh._impl))
  * 
  */
 
@@ -27724,15 +27713,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":453
+/* "littlefs/lfs.pyx":456
  * 
  * 
  * def file_rewind(LFSFilesystem fs, LFSFile fh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_file_rewind(&fs._impl, &fh._impl))
  * 
  */
 
@@ -27789,58 +27778,58 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 453, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 456, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fh)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 453, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 456, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("file_rewind", 1, 2, 2, 1); __PYX_ERR(0, 453, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("file_rewind", 1, 2, 2, 1); __PYX_ERR(0, 456, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "file_rewind") < 0)) __PYX_ERR(0, 453, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "file_rewind") < 0)) __PYX_ERR(0, 456, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
     __pyx_v_fh = ((struct __pyx_obj_8littlefs_3lfs_LFSFile *)values[1]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("file_rewind", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 453, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("file_rewind", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 456, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.file_rewind", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 453, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fh), __pyx_ptype_8littlefs_3lfs_LFSFile, 1, "fh", 0))) __PYX_ERR(0, 453, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 456, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fh), __pyx_ptype_8littlefs_3lfs_LFSFile, 1, "fh", 0))) __PYX_ERR(0, 456, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_44file_rewind(__pyx_self, __pyx_v_fs, __pyx_v_fh);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -27860,30 +27849,30 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("file_rewind", 1);
 
-  /* "littlefs/lfs.pyx":454
+  /* "littlefs/lfs.pyx":457
  * 
  * def file_rewind(LFSFilesystem fs, LFSFile fh):
  *     return _raise_on_error(lfs_file_rewind(&fs._impl, &fh._impl))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_file_rewind((&__pyx_v_fs->_impl), (&__pyx_v_fh->_impl))); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 454, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_file_rewind((&__pyx_v_fs->_impl), (&__pyx_v_fh->_impl))); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 457, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 457, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":453
+  /* "littlefs/lfs.pyx":456
  * 
  * 
  * def file_rewind(LFSFilesystem fs, LFSFile fh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_file_rewind(&fs._impl, &fh._impl))
  * 
  */
 
@@ -27894,15 +27883,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":457
+/* "littlefs/lfs.pyx":460
  * 
  * 
  * def file_size(LFSFilesystem fs, LFSFile fh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_file_size(&fs._impl, &fh._impl))
  * 
  */
 
@@ -27959,58 +27948,58 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 457, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 460, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fh)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 457, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 460, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("file_size", 1, 2, 2, 1); __PYX_ERR(0, 457, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("file_size", 1, 2, 2, 1); __PYX_ERR(0, 460, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "file_size") < 0)) __PYX_ERR(0, 457, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "file_size") < 0)) __PYX_ERR(0, 460, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
     __pyx_v_fh = ((struct __pyx_obj_8littlefs_3lfs_LFSFile *)values[1]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("file_size", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 457, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("file_size", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 460, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.file_size", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 457, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fh), __pyx_ptype_8littlefs_3lfs_LFSFile, 1, "fh", 0))) __PYX_ERR(0, 457, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 460, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fh), __pyx_ptype_8littlefs_3lfs_LFSFile, 1, "fh", 0))) __PYX_ERR(0, 460, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_46file_size(__pyx_self, __pyx_v_fs, __pyx_v_fh);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -28030,30 +28019,30 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("file_size", 1);
 
-  /* "littlefs/lfs.pyx":458
+  /* "littlefs/lfs.pyx":461
  * 
  * def file_size(LFSFilesystem fs, LFSFile fh):
  *     return _raise_on_error(lfs_file_size(&fs._impl, &fh._impl))             # <<<<<<<<<<<<<<
  * 
  * def mkdir(LFSFilesystem fs, path):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_file_size((&__pyx_v_fs->_impl), (&__pyx_v_fh->_impl))); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 458, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 458, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_file_size((&__pyx_v_fs->_impl), (&__pyx_v_fh->_impl))); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 461, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 461, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":457
+  /* "littlefs/lfs.pyx":460
  * 
  * 
  * def file_size(LFSFilesystem fs, LFSFile fh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_file_size(&fs._impl, &fh._impl))
  * 
  */
 
@@ -28064,15 +28053,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":460
+/* "littlefs/lfs.pyx":463
  *     return _raise_on_error(lfs_file_size(&fs._impl, &fh._impl))
  * 
  * def mkdir(LFSFilesystem fs, path):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_mkdir(&fs._impl, path.encode(FILENAME_ENCODING)))
  * 
  */
 
@@ -28129,57 +28118,57 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 460, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 463, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_path)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 460, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 463, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("mkdir", 1, 2, 2, 1); __PYX_ERR(0, 460, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("mkdir", 1, 2, 2, 1); __PYX_ERR(0, 463, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "mkdir") < 0)) __PYX_ERR(0, 460, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "mkdir") < 0)) __PYX_ERR(0, 463, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
     __pyx_v_path = values[1];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("mkdir", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 460, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("mkdir", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 463, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.mkdir", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 460, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 463, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_48mkdir(__pyx_self, __pyx_v_fs, __pyx_v_path);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -28203,25 +28192,25 @@
   int __pyx_t_5;
   char const *__pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("mkdir", 1);
 
-  /* "littlefs/lfs.pyx":461
+  /* "littlefs/lfs.pyx":464
  * 
  * def mkdir(LFSFilesystem fs, path):
  *     return _raise_on_error(lfs_mkdir(&fs._impl, path.encode(FILENAME_ENCODING)))             # <<<<<<<<<<<<<<
  * 
  * def dir_open(LFSFilesystem fs, path):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_path, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 461, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_path, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 464, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FILENAME_ENCODING); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 461, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FILENAME_ENCODING); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 464, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
@@ -28234,28 +28223,28 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_3};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 461, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 464, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_t_6 = __Pyx_PyObject_AsString(__pyx_t_1); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 461, __pyx_L1_error)
-  __pyx_t_5 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_mkdir((&__pyx_v_fs->_impl), __pyx_t_6)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 461, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_AsString(__pyx_t_1); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 464, __pyx_L1_error)
+  __pyx_t_5 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_mkdir((&__pyx_v_fs->_impl), __pyx_t_6)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 464, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 461, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 464, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":460
+  /* "littlefs/lfs.pyx":463
  *     return _raise_on_error(lfs_file_size(&fs._impl, &fh._impl))
  * 
  * def mkdir(LFSFilesystem fs, path):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_mkdir(&fs._impl, path.encode(FILENAME_ENCODING)))
  * 
  */
 
@@ -28269,15 +28258,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":463
+/* "littlefs/lfs.pyx":466
  *     return _raise_on_error(lfs_mkdir(&fs._impl, path.encode(FILENAME_ENCODING)))
  * 
  * def dir_open(LFSFilesystem fs, path):             # <<<<<<<<<<<<<<
  *     handle = LFSDirectory()
  *     _raise_on_error(lfs_dir_open(&fs._impl, &handle._impl, path.encode(FILENAME_ENCODING)))
  */
 
@@ -28334,57 +28323,57 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 463, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 466, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_path)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 463, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 466, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("dir_open", 1, 2, 2, 1); __PYX_ERR(0, 463, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("dir_open", 1, 2, 2, 1); __PYX_ERR(0, 466, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "dir_open") < 0)) __PYX_ERR(0, 463, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "dir_open") < 0)) __PYX_ERR(0, 466, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
     __pyx_v_path = values[1];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("dir_open", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 463, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("dir_open", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 466, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.dir_open", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 463, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 466, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_50dir_open(__pyx_self, __pyx_v_fs, __pyx_v_path);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -28409,36 +28398,36 @@
   int __pyx_t_5;
   char const *__pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dir_open", 1);
 
-  /* "littlefs/lfs.pyx":464
+  /* "littlefs/lfs.pyx":467
  * 
  * def dir_open(LFSFilesystem fs, path):
  *     handle = LFSDirectory()             # <<<<<<<<<<<<<<
  *     _raise_on_error(lfs_dir_open(&fs._impl, &handle._impl, path.encode(FILENAME_ENCODING)))
  *     return handle
  */
-  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8littlefs_3lfs_LFSDirectory)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 464, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8littlefs_3lfs_LFSDirectory)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 467, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_handle = ((struct __pyx_obj_8littlefs_3lfs_LFSDirectory *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "littlefs/lfs.pyx":465
+  /* "littlefs/lfs.pyx":468
  * def dir_open(LFSFilesystem fs, path):
  *     handle = LFSDirectory()
  *     _raise_on_error(lfs_dir_open(&fs._impl, &handle._impl, path.encode(FILENAME_ENCODING)))             # <<<<<<<<<<<<<<
  *     return handle
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_path, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 465, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_path, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 468, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FILENAME_ENCODING); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 465, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FILENAME_ENCODING); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 468, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
@@ -28451,35 +28440,35 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_3};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 465, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 468, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_t_6 = __Pyx_PyObject_AsString(__pyx_t_1); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 465, __pyx_L1_error)
-  __pyx_t_5 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_dir_open((&__pyx_v_fs->_impl), (&__pyx_v_handle->_impl), __pyx_t_6)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 465, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_AsString(__pyx_t_1); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 468, __pyx_L1_error)
+  __pyx_t_5 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_dir_open((&__pyx_v_fs->_impl), (&__pyx_v_handle->_impl), __pyx_t_6)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 468, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "littlefs/lfs.pyx":466
+  /* "littlefs/lfs.pyx":469
  *     handle = LFSDirectory()
  *     _raise_on_error(lfs_dir_open(&fs._impl, &handle._impl, path.encode(FILENAME_ENCODING)))
  *     return handle             # <<<<<<<<<<<<<<
  * 
  * def dir_close(LFSFilesystem fs, LFSDirectory dh):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF((PyObject *)__pyx_v_handle);
   __pyx_r = ((PyObject *)__pyx_v_handle);
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":463
+  /* "littlefs/lfs.pyx":466
  *     return _raise_on_error(lfs_mkdir(&fs._impl, path.encode(FILENAME_ENCODING)))
  * 
  * def dir_open(LFSFilesystem fs, path):             # <<<<<<<<<<<<<<
  *     handle = LFSDirectory()
  *     _raise_on_error(lfs_dir_open(&fs._impl, &handle._impl, path.encode(FILENAME_ENCODING)))
  */
 
@@ -28494,15 +28483,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_handle);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":468
+/* "littlefs/lfs.pyx":471
  *     return handle
  * 
  * def dir_close(LFSFilesystem fs, LFSDirectory dh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_dir_close(&fs._impl, &dh._impl))
  * 
  */
 
@@ -28559,58 +28548,58 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 468, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 471, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_dh)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 468, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 471, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("dir_close", 1, 2, 2, 1); __PYX_ERR(0, 468, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("dir_close", 1, 2, 2, 1); __PYX_ERR(0, 471, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "dir_close") < 0)) __PYX_ERR(0, 468, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "dir_close") < 0)) __PYX_ERR(0, 471, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
     __pyx_v_dh = ((struct __pyx_obj_8littlefs_3lfs_LFSDirectory *)values[1]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("dir_close", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 468, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("dir_close", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 471, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.dir_close", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 468, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_dh), __pyx_ptype_8littlefs_3lfs_LFSDirectory, 1, "dh", 0))) __PYX_ERR(0, 468, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 471, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_dh), __pyx_ptype_8littlefs_3lfs_LFSDirectory, 1, "dh", 0))) __PYX_ERR(0, 471, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_52dir_close(__pyx_self, __pyx_v_fs, __pyx_v_dh);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -28630,30 +28619,30 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dir_close", 1);
 
-  /* "littlefs/lfs.pyx":469
+  /* "littlefs/lfs.pyx":472
  * 
  * def dir_close(LFSFilesystem fs, LFSDirectory dh):
  *     return _raise_on_error(lfs_dir_close(&fs._impl, &dh._impl))             # <<<<<<<<<<<<<<
  * 
  * def dir_read(LFSFilesystem fs, LFSDirectory dh):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_dir_close((&__pyx_v_fs->_impl), (&__pyx_v_dh->_impl))); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 469, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 469, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_dir_close((&__pyx_v_fs->_impl), (&__pyx_v_dh->_impl))); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 472, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 472, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":468
+  /* "littlefs/lfs.pyx":471
  *     return handle
  * 
  * def dir_close(LFSFilesystem fs, LFSDirectory dh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_dir_close(&fs._impl, &dh._impl))
  * 
  */
 
@@ -28664,15 +28653,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":471
+/* "littlefs/lfs.pyx":474
  *     return _raise_on_error(lfs_dir_close(&fs._impl, &dh._impl))
  * 
  * def dir_read(LFSFilesystem fs, LFSDirectory dh):             # <<<<<<<<<<<<<<
  *     cdef lfs_info * info = <lfs_info *>malloc(sizeof(lfs_info))
  *     try:
  */
 
@@ -28729,58 +28718,58 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 471, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 474, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_dh)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 471, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 474, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("dir_read", 1, 2, 2, 1); __PYX_ERR(0, 471, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("dir_read", 1, 2, 2, 1); __PYX_ERR(0, 474, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "dir_read") < 0)) __PYX_ERR(0, 471, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "dir_read") < 0)) __PYX_ERR(0, 474, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
     __pyx_v_dh = ((struct __pyx_obj_8littlefs_3lfs_LFSDirectory *)values[1]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("dir_read", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 471, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("dir_read", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 474, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.dir_read", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 471, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_dh), __pyx_ptype_8littlefs_3lfs_LFSDirectory, 1, "dh", 0))) __PYX_ERR(0, 471, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 474, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_dh), __pyx_ptype_8littlefs_3lfs_LFSDirectory, 1, "dh", 0))) __PYX_ERR(0, 474, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_54dir_read(__pyx_self, __pyx_v_fs, __pyx_v_dh);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -28818,92 +28807,92 @@
   PyObject *__pyx_t_17 = NULL;
   PyObject *__pyx_t_18 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dir_read", 1);
 
-  /* "littlefs/lfs.pyx":472
+  /* "littlefs/lfs.pyx":475
  * 
  * def dir_read(LFSFilesystem fs, LFSDirectory dh):
  *     cdef lfs_info * info = <lfs_info *>malloc(sizeof(lfs_info))             # <<<<<<<<<<<<<<
  *     try:
  *         retval = _raise_on_error(lfs_dir_read(&fs._impl, &dh._impl, info))
  */
   __pyx_v_info = ((struct lfs_info *)malloc((sizeof(struct lfs_info))));
 
-  /* "littlefs/lfs.pyx":473
+  /* "littlefs/lfs.pyx":476
  * def dir_read(LFSFilesystem fs, LFSDirectory dh):
  *     cdef lfs_info * info = <lfs_info *>malloc(sizeof(lfs_info))
  *     try:             # <<<<<<<<<<<<<<
  *         retval = _raise_on_error(lfs_dir_read(&fs._impl, &dh._impl, info))
  *         if retval == 0:
  */
   /*try:*/ {
 
-    /* "littlefs/lfs.pyx":474
+    /* "littlefs/lfs.pyx":477
  *     cdef lfs_info * info = <lfs_info *>malloc(sizeof(lfs_info))
  *     try:
  *         retval = _raise_on_error(lfs_dir_read(&fs._impl, &dh._impl, info))             # <<<<<<<<<<<<<<
  *         if retval == 0:
  *             return None
  */
-    __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_dir_read((&__pyx_v_fs->_impl), (&__pyx_v_dh->_impl), __pyx_v_info)); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 474, __pyx_L4_error)
+    __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_dir_read((&__pyx_v_fs->_impl), (&__pyx_v_dh->_impl), __pyx_v_info)); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 477, __pyx_L4_error)
     __pyx_v_retval = __pyx_t_1;
 
-    /* "littlefs/lfs.pyx":475
+    /* "littlefs/lfs.pyx":478
  *     try:
  *         retval = _raise_on_error(lfs_dir_read(&fs._impl, &dh._impl, info))
  *         if retval == 0:             # <<<<<<<<<<<<<<
  *             return None
  *         return LFSStat(info.type, info.size, info.name.decode(FILENAME_ENCODING))
  */
     __pyx_t_2 = (__pyx_v_retval == 0);
     if (__pyx_t_2) {
 
-      /* "littlefs/lfs.pyx":476
+      /* "littlefs/lfs.pyx":479
  *         retval = _raise_on_error(lfs_dir_read(&fs._impl, &dh._impl, info))
  *         if retval == 0:
  *             return None             # <<<<<<<<<<<<<<
  *         return LFSStat(info.type, info.size, info.name.decode(FILENAME_ENCODING))
  *     finally:
  */
       __Pyx_XDECREF(__pyx_r);
       __pyx_r = Py_None; __Pyx_INCREF(Py_None);
       goto __pyx_L3_return;
 
-      /* "littlefs/lfs.pyx":475
+      /* "littlefs/lfs.pyx":478
  *     try:
  *         retval = _raise_on_error(lfs_dir_read(&fs._impl, &dh._impl, info))
  *         if retval == 0:             # <<<<<<<<<<<<<<
  *             return None
  *         return LFSStat(info.type, info.size, info.name.decode(FILENAME_ENCODING))
  */
     }
 
-    /* "littlefs/lfs.pyx":477
+    /* "littlefs/lfs.pyx":480
  *         if retval == 0:
  *             return None
  *         return LFSStat(info.type, info.size, info.name.decode(FILENAME_ENCODING))             # <<<<<<<<<<<<<<
  *     finally:
  *         free(info)
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_LFSStat); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 477, __pyx_L4_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_LFSStat); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 480, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyInt_From_uint8_t(__pyx_v_info->type); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 477, __pyx_L4_error)
+    __pyx_t_5 = __Pyx_PyInt_From_uint8_t(__pyx_v_info->type); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 480, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyInt_From_uint32_t(__pyx_v_info->size); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 477, __pyx_L4_error)
+    __pyx_t_6 = __Pyx_PyInt_From_uint32_t(__pyx_v_info->size); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 480, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_8 = __Pyx_PyObject_FromString(__pyx_v_info->name); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 477, __pyx_L4_error)
+    __pyx_t_8 = __Pyx_PyObject_FromString(__pyx_v_info->name); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 480, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_decode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 477, __pyx_L4_error)
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_decode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 480, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_FILENAME_ENCODING); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 477, __pyx_L4_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_FILENAME_ENCODING); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 480, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_10 = NULL;
     __pyx_t_1 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_9))) {
       __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
       if (likely(__pyx_t_10)) {
@@ -28916,15 +28905,15 @@
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_10, __pyx_t_8};
       __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 477, __pyx_L4_error)
+      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 480, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     }
     __pyx_t_9 = NULL;
     __pyx_t_1 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_4))) {
@@ -28941,24 +28930,24 @@
     {
       PyObject *__pyx_callargs[4] = {__pyx_t_9, __pyx_t_5, __pyx_t_6, __pyx_t_7};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_1, 3+__pyx_t_1);
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 477, __pyx_L4_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 480, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L3_return;
   }
 
-  /* "littlefs/lfs.pyx":479
+  /* "littlefs/lfs.pyx":482
  *         return LFSStat(info.type, info.size, info.name.decode(FILENAME_ENCODING))
  *     finally:
  *         free(info)             # <<<<<<<<<<<<<<
  * 
  * def dir_tell(LFSFilesystem fs, LFSDirectory dh):
  */
   /*finally:*/ {
@@ -29007,15 +28996,15 @@
       free(__pyx_v_info);
       __pyx_r = __pyx_t_18;
       __pyx_t_18 = 0;
       goto __pyx_L0;
     }
   }
 
-  /* "littlefs/lfs.pyx":471
+  /* "littlefs/lfs.pyx":474
  *     return _raise_on_error(lfs_dir_close(&fs._impl, &dh._impl))
  * 
  * def dir_read(LFSFilesystem fs, LFSDirectory dh):             # <<<<<<<<<<<<<<
  *     cdef lfs_info * info = <lfs_info *>malloc(sizeof(lfs_info))
  *     try:
  */
 
@@ -29033,15 +29022,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":481
+/* "littlefs/lfs.pyx":484
  *         free(info)
  * 
  * def dir_tell(LFSFilesystem fs, LFSDirectory dh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_dir_tell(&fs._impl, &dh._impl))
  * 
  */
 
@@ -29098,58 +29087,58 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 481, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 484, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_dh)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 481, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 484, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("dir_tell", 1, 2, 2, 1); __PYX_ERR(0, 481, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("dir_tell", 1, 2, 2, 1); __PYX_ERR(0, 484, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "dir_tell") < 0)) __PYX_ERR(0, 481, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "dir_tell") < 0)) __PYX_ERR(0, 484, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
     __pyx_v_dh = ((struct __pyx_obj_8littlefs_3lfs_LFSDirectory *)values[1]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("dir_tell", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 481, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("dir_tell", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 484, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.dir_tell", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 481, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_dh), __pyx_ptype_8littlefs_3lfs_LFSDirectory, 1, "dh", 0))) __PYX_ERR(0, 481, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 484, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_dh), __pyx_ptype_8littlefs_3lfs_LFSDirectory, 1, "dh", 0))) __PYX_ERR(0, 484, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_56dir_tell(__pyx_self, __pyx_v_fs, __pyx_v_dh);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -29169,30 +29158,30 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dir_tell", 1);
 
-  /* "littlefs/lfs.pyx":482
+  /* "littlefs/lfs.pyx":485
  * 
  * def dir_tell(LFSFilesystem fs, LFSDirectory dh):
  *     return _raise_on_error(lfs_dir_tell(&fs._impl, &dh._impl))             # <<<<<<<<<<<<<<
  * 
  * def dir_rewind(LFSFilesystem fs, LFSDirectory dh):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_dir_tell((&__pyx_v_fs->_impl), (&__pyx_v_dh->_impl))); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 482, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 482, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_dir_tell((&__pyx_v_fs->_impl), (&__pyx_v_dh->_impl))); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 485, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 485, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":481
+  /* "littlefs/lfs.pyx":484
  *         free(info)
  * 
  * def dir_tell(LFSFilesystem fs, LFSDirectory dh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_dir_tell(&fs._impl, &dh._impl))
  * 
  */
 
@@ -29203,20 +29192,19 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "littlefs/lfs.pyx":484
+/* "littlefs/lfs.pyx":487
  *     return _raise_on_error(lfs_dir_tell(&fs._impl, &dh._impl))
  * 
  * def dir_rewind(LFSFilesystem fs, LFSDirectory dh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_dir_rewind(&fs._impl, &dh._impl))
- * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8littlefs_3lfs_59dir_rewind(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
@@ -29268,58 +29256,58 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 484, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 487, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_dh)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 484, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 487, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("dir_rewind", 1, 2, 2, 1); __PYX_ERR(0, 484, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("dir_rewind", 1, 2, 2, 1); __PYX_ERR(0, 487, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "dir_rewind") < 0)) __PYX_ERR(0, 484, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "dir_rewind") < 0)) __PYX_ERR(0, 487, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_fs = ((struct __pyx_obj_8littlefs_3lfs_LFSFilesystem *)values[0]);
     __pyx_v_dh = ((struct __pyx_obj_8littlefs_3lfs_LFSDirectory *)values[1]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("dir_rewind", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 484, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("dir_rewind", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 487, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("littlefs.lfs.dir_rewind", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 484, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_dh), __pyx_ptype_8littlefs_3lfs_LFSDirectory, 1, "dh", 0))) __PYX_ERR(0, 484, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fs), __pyx_ptype_8littlefs_3lfs_LFSFilesystem, 1, "fs", 0))) __PYX_ERR(0, 487, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_dh), __pyx_ptype_8littlefs_3lfs_LFSDirectory, 1, "dh", 0))) __PYX_ERR(0, 487, __pyx_L1_error)
   __pyx_r = __pyx_pf_8littlefs_3lfs_58dir_rewind(__pyx_self, __pyx_v_fs, __pyx_v_dh);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -29339,34 +29327,32 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dir_rewind", 1);
 
-  /* "littlefs/lfs.pyx":485
+  /* "littlefs/lfs.pyx":488
  * 
  * def dir_rewind(LFSFilesystem fs, LFSDirectory dh):
  *     return _raise_on_error(lfs_dir_rewind(&fs._impl, &dh._impl))             # <<<<<<<<<<<<<<
- * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_dir_rewind((&__pyx_v_fs->_impl), (&__pyx_v_dh->_impl))); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 485, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 485, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8littlefs_3lfs__raise_on_error(lfs_dir_rewind((&__pyx_v_fs->_impl), (&__pyx_v_dh->_impl))); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 488, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 488, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "littlefs/lfs.pyx":484
+  /* "littlefs/lfs.pyx":487
  *     return _raise_on_error(lfs_dir_tell(&fs._impl, &dh._impl))
  * 
  * def dir_rewind(LFSFilesystem fs, LFSDirectory dh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_dir_rewind(&fs._impl, &dh._impl))
- * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_AddTraceback("littlefs.lfs.dir_rewind", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
@@ -31213,44 +31199,45 @@
     {&__pyx_n_s_LFSConfig, __pyx_k_LFSConfig, sizeof(__pyx_k_LFSConfig), 0, 0, 1, 1},
     {&__pyx_n_s_LFSConfig___reduce_cython, __pyx_k_LFSConfig___reduce_cython, sizeof(__pyx_k_LFSConfig___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_LFSConfig___setstate_cython, __pyx_k_LFSConfig___setstate_cython, sizeof(__pyx_k_LFSConfig___setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_LFSDirectory, __pyx_k_LFSDirectory, sizeof(__pyx_k_LFSDirectory), 0, 0, 1, 1},
     {&__pyx_n_s_LFSDirectory___reduce_cython, __pyx_k_LFSDirectory___reduce_cython, sizeof(__pyx_k_LFSDirectory___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_LFSDirectory___setstate_cython, __pyx_k_LFSDirectory___setstate_cython, sizeof(__pyx_k_LFSDirectory___setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_LFSFSStat, __pyx_k_LFSFSStat, sizeof(__pyx_k_LFSFSStat), 0, 0, 1, 1},
-    {&__pyx_n_u_LFSFSStat, __pyx_k_LFSFSStat, sizeof(__pyx_k_LFSFSStat), 0, 1, 0, 1},
     {&__pyx_n_s_LFSFile, __pyx_k_LFSFile, sizeof(__pyx_k_LFSFile), 0, 0, 1, 1},
     {&__pyx_n_s_LFSFileFlag, __pyx_k_LFSFileFlag, sizeof(__pyx_k_LFSFileFlag), 0, 0, 1, 1},
     {&__pyx_n_s_LFSFile___reduce_cython, __pyx_k_LFSFile___reduce_cython, sizeof(__pyx_k_LFSFile___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_LFSFile___setstate_cython, __pyx_k_LFSFile___setstate_cython, sizeof(__pyx_k_LFSFile___setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_LFSFilesystem, __pyx_k_LFSFilesystem, sizeof(__pyx_k_LFSFilesystem), 0, 0, 1, 1},
     {&__pyx_n_s_LFSFilesystem___reduce_cython, __pyx_k_LFSFilesystem___reduce_cython, sizeof(__pyx_k_LFSFilesystem___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_LFSFilesystem___setstate_cython, __pyx_k_LFSFilesystem___setstate_cython, sizeof(__pyx_k_LFSFilesystem___setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_LFSStat, __pyx_k_LFSStat, sizeof(__pyx_k_LFSStat), 0, 0, 1, 1},
-    {&__pyx_n_u_LFSStat, __pyx_k_LFSStat, sizeof(__pyx_k_LFSStat), 0, 1, 0, 1},
     {&__pyx_n_s_LFS_DISK_VERSION, __pyx_k_LFS_DISK_VERSION, sizeof(__pyx_k_LFS_DISK_VERSION), 0, 0, 1, 1},
     {&__pyx_n_s_LFS_VERSION, __pyx_k_LFS_VERSION, sizeof(__pyx_k_LFS_VERSION), 0, 0, 1, 1},
     {&__pyx_n_s_LittleFSError, __pyx_k_LittleFSError, sizeof(__pyx_k_LittleFSError), 0, 0, 1, 1},
-    {&__pyx_kp_u_Littlefs_File_Directory_status, __pyx_k_Littlefs_File_Directory_status, sizeof(__pyx_k_Littlefs_File_Directory_status), 0, 1, 0, 0},
+    {&__pyx_kp_s_Littlefs_File_Directory_status, __pyx_k_Littlefs_File_Directory_status, sizeof(__pyx_k_Littlefs_File_Directory_status), 0, 0, 1, 0},
     {&__pyx_kp_s_Littlefs_file_mode_flags, __pyx_k_Littlefs_file_mode_flags, sizeof(__pyx_k_Littlefs_file_mode_flags), 0, 0, 1, 0},
-    {&__pyx_kp_u_Littlefs_filesystem_status, __pyx_k_Littlefs_filesystem_status, sizeof(__pyx_k_Littlefs_filesystem_status), 0, 1, 0, 0},
+    {&__pyx_kp_s_Littlefs_filesystem_status, __pyx_k_Littlefs_filesystem_status, sizeof(__pyx_k_Littlefs_filesystem_status), 0, 0, 1, 0},
     {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
     {&__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_k_MemoryView_of_r_at_0x_x, sizeof(__pyx_k_MemoryView_of_r_at_0x_x), 0, 0, 1, 0},
     {&__pyx_kp_s_MemoryView_of_r_object, __pyx_k_MemoryView_of_r_object, sizeof(__pyx_k_MemoryView_of_r_object), 0, 0, 1, 0},
     {&__pyx_kp_u_Minimal_block_size_is_128, __pyx_k_Minimal_block_size_is_128, sizeof(__pyx_k_Minimal_block_size_is_128), 0, 1, 0, 0},
+    {&__pyx_n_s_NamedTuple, __pyx_k_NamedTuple, sizeof(__pyx_k_NamedTuple), 0, 0, 1, 1},
     {&__pyx_n_s_NotImplementedError, __pyx_k_NotImplementedError, sizeof(__pyx_k_NotImplementedError), 0, 0, 1, 1},
     {&__pyx_kp_u_Not_all_data_written, __pyx_k_Not_all_data_written, sizeof(__pyx_k_Not_all_data_written), 0, 1, 0, 0},
     {&__pyx_n_b_O, __pyx_k_O, sizeof(__pyx_k_O), 0, 0, 0, 1},
     {&__pyx_kp_u_Out_of_bounds_on_buffer_access_a, __pyx_k_Out_of_bounds_on_buffer_access_a, sizeof(__pyx_k_Out_of_bounds_on_buffer_access_a), 0, 1, 0, 0},
     {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
     {&__pyx_kp_s_Pickling_of_struct_members_such, __pyx_k_Pickling_of_struct_members_such, sizeof(__pyx_k_Pickling_of_struct_members_such), 0, 0, 1, 0},
     {&__pyx_n_s_RuntimeError, __pyx_k_RuntimeError, sizeof(__pyx_k_RuntimeError), 0, 0, 1, 1},
     {&__pyx_n_s_Sequence, __pyx_k_Sequence, sizeof(__pyx_k_Sequence), 0, 0, 1, 1},
     {&__pyx_kp_u_Size_must_be_0, __pyx_k_Size_must_be_0, sizeof(__pyx_k_Size_must_be_0), 0, 1, 0, 0},
     {&__pyx_kp_s_Step_may_not_be_zero_axis_d, __pyx_k_Step_may_not_be_zero_axis_d, sizeof(__pyx_k_Step_may_not_be_zero_axis_d), 0, 0, 1, 0},
+    {&__pyx_n_s_TYPE_DIR, __pyx_k_TYPE_DIR, sizeof(__pyx_k_TYPE_DIR), 0, 0, 1, 1},
+    {&__pyx_n_s_TYPE_REG, __pyx_k_TYPE_REG, sizeof(__pyx_k_TYPE_REG), 0, 0, 1, 1},
     {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
     {&__pyx_kp_s_Unable_to_convert_item_to_object, __pyx_k_Unable_to_convert_item_to_object, sizeof(__pyx_k_Unable_to_convert_item_to_object), 0, 0, 1, 0},
     {&__pyx_n_s_UserContext, __pyx_k_UserContext, sizeof(__pyx_k_UserContext), 0, 0, 1, 1},
     {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
     {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
     {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
     {&__pyx_kp_u__23, __pyx_k__23, sizeof(__pyx_k__23), 0, 1, 0, 0},
@@ -31260,32 +31247,30 @@
     {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
     {&__pyx_kp_u__7, __pyx_k__7, sizeof(__pyx_k__7), 0, 1, 0, 0},
     {&__pyx_n_s__99, __pyx_k__99, sizeof(__pyx_k__99), 0, 0, 1, 1},
     {&__pyx_n_u_a, __pyx_k_a, sizeof(__pyx_k_a), 0, 1, 0, 1},
     {&__pyx_n_s_abc, __pyx_k_abc, sizeof(__pyx_k_abc), 0, 0, 1, 1},
     {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
     {&__pyx_kp_u_and, __pyx_k_and, sizeof(__pyx_k_and), 0, 1, 0, 0},
+    {&__pyx_n_s_annotations, __pyx_k_annotations, sizeof(__pyx_k_annotations), 0, 0, 1, 1},
     {&__pyx_n_s_append, __pyx_k_append, sizeof(__pyx_k_append), 0, 0, 1, 1},
     {&__pyx_n_s_appending, __pyx_k_appending, sizeof(__pyx_k_appending), 0, 0, 1, 1},
     {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
     {&__pyx_n_u_ascii, __pyx_k_ascii, sizeof(__pyx_k_ascii), 0, 1, 0, 1},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_attr_max, __pyx_k_attr_max, sizeof(__pyx_k_attr_max), 0, 0, 1, 1},
-    {&__pyx_n_u_attr_max, __pyx_k_attr_max, sizeof(__pyx_k_attr_max), 0, 1, 0, 1},
     {&__pyx_kp_u_attr_max_2, __pyx_k_attr_max_2, sizeof(__pyx_k_attr_max_2), 0, 1, 0, 0},
     {&__pyx_n_s_attr_size, __pyx_k_attr_size, sizeof(__pyx_k_attr_size), 0, 0, 1, 1},
     {&__pyx_n_u_b, __pyx_k_b, sizeof(__pyx_k_b), 0, 1, 0, 1},
     {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
     {&__pyx_n_s_block_count, __pyx_k_block_count, sizeof(__pyx_k_block_count), 0, 0, 1, 1},
-    {&__pyx_n_u_block_count, __pyx_k_block_count, sizeof(__pyx_k_block_count), 0, 1, 0, 1},
     {&__pyx_kp_u_block_count_2, __pyx_k_block_count_2, sizeof(__pyx_k_block_count_2), 0, 1, 0, 0},
     {&__pyx_n_s_block_cycles, __pyx_k_block_cycles, sizeof(__pyx_k_block_cycles), 0, 0, 1, 1},
     {&__pyx_kp_u_block_cycles_2, __pyx_k_block_cycles_2, sizeof(__pyx_k_block_cycles_2), 0, 1, 0, 0},
     {&__pyx_n_s_block_size, __pyx_k_block_size, sizeof(__pyx_k_block_size), 0, 0, 1, 1},
-    {&__pyx_n_u_block_size, __pyx_k_block_size, sizeof(__pyx_k_block_size), 0, 1, 0, 1},
     {&__pyx_kp_u_block_size_2, __pyx_k_block_size_2, sizeof(__pyx_k_block_size_2), 0, 1, 0, 0},
     {&__pyx_n_s_buf, __pyx_k_buf, sizeof(__pyx_k_buf), 0, 0, 1, 1},
     {&__pyx_n_s_buf_view, __pyx_k_buf_view, sizeof(__pyx_k_buf_view), 0, 0, 1, 1},
     {&__pyx_n_s_buffer, __pyx_k_buffer, sizeof(__pyx_k_buffer), 0, 0, 1, 1},
     {&__pyx_n_s_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 0, 1, 1},
     {&__pyx_n_u_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 1, 0, 1},
     {&__pyx_n_s_cache_size, __pyx_k_cache_size, sizeof(__pyx_k_cache_size), 0, 0, 1, 1},
@@ -31314,15 +31299,14 @@
     {&__pyx_n_s_dir_close, __pyx_k_dir_close, sizeof(__pyx_k_dir_close), 0, 0, 1, 1},
     {&__pyx_n_s_dir_open, __pyx_k_dir_open, sizeof(__pyx_k_dir_open), 0, 0, 1, 1},
     {&__pyx_n_s_dir_read, __pyx_k_dir_read, sizeof(__pyx_k_dir_read), 0, 0, 1, 1},
     {&__pyx_n_s_dir_rewind, __pyx_k_dir_rewind, sizeof(__pyx_k_dir_rewind), 0, 0, 1, 1},
     {&__pyx_n_s_dir_tell, __pyx_k_dir_tell, sizeof(__pyx_k_dir_tell), 0, 0, 1, 1},
     {&__pyx_kp_u_disable, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
     {&__pyx_n_s_disk_version, __pyx_k_disk_version, sizeof(__pyx_k_disk_version), 0, 0, 1, 1},
-    {&__pyx_n_u_disk_version, __pyx_k_disk_version, sizeof(__pyx_k_disk_version), 0, 1, 0, 1},
     {&__pyx_kp_u_disk_version_2, __pyx_k_disk_version_2, sizeof(__pyx_k_disk_version_2), 0, 1, 0, 0},
     {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
     {&__pyx_n_s_dtype_is_object, __pyx_k_dtype_is_object, sizeof(__pyx_k_dtype_is_object), 0, 0, 1, 1},
     {&__pyx_kp_u_enable, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
     {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
     {&__pyx_n_s_enum, __pyx_k_enum, sizeof(__pyx_k_enum), 0, 0, 1, 1},
     {&__pyx_n_s_enumerate, __pyx_k_enumerate, sizeof(__pyx_k_enumerate), 0, 0, 1, 1},
@@ -31330,15 +31314,14 @@
     {&__pyx_n_s_error, __pyx_k_error, sizeof(__pyx_k_error), 0, 0, 1, 1},
     {&__pyx_n_s_errors, __pyx_k_errors, sizeof(__pyx_k_errors), 0, 0, 1, 1},
     {&__pyx_n_s_excl, __pyx_k_excl, sizeof(__pyx_k_excl), 0, 0, 1, 1},
     {&__pyx_n_s_exclusive_modes, __pyx_k_exclusive_modes, sizeof(__pyx_k_exclusive_modes), 0, 0, 1, 1},
     {&__pyx_n_s_fh, __pyx_k_fh, sizeof(__pyx_k_fh), 0, 0, 1, 1},
     {&__pyx_n_s_file_close, __pyx_k_file_close, sizeof(__pyx_k_file_close), 0, 0, 1, 1},
     {&__pyx_n_s_file_max, __pyx_k_file_max, sizeof(__pyx_k_file_max), 0, 0, 1, 1},
-    {&__pyx_n_u_file_max, __pyx_k_file_max, sizeof(__pyx_k_file_max), 0, 1, 0, 1},
     {&__pyx_kp_u_file_max_2, __pyx_k_file_max_2, sizeof(__pyx_k_file_max_2), 0, 1, 0, 0},
     {&__pyx_n_s_file_open, __pyx_k_file_open, sizeof(__pyx_k_file_open), 0, 0, 1, 1},
     {&__pyx_n_s_file_open_cfg, __pyx_k_file_open_cfg, sizeof(__pyx_k_file_open_cfg), 0, 0, 1, 1},
     {&__pyx_n_s_file_open_locals_genexpr, __pyx_k_file_open_locals_genexpr, sizeof(__pyx_k_file_open_locals_genexpr), 0, 0, 1, 1},
     {&__pyx_n_s_file_read, __pyx_k_file_read, sizeof(__pyx_k_file_read), 0, 0, 1, 1},
     {&__pyx_n_s_file_rewind, __pyx_k_file_rewind, sizeof(__pyx_k_file_rewind), 0, 0, 1, 1},
     {&__pyx_n_s_file_seek, __pyx_k_file_seek, sizeof(__pyx_k_file_seek), 0, 0, 1, 1},
@@ -31389,21 +31372,18 @@
     {&__pyx_n_s_mkdir, __pyx_k_mkdir, sizeof(__pyx_k_mkdir), 0, 0, 1, 1},
     {&__pyx_n_s_mode, __pyx_k_mode, sizeof(__pyx_k_mode), 0, 0, 1, 1},
     {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
     {&__pyx_n_s_mount, __pyx_k_mount, sizeof(__pyx_k_mount), 0, 0, 1, 1},
     {&__pyx_n_s_mro_entries, __pyx_k_mro_entries, sizeof(__pyx_k_mro_entries), 0, 0, 1, 1},
     {&__pyx_kp_u_must_have_exactly_one_of_create, __pyx_k_must_have_exactly_one_of_create, sizeof(__pyx_k_must_have_exactly_one_of_create), 0, 1, 0, 0},
     {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
-    {&__pyx_n_u_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 1, 0, 1},
     {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
     {&__pyx_n_s_name_max, __pyx_k_name_max, sizeof(__pyx_k_name_max), 0, 0, 1, 1},
-    {&__pyx_n_u_name_max, __pyx_k_name_max, sizeof(__pyx_k_name_max), 0, 1, 0, 1},
     {&__pyx_kp_u_name_max_2, __pyx_k_name_max_2, sizeof(__pyx_k_name_max_2), 0, 1, 0, 0},
     {&__pyx_kp_u_name_max_must_be_1022, __pyx_k_name_max_must_be_1022, sizeof(__pyx_k_name_max_must_be_1022), 0, 1, 0, 0},
-    {&__pyx_n_s_namedtuple, __pyx_k_namedtuple, sizeof(__pyx_k_namedtuple), 0, 0, 1, 1},
     {&__pyx_n_s_ndim, __pyx_k_ndim, sizeof(__pyx_k_ndim), 0, 0, 1, 1},
     {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
     {&__pyx_n_s_newpath, __pyx_k_newpath, sizeof(__pyx_k_newpath), 0, 0, 1, 1},
     {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
     {&__pyx_n_s_obj, __pyx_k_obj, sizeof(__pyx_k_obj), 0, 0, 1, 1},
     {&__pyx_n_s_off, __pyx_k_off, sizeof(__pyx_k_off), 0, 0, 1, 1},
     {&__pyx_n_s_oldpath, __pyx_k_oldpath, sizeof(__pyx_k_oldpath), 0, 0, 1, 1},
@@ -31445,36 +31425,37 @@
     {&__pyx_n_s_send, __pyx_k_send, sizeof(__pyx_k_send), 0, 0, 1, 1},
     {&__pyx_n_s_set_name, __pyx_k_set_name, sizeof(__pyx_k_set_name), 0, 0, 1, 1},
     {&__pyx_n_s_setattr, __pyx_k_setattr, sizeof(__pyx_k_setattr), 0, 0, 1, 1},
     {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
     {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_shape, __pyx_k_shape, sizeof(__pyx_k_shape), 0, 0, 1, 1},
     {&__pyx_n_s_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 0, 1, 1},
-    {&__pyx_n_u_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 1, 0, 1},
     {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
     {&__pyx_kp_s_src_littlefs_lfs_pyx, __pyx_k_src_littlefs_lfs_pyx, sizeof(__pyx_k_src_littlefs_lfs_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_start, __pyx_k_start, sizeof(__pyx_k_start), 0, 0, 1, 1},
     {&__pyx_n_s_stat, __pyx_k_stat, sizeof(__pyx_k_stat), 0, 0, 1, 1},
     {&__pyx_n_s_step, __pyx_k_step, sizeof(__pyx_k_step), 0, 0, 1, 1},
     {&__pyx_n_s_stop, __pyx_k_stop, sizeof(__pyx_k_stop), 0, 0, 1, 1},
+    {&__pyx_n_s_str, __pyx_k_str, sizeof(__pyx_k_str), 0, 0, 1, 1},
     {&__pyx_kp_s_strided_and_direct, __pyx_k_strided_and_direct, sizeof(__pyx_k_strided_and_direct), 0, 0, 1, 0},
     {&__pyx_kp_s_strided_and_direct_or_indirect, __pyx_k_strided_and_direct_or_indirect, sizeof(__pyx_k_strided_and_direct_or_indirect), 0, 0, 1, 0},
     {&__pyx_kp_s_strided_and_indirect, __pyx_k_strided_and_indirect, sizeof(__pyx_k_strided_and_indirect), 0, 0, 1, 0},
     {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
     {&__pyx_n_s_struct, __pyx_k_struct, sizeof(__pyx_k_struct), 0, 0, 1, 1},
     {&__pyx_n_s_sum, __pyx_k_sum, sizeof(__pyx_k_sum), 0, 0, 1, 1},
     {&__pyx_n_s_super, __pyx_k_super, sizeof(__pyx_k_super), 0, 0, 1, 1},
     {&__pyx_n_s_sync, __pyx_k_sync, sizeof(__pyx_k_sync), 0, 0, 1, 1},
     {&__pyx_n_s_sys, __pyx_k_sys, sizeof(__pyx_k_sys), 0, 0, 1, 1},
     {&__pyx_n_u_t, __pyx_k_t, sizeof(__pyx_k_t), 0, 1, 0, 1},
     {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
     {&__pyx_n_s_throw, __pyx_k_throw, sizeof(__pyx_k_throw), 0, 0, 1, 1},
     {&__pyx_n_s_trunc, __pyx_k_trunc, sizeof(__pyx_k_trunc), 0, 0, 1, 1},
     {&__pyx_n_s_typ, __pyx_k_typ, sizeof(__pyx_k_typ), 0, 0, 1, 1},
-    {&__pyx_n_u_type, __pyx_k_type, sizeof(__pyx_k_type), 0, 1, 0, 1},
+    {&__pyx_n_s_type, __pyx_k_type, sizeof(__pyx_k_type), 0, 0, 1, 1},
+    {&__pyx_n_s_typing, __pyx_k_typing, sizeof(__pyx_k_typing), 0, 0, 1, 1},
     {&__pyx_kp_s_unable_to_allocate_array_data, __pyx_k_unable_to_allocate_array_data, sizeof(__pyx_k_unable_to_allocate_array_data), 0, 0, 1, 0},
     {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
     {&__pyx_n_s_unmount, __pyx_k_unmount, sizeof(__pyx_k_unmount), 0, 0, 1, 1},
     {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
     {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
     {&__pyx_n_s_updating, __pyx_k_updating, sizeof(__pyx_k_updating), 0, 0, 1, 1},
     {&__pyx_n_s_user_context, __pyx_k_user_context, sizeof(__pyx_k_user_context), 0, 0, 1, 1},
@@ -31487,20 +31468,20 @@
     {&__pyx_kp_b_xff, __pyx_k_xff, sizeof(__pyx_k_xff), 0, 0, 0, 0},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 153, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 156, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
-  __pyx_builtin_sum = __Pyx_GetBuiltinName(__pyx_n_s_sum); if (!__pyx_builtin_sum) __PYX_ERR(0, 390, __pyx_L1_error)
-  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 414, __pyx_L1_error)
-  __pyx_builtin_AssertionError = __Pyx_GetBuiltinName(__pyx_n_s_AssertionError); if (!__pyx_builtin_AssertionError) __PYX_ERR(0, 426, __pyx_L1_error)
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 437, __pyx_L1_error)
+  __pyx_builtin_sum = __Pyx_GetBuiltinName(__pyx_n_s_sum); if (!__pyx_builtin_sum) __PYX_ERR(0, 393, __pyx_L1_error)
+  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 417, __pyx_L1_error)
+  __pyx_builtin_AssertionError = __Pyx_GetBuiltinName(__pyx_n_s_AssertionError); if (!__pyx_builtin_AssertionError) __PYX_ERR(0, 429, __pyx_L1_error)
+  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 440, __pyx_L1_error)
   __pyx_builtin___import__ = __Pyx_GetBuiltinName(__pyx_n_s_import); if (!__pyx_builtin___import__) __PYX_ERR(1, 100, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 156, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 159, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(1, 261, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 408, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 618, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 914, __pyx_L1_error)
@@ -31546,55 +31527,55 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "littlefs/lfs.pyx":153
+  /* "littlefs/lfs.pyx":156
  * 
  *         if block_size < 128:
  *             raise ValueError('Minimal block size is 128')             # <<<<<<<<<<<<<<
  * 
  *         if name_max > 1022:  # LittleFS maximum name length limitation
  */
-  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_u_Minimal_block_size_is_128); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 153, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_u_Minimal_block_size_is_128); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__21);
   __Pyx_GIVEREF(__pyx_tuple__21);
 
-  /* "littlefs/lfs.pyx":156
+  /* "littlefs/lfs.pyx":159
  * 
  *         if name_max > 1022:  # LittleFS maximum name length limitation
  *             raise ValueError(f"name_max must be <=1022.")             # <<<<<<<<<<<<<<
  * 
  *         self._impl.read_size = read_size if read_size else block_size
  */
-  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_u_name_max_must_be_1022); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 156, __pyx_L1_error)
+  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_u_name_max_must_be_1022); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__22);
   __Pyx_GIVEREF(__pyx_tuple__22);
 
-  /* "littlefs/lfs.pyx":391
+  /* "littlefs/lfs.pyx":394
  * 
  *         if sum(int(m) for m in exclusive_modes) > 1:
  *             raise ValueError(             # <<<<<<<<<<<<<<
  *                 "must have exactly one of create/read/write/append mode"
  *             )
  */
-  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_u_must_have_exactly_one_of_create); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_u_must_have_exactly_one_of_create); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 394, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__26);
   __Pyx_GIVEREF(__pyx_tuple__26);
 
-  /* "littlefs/lfs.pyx":437
+  /* "littlefs/lfs.pyx":440
  *     code =_raise_on_error(lfs_file_write(&fs._impl, &fh._impl, <char *>data, len(data)))
  *     if code != len(data):
  *         raise RuntimeError("Not all data written")             # <<<<<<<<<<<<<<
  *     return code
  * 
  */
-  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_u_Not_all_data_written); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 437, __pyx_L1_error)
+  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_u_Not_all_data_written); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 440, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__27);
   __Pyx_GIVEREF(__pyx_tuple__27);
 
   /* "View.MemoryView":100
  * cdef object __pyx_collections_abc_Sequence "__pyx_collections_abc_Sequence"
  * try:
  *     if __import__("sys").version_info >= (3, 3):             # <<<<<<<<<<<<<<
@@ -31751,343 +31732,342 @@
  * def __reduce_cython__(self):
  *     raise TypeError, "Pickling of struct members such as self._impl must be explicitly requested with @auto_pickle(True)"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "Pickling of struct members such as self._impl must be explicitly requested with @auto_pickle(True)"
  */
   __pyx_codeobj__48 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__48)) __PYX_ERR(1, 3, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":263
+  /* "littlefs/lfs.pyx":266
  * 
  * 
  * def fs_stat(LFSFilesystem fs):             # <<<<<<<<<<<<<<
  *     """Get filesystem status"""
  *     cdef lfs_fsinfo * info = <lfs_fsinfo *>malloc(sizeof(lfs_fsinfo))
  */
-  __pyx_tuple__49 = PyTuple_Pack(2, __pyx_n_s_fs, __pyx_n_s_info); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(0, 263, __pyx_L1_error)
+  __pyx_tuple__49 = PyTuple_Pack(2, __pyx_n_s_fs, __pyx_n_s_info); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(0, 266, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__49);
   __Pyx_GIVEREF(__pyx_tuple__49);
-  __pyx_codeobj__50 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__49, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_fs_stat, 263, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__50)) __PYX_ERR(0, 263, __pyx_L1_error)
+  __pyx_codeobj__50 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__49, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_fs_stat, 266, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__50)) __PYX_ERR(0, 266, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":280
+  /* "littlefs/lfs.pyx":283
  * 
  * 
  * def fs_size(LFSFilesystem fs):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_fs_size(&fs._impl))
  * 
  */
-  __pyx_tuple__51 = PyTuple_Pack(1, __pyx_n_s_fs); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(0, 280, __pyx_L1_error)
+  __pyx_tuple__51 = PyTuple_Pack(1, __pyx_n_s_fs); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__51);
   __Pyx_GIVEREF(__pyx_tuple__51);
-  __pyx_codeobj__52 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__51, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_fs_size, 280, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__52)) __PYX_ERR(0, 280, __pyx_L1_error)
+  __pyx_codeobj__52 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__51, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_fs_size, 283, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__52)) __PYX_ERR(0, 283, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":284
+  /* "littlefs/lfs.pyx":287
  * 
  * 
  * def format(LFSFilesystem fs, LFSConfig cfg):             # <<<<<<<<<<<<<<
  *     """Format the filesystem"""
  *     return _raise_on_error(lfs_format(&fs._impl, &cfg._impl))
  */
-  __pyx_tuple__53 = PyTuple_Pack(2, __pyx_n_s_fs, __pyx_n_s_cfg); if (unlikely(!__pyx_tuple__53)) __PYX_ERR(0, 284, __pyx_L1_error)
+  __pyx_tuple__53 = PyTuple_Pack(2, __pyx_n_s_fs, __pyx_n_s_cfg); if (unlikely(!__pyx_tuple__53)) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__53);
   __Pyx_GIVEREF(__pyx_tuple__53);
-  __pyx_codeobj__54 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__53, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_format, 284, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__54)) __PYX_ERR(0, 284, __pyx_L1_error)
+  __pyx_codeobj__54 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__53, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_format, 287, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__54)) __PYX_ERR(0, 287, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":289
+  /* "littlefs/lfs.pyx":292
  * 
  * 
  * def mount(LFSFilesystem fs, LFSConfig cfg):             # <<<<<<<<<<<<<<
  *     """Mount the filesystem"""
  *     return _raise_on_error(lfs_mount(&fs._impl, &cfg._impl))
  */
-  __pyx_codeobj__55 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__53, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_mount, 289, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__55)) __PYX_ERR(0, 289, __pyx_L1_error)
+  __pyx_codeobj__55 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__53, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_mount, 292, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__55)) __PYX_ERR(0, 292, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":294
+  /* "littlefs/lfs.pyx":297
  * 
  * 
  * def unmount(LFSFilesystem fs):             # <<<<<<<<<<<<<<
  *     """Unmount the filesystem
  * 
  */
-  __pyx_codeobj__56 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__51, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_unmount, 294, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__56)) __PYX_ERR(0, 294, __pyx_L1_error)
+  __pyx_codeobj__56 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__51, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_unmount, 297, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__56)) __PYX_ERR(0, 297, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":302
+  /* "littlefs/lfs.pyx":305
  * 
  * 
  * def fs_mkconsistent(LFSFilesystem fs):             # <<<<<<<<<<<<<<
  *     """Attempt to make the filesystem consistent and ready for writing"""
  *     return _raise_on_error(lfs_fs_mkconsistent(&fs._impl))
  */
-  __pyx_codeobj__57 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__51, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_fs_mkconsistent, 302, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__57)) __PYX_ERR(0, 302, __pyx_L1_error)
+  __pyx_codeobj__57 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__51, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_fs_mkconsistent, 305, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__57)) __PYX_ERR(0, 305, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":307
+  /* "littlefs/lfs.pyx":310
  * 
  * 
  * def fs_grow(LFSFilesystem fs, block_count) -> int:             # <<<<<<<<<<<<<<
  *     """Irreversibly grows the filesystem to a new size.
  * 
  */
-  __pyx_tuple__58 = PyTuple_Pack(2, __pyx_n_s_fs, __pyx_n_s_block_count); if (unlikely(!__pyx_tuple__58)) __PYX_ERR(0, 307, __pyx_L1_error)
+  __pyx_tuple__58 = PyTuple_Pack(2, __pyx_n_s_fs, __pyx_n_s_block_count); if (unlikely(!__pyx_tuple__58)) __PYX_ERR(0, 310, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__58);
   __Pyx_GIVEREF(__pyx_tuple__58);
-  __pyx_codeobj__59 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__58, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_fs_grow, 307, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__59)) __PYX_ERR(0, 307, __pyx_L1_error)
+  __pyx_codeobj__59 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__58, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_fs_grow, 310, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__59)) __PYX_ERR(0, 310, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":319
+  /* "littlefs/lfs.pyx":322
  * 
  * 
  * def remove(LFSFilesystem fs, path):             # <<<<<<<<<<<<<<
  *     """Remove a file or directory
  * 
  */
-  __pyx_tuple__60 = PyTuple_Pack(2, __pyx_n_s_fs, __pyx_n_s_path); if (unlikely(!__pyx_tuple__60)) __PYX_ERR(0, 319, __pyx_L1_error)
+  __pyx_tuple__60 = PyTuple_Pack(2, __pyx_n_s_fs, __pyx_n_s_path); if (unlikely(!__pyx_tuple__60)) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__60);
   __Pyx_GIVEREF(__pyx_tuple__60);
-  __pyx_codeobj__61 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__60, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_remove, 319, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__61)) __PYX_ERR(0, 319, __pyx_L1_error)
+  __pyx_codeobj__61 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__60, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_remove, 322, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__61)) __PYX_ERR(0, 322, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":326
+  /* "littlefs/lfs.pyx":329
  *     return _raise_on_error(lfs_remove(&fs._impl, path.encode(FILENAME_ENCODING)))
  * 
  * def rename(LFSFilesystem fs, oldpath, newpath):             # <<<<<<<<<<<<<<
  *     """Rename or move a file or directory
  * 
  */
-  __pyx_tuple__62 = PyTuple_Pack(3, __pyx_n_s_fs, __pyx_n_s_oldpath, __pyx_n_s_newpath); if (unlikely(!__pyx_tuple__62)) __PYX_ERR(0, 326, __pyx_L1_error)
+  __pyx_tuple__62 = PyTuple_Pack(3, __pyx_n_s_fs, __pyx_n_s_oldpath, __pyx_n_s_newpath); if (unlikely(!__pyx_tuple__62)) __PYX_ERR(0, 329, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__62);
   __Pyx_GIVEREF(__pyx_tuple__62);
-  __pyx_codeobj__63 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__62, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_rename, 326, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__63)) __PYX_ERR(0, 326, __pyx_L1_error)
+  __pyx_codeobj__63 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__62, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_rename, 329, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__63)) __PYX_ERR(0, 329, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":336
+  /* "littlefs/lfs.pyx":339
  * 
  * 
  * def stat(LFSFilesystem fs, path):             # <<<<<<<<<<<<<<
  *     """Find info about a file or directory"""
  *     cdef lfs_info * info = <lfs_info *>malloc(sizeof(lfs_info))
  */
-  __pyx_tuple__64 = PyTuple_Pack(3, __pyx_n_s_fs, __pyx_n_s_path, __pyx_n_s_info); if (unlikely(!__pyx_tuple__64)) __PYX_ERR(0, 336, __pyx_L1_error)
+  __pyx_tuple__64 = PyTuple_Pack(3, __pyx_n_s_fs, __pyx_n_s_path, __pyx_n_s_info); if (unlikely(!__pyx_tuple__64)) __PYX_ERR(0, 339, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__64);
   __Pyx_GIVEREF(__pyx_tuple__64);
-  __pyx_codeobj__65 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__64, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_stat, 336, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__65)) __PYX_ERR(0, 336, __pyx_L1_error)
+  __pyx_codeobj__65 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__64, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_stat, 339, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__65)) __PYX_ERR(0, 339, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":346
+  /* "littlefs/lfs.pyx":349
  * 
  * 
  * def getattr(LFSFilesystem fs, path, typ):             # <<<<<<<<<<<<<<
  *     buf = bytearray(LFS_ATTR_MAX)
  *     cdef unsigned char[::1] buf_view = buf
  */
-  __pyx_tuple__66 = PyTuple_Pack(6, __pyx_n_s_fs, __pyx_n_s_path, __pyx_n_s_typ, __pyx_n_s_buf, __pyx_n_s_buf_view, __pyx_n_s_attr_size); if (unlikely(!__pyx_tuple__66)) __PYX_ERR(0, 346, __pyx_L1_error)
+  __pyx_tuple__66 = PyTuple_Pack(6, __pyx_n_s_fs, __pyx_n_s_path, __pyx_n_s_typ, __pyx_n_s_buf, __pyx_n_s_buf_view, __pyx_n_s_attr_size); if (unlikely(!__pyx_tuple__66)) __PYX_ERR(0, 349, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__66);
   __Pyx_GIVEREF(__pyx_tuple__66);
-  __pyx_codeobj__67 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__66, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_getattr, 346, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__67)) __PYX_ERR(0, 346, __pyx_L1_error)
+  __pyx_codeobj__67 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__66, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_getattr, 349, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__67)) __PYX_ERR(0, 349, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":353
+  /* "littlefs/lfs.pyx":356
  * 
  * 
  * def setattr(LFSFilesystem fs, path, typ, data):             # <<<<<<<<<<<<<<
  *     cdef const unsigned char[::1] buf_view = data
  *     _raise_on_error(lfs_setattr(&fs._impl, path.encode(FILENAME_ENCODING), typ, &buf_view[0], len(data)))
  */
-  __pyx_tuple__68 = PyTuple_Pack(5, __pyx_n_s_fs, __pyx_n_s_path, __pyx_n_s_typ, __pyx_n_s_data, __pyx_n_s_buf_view); if (unlikely(!__pyx_tuple__68)) __PYX_ERR(0, 353, __pyx_L1_error)
+  __pyx_tuple__68 = PyTuple_Pack(5, __pyx_n_s_fs, __pyx_n_s_path, __pyx_n_s_typ, __pyx_n_s_data, __pyx_n_s_buf_view); if (unlikely(!__pyx_tuple__68)) __PYX_ERR(0, 356, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__68);
   __Pyx_GIVEREF(__pyx_tuple__68);
-  __pyx_codeobj__69 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_setattr, 353, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__69)) __PYX_ERR(0, 353, __pyx_L1_error)
+  __pyx_codeobj__69 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_setattr, 356, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__69)) __PYX_ERR(0, 356, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":358
+  /* "littlefs/lfs.pyx":361
  * 
  * 
  * def removeattr(LFSFilesystem fs, path, typ):             # <<<<<<<<<<<<<<
  *     _raise_on_error(lfs_removeattr(&fs._impl, path.encode(FILENAME_ENCODING), typ))
  * 
  */
-  __pyx_tuple__70 = PyTuple_Pack(3, __pyx_n_s_fs, __pyx_n_s_path, __pyx_n_s_typ); if (unlikely(!__pyx_tuple__70)) __PYX_ERR(0, 358, __pyx_L1_error)
+  __pyx_tuple__70 = PyTuple_Pack(3, __pyx_n_s_fs, __pyx_n_s_path, __pyx_n_s_typ); if (unlikely(!__pyx_tuple__70)) __PYX_ERR(0, 361, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__70);
   __Pyx_GIVEREF(__pyx_tuple__70);
-  __pyx_codeobj__71 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__70, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_removeattr, 358, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__71)) __PYX_ERR(0, 358, __pyx_L1_error)
+  __pyx_codeobj__71 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__70, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_removeattr, 361, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__71)) __PYX_ERR(0, 361, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":362
+  /* "littlefs/lfs.pyx":365
  * 
  * 
  * def file_open(LFSFilesystem fs, path, flags):             # <<<<<<<<<<<<<<
  *     if isinstance(flags, str):
  *         creating = False
  */
-  __pyx_tuple__72 = PyTuple_Pack(13, __pyx_n_s_fs, __pyx_n_s_path, __pyx_n_s_flags, __pyx_n_s_creating, __pyx_n_s_reading, __pyx_n_s_writing, __pyx_n_s_appending, __pyx_n_s_updating, __pyx_n_s_ch, __pyx_n_s_exclusive_modes, __pyx_n_s_fh, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__72)) __PYX_ERR(0, 362, __pyx_L1_error)
+  __pyx_tuple__72 = PyTuple_Pack(13, __pyx_n_s_fs, __pyx_n_s_path, __pyx_n_s_flags, __pyx_n_s_creating, __pyx_n_s_reading, __pyx_n_s_writing, __pyx_n_s_appending, __pyx_n_s_updating, __pyx_n_s_ch, __pyx_n_s_exclusive_modes, __pyx_n_s_fh, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__72)) __PYX_ERR(0, 365, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__72);
   __Pyx_GIVEREF(__pyx_tuple__72);
-  __pyx_codeobj__73 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__72, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_file_open, 362, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__73)) __PYX_ERR(0, 362, __pyx_L1_error)
+  __pyx_codeobj__73 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__72, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_file_open, 365, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__73)) __PYX_ERR(0, 365, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":413
+  /* "littlefs/lfs.pyx":416
  * 
  * 
  * def file_open_cfg(self, path, flags, config):             # <<<<<<<<<<<<<<
  *     raise NotImplementedError
  * 
  */
-  __pyx_tuple__74 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_path, __pyx_n_s_flags, __pyx_n_s_config); if (unlikely(!__pyx_tuple__74)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_tuple__74 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_path, __pyx_n_s_flags, __pyx_n_s_config); if (unlikely(!__pyx_tuple__74)) __PYX_ERR(0, 416, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__74);
   __Pyx_GIVEREF(__pyx_tuple__74);
-  __pyx_codeobj__75 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__74, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_file_open_cfg, 413, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__75)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_codeobj__75 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__74, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_file_open_cfg, 416, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__75)) __PYX_ERR(0, 416, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":417
+  /* "littlefs/lfs.pyx":420
  * 
  * 
  * def file_close(LFSFilesystem fs, LFSFile fh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_file_close(&fs._impl, &fh._impl))
  * 
  */
-  __pyx_tuple__76 = PyTuple_Pack(2, __pyx_n_s_fs, __pyx_n_s_fh); if (unlikely(!__pyx_tuple__76)) __PYX_ERR(0, 417, __pyx_L1_error)
+  __pyx_tuple__76 = PyTuple_Pack(2, __pyx_n_s_fs, __pyx_n_s_fh); if (unlikely(!__pyx_tuple__76)) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__76);
   __Pyx_GIVEREF(__pyx_tuple__76);
-  __pyx_codeobj__77 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__76, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_file_close, 417, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__77)) __PYX_ERR(0, 417, __pyx_L1_error)
+  __pyx_codeobj__77 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__76, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_file_close, 420, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__77)) __PYX_ERR(0, 420, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":421
+  /* "littlefs/lfs.pyx":424
  * 
  * 
  * def file_sync(LFSFilesystem fs, LFSFile fh):             # <<<<<<<<<<<<<<
  *     _raise_on_error(lfs_file_sync(&fs._impl, &fh._impl))
  * 
  */
-  __pyx_codeobj__78 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__76, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_file_sync, 421, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__78)) __PYX_ERR(0, 421, __pyx_L1_error)
+  __pyx_codeobj__78 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__76, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_file_sync, 424, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__78)) __PYX_ERR(0, 424, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":425
+  /* "littlefs/lfs.pyx":428
  * 
  * 
  * def file_read(LFSFilesystem fs, LFSFile fh, size):             # <<<<<<<<<<<<<<
  *     assert size >= 0, 'Size must be >= 0'
  *     buffer = b'\0xff' * size
  */
-  __pyx_tuple__79 = PyTuple_Pack(5, __pyx_n_s_fs, __pyx_n_s_fh, __pyx_n_s_size, __pyx_n_s_buffer, __pyx_n_s_rsize); if (unlikely(!__pyx_tuple__79)) __PYX_ERR(0, 425, __pyx_L1_error)
+  __pyx_tuple__79 = PyTuple_Pack(5, __pyx_n_s_fs, __pyx_n_s_fh, __pyx_n_s_size, __pyx_n_s_buffer, __pyx_n_s_rsize); if (unlikely(!__pyx_tuple__79)) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__79);
   __Pyx_GIVEREF(__pyx_tuple__79);
-  __pyx_codeobj__80 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__79, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_file_read, 425, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__80)) __PYX_ERR(0, 425, __pyx_L1_error)
+  __pyx_codeobj__80 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__79, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_file_read, 428, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__80)) __PYX_ERR(0, 428, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":432
+  /* "littlefs/lfs.pyx":435
  * 
  * 
  * def file_write(LFSFilesystem fs, LFSFile fh, data):             # <<<<<<<<<<<<<<
  *     assert isinstance(data, (bytes, bytearray))
  *     pdata = <char *>data
  */
-  __pyx_tuple__81 = PyTuple_Pack(5, __pyx_n_s_fs, __pyx_n_s_fh, __pyx_n_s_data, __pyx_n_s_pdata, __pyx_n_s_code); if (unlikely(!__pyx_tuple__81)) __PYX_ERR(0, 432, __pyx_L1_error)
+  __pyx_tuple__81 = PyTuple_Pack(5, __pyx_n_s_fs, __pyx_n_s_fh, __pyx_n_s_data, __pyx_n_s_pdata, __pyx_n_s_code); if (unlikely(!__pyx_tuple__81)) __PYX_ERR(0, 435, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__81);
   __Pyx_GIVEREF(__pyx_tuple__81);
-  __pyx_codeobj__82 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__81, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_file_write, 432, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__82)) __PYX_ERR(0, 432, __pyx_L1_error)
+  __pyx_codeobj__82 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__81, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_file_write, 435, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__82)) __PYX_ERR(0, 435, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":441
+  /* "littlefs/lfs.pyx":444
  * 
  * 
  * def file_seek(LFSFilesystem fs, LFSFile fh, off, whence):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_file_seek(&fs._impl, &fh._impl, off, whence))
  * 
  */
-  __pyx_tuple__83 = PyTuple_Pack(4, __pyx_n_s_fs, __pyx_n_s_fh, __pyx_n_s_off, __pyx_n_s_whence); if (unlikely(!__pyx_tuple__83)) __PYX_ERR(0, 441, __pyx_L1_error)
+  __pyx_tuple__83 = PyTuple_Pack(4, __pyx_n_s_fs, __pyx_n_s_fh, __pyx_n_s_off, __pyx_n_s_whence); if (unlikely(!__pyx_tuple__83)) __PYX_ERR(0, 444, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__83);
   __Pyx_GIVEREF(__pyx_tuple__83);
-  __pyx_codeobj__84 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_file_seek, 441, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__84)) __PYX_ERR(0, 441, __pyx_L1_error)
+  __pyx_codeobj__84 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_file_seek, 444, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__84)) __PYX_ERR(0, 444, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":445
+  /* "littlefs/lfs.pyx":448
  * 
  * 
  * def file_truncate(LFSFilesystem fs, LFSFile fh, size):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_file_truncate(&fs._impl, &fh._impl, size))
  * 
  */
-  __pyx_tuple__85 = PyTuple_Pack(3, __pyx_n_s_fs, __pyx_n_s_fh, __pyx_n_s_size); if (unlikely(!__pyx_tuple__85)) __PYX_ERR(0, 445, __pyx_L1_error)
+  __pyx_tuple__85 = PyTuple_Pack(3, __pyx_n_s_fs, __pyx_n_s_fh, __pyx_n_s_size); if (unlikely(!__pyx_tuple__85)) __PYX_ERR(0, 448, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__85);
   __Pyx_GIVEREF(__pyx_tuple__85);
-  __pyx_codeobj__86 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__85, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_file_truncate, 445, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__86)) __PYX_ERR(0, 445, __pyx_L1_error)
+  __pyx_codeobj__86 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__85, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_file_truncate, 448, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__86)) __PYX_ERR(0, 448, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":449
+  /* "littlefs/lfs.pyx":452
  * 
  * 
  * def file_tell(LFSFilesystem fs, LFSFile fh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_file_tell(&fs._impl, &fh._impl))
  * 
  */
-  __pyx_codeobj__87 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__76, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_file_tell, 449, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__87)) __PYX_ERR(0, 449, __pyx_L1_error)
+  __pyx_codeobj__87 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__76, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_file_tell, 452, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__87)) __PYX_ERR(0, 452, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":453
+  /* "littlefs/lfs.pyx":456
  * 
  * 
  * def file_rewind(LFSFilesystem fs, LFSFile fh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_file_rewind(&fs._impl, &fh._impl))
  * 
  */
-  __pyx_codeobj__88 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__76, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_file_rewind, 453, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__88)) __PYX_ERR(0, 453, __pyx_L1_error)
+  __pyx_codeobj__88 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__76, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_file_rewind, 456, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__88)) __PYX_ERR(0, 456, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":457
+  /* "littlefs/lfs.pyx":460
  * 
  * 
  * def file_size(LFSFilesystem fs, LFSFile fh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_file_size(&fs._impl, &fh._impl))
  * 
  */
-  __pyx_codeobj__89 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__76, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_file_size, 457, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__89)) __PYX_ERR(0, 457, __pyx_L1_error)
+  __pyx_codeobj__89 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__76, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_file_size, 460, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__89)) __PYX_ERR(0, 460, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":460
+  /* "littlefs/lfs.pyx":463
  *     return _raise_on_error(lfs_file_size(&fs._impl, &fh._impl))
  * 
  * def mkdir(LFSFilesystem fs, path):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_mkdir(&fs._impl, path.encode(FILENAME_ENCODING)))
  * 
  */
-  __pyx_codeobj__90 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__60, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_mkdir, 460, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__90)) __PYX_ERR(0, 460, __pyx_L1_error)
+  __pyx_codeobj__90 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__60, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_mkdir, 463, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__90)) __PYX_ERR(0, 463, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":463
+  /* "littlefs/lfs.pyx":466
  *     return _raise_on_error(lfs_mkdir(&fs._impl, path.encode(FILENAME_ENCODING)))
  * 
  * def dir_open(LFSFilesystem fs, path):             # <<<<<<<<<<<<<<
  *     handle = LFSDirectory()
  *     _raise_on_error(lfs_dir_open(&fs._impl, &handle._impl, path.encode(FILENAME_ENCODING)))
  */
-  __pyx_tuple__91 = PyTuple_Pack(3, __pyx_n_s_fs, __pyx_n_s_path, __pyx_n_s_handle); if (unlikely(!__pyx_tuple__91)) __PYX_ERR(0, 463, __pyx_L1_error)
+  __pyx_tuple__91 = PyTuple_Pack(3, __pyx_n_s_fs, __pyx_n_s_path, __pyx_n_s_handle); if (unlikely(!__pyx_tuple__91)) __PYX_ERR(0, 466, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__91);
   __Pyx_GIVEREF(__pyx_tuple__91);
-  __pyx_codeobj__92 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__91, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_dir_open, 463, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__92)) __PYX_ERR(0, 463, __pyx_L1_error)
+  __pyx_codeobj__92 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__91, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_dir_open, 466, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__92)) __PYX_ERR(0, 466, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":468
+  /* "littlefs/lfs.pyx":471
  *     return handle
  * 
  * def dir_close(LFSFilesystem fs, LFSDirectory dh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_dir_close(&fs._impl, &dh._impl))
  * 
  */
-  __pyx_tuple__93 = PyTuple_Pack(2, __pyx_n_s_fs, __pyx_n_s_dh); if (unlikely(!__pyx_tuple__93)) __PYX_ERR(0, 468, __pyx_L1_error)
+  __pyx_tuple__93 = PyTuple_Pack(2, __pyx_n_s_fs, __pyx_n_s_dh); if (unlikely(!__pyx_tuple__93)) __PYX_ERR(0, 471, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__93);
   __Pyx_GIVEREF(__pyx_tuple__93);
-  __pyx_codeobj__94 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__93, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_dir_close, 468, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__94)) __PYX_ERR(0, 468, __pyx_L1_error)
+  __pyx_codeobj__94 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__93, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_dir_close, 471, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__94)) __PYX_ERR(0, 471, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":471
+  /* "littlefs/lfs.pyx":474
  *     return _raise_on_error(lfs_dir_close(&fs._impl, &dh._impl))
  * 
  * def dir_read(LFSFilesystem fs, LFSDirectory dh):             # <<<<<<<<<<<<<<
  *     cdef lfs_info * info = <lfs_info *>malloc(sizeof(lfs_info))
  *     try:
  */
-  __pyx_tuple__95 = PyTuple_Pack(4, __pyx_n_s_fs, __pyx_n_s_dh, __pyx_n_s_info, __pyx_n_s_retval); if (unlikely(!__pyx_tuple__95)) __PYX_ERR(0, 471, __pyx_L1_error)
+  __pyx_tuple__95 = PyTuple_Pack(4, __pyx_n_s_fs, __pyx_n_s_dh, __pyx_n_s_info, __pyx_n_s_retval); if (unlikely(!__pyx_tuple__95)) __PYX_ERR(0, 474, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__95);
   __Pyx_GIVEREF(__pyx_tuple__95);
-  __pyx_codeobj__96 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__95, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_dir_read, 471, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__96)) __PYX_ERR(0, 471, __pyx_L1_error)
+  __pyx_codeobj__96 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__95, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_dir_read, 474, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__96)) __PYX_ERR(0, 474, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":481
+  /* "littlefs/lfs.pyx":484
  *         free(info)
  * 
  * def dir_tell(LFSFilesystem fs, LFSDirectory dh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_dir_tell(&fs._impl, &dh._impl))
  * 
  */
-  __pyx_codeobj__97 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__93, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_dir_tell, 481, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__97)) __PYX_ERR(0, 481, __pyx_L1_error)
+  __pyx_codeobj__97 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__93, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_dir_tell, 484, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__97)) __PYX_ERR(0, 484, __pyx_L1_error)
 
-  /* "littlefs/lfs.pyx":484
+  /* "littlefs/lfs.pyx":487
  *     return _raise_on_error(lfs_dir_tell(&fs._impl, &dh._impl))
  * 
  * def dir_rewind(LFSFilesystem fs, LFSDirectory dh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_dir_rewind(&fs._impl, &dh._impl))
- * 
  */
-  __pyx_codeobj__98 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__93, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_dir_rewind, 484, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__98)) __PYX_ERR(0, 484, __pyx_L1_error)
+  __pyx_codeobj__98 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__93, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_littlefs_lfs_pyx, __pyx_n_s_dir_rewind, 487, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__98)) __PYX_ERR(0, 487, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -32167,120 +32147,120 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_8littlefs_3lfs_LFSConfig = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8littlefs_3lfs_LFSConfig_spec, NULL); if (unlikely(!__pyx_ptype_8littlefs_3lfs_LFSConfig)) __PYX_ERR(0, 78, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8littlefs_3lfs_LFSConfig_spec, __pyx_ptype_8littlefs_3lfs_LFSConfig) < 0) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_ptype_8littlefs_3lfs_LFSConfig = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8littlefs_3lfs_LFSConfig_spec, NULL); if (unlikely(!__pyx_ptype_8littlefs_3lfs_LFSConfig)) __PYX_ERR(0, 81, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8littlefs_3lfs_LFSConfig_spec, __pyx_ptype_8littlefs_3lfs_LFSConfig) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
   #else
   __pyx_ptype_8littlefs_3lfs_LFSConfig = &__pyx_type_8littlefs_3lfs_LFSConfig;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_8littlefs_3lfs_LFSConfig) < 0) __PYX_ERR(0, 78, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_8littlefs_3lfs_LFSConfig) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_8littlefs_3lfs_LFSConfig->tp_print = 0;
   #endif
   #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
-    PyObject *wrapper = PyObject_GetAttrString((PyObject *)__pyx_ptype_8littlefs_3lfs_LFSConfig, "__init__"); if (unlikely(!wrapper)) __PYX_ERR(0, 78, __pyx_L1_error)
+    PyObject *wrapper = PyObject_GetAttrString((PyObject *)__pyx_ptype_8littlefs_3lfs_LFSConfig, "__init__"); if (unlikely(!wrapper)) __PYX_ERR(0, 81, __pyx_L1_error)
     if (__Pyx_IS_TYPE(wrapper, &PyWrapperDescr_Type)) {
       __pyx_wrapperbase_8littlefs_3lfs_9LFSConfig_2__init__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_8littlefs_3lfs_9LFSConfig_2__init__.doc = __pyx_doc_8littlefs_3lfs_9LFSConfig_2__init__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_8littlefs_3lfs_9LFSConfig_2__init__;
     }
   }
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_LFSConfig, (PyObject *) __pyx_ptype_8littlefs_3lfs_LFSConfig) < 0) __PYX_ERR(0, 78, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_LFSConfig, (PyObject *) __pyx_ptype_8littlefs_3lfs_LFSConfig) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_8littlefs_3lfs_LFSConfig) < 0) __PYX_ERR(0, 78, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_8littlefs_3lfs_LFSConfig) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_8littlefs_3lfs_LFSFilesystem = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8littlefs_3lfs_LFSFilesystem_spec, NULL); if (unlikely(!__pyx_ptype_8littlefs_3lfs_LFSFilesystem)) __PYX_ERR(0, 242, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8littlefs_3lfs_LFSFilesystem_spec, __pyx_ptype_8littlefs_3lfs_LFSFilesystem) < 0) __PYX_ERR(0, 242, __pyx_L1_error)
+  __pyx_ptype_8littlefs_3lfs_LFSFilesystem = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8littlefs_3lfs_LFSFilesystem_spec, NULL); if (unlikely(!__pyx_ptype_8littlefs_3lfs_LFSFilesystem)) __PYX_ERR(0, 245, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8littlefs_3lfs_LFSFilesystem_spec, __pyx_ptype_8littlefs_3lfs_LFSFilesystem) < 0) __PYX_ERR(0, 245, __pyx_L1_error)
   #else
   __pyx_ptype_8littlefs_3lfs_LFSFilesystem = &__pyx_type_8littlefs_3lfs_LFSFilesystem;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_8littlefs_3lfs_LFSFilesystem) < 0) __PYX_ERR(0, 242, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_8littlefs_3lfs_LFSFilesystem) < 0) __PYX_ERR(0, 245, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_8littlefs_3lfs_LFSFilesystem->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_8littlefs_3lfs_LFSFilesystem->tp_dictoffset && __pyx_ptype_8littlefs_3lfs_LFSFilesystem->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_8littlefs_3lfs_LFSFilesystem->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_LFSFilesystem, (PyObject *) __pyx_ptype_8littlefs_3lfs_LFSFilesystem) < 0) __PYX_ERR(0, 242, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_LFSFilesystem, (PyObject *) __pyx_ptype_8littlefs_3lfs_LFSFilesystem) < 0) __PYX_ERR(0, 245, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_8littlefs_3lfs_LFSFilesystem) < 0) __PYX_ERR(0, 242, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_8littlefs_3lfs_LFSFilesystem) < 0) __PYX_ERR(0, 245, __pyx_L1_error)
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_8littlefs_3lfs_LFSFile = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8littlefs_3lfs_LFSFile_spec, NULL); if (unlikely(!__pyx_ptype_8littlefs_3lfs_LFSFile)) __PYX_ERR(0, 250, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8littlefs_3lfs_LFSFile_spec, __pyx_ptype_8littlefs_3lfs_LFSFile) < 0) __PYX_ERR(0, 250, __pyx_L1_error)
+  __pyx_ptype_8littlefs_3lfs_LFSFile = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8littlefs_3lfs_LFSFile_spec, NULL); if (unlikely(!__pyx_ptype_8littlefs_3lfs_LFSFile)) __PYX_ERR(0, 253, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8littlefs_3lfs_LFSFile_spec, __pyx_ptype_8littlefs_3lfs_LFSFile) < 0) __PYX_ERR(0, 253, __pyx_L1_error)
   #else
   __pyx_ptype_8littlefs_3lfs_LFSFile = &__pyx_type_8littlefs_3lfs_LFSFile;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_8littlefs_3lfs_LFSFile) < 0) __PYX_ERR(0, 250, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_8littlefs_3lfs_LFSFile) < 0) __PYX_ERR(0, 253, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_8littlefs_3lfs_LFSFile->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_8littlefs_3lfs_LFSFile->tp_dictoffset && __pyx_ptype_8littlefs_3lfs_LFSFile->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_8littlefs_3lfs_LFSFile->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_LFSFile, (PyObject *) __pyx_ptype_8littlefs_3lfs_LFSFile) < 0) __PYX_ERR(0, 250, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_LFSFile, (PyObject *) __pyx_ptype_8littlefs_3lfs_LFSFile) < 0) __PYX_ERR(0, 253, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_8littlefs_3lfs_LFSFile) < 0) __PYX_ERR(0, 250, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_8littlefs_3lfs_LFSFile) < 0) __PYX_ERR(0, 253, __pyx_L1_error)
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_8littlefs_3lfs_LFSDirectory = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8littlefs_3lfs_LFSDirectory_spec, NULL); if (unlikely(!__pyx_ptype_8littlefs_3lfs_LFSDirectory)) __PYX_ERR(0, 259, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8littlefs_3lfs_LFSDirectory_spec, __pyx_ptype_8littlefs_3lfs_LFSDirectory) < 0) __PYX_ERR(0, 259, __pyx_L1_error)
+  __pyx_ptype_8littlefs_3lfs_LFSDirectory = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8littlefs_3lfs_LFSDirectory_spec, NULL); if (unlikely(!__pyx_ptype_8littlefs_3lfs_LFSDirectory)) __PYX_ERR(0, 262, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8littlefs_3lfs_LFSDirectory_spec, __pyx_ptype_8littlefs_3lfs_LFSDirectory) < 0) __PYX_ERR(0, 262, __pyx_L1_error)
   #else
   __pyx_ptype_8littlefs_3lfs_LFSDirectory = &__pyx_type_8littlefs_3lfs_LFSDirectory;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_8littlefs_3lfs_LFSDirectory) < 0) __PYX_ERR(0, 259, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_8littlefs_3lfs_LFSDirectory) < 0) __PYX_ERR(0, 262, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_8littlefs_3lfs_LFSDirectory->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_8littlefs_3lfs_LFSDirectory->tp_dictoffset && __pyx_ptype_8littlefs_3lfs_LFSDirectory->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_8littlefs_3lfs_LFSDirectory->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_LFSDirectory, (PyObject *) __pyx_ptype_8littlefs_3lfs_LFSDirectory) < 0) __PYX_ERR(0, 259, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_LFSDirectory, (PyObject *) __pyx_ptype_8littlefs_3lfs_LFSDirectory) < 0) __PYX_ERR(0, 262, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_8littlefs_3lfs_LFSDirectory) < 0) __PYX_ERR(0, 259, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_8littlefs_3lfs_LFSDirectory) < 0) __PYX_ERR(0, 262, __pyx_L1_error)
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_8littlefs_3lfs___pyx_scope_struct__genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8littlefs_3lfs___pyx_scope_struct__genexpr_spec, NULL); if (unlikely(!__pyx_ptype_8littlefs_3lfs___pyx_scope_struct__genexpr)) __PYX_ERR(0, 390, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8littlefs_3lfs___pyx_scope_struct__genexpr_spec, __pyx_ptype_8littlefs_3lfs___pyx_scope_struct__genexpr) < 0) __PYX_ERR(0, 390, __pyx_L1_error)
+  __pyx_ptype_8littlefs_3lfs___pyx_scope_struct__genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8littlefs_3lfs___pyx_scope_struct__genexpr_spec, NULL); if (unlikely(!__pyx_ptype_8littlefs_3lfs___pyx_scope_struct__genexpr)) __PYX_ERR(0, 393, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8littlefs_3lfs___pyx_scope_struct__genexpr_spec, __pyx_ptype_8littlefs_3lfs___pyx_scope_struct__genexpr) < 0) __PYX_ERR(0, 393, __pyx_L1_error)
   #else
   __pyx_ptype_8littlefs_3lfs___pyx_scope_struct__genexpr = &__pyx_type_8littlefs_3lfs___pyx_scope_struct__genexpr;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_8littlefs_3lfs___pyx_scope_struct__genexpr) < 0) __PYX_ERR(0, 390, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_8littlefs_3lfs___pyx_scope_struct__genexpr) < 0) __PYX_ERR(0, 393, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_8littlefs_3lfs___pyx_scope_struct__genexpr->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_8littlefs_3lfs___pyx_scope_struct__genexpr->tp_dictoffset && __pyx_ptype_8littlefs_3lfs___pyx_scope_struct__genexpr->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_8littlefs_3lfs___pyx_scope_struct__genexpr->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
@@ -32649,15 +32629,15 @@
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("lfs", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to lfs pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "lfs" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
@@ -33255,50 +33235,50 @@
   __Pyx_GOTREF(__pyx_t_7);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_Enum, __pyx_t_7) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "littlefs/lfs.pyx":1
  * import logging             # <<<<<<<<<<<<<<
  * import enum
- * from collections import namedtuple
+ * from typing import NamedTuple
  */
   __pyx_t_7 = __Pyx_ImportDottedModule(__pyx_n_s_logging, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_logging, __pyx_t_7) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "littlefs/lfs.pyx":2
  * import logging
  * import enum             # <<<<<<<<<<<<<<
- * from collections import namedtuple
+ * from typing import NamedTuple
  * # Import all definitions
  */
   __pyx_t_7 = __Pyx_ImportDottedModule(__pyx_n_s_enum, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_enum, __pyx_t_7) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "littlefs/lfs.pyx":3
  * import logging
  * import enum
- * from collections import namedtuple             # <<<<<<<<<<<<<<
+ * from typing import NamedTuple             # <<<<<<<<<<<<<<
  * # Import all definitions
  * # from littlefs._lfs cimport *
  */
   __pyx_t_7 = PyList_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_INCREF(__pyx_n_s_namedtuple);
-  __Pyx_GIVEREF(__pyx_n_s_namedtuple);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_7, 0, __pyx_n_s_namedtuple)) __PYX_ERR(0, 3, __pyx_L1_error);
-  __pyx_t_4 = __Pyx_Import(__pyx_n_s_collections, __pyx_t_7, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __Pyx_INCREF(__pyx_n_s_NamedTuple);
+  __Pyx_GIVEREF(__pyx_n_s_NamedTuple);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_7, 0, __pyx_n_s_NamedTuple)) __PYX_ERR(0, 3, __pyx_L1_error);
+  __pyx_t_4 = __Pyx_Import(__pyx_n_s_typing, __pyx_t_7, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_namedtuple); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_NamedTuple); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_namedtuple, __pyx_t_7) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_NamedTuple, __pyx_t_7) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "littlefs/lfs.pyx":7
  * # from littlefs._lfs cimport *
  * 
  * from littlefs.context import UserContext             # <<<<<<<<<<<<<<
@@ -33348,882 +33328,899 @@
  * 
  */
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_FILENAME_ENCODING, __pyx_n_u_ascii) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
 
   /* "littlefs/lfs.pyx":14
  * """Default filename encoding"""
  * 
- * LFSStat = namedtuple('LFSStat', ['type', 'size', 'name'])             # <<<<<<<<<<<<<<
- * LFSStat.__doc__ = """\
- * Littlefs File / Directory status
+ * class LFSStat(NamedTuple):             # <<<<<<<<<<<<<<
+ *     """Littlefs File / Directory status."""
+ *     type: int
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_namedtuple); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_NamedTuple); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_7 = PyList_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_INCREF(__pyx_n_u_type);
-  __Pyx_GIVEREF(__pyx_n_u_type);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_7, 0, __pyx_n_u_type)) __PYX_ERR(0, 14, __pyx_L1_error);
-  __Pyx_INCREF(__pyx_n_u_size);
-  __Pyx_GIVEREF(__pyx_n_u_size);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_7, 1, __pyx_n_u_size)) __PYX_ERR(0, 14, __pyx_L1_error);
-  __Pyx_INCREF(__pyx_n_u_name);
-  __Pyx_GIVEREF(__pyx_n_u_name);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_7, 2, __pyx_n_u_name)) __PYX_ERR(0, 14, __pyx_L1_error);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_4);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4)) __PYX_ERR(0, 14, __pyx_L1_error);
+  __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PEP560_update_bases(__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_INCREF(__pyx_n_u_LFSStat);
-  __Pyx_GIVEREF(__pyx_n_u_LFSStat);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_n_u_LFSStat)) __PYX_ERR(0, 14, __pyx_L1_error);
-  __Pyx_GIVEREF(__pyx_t_7);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_7)) __PYX_ERR(0, 14, __pyx_L1_error);
-  __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_Py3MetaclassPrepare(__pyx_t_5, __pyx_t_4, __pyx_n_s_LFSStat, __pyx_n_s_LFSStat, (PyObject *) NULL, __pyx_n_s_littlefs_lfs, __pyx_kp_s_Littlefs_File_Directory_status); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  if (__pyx_t_4 != __pyx_t_7) {
+    if (unlikely((PyDict_SetItemString(__pyx_t_9, "__orig_bases__", __pyx_t_7) < 0))) __PYX_ERR(0, 14, __pyx_L1_error)
+  }
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LFSStat, __pyx_t_7) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_type, __pyx_n_s_int) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_size, __pyx_n_s_int) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_name, __pyx_n_s_str) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_9, __pyx_n_s_annotations, __pyx_t_7) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "littlefs/lfs.pyx":15
+  /* "littlefs/lfs.pyx":21
+ * 
+ *     # Constants
+ *     TYPE_REG = LFS_TYPE_REG             # <<<<<<<<<<<<<<
+ *     TYPE_DIR = LFS_TYPE_DIR
  * 
- * LFSStat = namedtuple('LFSStat', ['type', 'size', 'name'])
- * LFSStat.__doc__ = """\             # <<<<<<<<<<<<<<
- * Littlefs File / Directory status
- * """
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_LFSStat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_enum__lfs_type(LFS_TYPE_REG); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_t_7, __pyx_n_s_doc, __pyx_kp_u_Littlefs_File_Directory_status) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_9, __pyx_n_s_TYPE_REG, __pyx_t_7) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "littlefs/lfs.pyx":19
- * """
+  /* "littlefs/lfs.pyx":22
+ *     # Constants
+ *     TYPE_REG = LFS_TYPE_REG
+ *     TYPE_DIR = LFS_TYPE_DIR             # <<<<<<<<<<<<<<
+ * 
  * 
- * LFSFSStat = namedtuple('LFSFSStat', [             # <<<<<<<<<<<<<<
- *     'disk_version',
- *     'name_max',
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_namedtuple); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_enum__lfs_type(LFS_TYPE_DIR); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_5 = PyList_New(6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 19, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_9, __pyx_n_s_TYPE_DIR, __pyx_t_7) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+
+  /* "littlefs/lfs.pyx":14
+ * """Default filename encoding"""
+ * 
+ * class LFSStat(NamedTuple):             # <<<<<<<<<<<<<<
+ *     """Littlefs File / Directory status."""
+ *     type: int
+ */
+  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_5, __pyx_n_s_LFSStat, __pyx_t_4, __pyx_t_9, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LFSStat, __pyx_t_7) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+  /* "littlefs/lfs.pyx":25
+ * 
+ * 
+ * class LFSFSStat(NamedTuple):             # <<<<<<<<<<<<<<
+ *     """Littlefs filesystem status."""
+ *     disk_version: int
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_NamedTuple); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_INCREF(__pyx_n_u_disk_version);
-  __Pyx_GIVEREF(__pyx_n_u_disk_version);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 0, __pyx_n_u_disk_version)) __PYX_ERR(0, 19, __pyx_L1_error);
-  __Pyx_INCREF(__pyx_n_u_name_max);
-  __Pyx_GIVEREF(__pyx_n_u_name_max);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 1, __pyx_n_u_name_max)) __PYX_ERR(0, 19, __pyx_L1_error);
-  __Pyx_INCREF(__pyx_n_u_file_max);
-  __Pyx_GIVEREF(__pyx_n_u_file_max);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 2, __pyx_n_u_file_max)) __PYX_ERR(0, 19, __pyx_L1_error);
-  __Pyx_INCREF(__pyx_n_u_attr_max);
-  __Pyx_GIVEREF(__pyx_n_u_attr_max);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 3, __pyx_n_u_attr_max)) __PYX_ERR(0, 19, __pyx_L1_error);
-  __Pyx_INCREF(__pyx_n_u_block_count);
-  __Pyx_GIVEREF(__pyx_n_u_block_count);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 4, __pyx_n_u_block_count)) __PYX_ERR(0, 19, __pyx_L1_error);
-  __Pyx_INCREF(__pyx_n_u_block_size);
-  __Pyx_GIVEREF(__pyx_n_u_block_size);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 5, __pyx_n_u_block_size)) __PYX_ERR(0, 19, __pyx_L1_error);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_4);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4)) __PYX_ERR(0, 25, __pyx_L1_error);
+  __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PEP560_update_bases(__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_INCREF(__pyx_n_u_LFSFSStat);
-  __Pyx_GIVEREF(__pyx_n_u_LFSFSStat);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_n_u_LFSFSStat)) __PYX_ERR(0, 19, __pyx_L1_error);
-  __Pyx_GIVEREF(__pyx_t_5);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_5)) __PYX_ERR(0, 19, __pyx_L1_error);
-  __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  __pyx_t_7 = __Pyx_Py3MetaclassPrepare(__pyx_t_9, __pyx_t_4, __pyx_n_s_LFSFSStat, __pyx_n_s_LFSFSStat, (PyObject *) NULL, __pyx_n_s_littlefs_lfs, __pyx_kp_s_Littlefs_filesystem_status); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  if (__pyx_t_4 != __pyx_t_5) {
+    if (unlikely((PyDict_SetItemString(__pyx_t_7, "__orig_bases__", __pyx_t_5) < 0))) __PYX_ERR(0, 25, __pyx_L1_error)
+  }
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LFSFSStat, __pyx_t_5) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_disk_version, __pyx_n_s_int) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_name_max, __pyx_n_s_int) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_file_max, __pyx_n_s_int) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_attr_max, __pyx_n_s_int) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_block_count, __pyx_n_s_int) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_block_size, __pyx_n_s_int) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_7, __pyx_n_s_annotations, __pyx_t_5) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "littlefs/lfs.pyx":27
- *     'block_size',
- * ])
- * LFSFSStat.__doc__ = """\             # <<<<<<<<<<<<<<
- * Littlefs filesystem status
- * """
+  /* "littlefs/lfs.pyx":32
+ *     attr_max: int
+ *     block_count: int
+ *     block_size: int             # <<<<<<<<<<<<<<
+ * 
+ * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_LFSFSStat); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3ClassCreate(__pyx_t_9, __pyx_n_s_LFSFSStat, __pyx_t_4, __pyx_t_7, NULL, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_t_5, __pyx_n_s_doc, __pyx_kp_u_Littlefs_filesystem_status) < 0) __PYX_ERR(0, 27, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LFSFSStat, __pyx_t_5) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "littlefs/lfs.pyx":32
+  /* "littlefs/lfs.pyx":35
  * 
  * 
  * class LFSFileFlag(enum.IntFlag):             # <<<<<<<<<<<<<<
  *     """Littlefs file mode flags"""
  *     rdonly = LFS_O_RDONLY
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_enum); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 32, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_IntFlag); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_enum); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 32, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4)) __PYX_ERR(0, 32, __pyx_L1_error);
-  __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PEP560_update_bases(__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_IntFlag); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_7 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 32, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_9 = __Pyx_Py3MetaclassPrepare(__pyx_t_7, __pyx_t_4, __pyx_n_s_LFSFileFlag, __pyx_n_s_LFSFileFlag, (PyObject *) NULL, __pyx_n_s_littlefs_lfs, __pyx_kp_s_Littlefs_file_mode_flags); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_9);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_9)) __PYX_ERR(0, 35, __pyx_L1_error);
+  __pyx_t_9 = 0;
+  __pyx_t_9 = __Pyx_PEP560_update_bases(__pyx_t_4); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  if (__pyx_t_4 != __pyx_t_5) {
-    if (unlikely((PyDict_SetItemString(__pyx_t_9, "__orig_bases__", __pyx_t_5) < 0))) __PYX_ERR(0, 32, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CalculateMetaclass(NULL, __pyx_t_9); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_7, __pyx_t_9, __pyx_n_s_LFSFileFlag, __pyx_n_s_LFSFileFlag, (PyObject *) NULL, __pyx_n_s_littlefs_lfs, __pyx_kp_s_Littlefs_file_mode_flags); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (__pyx_t_9 != __pyx_t_4) {
+    if (unlikely((PyDict_SetItemString(__pyx_t_5, "__orig_bases__", __pyx_t_4) < 0))) __PYX_ERR(0, 35, __pyx_L1_error)
   }
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "littlefs/lfs.pyx":34
+  /* "littlefs/lfs.pyx":37
  * class LFSFileFlag(enum.IntFlag):
  *     """Littlefs file mode flags"""
  *     rdonly = LFS_O_RDONLY             # <<<<<<<<<<<<<<
  *     wronly = LFS_O_WRONLY
  *     rdwr = LFS_O_RDWR
  */
-  __pyx_t_5 = __Pyx_PyInt_From_enum__lfs_open_flags(LFS_O_RDONLY); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 34, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetNameInClass(__pyx_t_9, __pyx_n_s_rdonly, __pyx_t_5) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_4 = __Pyx_PyInt_From_enum__lfs_open_flags(LFS_O_RDONLY); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_rdonly, __pyx_t_4) < 0) __PYX_ERR(0, 37, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "littlefs/lfs.pyx":35
+  /* "littlefs/lfs.pyx":38
  *     """Littlefs file mode flags"""
  *     rdonly = LFS_O_RDONLY
  *     wronly = LFS_O_WRONLY             # <<<<<<<<<<<<<<
  *     rdwr = LFS_O_RDWR
  *     creat = LFS_O_CREAT
  */
-  __pyx_t_5 = __Pyx_PyInt_From_enum__lfs_open_flags(LFS_O_WRONLY); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 35, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetNameInClass(__pyx_t_9, __pyx_n_s_wronly, __pyx_t_5) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_4 = __Pyx_PyInt_From_enum__lfs_open_flags(LFS_O_WRONLY); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_wronly, __pyx_t_4) < 0) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "littlefs/lfs.pyx":36
+  /* "littlefs/lfs.pyx":39
  *     rdonly = LFS_O_RDONLY
  *     wronly = LFS_O_WRONLY
  *     rdwr = LFS_O_RDWR             # <<<<<<<<<<<<<<
  *     creat = LFS_O_CREAT
  *     excl = LFS_O_EXCL
  */
-  __pyx_t_5 = __Pyx_PyInt_From_enum__lfs_open_flags(LFS_O_RDWR); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetNameInClass(__pyx_t_9, __pyx_n_s_rdwr, __pyx_t_5) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_4 = __Pyx_PyInt_From_enum__lfs_open_flags(LFS_O_RDWR); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_rdwr, __pyx_t_4) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "littlefs/lfs.pyx":37
+  /* "littlefs/lfs.pyx":40
  *     wronly = LFS_O_WRONLY
  *     rdwr = LFS_O_RDWR
  *     creat = LFS_O_CREAT             # <<<<<<<<<<<<<<
  *     excl = LFS_O_EXCL
  *     trunc = LFS_O_TRUNC
  */
-  __pyx_t_5 = __Pyx_PyInt_From_enum__lfs_open_flags(LFS_O_CREAT); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 37, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetNameInClass(__pyx_t_9, __pyx_n_s_creat, __pyx_t_5) < 0) __PYX_ERR(0, 37, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_4 = __Pyx_PyInt_From_enum__lfs_open_flags(LFS_O_CREAT); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_creat, __pyx_t_4) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "littlefs/lfs.pyx":38
+  /* "littlefs/lfs.pyx":41
  *     rdwr = LFS_O_RDWR
  *     creat = LFS_O_CREAT
  *     excl = LFS_O_EXCL             # <<<<<<<<<<<<<<
  *     trunc = LFS_O_TRUNC
  *     append = LFS_O_APPEND
  */
-  __pyx_t_5 = __Pyx_PyInt_From_enum__lfs_open_flags(LFS_O_EXCL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 38, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetNameInClass(__pyx_t_9, __pyx_n_s_excl, __pyx_t_5) < 0) __PYX_ERR(0, 38, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_4 = __Pyx_PyInt_From_enum__lfs_open_flags(LFS_O_EXCL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_excl, __pyx_t_4) < 0) __PYX_ERR(0, 41, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "littlefs/lfs.pyx":39
+  /* "littlefs/lfs.pyx":42
  *     creat = LFS_O_CREAT
  *     excl = LFS_O_EXCL
  *     trunc = LFS_O_TRUNC             # <<<<<<<<<<<<<<
  *     append = LFS_O_APPEND
  * 
  */
-  __pyx_t_5 = __Pyx_PyInt_From_enum__lfs_open_flags(LFS_O_TRUNC); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 39, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetNameInClass(__pyx_t_9, __pyx_n_s_trunc, __pyx_t_5) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_4 = __Pyx_PyInt_From_enum__lfs_open_flags(LFS_O_TRUNC); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_trunc, __pyx_t_4) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "littlefs/lfs.pyx":40
+  /* "littlefs/lfs.pyx":43
  *     excl = LFS_O_EXCL
  *     trunc = LFS_O_TRUNC
  *     append = LFS_O_APPEND             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_5 = __Pyx_PyInt_From_enum__lfs_open_flags(LFS_O_APPEND); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 40, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetNameInClass(__pyx_t_9, __pyx_n_s_append, __pyx_t_5) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_4 = __Pyx_PyInt_From_enum__lfs_open_flags(LFS_O_APPEND); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_append, __pyx_t_4) < 0) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "littlefs/lfs.pyx":32
+  /* "littlefs/lfs.pyx":35
  * 
  * 
  * class LFSFileFlag(enum.IntFlag):             # <<<<<<<<<<<<<<
  *     """Littlefs file mode flags"""
  *     rdonly = LFS_O_RDONLY
  */
-  __pyx_t_5 = __Pyx_Py3ClassCreate(__pyx_t_7, __pyx_n_s_LFSFileFlag, __pyx_t_4, __pyx_t_9, NULL, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 32, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LFSFileFlag, __pyx_t_5) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_7, __pyx_n_s_LFSFileFlag, __pyx_t_9, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LFSFileFlag, __pyx_t_4) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-  /* "littlefs/lfs.pyx":44
+  /* "littlefs/lfs.pyx":47
  * 
  * # Export LFS version and disk version to python
  * __LFS_VERSION__ = (LFS_VERSION_MAJOR, LFS_VERSION_MINOR)             # <<<<<<<<<<<<<<
  * __LFS_DISK_VERSION__ = (LFS_DISK_VERSION_MAJOR, LFS_DISK_VERSION_MINOR)
  * 
  */
-  __pyx_t_4 = __Pyx_PyInt_From_int(LFS_VERSION_MAJOR); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 44, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_7 = __Pyx_PyInt_From_int(LFS_VERSION_MINOR); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 44, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyInt_From_int(LFS_VERSION_MAJOR); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_4)) __PYX_ERR(0, 44, __pyx_L1_error);
+  __pyx_t_7 = __Pyx_PyInt_From_int(LFS_VERSION_MINOR); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_9);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_9)) __PYX_ERR(0, 47, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_7);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_t_7)) __PYX_ERR(0, 44, __pyx_L1_error);
-  __pyx_t_4 = 0;
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_7)) __PYX_ERR(0, 47, __pyx_L1_error);
+  __pyx_t_9 = 0;
   __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LFS_VERSION, __pyx_t_9) < 0) __PYX_ERR(0, 44, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LFS_VERSION, __pyx_t_5) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "littlefs/lfs.pyx":45
+  /* "littlefs/lfs.pyx":48
  * # Export LFS version and disk version to python
  * __LFS_VERSION__ = (LFS_VERSION_MAJOR, LFS_VERSION_MINOR)
  * __LFS_DISK_VERSION__ = (LFS_DISK_VERSION_MAJOR, LFS_DISK_VERSION_MINOR)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_9 = __Pyx_PyInt_From_int(LFS_DISK_VERSION_MAJOR); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 45, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_7 = __Pyx_PyInt_From_int(LFS_DISK_VERSION_MINOR); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(LFS_DISK_VERSION_MAJOR); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_7 = __Pyx_PyInt_From_int(LFS_DISK_VERSION_MINOR); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 45, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GIVEREF(__pyx_t_9);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_9)) __PYX_ERR(0, 45, __pyx_L1_error);
+  __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  __Pyx_GIVEREF(__pyx_t_5);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_5)) __PYX_ERR(0, 48, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_7);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_7)) __PYX_ERR(0, 45, __pyx_L1_error);
-  __pyx_t_9 = 0;
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_t_7)) __PYX_ERR(0, 48, __pyx_L1_error);
+  __pyx_t_5 = 0;
   __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LFS_DISK_VERSION, __pyx_t_4) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LFS_DISK_VERSION, __pyx_t_9) < 0) __PYX_ERR(0, 48, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-  /* "littlefs/lfs.pyx":93
+  /* "littlefs/lfs.pyx":96
  *                  context=None,
  *                  *,
  *                  block_size: int = 128,             # <<<<<<<<<<<<<<
  *                  block_count: int = 64,
  *                  read_size: int = 0,
  */
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_128)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_128))) __PYX_ERR(0, 93, __pyx_L1_error)
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_128)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_128))) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_128);
   __pyx_k__9 = ((PyObject*)__pyx_int_128);
   __Pyx_GIVEREF(__pyx_int_128);
 
-  /* "littlefs/lfs.pyx":94
+  /* "littlefs/lfs.pyx":97
  *                  *,
  *                  block_size: int = 128,
  *                  block_count: int = 64,             # <<<<<<<<<<<<<<
  *                  read_size: int = 0,
  *                  prog_size: int = 0,
  */
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_64)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_64))) __PYX_ERR(0, 94, __pyx_L1_error)
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_64)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_64))) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_64);
   __pyx_k__10 = ((PyObject*)__pyx_int_64);
   __Pyx_GIVEREF(__pyx_int_64);
 
-  /* "littlefs/lfs.pyx":95
+  /* "littlefs/lfs.pyx":98
  *                  block_size: int = 128,
  *                  block_count: int = 64,
  *                  read_size: int = 0,             # <<<<<<<<<<<<<<
  *                  prog_size: int = 0,
  *                  block_cycles: int = -1,
  */
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_0)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_0))) __PYX_ERR(0, 95, __pyx_L1_error)
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_0)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_0))) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_0);
   __pyx_k__11 = ((PyObject*)__pyx_int_0);
   __Pyx_GIVEREF(__pyx_int_0);
 
-  /* "littlefs/lfs.pyx":96
+  /* "littlefs/lfs.pyx":99
  *                  block_count: int = 64,
  *                  read_size: int = 0,
  *                  prog_size: int = 0,             # <<<<<<<<<<<<<<
  *                  block_cycles: int = -1,
  *                  cache_size: int = 0,
  */
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_0)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_0))) __PYX_ERR(0, 96, __pyx_L1_error)
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_0)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_0))) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_0);
   __pyx_k__12 = ((PyObject*)__pyx_int_0);
   __Pyx_GIVEREF(__pyx_int_0);
 
-  /* "littlefs/lfs.pyx":97
+  /* "littlefs/lfs.pyx":100
  *                  read_size: int = 0,
  *                  prog_size: int = 0,
  *                  block_cycles: int = -1,             # <<<<<<<<<<<<<<
  *                  cache_size: int = 0,
  *                  lookahead_size: int = 8,
  */
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_neg_1)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_neg_1))) __PYX_ERR(0, 97, __pyx_L1_error)
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_neg_1)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_neg_1))) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_neg_1);
   __pyx_k__13 = ((PyObject*)__pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_int_neg_1);
 
-  /* "littlefs/lfs.pyx":98
+  /* "littlefs/lfs.pyx":101
  *                  prog_size: int = 0,
  *                  block_cycles: int = -1,
  *                  cache_size: int = 0,             # <<<<<<<<<<<<<<
  *                  lookahead_size: int = 8,
  *                  name_max: int = 255,
  */
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_0)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_0))) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_0)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_0))) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_0);
   __pyx_k__14 = ((PyObject*)__pyx_int_0);
   __Pyx_GIVEREF(__pyx_int_0);
 
-  /* "littlefs/lfs.pyx":99
+  /* "littlefs/lfs.pyx":102
  *                  block_cycles: int = -1,
  *                  cache_size: int = 0,
  *                  lookahead_size: int = 8,             # <<<<<<<<<<<<<<
  *                  name_max: int = 255,
  *                  file_max: int = 0,
  */
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_8)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_8))) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_8)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_8))) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_8);
   __pyx_k__15 = ((PyObject*)__pyx_int_8);
   __Pyx_GIVEREF(__pyx_int_8);
 
-  /* "littlefs/lfs.pyx":100
+  /* "littlefs/lfs.pyx":103
  *                  cache_size: int = 0,
  *                  lookahead_size: int = 8,
  *                  name_max: int = 255,             # <<<<<<<<<<<<<<
  *                  file_max: int = 0,
  *                  attr_max: int = 0,
  */
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_255)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_255))) __PYX_ERR(0, 100, __pyx_L1_error)
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_255)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_255))) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_255);
   __pyx_k__16 = ((PyObject*)__pyx_int_255);
   __Pyx_GIVEREF(__pyx_int_255);
 
-  /* "littlefs/lfs.pyx":101
+  /* "littlefs/lfs.pyx":104
  *                  lookahead_size: int = 8,
  *                  name_max: int = 255,
  *                  file_max: int = 0,             # <<<<<<<<<<<<<<
  *                  attr_max: int = 0,
  *                  metadata_max: int = 0,
  */
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_0)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_0))) __PYX_ERR(0, 101, __pyx_L1_error)
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_0)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_0))) __PYX_ERR(0, 104, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_0);
   __pyx_k__17 = ((PyObject*)__pyx_int_0);
   __Pyx_GIVEREF(__pyx_int_0);
 
-  /* "littlefs/lfs.pyx":102
+  /* "littlefs/lfs.pyx":105
  *                  name_max: int = 255,
  *                  file_max: int = 0,
  *                  attr_max: int = 0,             # <<<<<<<<<<<<<<
  *                  metadata_max: int = 0,
  *                  disk_version: int = 0,
  */
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_0)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_0))) __PYX_ERR(0, 102, __pyx_L1_error)
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_0)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_0))) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_0);
   __pyx_k__18 = ((PyObject*)__pyx_int_0);
   __Pyx_GIVEREF(__pyx_int_0);
 
-  /* "littlefs/lfs.pyx":103
+  /* "littlefs/lfs.pyx":106
  *                  file_max: int = 0,
  *                  attr_max: int = 0,
  *                  metadata_max: int = 0,             # <<<<<<<<<<<<<<
  *                  disk_version: int = 0,
  *                 ):
  */
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_0)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_0))) __PYX_ERR(0, 103, __pyx_L1_error)
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_0)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_0))) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_0);
   __pyx_k__19 = ((PyObject*)__pyx_int_0);
   __Pyx_GIVEREF(__pyx_int_0);
 
-  /* "littlefs/lfs.pyx":104
+  /* "littlefs/lfs.pyx":107
  *                  attr_max: int = 0,
  *                  metadata_max: int = 0,
  *                  disk_version: int = 0,             # <<<<<<<<<<<<<<
  *                 ):
  *         """LittleFS Configuration.
  */
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_0)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_0))) __PYX_ERR(0, 104, __pyx_L1_error)
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_0)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_0))) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_0);
   __pyx_k__20 = ((PyObject*)__pyx_int_0);
   __Pyx_GIVEREF(__pyx_int_0);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_9LFSConfig_7__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LFSConfig___reduce_cython, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__40)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_4) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_9LFSConfig_7__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LFSConfig___reduce_cython, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__40)); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_9) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_9LFSConfig_9__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LFSConfig___setstate_cython, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__42)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_4) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_9LFSConfig_9__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LFSConfig___setstate_cython, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__42)); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_9) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "Pickling of struct members such as self._impl must be explicitly requested with @auto_pickle(True)"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_13LFSFilesystem_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LFSFilesystem___reduce_cython, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__43)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_4) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_13LFSFilesystem_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LFSFilesystem___reduce_cython, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__43)); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_9) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "Pickling of struct members such as self._impl must be explicitly requested with @auto_pickle(True)"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "Pickling of struct members such as self._impl must be explicitly requested with @auto_pickle(True)"
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_13LFSFilesystem_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LFSFilesystem___setstate_cython, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_4) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_13LFSFilesystem_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LFSFilesystem___setstate_cython, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_9) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "Pickling of struct members such as self._impl must be explicitly requested with @auto_pickle(True)"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_7LFSFile_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LFSFile___reduce_cython, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__45)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_4) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_7LFSFile_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LFSFile___reduce_cython, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__45)); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_9) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "Pickling of struct members such as self._impl must be explicitly requested with @auto_pickle(True)"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "Pickling of struct members such as self._impl must be explicitly requested with @auto_pickle(True)"
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_7LFSFile_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LFSFile___setstate_cython, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__46)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_4) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_7LFSFile_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LFSFile___setstate_cython, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__46)); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_9) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "Pickling of struct members such as self._impl must be explicitly requested with @auto_pickle(True)"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_12LFSDirectory_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LFSDirectory___reduce_cython, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__47)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_4) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_12LFSDirectory_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LFSDirectory___reduce_cython, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__47)); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_9) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "Pickling of struct members such as self._impl must be explicitly requested with @auto_pickle(True)"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "Pickling of struct members such as self._impl must be explicitly requested with @auto_pickle(True)"
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_12LFSDirectory_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LFSDirectory___setstate_cython, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__48)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_4) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_12LFSDirectory_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LFSDirectory___setstate_cython, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__48)); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_9) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-  /* "littlefs/lfs.pyx":263
+  /* "littlefs/lfs.pyx":266
  * 
  * 
  * def fs_stat(LFSFilesystem fs):             # <<<<<<<<<<<<<<
  *     """Get filesystem status"""
  *     cdef lfs_fsinfo * info = <lfs_fsinfo *>malloc(sizeof(lfs_fsinfo))
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_1fs_stat, 0, __pyx_n_s_fs_stat, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__50)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 263, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_fs_stat, __pyx_t_4) < 0) __PYX_ERR(0, 263, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_1fs_stat, 0, __pyx_n_s_fs_stat, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__50)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_fs_stat, __pyx_t_9) < 0) __PYX_ERR(0, 266, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-  /* "littlefs/lfs.pyx":280
+  /* "littlefs/lfs.pyx":283
  * 
  * 
  * def fs_size(LFSFilesystem fs):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_fs_size(&fs._impl))
  * 
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_3fs_size, 0, __pyx_n_s_fs_size, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__52)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 280, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_fs_size, __pyx_t_4) < 0) __PYX_ERR(0, 280, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_3fs_size, 0, __pyx_n_s_fs_size, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__52)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_fs_size, __pyx_t_9) < 0) __PYX_ERR(0, 283, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-  /* "littlefs/lfs.pyx":284
+  /* "littlefs/lfs.pyx":287
  * 
  * 
  * def format(LFSFilesystem fs, LFSConfig cfg):             # <<<<<<<<<<<<<<
  *     """Format the filesystem"""
  *     return _raise_on_error(lfs_format(&fs._impl, &cfg._impl))
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_5format, 0, __pyx_n_s_format, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__54)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 284, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_format, __pyx_t_4) < 0) __PYX_ERR(0, 284, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_5format, 0, __pyx_n_s_format, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__54)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_format, __pyx_t_9) < 0) __PYX_ERR(0, 287, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-  /* "littlefs/lfs.pyx":289
+  /* "littlefs/lfs.pyx":292
  * 
  * 
  * def mount(LFSFilesystem fs, LFSConfig cfg):             # <<<<<<<<<<<<<<
  *     """Mount the filesystem"""
  *     return _raise_on_error(lfs_mount(&fs._impl, &cfg._impl))
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_7mount, 0, __pyx_n_s_mount, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__55)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 289, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_mount, __pyx_t_4) < 0) __PYX_ERR(0, 289, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_7mount, 0, __pyx_n_s_mount, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__55)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_mount, __pyx_t_9) < 0) __PYX_ERR(0, 292, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-  /* "littlefs/lfs.pyx":294
+  /* "littlefs/lfs.pyx":297
  * 
  * 
  * def unmount(LFSFilesystem fs):             # <<<<<<<<<<<<<<
  *     """Unmount the filesystem
  * 
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_9unmount, 0, __pyx_n_s_unmount, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__56)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 294, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_unmount, __pyx_t_4) < 0) __PYX_ERR(0, 294, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_9unmount, 0, __pyx_n_s_unmount, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__56)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 297, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_unmount, __pyx_t_9) < 0) __PYX_ERR(0, 297, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-  /* "littlefs/lfs.pyx":302
+  /* "littlefs/lfs.pyx":305
  * 
  * 
  * def fs_mkconsistent(LFSFilesystem fs):             # <<<<<<<<<<<<<<
  *     """Attempt to make the filesystem consistent and ready for writing"""
  *     return _raise_on_error(lfs_fs_mkconsistent(&fs._impl))
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_11fs_mkconsistent, 0, __pyx_n_s_fs_mkconsistent, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__57)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 302, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_fs_mkconsistent, __pyx_t_4) < 0) __PYX_ERR(0, 302, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_9 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_11fs_mkconsistent, 0, __pyx_n_s_fs_mkconsistent, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__57)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 305, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_fs_mkconsistent, __pyx_t_9) < 0) __PYX_ERR(0, 305, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-  /* "littlefs/lfs.pyx":307
+  /* "littlefs/lfs.pyx":310
  * 
  * 
  * def fs_grow(LFSFilesystem fs, block_count) -> int:             # <<<<<<<<<<<<<<
  *     """Irreversibly grows the filesystem to a new size.
  * 
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 307, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(0, 307, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_13fs_grow, 0, __pyx_n_s_fs_grow, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__59)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 307, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 310, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(0, 310, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_13fs_grow, 0, __pyx_n_s_fs_grow, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__59)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 310, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_4);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_fs_grow, __pyx_t_7) < 0) __PYX_ERR(0, 307, __pyx_L1_error)
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_9);
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_fs_grow, __pyx_t_7) < 0) __PYX_ERR(0, 310, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "littlefs/lfs.pyx":319
+  /* "littlefs/lfs.pyx":322
  * 
  * 
  * def remove(LFSFilesystem fs, path):             # <<<<<<<<<<<<<<
  *     """Remove a file or directory
  * 
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_15remove, 0, __pyx_n_s_remove, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__61)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 319, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_15remove, 0, __pyx_n_s_remove, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__61)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_remove, __pyx_t_7) < 0) __PYX_ERR(0, 319, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_remove, __pyx_t_7) < 0) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "littlefs/lfs.pyx":326
+  /* "littlefs/lfs.pyx":329
  *     return _raise_on_error(lfs_remove(&fs._impl, path.encode(FILENAME_ENCODING)))
  * 
  * def rename(LFSFilesystem fs, oldpath, newpath):             # <<<<<<<<<<<<<<
  *     """Rename or move a file or directory
  * 
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_17rename, 0, __pyx_n_s_rename, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__63)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 326, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_17rename, 0, __pyx_n_s_rename, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__63)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 329, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_rename, __pyx_t_7) < 0) __PYX_ERR(0, 326, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_rename, __pyx_t_7) < 0) __PYX_ERR(0, 329, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "littlefs/lfs.pyx":336
+  /* "littlefs/lfs.pyx":339
  * 
  * 
  * def stat(LFSFilesystem fs, path):             # <<<<<<<<<<<<<<
  *     """Find info about a file or directory"""
  *     cdef lfs_info * info = <lfs_info *>malloc(sizeof(lfs_info))
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_19stat, 0, __pyx_n_s_stat, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__65)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 336, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_19stat, 0, __pyx_n_s_stat, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__65)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 339, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_stat, __pyx_t_7) < 0) __PYX_ERR(0, 336, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_stat, __pyx_t_7) < 0) __PYX_ERR(0, 339, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "littlefs/lfs.pyx":346
+  /* "littlefs/lfs.pyx":349
  * 
  * 
  * def getattr(LFSFilesystem fs, path, typ):             # <<<<<<<<<<<<<<
  *     buf = bytearray(LFS_ATTR_MAX)
  *     cdef unsigned char[::1] buf_view = buf
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_21getattr, 0, __pyx_n_s_getattr, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__67)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 346, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_21getattr, 0, __pyx_n_s_getattr, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__67)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 349, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_getattr, __pyx_t_7) < 0) __PYX_ERR(0, 346, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_getattr, __pyx_t_7) < 0) __PYX_ERR(0, 349, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "littlefs/lfs.pyx":353
+  /* "littlefs/lfs.pyx":356
  * 
  * 
  * def setattr(LFSFilesystem fs, path, typ, data):             # <<<<<<<<<<<<<<
  *     cdef const unsigned char[::1] buf_view = data
  *     _raise_on_error(lfs_setattr(&fs._impl, path.encode(FILENAME_ENCODING), typ, &buf_view[0], len(data)))
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_23setattr, 0, __pyx_n_s_setattr, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__69)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 353, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_23setattr, 0, __pyx_n_s_setattr, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__69)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 356, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_setattr, __pyx_t_7) < 0) __PYX_ERR(0, 353, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_setattr, __pyx_t_7) < 0) __PYX_ERR(0, 356, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "littlefs/lfs.pyx":358
+  /* "littlefs/lfs.pyx":361
  * 
  * 
  * def removeattr(LFSFilesystem fs, path, typ):             # <<<<<<<<<<<<<<
  *     _raise_on_error(lfs_removeattr(&fs._impl, path.encode(FILENAME_ENCODING), typ))
  * 
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_25removeattr, 0, __pyx_n_s_removeattr, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__71)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 358, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_25removeattr, 0, __pyx_n_s_removeattr, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__71)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 361, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_removeattr, __pyx_t_7) < 0) __PYX_ERR(0, 358, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_removeattr, __pyx_t_7) < 0) __PYX_ERR(0, 361, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "littlefs/lfs.pyx":362
+  /* "littlefs/lfs.pyx":365
  * 
  * 
  * def file_open(LFSFilesystem fs, path, flags):             # <<<<<<<<<<<<<<
  *     if isinstance(flags, str):
  *         creating = False
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_27file_open, 0, __pyx_n_s_file_open, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__73)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 362, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_27file_open, 0, __pyx_n_s_file_open, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__73)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 365, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_file_open, __pyx_t_7) < 0) __PYX_ERR(0, 362, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_file_open, __pyx_t_7) < 0) __PYX_ERR(0, 365, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "littlefs/lfs.pyx":413
+  /* "littlefs/lfs.pyx":416
  * 
  * 
  * def file_open_cfg(self, path, flags, config):             # <<<<<<<<<<<<<<
  *     raise NotImplementedError
  * 
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_29file_open_cfg, 0, __pyx_n_s_file_open_cfg, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__75)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_29file_open_cfg, 0, __pyx_n_s_file_open_cfg, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__75)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 416, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_file_open_cfg, __pyx_t_7) < 0) __PYX_ERR(0, 413, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_file_open_cfg, __pyx_t_7) < 0) __PYX_ERR(0, 416, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "littlefs/lfs.pyx":417
+  /* "littlefs/lfs.pyx":420
  * 
  * 
  * def file_close(LFSFilesystem fs, LFSFile fh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_file_close(&fs._impl, &fh._impl))
  * 
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_31file_close, 0, __pyx_n_s_file_close, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__77)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 417, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_31file_close, 0, __pyx_n_s_file_close, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__77)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_file_close, __pyx_t_7) < 0) __PYX_ERR(0, 417, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_file_close, __pyx_t_7) < 0) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "littlefs/lfs.pyx":421
+  /* "littlefs/lfs.pyx":424
  * 
  * 
  * def file_sync(LFSFilesystem fs, LFSFile fh):             # <<<<<<<<<<<<<<
  *     _raise_on_error(lfs_file_sync(&fs._impl, &fh._impl))
  * 
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_33file_sync, 0, __pyx_n_s_file_sync, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__78)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 421, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_33file_sync, 0, __pyx_n_s_file_sync, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__78)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_file_sync, __pyx_t_7) < 0) __PYX_ERR(0, 421, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_file_sync, __pyx_t_7) < 0) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "littlefs/lfs.pyx":425
+  /* "littlefs/lfs.pyx":428
  * 
  * 
  * def file_read(LFSFilesystem fs, LFSFile fh, size):             # <<<<<<<<<<<<<<
  *     assert size >= 0, 'Size must be >= 0'
  *     buffer = b'\0xff' * size
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_35file_read, 0, __pyx_n_s_file_read, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__80)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 425, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_35file_read, 0, __pyx_n_s_file_read, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__80)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_file_read, __pyx_t_7) < 0) __PYX_ERR(0, 425, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_file_read, __pyx_t_7) < 0) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "littlefs/lfs.pyx":432
+  /* "littlefs/lfs.pyx":435
  * 
  * 
  * def file_write(LFSFilesystem fs, LFSFile fh, data):             # <<<<<<<<<<<<<<
  *     assert isinstance(data, (bytes, bytearray))
  *     pdata = <char *>data
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_37file_write, 0, __pyx_n_s_file_write, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 432, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_37file_write, 0, __pyx_n_s_file_write, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 435, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_file_write, __pyx_t_7) < 0) __PYX_ERR(0, 432, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_file_write, __pyx_t_7) < 0) __PYX_ERR(0, 435, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "littlefs/lfs.pyx":441
+  /* "littlefs/lfs.pyx":444
  * 
  * 
  * def file_seek(LFSFilesystem fs, LFSFile fh, off, whence):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_file_seek(&fs._impl, &fh._impl, off, whence))
  * 
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_39file_seek, 0, __pyx_n_s_file_seek, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__84)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 441, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_39file_seek, 0, __pyx_n_s_file_seek, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__84)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 444, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_file_seek, __pyx_t_7) < 0) __PYX_ERR(0, 441, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_file_seek, __pyx_t_7) < 0) __PYX_ERR(0, 444, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "littlefs/lfs.pyx":445
+  /* "littlefs/lfs.pyx":448
  * 
  * 
  * def file_truncate(LFSFilesystem fs, LFSFile fh, size):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_file_truncate(&fs._impl, &fh._impl, size))
  * 
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_41file_truncate, 0, __pyx_n_s_file_truncate, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__86)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 445, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_41file_truncate, 0, __pyx_n_s_file_truncate, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__86)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 448, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_file_truncate, __pyx_t_7) < 0) __PYX_ERR(0, 445, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_file_truncate, __pyx_t_7) < 0) __PYX_ERR(0, 448, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "littlefs/lfs.pyx":449
+  /* "littlefs/lfs.pyx":452
  * 
  * 
  * def file_tell(LFSFilesystem fs, LFSFile fh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_file_tell(&fs._impl, &fh._impl))
  * 
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_43file_tell, 0, __pyx_n_s_file_tell, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__87)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 449, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_43file_tell, 0, __pyx_n_s_file_tell, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__87)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 452, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_file_tell, __pyx_t_7) < 0) __PYX_ERR(0, 449, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_file_tell, __pyx_t_7) < 0) __PYX_ERR(0, 452, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "littlefs/lfs.pyx":453
+  /* "littlefs/lfs.pyx":456
  * 
  * 
  * def file_rewind(LFSFilesystem fs, LFSFile fh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_file_rewind(&fs._impl, &fh._impl))
  * 
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_45file_rewind, 0, __pyx_n_s_file_rewind, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__88)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 453, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_45file_rewind, 0, __pyx_n_s_file_rewind, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__88)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 456, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_file_rewind, __pyx_t_7) < 0) __PYX_ERR(0, 453, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_file_rewind, __pyx_t_7) < 0) __PYX_ERR(0, 456, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "littlefs/lfs.pyx":457
+  /* "littlefs/lfs.pyx":460
  * 
  * 
  * def file_size(LFSFilesystem fs, LFSFile fh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_file_size(&fs._impl, &fh._impl))
  * 
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_47file_size, 0, __pyx_n_s_file_size, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__89)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 457, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_47file_size, 0, __pyx_n_s_file_size, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__89)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 460, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_file_size, __pyx_t_7) < 0) __PYX_ERR(0, 457, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_file_size, __pyx_t_7) < 0) __PYX_ERR(0, 460, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "littlefs/lfs.pyx":460
+  /* "littlefs/lfs.pyx":463
  *     return _raise_on_error(lfs_file_size(&fs._impl, &fh._impl))
  * 
  * def mkdir(LFSFilesystem fs, path):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_mkdir(&fs._impl, path.encode(FILENAME_ENCODING)))
  * 
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_49mkdir, 0, __pyx_n_s_mkdir, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__90)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 460, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_49mkdir, 0, __pyx_n_s_mkdir, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__90)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 463, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_mkdir, __pyx_t_7) < 0) __PYX_ERR(0, 460, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_mkdir, __pyx_t_7) < 0) __PYX_ERR(0, 463, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "littlefs/lfs.pyx":463
+  /* "littlefs/lfs.pyx":466
  *     return _raise_on_error(lfs_mkdir(&fs._impl, path.encode(FILENAME_ENCODING)))
  * 
  * def dir_open(LFSFilesystem fs, path):             # <<<<<<<<<<<<<<
  *     handle = LFSDirectory()
  *     _raise_on_error(lfs_dir_open(&fs._impl, &handle._impl, path.encode(FILENAME_ENCODING)))
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_51dir_open, 0, __pyx_n_s_dir_open, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__92)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 463, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_51dir_open, 0, __pyx_n_s_dir_open, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__92)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 466, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_dir_open, __pyx_t_7) < 0) __PYX_ERR(0, 463, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_dir_open, __pyx_t_7) < 0) __PYX_ERR(0, 466, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "littlefs/lfs.pyx":468
+  /* "littlefs/lfs.pyx":471
  *     return handle
  * 
  * def dir_close(LFSFilesystem fs, LFSDirectory dh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_dir_close(&fs._impl, &dh._impl))
  * 
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_53dir_close, 0, __pyx_n_s_dir_close, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__94)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 468, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_53dir_close, 0, __pyx_n_s_dir_close, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__94)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 471, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_dir_close, __pyx_t_7) < 0) __PYX_ERR(0, 468, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_dir_close, __pyx_t_7) < 0) __PYX_ERR(0, 471, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "littlefs/lfs.pyx":471
+  /* "littlefs/lfs.pyx":474
  *     return _raise_on_error(lfs_dir_close(&fs._impl, &dh._impl))
  * 
  * def dir_read(LFSFilesystem fs, LFSDirectory dh):             # <<<<<<<<<<<<<<
  *     cdef lfs_info * info = <lfs_info *>malloc(sizeof(lfs_info))
  *     try:
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_55dir_read, 0, __pyx_n_s_dir_read, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__96)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 471, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_55dir_read, 0, __pyx_n_s_dir_read, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__96)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 474, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_dir_read, __pyx_t_7) < 0) __PYX_ERR(0, 471, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_dir_read, __pyx_t_7) < 0) __PYX_ERR(0, 474, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "littlefs/lfs.pyx":481
+  /* "littlefs/lfs.pyx":484
  *         free(info)
  * 
  * def dir_tell(LFSFilesystem fs, LFSDirectory dh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_dir_tell(&fs._impl, &dh._impl))
  * 
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_57dir_tell, 0, __pyx_n_s_dir_tell, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__97)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 481, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_57dir_tell, 0, __pyx_n_s_dir_tell, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__97)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_dir_tell, __pyx_t_7) < 0) __PYX_ERR(0, 481, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_dir_tell, __pyx_t_7) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "littlefs/lfs.pyx":484
+  /* "littlefs/lfs.pyx":487
  *     return _raise_on_error(lfs_dir_tell(&fs._impl, &dh._impl))
  * 
  * def dir_rewind(LFSFilesystem fs, LFSDirectory dh):             # <<<<<<<<<<<<<<
  *     return _raise_on_error(lfs_dir_rewind(&fs._impl, &dh._impl))
- * 
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_59dir_rewind, 0, __pyx_n_s_dir_rewind, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__98)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 484, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8littlefs_3lfs_59dir_rewind, 0, __pyx_n_s_dir_rewind, NULL, __pyx_n_s_littlefs_lfs, __pyx_d, ((PyObject *)__pyx_codeobj__98)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 487, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_dir_rewind, __pyx_t_7) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_dir_rewind, __pyx_t_7) < 0) __PYX_ERR(0, 487, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "littlefs/lfs.pyx":1
  * import logging             # <<<<<<<<<<<<<<
  * import enum
- * from collections import namedtuple
+ * from typing import NamedTuple
  */
   __pyx_t_7 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_7) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /*--- Wrapped vars code ---*/
@@ -34651,19 +34648,19 @@
     {
         if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
     }
     for (i = 0; i < n; i++)
     {
         int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
         if (unlikely(eq != 0)) {
-            if (unlikely(eq < 0)) return NULL;  // error
+            if (unlikely(eq < 0)) return NULL;
             return kwvalues[i];
         }
     }
-    return NULL;  // not found (no exception set)
+    return NULL;
 }
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
 CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
     Py_ssize_t i, nkwargs = PyTuple_GET_SIZE(kwnames);
     PyObject *dict;
     dict = PyDict_New();
     if (unlikely(!dict))
@@ -34768,15 +34765,15 @@
 #endif
         }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_INCREF(value); // transfer ownership of value to values
+            Py_INCREF(value);
             Py_DECREF(key);
 #endif
             key = NULL;
             value = NULL;
             continue;
         }
 #if !CYTHON_AVOID_BORROWED_REFS
@@ -34787,15 +34784,15 @@
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL;  // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -34819,15 +34816,15 @@
                 #endif
                     PyUnicode_Compare(**name, key)
                 );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL; // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -39345,15 +39342,15 @@
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
     #else
     py_code = PyCode_NewEmpty(filename, funcname, py_line);
     #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_XDECREF(py_funcname);
     return py_code;
 bad:
     Py_XDECREF(py_funcname);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
     #endif
     return NULL;
@@ -40494,14 +40491,78 @@
     } else {
         __pyx_fatalerror("Acquisition count is %d (line %d)",
                          old_acquisition_count-1, lineno);
     }
 }
 
 /* CIntToPy */
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__lfs_type(enum lfs_type value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const enum lfs_type neg_one = (enum lfs_type) -1, const_zero = (enum lfs_type) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(enum lfs_type) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(enum lfs_type) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(enum lfs_type) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(enum lfs_type) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(enum lfs_type) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
+        return _PyLong_FromByteArray(bytes, sizeof(enum lfs_type),
+                                     little, !is_unsigned);
+#else
+        PyObject *from_bytes, *result = NULL;
+        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
+        if (!from_bytes) return NULL;
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(enum lfs_type));
+        if (!py_bytes) goto limited_bad;
+        order_str = PyUnicode_FromString(little ? "little" : "big");
+        if (!order_str) goto limited_bad;
+        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
+        if (!arg_tuple) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
+        result = PyObject_Call(from_bytes, arg_tuple, kwds);
+        limited_bad:
+        Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
+        return result;
+#endif
+    }
+}
+
+/* CIntToPy */
   static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__lfs_open_flags(enum lfs_open_flags value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const enum lfs_open_flags neg_one = (enum lfs_open_flags) -1, const_zero = (enum lfs_open_flags) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
```

### Comparing `littlefs-python-0.9.1/src/littlefs/lfs.pxd` & `littlefs-python-0.9.3/src/littlefs/lfs.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,18 @@
         LFS_F_DIRTY   = 0x010000 # File does not match storage
         LFS_F_WRITING = 0x020000 # File has been written since last flush
         LFS_F_READING = 0x040000 # File has been read since last flush
         LFS_F_ERRED   = 0x080000 # An error occurred during write
         LFS_F_INLINE  = 0x100000 # Currently inlined in directory entry
         LFS_F_OPENED  = 0x200000 # File has been opened
 
+    cdef enum lfs_type:
+        # littlefs-python: Only exporting public values for now.
+        LFS_TYPE_REG = 0x001
+        LFS_TYPE_DIR = 0x002
 
     cdef struct lfs:
         lfs_size_t block_count
 
     ctypedef lfs lfs_t
 
     cdef struct lfs_info:
```

### Comparing `littlefs-python-0.9.1/src/littlefs/lfs.pyi` & `littlefs-python-0.9.3/src/littlefs/lfs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,108 +2,101 @@
 from typing import Tuple, NamedTuple, Optional, Union
 from littlefs.context import UserContext
 
 FILENAME_ENCODING: str = ...
 __LFS_VERSION__: Tuple[int, int] = ...
 __LFS_DISK_VERSION__: Tuple[int, int] = ...
 
-LFSStat = NamedTuple('LFSStat', [
-    ('type', int),
-    ('size', int),
-    ('name', str)
-])
-
-LFSFSStat = NamedTuple('LFSFSStat', [
-    'disk_version',
-    'name_max',
-    'file_max',
-    'attr_max',
-    'block_count',
-    'block_size',
-])
-
+class LFSStat(NamedTuple):
+    type: int
+    size: int
+    name: str
+
+    # Constants
+    TYPE_REG: int = LFS_TYPE_REG
+    TYPE_DIR: int = LFS_TYPE_DIR
+
+class LFSFSStat(NamedTuple):
+    """Littlefs filesystem status."""
+
+    disk_version: int
+    name_max: int
+    file_max: int
+    attr_max: int
+    block_count: int
+    block_size: int
 
 class LFSFileFlag(enum.IntFlag): ...
 
 class LFSConfig:
-
     user_context: UserContext = ...
 
-    def __init__(self,
-                 context=None,
-                 *,
-                 block_size: int = 128,
-                 block_count: int = 64,
-                 read_size: int = 0,
-                 prog_size: int = 0,
-                 block_cycles: int = -1,
-                 cache_size: int = 0,
-                 lookahead_size: int = 8,
-                 name_max: int = 255,
-                 file_max: int = 0,
-                 attr_max: int = 0,
-                 metadata_max: int = 0,
-                 disk_version: int = 0,
-                )-> None: ...
-
+    def __init__(
+        self,
+        context=None,
+        *,
+        block_size: int = 128,
+        block_count: int = 64,
+        read_size: int = 0,
+        prog_size: int = 0,
+        block_cycles: int = -1,
+        cache_size: int = 0,
+        lookahead_size: int = 8,
+        name_max: int = 255,
+        file_max: int = 0,
+        attr_max: int = 0,
+        metadata_max: int = 0,
+        disk_version: int = 0,
+    ) -> None: ...
     @property
     def read_size(self) -> int: ...
-
     @property
     def prog_size(self) -> int: ...
-
     @property
     def block_size(self) -> int: ...
-
     @property
     def block_count(self) -> int: ...
-
     @property
     def cache_size(self) -> int: ...
-
     @property
     def lookahead_size(self) -> int: ...
-
     @property
     def name_max(self) -> int: ...
-
     @property
     def file_max(self) -> int: ...
-
     @property
     def attr_max(self) -> int: ...
 
 class LFSFilesystem:
     @property
     def block_count(self) -> int: ...
 
 # The following classes are opaque wrappers around the actual handles
 class LFSFile: ...
 class LFSDirectory: ...
 
-
 def fs_stat(fs: LFSFilesystem) -> LFSFSStat: ...
 def fs_size(fs: LFSFilesystem) -> int: ...
 def format(fs: LFSFilesystem, cfg: LFSConfig) -> int: ...
 def mount(fs: LFSFilesystem, cfg: LFSConfig) -> int: ...
 def unmount(fs: LFSFilesystem) -> int: ...
 def fs_mkconsistent(fs: LFSFilesystem) -> int: ...
 def fs_grow(fs: LFSFilesystem, block_count) -> int: ...
-
 def remove(fs: LFSFilesystem, path: str) -> int: ...
 def rename(fs: LFSFilesystem, oldpath: str, newpath: str) -> int: ...
 def stat(fs: LFSFilesystem, path: str) -> LFSStat: ...
 
 # Attributes
 def getattr(fs: LFSFilesystem, path: str, typ) -> bytes: ...
 def setattr(fs: LFSFilesystem, path: str, typ, data) -> None: ...
 def removeattr(fs: LFSFilesystem, path: str, typ) -> None: ...
 
 # File Handling
 def file_open(fs: LFSFilesystem, path: str, flags: Union[str, LFSFileFlag]) -> LFSFile: ...
+
 # def file_open_cfg(self, path, flags, config): ...
 def file_close(fs: LFSFilesystem, fh: LFSFile) -> int: ...
 def file_sync(fs: LFSFilesystem, fh: LFSFile) -> int: ...
 def file_read(fs: LFSFilesystem, fh: LFSFile, size) -> bytes: ...
 def file_write(fs: LFSFilesystem, fh: LFSFile, data) -> int: ...
 def file_seek(fs: LFSFilesystem, fh: LFSFile, off, whence) -> int: ...
 def file_truncate(fs: LFSFilesystem, fh: LFSFile, size) -> int: ...
@@ -114,8 +107,7 @@
 # Directory Handling
 def mkdir(fs: LFSFilesystem, path: str) -> int: ...
 def dir_open(fs: LFSFilesystem, path: str) -> LFSDirectory: ...
 def dir_close(fs: LFSFilesystem, dh: LFSDirectory) -> int: ...
 def dir_read(fs: LFSFilesystem, dh: LFSDirectory) -> LFSStat: ...
 def dir_tell(fs: LFSFilesystem, dh: LFSDirectory) -> int: ...
 def dir_rewind(fs: LFSFilesystem, dh: LFSDirectory) -> int: ...
-
```

### Comparing `littlefs-python-0.9.1/src/littlefs/lfs.pyx` & `littlefs-python-0.9.3/src/littlefs/lfs.pyx`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 import logging
 import enum
-from collections import namedtuple
+from typing import NamedTuple
 # Import all definitions
 # from littlefs._lfs cimport *
 
 from littlefs.context import UserContext
 from littlefs import errors
 
 
 FILENAME_ENCODING = 'ascii'
 """Default filename encoding"""
 
-LFSStat = namedtuple('LFSStat', ['type', 'size', 'name'])
-LFSStat.__doc__ = """\
-Littlefs File / Directory status
-"""
-
-LFSFSStat = namedtuple('LFSFSStat', [
-    'disk_version',
-    'name_max',
-    'file_max',
-    'attr_max',
-    'block_count',
-    'block_size',
-])
-LFSFSStat.__doc__ = """\
-Littlefs filesystem status
-"""
+class LFSStat(NamedTuple):
+    """Littlefs File / Directory status."""
+    type: int
+    size: int
+    name: str
+
+    # Constants
+    TYPE_REG = LFS_TYPE_REG
+    TYPE_DIR = LFS_TYPE_DIR
+
+
+class LFSFSStat(NamedTuple):
+    """Littlefs filesystem status."""
+    disk_version: int
+    name_max: int
+    file_max: int
+    attr_max: int
+    block_count: int
+    block_size: int
 
 
 class LFSFileFlag(enum.IntFlag):
     """Littlefs file mode flags"""
     rdonly = LFS_O_RDONLY
     wronly = LFS_O_WRONLY
     rdwr = LFS_O_RDWR
@@ -479,8 +482,7 @@
         free(info)
 
 def dir_tell(LFSFilesystem fs, LFSDirectory dh):
     return _raise_on_error(lfs_dir_tell(&fs._impl, &dh._impl))
 
 def dir_rewind(LFSFilesystem fs, LFSDirectory dh):
     return _raise_on_error(lfs_dir_rewind(&fs._impl, &dh._impl))
-
```

### Comparing `littlefs-python-0.9.1/src/littlefs_python.egg-info/PKG-INFO` & `littlefs-python-0.9.3/src/littlefs_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: littlefs-python
-Version: 0.9.1
+Version: 0.9.3
 Summary: A python wrapper for littlefs
 Home-page: https://github.com/jrast/littlefs-python
 Author: Jürg Rast
 Author-email: juergr@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `littlefs-python-0.9.1/src/littlefs_python.egg-info/SOURCES.txt` & `littlefs-python-0.9.3/src/littlefs_python.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .gitattributes
 .gitignore
 .gitmodules
+.pre-commit-config.yaml
 .readthedocs.yml
 LICENSE
 MANIFEST.in
 README.rst
 mypy.ini
 pyproject.toml
 requirements.txt
```

### Comparing `littlefs-python-0.9.1/test/lfs/conftest.py` & `littlefs-python-0.9.3/test/lfs/conftest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import pytest
 from littlefs import lfs
 
-@pytest.fixture(scope='function')
+
+@pytest.fixture(scope="function")
 def fs():
     """Littlefs filesystem fixture"""
     fs = lfs.LFSFilesystem()
     yield fs
 
-@pytest.fixture(scope='function')
+
+@pytest.fixture(scope="function")
 def cfg():
     """Littlefs configuration fixture"""
     cfg = lfs.LFSConfig(block_size=128, block_count=4)
     yield cfg
 
-@pytest.fixture(scope='function')
+
+@pytest.fixture(scope="function")
 def formated_fs(fs, cfg):
     """fixutre for a formatted filesystem"""
     lfs.format(fs, cfg)
     yield fs
 
-@pytest.fixture(scope='function')
+
+@pytest.fixture(scope="function")
 def mounted_fs(formated_fs, cfg):
     """fixture for a formatted and mounted filesystem"""
     lfs.mount(formated_fs, cfg)
-    yield formated_fs
+    yield formated_fs
```

### Comparing `littlefs-python-0.9.1/test/lfs/test_dir_functions.py` & `littlefs-python-0.9.3/test/lfs/test_dir_functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 import pytest
 from littlefs import lfs
 
 
-@pytest.fixture(scope='function')
+@pytest.fixture(scope="function")
 def testfs(mounted_fs):
-    lfs.mkdir(mounted_fs, 'testdir')
+    lfs.mkdir(mounted_fs, "testdir")
     yield mounted_fs
 
 
 def test_mkdir(mounted_fs):
-    assert lfs.mkdir(mounted_fs, 'directory') == 0
+    assert lfs.mkdir(mounted_fs, "directory") == 0
 
 
 def test_dir_open(testfs):
-    dh = lfs.dir_open(testfs, 'testdir')
+    dh = lfs.dir_open(testfs, "testdir")
     assert dh != None
 
 
 def test_dir_close(testfs):
-    dh = lfs.dir_open(testfs, 'testdir')
+    dh = lfs.dir_open(testfs, "testdir")
     lfs.dir_close(testfs, dh)
 
 
 def test_dir_read(testfs):
-    dh = lfs.dir_open(testfs, '')
+    dh = lfs.dir_open(testfs, "")
     info = lfs.dir_read(testfs, dh)
-    assert info.name == '.'
+    assert info.name == "."
 
     info = lfs.dir_read(testfs, dh)
-    assert info.name == '..'
+    assert info.name == ".."
 
     info = lfs.dir_read(testfs, dh)
-    assert info.name == 'testdir'
+    assert info.name == "testdir"
 
 
 def test_dir_read_overflow(testfs):
-    dh = lfs.dir_open(testfs, '')
+    dh = lfs.dir_open(testfs, "")
 
     # There are three directories: ., .., testdir
     for _ in range(3):
         info = lfs.dir_read(testfs, dh)
         assert info is not None
 
     # If we read one more, we should get None
     info = lfs.dir_read(testfs, dh)
     assert info is None
 
 
 def test_dir_rewind(testfs):
-    dirs = ['.', '..', 'testdir']
-    dh = lfs.dir_open(testfs, '')
+    dirs = [".", "..", "testdir"]
+    dh = lfs.dir_open(testfs, "")
 
     for name in dirs:
         info = lfs.dir_read(testfs, dh)
         assert info.name == name
 
     lfs.dir_rewind(testfs, dh)
```

### Comparing `littlefs-python-0.9.1/test/lfs/test_fs_functions.py` & `littlefs-python-0.9.3/test/lfs/test_fs_functions.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,29 +27,33 @@
 def test_unmount(mounted_fs):
     """Test if the filesystem can be unmounted"""
     assert lfs.unmount(mounted_fs) == 0
 
 
 def test_stat_root_directory(mounted_fs):
     """Test if stat works"""
-    stat = lfs.stat(mounted_fs, '/')
-    assert stat.type == 2, 'Expected a directory type'
-    assert stat.name == '/'
+    stat = lfs.stat(mounted_fs, "/")
+    assert stat.type == 2, "Expected a directory type"
+    assert stat.name == "/"
 
 
 def test_stat_file(mounted_fs):
-    fh = lfs.file_open(mounted_fs, 'test.txt', 'w')
-    lfs.file_write(mounted_fs, fh, b'0123456789')
+    fh = lfs.file_open(mounted_fs, "test.txt", "w")
+    lfs.file_write(mounted_fs, fh, b"0123456789")
     lfs.file_close(mounted_fs, fh)
 
-    stat = lfs.stat(mounted_fs, 'test.txt')
+    stat = lfs.stat(mounted_fs, "test.txt")
 
     assert stat.size == 10
     assert stat.type == 1
-    assert stat.name == 'test.txt'
+    assert stat.name == "test.txt"
+
+    # Double checking that these constant got passed through.
+    assert stat.TYPE_REG == 0x001
+    assert stat.TYPE_DIR == 0x002
 
 
 def test_fs_stat(mounted_fs):
     """Test if fs stat works"""
     stat = lfs.fs_stat(mounted_fs)
     # The following values are defaults in littlefs.
     assert stat.disk_version == 0x00020001
```

### Comparing `littlefs-python-0.9.1/test/test_attr.py` & `littlefs-python-0.9.3/test/test_attr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import pytest
 from littlefs import LittleFS, LittleFSError
 
 
-@pytest.fixture(scope='function')
+@pytest.fixture(scope="function")
 def fs():
     fs = LittleFS(block_size=128, block_count=64)
-    with fs.open('/file.txt', 'w') as fh:
-        fh.write('Sample Text')
+    with fs.open("/file.txt", "w") as fh:
+        fh.write("Sample Text")
     yield fs
 
 
 def test_attr(fs):
     # Test if 2 attributes can be set without impacting each other.
     fs.setattr("/file.txt", "f", b"foo")
     fs.setattr("/file.txt", "b", b"bar")
 
-    assert(b"foo" == fs.getattr("/file.txt", "f"))
-    assert(b"bar" == fs.getattr("/file.txt", "b"))
+    assert b"foo" == fs.getattr("/file.txt", "f")
+    assert b"bar" == fs.getattr("/file.txt", "b")
 
     fs.removeattr("/file.txt", "f")
     with pytest.raises(LittleFSError):
         fs.getattr("/file.txt", "f")
 
     # Make sure "b" wasn't impacted
-    assert(b"bar" == fs.getattr("/file.txt", "b"))
+    assert b"bar" == fs.getattr("/file.txt", "b")
```

### Comparing `littlefs-python-0.9.1/test/test_files.py` & `littlefs-python-0.9.3/test/test_files.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,230 +1,229 @@
 import pytest
 from littlefs import LittleFS, FileHandle
 
 
-@pytest.fixture(scope='function')
+@pytest.fixture(scope="function")
 def fs():
     fs = LittleFS(block_size=128, block_count=64)
-    fs.mkdir('mydir')
+    fs.mkdir("mydir")
 
-    with fs.open('test.txt', 'w') as f:
-        f.write('1234567890')
+    with fs.open("test.txt", "w") as f:
+        f.write("1234567890")
 
-    with fs.open('test.bin', 'wb') as f:
-        contents = bytes.fromhex('11 22 33 44 aa bb cc dd ee ff')
+    with fs.open("test.bin", "wb") as f:
+        contents = bytes.fromhex("11 22 33 44 aa bb cc dd ee ff")
         f.write(contents)
 
     yield fs
 
 
 def test_open_notfound(fs):
     with pytest.raises(FileNotFoundError):
-        with fs.open('test2.txt') as f:
+        with fs.open("test2.txt") as f:
             pass
 
 
 def test_open_isdir(fs):
     with pytest.raises(IsADirectoryError):
-        with fs.open('mydir') as f:
+        with fs.open("mydir") as f:
             pass
 
 
 def test_open_exists(fs):
     with pytest.raises(FileExistsError):
-        with fs.open('test.txt', 'x') as f:
+        with fs.open("test.txt", "x") as f:
             pass
 
+
 def test_open_invalid_mode(fs):
     with pytest.raises(ValueError) as excinfo:
-        with fs.open('test.txt', 'c') as fh:
+        with fs.open("test.txt", "c") as fh:
             pass
-    
+
     assert str(excinfo.value) == "invalid mode: 'c'"
 
+
 def test_open_binary_and_text(fs):
     with pytest.raises(ValueError) as excinfo:
-        with fs.open('test.txt', 'bt') as fh:
+        with fs.open("test.txt", "bt") as fh:
             pass
 
     assert str(excinfo.value) == "can't have text and binary mode at once"
 
 
 def test_bin_read(fs):
-    with fs.open('test.txt', 'rb') as f:
+    with fs.open("test.txt", "rb") as f:
         data = f.read()
 
-    assert data == b'1234567890'
+    assert data == b"1234567890"
 
 
 def test_text_read(fs):
-    with fs.open('test.txt', 'rt') as f:
+    with fs.open("test.txt", "rt") as f:
         data = f.read()
 
-    assert data == '1234567890'
+    assert data == "1234567890"
 
 
 def test_bin_append(fs):
-    with fs.open('test.txt', 'ab') as f:
-        f.write(b'1234567890')
+    with fs.open("test.txt", "ab") as f:
+        f.write(b"1234567890")
 
-    info = fs.stat('test.txt')
+    info = fs.stat("test.txt")
     assert info.size == 20
 
 
 def test_text_encoding(fs):
-    txt_data = (
-        'abcdefghijklmnopqrstuvwxyz'
-        'αβγδεζηθικλμνξοπρστυφχψω'
-    )
-    bin_data = txt_data.encode('utf8')
+    txt_data = "abcdefghijklmnopqrstuvwxyz" "αβγδεζηθικλμνξοπρστυφχψω"
+    bin_data = txt_data.encode("utf8")
 
-    with fs.open("test2.txt", "w", encoding='utf8') as f:
+    with fs.open("test2.txt", "w", encoding="utf8") as f:
         f.write(txt_data)
 
-    info = fs.stat('test2.txt')
+    info = fs.stat("test2.txt")
     assert info.size == len(bin_data)
 
-    with fs.open('test2.txt', 'rb') as f:
+    with fs.open("test2.txt", "rb") as f:
         data = f.read()
         assert data == bin_data
 
-    with fs.open('test2.txt', 'r', encoding='utf8') as f:
+    with fs.open("test2.txt", "r", encoding="utf8") as f:
         data = f.read()
         assert data == txt_data
 
     offset = 30
-    file_offset = len(txt_data[:offset].encode('utf8'))
+    file_offset = len(txt_data[:offset].encode("utf8"))
 
-    with fs.open('test2.txt', 'r', encoding='utf8') as f:
+    with fs.open("test2.txt", "r", encoding="utf8") as f:
         f.seek(file_offset)
         data = f.read(4)
-        assert data == txt_data[offset:offset+4]
+        assert data == txt_data[offset : offset + 4]
 
 
 def test_text_lines(fs):
     fname = "test2.txt"
     lipsum = (
-        'Lorem ipsum dolor sit amet, consectetur adipiscing elit, \n'
-        'sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.\n'
-        'Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris \n'
-        'nisi ut aliquip ex ea commodo consequat.'
+        "Lorem ipsum dolor sit amet, consectetur adipiscing elit, \n"
+        "sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.\n"
+        "Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris \n"
+        "nisi ut aliquip ex ea commodo consequat."
     )
 
-
-    with fs.open(fname, 'w') as f:
+    with fs.open(fname, "w") as f:
         f.write(lipsum)
 
     num_lines = 0
 
-    with fs.open(fname, 'r') as f:
+    with fs.open(fname, "r") as f:
         for _ in f:
             num_lines += 1
 
     assert num_lines == len(lipsum.splitlines())
 
 
 def test_bin_read_update(fs):
-    with fs.open('test.bin', 'r+b') as f:
+    with fs.open("test.bin", "r+b") as f:
         f.seek(2)
         a = f.read(2)
         b = f.read(2)
 
-        assert a == bytes.fromhex('33 44')
-        assert b == bytes.fromhex('aa bb')
+        assert a == bytes.fromhex("33 44")
+        assert b == bytes.fromhex("aa bb")
         assert f.tell() == 6
 
         f.seek(2)
         f.write(b)
         f.write(a)
 
-    expected = bytes.fromhex('11 22 aa bb 33 44 cc dd ee ff')
+    expected = bytes.fromhex("11 22 aa bb 33 44 cc dd ee ff")
 
-    with fs.open('test.bin', 'rb') as f:
+    with fs.open("test.bin", "rb") as f:
         data = f.read()
         assert data == expected
 
 
 def test_bin_write_update(fs):
-    contents = bytes.fromhex('11 aa 22 bb 33 cc 44 dd')
+    contents = bytes.fromhex("11 aa 22 bb 33 cc 44 dd")
 
-    with fs.open('test.bin', 'w+b') as f:
+    with fs.open("test.bin", "w+b") as f:
         data = f.read()
-        assert data == b''
+        assert data == b""
 
         f.write(contents)
         f.seek(4)
         data = f.read(4)
         assert data == contents[4:8]
 
 
 def test_bin_append_update(fs):
-    fname = 'test2.bin'
-    contents = bytes.fromhex('11 aa 22 bb 33 cc 44 dd')
+    fname = "test2.bin"
+    contents = bytes.fromhex("11 aa 22 bb 33 cc 44 dd")
 
-    with fs.open(fname, 'wb') as f:
+    with fs.open(fname, "wb") as f:
         f.write(contents[0:6])
 
-    with fs.open(fname, 'a+b') as f:
+    with fs.open(fname, "a+b") as f:
         f.write(contents[6:])
         f.seek(0)
 
         data = f.read()
         assert data == contents
 
 
 def test_text_read_update(fs):
-    with fs.open('test.txt', 'r+') as f:
+    with fs.open("test.txt", "r+") as f:
         f.seek(2)
         a = f.read(2)
         b = f.read(2)
 
         assert a == "34"
         assert b == "56"
         assert f.tell() == 6
 
         f.seek(2)
         f.write(b)
         f.write(a)
 
     expected = "1256347890"
 
-    with fs.open('test.txt', 'r') as f:
+    with fs.open("test.txt", "r") as f:
         data = f.read()
         assert data == expected
 
 
 def test_text_write_update(fs):
     contents = "1a2b3c4d"
 
-    with fs.open('test.txt', 'w+') as f:
+    with fs.open("test.txt", "w+") as f:
         data = f.read()
         assert data == ""
 
         f.write(contents)
         f.seek(4)
         data = f.read(4)
         assert data == contents[4:8]
 
 
 def test_text_append_update(fs):
-    fname = 'test2.txt'
+    fname = "test2.txt"
     contents = "1a2b3c4d"
 
-    with fs.open(fname, 'w') as f:
+    with fs.open(fname, "w") as f:
         f.write(contents[0:6])
 
-    with fs.open(fname, 'a+') as f:
+    with fs.open(fname, "a+") as f:
         f.write(contents[6:])
         f.seek(0)
 
         data = f.read()
         assert data == contents
 
+
 def test_text_truncate(fs: LittleFS):
-    with fs.open('trunc.txt', 'w') as f:
-        f.write('Some Content')
+    with fs.open("trunc.txt", "w") as f:
+        f.write("Some Content")
 
-    with fs.open('trunc.txt', 'r+') as f:
+    with fs.open("trunc.txt", "r+") as f:
         f.truncate()
 
-    assert fs.open('trunc.txt', 'r').read() == ''
+    assert fs.open("trunc.txt", "r").read() == ""
```

### Comparing `littlefs-python-0.9.1/test/test_multiversion.py` & `littlefs-python-0.9.3/test/test_multiversion.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,57 @@
 import pytest
 from littlefs import LittleFS, FileHandle, LittleFSError
 
 
 def create_image(version):
     fs = LittleFS(block_size=128, block_count=64, disk_version=version)
-    fs.mkdir('testdir')
-    with fs.open('file.txt', 'w') as f:
-        f.write('Sample Content')
-    
+    fs.mkdir("testdir")
+    with fs.open("file.txt", "w") as f:
+        f.write("Sample Content")
+
     return fs.context.buffer
 
 
-@pytest.fixture(scope='function')
+@pytest.fixture(scope="function")
 def fs20():
     fs = LittleFS(block_size=128, block_count=64, disk_version=0x00020000)
-    fs.mkdir('mydir')
+    fs.mkdir("mydir")
 
-    with fs.open('test.txt', 'w') as f:
-        f.write('1234567890')
+    with fs.open("test.txt", "w") as f:
+        f.write("1234567890")
 
     yield fs
 
-@pytest.fixture(scope='function')
+
+@pytest.fixture(scope="function")
 def fs21():
     fs = LittleFS(block_size=128, block_count=64, disk_version=0x00020001)
-    fs.mkdir('mydir')
+    fs.mkdir("mydir")
 
-    with fs.open('test.txt', 'w') as f:
-        f.write('1234567890')
+    with fs.open("test.txt", "w") as f:
+        f.write("1234567890")
 
     yield fs
 
+
 def test_lfs20(fs20):
     assert fs20.fs_stat().disk_version == 0x00020000
 
+
 def test_lfs21(fs21):
     assert fs21.fs_stat().disk_version == 0x00020001
 
 
-@pytest.mark.parametrize('version', [0x00020000, 0x00020001], ids=['FS2.0', 'FS2.1'])
+@pytest.mark.parametrize("version", [0x00020000, 0x00020001], ids=["FS2.0", "FS2.1"])
 def test_load_images(version):
     fs = LittleFS(block_size=128, block_count=64, disk_version=0x00020001)
     fs.context.buffer = create_image(version)
     fs.mount()
     stat = fs.fs_stat()
     assert stat.disk_version == version
 
 
-
 def test_load_incompatible_image():
     fs = LittleFS(block_size=128, block_count=64, disk_version=0x00020000)
     fs.context.buffer = create_image(0x00020001)
-    with pytest.raises(LittleFSError, match='-22: LFS_ERR_INVAL'):
-        assert fs.mount()    
+    with pytest.raises(LittleFSError, match="-22: LFS_ERR_INVAL"):
+        assert fs.mount()
```

### Comparing `littlefs-python-0.9.1/test/test_name_max.py` & `littlefs-python-0.9.3/test/test_name_max.py`

 * *Files identical despite different names*

