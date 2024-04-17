# Comparing `tmp/etabs_sdk-0.0.0.post0.tar.gz` & `tmp/etabs_sdk-0.0.1.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etabs_sdk-0.0.0.post0.tar", last modified: Wed Apr 17 15:55:41 2024, max compression
+gzip compressed data, was "etabs_sdk-0.0.1.post0.tar", last modified: Wed Apr 17 20:44:19 2024, max compression
```

## Comparing `etabs_sdk-0.0.0.post0.tar` & `etabs_sdk-0.0.1.post0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 15:55:41.953508 etabs_sdk-0.0.0.post0/
--rw-rw-rw-   0        0        0      171 2024-01-26 16:52:56.000000 etabs_sdk-0.0.0.post0/.editorconfig
--rw-rw-rw-   0        0        0     3072 2024-02-23 17:49:13.000000 etabs_sdk-0.0.0.post0/.gitignore
--rw-rw-rw-   0        0        0     2597 2024-04-17 14:08:02.000000 etabs_sdk-0.0.0.post0/LICENSE
--rw-rw-rw-   0        0        0     3629 2024-04-17 15:55:41.952508 etabs_sdk-0.0.0.post0/PKG-INFO
--rw-rw-rw-   0        0        0       71 2024-04-17 14:14:35.000000 etabs_sdk-0.0.0.post0/README.md
--rw-rw-rw-   0        0        0      639 2024-04-17 14:48:31.000000 etabs_sdk-0.0.0.post0/dev-requirements.txt
-drwxrwxrwx   0        0        0        0 2024-04-17 15:55:41.933509 etabs_sdk-0.0.0.post0/etabs_sdk/
--rw-rw-rw-   0        0        0      103 2024-04-17 15:27:29.000000 etabs_sdk-0.0.0.post0/etabs_sdk/__init__.py
--rw-rw-rw-   0        0        0      433 2024-04-17 15:55:41.000000 etabs_sdk-0.0.0.post0/etabs_sdk/_version.py
-drwxrwxrwx   0        0        0        0 2024-04-17 15:55:41.944511 etabs_sdk-0.0.0.post0/etabs_sdk/src/
--rw-rw-rw-   0        0        0      505 2024-04-17 15:23:22.000000 etabs_sdk-0.0.0.post0/etabs_sdk/src/enums.py
--rw-rw-rw-   0        0        0    10542 2024-04-17 15:48:26.000000 etabs_sdk-0.0.0.post0/etabs_sdk/src/etabs.py
--rw-rw-rw-   0        0        0     1151 2024-01-26 20:28:53.000000 etabs_sdk-0.0.0.post0/etabs_sdk/src/excepciones.py
-drwxrwxrwx   0        0        0        0 2024-04-17 15:55:41.950509 etabs_sdk-0.0.0.post0/etabs_sdk.egg-info/
--rw-rw-rw-   0        0        0     3629 2024-04-17 15:55:41.000000 etabs_sdk-0.0.0.post0/etabs_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2024-04-17 15:55:41.000000 etabs_sdk-0.0.0.post0/etabs_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 15:55:41.000000 etabs_sdk-0.0.0.post0/etabs_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2024-04-17 15:55:41.000000 etabs_sdk-0.0.0.post0/etabs_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-17 15:55:41.000000 etabs_sdk-0.0.0.post0/etabs_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2384 2024-04-17 14:47:57.000000 etabs_sdk-0.0.0.post0/pyproject.toml
--rw-rw-rw-   0        0        0      264 2024-04-17 14:47:25.000000 etabs_sdk-0.0.0.post0/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-04-17 15:55:41.947510 etabs_sdk-0.0.0.post0/scripts/
--rw-rw-rw-   0        0        0      685 2024-04-17 15:42:23.000000 etabs_sdk-0.0.0.post0/scripts/main.py
--rw-rw-rw-   0        0        0      737 2024-04-17 15:00:39.000000 etabs_sdk-0.0.0.post0/scripts/rescata_reacciones.py
--rw-rw-rw-   0        0        0       42 2024-04-17 15:55:41.953508 etabs_sdk-0.0.0.post0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-17 15:55:41.948509 etabs_sdk-0.0.0.post0/tests/
--rw-rw-rw-   0        0        0       31 2024-01-26 19:58:15.000000 etabs_sdk-0.0.0.post0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 20:44:19.000597 etabs_sdk-0.0.1.post0/
+-rw-rw-rw-   0        0        0      171 2024-01-26 16:52:56.000000 etabs_sdk-0.0.1.post0/.editorconfig
+-rw-rw-rw-   0        0        0     3108 2024-04-17 20:40:25.000000 etabs_sdk-0.0.1.post0/.gitignore
+-rw-rw-rw-   0        0        0     2597 2024-04-17 14:08:02.000000 etabs_sdk-0.0.1.post0/LICENSE
+-rw-rw-rw-   0        0        0     3629 2024-04-17 20:44:18.999600 etabs_sdk-0.0.1.post0/PKG-INFO
+-rw-rw-rw-   0        0        0       71 2024-04-17 14:14:35.000000 etabs_sdk-0.0.1.post0/README.md
+-rw-rw-rw-   0        0        0      639 2024-04-17 14:48:31.000000 etabs_sdk-0.0.1.post0/dev-requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 20:44:18.974597 etabs_sdk-0.0.1.post0/etabs_sdk/
+-rw-rw-rw-   0        0        0      154 2024-04-17 20:40:25.000000 etabs_sdk-0.0.1.post0/etabs_sdk/__init__.py
+-rw-rw-rw-   0        0        0      433 2024-04-17 20:44:18.000000 etabs_sdk-0.0.1.post0/etabs_sdk/_version.py
+drwxrwxrwx   0        0        0        0 2024-04-17 20:44:18.986601 etabs_sdk-0.0.1.post0/etabs_sdk/src/
+-rw-rw-rw-   0        0        0      787 2024-04-17 20:40:25.000000 etabs_sdk-0.0.1.post0/etabs_sdk/src/enums.py
+-rw-rw-rw-   0        0        0    11215 2024-04-17 20:40:25.000000 etabs_sdk-0.0.1.post0/etabs_sdk/src/etabs.py
+-rw-rw-rw-   0        0        0     1151 2024-01-26 20:28:53.000000 etabs_sdk-0.0.1.post0/etabs_sdk/src/excepciones.py
+drwxrwxrwx   0        0        0        0 2024-04-17 20:44:18.998596 etabs_sdk-0.0.1.post0/etabs_sdk.egg-info/
+-rw-rw-rw-   0        0        0     3629 2024-04-17 20:44:18.000000 etabs_sdk-0.0.1.post0/etabs_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2024-04-17 20:44:18.000000 etabs_sdk-0.0.1.post0/etabs_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 20:44:18.000000 etabs_sdk-0.0.1.post0/etabs_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2024-04-17 20:44:18.000000 etabs_sdk-0.0.1.post0/etabs_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-17 20:44:18.000000 etabs_sdk-0.0.1.post0/etabs_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2384 2024-04-17 14:47:57.000000 etabs_sdk-0.0.1.post0/pyproject.toml
+-rw-rw-rw-   0        0        0      264 2024-04-17 14:47:25.000000 etabs_sdk-0.0.1.post0/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 20:44:18.995597 etabs_sdk-0.0.1.post0/scripts/
+-rw-rw-rw-   0        0        0      742 2024-04-17 20:40:25.000000 etabs_sdk-0.0.1.post0/scripts/main.py
+-rw-rw-rw-   0        0        0      737 2024-04-17 15:00:39.000000 etabs_sdk-0.0.1.post0/scripts/rescata_reacciones.py
+-rw-rw-rw-   0        0        0       42 2024-04-17 20:44:19.001598 etabs_sdk-0.0.1.post0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 20:44:18.996599 etabs_sdk-0.0.1.post0/tests/
+-rw-rw-rw-   0        0        0       31 2024-01-26 19:58:15.000000 etabs_sdk-0.0.1.post0/tests/__init__.py
```

### Comparing `etabs_sdk-0.0.0.post0/.gitignore` & `etabs_sdk-0.0.1.post0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -153,7 +153,11 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+
+dist/
+secrets.txt
+edificio_prueba/
```

### Comparing `etabs_sdk-0.0.0.post0/LICENSE` & `etabs_sdk-0.0.1.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `etabs_sdk-0.0.0.post0/PKG-INFO` & `etabs_sdk-0.0.1.post0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etabs-sdk
-Version: 0.0.0.post0
+Version: 0.0.1.post0
 Summary: SDK para gestionar las comunicaciones con la API de Etabs con Python
 Author-email: Matías Glasner Vivanco <mglasner@iec.cl>, José Luis Barrios <jlbarrios@iec.cl>, Jorge Araya Varela <jaraya@iec.cl>
 License: Acuerdo de Licencia de Software de Código Abierto para etabs-sdk
         
         Propiedad Intelectual
         Este software y la documentación acompañante (en adelante, "el Software") están disponibles bajo los términos de esta Licencia de Código Abierto, la cual es administrada por IEC Ingeniería SA (en adelante, "la Empresa"). Aunque el Software es de código abierto, ciertos elementos pueden estar protegidos por derechos de autor u otros avisos de propiedad intelectual.
```

