# Comparing `tmp/symbolx-0.4.2.tar.gz` & `tmp/symbolx-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbolx-0.4.2.tar", last modified: Fri Jul 21 22:45:44 2023, max compression
+gzip compressed data, was "symbolx-0.4.3.tar", last modified: Wed Apr 17 21:56:45 2024, max compression
```

## Comparing `symbolx-0.4.2.tar` & `symbolx-0.4.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 cgaete    (1000) cgaete    (1000)        0 2023-07-21 22:45:44.825652 symbolx-0.4.2/
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     1069 2023-05-23 09:10:57.000000 symbolx-0.4.2/LICENSE
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     3090 2023-07-21 22:45:44.825652 symbolx-0.4.2/PKG-INFO
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     2227 2023-07-21 21:44:23.000000 symbolx-0.4.2/README.md
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)       38 2023-07-21 22:45:44.825652 symbolx-0.4.2/setup.cfg
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     1610 2023-07-21 22:44:42.000000 symbolx-0.4.2/setup.py
-drwxrwxr-x   0 cgaete    (1000) cgaete    (1000)        0 2023-07-21 22:45:44.825652 symbolx-0.4.2/symbolx/
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)      586 2023-07-21 22:44:51.000000 symbolx-0.4.2/symbolx/__init__.py
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)    12238 2023-05-23 09:10:57.000000 symbolx-0.4.2/symbolx/handler.py
-drwxrwxr-x   0 cgaete    (1000) cgaete    (1000)        0 2023-07-21 22:45:44.825652 symbolx-0.4.2/symbolx/parsers/
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)        0 2023-05-23 09:10:57.000000 symbolx-0.4.2/symbolx/parsers/__init__.py
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     4615 2023-05-23 09:10:57.000000 symbolx-0.4.2/symbolx/parsers/parser_csv.py
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     3395 2023-05-23 09:10:57.000000 symbolx-0.4.2/symbolx/parsers/parser_feather.py
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)    12426 2023-07-21 21:25:07.000000 symbolx-0.4.2/symbolx/parsers/parser_gdx.py
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     1388 2023-05-23 09:10:57.000000 symbolx-0.4.2/symbolx/settings.py
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)    54620 2023-05-23 09:10:57.000000 symbolx-0.4.2/symbolx/symbols.py
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     6725 2023-05-23 09:10:57.000000 symbolx-0.4.2/symbolx/utils.py
-drwxrwxr-x   0 cgaete    (1000) cgaete    (1000)        0 2023-07-21 22:45:44.825652 symbolx-0.4.2/symbolx.egg-info/
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     3090 2023-07-21 22:45:44.000000 symbolx-0.4.2/symbolx.egg-info/PKG-INFO
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)      410 2023-07-21 22:45:44.000000 symbolx-0.4.2/symbolx.egg-info/SOURCES.txt
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)        1 2023-07-21 22:45:44.000000 symbolx-0.4.2/symbolx.egg-info/dependency_links.txt
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)       35 2023-07-21 22:45:44.000000 symbolx-0.4.2/symbolx.egg-info/requires.txt
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)        8 2023-07-21 22:45:44.000000 symbolx-0.4.2/symbolx.egg-info/top_level.txt
-drwxrwxr-x   0 cgaete    (1000) cgaete    (1000)        0 2023-07-21 22:45:44.825652 symbolx-0.4.2/test/
--rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     3559 2023-06-16 18:52:39.000000 symbolx-0.4.2/test/test.py
+drwxr-xr-x   0 cgaete    (1000) cgaete    (1000)        0 2024-04-17 21:56:45.569210 symbolx-0.4.3/
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)     1069 2023-05-23 09:10:57.000000 symbolx-0.4.3/LICENSE
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)     3188 2024-04-17 21:56:45.569210 symbolx-0.4.3/PKG-INFO
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)     2227 2023-07-21 21:44:23.000000 symbolx-0.4.3/README.md
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)       38 2024-04-17 21:56:45.569210 symbolx-0.4.3/setup.cfg
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)     1613 2024-04-17 21:56:14.000000 symbolx-0.4.3/setup.py
+drwxr-xr-x   0 cgaete    (1000) cgaete    (1000)        0 2024-04-17 21:56:45.569210 symbolx-0.4.3/symbolx/
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)      869 2024-04-17 21:56:39.000000 symbolx-0.4.3/symbolx/__init__.py
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)    12242 2024-04-17 21:37:20.000000 symbolx-0.4.3/symbolx/handler.py
+drwxr-xr-x   0 cgaete    (1000) cgaete    (1000)        0 2024-04-17 21:56:45.569210 symbolx-0.4.3/symbolx/parsers/
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)        0 2023-05-23 09:10:57.000000 symbolx-0.4.3/symbolx/parsers/__init__.py
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)     4615 2023-05-23 09:10:57.000000 symbolx-0.4.3/symbolx/parsers/parser_csv.py
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)     3419 2024-04-17 21:37:20.000000 symbolx-0.4.3/symbolx/parsers/parser_feather.py
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)    14117 2024-04-17 21:37:20.000000 symbolx-0.4.3/symbolx/parsers/parser_gdx.py
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)     1131 2024-04-17 21:37:20.000000 symbolx-0.4.3/symbolx/settings.py
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)    69308 2024-04-17 21:37:20.000000 symbolx-0.4.3/symbolx/symbols.py
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)     6721 2024-04-17 21:37:20.000000 symbolx-0.4.3/symbolx/utils.py
+drwxr-xr-x   0 cgaete    (1000) cgaete    (1000)        0 2024-04-17 21:56:45.569210 symbolx-0.4.3/symbolx.egg-info/
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)     3188 2024-04-17 21:56:45.000000 symbolx-0.4.3/symbolx.egg-info/PKG-INFO
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)      410 2024-04-17 21:56:45.000000 symbolx-0.4.3/symbolx.egg-info/SOURCES.txt
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)        1 2024-04-17 21:56:45.000000 symbolx-0.4.3/symbolx.egg-info/dependency_links.txt
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)       38 2024-04-17 21:56:45.000000 symbolx-0.4.3/symbolx.egg-info/requires.txt
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)        8 2024-04-17 21:56:45.000000 symbolx-0.4.3/symbolx.egg-info/top_level.txt
+drwxr-xr-x   0 cgaete    (1000) cgaete    (1000)        0 2024-04-17 21:56:45.569210 symbolx-0.4.3/test/
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)     3559 2024-04-17 18:50:59.000000 symbolx-0.4.3/test/test.py
```

### Comparing `symbolx-0.4.2/LICENSE` & `symbolx-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `symbolx-0.4.2/PKG-INFO` & `symbolx-0.4.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbolx
-Version: 0.4.2
+Version: 0.4.3
 Summary:  Symbolx helps collecting several scenarios data such as multidimentional variables and parameters for reporting and visualization wiht help of karray
 Author: Carlos Gaete-Morales
 Author-email: cdgaete@gmail.com
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
@@ -13,14 +13,18 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: karray>=2024.3.7
+Requires-Dist: pyarrow
 
 # symbolx
 Dealling with multiple scenarios data?  This tool helps collecting several scenarios data such as multidimentional variables and parameters for reporting and visualization
 
 
 Initial setting to be able to collect scenarios info. The following example uses parser and loader for GAMS-dieterpy output. For CSV and Arrow file formats see the test folder in https://gitlab.com/diw-evu/symbolx/-/tree/main/test
```

