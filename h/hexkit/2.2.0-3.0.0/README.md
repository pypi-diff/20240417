# Comparing `tmp/hexkit-2.2.0.tar.gz` & `tmp/hexkit-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexkit-2.2.0.tar", last modified: Wed Apr 10 07:24:08 2024, max compression
+gzip compressed data, was "hexkit-3.0.0.tar", last modified: Wed Apr 17 13:49:18 2024, max compression
```

## Comparing `hexkit-2.2.0.tar` & `hexkit-3.0.0.tar`

### file list

```diff
@@ -1,57 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:24:08.499642 hexkit-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-04-10 07:24:04.000000 hexkit-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-10 07:24:04.000000 hexkit-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-04-10 07:24:08.499642 hexkit-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-04-10 07:24:04.000000 hexkit-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-10 07:24:04.000000 hexkit-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 07:24:08.499642 hexkit-2.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:24:08.491642 hexkit-2.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:24:08.491642 hexkit-2.2.0/src/hexkit/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:24:08.495642 hexkit-2.2.0/src/hexkit/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16935 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/protocols/dao.py
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/protocols/dao_outbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/protocols/eventpub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/protocols/eventsub.py
--rw-r--r--   0 runner    (1001) docker     (127)    24781 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/protocols/objstorage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:24:08.495642 hexkit-2.2.0/src/hexkit/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:24:08.495642 hexkit-2.2.0/src/hexkit/providers/akafka/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/providers/akafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17021 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/providers/akafka/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/providers/akafka/testcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    19785 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/providers/akafka/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:24:08.495642 hexkit-2.2.0/src/hexkit/providers/mongodb/
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/providers/mongodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18352 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/providers/mongodb/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/providers/mongodb/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:24:08.495642 hexkit-2.2.0/src/hexkit/providers/mongokafka/
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/providers/mongokafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15825 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/providers/mongokafka/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:24:08.495642 hexkit-2.2.0/src/hexkit/providers/s3/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/providers/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32747 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/providers/s3/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:24:08.499642 hexkit-2.2.0/src/hexkit/providers/s3/test_files/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/providers/s3/test_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/providers/s3/test_files/test_file1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/providers/s3/test_files/test_file2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/providers/s3/test_files/test_file3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/providers/s3/test_files/test_file4.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15133 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/providers/s3/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:24:08.499642 hexkit-2.2.0/src/hexkit/providers/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/providers/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/providers/testing/eventpub.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-10 07:24:04.000000 hexkit-2.2.0/src/hexkit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:24:08.499642 hexkit-2.2.0/src/hexkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-04-10 07:24:08.000000 hexkit-2.2.0/src/hexkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-10 07:24:08.000000 hexkit-2.2.0/src/hexkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 07:24:08.000000 hexkit-2.2.0/src/hexkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-10 07:24:08.000000 hexkit-2.2.0/src/hexkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 07:24:08.000000 hexkit-2.2.0/src/hexkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:49:18.025608 hexkit-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-04-17 13:49:12.000000 hexkit-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-17 13:49:12.000000 hexkit-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-04-17 13:49:18.025608 hexkit-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-04-17 13:49:12.000000 hexkit-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-17 13:49:12.000000 hexkit-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 13:49:18.025608 hexkit-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:49:18.013608 hexkit-3.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:49:18.017608 hexkit-3.0.0/src/hexkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:49:18.021608 hexkit-3.0.0/src/hexkit/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16935 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/protocols/dao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/protocols/daopub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/protocols/daosub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/protocols/eventpub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/protocols/eventsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24781 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/protocols/objstorage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:49:18.021608 hexkit-3.0.0/src/hexkit/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:49:18.021608 hexkit-3.0.0/src/hexkit/providers/akafka/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/akafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/akafka/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:49:18.021608 hexkit-3.0.0/src/hexkit/providers/akafka/provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/akafka/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/akafka/provider/daosub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/akafka/provider/eventpub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/akafka/provider/eventsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/akafka/provider/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/akafka/testcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19083 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/akafka/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:49:18.021608 hexkit-3.0.0/src/hexkit/providers/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/mongodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18352 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/mongodb/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/mongodb/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:49:18.021608 hexkit-3.0.0/src/hexkit/providers/mongokafka/
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/mongokafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16185 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/mongokafka/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:49:18.021608 hexkit-3.0.0/src/hexkit/providers/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33195 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/s3/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:49:18.025608 hexkit-3.0.0/src/hexkit/providers/s3/test_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/s3/test_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/s3/test_files/test_file1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/s3/test_files/test_file2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/s3/test_files/test_file3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/s3/test_files/test_file4.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15737 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/s3/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:49:18.025608 hexkit-3.0.0/src/hexkit/providers/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/testing/eventpub.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:49:18.025608 hexkit-3.0.0/src/hexkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-04-17 13:49:18.000000 hexkit-3.0.0/src/hexkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-17 13:49:18.000000 hexkit-3.0.0/src/hexkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 13:49:18.000000 hexkit-3.0.0/src/hexkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-17 13:49:18.000000 hexkit-3.0.0/src/hexkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 13:49:18.000000 hexkit-3.0.0/src/hexkit.egg-info/top_level.txt
```

### Comparing `hexkit-2.2.0/LICENSE` & `hexkit-3.0.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+   Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
    for the German Human Genome-Phenome Archive (GHGA)
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `hexkit-2.2.0/PKG-INFO` & `hexkit-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: hexkit
-Version: 2.2.0
+Version: 3.0.0
 Summary: A Toolkit for Building Microservices using the Hexagonal Architecture
 Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ghga-de/hexkit
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic<3,>=2
 Requires-Dist: pydantic_settings<3,>=2
 Requires-Dist: PyYAML<7,>=6.0
 Provides-Extra: akafka
-Requires-Dist: aiokafka~=0.8.0; extra == "akafka"
-Requires-Dist: jsonschema<5,>=4.17.3; extra == "akafka"
+Requires-Dist: aiokafka~=0.10.0; extra == "akafka"
+Requires-Dist: jsonschema<5,>=4.21; extra == "akafka"
 Provides-Extra: s3
 Requires-Dist: boto3<2,>=1.26.50; extra == "s3"
 Requires-Dist: botocore<2,>=1.29.50; extra == "s3"
 Provides-Extra: mongodb
 Requires-Dist: motor<4,>=3.1.1; extra == "mongodb"
 Provides-Extra: test-akafka
 Requires-Dist: hexkit[akafka]; extra == "test-akafka"
```

