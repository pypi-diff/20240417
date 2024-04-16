# Comparing `tmp/gama_cli-2.2.0.tar.gz` & `tmp/gama_cli-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gama_cli-2.2.0.tar", last modified: Wed Apr 10 12:27:42 2024, max compression
+gzip compressed data, was "gama_cli-2.3.0.tar", last modified: Tue Apr 16 22:04:43 2024, max compression
```

## Comparing `gama_cli-2.2.0.tar` & `gama_cli-2.3.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:27:42.628624 gama_cli-2.2.0/
--rw-r--r--   0 runner    (1000) runner    (1001)     2468 2024-04-10 12:27:42.628624 gama_cli-2.2.0/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)     1656 2024-04-10 12:26:35.000000 gama_cli-2.2.0/README.md
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:27:42.624623 gama_cli-2.2.0/gama_cli/
--rw-rw-r--   0 runner    (1000) runner    (1001)        0 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     2539 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/banner.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     2430 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/cli.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:27:42.624623 gama_cli-2.2.0/gama_cli/docker/
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:27:42.624623 gama_cli-2.2.0/gama_cli/docker/gs/
--rw-rw-r--   0 runner    (1000) runner    (1001)      402 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/gs/docker-compose.dev.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)       60 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/gs/docker-compose.network-host.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      172 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/gs/docker-compose.network-shared.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)       68 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/gs/docker-compose.prod.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      157 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/gs/docker-compose.warthog-combo.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      463 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/gs/docker-compose.yaml
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:27:42.628624 gama_cli-2.2.0/gama_cli/docker/vessel/
--rw-rw-r--   0 runner    (1000) runner    (1001)     2397 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/vessel/docker-compose.dev.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      109 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/vessel/docker-compose.network-host.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      517 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/vessel/docker-compose.network-shared.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      247 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/vessel/docker-compose.prod.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      296 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/vessel/docker-compose.variant.armidale.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      290 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/vessel/docker-compose.variant.educat.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      299 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/vessel/docker-compose.variant.oracle_22.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      387 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/vessel/docker-compose.variant.oracle_2_2.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      386 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/vessel/docker-compose.variant.whiskey_bravo.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)     1851 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/vessel/docker-compose.yaml
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:27:42.628624 gama_cli-2.2.0/gama_cli/groups/
--rw-rw-r--   0 runner    (1000) runner    (1001)        0 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/groups/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      839 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/groups/attach.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      327 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/groups/docker.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      249 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/groups/git.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     6993 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/groups/gs.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     2062 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/groups/misc.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     1168 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/groups/setup.py
--rw-rw-r--   0 runner    (1000) runner    (1001)    14953 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/groups/vessel.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     4345 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/helpers.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:27:42.628624 gama_cli-2.2.0/gama_cli.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1001)     2468 2024-04-10 12:27:42.000000 gama_cli-2.2.0/gama_cli.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)     1368 2024-04-10 12:27:42.000000 gama_cli-2.2.0/gama_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-10 12:27:42.000000 gama_cli-2.2.0/gama_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       70 2024-04-10 12:27:42.000000 gama_cli-2.2.0/gama_cli.egg-info/entry_points.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       73 2024-04-10 12:27:42.000000 gama_cli-2.2.0/gama_cli.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        9 2024-04-10 12:27:42.000000 gama_cli-2.2.0/gama_cli.egg-info/top_level.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-10 12:27:28.000000 gama_cli-2.2.0/gama_cli.egg-info/zip-safe
--rw-rw-r--   0 runner    (1000) runner    (1001)     1017 2024-04-10 12:27:42.628624 gama_cli-2.2.0/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-04-10 12:26:35.000000 gama_cli-2.2.0/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-16 22:04:43.349051 gama_cli-2.3.0/
+-rw-r--r--   0 runner    (1000) runner    (1001)     2468 2024-04-16 22:04:43.349051 gama_cli-2.3.0/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1656 2024-04-16 22:03:46.000000 gama_cli-2.3.0/README.md
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-16 22:04:43.345051 gama_cli-2.3.0/gama_cli/
+-rw-rw-r--   0 runner    (1000) runner    (1001)        0 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2539 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/banner.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2430 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/cli.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-16 22:04:43.345051 gama_cli-2.3.0/gama_cli/docker/
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-16 22:04:43.345051 gama_cli-2.3.0/gama_cli/docker/gs/
+-rw-rw-r--   0 runner    (1000) runner    (1001)      402 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/docker/gs/docker-compose.dev.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)       60 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/docker/gs/docker-compose.network-host.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      172 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/docker/gs/docker-compose.network-shared.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)       68 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/docker/gs/docker-compose.prod.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      157 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/docker/gs/docker-compose.warthog-combo.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      463 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/docker/gs/docker-compose.yaml
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-16 22:04:43.349051 gama_cli-2.3.0/gama_cli/docker/vessel/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2397 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/docker/vessel/docker-compose.dev.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      109 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/docker/vessel/docker-compose.network-host.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      517 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/docker/vessel/docker-compose.network-shared.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      247 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/docker/vessel/docker-compose.prod.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      296 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/docker/vessel/docker-compose.variant.armidale.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      290 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/docker/vessel/docker-compose.variant.educat.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      299 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/docker/vessel/docker-compose.variant.oracle_22.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      387 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/docker/vessel/docker-compose.variant.oracle_2_2.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      386 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/docker/vessel/docker-compose.variant.whiskey_bravo.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1851 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/docker/vessel/docker-compose.yaml
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-16 22:04:43.349051 gama_cli-2.3.0/gama_cli/groups/
+-rw-rw-r--   0 runner    (1000) runner    (1001)        0 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/groups/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      839 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/groups/attach.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      327 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/groups/docker.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      249 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/groups/git.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     6993 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/groups/gs.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2062 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/groups/misc.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1168 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/groups/setup.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)    15038 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/groups/vessel.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     4345 2024-04-16 22:03:46.000000 gama_cli-2.3.0/gama_cli/helpers.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-16 22:04:43.349051 gama_cli-2.3.0/gama_cli.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1001)     2468 2024-04-16 22:04:43.000000 gama_cli-2.3.0/gama_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1368 2024-04-16 22:04:43.000000 gama_cli-2.3.0/gama_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-16 22:04:43.000000 gama_cli-2.3.0/gama_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       70 2024-04-16 22:04:43.000000 gama_cli-2.3.0/gama_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       73 2024-04-16 22:04:43.000000 gama_cli-2.3.0/gama_cli.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        9 2024-04-16 22:04:43.000000 gama_cli-2.3.0/gama_cli.egg-info/top_level.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-16 22:04:27.000000 gama_cli-2.3.0/gama_cli.egg-info/zip-safe
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1017 2024-04-16 22:04:43.349051 gama_cli-2.3.0/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-04-16 22:03:46.000000 gama_cli-2.3.0/setup.py
```

### Comparing `gama_cli-2.2.0/PKG-INFO` & `gama_cli-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gama_cli
-Version: 2.2.0
+Version: 2.3.0
 Summary: A CLI for interacting with the GAMA platform
 Home-page: https://github.com/Greenroom-Robotics/gama
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `gama_cli-2.2.0/README.md` & `gama_cli-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gama_cli-2.2.0/gama_cli/banner.py` & `gama_cli-2.3.0/gama_cli/banner.py`

 * *Files identical despite different names*

