# Comparing `tmp/tipo-kgen-0.0.1.tar.gz` & `tmp/tipo-kgen-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tipo-kgen-0.0.1.tar", last modified: Wed Apr 17 17:29:04 2024, max compression
+gzip compressed data, was "tipo-kgen-0.0.2.tar", last modified: Wed Apr 17 17:48:05 2024, max compression
```

## Comparing `tipo-kgen-0.0.1.tar` & `tipo-kgen-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 17:29:04.457882 tipo-kgen-0.0.1/
--rw-rw-rw-   0        0        0      386 2024-04-17 17:29:04.456878 tipo-kgen-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      144 2024-04-17 17:13:19.000000 tipo-kgen-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 17:29:04.435855 tipo-kgen-0.0.1/kgen/
--rw-rw-rw-   0        0        0        0 2024-04-17 15:02:12.000000 tipo-kgen-0.0.1/kgen/__init__.py
--rw-rw-rw-   0        0        0     4111 2024-04-17 15:02:12.000000 tipo-kgen-0.0.1/kgen/formatter.py
--rw-rw-rw-   0        0        0     4379 2024-04-17 17:13:55.000000 tipo-kgen-0.0.1/kgen/generate.py
--rw-rw-rw-   0        0        0     1153 2024-04-17 15:02:12.000000 tipo-kgen-0.0.1/kgen/logging.py
--rw-rw-rw-   0        0        0      876 2024-04-17 15:02:12.000000 tipo-kgen-0.0.1/kgen/metainfo.py
--rw-rw-rw-   0        0        0     2484 2024-04-17 15:02:12.000000 tipo-kgen-0.0.1/kgen/models.py
-drwxrwxrwx   0        0        0        0 2024-04-17 17:29:04.443859 tipo-kgen-0.0.1/kgen/tag-list/
--rw-rw-rw-   0        0        0        0 2024-04-17 16:47:26.000000 tipo-kgen-0.0.1/kgen/tag-list/__init__.py
--rw-rw-rw-   0        0        0  4459440 2024-04-17 15:02:11.000000 tipo-kgen-0.0.1/kgen/tag-list/artist.txt
--rw-rw-rw-   0        0        0  4079093 2024-04-17 15:02:11.000000 tipo-kgen-0.0.1/kgen/tag-list/characters.txt
--rw-rw-rw-   0        0        0   823337 2024-04-17 15:02:11.000000 tipo-kgen-0.0.1/kgen/tag-list/copyrights.txt
--rw-rw-rw-   0        0        0     8830 2024-04-17 15:02:11.000000 tipo-kgen-0.0.1/kgen/tag-list/meta.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 17:29:04.457882 tipo-kgen-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      603 2024-04-17 17:29:00.000000 tipo-kgen-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 17:29:04.455878 tipo-kgen-0.0.1/tipo_kgen.egg-info/
--rw-rw-rw-   0        0        0      386 2024-04-17 17:29:04.000000 tipo-kgen-0.0.1/tipo_kgen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      446 2024-04-17 17:29:04.000000 tipo-kgen-0.0.1/tipo_kgen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 17:29:04.000000 tipo-kgen-0.0.1/tipo_kgen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-17 17:29:04.000000 tipo-kgen-0.0.1/tipo_kgen.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2024-04-17 17:29:04.000000 tipo-kgen-0.0.1/tipo_kgen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-17 17:29:04.000000 tipo-kgen-0.0.1/tipo_kgen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 17:48:05.184518 tipo-kgen-0.0.2/
+-rw-rw-rw-   0        0        0      386 2024-04-17 17:48:05.183519 tipo-kgen-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      144 2024-04-17 17:13:19.000000 tipo-kgen-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 17:48:05.160031 tipo-kgen-0.0.2/kgen/
+-rw-rw-rw-   0        0        0        0 2024-04-17 15:02:12.000000 tipo-kgen-0.0.2/kgen/__init__.py
+-rw-rw-rw-   0        0        0     4111 2024-04-17 15:02:12.000000 tipo-kgen-0.0.2/kgen/formatter.py
+-rw-rw-rw-   0        0        0     4379 2024-04-17 17:13:55.000000 tipo-kgen-0.0.2/kgen/generate.py
+-rw-rw-rw-   0        0        0     1153 2024-04-17 17:47:41.000000 tipo-kgen-0.0.2/kgen/logging.py
+-rw-rw-rw-   0        0        0      876 2024-04-17 15:02:12.000000 tipo-kgen-0.0.2/kgen/metainfo.py
+-rw-rw-rw-   0        0        0     2484 2024-04-17 15:02:12.000000 tipo-kgen-0.0.2/kgen/models.py
+drwxrwxrwx   0        0        0        0 2024-04-17 17:48:05.168542 tipo-kgen-0.0.2/kgen/tag-list/
+-rw-rw-rw-   0        0        0        0 2024-04-17 16:47:26.000000 tipo-kgen-0.0.2/kgen/tag-list/__init__.py
+-rw-rw-rw-   0        0        0  4459440 2024-04-17 15:02:11.000000 tipo-kgen-0.0.2/kgen/tag-list/artist.txt
+-rw-rw-rw-   0        0        0  4079093 2024-04-17 15:02:11.000000 tipo-kgen-0.0.2/kgen/tag-list/characters.txt
+-rw-rw-rw-   0        0        0   823337 2024-04-17 15:02:11.000000 tipo-kgen-0.0.2/kgen/tag-list/copyrights.txt
+-rw-rw-rw-   0        0        0     8830 2024-04-17 15:02:11.000000 tipo-kgen-0.0.2/kgen/tag-list/meta.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 17:48:05.184518 tipo-kgen-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      603 2024-04-17 17:47:55.000000 tipo-kgen-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 17:48:05.182515 tipo-kgen-0.0.2/tipo_kgen.egg-info/
+-rw-rw-rw-   0        0        0      386 2024-04-17 17:48:05.000000 tipo-kgen-0.0.2/tipo_kgen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      446 2024-04-17 17:48:05.000000 tipo-kgen-0.0.2/tipo_kgen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 17:48:05.000000 tipo-kgen-0.0.2/tipo_kgen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-17 17:29:04.000000 tipo-kgen-0.0.2/tipo_kgen.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2024-04-17 17:48:05.000000 tipo-kgen-0.0.2/tipo_kgen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-17 17:48:05.000000 tipo-kgen-0.0.2/tipo_kgen.egg-info/top_level.txt
```

### Comparing `tipo-kgen-0.0.1/kgen/formatter.py` & `tipo-kgen-0.0.2/kgen/formatter.py`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.1/kgen/generate.py` & `tipo-kgen-0.0.2/kgen/generate.py`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.1/kgen/logging.py` & `tipo-kgen-0.0.2/kgen/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         levelname = colored_record.levelname
         seq = self.COLORS.get(levelname, self.COLORS["RESET"])
         colored_record.levelname = f"{seq}{levelname}{self.COLORS['RESET']}"
         return super().format(colored_record)
 
 
 # Create a new logger