### Comparing `hexkit-2.2.0/README.md` & `hexkit-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `hexkit-2.2.0/pyproject.toml` & `hexkit-3.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [build-system]
 requires = [
-    "setuptools>=67.7.2",
+    "setuptools>=69",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 readme = "README.md"
 authors = [
     { name = "German Human Genome Phenome Archive (GHGA)", email = "contact@ghga.de" },
@@ -12,35 +12,36 @@
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 1 - Planning",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Software Development :: Libraries",
     "Intended Audience :: Developers",
 ]
 name = "hexkit"
-version = "2.2.0"
+version = "3.0.0"
 description = "A Toolkit for Building Microservices using the Hexagonal Architecture"
 dependencies = [
     "pydantic >=2, <3",
     "pydantic_settings >=2, <3",
     "PyYAML >=6.0, <7",
 ]
 
 [project.license]
 text = "Apache 2.0"
 
 [project.optional-dependencies]
 akafka = [
-    "aiokafka~=0.8.0",
-    "jsonschema >=4.17.3, <5",
+    "aiokafka~=0.10.0",
+    "jsonschema >=4.21, <5",
 ]
 s3 = [
     "boto3 >=1.26.50, <2",
     "botocore >=1.29.50, <2",
 ]
 mongodb = [
     "motor >=3.1.1, <4",
@@ -92,16 +93,17 @@
 [tool.ruff.lint]
 fixable = [
     "UP",
     "I",
     "D",
 ]
 ignore = [
-    "E",
-    "W",
+    "E111",
+    "E114",
+    "E116",
     "PLW",
     "RUF001",
     "RUF010",
     "RUF012",
     "N818",
     "B008",
     "PLR2004",
@@ -166,19 +168,19 @@
 ]
 warn_redundant_casts = true
 warn_unused_ignores = true
 check_untyped_defs = true
 no_site_packages = false
 
 [tool.pytest.ini_options]
-minversion = "7.1"
+minversion = "8.0"
 asyncio_mode = "strict"
 
 [tool.coverage.paths]
 source = [
     "src",
     "/workspace/src",
     "**/lib/python*/site-packages",
 ]
 
 [tool.tox]
-legacy_tox_ini = "    [tox]\n    min_version = 4.0\n    env_list =\n        py39\n        py311\n\n    [testenv]\n    pass_env=\n        TC_HOST\n        DOCKER_HOST\n    deps =\n        --no-deps -r ./lock/requirements-dev.txt\n    commands = pytest ./tests {posargs}\n"
+legacy_tox_ini = "    [tox]\n    env_list = py3{9,12}\n\n    [gh-actions]\n    python =\n        3.9: py39\n        3.10: py310\n        3.11: py311\n        3.12: py312\n\n    [testenv]\n    pass_env =\n        TC_HOST\n        DOCKER_HOST\n    deps =\n        --no-deps -r ./lock/requirements-dev.txt\n    commands = pytest {posargs}\n"
```

### Comparing `hexkit-2.2.0/src/hexkit/__init__.py` & `hexkit-3.0.0/src/hexkit/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `hexkit-2.2.0/src/hexkit/__main__.py` & `hexkit-3.0.0/src/hexkit/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `hexkit-2.2.0/src/hexkit/base.py` & `hexkit-3.0.0/src/hexkit/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `hexkit-2.2.0/src/hexkit/config.py` & `hexkit-3.0.0/src/hexkit/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `hexkit-2.2.0/src/hexkit/correlation.py` & `hexkit-3.0.0/src/hexkit/correlation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `hexkit-2.2.0/src/hexkit/custom_types.py` & `hexkit-3.0.0/src/hexkit/custom_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `hexkit-2.2.0/src/hexkit/log.py` & `hexkit-3.0.0/src/hexkit/log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `hexkit-2.2.0/src/hexkit/protocols/__init__.py` & `hexkit-3.0.0/src/hexkit/providers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-"""Sub-package containing protocols."""
+"""Sub-package containing providers."""
```

### Comparing `hexkit-2.2.0/src/hexkit/protocols/dao.py` & `hexkit-3.0.0/src/hexkit/protocols/dao.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `hexkit-2.2.0/src/hexkit/protocols/dao_outbox.py` & `hexkit-3.0.0/src/hexkit/protocols/daopub.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -30,15 +30,15 @@
 from hexkit.protocols.dao import (
     DaoFactoryBase,
     DaoNaturalId,
     Dto,
 )
 
 
-class DaoOutbox(DaoNaturalId[Dto], typing.Protocol[Dto]):
+class DaoPublisher(DaoNaturalId[Dto], typing.Protocol[Dto]):
     """A Data Access Object (DAO) that automatically publishes changes according to the
     outbox pattern.
     """
 
     async def publish_pending(self) -> None:
         """Publishes all non-published changes."""
         ...
@@ -46,30 +46,30 @@
     async def republish(self) -> None:
         """Republishes the state of all resources independent of whether they have
         already been published or not.
         """
         ...
 
 
-class DaoOutboxFactoryProtocol(DaoFactoryBase, ABC):
+class DaoPublisherFactoryProtocol(DaoFactoryBase, ABC):
     """A protocol describing a factory to produce Data Access Objects (DAO) objects
     which automatically publish changes according to the outbox pattern.
     """
 
     async def get_dao(
         self,
         *,
         name: str,
         dto_model: type[Dto],
         id_field: str,
         fields_to_index: Optional[Collection[str]] = None,
         dto_to_event: Callable[[Dto], JsonObject],
         event_topic: str,
         autopublish: bool = True,
-    ) -> DaoOutbox[Dto]:
+    ) -> DaoPublisher[Dto]:
         """Constructs an Outbox DAO for interacting with resources in a database.
 
         Args:
             name:
                 The name of the resource type (roughly equivalent to the name of a
                 database table or collection).
             dto_model:
@@ -84,15 +84,15 @@
                 A function that takes a DTO and returns the payload for an event.
             event_topic:
                 The topic to which events should be published.
             autopublish:
                 Whether to automatically publish changes. Defaults to True.
 
         Returns:
-            A DAO of type DaoOutbox, which requires ID specification upon resource
+            A DAO of type DaoPublisher, which requires ID specification upon resource
             creation.
 
         Raises:
             self.IdFieldNotFoundError:
                 Raised when the dto_model did not contain the expected id_field.
         """
         self._validate(
@@ -119,12 +119,12 @@
         name: str,
         dto_model: type[Dto],
         id_field: str,
         fields_to_index: Optional[Collection[str]],
         dto_to_event: Callable[[Dto], JsonObject],
         event_topic: str,
         autopublish: bool,
-    ) -> DaoOutbox[Dto]:
+    ) -> DaoPublisher[Dto]:
         """*To be implemented by the provider. Input validation is done outside of this
         method.*
         """
         ...