### Comparing `symbolx-0.4.2/README.md` & `symbolx-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `symbolx-0.4.2/setup.py` & `symbolx-0.4.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,23 +15,23 @@
         pkg = dirpath.replace(os.path.sep, ".")
         if os.path.altsep:
             pkg = pkg.replace(os.path.altsep, ".")
         packages.append(pkg)
 
 setup(
     name="symbolx",
-    version="0.4.2",
+    version="0.4.3",
     packages=packages,
     author="Carlos Gaete-Morales",
     author_email="cdgaete@gmail.com",
     install_requires=[
         "numpy",
         "pandas",
+        "karray >= 2024.3.7",
         "pyarrow",
-        "karray >= 0.3.1",
     ],
     include_package_data=True,
     long_description=long_description,
     long_description_content_type="text/markdown",
     description=" Symbolx helps collecting several scenarios data such as multidimentional variables and parameters for reporting and visualization wiht help of karray",
     classifiers=[
         "Intended Audience :: Science/Research",
```

### Comparing `symbolx-0.4.2/symbolx/__init__.py` & `symbolx-0.4.3/symbolx/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # symbolx
 # copyright 2022, Carlos Gaete-Morales, DIW-Berlin 
 """
     symbolx
     copyright 2022, Carlos Gaete-Morales, DIW-Berlin 
 """
-__version__ = (0, 4, 2)
+__version__ = (0, 4, 3)
 __author__ = 'Carlos Gaete-Morales'
+__all__ = ['DataCollection', 'SymbolsHandler', 'Symbol', 'from_feather',
+           'compress_subdirs', 'compress_dir', 'unzip_all', 'unzip',
+           'symbol_parser_csv', 'load_csv', 'symbol_parser_feather', 'load_feather',
+           'symbol_parser_gdx', 'load_gdx', 'settings']
 
 
 from .parsers.parser_csv import symbol_parser_csv, load_csv
 from .parsers.parser_feather import symbol_parser_feather, load_feather
 from .parsers.parser_gdx import symbol_parser_gdx, load_gdx
 from .handler import DataCollection
 from .utils import compress_subdirs, compress_dir, unzip_all, unzip
```

### Comparing `symbolx-0.4.2/symbolx/handler.py` & `symbolx-0.4.3/symbolx/handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         pattern = re.compile(r"(\d+)", re.IGNORECASE)
         names = []
         numbs = []
         shortnames = {}
         for scen in self.config:
             name = scen
             names.append(name)
-            if pattern.search(name) != None:
+            if pattern.search(name) is not None:
                 numbs.append(int(pattern.search(name)[0]))
             else:
                 flag = True
         nrmax = max(numbs)
         for i in range(1,11):
             result = nrmax//10**i
             if result <= 1:
```

### Comparing `symbolx-0.4.2/symbolx/parsers/parser_csv.py` & `symbolx-0.4.3/symbolx/parsers/parser_csv.py`

 * *Files identical despite different names*

### Comparing `symbolx-0.4.2/symbolx/parsers/parser_feather.py` & `symbolx-0.4.3/symbolx/parsers/parser_feather.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,18 +56,18 @@
         with_ = "pandas"
     if zip_extension is not None:
         path_parts = path.split(zip_extension+os.sep)
         zip_fpath = path_parts[0] + zip_extension
         target_fpath = path_parts[1]
         with zipfile.ZipFile(zip_fpath, mode="r") as zip_io:
             with zip_io.open(target_fpath) as the_file:
-                arr = ka._from_feather(the_file, use_threads=threads, with_=with_)
-        return arr
+                arr_dict = ka.from_feather_to_dict(the_file, use_threads=threads, with_=with_)
+        return arr_dict
     else:
-        return ka._from_feather(path, use_threads=threads, with_=with_)
+        return ka.from_feather_to_dict(path, use_threads=threads, with_=with_)
 
 def _info_feather(path:str, tool_name:str):
     '''
     Load symbol info from feather file.
     '''
     import pyarrow.feather as ft
     table = ft.read_table(path)
```

### Comparing `symbolx-0.4.2/symbolx/parsers/parser_gdx.py` & `symbolx-0.4.3/symbolx/parsers/parser_gdx.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,48 +88,60 @@
         zip_fpath = path_parts[0] + zip_extension
         target_fpath = path_parts[1]
         with zipfile.ZipFile(zip_fpath, mode="r") as zip_io:
             listOfFileNames = zip_io.namelist()
             assert target_fpath in listOfFileNames
             with tempfile.TemporaryDirectory() as tmpdirname:
                 zip_io.extract(target_fpath, tmpdirname)
-                tempfile_path = os.path.join(tmpdirname,target_fpath)
+                tempfile_path = os.path.join(tmpdirname, target_fpath)
                 metadata = _gdx_get_symbol_data_dict(symbol_name=symbol_name, gdx_file=tempfile_path, gams_dir=gams_dir)
                 symbol = _gdx_get_symbol_array_str(symbol_name=symbol_name, gdx_file=tempfile_path, gams_dir=gams_dir)
                 nrdims = len(metadata['dims'])
-                col_index = nrdims + value_types[value_type]
-                raw_coo = symbol[:, list(range(nrdims)) + [col_index]]
+                if isinstance(symbol, np.ndarray):
+                    symbol = (symbol[:, :nrdims], symbol[:, nrdims:])
+                assert isinstance(symbol, tuple)
+                raw_index, raw_value = symbol
+                col_index = value_types[value_type]
+                value = raw_value[:, col_index]
+                value = value.astype(np.float64)
                 # Warning: gams2numpy pkg convert EPS to INF as 5e+300
                 if inf_to_zero:
-                    EPS = raw_coo[:, nrdims] == np.float64("5e+300")
-                    raw_coo[EPS, nrdims] = 0.0
+                    # Warning: gams2numpy pkg convert EPS to INF as 5e+300
+                    # to verify this open a gdx with gams studio and check the values
+                    EPS = value == np.float64("5e+300")
+                    value[EPS] = 0.0
                     if verbose:
                         if sum(EPS) > 0:
                             print('GAMS EPS to 0.0 changed')
-                value = raw_coo[:, nrdims].astype(float)
-                index = {dim: raw_coo[:,idx] for idx, dim in enumerate(metadata['dims'])}
+                index = {dim: raw_index[:, idx] for idx, dim in enumerate(metadata['dims'])}
                 coords = {dim: metadata['coords'][dim] for dim in metadata['dims']}
-                return {'data': (index, value),'coords': coords}
+            return {'data': (index, value), 'coords': coords}
     else:
         metadata = _gdx_get_symbol_data_dict(symbol_name=symbol_name, gdx_file=path, gams_dir=gams_dir)
         symbol = _gdx_get_symbol_array_str(symbol_name=symbol_name, gdx_file=path, gams_dir=gams_dir)
         nrdims = len(metadata['dims'])
-        col_index = nrdims + value_types[value_type]
-        raw_coo = symbol[:, list(range(nrdims)) + [col_index]]
+        if isinstance(symbol, np.ndarray):
+            symbol = (symbol[:, :nrdims], symbol[:, nrdims:])
+        assert isinstance(symbol, tuple)
+        raw_index, raw_value = symbol
+        col_index = value_types[value_type]
+        value = raw_value[:, col_index]
+        value = value.astype(np.float64)
         # Warning: gams2numpy pkg convert EPS to INF as 5e+300
         if inf_to_zero:
-            EPS = raw_coo[:, nrdims] == np.float64("5e+300")
-            raw_coo[EPS, nrdims] = 0.0
+            # Warning: gams2numpy pkg convert EPS to INF as 5e+300
+            # to verify this open a gdx with gams studio and check the values
+            EPS = value == np.float64("5e+300")
+            value[EPS] = 0.0
             if verbose:
                 if sum(EPS) > 0:
                     print('GAMS EPS to 0.0 changed')
-        value = raw_coo[:, nrdims].astype(float)
-        index = {dim: raw_coo[:,idx] for idx, dim in enumerate(metadata['dims'])}
+        index = {dim: raw_index[:, idx] for idx, dim in enumerate(metadata['dims'])}
         coords = {dim: metadata['coords'][dim] for dim in metadata['dims']}
-        return {'data': (index, value),'coords': coords}
+        return {'data': (index, value), 'coords': coords}
 
 def _symbols_list_from_gdx(filename: str = None, gams_dir: str = None):
     """ It returns a list of symbols' names contained in the GDX file
 
     Args:
         gams_dir (str, optional): GAMS.exe path, if None the API looks at environment variables. Defaults to None.
         filename (str, optional): GDX filename. Defaults to None.
@@ -148,15 +160,15 @@
             gdxOpenRead,
             gdxDataReadDone,
             new_gdxHandle_tp,
             gdxClose,
             gdxFree,
             GMS_SSSIZE,
         )
-    except:
+    except ImportError:
         from gams.core.gdx import (
             gdxSystemInfo,
             gdxSymbolInfo,
             gdxCreateD,
             gdxOpenRead,
             gdxDataReadDone,
             new_gdxHandle_tp,
@@ -174,23 +186,35 @@
         ret, name, nrdims, symb_type = gdxSymbolInfo(gdxHandle, symNr)
         symbols.append((name, symb_type, nrdims))
     gdxDataReadDone(gdxHandle)
     gdxClose(gdxHandle)
     gdxFree(gdxHandle)
     return symbols
 
-def _gdx_get_symbol_array_str(symbol_name: str, gdx_file: str,  gams_dir: str=None):
+def _gdx_get_symbol_array_str(symbol_name: str, gdx_file: str,  gams_dir: str = None):
     try:
-        from gams2numpy import Gams2Numpy
-    except:
-        from gams.numpy import Gams2Numpy
+        from gams2numpy import Gams2Numpy  # GAMS version < 43
+    except ImportError:
+        try:
+            from gams.numpy import Gams2Numpy  # GAMS version >= 43, 44,  < 45
+        except ImportError:
+            try:
+                from gams.transfer.numpy import Gams2Numpy  # GAMS version == 45
+            except ImportError:
+                try:
+                    from gams.core.numpy import Gams2Numpy  # GAMS version >= 46 (date 2024-04-01)
+                except ImportError:
+                    raise Exception(
+                        "Symbolx parser not implemented for GAMS above 46. Please, install an older version of GAMS")
 
     g2np = Gams2Numpy(gams_dir)
     uel_map = g2np.gdxGetUelList(gdx_file)
-    arr = g2np.gdxReadSymbolStr(gdx_file, symbol_name,uel_map)
+    # Below GAMS 44 arr is a numpy array with dims and values as columns
+    # from GAMS 45 arr is a tuple with two arrays: dimensions-coords numpy array and values numpy array
+    arr = g2np.gdxReadSymbolStr(gdx_file, symbol_name, uel_map)
     return arr
 
 def _gdx_get_symbol_data_dict(symbol_name: str, gdx_file: str, gams_dir: str=None):
 
     try:
         from gdxcc import (
             gdxSymbolInfo,
@@ -200,15 +224,15 @@
             gdxCreateD,
             gdxOpenRead,
             new_gdxHandle_tp,
             gdxClose,
             gdxFree,
             GMS_SSSIZE,
         )
-    except:
+    except ImportError:
         from gams.core.gdx import (
             gdxSymbolInfo,
             gdxFindSymbol,
             gdxSymbolGetDomainX,
             gdxSymbolInfoX,
             gdxCreateD,
             gdxOpenRead,
@@ -231,15 +255,23 @@
     _, NrRecs, _, description = gdxSymbolInfoX(gdxHandle, symidx)
     gdxClose(gdxHandle)
     gdxFree(gdxHandle)
 
     data = {}
     data['symbol'] = symbol_name
     data['dims'] = gdx_domain
-    data['coords'] = {dim: sorted(np.sort(_gdx_get_symbol_array_str(symbol_name=dim, gdx_file=gdx_file, gams_dir=gams_dir)[:,0])) for dim in gdx_domain}
+    data['coords'] = {}
+    for dim in gdx_domain:
+        indexes = _gdx_get_symbol_array_str(symbol_name=dim, gdx_file=gdx_file, gams_dir=gams_dir)
+        if isinstance(indexes, np.ndarray):
+            data['coords'][dim] = sorted(np.sort(indexes[:,0]))
+        elif isinstance(indexes, tuple):
+            data['coords'][dim] = sorted(np.sort(indexes[0][:,0]))
+        else:
+            raise Exception(f"Unknown indexes type: {type(indexes)} from dim {dim} and symbol {symbol_name} in file {gdx_file}")
     return data
 
 
 
 def find_gams():
     if platform.system() == "Linux":
         path = subprocess.check_output(['which', 'gams']).decode().rstrip('\n')
@@ -264,29 +296,29 @@
 def exists_gams(gams_dir):
     if gams_dir is None:
         return False, None
     else:
         if os.path.exists(gams_dir):
             path = os.path.join(gams_dir, 'gams')
             try:
-                script = subprocess.check_output([path]).decode().rstrip('\n')
+                _ = subprocess.check_output([path]).decode().rstrip('\n')
                 return True, gams_dir
             except FileNotFoundError:
                 return False, gams_dir
         else:
             return False, gams_dir
         
 def get_gams_dir(gams_dir):
     if gams_dir is None:
         ret, gams_dir = find_gams()
         if ret:
             print(f"Found gams in {gams_dir}")
             return ret, gams_dir
         else:
-            print(f'''
+            print('''
                   gams cannot be detected. Make sure you have gams installed. 
                   If gams is already installed, add gams_dir argument with the correct path to gams 
                   e.g. data_collection_instance.adquire(gams_dir="gams/path/here"); or
                   add gams directory to the PATH.
                   ''')
             return ret, gams_dir
     else:
```

### Comparing `symbolx-0.4.2/symbolx/settings.py` & `symbolx-0.4.3/symbolx/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,23 +12,18 @@
 
 class Settings:
     def __init__(self):
         self.name_value_type_token = {}
 
     def append(self, name_value_type_token:tuple):
         assert isinstance(name_value_type_token, tuple), "A tuple of symbol name, value_type, and symbol_handler_token must be provided."
-        assert name_value_type_token not in self.name_value_type_token, f"Symbol {name_value_type_token} already exists in a SymbolsHandler instance. Can not be loaded again."
-        self.name_value_type_token[name_value_type_token] = True
-
-    def exists(self, name_value_type_token:tuple):
-        assert isinstance(name_value_type_token, tuple), "Symbol name, value_type, and symbol_handler_token must be provided."
         if name_value_type_token in self.name_value_type_token:
-            return True
-        else:
-            return False
+            pass
+            # print(f"Warning:\nSymbol {name_value_type_token} already exists as a Symbol instance. Make sure that the symbol name is unique.")
+        self.name_value_type_token[name_value_type_token] = True
 
     def getnames(self):
         return self.name_value_type_token
 
 settings = Settings()
```

### Comparing `symbolx-0.4.2/symbolx/symbols.py` & `symbolx-0.4.3/symbolx/symbols.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 import glob
 import uuid
-import itertools
 import numpy as np
 import karray as ka
 import json
-from json import JSONDecodeError
-from typing import Union, List, Dict
+from typing import Union, List, Callable
+import pandas as pd
 from .handler import DataCollection
 from .settings import settings, allowed_string, value_type_name_map
 
-
+# TODO: update Metadata after an operation is done that may modify the symbols attributes coords
+# TODO: update metadata_union with union of coordinates also for symbols
 class SymbolsHandler:
-    def __init__(self, method:str, folder_path:str=None, obj:DataCollection=None):
+    def __init__(self, method:str, folder_path:str=None, obj:DataCollection=None, symbol_handler_token:str=None):
         ''' 
         Initialize SymbolsHandler object.
 
         Parameters
         ----------
         method : str
             The method used to collect raw variables or symbols. Two methods are available: 1. 'folder' - the symbols are collected from the folder specified by folder_path. 2. 'object' - the variables are collected from the object specified by obj which must be a DataCollection object.
@@ -34,36 +34,36 @@
         Build symbols from raw scenarios output (parser and loader from arrow tables and feather file format).
 
             >>> import symbolx as syx
             >>> from symbolx import DataCollection, SymbolsHandler
             >>> DC = DataCollection()
             >>> DC.add_collector(collector_name='opt_model', parser=syx.symbol_parser_feather, loader=syx.load_feather)
             >>> DC.add_folder(collector_name='opt_model', './raw_model_output')
-            >>> DC.add_custom_attr(collector_name='opt_model', with_='pandas')
+            >>> DC.add_custom_attr(collector_name='opt_model')
             >>> DC.adquire(id_integer=True, zip_extension=None)
             >>> SH = SymbolsHandler(method='object', obj=DC)
 
             
         Load symbols from folder.
 
-            >>> from symbolx import , SymbolsHandler
+            >>> from symbolx import SymbolsHandler
             >>> SH = SymbolsHandler(method='folder', folder_path='./symbols_files')
 
             
         '''
 
         assert isinstance(method, str), "Arg 'method' must be a string."
         assert method in ["folder", "object"], "Arg 'method' must be either 'folder' or 'object'"
         self.method = method
         self.folder_path = None
         self.symbols_book = None
-        self.symbol_handler_token = str(uuid.uuid4()) # TODO: this can be changed by hashing the input file
         self.saved_symbols = {}
         self.token_info = None
-        self.input_method(method=method, folder_path=folder_path, obj=obj)
+        # self.symbol_handler_token = None
+        self.input_method(method=method, folder_path=folder_path, obj=obj, symbol_handler_token=symbol_handler_token)
 
     def input_method(self, method:str, **kwargs):
         '''
         Input the method used to collect raw variables or symbols.
 
         Parameters
         ----------
@@ -79,21 +79,21 @@
         Returns
         -------
         None.
 
         '''
 
         if method == "object":
-            self.from_object(obj=kwargs['obj'])
+            self.from_object(obj=kwargs['obj'], symbol_handler_token=kwargs['symbol_handler_token'])
         elif method == "folder":
             self.from_folder(folder_path=kwargs['folder_path'])
         else:
             raise Exception('A method mus be provided from either "object" or "folder"')
 
-    def from_object(self, obj:DataCollection):
+    def from_object(self, obj:DataCollection, symbol_handler_token:str=None):
         '''
         Extracts information from the DataCollection object, such as variable name and value type. Value type can be either 'value', 'marginal', 'lower', or 'upper' as define in GAMS for variables.
 
         It also populates a dictionary with the variable name, value type and symbol_handler_token—A symbol_handler_token is generated per instance; this helps to avoid mixup variables of other problems.
 
         Parameters
         ----------
@@ -105,16 +105,22 @@
         None.
 
         '''
 
         self.symbols_book = obj.symbols_book
         self.collector = obj.collector
         self.short_names = obj.short_names
-        for n_v in self.symbols_book:
-            settings.append((*n_v,self.symbol_handler_token))
+
+        if symbol_handler_token is not None:
+            self.symbol_handler_token = symbol_handler_token
+        else:
+            self.symbol_handler_token = str(uuid.uuid4()) # TODO: this can be changed by hashing the input file
+
+        # for n_v in self.symbols_book:
+        #     settings.append((*n_v,self.symbol_handler_token))
 
 
     def from_folder(self, folder_path:str=None):
         '''
         Extracts information from the folder, such as variable name and value type of all symbols saved with extension 'feather'.
         
         Parameters 
@@ -134,25 +140,33 @@
         files = glob.glob(os.path.join(self.folder_path, "*.feather"))
         self.symbols_book = {}
         for file in files:
             loaded_file_dict = from_feather_info(file)
             self.symbols_book[(loaded_file_dict['name'],loaded_file_dict['value_type'])] = file
 
             token = loaded_file_dict['symbol_handler_token']
-            settings.append((loaded_file_dict['name'],loaded_file_dict['value_type'],loaded_file_dict['symbol_handler_token']))
+            # settings.append((loaded_file_dict['name'],loaded_file_dict['value_type'],loaded_file_dict['symbol_handler_token']))
 
             if token not in self.token_info:
                 self.token_info[token] = {}
             self.token_info[token][(loaded_file_dict['name'],loaded_file_dict['value_type'])] = file
-        if len(self.token_info) > 1:
+        if len(self.token_info) == 0:
+            print(f"No Symbols' files found in {folder_path}")
+            self.symbol_handler_token = None
+        elif len(self.token_info) == 1:
+            self.symbol_handler_token = list(self.token_info.keys())[0]
+        elif len(self.token_info) > 1:
+            # TODO: add this to logger
+            print("Warning:")
             print(f"There are Symbols' files with different symbol_handler_token in {folder_path}")
             print("       Symbol's scenario short names or id's might be in conflict.")
             print("       Make sure all Symbols are from the same symbol_handler_token")
             print("       Otherwise, it may happen, for example, different scenarios have the same id.")
             print("       See 'token_info' attribute of SymbolsHandler for more information")
+            self.symbol_handler_token = None
 
 
     def append(self, **kwargs):
         '''
         Store a symbol in a temporal container to posterior saving. The container can be accessed by the 'saved_symbols' attribute.
 
         Parameters
@@ -382,14 +396,15 @@
         self,
         name: str=                      None,
         value_type: str=                'v',
         metadata: dict=                 None,
         array: ka.Array=                None,
         symbol_handler_token: str=      None,
         symbol_handler: SymbolsHandler= None,
+        load_with:str=                  "pandas",
         ):
         '''
         Symbol constructor.
 
         Parameters
         ----------
         name : str
@@ -400,14 +415,16 @@
             Nested dictionary with metadata about the symbol. The structure is as follows: {'metadata_1': {1: 'metadata_1_value of scenario 1', 2: 'metadata_2_value of scenario 2'}, ...}
         array : karray.Array
             The symbol array. This must be provided if 'symbol_handler' is not provided.
         symbol_handler_token : str
             The symbol handler token. This must be provided if 'symbol_handler' is not provided.
         symbol_handler : SymbolsHandler
             The symbol handler instance that contains information about the variables and scenarios or the symbol file path.
+        load_with: str
+            Only when reading a symbolx feather file (When instantiating symbol_handler 'folder' option)
 
         Returns
         -------
         symbol : Symbol
             The symbol.
 
         Examples
@@ -431,31 +448,36 @@
             
         '''
         self.__dict__["_repo"] = {}
         if symbol_handler is not None:
             if 'object' == symbol_handler.method:
                 self.build(symbol_handler, name, value_type)
             elif 'folder' == symbol_handler.method:
-                self.load(symbol_handler, name, value_type)
+                self.load(symbol_handler, name, value_type, load_with)
         else:
-            if settings.exists((name,value_type,symbol_handler_token)):
-                print("The symbol name has already been taken by another Symbol stored in SymbolsHandler.")
-                print("Please choose another name to avoid overwriting the existing symbol when saving the current symbol.")
+            settings.append((name,value_type, symbol_handler_token))
             self.name=                 name
             self.value_type=           value_type
-            self.metadata=             metadata
             self.array=                array
+            self.metadata=             metadata
             self.symbol_handler_token= symbol_handler_token
         self.check_input()
         # optional attributes
         self.dataframe = None
 
 
     def __setattr__(self, name, value):
-        self._repo[name] = value
+        if name == "metadata":
+            ids = self._repo["array"].coords["id"]
+            metadata = {}
+            for attr in value:
+                metadata[attr] = {k: value[attr][k] for k in value[attr] if k in ids}
+            self._repo[name] = metadata
+        else:
+            self._repo[name] = value
 
     def __getattr__(self, name):
         if name.startswith('_'):
             raise AttributeError(name) # ipython requirement for repr_html
         if name == "dataframe":
             if name in self._repo:
                 if self._repo[name] is None:
@@ -464,15 +486,15 @@
                 else:
                     #Sanity check
                     df = self._repo[name]
                     dense = df.value.values.reshape(self.array.shape)
                     if np.allclose(dense, self.array.dense):
                         return df.copy()
                     else:
-                        print(f"Getting dataframe again...")
+                        print("Getting dataframe again...")
                         self._repo[name] = self.array.to_pandas()
                         return self._repo[name].copy()
             else:
                 self.definition_msg(name) # dev msg
         else:
             return self._repo[name]
 
@@ -500,21 +522,23 @@
         assert isinstance(name, str), "'name' must be a string"
         assert isinstance(value_type, str), "'value_type' must be a string"
         print(f"{name:<25} value_type: {value_type_name_map[value_type]} ({value_type})")
 
         key = (name,value_type)
         assert key in symbol_handler.symbols_book, f"'{key}' is not present in 'symbol_handler.symbols_book' dictionary"
 
+        settings.append((name, value_type, symbol_handler.symbol_handler_token))
         self.name=                 name
         self.value_type=           value_type
-        self.metadata=             symbol_handler.get_info(*key)['metadata']
         self.array=                build_array(name, value_type, symbol_handler)
+        self.metadata=             symbol_handler.get_info(*key)['metadata']
         self.symbol_handler_token= symbol_handler.symbol_handler_token
         
-    def load(self, symbol_handler:SymbolsHandler, name: str=None, value_type: str=None):
+        
+    def load(self, symbol_handler:SymbolsHandler, name: str=None, value_type: str=None, load_with:str="pandas"):
         '''
         Symbol is recreated from feather file. This method is used when the symbol handler is instantiated with 'folder' method providing the path of the symbol file.
 
         Parameters
         ----------
         symbol_handler : SymbolsHandler
             The symbol handler instance that contains information about the variables and scenarios. This method is used when the symbol handler is instantiated with 'folder' method.
@@ -535,20 +559,25 @@
         assert isinstance(value_type, str), "'value_type' must be a string"
         print(f"{name:<25} value_type: {value_type_name_map[value_type]} ({value_type})")
 
         key = (name,value_type)
         assert key in symbol_handler.symbols_book, f"'{key}' is not present in 'symbol_handler.symbols_book' dictionary"
 
         file_path = symbol_handler.get_info(*key)
-        symbol_dict = from_feather_dict(file_path, with_=ka.settings.feather_with)
+        symbol_dict = from_feather_dict(file_path, with_=load_with)
+        settings.append((name, value_type, symbol_dict['symbol_handler_token']))
         self.name=                 name
         self.value_type=           value_type
-        self.metadata=             symbol_dict['metadata']
         self.array=                symbol_dict['array']
+        self.metadata=             symbol_dict['metadata']
         self.symbol_handler_token= symbol_dict['symbol_handler_token']
+        
+    @property
+    def metadf(self):
+        return pd.DataFrame(self.metadata)
 
     def to_arrow(self):
         '''
         Convert the symbol to an arrow table with metadata. The symbol array contains karray array and the karray metadata. The returned table contains karray and symbox metadata as well.
 
         Returns
         -------
@@ -586,16 +615,17 @@
         None
 
         '''
 
         import pyarrow.feather as ft
         sets = set(allowed_string)
         sets.add(os.path.sep)
-        joint = ''.join(sorted(sets))
-        assert len(set(path).difference(sets)) == 0, f"There are/is special characters in path '{path}'. Allowed chars are: {joint}"
+        conflicting_path_chars = set(path).difference(sets)
+        if len(conflicting_path_chars) != 0:
+            print(f"The path {path} contains conflicting characters that may affect loading the file: {conflicting_path_chars}")
 
         table = self.to_arrow()
         ft.write_feather(table, path)
         print(f"{path}")
         return None
 
     def check_input(self):
@@ -603,19 +633,18 @@
         Check the input of the symbol. 
 
         Returns
         -------
         None
 
         '''
-
         assert self.name is not None and isinstance(self.name, str), "Name of symbol must be provided."
         assert self.value_type is not None and isinstance(self.value_type, str), "Value type of symbol must be provided."
-        assert self.metadata is not None and isinstance(self.metadata, dict), "metadata of symbol must be provided."
         assert self.array is not None and isinstance(self.array, ka.Array), "Array must be provided."
+        assert self.metadata is not None and isinstance(self.metadata, dict), "metadata of symbol must be provided."
         assert self.symbol_handler_token is not None and isinstance(self.symbol_handler_token, str), "Symbol handler token must be provided."
 
     @property
     def dims(self):
         '''
         Get the dimensions of the symbol.
 
@@ -634,19 +663,21 @@
 
         Returns
         -------
         df : pandas.DataFrame
             The multiindex dataframe of the symbol. Long data format.
 
         '''
-
-        return self.dataframe.set_index(self.array.dims)
+        if len(self.array.dims) == 0:
+            return self.dataframe
+        else:
+            return self.dataframe.set_index(self.array.dims)
 
     @property
-    def dfm(self):
+    def dfm(self) -> pd.DataFrame:
         '''
         Get the dataframe of the symbol with metadata as additional columns. Dimenssions coordinates are as columns.
 
         Returns
         -------
         dfm : pandas.DataFrame
             The dataframe of the symbol with long data format.
@@ -655,15 +686,15 @@
 
         dfm = self.dataframe
         for k, v in self.metadata.items():
             dfm[k] = dfm["id"].map(v)
         return dfm
 
     @property
-    def dfc(self):
+    def dfc(self) -> pd.DataFrame:
         '''
         Get the dataframe of the symbol with only custom metadata as additional columns. Dimenssions coordinates are as columns.
 
         Returns
         -------
         dfc : pandas.DataFrame
             The dataframe of the symbol with long data format.
@@ -672,14 +703,26 @@
 
         dfc = self.dataframe
         for k, v in self.metadata.items():
             if 'custom_' in k:
                 dfc[k] = dfc["id"].map(v)
         return dfc
     
+    @property
+    def summary(self):
+        summary = {}
+        for key,value in self.metadata.items():
+            collection = set(list(value.values()))
+            if None in collection:
+                meta_coords = collection
+            else:
+                meta_coords = sorted(collection)
+            summary[key] = meta_coords
+        return {key:value for key, value in summary.items() if key not in ["run", "long_id"]}
+    
     def to_polars(self):
         '''
         Convert the symbol to a polar data frame.
 
         Returns
         -------
         polar_df : polars.DataFrame
@@ -712,15 +755,14 @@
 
         Returns
         -------
         metadata : dict
             The union of the metadata of two symbols.
 
         '''
-
         self_metadata = self.metadata
         other_metadata = other.metadata
         new_metadata = {}
         for elem in self_metadata.keys():
             new_metadata[elem] = {**self_metadata[elem],**other_metadata[elem]}
         return new_metadata
 
@@ -938,15 +980,15 @@
         new_symbol : Symbol
             The new symbol.
 
         '''
 
         return self.new_symbol(self.array, new_name)
 
-    def dimreduc(self, dim:str='h', aggfunc=np.add.reduce):
+    def dimreduc(self, dim:str='h', aggfunc:Union[str,Callable]=np.add.reduce):
         '''
         Reduce one dimension of the symbol by applying a numpy ufunc over all coordinates of the dimension.
         
         Parameters
         ----------
         dim : str
             The dimension to reduce.
@@ -957,15 +999,18 @@
         -------
         new_symbol : Symbol
             The new symbol.
 
         '''
 
         new_array = self.array.reduce(dim, aggfunc)
-        new_name = f"({self.name}).dimreduc({dim},{aggfunc})"
+        if isinstance(aggfunc, str):
+            new_name = f"({self.name}).dimreduc({dim},{aggfunc})"
+        elif isinstance(aggfunc, Callable):
+            new_name = f"({self.name}).dimreduc({dim},{aggfunc.__name__})"
         return self.new_symbol(new_array, new_name)
 
     @property
     def items(self):
         '''
         Get the items of the symbol or coordinates.
 
@@ -989,15 +1034,15 @@
 
         Returns
         -------
         new_symbol : Symbol
             The new symbol.
 
         """
-
+        assert len(kwargs) > 0, "Must provide at least one keyword argument"
         new_array = self.array.rename(**kwargs)
         new_name = f"({self.name}).rename_dim(**{kwargs})"
         return self.new_symbol(new_array, new_name)
     
     def add_dim(self, dim_name: str, value: Union[str,int,dict]):
         '''
         Deprecated: Use add_dims instead.
@@ -1024,15 +1069,15 @@
             return self.new_symbol(new_array, new_name)
 
         elif isinstance(value, dict):
             new_array = self.array.add_dim(**{dim_name:value})
             new_name = f"({self.name}).add_dim({dim_name},{value})"
             return self.new_symbol(new_array, new_name)
         else:
-            raise Exception('value is neither str nor dict')
+            raise Exception('value is neither str, int or dict')
         
     def add_dims(self, **kwargs):
         '''
         Add a dimension to the symbol.
 
         Parameters
         ----------
@@ -1049,14 +1094,34 @@
             The new symbol.
 
         '''
 
         new_array = self.array.add_dim(**kwargs)
         new_name = f"({self.name}).add_dims({','.join(list(kwargs))})"
         return self.new_symbol(new_array, new_name)
+    
+    def expand(self, **kwargs):
+        '''
+        Broadcast array on the new dimenssions corrdinates.
+
+        Parameters
+        ----------
+        kwargs : dict
+            The keyword arguments must be new dimension names and the value arguments contain list of the new coordinates.
+
+        Returns
+        -------
+        new_symbol : Symbol
+            The new symbol.
+
+        '''
+
+        new_array = self.array.expand(**kwargs)
+        new_name = f"({self.name}).expand({'=[...],'.join(list(kwargs))})"
+        return self.new_symbol(new_array, new_name)    
 
     def dropna(self):
         '''
         Drop the NaN values from the symbol.
 
         Returns
         -------
@@ -1127,40 +1192,40 @@
 
         '''
 
         new_array = self.array.round(decimals=decimals)
         new_name = f"({self.name}).round({decimals=})"
         return self.new_symbol(new_array, new_name)
 
-    def elems_to_datetime(self, new_dim:str, actual_dim:str, reference_date:str='01-01-2030', freq:str='H', sort_corrds:bool=True):
+    def elems_to_datetime(self, new_dim:str, actual_dim:str, reference_date:str='01-01-2030', freq:str='H', sort_coords:bool=True):
         '''
         Convert the elements of the symbol to datetime.
 
         Parameters
         ----------
         new_dim : str
             The new dimension name.
         actual_dim : str
             The actual dimension name.
         reference_date : str
             The reference date.
         freq : str
             The frequency of the datetime.
-        sort_corrds : bool
+        sort_coords : bool
             If True, sort the coordinates of the symbol.
 
         Returns
         -------
         new_symbol : Symbol
             The new symbol.
 
         '''
 
-        new_array = self.array.elems_to_datetime(new_dim=new_dim, actual_dim=actual_dim, reference_date=reference_date, freq=freq, sort_coords=sort_corrds)
-        new_name = f"({self.name}).elems_to_datetime({new_dim}{actual_dim},{reference_date},{freq},{sort_corrds})"
+        new_array = self.array.elems_to_datetime(new_dim=new_dim, actual_dim=actual_dim, reference_date=reference_date, freq=freq, sort_coords=sort_coords)
+        new_name = f"({self.name}).elems_to_datetime({new_dim}{actual_dim},{reference_date},{freq},{sort_coords})"
         return self.new_symbol(new_array, new_name)
 
     def elems_to_int(self, new_dim:str, actual_dim:str):
         '''
         Convert the elements of the symbol to integers.
 
         Parameters
@@ -1179,14 +1244,16 @@
 
         new_array = self.array.elems_to_int(new_dim, actual_dim)
         new_name = f"({self.name}).elems_to_int({new_dim=},{actual_dim=})"
         return self.new_symbol(new_array, new_name)
 
     def find_ids(self, **kwargs):
         '''
+        DEPRECATED: Will be removed in future versions. Use get_id_query instead.
+        
         Find scenarios ids in a symbol that comply with the criteria given by the keyword arguments. Several criteria can be specified where the result would be the intersection of all criteria.
 
         Parameters
         ----------
         kwargs : dict
             The keyword arguments must be the following:
 
@@ -1332,23 +1399,28 @@
                 new_neg = []
                 for _ in range(len(kwargs)):
                     new_neg.append(neg)
                 neg = new_neg
         else:
             neg = [neg]
 
-        for key, value in kwargs.items():
+        for i, items in enumerate(kwargs.items()):
+            key, value = items
             if key in self.dims:
                 if set(value).issubset(self.items[key]):
                     pass
                 else:
                     not_present = set(value) - (set(value) & set(self.items[key]))
                     present = (set(value) & set(self.items[key]))
                     if len(present) == 0:
-                        raise Exception(f"{not_present} is/are not in {self.items[key]}")
+                        # raise Exception(f"{not_present} is/are not in {self.items[key]}")
+                        if not neg[i]:
+                            print(f"Symbol: {self.name}\n   Shrink works over 'id' dimension. The query identify ids: {not_present} is/are not present in the symbol. It will return an empty array. In Karray setting.fill_missing is by default False, which is evaluated as float(False), hence zero. In such case, this will return a full-zero array of the same shape. For more details, please refer _filler_and_dtype function in karray.")
+                        kwargs[key] = []
+
                     else:
                         # print(f"    Only {present} exist in {self.items[key]} and meet criteria at '{key}', while not {not_present}")
                         kwargs[key] = sorted(present)
             else:
                 raise Exception(f"'{key}' is not in {self.dims} for symbol {self.name}")
 
         right_kwargs = {k:v for k,v in kwargs.items()}
@@ -1391,24 +1463,23 @@
         --------
         >>> Z.shrink_by_attr(**{'run':[0,1], 'country_set':['NA']})
 
         >>> Z.shrink_by_attr(run=[0,1], country_set=['NA'])
 
         '''
         for key, value in kwargs.items():
-            dc = self.metadata
-            if key not in dc.keys():
-                raise Exception(f"'{key}' is not in {list(dc.keys())} for symbol {self.name}")
+            if key not in self.metadata:
+                raise Exception(f"'{key}' is not in {list(self.metadata.keys())} for symbol {self.name}")
         
-        id_list = sorted(set([item for sublist in list(self.create_mix(kwargs).values()) for item in sublist]))
+        id_list = self.get_id_query(query=' and '.join([f'{k} in {kwargs[k]}' for k in kwargs]))
         new_object = self.shrink(id=id_list, neg=neg)
-        new_object.name = f"(neg={neg},{self.name}).shrink_by_attr({','.join(['='.join([k,str(v)]) for k,v in kwargs.items()])})"
+        new_object.name = f"({self.name}).shrink_by_attr(neg={neg},{','.join(['='.join([k,str(v)]) for k,v in kwargs.items()])})"
         return new_object
 
-    def refdiff(self, reference_id:Union[int,str]=0):
+    def refdiff(self, reference_id:Union[int,str]):
         ''' 
         Returns the difference between the reference scenario (with its respective id) and the rest of the scenarios in a symbol. The symbol must have the dimension name 'id'.
         
         Parameters
         ----------
         reference_id : Union[int,str]
             The id of the reference scenario.
@@ -1420,64 +1491,64 @@
 
         Examples
         --------
 
         >>> Z.refdiff(reference_id='S0001')
         
         '''
-        new_object = self - self.shrink(id=[reference_id]).dimreduc('id')
-        new_object.name = f"({self.name}).refdiff({reference_id})"
-        return new_object
+        new_array = self.array - self.shrink(id=[reference_id]).array.reduce("id")
+        new_name = f"({self.name}).refdiff({reference_id})"
+        return self.new_symbol(new_array, new_name)
 
     def create_mix(self, criteria):
         ''' 
         Private function used for refdiff_by_sections.
         '''
+        pandas_group = pd.DataFrame(self.metadata).query(expr=' and '.join([f'{k} in {v}' for k,v in criteria.items()])).groupby(list(criteria))
+        return {name:pandas_group.get_group(name).index.tolist() for name in pandas_group.groups}
 
-        combination = self.create_combination(criteria)
-        order = criteria.keys()
-        return self._find_ids_by_tuple(order,combination)
-
-    def create_combination(self, criteria: dict):
-        '''
-        Private function used for refdiff_by_sections.
-        '''
-
-        return list(itertools.product(*criteria.values()))
-
+    # def create_combination(self, criteria: dict):
+    #     '''
+    #     Private function used for refdiff_by_sections.
+    #     '''
+
+    #     return list(itertools.product(*criteria.values()))
+
+
+    # def _find_ids_by_tuple(self,key_order,combination):
+    #     '''
+    #     Private function used for refdiff_by_sections.
+    #     '''
+
+    #     groups = {}
+    #     for i, pair in enumerate(combination):
+    #         config = {}
+    #         for k, v in zip(key_order, pair):
+    #             config[k] = ('==',v)
+    #         groups[i] = list(self.find_ids(**config))
+    #     return groups
 
-    def _find_ids_by_tuple(self,key_order,combination):
+    def _ref_diff_group(self, reference_groups: dict, groups:dict, verbose:bool=False):
         '''
         Private function used for refdiff_by_sections.
         '''
-
-        groups = {}
-        for i, pair in enumerate(combination):
-            config = {}
-            for k, v in zip(key_order, pair):
-                config[k] = ('==',v)
-            groups[i] = list(self.find_ids(**config))
-        return groups
-
-    def _ref_diff_group(self,refs,groups, verbose=False):
-        '''
-        Private function used for refdiff_by_sections.
-        '''
-
-        symbols = []
+        assert len(reference_groups) == len(groups)
+        arrays = []
         for key in groups:
-            if len(refs[key]) == 0:
+            if len(reference_groups[key]) == 0:
                 if verbose:
-                    print(f"{refs} for key = {key} no reference id found")
-                    print(groups)
+                    print(f"reference_groups[{key}] is empty")
+                    print(f"groups[{key}] is {groups[key]}")
                 continue
+            elif len(reference_groups[key]) > 1:
+                raise Exception(f"reference_group[{key}] has more than one element: {reference_groups[key]}"+"\n"+f"groups[{key}] is {groups[key]}")
             else:
-                refdiff_symbol = self.shrink(id=list(groups[key])).refdiff(refs[key][0])
-                symbols.append(refdiff_symbol)
-        return sum(symbols)
+                refdiff_symbol = self.shrink(id=list(groups[key])).refdiff(reference_groups[key][0])
+                arrays.append(refdiff_symbol.array)
+        return ka.concat(arrays)
 
     def refdiff_by_sections(self, criteria_dict, criteria_ref_dict, verbose=False):
         '''
         Returns the difference between the reference scenario following criteria based on the metadata attributes. 
 
         Parameters
         ----------
@@ -1492,26 +1563,297 @@
         -------
         new_symbol : Symbol
             The new symbol.
 
         Examples
         --------
         
-        >>> Z.refdiff_by_sections(**{'run':[0,1], 'country_set':['NA']})
+        >>> Z.refdiff_by_sections(criteria_dict={'run':[0,1], 'country_set':['NA']}, criteria_ref_dict={'case':['ref']})
 
         '''
-
+        ref = next(iter(criteria_ref_dict.values()))[0]
+        
         groups = self.create_mix(criteria_dict)
         criteria_ref_full = {**criteria_dict,**criteria_ref_dict}
         refs = self.create_mix(criteria_ref_full)
-        assert all([len(refs[key]) <= 1 for key in refs]), f"It should be only one reference scenario per group {criteria_ref_full.keys()} but more were found: {refs}"
-        return self._ref_diff_group(refs,groups,verbose)
+        ref_group = {}
+        for key in groups:
+            key_ref = (*key,ref,)
+            if key_ref in refs:
+                ref_group[key] = refs[key_ref]
+            else:
+                ref_group[key] = []
+        new_array = self._ref_diff_group(ref_group,groups,verbose)
+        new_name = f"({self.name}).refdiff_by_sections({criteria_dict=}, {criteria_ref_dict=})"
+        return self.new_symbol(new_array, new_name)
 
     def definition_msg(self, name):
         print(f"Attribute '{name}' must be defined first in __init__ method")
 
     def __repr__(self):
-        return f'''Symbol(name='{self.name}', \n       value_type='{self.value_type}')'''
+        return f'''Symbol(name='{self.name}', value_type='{self.value_type}')'''
+
+    def get_id_query(self, query:str) -> list:
+        '''
+        Get the ids that match the query. IMPORTANT: metadata attributes should be included in the query.
+        '''
+        return sorted(pd.DataFrame(self.metadata).query(expr=query).index.tolist())
+    
+    def query(self, query:str):
+        '''
+        Query the symbol. Metadata attributes can only be included in the query.
+        
+        Parameters
+        ----------
+        query : str
+            The query.
+
+        Returns
+        -------
+        symbol : Symbol
+            The symbol.
+             
+        '''
+        ids = self.get_id_query(query)
+        new_symbol = self.shrink(id=ids)
+        new_symbol.name = f"({self.name}).query({query=})"
+        return new_symbol
+    
+    def get_id_contains(self, metadata_attr:list) -> list:
+        '''
+        Get the ids that match the groupby. IMPORTANT: metadata attributes should be included in the groupby.
+        '''
+        group = pd.DataFrame(self.metadata).groupby(metadata_attr)
+        ids = [item for name in group.groups for item in group.get_group(name).index.tolist()]
+        return sorted(ids)
 
+    def groupby(self, metadata_attr:list):
+        '''
+        Groupby the symbol. Metadata attributes should be included in the groupby.
+        
+        Parameters
+        ----------
+        attributes : list
+            The attributes to groupby.
+
+        Returns
+        -------
+        Dictionary of symbols
+
+        '''
+        group = pd.DataFrame(self.metadata).groupby(metadata_attr)
+        return {name: self.shrink(id=group.get_group(name).index.tolist()) for name in group.groups}
+
+    def transform(self, metadata_attr:list, function:str):
+        '''
+        Transform the symbol with a function. Metadata attributes is a list of metadata attributes to groupby.
+        
+        Parameters
+        ----------
+        metadata_attr: list
+            List of metadata attributes to apply the function to.
+
+                
+        function: str
+            The function to apply. It can be one of the following:
+                - 'sum'
+                - 'mean'
+                - 'std'
+
+        Returns
+        -------
+        symbol : Symbol
+            The symbol.
 
-def from_feather(path):
-    return Symbol(**from_feather_dict(path, with_=ka.settings.feather_with))
+
+        This method applies between scenarios and broadcasts across scenarios id (most of the methods in this class apply within scenarios).
+        
+        
+        The example below shows how to use Pandas transform function over the dataframe obtained from the method 'dfc' (It could be slow with large symbols). At the end we show how it works with this method.
+        
+     
+        Examples:
+        ---------
+            For example if you have a Symbol EXPORT:
+            
+            EXPORT.dfc
+            
+               | id | country |value | custom_A | custom_B |
+             0 |  1 |   DE    | 1.0  |  summer  |   cars   |
+             1 |  1 |   FR    | 2.0  |  summer  |   cars   |
+             2 |  2 |   DE    | 3.0  |  summer  |   cars   |
+             3 |  2 |   FR    | 4.0  |  summer  |   cars   |
+             4 |  3 |   DE    | 5.0  |  winter  |   cars   |
+             5 |  3 |   FR    | 6.0  |  winter  |   cars   |
+             6 |  4 |   DE    | 7.0  |  winter  |   cars   |
+             7 |  4 |   FR    | 8.0  |  winter  |   cars   |
+             8 |  5 |   DE    | 9.0  |  summer  |  phones  |
+             9 |  5 |   FR    | 1.0  |  summer  |  phones  |
+            10 |  6 |   DE    | 2.0  |  summer  |  phones  |
+            11 |  6 |   FR    | 3.0  |  summer  |  phones  |
+            12 |  7 |   DE    | 4.0  |  winter  |  phones  |
+            13 |  7 |   FR    | 5.0  |  winter  |  phones  |
+            14 |  8 |   DE    | 6.0  |  winter  |  phones  |
+            15 |  8 |   FR    | 7.0  |  winter  |  phones  |
+        
+            where 'id', 'country' and 'day' are dimenssions, 'value' is the actual value, 
+            and 'custom_A', and 'custom_B' are metadata.
+            
+            As we want to sum up the values by 'custom_B' between scenarios, we will omit 'id' and 'custom_B'
+            
+            EXPORT.dfc.groupby(["country", "day", "custom_A"])['value'].transform('sum')
+            
+            this will return a pd.Series of 'value' with the same index as the original dataframe
+            
+              | value |
+            0 |  4.0  |
+            1 |  6.0  |
+            2 |  4.0  |
+            3 |  6.0  |
+            4 | 12.0  |
+            5 | 14.0  |
+            6 | 12.0  |
+            7 | 14.0  |
+            8 | 10.0  |
+            9 |  4.0  |
+           10 | 10.0  |
+           11 |  4.0  |
+           12 | 10.0  |
+           13 | 12.0  |
+           14 | 10.0  |
+           15 | 12.0  |
+
+            Bear in mind that after this operation there are scenarios with repeated values. Therefore a 'shrink' operation is needed to remove them.
+            
+            The example above shows the pure Pandas implemntation of groupby and transform.
+            
+            HERE, we use the Symbolx implemntation to get the same result as show above:
+            
+            NEW_EXPORT = EXPORT.transform(metadata_custom=["custom_A"], function="sum") # Consider that the operation is on 'custom_B'
+            
+        '''
+
+        ufunction_options = {"sum": np.sum, "mean": np.mean, "min": np.min, "max": np.max, "std": np.std}
+        assert function in ufunction_options, "function must be one of 'sum', 'mean', 'min', 'max', 'std'"
+        
+        group = pd.DataFrame(self.metadata).groupby(metadata_attr)
+        arrays = []
+        for name in group.groups:
+            df = group.get_group(name)
+            ids = df.index.tolist()
+            array = self.shrink(id=ids).array
+            new_array = array.ufunc(dim="id", func=ufunction_options[function], keepdims=True)
+            arrays.append(new_array)
+        
+        new_array = ka.concat(arrays=arrays)
+        new_name = f"({self.name}).transform({metadata_attr}, {function})"
+        return self.new_symbol(new_array, new_name)
+
+    def __eq__(self, other):
+        if isinstance(other, (int, float)):
+            array = self.array == other
+            new_name = f"({self.name})==({other})"
+            return self.new_symbol(array, new_name)
+        elif isinstance(other, Symbol):
+            array = self.array == other.array
+            new_name = f"({self.name})==({other.name})"
+            return self.new_symbol(array, new_name, other)
+        else:
+            raise Exception(f"{type(other)} is not supported. Must be Symbol, int or float")
+        
+    def __ne__(self, other):
+        if isinstance(other, (int, float)):
+            array = self.array != other
+            new_name = f"({self.name})!=({other})"
+            return self.new_symbol(array, new_name)
+        elif isinstance(other, Symbol):
+            array = self.array != other.array
+            new_name = f"({self.name})!=({other.name})"
+            return self.new_symbol(array, new_name, other)
+        else:
+            raise Exception(f"{type(other)} is not supported. Must be Symbol, int or float")
+    
+    def __gt__(self, other):
+        if isinstance(other, (int, float)):
+            array = self.array > other
+            new_name = f"({self.name})>({other})"
+            return self.new_symbol(array, new_name)
+        elif isinstance(other, Symbol):
+            array = self.array > other.array
+            new_name = f"({self.name})>({other.name})"
+            return self.new_symbol(array, new_name, other)
+        else:
+            raise Exception(f"{type(other)} is not supported. Must be Symbol, int or float")
+        
+    def __rgt__(self, other):
+        if isinstance(other, (int, float)):
+            array = other > self.array
+            new_name = f"({other})>({self.name})"
+            return self.new_symbol(array, new_name)
+        
+    def __lt__(self, other):
+        if isinstance(other, (int, float)):
+            array = self.array < other
+            new_name = f"({self.name})<({other})"
+            return self.new_symbol(array, new_name)
+        elif isinstance(other, Symbol):
+            array = self.array < other.array
+            new_name = f"({self.name})<({other.name})"
+            return self.new_symbol(array, new_name, other)
+        else:
+            raise Exception(f"{type(other)} is not supported. Must be Symbol, int or float")
+        
+    def __rlt__(self, other):
+        if isinstance(other, (int, float)):
+            array = other < self.array
+            new_name = f"({other})<({self.name})"
+            return self.new_symbol(array, new_name)
+        
+    def __ge__(self, other):
+        if isinstance(other, (int, float)):
+            array = self.array >= other
+            new_name = f"({self.name})>=({other})"
+            return self.new_symbol(array, new_name)
+        elif isinstance(other, Symbol):
+            array = self.array >= other.array
+            new_name = f"({self.name})>=({other.name})"
+            return self.new_symbol(array, new_name, other)
+        else:
+            raise Exception(f"{type(other)} is not supported. Must be Symbol, int or float")
+        
+    def __rge__(self, other):
+        if isinstance(other, (int, float)):
+            array = other >= self.array
+            new_name = f"({other})>=({self.name})"
+            return self.new_symbol(array, new_name)
+        
+    def __le__(self, other):
+        if isinstance(other, (int, float)):
+            array = self.array <= other
+            new_name = f"({self.name})<=({other})"
+            return self.new_symbol(array, new_name)
+        elif isinstance(other, Symbol):
+            array = self.array <= other.array
+            new_name = f"({self.name})<=({other.name})"
+            return self.new_symbol(array, new_name, other)
+        else:
+            raise Exception(f"{type(other)} is not supported. Must be Symbol, int or float")
+    
+    def __rle__(self, other):
+        if isinstance(other, (int, float)):
+            array = other <= self.array
+            new_name = f"({other})<=({self.name})"
+            return self.new_symbol(array, new_name)
+        
+    def _repr_html_(self):
+        # TODO: add metadata same like "show unique coords"
+        string = self.array._repr_html_().replace("[k]array", "SymbolX")
+        string += "<br><b>Symbol name:</b><br>"
+        string += self.name
+        return string
+        
+        
+def from_feather(path, load_with:str="pandas"):
+    """Path: Feather file. Condition to created previously with symbolx
+        load_with: ["pandas","polars"]
+    """
+    return Symbol(**from_feather_dict(path, with_=load_with))
```

### Comparing `symbolx-0.4.2/symbolx/utils.py` & `symbolx-0.4.3/symbolx/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,17 +119,17 @@
     directory = pathlib.Path(folder_path)
     with zipfile.ZipFile(f"{folder_path}.{zip_extension}", "w", EXT_CONF[zip_extension], compresslevel=compresslevel, allowZip64=allowZip64) as archive:
         for file_path in directory.rglob("*"):
             archive.write(file_path, arcname=file_path.relative_to(directory))
     if delete:
         try:
             shutil.rmtree(folder_path)
-        except OSError as e:
+        except OSError:
             print(f"Error folder not deleted {folder_path}")
-            #TODO: logger with details about the error (permission denied?)
+            # TODO: logger with details about the error (permission denied?)
     return None
 
 def unzip(source_filename, dest_dir, delete=False):
     with zipfile.ZipFile(source_filename) as zf:
         zf.extractall(dest_dir)
     if delete:
         try:
```

### Comparing `symbolx-0.4.2/symbolx.egg-info/PKG-INFO` & `symbolx-0.4.3/symbolx.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbolx
-Version: 0.4.2
+Version: 0.4.3
 Summary:  Symbolx helps collecting several scenarios data such as multidimentional variables and parameters for reporting and visualization wiht help of karray
 Author: Carlos Gaete-Morales
 Author-email: cdgaete@gmail.com
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
@@ -13,14 +13,18 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: karray>=2024.3.7
+Requires-Dist: pyarrow
 
 # symbolx
 Dealling with multiple scenarios data?  This tool helps collecting several scenarios data such as multidimentional variables and parameters for reporting and visualization
 
 
 Initial setting to be able to collect scenarios info. The following example uses parser and loader for GAMS-dieterpy output. For CSV and Arrow file formats see the test folder in https://gitlab.com/diw-evu/symbolx/-/tree/main/test
```

### Comparing `symbolx-0.4.2/test/test.py` & `symbolx-0.4.3/test/test.py`

 * *Files identical despite different names*