### Comparing `gama_cli-2.2.0/gama_cli/cli.py` & `gama_cli-2.3.0/gama_cli/cli.py`

 * *Files identical despite different names*

### Comparing `gama_cli-2.2.0/gama_cli/docker/vessel/docker-compose.dev.yaml` & `gama_cli-2.3.0/gama_cli/docker/vessel/docker-compose.dev.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-2.2.0/gama_cli/docker/vessel/docker-compose.network-shared.yaml` & `gama_cli-2.3.0/gama_cli/docker/vessel/docker-compose.network-shared.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-2.2.0/gama_cli/docker/vessel/docker-compose.yaml` & `gama_cli-2.3.0/gama_cli/docker/vessel/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-2.2.0/gama_cli/groups/attach.py` & `gama_cli-2.3.0/gama_cli/groups/attach.py`

 * *Files identical despite different names*

### Comparing `gama_cli-2.2.0/gama_cli/groups/gs.py` & `gama_cli-2.3.0/gama_cli/groups/gs.py`

 * *Files identical despite different names*

### Comparing `gama_cli-2.2.0/gama_cli/groups/misc.py` & `gama_cli-2.3.0/gama_cli/groups/misc.py`

 * *Files identical despite different names*

### Comparing `gama_cli-2.2.0/gama_cli/groups/setup.py` & `gama_cli-2.3.0/gama_cli/groups/setup.py`

 * *Files identical despite different names*

### Comparing `gama_cli-2.2.0/gama_cli/groups/vessel.py` & `gama_cli-2.3.0/gama_cli/groups/vessel.py`

 * *Files 1% similar despite different names*

```diff
@@ -504,14 +504,15 @@
                 type=click.Choice([item.value for item in Network]),
             ),
             log_level=click.prompt(
                 "Log level",
                 default=config_current.log_level,
                 type=click.Choice([item.value for item in LogLevel]),
             ),
+            record=click.prompt("Record", default=config_current.record, type=bool),
         )
         write_vessel_config(config)
 
 
 @click.command(name="config")
 def config():  # type: ignore
     """Read Config"""
```

### Comparing `gama_cli-2.2.0/gama_cli/helpers.py` & `gama_cli-2.3.0/gama_cli/helpers.py`

 * *Files identical despite different names*

### Comparing `gama_cli-2.2.0/gama_cli.egg-info/PKG-INFO` & `gama_cli-2.3.0/gama_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gama_cli
-Version: 2.2.0
+Version: 2.3.0
 Summary: A CLI for interacting with the GAMA platform
 Home-page: https://github.com/Greenroom-Robotics/gama
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `gama_cli-2.2.0/gama_cli.egg-info/SOURCES.txt` & `gama_cli-2.3.0/gama_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gama_cli-2.2.0/setup.cfg` & `gama_cli-2.3.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gama_cli
-version = 2.2.0
+version = 2.3.0
 url = https://github.com/Greenroom-Robotics/gama
 author = Greenroom Robotics
 author_email = team@greenroomrobotics.com
 maintainer = David Revay
 maintainer_email = david.revay@greenroomrobotics.com
 classifiers = 
 	Development Status :: 3 - Alpha
```

