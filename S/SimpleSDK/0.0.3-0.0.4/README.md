# Comparing `tmp/simplesdk-0.0.3.tar.gz` & `tmp/simplesdk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplesdk-0.0.3.tar", last modified: Sat Apr 13 22:23:26 2024, max compression
+gzip compressed data, was "simplesdk-0.0.4.tar", last modified: Wed Apr 17 18:09:34 2024, max compression
```

## Comparing `simplesdk-0.0.3.tar` & `simplesdk-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:23:26.477647 simplesdk-0.0.3/
--rw-r--r--   0 naiel      (501) staff       (20)     1063 2024-04-13 21:41:46.000000 simplesdk-0.0.3/LICENSE
--rw-r--r--   0 naiel      (501) staff       (20)      392 2024-04-13 22:23:26.477362 simplesdk-0.0.3/PKG-INFO
--rw-r--r--   0 naiel      (501) staff       (20)       53 2024-04-13 21:41:46.000000 simplesdk-0.0.3/README.md
-drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:23:26.477102 simplesdk-0.0.3/SimpleSDK.egg-info/
--rw-r--r--   0 naiel      (501) staff       (20)      392 2024-04-13 22:23:26.000000 simplesdk-0.0.3/SimpleSDK.egg-info/PKG-INFO
--rw-r--r--   0 naiel      (501) staff       (20)      228 2024-04-13 22:23:26.000000 simplesdk-0.0.3/SimpleSDK.egg-info/SOURCES.txt
--rw-r--r--   0 naiel      (501) staff       (20)        1 2024-04-13 22:23:26.000000 simplesdk-0.0.3/SimpleSDK.egg-info/dependency_links.txt
--rw-r--r--   0 naiel      (501) staff       (20)       10 2024-04-13 22:23:26.000000 simplesdk-0.0.3/SimpleSDK.egg-info/top_level.txt
--rw-r--r--   0 naiel      (501) staff       (20)       38 2024-04-13 22:23:26.477694 simplesdk-0.0.3/setup.cfg
--rw-r--r--   0 naiel      (501) staff       (20)      700 2024-04-13 22:23:23.000000 simplesdk-0.0.3/setup.py
-drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:23:26.476936 simplesdk-0.0.3/simplesdk/
--rw-r--r--   0 naiel      (501) staff       (20)       23 2024-04-13 21:56:32.000000 simplesdk-0.0.3/simplesdk/__init__.py
--rw-r--r--   0 naiel      (501) staff       (20)    11876 2024-04-13 21:46:58.000000 simplesdk-0.0.3/simplesdk/internal.py
--rw-r--r--   0 naiel      (501) staff       (20)      270 2024-04-13 22:13:55.000000 simplesdk-0.0.3/simplesdk/translations.py
+drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-17 18:09:34.313114 simplesdk-0.0.4/
+-rw-r--r--   0 naiel      (501) staff       (20)     1063 2024-04-13 21:41:46.000000 simplesdk-0.0.4/LICENSE
+-rw-r--r--   0 naiel      (501) staff       (20)      392 2024-04-17 18:09:34.312809 simplesdk-0.0.4/PKG-INFO
+-rw-r--r--   0 naiel      (501) staff       (20)       53 2024-04-13 21:41:46.000000 simplesdk-0.0.4/README.md
+drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-17 18:09:34.312576 simplesdk-0.0.4/SimpleSDK.egg-info/
+-rw-r--r--   0 naiel      (501) staff       (20)      392 2024-04-17 18:09:34.000000 simplesdk-0.0.4/SimpleSDK.egg-info/PKG-INFO
+-rw-r--r--   0 naiel      (501) staff       (20)      228 2024-04-17 18:09:34.000000 simplesdk-0.0.4/SimpleSDK.egg-info/SOURCES.txt
+-rw-r--r--   0 naiel      (501) staff       (20)        1 2024-04-17 18:09:34.000000 simplesdk-0.0.4/SimpleSDK.egg-info/dependency_links.txt
+-rw-r--r--   0 naiel      (501) staff       (20)       10 2024-04-17 18:09:34.000000 simplesdk-0.0.4/SimpleSDK.egg-info/top_level.txt
+-rw-r--r--   0 naiel      (501) staff       (20)       38 2024-04-17 18:09:34.313157 simplesdk-0.0.4/setup.cfg
+-rw-r--r--   0 naiel      (501) staff       (20)      700 2024-04-17 18:09:33.000000 simplesdk-0.0.4/setup.py
+drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-17 18:09:34.312372 simplesdk-0.0.4/simplesdk/
+-rw-r--r--   0 naiel      (501) staff       (20)       23 2024-04-13 21:56:32.000000 simplesdk-0.0.4/simplesdk/__init__.py
+-rw-r--r--   0 naiel      (501) staff       (20)    13375 2024-04-17 18:08:04.000000 simplesdk-0.0.4/simplesdk/internal.py
+-rw-r--r--   0 naiel      (501) staff       (20)      270 2024-04-13 22:13:55.000000 simplesdk-0.0.4/simplesdk/translations.py
```

### Comparing `simplesdk-0.0.3/LICENSE` & `simplesdk-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `simplesdk-0.0.3/setup.py` & `simplesdk-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup  # type: ignore
 
 __project__ = "SimpleSDK"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 __description__ = (
     "SDK for EuskadiTech's Simple Axel (https://git.tech.eus/EuskadiTech/SimpleSDK)"
 )
 __packages__ = ["simplesdk"]
 __url__ = "https://git.tech.eus/EuskadiTech/SimpleSDK"
 __author__ = "EuskadiTech"
 __classifiers__ = [
```

