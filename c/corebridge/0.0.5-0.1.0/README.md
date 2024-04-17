# Comparing `tmp/corebridge-0.0.5.tar.gz` & `tmp/corebridge-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corebridge-0.0.5.tar", last modified: Tue Apr 16 10:11:52 2024, max compression
+gzip compressed data, was "corebridge-0.1.0.tar", last modified: Wed Apr 17 14:53:26 2024, max compression
```

## Comparing `corebridge-0.0.5.tar` & `corebridge-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-04-16 10:11:52.768525 corebridge-0.0.5/
--rw-r--r--   0 fenke     (1000) users      (100)    11337 2024-01-31 12:54:47.000000 corebridge-0.0.5/LICENSE
--rw-r--r--   0 fenke     (1000) users      (100)      111 2024-01-31 12:54:47.000000 corebridge-0.0.5/MANIFEST.in
--rw-r--r--   0 fenke     (1000) users      (100)     1203 2024-04-16 10:11:52.768525 corebridge-0.0.5/PKG-INFO
--rw-r--r--   0 fenke     (1000) users      (100)      435 2024-04-16 10:09:45.000000 corebridge-0.0.5/README.md
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-04-16 10:11:52.768525 corebridge-0.0.5/corebridge/
--rw-r--r--   0 fenke     (1000) users      (100)       22 2024-04-16 10:09:53.000000 corebridge-0.0.5/corebridge/__init__.py
--rw-r--r--   0 fenke     (1000) users      (100)     3024 2024-04-16 10:09:53.000000 corebridge-0.0.5/corebridge/_modidx.py
--rw-r--r--   0 fenke     (1000) users      (100)     7767 2024-04-16 10:09:53.000000 corebridge-0.0.5/corebridge/aicorebridge.py
--rw-r--r--   0 fenke     (1000) users      (100)     3766 2024-04-16 10:09:53.000000 corebridge-0.0.5/corebridge/core.py
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-04-16 10:11:52.768525 corebridge-0.0.5/corebridge.egg-info/
--rw-r--r--   0 fenke     (1000) users      (100)     1203 2024-04-16 10:11:52.000000 corebridge-0.0.5/corebridge.egg-info/PKG-INFO
--rw-r--r--   0 fenke     (1000) users      (100)      381 2024-04-16 10:11:52.000000 corebridge-0.0.5/corebridge.egg-info/SOURCES.txt
--rw-r--r--   0 fenke     (1000) users      (100)        1 2024-04-16 10:11:52.000000 corebridge-0.0.5/corebridge.egg-info/dependency_links.txt
--rw-r--r--   0 fenke     (1000) users      (100)       42 2024-04-16 10:11:52.000000 corebridge-0.0.5/corebridge.egg-info/entry_points.txt
--rw-r--r--   0 fenke     (1000) users      (100)        1 2024-01-31 15:42:47.000000 corebridge-0.0.5/corebridge.egg-info/not-zip-safe
--rw-r--r--   0 fenke     (1000) users      (100)      225 2024-04-16 10:11:52.000000 corebridge-0.0.5/corebridge.egg-info/requires.txt
--rw-r--r--   0 fenke     (1000) users      (100)       11 2024-04-16 10:11:52.000000 corebridge-0.0.5/corebridge.egg-info/top_level.txt
--rw-r--r--   0 fenke     (1000) users      (100)     1146 2024-01-31 15:48:02.000000 corebridge-0.0.5/settings.ini
--rw-r--r--   0 fenke     (1000) users      (100)       38 2024-04-16 10:11:52.768525 corebridge-0.0.5/setup.cfg
--rw-r--r--   0 fenke     (1000) users      (100)     2596 2024-01-31 12:54:47.000000 corebridge-0.0.5/setup.py
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-04-17 14:53:26.860277 corebridge-0.1.0/
+-rw-r--r--   0 fenke     (1000) users      (100)    11337 2024-01-31 12:54:47.000000 corebridge-0.1.0/LICENSE
+-rw-r--r--   0 fenke     (1000) users      (100)      111 2024-01-31 12:54:47.000000 corebridge-0.1.0/MANIFEST.in
+-rw-r--r--   0 fenke     (1000) users      (100)     1203 2024-04-17 14:53:26.860277 corebridge-0.1.0/PKG-INFO
+-rw-r--r--   0 fenke     (1000) users      (100)      435 2024-04-17 14:51:56.000000 corebridge-0.1.0/README.md
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-04-17 14:53:26.860277 corebridge-0.1.0/corebridge/
+-rw-r--r--   0 fenke     (1000) users      (100)       22 2024-04-17 14:52:06.000000 corebridge-0.1.0/corebridge/__init__.py
+-rw-r--r--   0 fenke     (1000) users      (100)     3300 2024-04-17 14:52:06.000000 corebridge-0.1.0/corebridge/_modidx.py
+-rw-r--r--   0 fenke     (1000) users      (100)     8155 2024-04-17 14:52:06.000000 corebridge-0.1.0/corebridge/aicorebridge.py
+-rw-r--r--   0 fenke     (1000) users      (100)     3766 2024-04-17 14:52:06.000000 corebridge-0.1.0/corebridge/core.py
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-04-17 14:53:26.860277 corebridge-0.1.0/corebridge.egg-info/
+-rw-r--r--   0 fenke     (1000) users      (100)     1203 2024-04-17 14:53:26.000000 corebridge-0.1.0/corebridge.egg-info/PKG-INFO
+-rw-r--r--   0 fenke     (1000) users      (100)      381 2024-04-17 14:53:26.000000 corebridge-0.1.0/corebridge.egg-info/SOURCES.txt
+-rw-r--r--   0 fenke     (1000) users      (100)        1 2024-04-17 14:53:26.000000 corebridge-0.1.0/corebridge.egg-info/dependency_links.txt
+-rw-r--r--   0 fenke     (1000) users      (100)       42 2024-04-17 14:53:26.000000 corebridge-0.1.0/corebridge.egg-info/entry_points.txt
+-rw-r--r--   0 fenke     (1000) users      (100)        1 2024-01-31 15:42:47.000000 corebridge-0.1.0/corebridge.egg-info/not-zip-safe
+-rw-r--r--   0 fenke     (1000) users      (100)      225 2024-04-17 14:53:26.000000 corebridge-0.1.0/corebridge.egg-info/requires.txt
+-rw-r--r--   0 fenke     (1000) users      (100)       11 2024-04-17 14:53:26.000000 corebridge-0.1.0/corebridge.egg-info/top_level.txt
+-rw-r--r--   0 fenke     (1000) users      (100)     1146 2024-04-17 14:47:59.000000 corebridge-0.1.0/settings.ini
+-rw-r--r--   0 fenke     (1000) users      (100)       38 2024-04-17 14:53:26.860277 corebridge-0.1.0/setup.cfg
+-rw-r--r--   0 fenke     (1000) users      (100)     2596 2024-01-31 12:54:47.000000 corebridge-0.1.0/setup.py
```

### Comparing `corebridge-0.0.5/LICENSE` & `corebridge-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `corebridge-0.0.5/PKG-INFO` & `corebridge-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corebridge
-Version: 0.0.5
+Version: 0.1.0
 Summary: Bridge for Stactics AICore
 Home-page: https://github.com/fenke/corebridge
 Author: Fenke Meijer
 Author-email: fenkemeijer@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `corebridge-0.0.5/corebridge/_modidx.py` & `corebridge-0.1.0/corebridge/_modidx.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,16 @@
                 'lib_path': 'corebridge'},
   'syms': { 'corebridge.aicorebridge': { 'corebridge.aicorebridge.AICoreModule': ( 'aicorebridge.html#aicoremodule',
                                                                                    'corebridge/aicorebridge.py'),
                                          'corebridge.aicorebridge.AICoreModule.__init__': ( 'aicorebridge.html#aicoremodule.__init__',
                                                                                             'corebridge/aicorebridge.py'),
                                          'corebridge.aicorebridge.AICoreModule._init_processor': ( 'aicorebridge.html#aicoremodule._init_processor',
                                                                                                    'corebridge/aicorebridge.py'),
+                                         'corebridge.aicorebridge.AICoreModule.call_processor': ( 'aicorebridge.html#aicoremodule.call_processor',
+                                                                                                  'corebridge/aicorebridge.py'),
                                          'corebridge.aicorebridge.AICoreModule.convert_to_dataframe': ( 'aicorebridge.html#aicoremodule.convert_to_dataframe',
                                                                                                         'corebridge/aicorebridge.py'),
                                          'corebridge.aicorebridge.AICoreModule.get_call_data': ( 'aicorebridge.html#aicoremodule.get_call_data',
                                                                                                  'corebridge/aicorebridge.py'),
                                          'corebridge.aicorebridge.AICoreModule.get_callargs': ( 'aicorebridge.html#aicoremodule.get_callargs',
                                                                                                 'corebridge/aicorebridge.py'),
                                          'corebridge.aicorebridge.AICoreModule.infer': ( 'aicorebridge.html#aicoremodule.infer',
```

### Comparing `corebridge-0.0.5/corebridge/aicorebridge.py` & `corebridge-0.1.0/corebridge/aicorebridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,25 +13,30 @@
 import numpy as np
 
 from fastcore.basics import patch_to, patch
 
 # %% ../nbs/01_aicorebridge.ipynb 4
 syslog = logging.getLogger(__name__)
 
+# %% ../nbs/01_aicorebridge.ipynb 5
+print(f"loading {__name__}")
+
 # %% ../nbs/01_aicorebridge.ipynb 6
 class AICoreModule(): pass
 
 # %% ../nbs/01_aicorebridge.ipynb 7
 @patch
 def __init__(self:AICoreModule, 
              save_dir:str, # path where the module can keep files 
+             assets_dir:str,
              processor:typing.Callable, # data processing function
              *args, **kwargs):
     
     self.save_dir  = save_dir
+    self.assets_dir  = assets_dir
     self._init_processor(processor)
 
     self.init_args = args
     self.init_kwargs = kwargs
 
 
 
@@ -47,14 +52,20 @@
     self.processor_params = dict(self.processor_signature.parameters)
     self.return_param = self.processor_params.pop('return', None)
     self.data_param, *self.call_params = list(self.processor_params.keys())
 
 
 # %% ../nbs/01_aicorebridge.ipynb 9
 @patch
+def call_processor(self:AICoreModule, calldata, **callargs):
+    return self.processor(calldata, **callargs)
+
+
+# %% ../nbs/01_aicorebridge.ipynb 10
+@patch
 def infer(self:AICoreModule, data:dict, *_, **kwargs):
     try:
 
         msg=[
             f"{self.processor.__name__}({self.processor_signature})",
             f"init_args: {self.init_args}, init_kwargs: {self.init_kwargs}",
         ]
@@ -74,15 +85,15 @@
         msg.append(f"calldata shape: {calldata.shape}")
 
         callargs = self.get_callargs(**kwargs)
 
         for arg, val in callargs.items():
             msg.append(f"{arg}: {val}")
             
-        result = self.processor(calldata, **callargs)
+        result = self.call_processor(calldata, **callargs)
         msg.append(f"result shape: {result.shape}")
 
         return {
             'msg':msg,
             'data': self.rewrite_data(
                 result if not lastSeen else result[-1:],
                 recordformat=recordformat,
@@ -92,28 +103,31 @@
     except Exception as err:
         return {
             'msg': f"Unexpected {err=}, {type(err)=}",
             'data': []
         }
 
 
-# %% ../nbs/01_aicorebridge.ipynb 10
+# %% ../nbs/01_aicorebridge.ipynb 11
 @patch
 def get_callargs(self:AICoreModule, **kwargs):
     "Get arguments for the processor call"
 
+    # Remove null / None values
+    kwargs = {k:v for k,v in kwargs.items() if v is not None}
+    
     metadata = kwargs.pop('metadata', {}) # TODO: historic metadata
 
     return {
         K:self.processor_signature.parameters[K].annotation(kwargs.get(K,metadata.get(K, self.init_kwargs.get(K, self.processor_signature.parameters[K].default))))
         for K in self.call_params
     }
 
 
-# %% ../nbs/01_aicorebridge.ipynb 11
+# %% ../nbs/01_aicorebridge.ipynb 12
 @patch
 def get_call_data(
         self:AICoreModule, 
         data:dict, 
         recordformat='records', 
         timezone='UTC', 
         reversed=False):
@@ -155,15 +169,15 @@
         df.index = (df.index - datetime.datetime(1970,1,1, tzinfo=datetime.timezone.utc)) / datetime.timedelta(seconds=1)
         return df.to_records(index=True)
     else:
         df.index = (df.index - datetime.datetime(1970,1,1, tzinfo=datetime.timezone.utc)) / datetime.timedelta(seconds=1)
         return df.reset_index().to_numpy()
         
 
-# %% ../nbs/01_aicorebridge.ipynb 12
+# %% ../nbs/01_aicorebridge.ipynb 13
 @patch
 def rewrite_data(
         self:AICoreModule, 
         data:typing.Union[pd.DataFrame, pd.Series, dict], 
         recordformat:str='split', 
         timezone:str='UTC', 
         reversed:bool=False):
@@ -190,15 +204,15 @@
     if normalized_data.isna().any(axis=None):
         return [ {k:v for k,v in m.items() if pd.notnull(v)} for m in records]
     else:
         return records
 
     
 
-# %% ../nbs/01_aicorebridge.ipynb 13
+# %% ../nbs/01_aicorebridge.ipynb 14
 @patch
 def convert_to_dataframe(
         self:AICoreModule, 
         adata:typing.Union[pd.DataFrame, pd.Series, dict, np.ndarray, np.recarray], 
         timezone='UTC', 
         columnnames=None):
     """Convert various data formats to standardized timeseries DataFrame"""
```

### Comparing `corebridge-0.0.5/corebridge/core.py` & `corebridge-0.1.0/corebridge/core.py`

 * *Files identical despite different names*

### Comparing `corebridge-0.0.5/corebridge.egg-info/PKG-INFO` & `corebridge-0.1.0/corebridge.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corebridge
-Version: 0.0.5
+Version: 0.1.0
 Summary: Bridge for Stactics AICore
 Home-page: https://github.com/fenke/corebridge
 Author: Fenke Meijer
 Author-email: fenkemeijer@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `corebridge-0.0.5/settings.ini` & `corebridge-0.1.0/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = corebridge
 lib_name = %(repo)s
-version = 0.0.5
+version = 0.1.0
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = corebridge
```

### Comparing `corebridge-0.0.5/setup.py` & `corebridge-0.1.0/setup.py`

 * *Files identical despite different names*