```

### Comparing `hexkit-2.2.0/src/hexkit/protocols/eventpub.py` & `hexkit-3.0.0/src/hexkit/protocols/eventpub.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `hexkit-2.2.0/src/hexkit/protocols/eventsub.py` & `hexkit-3.0.0/src/hexkit/protocols/eventsub.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -41,31 +41,51 @@
         Raised if the payload of a received event was not formatted as expected given
         the type.
         """
 
     topics_of_interest: list[Ascii]
     types_of_interest: list[Ascii]
 
-    async def consume(self, *, payload: JsonObject, type_: Ascii, topic: Ascii) -> None:
+    async def consume(
+        self,
+        *,
+        payload: JsonObject,
+        type_: Ascii,
+        topic: Ascii,
+        key: Ascii,
+    ) -> None:
         """Receive an event of interest and process it according to its type.
 
         Args:
-            payload (JsonObject): The data/payload to send with the event.
-            type_ (str): The type of the event.
-            topic (str): Name of the topic the event was published to.
+            payload: The data/payload to send with the event.
+            type_: The type of the event.
+            topic: Name of the topic the event was published to.
+            key: A key used for routing the event.
         """
         check_ascii(type_, topic)
-        await self._consume_validated(payload=payload, type_=type_, topic=topic)
+
+        if key:
+            check_ascii(key)
+
+        await self._consume_validated(
+            payload=payload, type_=type_, topic=topic, key=key
+        )
 
     @abstractmethod
     async def _consume_validated(
-        self, *, payload: JsonObject, type_: Ascii, topic: Ascii
+        self,
+        *,
+        payload: JsonObject,
+        type_: Ascii,
+        topic: Ascii,
+        key: Ascii,
     ) -> None:
         """
-        Receive and process an event with already validated topic and type.
+        Receive and process an event with already validated topic, type, and key.
 
         Args:
-            payload (JsonObject): The data/payload to send with the event.
-            type_ (str): The type of the event.
-            topic (str): Name of the topic the event was published to.
+            payload: The data/payload to send with the event.
+            type_: The type of the event.
+            topic: Name of the topic the event was published to.
+            key: A key used for routing the event.
         """
         ...
```

### Comparing `hexkit-2.2.0/src/hexkit/protocols/objstorage.py` & `hexkit-3.0.0/src/hexkit/protocols/objstorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `hexkit-2.2.0/src/hexkit/providers/__init__.py` & `hexkit-3.0.0/src/hexkit/providers/s3/test_files/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-#
-
-"""Sub-package containing providers."""
```

### Comparing `hexkit-2.2.0/src/hexkit/providers/akafka/__init__.py` & `hexkit-3.0.0/src/hexkit/providers/akafka/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -15,14 +15,20 @@
 #
 
 """Apache Kafka-specific event publisher and subscriber provider.
 They correspond to the `EventPublisherProtocol` and `EventSubscriberProtocol`,
 respectively.
 """
 
+from .config import KafkaConfig
 from .provider import (
-    KafkaConfig,
     KafkaEventPublisher,
     KafkaEventSubscriber,
+    KafkaOutboxSubscriber,
 )
 
