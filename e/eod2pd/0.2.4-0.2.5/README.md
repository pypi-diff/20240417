# Comparing `tmp/eod2pd-0.2.4.tar.gz` & `tmp/eod2pd-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eod2pd-0.2.4.tar", last modified: Tue Apr  2 18:22:51 2024, max compression
+gzip compressed data, was "eod2pd-0.2.5.tar", last modified: Wed Apr 17 17:24:31 2024, max compression
```

## Comparing `eod2pd-0.2.4.tar` & `eod2pd-0.2.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-02 18:22:51.132999 eod2pd-0.2.4/
--rw-r--r--   0 neutro2    (501) staff       (20)     8882 2024-04-02 18:22:51.132477 eod2pd-0.2.4/PKG-INFO
--rw-r--r--   0 neutro2    (501) staff       (20)     1074 2024-03-22 21:23:52.000000 eod2pd-0.2.4/license
--rw-r--r--   0 neutro2    (501) staff       (20)     1042 2024-03-29 15:47:09.000000 eod2pd-0.2.4/pyproject.toml
--rw-r--r--   0 neutro2    (501) staff       (20)     6844 2024-03-24 19:07:03.000000 eod2pd-0.2.4/readme.md
--rw-r--r--   0 neutro2    (501) staff       (20)       38 2024-04-02 18:22:51.133096 eod2pd-0.2.4/setup.cfg
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-02 18:22:51.123624 eod2pd-0.2.4/src/
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-02 18:22:51.127720 eod2pd-0.2.4/src/eod2pd/
--rw-r--r--   0 neutro2    (501) staff       (20)     1638 2024-03-24 18:23:55.000000 eod2pd-0.2.4/src/eod2pd/__init__.py
--rw-r--r--   0 neutro2    (501) staff       (20)     6179 2024-03-24 18:23:05.000000 eod2pd-0.2.4/src/eod2pd/downloader.py
--rw-r--r--   0 neutro2    (501) staff       (20)    23344 2024-03-29 13:43:53.000000 eod2pd-0.2.4/src/eod2pd/downloaderfunctions.py
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-02 18:22:51.131662 eod2pd-0.2.4/src/eod2pd.egg-info/
--rw-r--r--   0 neutro2    (501) staff       (20)     8882 2024-04-02 18:22:51.000000 eod2pd-0.2.4/src/eod2pd.egg-info/PKG-INFO
--rw-r--r--   0 neutro2    (501) staff       (20)      301 2024-04-02 18:22:51.000000 eod2pd-0.2.4/src/eod2pd.egg-info/SOURCES.txt
--rw-r--r--   0 neutro2    (501) staff       (20)        1 2024-04-02 18:22:51.000000 eod2pd-0.2.4/src/eod2pd.egg-info/dependency_links.txt
--rw-r--r--   0 neutro2    (501) staff       (20)      114 2024-04-02 18:22:51.000000 eod2pd-0.2.4/src/eod2pd.egg-info/requires.txt
--rw-r--r--   0 neutro2    (501) staff       (20)        7 2024-04-02 18:22:51.000000 eod2pd-0.2.4/src/eod2pd.egg-info/top_level.txt
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-17 17:24:31.039493 eod2pd-0.2.5/
+-rw-r--r--   0 neutro2    (501) staff       (20)     8882 2024-04-17 17:24:31.038936 eod2pd-0.2.5/PKG-INFO
+-rw-r--r--   0 neutro2    (501) staff       (20)     1074 2024-03-22 21:23:52.000000 eod2pd-0.2.5/license
+-rw-r--r--   0 neutro2    (501) staff       (20)     1042 2024-04-16 11:30:23.000000 eod2pd-0.2.5/pyproject.toml
+-rw-r--r--   0 neutro2    (501) staff       (20)     6844 2024-03-24 19:07:03.000000 eod2pd-0.2.5/readme.md
+-rw-r--r--   0 neutro2    (501) staff       (20)       38 2024-04-17 17:24:31.039585 eod2pd-0.2.5/setup.cfg
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-17 17:24:31.030183 eod2pd-0.2.5/src/
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-17 17:24:31.035448 eod2pd-0.2.5/src/eod2pd/
+-rw-r--r--   0 neutro2    (501) staff       (20)     1638 2024-03-24 18:23:55.000000 eod2pd-0.2.5/src/eod2pd/__init__.py
+-rw-r--r--   0 neutro2    (501) staff       (20)     6179 2024-03-24 18:23:05.000000 eod2pd-0.2.5/src/eod2pd/downloader.py
+-rw-r--r--   0 neutro2    (501) staff       (20)    23939 2024-04-17 17:22:10.000000 eod2pd-0.2.5/src/eod2pd/downloaderfunctions.py
+-rw-r--r--   0 neutro2    (501) staff       (20)     4100 2024-04-16 11:26:20.000000 eod2pd-0.2.5/src/eod2pd/utilityfunctions.py
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-17 17:24:31.038183 eod2pd-0.2.5/src/eod2pd.egg-info/
+-rw-r--r--   0 neutro2    (501) staff       (20)     8882 2024-04-17 17:24:31.000000 eod2pd-0.2.5/src/eod2pd.egg-info/PKG-INFO
+-rw-r--r--   0 neutro2    (501) staff       (20)      332 2024-04-17 17:24:31.000000 eod2pd-0.2.5/src/eod2pd.egg-info/SOURCES.txt
+-rw-r--r--   0 neutro2    (501) staff       (20)        1 2024-04-17 17:24:31.000000 eod2pd-0.2.5/src/eod2pd.egg-info/dependency_links.txt
+-rw-r--r--   0 neutro2    (501) staff       (20)      114 2024-04-17 17:24:31.000000 eod2pd-0.2.5/src/eod2pd.egg-info/requires.txt
+-rw-r--r--   0 neutro2    (501) staff       (20)        7 2024-04-17 17:24:31.000000 eod2pd-0.2.5/src/eod2pd.egg-info/top_level.txt
```

### Comparing `eod2pd-0.2.4/PKG-INFO` & `eod2pd-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eod2pd
-Version: 0.2.4
+Version: 0.2.5
 Summary: a simple library to quere EODHistoricalData in a multithreaded environment
 Author-email: NeuralDevelopment <neutro2@outlook.de>
 License: MIT License
         
         Copyright (c) 2023 NeuralDevelopment
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `eod2pd-0.2.4/license` & `eod2pd-0.2.5/license`

 * *Files identical despite different names*

