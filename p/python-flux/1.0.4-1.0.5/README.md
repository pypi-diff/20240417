# Comparing `tmp/python_flux-1.0.4.tar.gz` & `tmp/python_flux-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_flux-1.0.4.tar", max compression
+gzip compressed data, was "python_flux-1.0.5.tar", max compression
```

## Comparing `python_flux-1.0.4.tar` & `python_flux-1.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     6282 2024-04-14 14:45:54.103087 python_flux-1.0.4/README.rst
--rw-r--r--   0        0        0      741 2024-04-14 14:51:59.413601 python_flux-1.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-1.0.4/python_flux/__init__.py
--rw-r--r--   0        0        0    15271 2024-04-14 14:19:20.119928 python_flux-1.0.4/python_flux/flux.py
--rw-r--r--   0        0        0      703 2024-04-14 03:28:17.497751 python_flux-1.0.4/python_flux/flux_utilis.py
--rw-r--r--   0        0        0     1596 2024-04-14 04:36:37.930223 python_flux-1.0.4/python_flux/producers.py
--rw-r--r--   0        0        0     1246 2024-04-14 03:28:17.498326 python_flux-1.0.4/python_flux/subscribers.py
--rw-r--r--   0        0        0     7013 1970-01-01 00:00:00.000000 python_flux-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     6355 2024-04-17 01:58:32.999118 python_flux-1.0.5/README.rst
+-rw-r--r--   0        0        0      741 2024-04-17 02:00:40.891529 python_flux-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-1.0.5/python_flux/__init__.py
+-rw-r--r--   0        0        0    15602 2024-04-17 02:33:29.437540 python_flux-1.0.5/python_flux/flux.py
+-rw-r--r--   0        0        0      768 2024-04-17 01:57:13.061985 python_flux-1.0.5/python_flux/flux_utilis.py
+-rw-r--r--   0        0        0     1596 2024-04-14 04:36:37.930223 python_flux-1.0.5/python_flux/producers.py
+-rw-r--r--   0        0        0     1348 2024-04-17 01:56:35.567056 python_flux-1.0.5/python_flux/subscribers.py
+-rw-r--r--   0        0        0     7086 1970-01-01 00:00:00.000000 python_flux-1.0.5/PKG-INFO
```

### Comparing `python_flux-1.0.4/README.rst` & `python_flux-1.0.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,16 @@
 
 Itera sobre los elementos del flujo e invoca a funciones **on_success** y on_error dependiendo el estado del flujo.
 
 -  **on_success**: función(valor, contexto) se invoca si el flujo procesa correctamente un valor
 
 -  **on_error**: función(ex, contexto) se invoca si hay un error en el flujo. Esto no corta el procesamiento a menos que se lance una excepción en el método
 
+-  **on_finish**: función(contexto) se invoca cuando el flujo finaliza
+
 -  **context**: Contexto inicial para el flujo
 
 
 to_list(context={})
 -------------------
 
 Itera sobre los elementos del flujo y los retorna todos dentro de una lista.
