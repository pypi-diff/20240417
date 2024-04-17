# Comparing `tmp/speasy-1.2.5.tar.gz` & `tmp/speasy-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speasy-1.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "speasy-1.2.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `speasy-1.2.5.tar` & `speasy-1.2.6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1660 2024-04-17 08:07:34.727636 speasy-1.2.5/LICENSE
--rw-r--r--   0        0        0     9241 2024-04-17 08:07:34.727636 speasy-1.2.5/README.md
--rw-r--r--   0        0        0     1423 2024-04-17 08:07:34.799636 speasy-1.2.5/pyproject.toml
--rw-r--r--   0        0        0      966 2024-04-17 08:07:34.799636 speasy-1.2.5/speasy/__init__.py
--rw-r--r--   0        0        0     7936 2024-04-17 08:07:34.799636 speasy-1.2.5/speasy/config/__init__.py
--rw-r--r--   0        0        0     6636 2024-04-17 08:07:34.799636 speasy-1.2.5/speasy/core/__init__.py
--rw-r--r--   0        0        0     4905 2024-04-17 08:07:34.799636 speasy-1.2.5/speasy/core/any_files.py
--rw-r--r--   0        0        0      576 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/core/cache/__init__.py
--rw-r--r--   0        0        0     2061 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/core/cache/_function_cache.py
--rw-r--r--   0        0        0      100 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/core/cache/_instance.py
--rw-r--r--   0        0        0    14358 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/core/cache/_providers_caches.py
--rw-r--r--   0        0        0     2659 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/core/cache/cache.py
--rw-r--r--   0        0        0     1941 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/core/cache/version.py
--rw-r--r--   0        0        0     3505 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/core/cdf/__init__.py
--rw-r--r--   0        0        0     3322 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/core/cdf/inventory_extractor.py
--rw-r--r--   0        0        0     8835 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/core/data_containers.py
--rw-r--r--   0        0        0     5080 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/core/dataprovider.py
--rw-r--r--   0        0        0     2204 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/core/datetime_range.py
--rw-r--r--   0        0        0       51 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/core/direct_archive_downloader/__init__.py
--rw-r--r--   0        0        0     7877 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/core/direct_archive_downloader/direct_archive_downloader.py
--rw-r--r--   0        0        0     4083 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/core/http.py
--rw-r--r--   0        0        0       80 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/core/index/__init__.py
--rw-r--r--   0        0        0      525 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/core/index/speasy_index.py
--rw-r--r--   0        0        0     1871 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/core/inventory/__init__.py
--rw-r--r--   0        0        0     4975 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/core/inventory/indexes.py
--rw-r--r--   0        0        0     5325 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/core/proxy/__init__.py
--rw-r--r--   0        0        0       92 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/core/requests_scheduling/__init__.py
--rw-r--r--   0        0        0    12388 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/core/requests_scheduling/request_dispatch.py
--rw-r--r--   0        0        0     1175 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/core/requests_scheduling/split_large_requests.py
--rw-r--r--   0        0        0     3500 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/core/span_utils.py
--rw-r--r--   0        0        0     1980 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/core/url_utils.py
--rw-r--r--   0        0        0     6003 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/data/archive/cda.yaml
--rw-r--r--   0        0        0    17130 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/data/archive/themis_cdpp.yaml
--rw-r--r--   0        0        0      165 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/inventories/__init__.py
--rw-r--r--   0        0        0     2875 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/plotting/__init__.py
--rw-r--r--   0        0        0     2240 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/plotting/mpl_backend/__init__.py
--rw-r--r--   0        0        0      686 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/products/__init__.py
--rw-r--r--   0        0        0      241 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/products/base_product.py
--rw-r--r--   0        0        0     4582 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/products/catalog.py
--rw-r--r--   0        0        0     1654 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/products/dataset.py
--rw-r--r--   0        0        0     1696 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/products/timetable.py
--rw-r--r--   0        0        0    18641 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/products/variable.py
--rw-r--r--   0        0        0      174 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/webservices/__init__.py
--rw-r--r--   0        0        0     1729 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/webservices/amda/__init__.py
--rw-r--r--   0        0        0     9427 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/webservices/amda/_impl.py
--rw-r--r--   0        0        0       46 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/webservices/amda/exceptions.py
--rw-r--r--   0        0        0     6050 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/webservices/amda/inventory.py
--rw-r--r--   0        0        0    11888 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/webservices/amda/rest_client.py
--rw-r--r--   0        0        0     6965 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/webservices/amda/utils.py
--rw-r--r--   0        0        0    25547 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/webservices/amda/ws.py
--rw-r--r--   0        0        0     7199 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/webservices/cda/__init__.py
--rw-r--r--   0        0        0     2933 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/webservices/cda/_inventory_builder/__init__.py
--rw-r--r--   0        0        0     1564 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/webservices/cda/_inventory_builder/_cdf_masters_parser.py
--rw-r--r--   0        0        0     3456 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/webservices/cda/_inventory_builder/_xml_catalogs_parser.py
--rw-r--r--   0        0        0     9942 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/webservices/csa/__init__.py
--rw-r--r--   0        0        0     4732 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/webservices/generic_archive/__init__.py
--rw-r--r--   0        0        0     5776 2024-04-17 08:07:34.803636 speasy-1.2.5/speasy/webservices/ssc/__init__.py
--rw-r--r--   0        0        0    10687 1970-01-01 00:00:00.000000 speasy-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1660 2024-04-17 09:29:45.077110 speasy-1.2.6/LICENSE
+-rw-r--r--   0        0        0     9241 2024-04-17 09:29:45.081110 speasy-1.2.6/README.md
+-rw-r--r--   0        0        0     1423 2024-04-17 09:29:45.153110 speasy-1.2.6/pyproject.toml
+-rw-r--r--   0        0        0      966 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/__init__.py
+-rw-r--r--   0        0        0     7936 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/config/__init__.py
+-rw-r--r--   0        0        0     6636 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/core/__init__.py
+-rw-r--r--   0        0        0     4905 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/core/any_files.py
+-rw-r--r--   0        0        0      576 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/core/cache/__init__.py
+-rw-r--r--   0        0        0     2061 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/core/cache/_function_cache.py
+-rw-r--r--   0        0        0      100 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/core/cache/_instance.py
+-rw-r--r--   0        0        0    14358 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/core/cache/_providers_caches.py
+-rw-r--r--   0        0        0     2659 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/core/cache/cache.py
+-rw-r--r--   0        0        0     1941 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/core/cache/version.py
+-rw-r--r--   0        0        0     3505 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/core/cdf/__init__.py
+-rw-r--r--   0        0        0     3322 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/core/cdf/inventory_extractor.py
+-rw-r--r--   0        0        0     8835 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/core/data_containers.py
+-rw-r--r--   0        0        0     5080 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/core/dataprovider.py
+-rw-r--r--   0        0        0     2204 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/core/datetime_range.py
+-rw-r--r--   0        0        0       51 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/core/direct_archive_downloader/__init__.py
+-rw-r--r--   0        0        0     7877 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/core/direct_archive_downloader/direct_archive_downloader.py
+-rw-r--r--   0        0        0     4083 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/core/http.py
+-rw-r--r--   0        0        0       80 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/core/index/__init__.py
+-rw-r--r--   0        0        0      525 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/core/index/speasy_index.py
+-rw-r--r--   0        0        0     1871 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/core/inventory/__init__.py
+-rw-r--r--   0        0        0     4975 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/core/inventory/indexes.py
+-rw-r--r--   0        0        0     5325 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/core/proxy/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/core/requests_scheduling/__init__.py
+-rw-r--r--   0        0        0    12388 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/core/requests_scheduling/request_dispatch.py
+-rw-r--r--   0        0        0     1175 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/core/requests_scheduling/split_large_requests.py
+-rw-r--r--   0        0        0     3500 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/core/span_utils.py
+-rw-r--r--   0        0        0     1980 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/core/url_utils.py
+-rw-r--r--   0        0        0     6003 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/data/archive/cda.yaml
+-rw-r--r--   0        0        0    17130 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/data/archive/themis_cdpp.yaml
+-rw-r--r--   0        0        0      165 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/inventories/__init__.py
+-rw-r--r--   0        0        0     2875 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/plotting/__init__.py
+-rw-r--r--   0        0        0     2240 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/plotting/mpl_backend/__init__.py
+-rw-r--r--   0        0        0      686 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/products/__init__.py
+-rw-r--r--   0        0        0      241 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/products/base_product.py
+-rw-r--r--   0        0        0     4582 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/products/catalog.py
+-rw-r--r--   0        0        0     1654 2024-04-17 09:29:45.153110 speasy-1.2.6/speasy/products/dataset.py
+-rw-r--r--   0        0        0     1696 2024-04-17 09:29:45.157110 speasy-1.2.6/speasy/products/timetable.py
+-rw-r--r--   0        0        0    18641 2024-04-17 09:29:45.157110 speasy-1.2.6/speasy/products/variable.py
+-rw-r--r--   0        0        0      174 2024-04-17 09:29:45.157110 speasy-1.2.6/speasy/webservices/__init__.py
+-rw-r--r--   0        0        0     1729 2024-04-17 09:29:45.157110 speasy-1.2.6/speasy/webservices/amda/__init__.py
+-rw-r--r--   0        0        0     9427 2024-04-17 09:29:45.157110 speasy-1.2.6/speasy/webservices/amda/_impl.py
+-rw-r--r--   0        0        0       46 2024-04-17 09:29:45.157110 speasy-1.2.6/speasy/webservices/amda/exceptions.py
+-rw-r--r--   0        0        0     6050 2024-04-17 09:29:45.157110 speasy-1.2.6/speasy/webservices/amda/inventory.py
+-rw-r--r--   0        0        0    11888 2024-04-17 09:29:45.157110 speasy-1.2.6/speasy/webservices/amda/rest_client.py
+-rw-r--r--   0        0        0     6965 2024-04-17 09:29:45.157110 speasy-1.2.6/speasy/webservices/amda/utils.py
+-rw-r--r--   0        0        0    25547 2024-04-17 09:29:45.157110 speasy-1.2.6/speasy/webservices/amda/ws.py
+-rw-r--r--   0        0        0     7199 2024-04-17 09:29:45.157110 speasy-1.2.6/speasy/webservices/cda/__init__.py
+-rw-r--r--   0        0        0     2933 2024-04-17 09:29:45.157110 speasy-1.2.6/speasy/webservices/cda/_inventory_builder/__init__.py
+-rw-r--r--   0        0        0     1564 2024-04-17 09:29:45.157110 speasy-1.2.6/speasy/webservices/cda/_inventory_builder/_cdf_masters_parser.py
+-rw-r--r--   0        0        0     3456 2024-04-17 09:29:45.157110 speasy-1.2.6/speasy/webservices/cda/_inventory_builder/_xml_catalogs_parser.py
+-rw-r--r--   0        0        0     9942 2024-04-17 09:29:45.157110 speasy-1.2.6/speasy/webservices/csa/__init__.py
+-rw-r--r--   0        0        0     4732 2024-04-17 09:29:45.157110 speasy-1.2.6/speasy/webservices/generic_archive/__init__.py
+-rw-r--r--   0        0        0     5757 2024-04-17 09:29:45.157110 speasy-1.2.6/speasy/webservices/ssc/__init__.py
+-rw-r--r--   0        0        0    10687 1970-01-01 00:00:00.000000 speasy-1.2.6/PKG-INFO
```

### Comparing `speasy-1.2.5/LICENSE` & `speasy-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/README.md` & `speasy-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/pyproject.toml` & `speasy-1.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core"]
 
 [project]
 name = 'speasy'