### Comparing `simplesdk-0.0.3/simplesdk/internal.py` & `simplesdk-0.0.4/simplesdk/internal.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import requests
 import random
 from threading import Thread
 from time import sleep
 import hashlib
 from os import environ as env
 from uuid import uuid4
+import yaml
 
 
 def safe_hash(value: str, salt: str = str(env.get("ET_SALT"))):
     salted_password = salt[::-1] + value + salt
     salted_password = salted_password[::-1] + salted_password
     hash = hashlib.sha512(salted_password.encode()).hexdigest()
     return hash
@@ -385,7 +386,51 @@
         Thread(target=self.get_alumnos, name="get tareas").start()
         Thread(target=self.get_comedor, name="get comedor").start()
         Thread(target=self.get_comedor_reciente, name="get comedor reciente").start()
         Thread(target=self.get_funcs, name="get funcs").start()
         while self.status < 5:
             sleep(0.01)
         return self.obj
+
+
+class AutoAula:
+    def __init__(self, sdk: AulaSDK):
+        self.sdk = sdk
+
+    def get_year_day(self):
+        return datetime.now().timetuple().tm_yday
+
+    def get_aula_id(self, aula_code: str):
+        return self.sdk.aulas__getByCode(aula_code)["0(aulas)"]["id"]
+
+    def create_task(
+        self, config: dict, alumno: str, tarea: str, fecha: str, orden: int
+    ):
+        id = self.get_aula_id(config["aula"])
+        self.sdk.tareas__new(id, alumno, tarea, fecha, orden)
+
+    def run_daily(self, config: dict, aula_code: str, dry_run: bool = False):
+        print(f"=== Ejecutando AutoAula para {config.get('friendly_name', aula_code)}")
+        self.sdk.auth()
+        iT = 0
+        cT = 0
+        for tarea in config["tareas"]:
+            i = self.get_year_day() % len(tarea["alumnos"])
+            a = tarea["alumnos"][i]
+            t = tarea["tarea"]
+            o = tarea["orden"]
+            f = datetime.now().isoformat().split("T")[0]
+            iT += 1
+            if not dry_run:
+                self.create_task(config, a, t, f, o)
+                cT += 1
+        print(f"{iT} tarea(s) procesada(s), {cT} tarea(s) creada(s)")
+
+    def run_all(self):
+        enabled = [
+            a
+            for a in self.sdk.aulas__all()
+            if "autoaula_enabled" in a["0(aulas)"]["funcs"]
+        ]
+        for aula in enabled:
+            config = yaml.safe_load(aula["0(aulas)"]["autoaula_conf"])
+            self.run_daily(config, aula["0(aulas)"]["code"])
```