### Comparing `eod2pd-0.2.4/pyproject.toml` & `eod2pd-0.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eod2pd"
-version = "0.2.4"
+version = "0.2.5"
 
 authors = [{ name = "NeuralDevelopment", email = "neutro2@outlook.de" }]
 description = "a simple library to quere EODHistoricalData in a multithreaded environment"
 
 readme = "readme.md"
 license = { file = "license" }
 requires-python = ">=3.10"
```

### Comparing `eod2pd-0.2.4/readme.md` & `eod2pd-0.2.5/readme.md`

 * *Files identical despite different names*

### Comparing `eod2pd-0.2.4/src/eod2pd/__init__.py` & `eod2pd-0.2.5/src/eod2pd/__init__.py`

 * *Files identical despite different names*

### Comparing `eod2pd-0.2.4/src/eod2pd/downloader.py` & `eod2pd-0.2.5/src/eod2pd/downloader.py`

 * *Files identical despite different names*

### Comparing `eod2pd-0.2.4/src/eod2pd/downloaderfunctions.py` & `eod2pd-0.2.5/src/eod2pd/downloaderfunctions.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 import basefunctions
 import basefunctions.threadpool
 import decouple
 import pandas as pd
 
 import eod2pd.downloader
+import eod2pd.utilityfunctions
 
 # -------------------------------------------------------------
 # IMPORTS
 # -------------------------------------------------------------
 
 # -------------------------------------------------------------
 # DEFINITIONS REGISTRY
@@ -133,19 +134,39 @@
     pandas.DataFrame | dict
         DataFrame containing the list of exchanges or
         a dictionary containing the list of exchanges.
     """
     # start jobs to get exchanges
     start_jobs_get_exchanges()
     # wait until all jobs are done
-    basefunctions.default_threadpool.get_input_queue().join()
+    basefunctions.get_default_threadpool().get_input_queue().join()
+    # add index to dataframe
+    index_row = {
+        "name": "Index Exchange",
+        "code": "INDX",
+        "operatingmic": "INDX",
+        "country": "Unknown",
+        "currency": "Unknown",
+        "countryiso2": "Unknown",
+        "countryiso3": "Unknown",
+    }
     # get dataframes from output queue
-    return basefunctions.default_threadpool.get_dataframes_from_output_queue(
-        dict_result=dict_result
-    )
+    result = eod2pd.utilityfunctions.get_dataframes_from_output_queue(dict_result=dict_result)
+
+    # check the type of result
+    if isinstance(result, dict):
+        # If it's a dictionary, get the first dataframe
+        df = list(result.values())[0]
+    else:
+        df = result
+
+    # append index_row to the dataframe
+    df = pd.concat([df, pd.DataFrame([index_row])], ignore_index=True)
+    # return the result
+    return df if dict_result is False else {"exchanges": df}
 
 
 # -------------------------------------------------------------
 #  start jobs get list of symbols for a specific exchange from EODHistoricalData
 # -------------------------------------------------------------
 def start_jobs_get_exchanges_symbols(
     exchange: str = None, params: dict = None, hook: Callable = None
@@ -224,19 +245,17 @@
     if isinstance(exchanges, str):
         exchanges = [exchanges]
     # loop over all exchanges
     for exchange in exchanges:
         # start jobs to get symbols for exchange
         start_jobs_get_exchanges_symbols(exchange.upper())
     # wait until all jobs are done
-    basefunctions.default_threadpool.get_input_queue().join()
+    basefunctions.get_default_threadpool().get_input_queue().join()
     # get dataframes from output queue
-    return basefunctions.default_threadpool.get_dataframes_from_output_queue(
-        dict_result=dict_result
-    )
+    return eod2pd.utilityfunctions.get_dataframes_from_output_queue(dict_result=dict_result)
 
 
 # -------------------------------------------------------------
 #  start jobs get symbol prices in a bulk message from EODHistoricalData
 # -------------------------------------------------------------
 def start_jobs_get_symbols_prices_bulk(
     exchange: str = None,
@@ -353,20 +372,18 @@
         exchanges = [exchanges]
     # loop over all exchanges
     for exchange in exchanges:
         # start jobs to get symbols bulk prices
         start_jobs_get_symbols_prices_bulk(exchange, start, end)
 
     # wait until all jobs are done
-    basefunctions.default_threadpool.get_input_queue().join()
+    basefunctions.get_default_threadpool().get_input_queue().join()
 
     # get dataframes from output queue
-    return basefunctions.default_threadpool.get_dataframes_from_output_queue(
-        dict_result=dict_result
-    )
+    return eod2pd.utilityfunctions.get_dataframes_from_output_queue(dict_result=dict_result)
 
 
 # -------------------------------------------------------------
 #  start_jobs_get symbol prices from EODHistoricalData
 # -------------------------------------------------------------
 def start_jobs_get_symbols_prices(
     symbols: List[str] | None,
@@ -469,19 +486,17 @@
     pandas.DataFrame | dict
         A DataFrame containing the symbol prices for the given symbols and date or
         a dictionary containing the symbols prices for the given symbols and date.
     """
     # start jobs to get symbols prices
     start_jobs_get_symbols_prices(symbols, start, end, freq)
     # wait until all jobs are done