-version = "1.2.5"
+version = "1.2.6"
 description = "A simple Python package to deal with main Space Physics WebServices (CDA, CSA, AMDA and SSC)."
 keywords = ["satellite", "plasma-physics", "nasa-data", "amda", "cdpp", "CDF"]
 authors = [
     { name = "Alexis Jeandet", email = "alexis.jeandet@member.fsf.org" }
 ]
 
 maintainers = [
```

### Comparing `speasy-1.2.5/speasy/__init__.py` & `speasy-1.2.6/speasy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
    import speasy as spz
 
 """
 
 __author__ = """Alexis Jeandet"""
 __email__ = 'alexis.jeandet@member.fsf.org'
-__version__ = '1.2.5'
+__version__ = '1.2.6'
 __all__ = ['amda', 'cda', 'ssc', 'csa', 'get_data', 'archive', 'SpeasyVariable', 'Catalog', 'Event', 'Dataset', 'TimeTable']
 __docformat__ = "numpy"
 
 from typing import List
 
 from speasy.core.inventory.indexes import SpeasyIndex
 from .products import SpeasyVariable, Catalog, Event, Dataset, TimeTable, MaybeAnyProduct
```

### Comparing `speasy-1.2.5/speasy/config/__init__.py` & `speasy-1.2.6/speasy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/core/__init__.py` & `speasy-1.2.6/speasy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/core/any_files.py` & `speasy-1.2.6/speasy/core/any_files.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/core/cache/__init__.py` & `speasy-1.2.6/speasy/core/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/core/cache/_function_cache.py` & `speasy-1.2.6/speasy/core/cache/_function_cache.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/core/cache/_providers_caches.py` & `speasy-1.2.6/speasy/core/cache/_providers_caches.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/core/cache/cache.py` & `speasy-1.2.6/speasy/core/cache/cache.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/core/cache/version.py` & `speasy-1.2.6/speasy/core/cache/version.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/core/cdf/__init__.py` & `speasy-1.2.6/speasy/core/cdf/__init__.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/core/cdf/inventory_extractor.py` & `speasy-1.2.6/speasy/core/cdf/inventory_extractor.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/core/data_containers.py` & `speasy-1.2.6/speasy/core/data_containers.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/core/dataprovider.py` & `speasy-1.2.6/speasy/core/dataprovider.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/core/datetime_range.py` & `speasy-1.2.6/speasy/core/datetime_range.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/core/direct_archive_downloader/direct_archive_downloader.py` & `speasy-1.2.6/speasy/core/direct_archive_downloader/direct_archive_downloader.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/core/http.py` & `speasy-1.2.6/speasy/core/http.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/core/index/speasy_index.py` & `speasy-1.2.6/speasy/core/index/speasy_index.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/core/inventory/__init__.py` & `speasy-1.2.6/speasy/core/inventory/__init__.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/core/inventory/indexes.py` & `speasy-1.2.6/speasy/core/inventory/indexes.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/core/proxy/__init__.py` & `speasy-1.2.6/speasy/core/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/core/requests_scheduling/request_dispatch.py` & `speasy-1.2.6/speasy/core/requests_scheduling/request_dispatch.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/core/requests_scheduling/split_large_requests.py` & `speasy-1.2.6/speasy/core/requests_scheduling/split_large_requests.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/core/span_utils.py` & `speasy-1.2.6/speasy/core/span_utils.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/core/url_utils.py` & `speasy-1.2.6/speasy/core/url_utils.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/data/archive/cda.yaml` & `speasy-1.2.6/speasy/data/archive/cda.yaml`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/data/archive/themis_cdpp.yaml` & `speasy-1.2.6/speasy/data/archive/themis_cdpp.yaml`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/plotting/__init__.py` & `speasy-1.2.6/speasy/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/plotting/mpl_backend/__init__.py` & `speasy-1.2.6/speasy/plotting/mpl_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/products/__init__.py` & `speasy-1.2.6/speasy/products/__init__.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/products/catalog.py` & `speasy-1.2.6/speasy/products/catalog.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/products/dataset.py` & `speasy-1.2.6/speasy/products/dataset.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/products/timetable.py` & `speasy-1.2.6/speasy/products/timetable.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/products/variable.py` & `speasy-1.2.6/speasy/products/variable.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/webservices/amda/__init__.py` & `speasy-1.2.6/speasy/webservices/amda/__init__.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/webservices/amda/_impl.py` & `speasy-1.2.6/speasy/webservices/amda/_impl.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/webservices/amda/inventory.py` & `speasy-1.2.6/speasy/webservices/amda/inventory.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/webservices/amda/rest_client.py` & `speasy-1.2.6/speasy/webservices/amda/rest_client.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/webservices/amda/utils.py` & `speasy-1.2.6/speasy/webservices/amda/utils.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/webservices/amda/ws.py` & `speasy-1.2.6/speasy/webservices/amda/ws.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/webservices/cda/__init__.py` & `speasy-1.2.6/speasy/webservices/cda/__init__.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/webservices/cda/_inventory_builder/__init__.py` & `speasy-1.2.6/speasy/webservices/cda/_inventory_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/webservices/cda/_inventory_builder/_cdf_masters_parser.py` & `speasy-1.2.6/speasy/webservices/cda/_inventory_builder/_cdf_masters_parser.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/webservices/cda/_inventory_builder/_xml_catalogs_parser.py` & `speasy-1.2.6/speasy/webservices/cda/_inventory_builder/_xml_catalogs_parser.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/webservices/csa/__init__.py` & `speasy-1.2.6/speasy/webservices/csa/__init__.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/webservices/generic_archive/__init__.py` & `speasy-1.2.6/speasy/webservices/generic_archive/__init__.py`

 * *Files identical despite different names*

### Comparing `speasy-1.2.5/speasy/webservices/ssc/__init__.py` & `speasy-1.2.6/speasy/webservices/ssc/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,42 +17,42 @@
 from speasy.core.datetime_range import DateTimeRange
 from speasy.core.inventory.indexes import ParameterIndex, SpeasyIndex
 from speasy.core.proxy import Proxyfiable, GetProduct, PROXY_ALLOWED_KWARGS
 from speasy.core.requests_scheduling import SplitLargeRequests
 from speasy.products.variable import SpeasyVariable, VariableTimeAxis, DataContainer
 from ...core import AllowedKwargs, http
 
-log = logging.getLogger(__name__)
-
-
-def _make_datetime(dt: str) -> np.datetime64:
-    '''
-        Hack to support python 3.6, once 3.6 support removed then go back to:
-        datetime.strptime(v[1], '%Y-%m-%dT%H:%M:%S.%f%z').timestamp()
-    '''
-    return np.datetime64(dt[:-6], 'ns')
-
 
 def _variable(orbit: dict) -> Optional[SpeasyVariable]:
-    data = orbit['Result']['Data'][1][0]['Coordinates'][1][0]
-    keys = list(data.keys())
-    keys.remove('CoordinateSystem')
+    data = orbit['Result'][1]['Data'][1][0][1]['Coordinates'][1][0][1]
+    time = orbit['Result'][1]['Data'][1][0][1]['Time'][1]
     values = np.array([data['X'][1], data['Y'][1], data['Z'][1]]).transpose()
+
     # this is damn slow!
-    time_axis = np.array([_make_datetime(v[1]) for v in
-                          orbit['Result']['Data'][1][0]['Time'][1]])
+    time_axis = np.array([_make_datetime(v[1]) for v in time])
     return SpeasyVariable(
         axes=[VariableTimeAxis(values=time_axis)],
         values=DataContainer(values, meta={'CoordinateSystem': data['CoordinateSystem'], 'UNITS': 'km'}),
         columns=['X', 'Y', 'Z']
     )
 
 
+log = logging.getLogger(__name__)
+
+
+def _make_datetime(dt: str) -> np.datetime64:
+    '''
+        Hack to support python 3.6, once 3.6 support removed then go back to:
+        datetime.strptime(v[1], '%Y-%m-%dT%H:%M:%S.%f%z').timestamp()
+    '''
+    return np.datetime64(dt[:-6], 'ns')
+
+
 def _is_valid(orbit: dict):
-    return orbit['Result']['StatusCode'] == 'SUCCESS' and orbit['Result']['StatusSubCode'] == 'SUCCESS'
+    return orbit['Result'][1]['StatusCode'] == 'SUCCESS' and orbit['Result'][1]['StatusSubCode'] == 'SUCCESS'
 
 
 def _make_cache_entry_name(prefix: str, product: str, start_time: str, **kwargs):
     return f"{prefix}/{product}/{kwargs.get('coordinate_system', 'gse')}/{start_time}"
 
 
 def get_parameter_args(start_time: datetime, stop_time: datetime, product: str, **kwargs):
@@ -82,15 +82,15 @@
         return root
 
     @CacheCall(cache_retention=7 * 24 * 60 * 60, is_pure=True)
     def get_observatories(self):
         res = http.get(f"{self.__url}/observatories", headers={"Accept": "application/json"})
         if not res.ok:
             return None
-        return res.json()['Observatory'][1]
+        return list(map(lambda x: x[1], res.json()[1]['Observatory'][1]))
 
     def version(self, product):
         return 2
 
     def parameter_range(self, parameter_id: str or ParameterIndex) -> Optional[DateTimeRange]:
         """Get product time range.
 
@@ -134,11 +134,11 @@
         url = f"{self.__url}/locations/{product}/{start_time.strftime('%Y%m%dT%H%M%SZ')},{stop_time.strftime('%Y%m%dT%H%M%SZ')}/{coordinate_system.lower()}/"
         if debug:
             print(url)
         headers = {"Accept": "application/json"}
         if extra_http_headers is not None:
             headers.update(extra_http_headers)
         res = http.get(url, headers=headers)
-        orbit = res.json()
+        orbit = res.json()[1]
         if res.ok and _is_valid(orbit):
             return _variable(orbit)[start_time:stop_time]
         return None
```

### Comparing `speasy-1.2.5/PKG-INFO` & `speasy-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speasy
-Version: 1.2.5
+Version: 1.2.6
 Summary: A simple Python package to deal with main Space Physics WebServices (CDA, CSA, AMDA and SSC).
 Keywords: satellite,plasma-physics,nasa-data,amda,cdpp,CDF
 Author-email: Alexis Jeandet <alexis.jeandet@member.fsf.org>
 Maintainer-email: Alexis Jeandet <alexis.jeandet@member.fsf.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
```