-logger = logging.getLogger("DanTagGen")
+logger = logging.getLogger("TOPI-KGen")
 logger.propagate = False
 
 # Add handler if we don't have one.
 if not logger.handlers:
     handler = logging.StreamHandler(sys.stdout)
     handler.setFormatter(
         ColoredFormatter(
```

### Comparing `tipo-kgen-0.0.1/kgen/metainfo.py` & `tipo-kgen-0.0.2/kgen/metainfo.py`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.1/kgen/models.py` & `tipo-kgen-0.0.2/kgen/models.py`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.1/kgen/tag-list/artist.txt` & `tipo-kgen-0.0.2/kgen/tag-list/artist.txt`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.1/kgen/tag-list/characters.txt` & `tipo-kgen-0.0.2/kgen/tag-list/characters.txt`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.1/kgen/tag-list/copyrights.txt` & `tipo-kgen-0.0.2/kgen/tag-list/copyrights.txt`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.1/kgen/tag-list/meta.txt` & `tipo-kgen-0.0.2/kgen/tag-list/meta.txt`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.1/setup.py` & `tipo-kgen-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="tipo-kgen",
     packages=find_packages(),
-    version="0.0.1",
+    version="0.0.2",
     license="Apache 2.0",
     url="https://github.com/KohakuBlueleaf/KGen",
     description=(
         "TIPO: Text to Image genration through "
         "text Presampling with LLMs for Optimal prompting"
     ),
     author="Shih-Ying Yeh(KohakuBlueLeaf)",
```