### Comparing `etabs_sdk-0.0.0.post0/dev-requirements.txt` & `etabs_sdk-0.0.1.post0/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `etabs_sdk-0.0.0.post0/etabs_sdk/src/etabs.py` & `etabs_sdk-0.0.1.post0/etabs_sdk/src/etabs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 """Etabs api."""
 
 import contextlib
-from ctypes import ArgumentError
 from pathlib import Path
 from typing import Any
 
 import comtypes
 import comtypes.client
 from tabulate import tabulate
 
-from .enums import LoadPatternType, Unidades
+from .enums import CasoOCombinacion, LoadPatternType, TipoDeCombinacion, Unidades
 from .excepciones import InstanciaActivaNoEncontradaError, ModeloNoEncontradoError, NuevoModeloError
 
 
 class Etabs:
     """Maneja la comunicación con la API de Etabs."""
 
-    def __init__(self, cerrar_intancia_abierta: bool = False, adjuntar_a_instancia: bool = False) -> None:
+    def __init__(self, cerrar_intancia_abierta: bool | None = None, adjuntar_a_instancia: bool | None = None) -> None:
         """Método init para la case Etabs."""
+        if cerrar_intancia_abierta is None:
+            cerrar_intancia_abierta = False
+
+        if adjuntar_a_instancia is None:
+            adjuntar_a_instancia = False
+
         self.etabs_object = self._conectar_etabs(cerrar_intancia_abierta, adjuntar_a_instancia)
         self.model = self.etabs_object.SapModel
 
     def _conectar_etabs(self, cerrar_instancia_abierta: bool, adjuntar_a_instancia: bool) -> Any:
         """Conectar al modelo indicado o a la instancia activa."""
         if cerrar_instancia_abierta:
             with contextlib.suppress(OSError, comtypes.COMError):
