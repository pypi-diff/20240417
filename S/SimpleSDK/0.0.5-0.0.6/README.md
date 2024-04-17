# Comparing `tmp/simplesdk-0.0.5.tar.gz` & `tmp/simplesdk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplesdk-0.0.5.tar", last modified: Wed Apr 17 18:18:00 2024, max compression
+gzip compressed data, was "simplesdk-0.0.6.tar", last modified: Wed Apr 17 18:39:30 2024, max compression
```

## Comparing `simplesdk-0.0.5.tar` & `simplesdk-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-17 18:18:00.758895 simplesdk-0.0.5/
--rw-r--r--   0 naiel      (501) staff       (20)     1063 2024-04-13 21:41:46.000000 simplesdk-0.0.5/LICENSE
--rw-r--r--   0 naiel      (501) staff       (20)      392 2024-04-17 18:18:00.758579 simplesdk-0.0.5/PKG-INFO
--rw-r--r--   0 naiel      (501) staff       (20)       53 2024-04-13 21:41:46.000000 simplesdk-0.0.5/README.md
-drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-17 18:18:00.758323 simplesdk-0.0.5/SimpleSDK.egg-info/
--rw-r--r--   0 naiel      (501) staff       (20)      392 2024-04-17 18:18:00.000000 simplesdk-0.0.5/SimpleSDK.egg-info/PKG-INFO
--rw-r--r--   0 naiel      (501) staff       (20)      228 2024-04-17 18:18:00.000000 simplesdk-0.0.5/SimpleSDK.egg-info/SOURCES.txt
--rw-r--r--   0 naiel      (501) staff       (20)        1 2024-04-17 18:18:00.000000 simplesdk-0.0.5/SimpleSDK.egg-info/dependency_links.txt
--rw-r--r--   0 naiel      (501) staff       (20)       10 2024-04-17 18:18:00.000000 simplesdk-0.0.5/SimpleSDK.egg-info/top_level.txt
--rw-r--r--   0 naiel      (501) staff       (20)       38 2024-04-17 18:18:00.758941 simplesdk-0.0.5/setup.cfg
--rw-r--r--   0 naiel      (501) staff       (20)      700 2024-04-17 18:17:21.000000 simplesdk-0.0.5/setup.py
-drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-17 18:18:00.758139 simplesdk-0.0.5/simplesdk/
--rw-r--r--   0 naiel      (501) staff       (20)       23 2024-04-13 21:56:32.000000 simplesdk-0.0.5/simplesdk/__init__.py
--rw-r--r--   0 naiel      (501) staff       (20)    13446 2024-04-17 18:17:53.000000 simplesdk-0.0.5/simplesdk/internal.py
--rw-r--r--   0 naiel      (501) staff       (20)      270 2024-04-13 22:13:55.000000 simplesdk-0.0.5/simplesdk/translations.py
+drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-17 18:39:30.820247 simplesdk-0.0.6/
+-rw-r--r--   0 naiel      (501) staff       (20)     1063 2024-04-13 21:41:46.000000 simplesdk-0.0.6/LICENSE
+-rw-r--r--   0 naiel      (501) staff       (20)      392 2024-04-17 18:39:30.819899 simplesdk-0.0.6/PKG-INFO
+-rw-r--r--   0 naiel      (501) staff       (20)       53 2024-04-13 21:41:46.000000 simplesdk-0.0.6/README.md
+drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-17 18:39:30.819522 simplesdk-0.0.6/SimpleSDK.egg-info/
+-rw-r--r--   0 naiel      (501) staff       (20)      392 2024-04-17 18:39:30.000000 simplesdk-0.0.6/SimpleSDK.egg-info/PKG-INFO
+-rw-r--r--   0 naiel      (501) staff       (20)      228 2024-04-17 18:39:30.000000 simplesdk-0.0.6/SimpleSDK.egg-info/SOURCES.txt
+-rw-r--r--   0 naiel      (501) staff       (20)        1 2024-04-17 18:39:30.000000 simplesdk-0.0.6/SimpleSDK.egg-info/dependency_links.txt
+-rw-r--r--   0 naiel      (501) staff       (20)       10 2024-04-17 18:39:30.000000 simplesdk-0.0.6/SimpleSDK.egg-info/top_level.txt
+-rw-r--r--   0 naiel      (501) staff       (20)       38 2024-04-17 18:39:30.820424 simplesdk-0.0.6/setup.cfg
+-rw-r--r--   0 naiel      (501) staff       (20)      700 2024-04-17 18:39:30.000000 simplesdk-0.0.6/setup.py
+drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-17 18:39:30.819102 simplesdk-0.0.6/simplesdk/
+-rw-r--r--   0 naiel      (501) staff       (20)       23 2024-04-13 21:56:32.000000 simplesdk-0.0.6/simplesdk/__init__.py
+-rw-r--r--   0 naiel      (501) staff       (20)    14000 2024-04-17 18:38:54.000000 simplesdk-0.0.6/simplesdk/internal.py
+-rw-r--r--   0 naiel      (501) staff       (20)      270 2024-04-13 22:13:55.000000 simplesdk-0.0.6/simplesdk/translations.py
```

### Comparing `simplesdk-0.0.5/LICENSE` & `simplesdk-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `simplesdk-0.0.5/setup.py` & `simplesdk-0.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup  # type: ignore
 
 __project__ = "SimpleSDK"
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 __description__ = (
     "SDK for EuskadiTech's Simple Axel (https://git.tech.eus/EuskadiTech/SimpleSDK)"
 )
 __packages__ = ["simplesdk"]
 __url__ = "https://git.tech.eus/EuskadiTech/SimpleSDK"
 __author__ = "EuskadiTech"
 __classifiers__ = [
```

### Comparing `simplesdk-0.0.5/simplesdk/internal.py` & `simplesdk-0.0.6/simplesdk/internal.py`

 * *Files 2% similar despite different names*

```diff
@@ -395,14 +395,19 @@
 class AutoAula:
     def __init__(self, sdk: AulaSDK):
         self.sdk = sdk
 
     def get_year_day(self):
         return datetime.now().timetuple().tm_yday
 
+    def contar_dias_laborables(self, desde_dia): # gracias a chatgpt ;-)
+        hoy = datetime.now()
+        desde_fecha = datetime(datetime.now().year, 1, 1) + timedelta(days=desde_dia - 1)  # Restamos 1 porque tm_yday cuenta desde 1
+        dias_laborables = sum(1 for i in range(desde_dia) if (desde_fecha + timedelta(days=i)).weekday() < 5)
+        return dias_laborables
     def get_aula_id(self, aula_code: str):
         return self.sdk.aulas__getByCode(aula_code)["0(aulas)"]["id"]
 
     def create_task(
         self,
         config: dict,
         aula_code: str,
@@ -416,15 +421,18 @@
 
     def run_daily(self, config: dict, aula_code: str, dry_run: bool = False):
         print(f"=== Ejecutando AutoAula para {config.get('friendly_name', aula_code)}")
         self.sdk.auth()
         iT = 0
         cT = 0
         for tarea in config["tareas"]:
-            i = self.get_year_day() % len(tarea["alumnos"])
+            if tarea.get("horario") == "laborales":
+                i = contar_dias_laborables(datetime.now().timetuple().tm_yday) % len(tarea["alumnos"])
+            else:
+                i = self.get_year_day() % len(tarea["alumnos"])
             a = tarea["alumnos"][i]
             t = tarea["tarea"]
             o = tarea["orden"]
             f = datetime.now().isoformat().split("T")[0]
             iT += 1
             if not dry_run:
                 self.create_task(config, aula_code, a, t, f, o)
```