-__all__ = ["KafkaEventPublisher", "KafkaEventSubscriber", "KafkaConfig"]
+__all__ = [
+    "KafkaEventPublisher",
+    "KafkaEventSubscriber",
+    "KafkaConfig",
+    "KafkaOutboxSubscriber",
+]
```

### Comparing `hexkit-2.2.0/src/hexkit/providers/akafka/testcontainer.py` & `hexkit-3.0.0/src/hexkit/providers/akafka/testcontainer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -15,26 +15,23 @@
 #
 
 """Improved Kafka test containers."""
 
 import tarfile
 import time
 from io import BytesIO
-from ssl import SSLError
 from textwrap import dedent
 from typing import Literal, Optional
 
-from kafka import KafkaConsumer
-from kafka.errors import KafkaError, NoBrokersAvailable, UnrecognizedBrokerVersion
 from testcontainers.core.container import DockerContainer
-from testcontainers.core.waiting_utils import wait_container_is_ready
+from testcontainers.core.waiting_utils import wait_for_logs
 
 __all__ = ["KafkaSSLContainer"]
 
-DEFAULT_IMAGE = "confluentinc/cp-kafka:7.5.1"
+DEFAULT_IMAGE = "confluentinc/cp-kafka:7.6.0"
 
 DEFAULT_PORT = 9093  # default port for the Kafka container
 BROKER_PORT = 9092  # auxiliary port for inter broker listener
 
 
 class KafkaSSLContainer(DockerContainer):
     """Kafka container that supports SSL (or actually TLS)."""
@@ -111,41 +108,24 @@
 
     def get_bootstrap_server(self) -> str:
         """Get the Kafka bootstrap server."""
         host = self.get_container_host_ip()
         port = self.get_exposed_port(self.port)
         return f"{host}:{port}"
 
-    def start(self) -> "KafkaSSLContainer":
+    def start(self, timeout: Optional[float] = 30) -> "KafkaSSLContainer":
         """Start the Docker container."""
         script = self.TC_START_SCRIPT
         command = f'sh -c "while [ ! -f {script} ]; do sleep 0.1; done; sh {script}"'
         self.with_command(command)
         super().start()
         self.tc_start()
-        self._connect()
+        wait_for_logs(self, r".*\[KafkaServer id=\d+\] started.*", timeout=timeout)
         return self
 
-    @wait_container_is_ready(
-        UnrecognizedBrokerVersion, NoBrokersAvailable, KafkaError, ValueError
-    )  # pyright: ignore
-    def _connect(self) -> None:
-        bootstrap_server = self.get_bootstrap_server()
-        try:
-            consumer = KafkaConsumer(
-                group_id="test",
-                bootstrap_servers=[bootstrap_server],
-                security_protocol=self.protocol,
-            )
-        except SSLError:
-            pass  # count this as connected
-        else:
-            if not consumer.bootstrap_connected():
-                raise KafkaError("Unable to connect with Kafka container!")
-
     def tc_start(self) -> None:
         """Start the test container."""
         protocol = self.protocol
         host = self.get_container_host_ip()
         port = self.get_exposed_port(self.port)
         listeners = f"{protocol}://{host}:{port},BROKER://127.0.0.1:{self.broker_port}"
         script = f"""
```

### Comparing `hexkit-2.2.0/src/hexkit/providers/akafka/testutils.py` & `hexkit-3.0.0/src/hexkit/providers/akafka/testutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -16,31 +16,29 @@
 
 """Utilities for testing code that uses Kafka-based provider.
 
 Please note, only use for testing purposes.
 """
 
 import json
-import warnings
 from collections.abc import AsyncGenerator, Sequence
 from contextlib import asynccontextmanager
 from dataclasses import dataclass
 from functools import partial
 from typing import Callable, Optional, Union
 
 import pytest_asyncio
 from aiokafka import AIOKafkaConsumer, TopicPartition
-from kafka import KafkaAdminClient
-from kafka.errors import KafkaError
+from aiokafka.admin import AIOKafkaAdminClient
 from testcontainers.kafka import KafkaContainer
 
 from hexkit.custom_types import Ascii, JsonObject, PytestScope
+from hexkit.providers.akafka import KafkaConfig
 from hexkit.providers.akafka.provider import (
     ConsumerEvent,
-    KafkaConfig,
     KafkaEventPublisher,
     get_header_value,
     headers_as_dict,
 )
 from hexkit.providers.akafka.testcontainer import DEFAULT_IMAGE as KAFKA_IMAGE
 
 
@@ -404,79 +402,59 @@
         echo_command = f"echo '{json_data}' > {file_name}"
         deletion_command = (
             "kafka-delete-records --bootstrap-server localhost:9092 "
             + f"--offset-json-file {file_name}"
         )
         return f"{echo_command} && {deletion_command}"
 
-    def clear_topics(
+    async def _get_topic_description(
         self,
-        *,
-        topics: Optional[Union[str, list[str]]] = None,
-    ):
-        """
-        Clear messages from given topic(s).
+        topics: Optional[Union[list[str], str]] = None,
+        exclude_internal: bool = True,
+    ) -> JsonObject:
+        """Get a decription of the given topic(s).
 
-        When no topics are specified, all existing topics will be cleared.
+        If no topics are specified, all topics will be covered, except internal topics
+        unless otherwise specified.
         """
-        admin_client = KafkaAdminClient(bootstrap_servers=self.kafka_servers)
+        admin_client = AIOKafkaAdminClient(bootstrap_servers=self.kafka_servers)
+        await admin_client.start()
         try:
-            all_topics = admin_client.list_topics()
-
-            # If not clearing specific topics, delete all aside from the internal
-            # __consumer_offsets topic
             if topics is None:
-                topics = [
-                    topic for topic in all_topics if topic != "__consumer_offsets"
-                ]
+                # if topics is None, the admin client gets all topics
+                if exclude_internal:
+                    topics = [
+                        topic
+                        for topic in await admin_client.list_topics()
+                        if not topic.startswith("__")
+                    ]
             elif isinstance(topics, str):
                 topics = [topics]
+            return await admin_client.describe_topics(topics)
+        finally:
+            await admin_client.close()
 
-            # Get partition info for the topics requested to be cleared
-            partition_info: JsonObject = admin_client.describe_topics(topics)
-
-            # Get the command and then run it in a shell
-            deletion_config = self._build_record_deletion_config(partition_info)
-            command = self._build_record_deletion_command(deletion_config)
+    async def clear_topics(
+        self,
+        topics: Optional[Union[str, list[str]]] = None,
+        exclude_internal: bool = True,
+    ):
+        """Clear messages from given topic(s).
 
-            self._cmd_exec_func(command, True)
+        If no topics are specified, all topics will be cleared, except internal topics
+        unless otherwise specified.
+        """
+        # Get the description of the topics to be deleted
+        partition_info = await self._get_topic_description(topics, exclude_internal)
 
-        finally:
-            # Close the client
-            admin_client.close()
+        # Build the command line and then run it in a shell
+        deletion_config = self._build_record_deletion_config(partition_info)
+        command = self._build_record_deletion_command(deletion_config)
 