-    basefunctions.default_threadpool.get_input_queue().join()
+    basefunctions.get_default_threadpool().get_input_queue().join()
     # get dataframes from output queue
-    return basefunctions.default_threadpool.get_dataframes_from_output_queue(
-        dict_result=dict_result
-    )
+    return eod2pd.utilityfunctions.get_dataframes_from_output_queue(dict_result=dict_result)
 
 
 # -------------------------------------------------------------
 #  start jobs get symbol dividends from EODHistoricalData
 # -------------------------------------------------------------
 def start_jobs_get_symbols_dividends(
     symbols: List[str] | None,
@@ -573,19 +588,17 @@
     pandas.DataFrame | dict
         A DataFrame containing the historical symbol dividends for the given symbols or
         a dictionary containing the historical symbols dividends for the given symbols.
     """
     # start jobs to get symbols dividends
     start_jobs_get_symbols_dividends(symbols, start, end)
     # wait until all jobs are done
-    basefunctions.default_threadpool.get_input_queue().join()
+    basefunctions.get_default_threadpool().get_input_queue().join()
     # get dataframes from output queue
-    return basefunctions.default_threadpool.get_dataframes_from_output_queue(
-        dict_result=dict_result
-    )
+    return eod2pd.utilityfunctions.get_dataframes_from_output_queue(dict_result=dict_result)
 
 
 # -------------------------------------------------------------
 #  start jobs get symbol splits from EODHistoricalData
 # -------------------------------------------------------------
 def start_jobs_get_symbols_splits(
     symbols: List[str] | None,
@@ -676,19 +689,17 @@
     pandas.DataFrame | dict
         A DataFrame containing the historical symbol dividends for the given symbols or
         a dictionary containing the historical symbols dividends for the given symbols.
     """
     # start jobs to get symbols splits
     start_jobs_get_symbols_splits(symbols, start, end)
     # wait until all jobs are done
-    basefunctions.default_threadpool.get_input_queue().join()
+    basefunctions.get_default_threadpool().get_input_queue().join()
     # get dataframes from output queue
-    return basefunctions.default_threadpool.get_dataframes_from_output_queue(
-        dict_result=dict_result
-    )
+    return eod2pd.utilityfunctions.get_dataframes_from_output_queue(dict_result=dict_result)
 
 
 # =========================================================================
 #
 # helper functions
 #
 # =========================================================================
@@ -706,8 +717,8 @@
     timeout = decouple.config("EOD2PD_TIMEOUT", default=10, cast=int)
     message = basefunctions.threadpool.create_threadpool_message(
         _type=eod2pd.EOD2PDMESSAGEIDENTIFIER,
         content=content,
         timeout=timeout,
         hook=hook,
     )
-    basefunctions.default_threadpool.get_input_queue().put(message)
+    basefunctions.get_default_threadpool().get_input_queue().put(message)
```

### Comparing `eod2pd-0.2.4/src/eod2pd.egg-info/PKG-INFO` & `eod2pd-0.2.5/src/eod2pd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eod2pd
-Version: 0.2.4
+Version: 0.2.5
 Summary: a simple library to quere EODHistoricalData in a multithreaded environment
 Author-email: NeuralDevelopment <neutro2@outlook.de>
 License: MIT License
         
         Copyright (c) 2023 NeuralDevelopment
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