```

### Comparing `python_flux-1.0.4/pyproject.toml` & `python_flux-1.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-flux"
-version = "1.0.4"
+version = "1.0.5"
 description = "Librería que utiliza generadores de python para simular procesamiento de flujo de datos"
 authors = ["Juan Pablo Bochard <jbochard@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.rst"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `python_flux-1.0.4/python_flux/flux.py` & `python_flux-1.0.5/python_flux/flux.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,22 +49,23 @@
         Recibe una función(valor, contexto) que se evaluará para cada elemento del flujo original y retornará un
         flujo cuyos elementos se usarán como nuevo origen del flujo de datos.
 
         flatmap_function: función(valor, contexto) desde donde se obtendrá el valor a subsituir.
         """
         return FFlatMap(flatmap_function, self)
 
-    def do_on_next(self, on_next):
+    def do_on_next(self, on_next, on_error=fu.default_action):
         """
         Ejecuta par cada elemento del flujo una acción de forma asincrónica. No afecta a los valores
         del flujo.
 
-        :param on_next: función(valor, contexto) que se ejecutará para cada valor del flujo
+        :param on_next: función(valor, contexto) se ejecuta para cada valor del flujo
+        :param on_error: función(ex, contexto) se ejecuta en caso de error
         """
-        return FDoOnNext(on_next, self)
+        return FDoOnNext(on_next, on_error, self)
 
     def delay_ms(self, delay_ms, predicate=fu.default_predicate):
         """
         Retrasa en delay milisegundos la ejecución de paso del flujo. Esto marca el tiempo en que
         se procesarán sus elementos.
 
         :param delay_ms: Delay en milisegundos que se retrasará el procesamiento de los elementos del flujo
@@ -140,21 +141,22 @@
         Crea un objeto iterable a partir del flujo. Si se itera sobre este objeto se obtendrán
         los valores del flujo.
         :param context: Contexto inicial para el flujo
         :return: Objeto iterable
         """
         return SSubscribe(context, self)
 
-    def foreach(self, on_success=fu.default_success, on_error=fu.default_error, context={}):
+    def foreach(self, on_success=fu.default_success, on_error=fu.default_error, on_finish=fu.default_finish, context={}):
         """
         Itera sobre los elementos del flujo e invoca a funciones on_success y on_error dependiendo
         el estado del flujo.
         :param on_success: función(valor, contexto) se invoca si el flujo procesa correctamente un valor
         :param on_error:  función(ex, contexto) se invoca si hay un error en el flujo.
                           Esto no corta el procesamiento a menos que se lance una excepción en el método
+        :param on_finish: función(contexto) se invoca al finalizar el flujo
         :param context: Contexto inicial para el flujo
         """
         flux = self.subscribe(context)
         while True:
             try:
                 value = next(flux)
                 fu.try_or(partial(on_success), value, context)
@@ -395,17 +397,19 @@
         return value, e, ctx
 
 
 class FDoOnNext(Stream):
     async def __async_coroutine(self, f, value, context):
         f(value, context)
 
-    def __init__(self, func, flux):
+    def __init__(self, on_next, on_error, flux):
         super().__init__(flux)
-        self.function = func
+        self.on_next = on_next
+        self.on_error = on_error
 
     def next(self, context):
         value, e, ctx = super(FDoOnNext, self).next(context)
         if e is not None:
+            asyncio.run(self.__async_coroutine(self.on_error, e, ctx))
             return value, e, ctx
-        asyncio.run(self.__async_coroutine(self.function, value, ctx))
+        asyncio.run(self.__async_coroutine(self.on_next, value, ctx))
         return value, e, ctx
```

### Comparing `python_flux-1.0.4/python_flux/flux_utilis.py` & `python_flux-1.0.5/python_flux/flux_utilis.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,13 +20,17 @@
 
     @staticmethod
     def default_error(e, context):
         traceback.print_exception(type(e), e, e.__traceback__)
         raise e
 
     @staticmethod
+    def default_finish(context):
+        pass
+
+    @staticmethod
     def try_or(statement, value, ctx) -> (object, Exception):
         try:
             v = statement(value, ctx)
             return v, None
         except Exception as ex:
             return None, ex
```

### Comparing `python_flux-1.0.4/python_flux/producers.py` & `python_flux-1.0.5/python_flux/producers.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.0.4/python_flux/subscribers.py` & `python_flux-1.0.5/python_flux/subscribers.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,25 +21,27 @@
         if e is not None:
             raise e
         self.context = merge(self.context, ctx)
         return value
 
 
 class SForeach(object):
-    def __init__(self, on_success, on_error, ctx, f):
+    def __init__(self, on_success, on_error, on_finish, ctx, f):
         self.on_success = on_success
         self.on_error = on_error
+        self.on_finish = on_finish
         self.context = ctx
         self.flux = f
 
     def __next__(self):
         while True:
             self.flux.prepare_next()
             value, e, ctx = self.flux.next(self.context)
             if e is not None and isinstance(e, StopIteration):
+                fu.try_or(partial(self.on_finish), ctx)
                 raise e
             elif e is not None:
                 fu.try_or(partial(self.on_error), e, ctx)
             else:
                 fu.try_or(partial(self.on_success), value, ctx)
             self.context = merge(self.context, ctx)
             return value
```

### Comparing `python_flux-1.0.4/PKG-INFO` & `python_flux-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-flux
-Version: 1.0.4
+Version: 1.0.5
 Summary: Librería que utiliza generadores de python para simular procesamiento de flujo de datos
 License: GPL-3.0-or-later
 Author: Juan Pablo Bochard
 Author-email: jbochard@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -154,14 +154,16 @@
 
 Itera sobre los elementos del flujo e invoca a funciones **on_success** y on_error dependiendo el estado del flujo.
 
 -  **on_success**: función(valor, contexto) se invoca si el flujo procesa correctamente un valor
 
 -  **on_error**: función(ex, contexto) se invoca si hay un error en el flujo. Esto no corta el procesamiento a menos que se lance una excepción en el método
 
+-  **on_finish**: función(contexto) se invoca cuando el flujo finaliza
+
 -  **context**: Contexto inicial para el flujo
 
 
 to_list(context={})
 -------------------
 
 Itera sobre los elementos del flujo y los retorna todos dentro de una lista.
```

