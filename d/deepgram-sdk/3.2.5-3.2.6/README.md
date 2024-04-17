# Comparing `tmp/deepgram-sdk-3.2.5.tar.gz` & `tmp/deepgram_sdk-3.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepgram-sdk-3.2.5.tar", last modified: Mon Apr  8 17:06:31 2024, max compression
+gzip compressed data, was "deepgram_sdk-3.2.6.tar", last modified: Wed Apr 17 00:53:02 2024, max compression
```

## Comparing `deepgram-sdk-3.2.5.tar` & `deepgram_sdk-3.2.6.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.478757 deepgram-sdk-3.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11366 2024-04-08 17:06:31.478757 deepgram-sdk-3.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.466757 deepgram-sdk-3.2.5/deepgram/
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-08 17:06:22.000000 deepgram-sdk-3.2.5/deepgram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.466757 deepgram-sdk-3.2.5/deepgram/audio/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/audio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.466757 deepgram-sdk-3.2.5/deepgram/audio/microphone/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/audio/microphone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/audio/microphone/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/audio/microphone/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/audio/microphone/microphone.py
--rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.470757 deepgram-sdk-3.2.5/deepgram/clients/
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/abstract_async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/abstract_sync_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.470757 deepgram-sdk-3.2.5/deepgram/clients/analyze/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/analyze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/analyze/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/analyze/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/analyze/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.470757 deepgram-sdk-3.2.5/deepgram/clients/analyze/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/analyze/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12291 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/analyze/v1/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12411 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/analyze/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/analyze/v1/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/analyze/v1/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/analyze/v1/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/listen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.470757 deepgram-sdk-3.2.5/deepgram/clients/live/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/live/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/live/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/live/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/live/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/live/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.474757 deepgram-sdk-3.2.5/deepgram/clients/live/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/live/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21558 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/live/v1/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20861 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/live/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/live/v1/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/live/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.474757 deepgram-sdk-3.2.5/deepgram/clients/manage/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/manage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/manage/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.474757 deepgram-sdk-3.2.5/deepgram/clients/manage/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/manage/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33519 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/manage/v1/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    33112 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/manage/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/manage/v1/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    16279 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/manage/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.474757 deepgram-sdk-3.2.5/deepgram/clients/onprem/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/onprem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/onprem/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.474757 deepgram-sdk-3.2.5/deepgram/clients/onprem/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/onprem/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/onprem/v1/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/onprem/v1/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.474757 deepgram-sdk-3.2.5/deepgram/clients/prerecorded/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/prerecorded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/prerecorded/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/prerecorded/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/prerecorded/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.478757 deepgram-sdk-3.2.5/deepgram/clients/prerecorded/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/prerecorded/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12830 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/prerecorded/v1/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12762 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/prerecorded/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/prerecorded/v1/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/prerecorded/v1/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    21250 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/prerecorded/v1/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/read.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.478757 deepgram-sdk-3.2.5/deepgram/clients/speak/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/speak/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/speak/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/speak/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.478757 deepgram-sdk-3.2.5/deepgram/clients/speak/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/speak/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/speak/v1/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/speak/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/speak/v1/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/speak/v1/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/clients/speak/v1/response.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/deepgram/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:06:31.478757 deepgram-sdk-3.2.5/deepgram_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11366 2024-04-08 17:06:31.000000 deepgram-sdk-3.2.5/deepgram_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-08 17:06:31.000000 deepgram-sdk-3.2.5/deepgram_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:06:31.000000 deepgram-sdk-3.2.5/deepgram_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-08 17:06:31.000000 deepgram-sdk-3.2.5/deepgram_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 17:06:31.000000 deepgram-sdk-3.2.5/deepgram_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 17:06:31.478757 deepgram-sdk-3.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-08 17:06:21.000000 deepgram-sdk-3.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.702455 deepgram_sdk-3.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12275 2024-04-17 00:53:02.702455 deepgram_sdk-3.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11524 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.690455 deepgram_sdk-3.2.6/deepgram/
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.690455 deepgram_sdk-3.2.6/deepgram/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/audio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.690455 deepgram_sdk-3.2.6/deepgram/audio/microphone/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/audio/microphone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/audio/microphone/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/audio/microphone/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/audio/microphone/microphone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.694455 deepgram_sdk-3.2.6/deepgram/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/abstract_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/abstract_sync_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.694455 deepgram_sdk-3.2.6/deepgram/clients/analyze/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/analyze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/analyze/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/analyze/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/analyze/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.694455 deepgram_sdk-3.2.6/deepgram/clients/analyze/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/analyze/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12291 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/analyze/v1/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12411 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/analyze/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/analyze/v1/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/analyze/v1/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/analyze/v1/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/listen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.694455 deepgram_sdk-3.2.6/deepgram/clients/live/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/live/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/live/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/live/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/live/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/live/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.694455 deepgram_sdk-3.2.6/deepgram/clients/live/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/live/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21559 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/live/v1/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20858 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/live/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/live/v1/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/live/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.694455 deepgram_sdk-3.2.6/deepgram/clients/manage/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/manage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/manage/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.698455 deepgram_sdk-3.2.6/deepgram/clients/manage/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/manage/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33519 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/manage/v1/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33112 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/manage/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/manage/v1/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16279 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/manage/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.698455 deepgram_sdk-3.2.6/deepgram/clients/onprem/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/onprem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/onprem/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.698455 deepgram_sdk-3.2.6/deepgram/clients/onprem/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/onprem/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/onprem/v1/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/onprem/v1/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.698455 deepgram_sdk-3.2.6/deepgram/clients/prerecorded/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/prerecorded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/prerecorded/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/prerecorded/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/prerecorded/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.698455 deepgram_sdk-3.2.6/deepgram/clients/prerecorded/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/prerecorded/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12830 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/prerecorded/v1/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12762 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/prerecorded/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/prerecorded/v1/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/prerecorded/v1/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21250 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/prerecorded/v1/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/read.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.702455 deepgram_sdk-3.2.6/deepgram/clients/speak/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/speak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/speak/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/speak/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.702455 deepgram_sdk-3.2.6/deepgram/clients/speak/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/speak/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/speak/v1/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/speak/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/speak/v1/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/speak/v1/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/speak/v1/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.702455 deepgram_sdk-3.2.6/deepgram_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12275 2024-04-17 00:53:02.000000 deepgram_sdk-3.2.6/deepgram_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-17 00:53:02.000000 deepgram_sdk-3.2.6/deepgram_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 00:53:02.000000 deepgram_sdk-3.2.6/deepgram_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-17 00:53:02.000000 deepgram_sdk-3.2.6/deepgram_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 00:53:02.000000 deepgram_sdk-3.2.6/deepgram_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 00:53:02.702455 deepgram_sdk-3.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/setup.py
```

### Comparing `deepgram-sdk-3.2.5/LICENSE` & `deepgram_sdk-3.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/PKG-INFO` & `deepgram_sdk-3.2.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: deepgram-sdk
-Version: 3.2.5
-Summary: The official Python SDK for the Deepgram automated speech recognition platform.
-Home-page: https://github.com/deepgram/deepgram-python-sdk
-Author: Deepgram
-Author-email: devrel@deepgram.com
-License: MIT
-Keywords: deepgram,deepgram speech-to-text
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: httpx>=0.25.2
-Requires-Dist: websockets>=12.0
-Requires-Dist: dataclasses-json>=0.6.3
-Requires-Dist: typing_extensions>=4.9.0
-Requires-Dist: aiohttp>=3.9.1
-Requires-Dist: aiofiles>=23.2.1
-Requires-Dist: verboselogs>=1.7
-
 # Deepgram Python SDK
 
 [![Discord](https://dcbadge.vercel.app/api/server/xWRaCDBtW4?style=flat)](https://discord.gg/xWRaCDBtW4) [![GitHub Workflow Status](https://img.shields.io/github/workflow/status/deepgram/deepgram-python-sdk/CI)](https://github.com/deepgram/deepgram-python-sdk/actions/workflows/CI.yml) [![PyPI](https://img.shields.io/pypi/v/deepgram-sdk)](https://pypi.org/project/deepgram-sdk/)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg?style=flat-rounded)](./.github/CODE_OF_CONDUCT.md)
 
 Official Python SDK for [Deepgram](https://www.deepgram.com/). Power your apps with world-class speech and Language AI models.
 
@@ -32,14 +10,16 @@
 - [Getting an API Key](#getting-an-api-key)
 - [Requirements](#requirements)
 - [Installation](#installation)
 - [Quickstarts](#quickstarts)
   - [PreRecorded Audio Transcription Quickstart](#prerecorded-audio-transcription-quickstart)
   - [Live Audio Transcription Quickstart](#live-audio-transcription-quickstart)
 - [Examples](#examples)
+- [Logging](#logging)
+- [Backwards Compatibility](#backwards-compatibility)
 - [Development and Contributing](#development-and-contributing)
 - [Getting Help](#getting-help)
 
 # Documentation
 
 You can learn more about the Deepgram API at [developers.deepgram.com](https://developers.deepgram.com/docs).
 
@@ -221,14 +201,35 @@
     - Members - [examples/manage/members](https://github.com/deepgram/deepgram-python-sdk/blob/main/examples/manage/members/main.py)
     - Projects - [examples/manage/projects](https://github.com/deepgram/deepgram-python-sdk/blob/main/examples/manage/projects/main.py)
     - Scopes - [examples/manage/scopes](https://github.com/deepgram/deepgram-python-sdk/blob/main/examples/manage/scopes/main.py)
     - Usage - [examples/manage/usage](https://github.com/deepgram/deepgram-python-sdk/blob/main/examples/manage/usage/main.py)
 
 To run each example set the `DEEPGRAM_API_KEY` as an environment variable, then `cd` into each example folder and execute the example: `go run main.py`.
 
+
+# Logging
+
+This SDK provides logging as a means to troubleshoot and debug issues encountered. By default, this SDK will enable `Information` level messages and higher (ie `Warning`, `Error`, etc) when you initialize the library as follows:
+
+```python
+deepgram: DeepgramClient = DeepgramClient()
+```
+
+To increase the logging output/verbosity for debug or troubleshooting purposes, you can set the `DEBUG` level but using this code:
+
+```python
+config: DeepgramClientOptions = DeepgramClientOptions(
+    verbose=logging.DEBUG,
+)
+deepgram: DeepgramClient = DeepgramClient("", config)
+```
+# Backwards Compatibility
+
+Older SDK versions will receive Priority 1 (P1) bug support only. Security issues, both in our code and dependencies, are promptly addressed. Significant bugs without clear workarounds are also given priority attention.
+
 # Development and Contributing
 
 Interested in contributing? We ❤️ pull requests!
 
 To make sure our community is safe for all, be sure to review and agree to our
 [Code of Conduct](https://github.com/deepgram/deepgram-python-sdk/blob/main/.github/CODE_OF_CONDUCT.md). Then see the
 [Contribution](https://github.com/deepgram/deepgram-python-sdk/blob/main/.github/CONTRIBUTING.md) guidelines for more information.
```

### Comparing `deepgram-sdk-3.2.5/README.md` & `deepgram_sdk-3.2.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: deepgram-sdk
+Version: 3.2.6
+Summary: The official Python SDK for the Deepgram automated speech recognition platform.
+Home-page: https://github.com/deepgram/deepgram-python-sdk
+Author: Deepgram
+Author-email: devrel@deepgram.com
+License: MIT
+Keywords: deepgram,deepgram speech-to-text
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: httpx>=0.25.2
+Requires-Dist: websockets>=12.0
+Requires-Dist: dataclasses-json>=0.6.3
+Requires-Dist: typing_extensions>=4.9.0
+Requires-Dist: aiohttp>=3.9.1
+Requires-Dist: aiofiles>=23.2.1
+Requires-Dist: verboselogs>=1.7
+
 # Deepgram Python SDK
 
 [![Discord](https://dcbadge.vercel.app/api/server/xWRaCDBtW4?style=flat)](https://discord.gg/xWRaCDBtW4) [![GitHub Workflow Status](https://img.shields.io/github/workflow/status/deepgram/deepgram-python-sdk/CI)](https://github.com/deepgram/deepgram-python-sdk/actions/workflows/CI.yml) [![PyPI](https://img.shields.io/pypi/v/deepgram-sdk)](https://pypi.org/project/deepgram-sdk/)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg?style=flat-rounded)](./.github/CODE_OF_CONDUCT.md)
 
 Official Python SDK for [Deepgram](https://www.deepgram.com/). Power your apps with world-class speech and Language AI models.
 
@@ -10,14 +32,16 @@
 - [Getting an API Key](#getting-an-api-key)
 - [Requirements](#requirements)
 - [Installation](#installation)
 - [Quickstarts](#quickstarts)
   - [PreRecorded Audio Transcription Quickstart](#prerecorded-audio-transcription-quickstart)
   - [Live Audio Transcription Quickstart](#live-audio-transcription-quickstart)
 - [Examples](#examples)
+- [Logging](#logging)
+- [Backwards Compatibility](#backwards-compatibility)
 - [Development and Contributing](#development-and-contributing)
 - [Getting Help](#getting-help)
 
 # Documentation
 
 You can learn more about the Deepgram API at [developers.deepgram.com](https://developers.deepgram.com/docs).
 
@@ -199,14 +223,35 @@
     - Members - [examples/manage/members](https://github.com/deepgram/deepgram-python-sdk/blob/main/examples/manage/members/main.py)
     - Projects - [examples/manage/projects](https://github.com/deepgram/deepgram-python-sdk/blob/main/examples/manage/projects/main.py)
     - Scopes - [examples/manage/scopes](https://github.com/deepgram/deepgram-python-sdk/blob/main/examples/manage/scopes/main.py)
     - Usage - [examples/manage/usage](https://github.com/deepgram/deepgram-python-sdk/blob/main/examples/manage/usage/main.py)
 
 To run each example set the `DEEPGRAM_API_KEY` as an environment variable, then `cd` into each example folder and execute the example: `go run main.py`.
 
+
+# Logging
+
+This SDK provides logging as a means to troubleshoot and debug issues encountered. By default, this SDK will enable `Information` level messages and higher (ie `Warning`, `Error`, etc) when you initialize the library as follows:
+
+```python
+deepgram: DeepgramClient = DeepgramClient()
+```
+
+To increase the logging output/verbosity for debug or troubleshooting purposes, you can set the `DEBUG` level but using this code:
+
+```python
+config: DeepgramClientOptions = DeepgramClientOptions(
+    verbose=logging.DEBUG,
+)
+deepgram: DeepgramClient = DeepgramClient("", config)
+```
+# Backwards Compatibility
+
+Older SDK versions will receive Priority 1 (P1) bug support only. Security issues, both in our code and dependencies, are promptly addressed. Significant bugs without clear workarounds are also given priority attention.
+
 # Development and Contributing
 
 Interested in contributing? We ❤️ pull requests!
 
 To make sure our community is safe for all, be sure to review and agree to our
 [Code of Conduct](https://github.com/deepgram/deepgram-python-sdk/blob/main/.github/CODE_OF_CONDUCT.md). Then see the
 [Contribution](https://github.com/deepgram/deepgram-python-sdk/blob/main/.github/CONTRIBUTING.md) guidelines for more information.
```

### Comparing `deepgram-sdk-3.2.5/deepgram/__init__.py` & `deepgram_sdk-3.2.6/deepgram/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2023-2024 Deepgram SDK contributors. All Rights Reserved.
 # Use of this source code is governed by a MIT license that can be found in the LICENSE file.
 # SPDX-License-Identifier: MIT
 
 # version
-__version__ = "v3.2.5"
+__version__ = "v3.2.6"
 
 # entry point for the deepgram python sdk
 from .client import Deepgram, DeepgramClient
 from .options import DeepgramClientOptions, ClientOptionsFromEnv
 import logging, verboselogs
 
 # listen client
```

### Comparing `deepgram-sdk-3.2.5/deepgram/audio/microphone/errors.py` & `deepgram_sdk-3.2.6/deepgram/audio/microphone/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/audio/microphone/microphone.py` & `deepgram_sdk-3.2.6/deepgram/audio/microphone/microphone.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/client.py` & `deepgram_sdk-3.2.6/deepgram/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/__init__.py` & `deepgram_sdk-3.2.6/deepgram/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/abstract_async_client.py` & `deepgram_sdk-3.2.6/deepgram/clients/abstract_async_client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/abstract_sync_client.py` & `deepgram_sdk-3.2.6/deepgram/clients/abstract_sync_client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/analyze/__init__.py` & `deepgram_sdk-3.2.6/deepgram/clients/analyze/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/analyze/client.py` & `deepgram_sdk-3.2.6/deepgram/clients/analyze/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/analyze/errors.py` & `deepgram_sdk-3.2.6/deepgram/clients/analyze/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/analyze/v1/__init__.py` & `deepgram_sdk-3.2.6/deepgram/clients/analyze/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/analyze/v1/async_client.py` & `deepgram_sdk-3.2.6/deepgram/clients/analyze/v1/async_client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/analyze/v1/client.py` & `deepgram_sdk-3.2.6/deepgram/clients/analyze/v1/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/analyze/v1/helpers.py` & `deepgram_sdk-3.2.6/deepgram/clients/analyze/v1/helpers.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/analyze/v1/options.py` & `deepgram_sdk-3.2.6/deepgram/clients/analyze/v1/options.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/analyze/v1/response.py` & `deepgram_sdk-3.2.6/deepgram/clients/analyze/v1/response.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/errors.py` & `deepgram_sdk-3.2.6/deepgram/clients/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/helpers.py` & `deepgram_sdk-3.2.6/deepgram/clients/helpers.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/listen.py` & `deepgram_sdk-3.2.6/deepgram/clients/listen.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/live/__init__.py` & `deepgram_sdk-3.2.6/deepgram/clients/live/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/live/client.py` & `deepgram_sdk-3.2.6/deepgram/clients/live/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/live/enums.py` & `deepgram_sdk-3.2.6/deepgram/clients/live/enums.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/live/errors.py` & `deepgram_sdk-3.2.6/deepgram/clients/live/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/live/helpers.py` & `deepgram_sdk-3.2.6/deepgram/clients/live/helpers.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/live/v1/__init__.py` & `deepgram_sdk-3.2.6/deepgram/clients/live/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/live/v1/async_client.py` & `deepgram_sdk-3.2.6/deepgram/clients/live/v1/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         self.logger = logging.getLogger(__name__)
         self.logger.addHandler(logging.StreamHandler())
         self.logger.setLevel(config.verbose)
 
         self.config = config
         self.endpoint = "v1/listen"
         self._socket = None
-        self._exit_event = None
+        self._exit_event = asyncio.Event()
         self._event_handlers = {event: [] for event in LiveTranscriptionEvents}
         self.websocket_url = convert_to_websocket_url(self.config.url, self.endpoint)
 
     # starts the WebSocket connection for live transcription
     async def start(
         self,
         options: Optional[Union[LiveOptions, Dict]] = None,
@@ -119,15 +119,15 @@
 
         try:
             self._socket = await websockets.connect(
                 url_with_params,
                 extra_headers=combined_headers,
                 ping_interval=PING_INTERVAL,
             )
-            self._exit_event = asyncio.Event()
+            self._exit_event.clear()
 
             # listen thread
             self._listen_thread = asyncio.create_task(self._listening())
 
             # keepalive thread
             if self.config.options.get("keepalive") == "true":
                 self.logger.notice("keepalive is enabled")
```

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/live/v1/client.py` & `deepgram_sdk-3.2.6/deepgram/clients/live/v1/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,16 @@
         self.logger = logging.getLogger(__name__)
         self.logger.addHandler(logging.StreamHandler())
         self.logger.setLevel(config.verbose)
 
         self.config = config
         self.endpoint = "v1/listen"
         self._socket = None
-        self._exit_event = None
+        self._exit_event = threading.Event()
+        self._lock_send = threading.Lock()
         self._event_handlers = {event: [] for event in LiveTranscriptionEvents}
         self.websocket_url = convert_to_websocket_url(self.config.url, self.endpoint)
 
     # starts the WebSocket connection for live transcription
     def start(
         self,
         options: Optional[Union[LiveOptions, Dict]] = None,
@@ -116,16 +117,15 @@
             combined_headers.update(self.headers)
             self.logger.info("new headers: %s", combined_headers)
         self.logger.debug("combined_headers: %s", combined_headers)
 
         url_with_params = append_query_params(self.websocket_url, combined_options)
         try:
             self._socket = connect(url_with_params, additional_headers=combined_headers)
-            self._exit_event = threading.Event()
-            self._lock_send = threading.Lock()
+            self._exit_event.clear()
 
             # listening thread
             self._listen_thread = threading.Thread(target=self._listening)
             self._listen_thread.start()
 
             # keepalive thread
             if self.config.options.get("keepalive") == "true":
```

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/live/v1/options.py` & `deepgram_sdk-3.2.6/deepgram/clients/live/v1/options.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/live/v1/response.py` & `deepgram_sdk-3.2.6/deepgram/clients/live/v1/response.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/manage/__init__.py` & `deepgram_sdk-3.2.6/deepgram/clients/manage/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/manage/client.py` & `deepgram_sdk-3.2.6/deepgram/clients/manage/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/manage/v1/__init__.py` & `deepgram_sdk-3.2.6/deepgram/clients/manage/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/manage/v1/async_client.py` & `deepgram_sdk-3.2.6/deepgram/clients/manage/v1/async_client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/manage/v1/client.py` & `deepgram_sdk-3.2.6/deepgram/clients/manage/v1/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/manage/v1/options.py` & `deepgram_sdk-3.2.6/deepgram/clients/manage/v1/options.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/manage/v1/response.py` & `deepgram_sdk-3.2.6/deepgram/clients/manage/v1/response.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/onprem/client.py` & `deepgram_sdk-3.2.6/deepgram/clients/onprem/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/onprem/v1/async_client.py` & `deepgram_sdk-3.2.6/deepgram/clients/onprem/v1/async_client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/onprem/v1/client.py` & `deepgram_sdk-3.2.6/deepgram/clients/onprem/v1/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/prerecorded/__init__.py` & `deepgram_sdk-3.2.6/deepgram/clients/prerecorded/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/prerecorded/client.py` & `deepgram_sdk-3.2.6/deepgram/clients/prerecorded/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/prerecorded/errors.py` & `deepgram_sdk-3.2.6/deepgram/clients/prerecorded/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/prerecorded/v1/__init__.py` & `deepgram_sdk-3.2.6/deepgram/clients/prerecorded/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/prerecorded/v1/async_client.py` & `deepgram_sdk-3.2.6/deepgram/clients/prerecorded/v1/async_client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/prerecorded/v1/client.py` & `deepgram_sdk-3.2.6/deepgram/clients/prerecorded/v1/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/prerecorded/v1/helpers.py` & `deepgram_sdk-3.2.6/deepgram/clients/prerecorded/v1/helpers.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/prerecorded/v1/options.py` & `deepgram_sdk-3.2.6/deepgram/clients/prerecorded/v1/options.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/prerecorded/v1/response.py` & `deepgram_sdk-3.2.6/deepgram/clients/prerecorded/v1/response.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/read.py` & `deepgram_sdk-3.2.6/deepgram/clients/read.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/speak/client.py` & `deepgram_sdk-3.2.6/deepgram/clients/speak/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/speak/errors.py` & `deepgram_sdk-3.2.6/deepgram/clients/speak/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/speak/v1/async_client.py` & `deepgram_sdk-3.2.6/deepgram/clients/speak/v1/async_client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/speak/v1/client.py` & `deepgram_sdk-3.2.6/deepgram/clients/speak/v1/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/speak/v1/options.py` & `deepgram_sdk-3.2.6/deepgram/clients/speak/v1/options.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/clients/speak/v1/response.py` & `deepgram_sdk-3.2.6/deepgram/clients/speak/v1/response.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/errors.py` & `deepgram_sdk-3.2.6/deepgram/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram/options.py` & `deepgram_sdk-3.2.6/deepgram/options.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/deepgram_sdk.egg-info/PKG-INFO` & `deepgram_sdk-3.2.6/deepgram_sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepgram-sdk
-Version: 3.2.5
+Version: 3.2.6
 Summary: The official Python SDK for the Deepgram automated speech recognition platform.
 Home-page: https://github.com/deepgram/deepgram-python-sdk
 Author: Deepgram
 Author-email: devrel@deepgram.com
 License: MIT
 Keywords: deepgram,deepgram speech-to-text
 Classifier: Intended Audience :: Developers
@@ -32,14 +32,16 @@
 - [Getting an API Key](#getting-an-api-key)
 - [Requirements](#requirements)
 - [Installation](#installation)
 - [Quickstarts](#quickstarts)
   - [PreRecorded Audio Transcription Quickstart](#prerecorded-audio-transcription-quickstart)
   - [Live Audio Transcription Quickstart](#live-audio-transcription-quickstart)
 - [Examples](#examples)
+- [Logging](#logging)
+- [Backwards Compatibility](#backwards-compatibility)
 - [Development and Contributing](#development-and-contributing)
 - [Getting Help](#getting-help)
 
 # Documentation
 
 You can learn more about the Deepgram API at [developers.deepgram.com](https://developers.deepgram.com/docs).
 
@@ -221,14 +223,35 @@
     - Members - [examples/manage/members](https://github.com/deepgram/deepgram-python-sdk/blob/main/examples/manage/members/main.py)
     - Projects - [examples/manage/projects](https://github.com/deepgram/deepgram-python-sdk/blob/main/examples/manage/projects/main.py)
     - Scopes - [examples/manage/scopes](https://github.com/deepgram/deepgram-python-sdk/blob/main/examples/manage/scopes/main.py)
     - Usage - [examples/manage/usage](https://github.com/deepgram/deepgram-python-sdk/blob/main/examples/manage/usage/main.py)
 
 To run each example set the `DEEPGRAM_API_KEY` as an environment variable, then `cd` into each example folder and execute the example: `go run main.py`.
 
+
+# Logging
+
+This SDK provides logging as a means to troubleshoot and debug issues encountered. By default, this SDK will enable `Information` level messages and higher (ie `Warning`, `Error`, etc) when you initialize the library as follows:
+
+```python
+deepgram: DeepgramClient = DeepgramClient()
+```
+
+To increase the logging output/verbosity for debug or troubleshooting purposes, you can set the `DEBUG` level but using this code:
+
+```python
+config: DeepgramClientOptions = DeepgramClientOptions(
+    verbose=logging.DEBUG,
+)
+deepgram: DeepgramClient = DeepgramClient("", config)
+```
+# Backwards Compatibility
+
+Older SDK versions will receive Priority 1 (P1) bug support only. Security issues, both in our code and dependencies, are promptly addressed. Significant bugs without clear workarounds are also given priority attention.
+
 # Development and Contributing
 
 Interested in contributing? We ❤️ pull requests!
 
 To make sure our community is safe for all, be sure to review and agree to our
 [Code of Conduct](https://github.com/deepgram/deepgram-python-sdk/blob/main/.github/CODE_OF_CONDUCT.md). Then see the
 [Contribution](https://github.com/deepgram/deepgram-python-sdk/blob/main/.github/CONTRIBUTING.md) guidelines for more information.
```

### Comparing `deepgram-sdk-3.2.5/deepgram_sdk.egg-info/SOURCES.txt` & `deepgram_sdk-3.2.6/deepgram_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/pyproject.toml` & `deepgram_sdk-3.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.5/setup.py` & `deepgram_sdk-3.2.6/setup.py`

 * *Files identical despite different names*

