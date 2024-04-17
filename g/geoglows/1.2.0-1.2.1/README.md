# Comparing `tmp/geoglows-1.2.0.tar.gz` & `tmp/geoglows-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoglows-1.2.0.tar", last modified: Sun Apr 14 04:36:00 2024, max compression
+gzip compressed data, was "geoglows-1.2.1.tar", last modified: Wed Apr 17 19:42:49 2024, max compression
```

## Comparing `geoglows-1.2.0.tar` & `geoglows-1.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:36:00.587682 geoglows-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-14 04:35:54.000000 geoglows-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-14 04:35:54.000000 geoglows-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-14 04:36:00.587682 geoglows-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-14 04:35:54.000000 geoglows-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:36:00.583682 geoglows-1.2.0/geoglows/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:36:00.587682 geoglows-1.2.0/geoglows/_plots/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/_plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/_plots/format_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    16447 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/_plots/plotly_bias_corrected.py
--rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/_plots/plotly_forecasts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/_plots/plotly_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/_plots/plotly_retrospective.py
--rw-r--r--   0 runner    (1001) docker     (127)    11701 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/_plots/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/bias.py
--rw-r--r--   0 runner    (1001) docker     (127)    15146 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15652 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/streamflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:36:00.587682 geoglows-1.2.0/geoglows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-14 04:36:00.000000 geoglows-1.2.0/geoglows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-14 04:36:00.000000 geoglows-1.2.0/geoglows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 04:36:00.000000 geoglows-1.2.0/geoglows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-14 04:36:00.000000 geoglows-1.2.0/geoglows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 04:36:00.000000 geoglows-1.2.0/geoglows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-14 04:35:54.000000 geoglows-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 04:36:00.587682 geoglows-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-14 04:35:54.000000 geoglows-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:42:49.250964 geoglows-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-17 19:42:44.000000 geoglows-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-17 19:42:44.000000 geoglows-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-17 19:42:49.250964 geoglows-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-17 19:42:44.000000 geoglows-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:42:49.246964 geoglows-1.2.1/geoglows/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:42:49.250964 geoglows-1.2.1/geoglows/_plots/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/_plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/_plots/format_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16447 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/_plots/plotly_bias_corrected.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/_plots/plotly_forecasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/_plots/plotly_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/_plots/plotly_retrospective.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11701 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/_plots/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15279 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15652 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/streamflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-17 19:42:44.000000 geoglows-1.2.1/geoglows/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:42:49.250964 geoglows-1.2.1/geoglows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-17 19:42:49.000000 geoglows-1.2.1/geoglows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-17 19:42:49.000000 geoglows-1.2.1/geoglows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:42:49.000000 geoglows-1.2.1/geoglows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-17 19:42:49.000000 geoglows-1.2.1/geoglows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 19:42:49.000000 geoglows-1.2.1/geoglows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-17 19:42:44.000000 geoglows-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 19:42:49.250964 geoglows-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-17 19:42:44.000000 geoglows-1.2.1/setup.py
```

### Comparing `geoglows-1.2.0/LICENSE` & `geoglows-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.0/PKG-INFO` & `geoglows-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.2.0
+Version: 1.2.1
 Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
```

### Comparing `geoglows-1.2.0/README.md` & `geoglows-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.0/geoglows/_plots/__init__.py` & `geoglows-1.2.1/geoglows/_plots/__init__.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.0/geoglows/_plots/format_tools.py` & `geoglows-1.2.1/geoglows/_plots/format_tools.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.0/geoglows/_plots/plotly_bias_corrected.py` & `geoglows-1.2.1/geoglows/_plots/plotly_bias_corrected.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.0/geoglows/_plots/plotly_forecasts.py` & `geoglows-1.2.1/geoglows/_plots/plotly_forecasts.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.0/geoglows/_plots/plotly_helpers.py` & `geoglows-1.2.1/geoglows/_plots/plotly_helpers.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.0/geoglows/_plots/plotly_retrospective.py` & `geoglows-1.2.1/geoglows/_plots/plotly_retrospective.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.0/geoglows/_plots/plots.py` & `geoglows-1.2.1/geoglows/_plots/plots.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.0/geoglows/analyze.py` & `geoglows-1.2.1/geoglows/analyze.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.0/geoglows/bias.py` & `geoglows-1.2.1/geoglows/bias.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.0/geoglows/data.py` & `geoglows-1.2.1/geoglows/data.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import warnings
 from io import StringIO
 
 import pandas as pd
 import requests
 import s3fs
 import xarray as xr
