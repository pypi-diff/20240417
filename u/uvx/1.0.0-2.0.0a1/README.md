# Comparing `tmp/uvx-1.0.0.tar.gz` & `tmp/uvx-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data
```

## Comparing `uvx-1.0.0.tar` & `uvx-2.0.0a1.tar`

### file list

```diff
@@ -1,18 +1,30 @@
--rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 uvx-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 uvx-1.0.0/src/uvx/__about__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 uvx-1.0.0/src/uvx/__init__.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 uvx-1.0.0/src/uvx/_cli_support.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 uvx-1.0.0/src/uvx/_constants.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 uvx-1.0.0/src/uvx/_maybe.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 uvx-1.0.0/src/uvx/_python.py
--rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 uvx-1.0.0/src/uvx/_symlinks.py
--rw-r--r--   0        0        0    13957 2020-02-02 00:00:00.000000 uvx-1.0.0/src/uvx/cli.py
--rw-r--r--   0        0        0    19286 2020-02-02 00:00:00.000000 uvx-1.0.0/src/uvx/core.py
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 uvx-1.0.0/src/uvx/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uvx-1.0.0/src/uvx/py.typed
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 uvx-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 uvx-1.0.0/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 uvx-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 uvx-1.0.0/README.md
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 uvx-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 uvx-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1587 1970-01-01 00:00:00.000000 uvx-2.0.0a1/Cargo.toml
+-rw-rw-r--   0     1000     1000       77 2024-04-15 17:07:31.000000 uvx-2.0.0a1/.cargo/config.toml
+-rw-rw-r--   0     1000     1000      686 2024-04-11 15:03:17.000000 uvx-2.0.0a1/.gitignore
+-rw-rw-r--   0     1000     1000    85890 2024-04-15 17:25:03.000000 uvx-2.0.0a1/Cargo.lock
+-rw-rw-r--   0     1000     1000      137 2024-04-15 17:26:36.000000 uvx-2.0.0a1/build.sh
+-rw-rw-r--   0     1000     1000      106 2024-04-15 17:06:44.000000 uvx-2.0.0a1/rustfmt.toml
+-rw-rw-r--   0     1000     1000     1852 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/animate.rs
+-rw-rw-r--   0     1000     1000     6162 2024-04-15 17:06:13.000000 uvx-2.0.0a1/src/cli.rs
+-rw-rw-r--   0     1000     1000     2262 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/commands/ensurepath.rs
+-rw-rw-r--   0     1000     1000      198 2024-04-15 16:59:35.000000 uvx-2.0.0a1/src/commands/inject.rs
+-rw-rw-r--   0     1000     1000     5052 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/commands/install.rs
+-rw-rw-r--   0     1000     1000     2485 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/commands/list.rs
+-rw-rw-r--   0     1000     1000      214 2024-04-11 18:39:14.000000 uvx-2.0.0a1/src/commands/mod.rs
+-rw-rw-r--   0     1000     1000     2205 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/commands/reinstall.rs
+-rw-rw-r--   0     1000     1000      734 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/commands/runpip.rs
+-rw-rw-r--   0     1000     1000      207 2024-04-15 16:59:35.000000 uvx-2.0.0a1/src/commands/runpython.rs
+-rw-rw-r--   0     1000     1000      643 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/commands/runuv.rs
+-rw-rw-r--   0     1000     1000      211 2024-04-15 16:59:35.000000 uvx-2.0.0a1/src/commands/self_update.rs
+-rw-rw-r--   0     1000     1000     2033 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/commands/uninstall.rs
+-rw-rw-r--   0     1000     1000     4066 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/commands/upgrade.rs
+-rw-rw-r--   0     1000     1000      211 2024-04-15 16:59:35.000000 uvx-2.0.0a1/src/commands/upgrade_all.rs
+-rw-rw-r--   0     1000     1000      970 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/helpers.rs
+-rw-rw-r--   0     1000     1000      565 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/main.rs
+-rw-rw-r--   0     1000     1000     7641 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/metadata.rs
+-rw-rw-r--   0     1000     1000     4637 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/pip.rs
+-rw-rw-r--   0     1000     1000     3724 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/symlinks.rs
+-rw-rw-r--   0     1000     1000     4776 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/uv.rs
+-rw-rw-r--   0     1000     1000     2320 2024-04-15 17:06:47.000000 uvx-2.0.0a1/src/venv.rs
+-rw-rw-r--   0     1000     1000      526 2024-04-15 17:21:16.000000 uvx-2.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0      297 1970-01-01 00:00:00.000000 uvx-2.0.0a1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