@@ -232,7 +237,18 @@
             value = self.model.LoadPatterns.Add(name, load_pattern_type, multiplier, add_case)
             if value != 0:
                 raise ValueError(f"The load pattern could not be added: {name}")
 
         except Exception as error:
             # sourcery skip: raise-specific-error
             raise Exception from error
+
+    def agregar_combinacion(
+        self,
+        nombre_combinacion: str,
+        tipo_de_combinacion: TipoDeCombinacion,
+        estados_de_carga: list[tuple[str, float, CasoOCombinacion]],
+    ) -> None:
+        """Agregar una nueva combinacion de cargas."""
+        self.model.RespCombo.Add(nombre_combinacion, tipo_de_combinacion)
+        for nombre_ec, factor, tipo in estados_de_carga:
+            self.model.RespCombo.SetCaseList(nombre_combinacion, tipo, nombre_ec, factor)
```

### Comparing `etabs_sdk-0.0.0.post0/etabs_sdk/src/excepciones.py` & `etabs_sdk-0.0.1.post0/etabs_sdk/src/excepciones.py`

 * *Files identical despite different names*

### Comparing `etabs_sdk-0.0.0.post0/etabs_sdk.egg-info/PKG-INFO` & `etabs_sdk-0.0.1.post0/etabs_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etabs-sdk
-Version: 0.0.0.post0
+Version: 0.0.1.post0
 Summary: SDK para gestionar las comunicaciones con la API de Etabs con Python
 Author-email: Matías Glasner Vivanco <mglasner@iec.cl>, José Luis Barrios <jlbarrios@iec.cl>, Jorge Araya Varela <jaraya@iec.cl>
 License: Acuerdo de Licencia de Software de Código Abierto para etabs-sdk
         
         Propiedad Intelectual
         Este software y la documentación acompañante (en adelante, "el Software") están disponibles bajo los términos de esta Licencia de Código Abierto, la cual es administrada por IEC Ingeniería SA (en adelante, "la Empresa"). Aunque el Software es de código abierto, ciertos elementos pueden estar protegidos por derechos de autor u otros avisos de propiedad intelectual.
```

### Comparing `etabs_sdk-0.0.0.post0/pyproject.toml` & `etabs_sdk-0.0.1.post0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `etabs_sdk-0.0.0.post0/scripts/rescata_reacciones.py` & `etabs_sdk-0.0.1.post0/scripts/rescata_reacciones.py`

 * *Files identical despite different names*