+import numpy as np
 
 from ._constants import METADATA_TABLE_PATH
 from .analyze import (
     simple_forecast as calc_simple_forecast,
     forecast_stats as calc_forecast_stats,
     daily_averages as calc_daily_averages,
     monthly_averages as calc_monthly_averages,
@@ -81,15 +82,15 @@
         if return_format == 'xarray' and product_name == 'forecastensembles':
             ds = ds.rename({'time': 'datetime', 'rivid': 'river_id'})
             ds.attrs = attrs
             return ds
         df = ds.to_dataframe().round(2).reset_index()
 
         # rename columns to match the REST API
-        if isinstance(river_id, int):
+        if isinstance(river_id, int) or isinstance(river_id, np.int64):
             df = df.pivot(index='time', columns='ensemble', values='Qout')
         else:
             df = df.pivot(index=['time', 'rivid'], columns='ensemble', values='Qout')
             df.index.names = ['time', 'river_id']
         df = df[sorted(df.columns)]
         df.columns = [f'ensemble_{str(x).zfill(2)}' for x in df.columns]
 
@@ -116,26 +117,26 @@
         # parse out the information necessary to build a request url
         endpoint = kwargs.get('endpoint', DEFAULT_REST_ENDPOINT)
         endpoint = endpoint[:-1] if endpoint[-1] == '/' else endpoint
         endpoint = endpoint + '/api' if not endpoint.endswith('/api') else endpoint
         endpoint = f'https://{endpoint}' if not endpoint.startswith(('https://', 'http://')) else endpoint
 
         version = kwargs.get('version', DEFAULT_REST_ENDPOINT_VERSION)
-        assert version in ('v1', 'v2', ), ValueError(f'Unrecognized model version parameter: {version}')
+        assert version in ('v2', ), ValueError(f'Unrecognized model version parameter: {version}')
 
         product_name = function.__name__.replace("_", "").lower()
 
         river_id = args[0] if len(args) > 0 else None
         river_id = kwargs.get('river_id', '') if not river_id else river_id
         if isinstance(river_id, list):
             raise ValueError('Multiple river_ids are not available via REST API or on v1. '
                              'Use data_source="aws" and version="v2" for multiple river_ids.')
         river_id = int(river_id) if river_id else None
         if river_id and version == 'v2':
-            assert river_id < 1_000_000_000 and river_id >= 110_000_000, ValueError('River ID must be a 9 digit integer')
+            assert 1_000_000_000 > river_id >= 110_000_000, ValueError('River ID must be a 9 digit integer')
 
         # request parameter validation before submitting
         for key in ('endpoint', 'version', 'river_id'):
             if key in kwargs:
                 del kwargs[key]
         for key, value in kwargs.items():
             if value is None:
@@ -174,121 +175,119 @@
             raise ValueError(f'Unsupported return format requested: {return_format}')
 
     def main(*args, **kwargs):
         source = kwargs.get('data_source', 'aws')
         assert source in ('rest', 'aws'), ValueError(f'Unrecognized data source requested: {source}')
         if source == 'rest':
             return from_rest(*args, **kwargs)
-        else:
-            return from_aws(*args, **kwargs)
+        return from_aws(*args, **kwargs)
     main.__doc__ = function.__doc__  # necessary for code documentation auto generators
     return main
 
 
 # Forecast data and derived products
 @_forecast_endpoint_decorator
 def dates(**kwargs) -> dict or str:
     """
     Gets a list of available forecast product dates
 
     Keyword Args:
-        data_source: location to query for data, either 'rest' or 'aws'. default is aws.
+        data_source (str): location to query for data, either 'rest' or 'aws'. default is aws.
 
     Returns:
         dict or str
 
         the csv is a single column with a header of 'available_dates' and 1 row per date, sorted oldest to newest
         The dictionary structure is {'available_dates': ['list', 'of', 'dates', 'YYYYMMDD', 'format']}
     """
     pass
 
 
 @_forecast_endpoint_decorator
 def forecast(*, river_id: int, date: str, format: str, data_source: str,
-             **kwargs) -> pd.DataFrame or dict or str:
+             **kwargs) -> pd.DataFrame or xr.Dataset:
     """
     Gets the average forecasted flow for a certain river_id on a certain date
 
     Keyword Args:
-        river_id (str): the ID of a stream, should be a 9 digit integer
+        river_id (int): the ID of a stream, should be a 9 digit integer
         date (str): a string specifying the date to request in YYYYMMDD format, returns the latest available if not specified
-        format (str): csv, json, or url, default csv
+        format: if data_source=="rest": csv, json, or url, default csv. if data_source=="aws": df or xarray
         data_source (str): location to query for data, either 'rest' or 'aws'. default is aws.
 
     Returns:
         pd.DataFrame or dict or str
     """
     pass
 
 
 @_forecast_endpoint_decorator
 def forecast_stats(*, river_id: int, date: str, format: str, data_source: str,
-                   **kwargs) -> pd.DataFrame or dict or str:
+                   **kwargs) -> pd.DataFrame or xr.Dataset:
     """
     Retrieves the min, 25%, mean, median, 75%, and max river discharge of the 51 ensembles members for a river_id
     The 52nd higher resolution member is excluded
 
     Keyword Args:
-        river_id: the ID of a stream, should be a 9 digit integer
-        date: a string specifying the date to request in YYYYMMDD format, returns the latest available if not specified
-        format: if data_source=="rest": csv, json, or url, default csv. if data_source=="aws": df or xarray
-        data_source: location to query for data, either 'rest' or 'aws'. default is aws.
+        river_id (int): the ID of a stream, should be a 9 digit integer
+        date (str): a string specifying the date to request in YYYYMMDD format, returns the latest available if not specified
+        format (str): if data_source=="rest": csv, json, or url, default csv. if data_source=="aws": df or xarray
+        data_source (str): location to query for data, either 'rest' or 'aws'. default is aws.
 
     Returns:
         pd.DataFrame or dict or str
     """
     pass
 
 
 @_forecast_endpoint_decorator
 def forecast_ensembles(*, river_id: int, date: str, format: str, data_source: str,
-                       **kwargs) -> pd.DataFrame or dict or str:
+                       **kwargs) -> pd.DataFrame or xr.Dataset:
     """
     Retrieves each of 52 time series of forecasted discharge for a river_id on a certain date
 
     Keyword Args:
-        river_id: the ID of a stream, should be a 9 digit integer
-        date: a string specifying the date to request in YYYYMMDD format, returns the latest available if not specified
-        format: if data_source=="rest": csv, json, or url, default csv. if data_source=="aws": df or xarray
-        data_source: location to query for data, either 'rest' or 'aws'. default is aws.
+        river_id (int): the ID of a stream, should be a 9 digit integer
+        date (str): a string specifying the date to request in YYYYMMDD format, returns the latest available if not specified
+        format (str): if data_source=="rest": csv, json, or url, default csv. if data_source=="aws": df or xarray
+        data_source (str): location to query for data, either 'rest' or 'aws'. default is aws.
 
     Returns:
         pd.DataFrame or dict or str
     """
     pass
 
 
 @_forecast_endpoint_decorator