-    def delete_topics(self, topics: Optional[Union[str, list[str]]] = None):
-        """
-        Delete given topic(s) from Kafka broker. When no topics are specified,
-        all existing topics will be deleted.
-        """
-        warnings.warn(
-            "delete_topics() is deprecated and will be removed in future versions. "
-            + f"Use {self.clear_topics.__name__}() instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        admin_client = KafkaAdminClient(bootstrap_servers=self.kafka_servers)
-        all_topics = admin_client.list_topics()
-        if topics is None:
-            topics = all_topics
-        elif isinstance(topics, str):
-            topics = [topics]
-        try:
-            existing_topics = set(all_topics)
-            for topic in topics:
-                if topic in existing_topics:
-                    try:
-                        admin_client.delete_topics([topic])
-                    except KafkaError as error:
-                        raise RuntimeError(
-                            f"Could not delete topic {topic} from Kafka"
-                        ) from error
-        finally:
-            admin_client.close()
+        self._cmd_exec_func(command, True)
 
     @asynccontextmanager
     async def expect_events(
         self, events: Sequence[ExpectedEvent], *, in_topic: Ascii
     ) -> AsyncGenerator[EventRecorder, None]:
         """Can be used in an async with block to record events in the specified topic
         (on __aenter__) and check that they match the specified sequence of expected
```

### Comparing `hexkit-2.2.0/src/hexkit/providers/mongodb/__init__.py` & `hexkit-3.0.0/src/hexkit/providers/mongodb/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `hexkit-2.2.0/src/hexkit/providers/mongodb/provider.py` & `hexkit-3.0.0/src/hexkit/providers/mongodb/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `hexkit-2.2.0/src/hexkit/providers/mongodb/testutils.py` & `hexkit-3.0.0/src/hexkit/providers/mongodb/testutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `hexkit-2.2.0/src/hexkit/providers/mongokafka/__init__.py` & `hexkit-3.0.0/src/hexkit/providers/mongokafka/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -10,10 +10,10 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-"""An implementation of the DaoOutboxFactoryProtocol based on MongoDB and Apache Kafka."""
+"""An implementation of the DaoPublisherFactoryProtocol based on MongoDB and Apache Kafka."""
 
-from .provider import MongoKafkaConfig, MongoKafkaDaoOutboxFactory  # noqa: F401
+from .provider import MongoKafkaConfig, MongoKafkaDaoPublisherFactory  # noqa: F401
```

### Comparing `hexkit-2.2.0/src/hexkit/providers/mongokafka/provider.py` & `hexkit-3.0.0/src/hexkit/providers/mongokafka/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -10,44 +10,47 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-"""An implementation of the DaoOutboxFactoryProtocol based on MongoDB and Apache Kafka."""
+"""An implementation of the DaoPublisherFactoryProtocol based on MongoDB and Apache Kafka.
+
+Require dependencies of the `akafka` and `mongodb` extras.
+"""
 
 import json
 from collections.abc import AsyncIterator, Awaitable, Collection, Mapping
 from contextlib import AbstractAsyncContextManager, asynccontextmanager, contextmanager
 from typing import Any, Callable, Generic, Optional
 
+from aiokafka import AIOKafkaProducer
 from motor.core import AgnosticCollection
 from motor.motor_asyncio import AsyncIOMotorClient
 
 from hexkit.custom_types import JsonObject
 from hexkit.protocols.dao import (
     DaoNaturalId,
     Dto,
     ResourceNotFoundError,
 )
-from hexkit.protocols.dao_outbox import DaoOutbox, DaoOutboxFactoryProtocol
+from hexkit.protocols.daopub import DaoPublisher, DaoPublisherFactoryProtocol
 from hexkit.protocols.eventpub import EventPublisherProtocol
-from hexkit.providers.akafka.provider import KafkaConfig, KafkaEventPublisher
+from hexkit.providers.akafka import KafkaConfig, KafkaEventPublisher
+from hexkit.providers.akafka.provider.daosub import CHANGE_EVENT_TYPE, DELETE_EVENT_TYPE
+from hexkit.providers.akafka.provider.eventpub import KafkaProducerCompatible
 from hexkit.providers.mongodb.provider import (
     MongoDbConfig,
     MongoDbDaoNaturalId,
     get_single_hit,
     replace_id_field_in_find_mapping,
     validate_find_mapping,
 )
 
-CHANGE_EVENT_TYPE = "upserted"
-DELETE_EVENT_TYPE = "deleted"
-
 
 class ResourceDeletedError(RuntimeError):
     """Raised when trying to interact with a resource that has been deleted."""
 
     def __init__(self, id_: str):
         """Initialize the exception."""
         super().__init__(f"Resource with ID {id_} has been deleted.")
@@ -142,15 +145,15 @@
     """A context manager that translates ResourceDeletedError into ResourceNotFoundError."""
     try:
         yield
     except ResourceDeletedError as error:
         raise ResourceNotFoundError(id_=error.id_) from error
 
 
-class MongoKafkaDaoOutbox(Generic[Dto]):
+class MongoKafkaDaoPublisher(Generic[Dto]):
     """A DAO that uses a natural resource ID provided by the client."""
 
     @classmethod
     def with_transaction(cls) -> AbstractAsyncContextManager["DaoNaturalId[Dto]"]:
         """Creates a transaction manager that uses an async context manager interface:
 
         Upon __aenter__, pens a new transactional scope. Returns a transaction-scoped
@@ -356,35 +359,38 @@
             await self.publish_document(document)
 
 
 class MongoKafkaConfig(MongoDbConfig, KafkaConfig):
     """Config parameters and their defaults."""
 
 
-class MongoKafkaDaoOutboxFactory(DaoOutboxFactoryProtocol):
-    """A provider implementing the DaoOutboxFactoryProtocol based on MongoDB and
+class MongoKafkaDaoPublisherFactory(DaoPublisherFactoryProtocol):
+    """A provider implementing the DaoPublisherFactoryProtocol based on MongoDB and
     Apache Kafka.
     """
 
     @classmethod
     @asynccontextmanager
     async def construct(
         cls,
         *,
         config: MongoKafkaConfig,
+        kafka_producer_cls: type[KafkaProducerCompatible] = AIOKafkaProducer,
     ):
         """Setup and teardown an instance of the provider.
 
         Args:
             config: MongoDB-specific config parameters.
 
         Returns:
             An instance of the provider.
         """
-        async with KafkaEventPublisher.construct(config=config) as event_publisher:
+        async with KafkaEventPublisher.construct(
+            config=config, kafka_producer_cls=kafka_producer_cls
+        ) as event_publisher:
             yield cls(config=config, event_publisher=event_publisher)
 
     def __init__(
         self, *, config: MongoKafkaConfig, event_publisher: EventPublisherProtocol
     ):
         """Please do not call directly! Should be called by the `construct` method."""
         self._config = config
@@ -406,19 +412,19 @@
         name: str,
         dto_model: type[Dto],
         id_field: str,
         fields_to_index: Optional[Collection[str]],
         dto_to_event: Callable[[Dto], JsonObject],
         event_topic: str,
         autopublish: bool,
-    ) -> DaoOutbox[Dto]:
+    ) -> DaoPublisher[Dto]:
         """Constructs a DAO for interacting with resources in a MongoDB database.
         Updates are automatically published to Apache Kafka.
 
-        Please see the DaoOutboxFactoryProtocol superclass for documentation of
+        Please see the DaoPublisherFactoryProtocol superclass for documentation of
         parameters.
         """
         if fields_to_index is not None:
             raise NotImplementedError(
                 "Indexing on non-ID fields has not been implemented, yet."
             )
 
@@ -446,15 +452,15 @@
         )
         publish_delete = get_delete_publish_func(
             event_topic=event_topic,
             event_publisher=self._event_publisher,
             collection=collection,
         )
 
-        return MongoKafkaDaoOutbox(
+        return MongoKafkaDaoPublisher(
             id_field=id_field,
             dto_model=dto_model,
             collection=collection,
             dao=dao,
             publish_change=publish_change,
             publish_delete=publish_delete,
             autopublish=autopublish,
```

### Comparing `hexkit-2.2.0/src/hexkit/providers/s3/__init__.py` & `hexkit-3.0.0/src/hexkit/providers/s3/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `hexkit-2.2.0/src/hexkit/providers/s3/provider.py` & `hexkit-3.0.0/src/hexkit/providers/s3/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -159,17 +159,25 @@
             endpoint_url=self.endpoint_url,
             aws_access_key_id=self._config.s3_access_key_id,
             aws_secret_access_key=self._config.s3_secret_access_key.get_secret_value(),
             aws_session_token=session_token,
             config=self._advanced_config,
         )
 
+        self._created_buckets: set[str] = set()
+
     def __repr__(self) -> str:
         return f"{self.__class__.__qualname__}(config={repr(self._config)})"
 
+    async def delete_created_buckets(self):
+        """Delete all the buckets that have been created by the provider."""
+        buckets = self._created_buckets
+        while buckets:
+            await self._delete_bucket(bucket_id=buckets.pop(), delete_content=True)
+
     @staticmethod
     def _format_s3_error_code(error_code: str):
         """Format a message to describe an S3 error code."""
         return f"S3 error with code: '{error_code}'"
 
     @classmethod
     def _translate_s3_client_errors(
@@ -257,14 +265,16 @@
 
         try:
             await asyncio.to_thread(self._client.create_bucket, Bucket=bucket_id)
         except botocore.exceptions.ClientError as error:
             raise self._translate_s3_client_errors(
                 error, bucket_id=bucket_id
             ) from error
+        else:
+            self._created_buckets.add(bucket_id)
 
     async def _delete_bucket(
         self, bucket_id: str, *, delete_content: bool = False
     ) -> None:
         """
         Delete a bucket (= a structure that can hold multiple file objects) with the
         specified unique ID. If `delete_content` is set to True, any contained objects
@@ -279,14 +289,16 @@
             if delete_content:
                 await asyncio.to_thread(content.delete)
             await asyncio.to_thread(bucket.delete)
         except botocore.exceptions.ClientError as error:
             raise self._translate_s3_client_errors(
                 error, bucket_id=bucket_id
             ) from error
+        else:
+            self._created_buckets.discard(bucket_id)
 
     async def _list_all_object_ids(self, *, bucket_id: str) -> list[str]:
         """Retrieve a list of IDs for all objects currently present in the specified bucket"""
         await self._assert_bucket_exists(bucket_id)
 
         try:
             bucket = self._resource.Bucket(bucket_id)
```

### Comparing `hexkit-2.2.0/src/hexkit/providers/s3/test_files/__init__.py` & `hexkit-3.0.0/src/hexkit/protocols/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+#
+
+"""Sub-package containing protocols."""
```

### Comparing `hexkit-2.2.0/src/hexkit/providers/s3/testutils.py` & `hexkit-3.0.0/src/hexkit/providers/s3/testutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -43,15 +43,15 @@
 TEST_FILE_PATHS = [
     TEST_FILE_DIR / filename
     for filename in os.listdir(TEST_FILE_DIR)
     if filename.startswith("test_") and filename.endswith(".yaml")
 ]
 
 MEBIBYTE = 1024 * 1024
-TIMEOUT = 30
+TIMEOUT = 60
 
 
 def calc_md5(content: bytes) -> str:
     """Calc the md5 checksum for the specified bytes."""
     return hashlib.md5(content, usedforsecurity=False).hexdigest()  # nosec
 
 
@@ -83,44 +83,44 @@
 
     def __init__(self, config: S3Config, storage: S3ObjectStorage):
         """Initialize with config."""
         self.config = config
         self.storage = storage
         self._buckets: set[str] = set()
 
-    async def empty_buckets(self, buckets_to_exclude: Optional[list[str]] = None):
-        """Clean the test artifacts or files from given bucket"""
-        if buckets_to_exclude is None:
-            buckets_to_exclude = []
-
-        for bucket in self._buckets:
-            if bucket in buckets_to_exclude:
-                continue
-
-            # Get list of all objects in the bucket
-            object_ids = await self.storage.list_all_object_ids(bucket_id=bucket)
-
-            # Delete all objects
-            for object_id in object_ids:
-                await self.storage.delete_object(bucket_id=bucket, object_id=object_id)
-
     async def populate_buckets(self, buckets: list[str]):
         """Populate the storage with buckets."""
         await populate_storage(
             self.storage, bucket_fixtures=buckets, object_fixtures=[]
         )
 
         self._buckets.update(buckets)
 
     async def populate_file_objects(self, file_objects: list[FileObject]):
         """Populate the storage with file objects."""
         await populate_storage(
             self.storage, bucket_fixtures=[], object_fixtures=file_objects
         )
 
+    async def empty_buckets(self, buckets_to_exclude: Optional[list[str]] = None):
+        """Clean the test artifacts or files from the populated buckets."""
+        for bucket in self._buckets.difference(buckets_to_exclude or []):
+            # Get list of all objects in the bucket
+            object_ids = await self.storage.list_all_object_ids(bucket_id=bucket)
+            # Delete all of these objects
+            for object_id in object_ids:
+                await self.storage.delete_object(bucket_id=bucket, object_id=object_id)
+
+    async def delete_buckets(self, buckets_to_exclude: Optional[list[str]] = None):
+        """Delete the populated buckets."""
+        buckets = self._buckets
+        for bucket in list(buckets.difference(buckets_to_exclude or [])):
+            await self.storage.delete_bucket(bucket, delete_content=True)
+            buckets.discard(bucket)
+
 
 def s3_fixture_function() -> Generator[S3Fixture, None, None]:
     """Pytest fixture for tests depending on the S3ObjectStorage DAO.
 
     **Do not call directly** Instead, use get_s3_fixture()
     """
     with LocalStackContainer(image="localstack/localstack:0.14.5").with_services(
@@ -138,16 +138,16 @@
 
 
 s3_fixture = get_s3_fixture()
 
 
 @contextmanager
 def temp_file_object(
-    bucket_id: str = "mydefaulttestbucket001",
-    object_id: str = "mydefaulttestobject001",
+    bucket_id: str = "default-test-bucket",
+    object_id: str = "default-test-object",
     size: int = 5 * MEBIBYTE,
 ) -> Generator[FileObject, None, None]:
     """Generates a file object with the specified size in bytes."""
     chunk_size = 1024
     chunk = b"\0" * chunk_size
     current_size = 0
     with NamedTemporaryFile("w+b") as temp_file:
@@ -160,16 +160,16 @@
         temp_file.flush()
 
         yield FileObject(
             file_path=Path(temp_file.name), bucket_id=bucket_id, object_id=object_id
         )
 
 
-@pytest.fixture
-def file_fixture():
+@pytest.fixture(name="tmp_file")
+def file_fixture() -> Generator[FileObject, None, None]:
     """A fixture that provides a temporary file."""
     with temp_file_object() as temp_file:
         yield temp_file
 
 
 def upload_file(presigned_url: PresignedPostURL, file_path: Path, file_md5: str):
     """Uploads the test file to the specified URL"""
@@ -370,17 +370,17 @@
 # This workflow is defined as a seperate function so that it can also be used
 # outside of the `tests` package e.g. to test the compliance of an S3-compatible
 # object storage implementation:
 async def typical_workflow(
     storage_client: ObjectStorageProtocol,
     test_file_path: Path,
     test_file_md5: str,
-    bucket1_id: str = "mytestbucket001",
-    bucket2_id: str = "mytestbucket002",
-    object_id: str = "mytestobject001",
+    bucket1_id: str = "example-bucket-1",
+    bucket2_id: str = "excample-bucket-2",
+    object_id: str = "example-object-1",
     use_multipart_upload: bool = True,
     part_size: int = ObjectStorageProtocol.DEFAULT_PART_SIZE,
 ):
     """Run a typical workflow of basic object operations using a S3 service."""
     print("Run a workflow for testing basic object operations using a S3 service:")
 
     print(f" - create new bucket {bucket1_id}")
@@ -447,8 +447,15 @@
     download_url2 = await storage_client.get_object_download_url(
         bucket_id=bucket2_id, object_id=object_id
     )
     download_and_check_test_file(
         presigned_url=download_url2, expected_md5=test_file_md5
     )
 
+    print(f" - delete bucket {bucket2_id}")
+    await storage_client.delete_object(bucket_id=bucket2_id, object_id=object_id)
+    await storage_client.delete_bucket(bucket2_id)
+
+    print(" - confirm bucket deletion")
+    assert not await storage_client.does_bucket_exist(bucket2_id)  # noqa: S101
+
     print("Done.")
```

### Comparing `hexkit-2.2.0/src/hexkit/providers/testing/__init__.py` & `hexkit-3.0.0/src/hexkit/providers/testing/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `hexkit-2.2.0/src/hexkit/providers/testing/eventpub.py` & `hexkit-3.0.0/src/hexkit/providers/testing/eventpub.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `hexkit-2.2.0/src/hexkit/utils.py` & `hexkit-3.0.0/src/hexkit/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `hexkit-2.2.0/src/hexkit.egg-info/PKG-INFO` & `hexkit-3.0.0/src/hexkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: hexkit
-Version: 2.2.0
+Version: 3.0.0
 Summary: A Toolkit for Building Microservices using the Hexagonal Architecture
 Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ghga-de/hexkit
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic<3,>=2
 Requires-Dist: pydantic_settings<3,>=2
 Requires-Dist: PyYAML<7,>=6.0
 Provides-Extra: akafka
-Requires-Dist: aiokafka~=0.8.0; extra == "akafka"
-Requires-Dist: jsonschema<5,>=4.17.3; extra == "akafka"
+Requires-Dist: aiokafka~=0.10.0; extra == "akafka"
+Requires-Dist: jsonschema<5,>=4.21; extra == "akafka"
 Provides-Extra: s3
 Requires-Dist: boto3<2,>=1.26.50; extra == "s3"
 Requires-Dist: botocore<2,>=1.29.50; extra == "s3"
 Provides-Extra: mongodb
 Requires-Dist: motor<4,>=3.1.1; extra == "mongodb"
 Provides-Extra: test-akafka
 Requires-Dist: hexkit[akafka]; extra == "test-akafka"
```

### Comparing `hexkit-2.2.0/src/hexkit.egg-info/SOURCES.txt` & `hexkit-3.0.0/src/hexkit.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,31 +5,38 @@
 src/hexkit/__init__.py
 src/hexkit/__main__.py
 src/hexkit/base.py
 src/hexkit/config.py
 src/hexkit/correlation.py
 src/hexkit/custom_types.py
 src/hexkit/log.py
+src/hexkit/py.typed
 src/hexkit/utils.py
 src/hexkit.egg-info/PKG-INFO
 src/hexkit.egg-info/SOURCES.txt
 src/hexkit.egg-info/dependency_links.txt
 src/hexkit.egg-info/requires.txt
 src/hexkit.egg-info/top_level.txt
 src/hexkit/protocols/__init__.py
 src/hexkit/protocols/dao.py
-src/hexkit/protocols/dao_outbox.py
+src/hexkit/protocols/daopub.py
+src/hexkit/protocols/daosub.py
 src/hexkit/protocols/eventpub.py
 src/hexkit/protocols/eventsub.py
 src/hexkit/protocols/objstorage.py
 src/hexkit/providers/__init__.py
 src/hexkit/providers/akafka/__init__.py
-src/hexkit/providers/akafka/provider.py
+src/hexkit/providers/akafka/config.py
 src/hexkit/providers/akafka/testcontainer.py
 src/hexkit/providers/akafka/testutils.py
+src/hexkit/providers/akafka/provider/__init__.py
+src/hexkit/providers/akafka/provider/daosub.py
+src/hexkit/providers/akafka/provider/eventpub.py
+src/hexkit/providers/akafka/provider/eventsub.py
+src/hexkit/providers/akafka/provider/utils.py
 src/hexkit/providers/mongodb/__init__.py
 src/hexkit/providers/mongodb/provider.py
 src/hexkit/providers/mongodb/testutils.py
 src/hexkit/providers/mongokafka/__init__.py
 src/hexkit/providers/mongokafka/provider.py
 src/hexkit/providers/s3/__init__.py
 src/hexkit/providers/s3/provider.py
```