-def forecast_records(*, river_id: int, start_date: str, end_date: str, format: str, data_source: str,
+def forecast_records(*, river_id: int, start_date: str, end_date: str, format: str,
                      **kwargs) -> pd.DataFrame or dict or str:
     """
     Retrieves a csv showing the ensemble average forecasted flow for the year from January 1 to the current date
 
     Keyword Args:
-        river_id: the ID of a stream, should be a 9 digit integer
-        start_date: a YYYYMMDD string giving the earliest date this year to include, defaults to 14 days ago.
-        end_date: a YYYYMMDD string giving the latest date this year to include, defaults to latest available
-        data_source: location to query for data, either 'rest' or 'aws'. default is aws.
-        format: if data_source=="rest": csv, json, or url, default csv. if data_source=="aws": df or xarray
+        river_id (int): the ID of a stream, should be a 9 digit integer
+        start_date (str): a YYYYMMDD string giving the earliest date this year to include, defaults to 14 days ago.
+        end_date (str): a YYYYMMDD string giving the latest date this year to include, defaults to latest available
+        format (str): csv, json, or url, default csv.
 
     Returns:
         pd.DataFrame or dict or str
     """
     pass
 
 
 # Retrospective simulation and derived products
 def retrospective(river_id: int or list, format: str = 'df') -> pd.DataFrame or xr.Dataset:
     """
     Retrieves the retrospective simulation of streamflow for a given river_id from the
-    AWS Open Data Program GEOGloWS V2 S3 bucket
+    AWS Open Data Program GEOGLOWS V2 S3 bucket
 
     Args:
-        river_id: the ID of a stream, should be a 9 digit integer
-        format: the format to return the data, either 'df' or 'xarray'. default is 'df'
+        river_id (int): the ID of a stream, should be a 9 digit integer
+        format (str): the format to return the data, either 'df' or 'xarray'. default is 'df'
 
     Returns:
         pd.DataFrame
     """
     s3 = s3fs.S3FileSystem(anon=True, client_kwargs=dict(region_name=ODP_S3_BUCKET_REGION))
     s3store = s3fs.S3Map(root=f'{ODP_RETROSPECTIVE_S3_BUCKET_URI}/retrospective.zarr', s3=s3, check=False)
     ds = xr.open_zarr(s3store).sel(rivid=river_id)
@@ -298,63 +297,63 @@
 
 
 def historical(*args, **kwargs):
     """Alias for retrospective"""
     return retrospective(*args, **kwargs)
 
 
-def daily_averages(river_id: int or list) -> pd.DataFrame or xr.Dataset:
+def daily_averages(river_id: int or list) -> pd.DataFrame:
     """
     Retrieves daily average streamflow for a given river_id
 
     Args:
-        river_id: the ID of a stream, should be a 9 digit integer
+        river_id (int): the ID of a stream, should be a 9 digit integer
 
     Returns:
         pd.DataFrame
     """
     df = retrospective(river_id)
     return calc_daily_averages(df)
 
 
 def monthly_averages(river_id: int or list) -> pd.DataFrame:
     """
     Retrieves monthly average streamflow for a given river_id
 
     Args:
-        river_id: the ID of a stream, should be a 9 digit integer
+        river_id (int): the ID of a stream, should be a 9 digit integer
 
     Returns:
         pd.DataFrame
     """
     df = retrospective(river_id)
     return calc_monthly_averages(df)
 
 
 def annual_averages(river_id: int or list) -> pd.DataFrame:
     """
     Retrieves annual average streamflow for a given river_id
 
     Args:
-        river_id: the ID of a stream, should be a 9 digit integer
+        river_id (int): the ID of a stream, should be a 9 digit integer
 
     Returns:
         pd.DataFrame
     """
     df = retrospective(river_id)
     return calc_annual_averages(df)
 
 
-def return_periods(river_id: int or list, format: str = 'df') -> pd.DataFrame:
+def return_periods(river_id: int or list, format: str = 'df') -> pd.DataFrame or xr.Dataset:
     """
     Retrieves the return period thresholds based on a specified historic simulation forcing on a certain river_id.
 
     Args:
-        river_id: the ID of a stream, should be a 9 digit integer
-        format: the format to return the data, either 'df' or 'xarray'. default is 'df'
+        river_id (int): the ID of a stream, should be a 9 digit integer
+        format (str): the format to return the data, either 'df' or 'xarray'. default is 'df'
 
     Returns:
         pd.DataFrame
     """
     s3 = s3fs.S3FileSystem(anon=True, client_kwargs=dict(region_name=ODP_S3_BUCKET_REGION))
     s3store = s3fs.S3Map(root=f'{ODP_RETROSPECTIVE_S3_BUCKET_URI}/return-periods.zarr', s3=s3, check=False)
     ds = xr.open_zarr(s3store).sel(rivid=river_id)
@@ -365,23 +364,24 @@
 
 
 # model config and supplementary data
 def metadata_tables(columns: list = None) -> pd.DataFrame:
     """
     Retrieves the master table of rivers metadata and properties as a pandas DataFrame
     Args:
-        columns: optional subset of columns names to read from the parquet
+        columns (list): optional subset of columns names to read from the parquet
 
     Returns:
         pd.DataFrame
     """
     if os.path.exists(METADATA_TABLE_PATH):
         return pd.read_parquet(METADATA_TABLE_PATH, columns=columns)
     warn = f"""
     Local copy of geoglows v2 metadata table not found. You should download a copy for optimal performance and 
     to make the data available when you are offline. A copy of the table will be cached at {METADATA_TABLE_PATH}.
+    Alternatively, set the environment variable PYGEOGLOWS_METADATA_TABLE_PATH to the path of the table.
     """
     warnings.warn(warn)
     df = pd.read_parquet('https://geoglows-v2.s3-website-us-west-2.amazonaws.com/tables/package-metadata-table.parquet')
     os.makedirs(os.path.dirname(METADATA_TABLE_PATH), exist_ok=True)
     df.to_parquet(METADATA_TABLE_PATH)
     return df[columns] if columns else df
```

### Comparing `geoglows-1.2.0/geoglows/streamflow.py` & `geoglows-1.2.1/geoglows/streamflow.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.0/geoglows/tables.py` & `geoglows-1.2.1/geoglows/tables.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.0/geoglows.egg-info/PKG-INFO` & `geoglows-1.2.1/geoglows.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.2.0
+Version: 1.2.1
 Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
```

### Comparing `geoglows-1.2.0/geoglows.egg-info/SOURCES.txt` & `geoglows-1.2.1/geoglows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geoglows-1.2.0/setup.py` & `geoglows-1.2.1/setup.py`

 * *Files identical despite different names*

