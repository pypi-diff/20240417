# Comparing `tmp/fastramqpi-7.1.0.tar.gz` & `tmp/fastramqpi-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastramqpi-7.1.0.tar", max compression
+gzip compressed data, was "fastramqpi-7.2.0.tar", max compression
```

## Comparing `fastramqpi-7.1.0.tar` & `fastramqpi-7.2.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0        0        0        0 2024-04-09 13:39:59.748712 fastramqpi-7.1.0/LICENSES/
--rw-r--r--   0        0        0    15177 2024-04-09 13:39:59.748712 fastramqpi-7.1.0/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0    14146 2024-04-09 13:39:59.749712 fastramqpi-7.1.0/README.md
--rw-r--r--   0        0        0       85 2024-04-09 13:39:59.759712 fastramqpi-7.1.0/fastramqpi/__init__.py
--rw-r--r--   0        0        0     7425 2024-04-09 13:39:59.759712 fastramqpi-7.1.0/fastramqpi/app.py
--rw-r--r--   0        0        0     2207 2024-04-09 13:39:59.759712 fastramqpi-7.1.0/fastramqpi/config.py
--rw-r--r--   0        0        0     1620 2024-04-09 13:39:59.759712 fastramqpi-7.1.0/fastramqpi/context.py
--rw-r--r--   0        0        0     1498 2024-04-09 13:39:59.759712 fastramqpi-7.1.0/fastramqpi/depends.py
--rw-r--r--   0        0        0     6738 2024-04-09 13:39:59.760712 fastramqpi-7.1.0/fastramqpi/main.py
--rw-r--r--   0        0        0      477 2024-04-09 13:39:59.760712 fastramqpi-7.1.0/fastramqpi/metrics.py
--rw-r--r--   0        0        0        0 2024-04-09 13:39:59.898722 fastramqpi-7.1.0/fastramqpi/py.typed
--rw-r--r--   0        0        0     3185 2024-04-09 13:39:59.760712 fastramqpi-7.1.0/fastramqpi/pytest_plugin.py
--rw-r--r--   0        0        0      884 2024-04-09 13:39:59.760712 fastramqpi-7.1.0/fastramqpi/pytest_util.py
--rw-r--r--   0        0        0       99 2024-04-09 13:39:59.760712 fastramqpi-7.1.0/fastramqpi/ra_utils/__init__.py
--rw-r--r--   0        0        0     2263 2024-04-09 13:39:59.761712 fastramqpi-7.1.0/fastramqpi/ra_utils/apply.py
--rw-r--r--   0        0        0     1051 2024-04-09 13:39:59.761712 fastramqpi-7.1.0/fastramqpi/ra_utils/async_to_sync.py
--rw-r--r--   0        0        0     2496 2024-04-09 13:39:59.761712 fastramqpi-7.1.0/fastramqpi/ra_utils/asyncio_utils.py
--rw-r--r--   0        0        0      805 2024-04-09 13:39:59.761712 fastramqpi-7.1.0/fastramqpi/ra_utils/attrdict.py
--rw-r--r--   0        0        0     1539 2024-04-09 13:39:59.761712 fastramqpi-7.1.0/fastramqpi/ra_utils/catchtime.py
--rw-r--r--   0        0        0      979 2024-04-09 13:39:59.761712 fastramqpi-7.1.0/fastramqpi/ra_utils/deprecation.py
--rw-r--r--   0        0        0     3961 2024-04-09 13:39:59.762713 fastramqpi-7.1.0/fastramqpi/ra_utils/dict_map.py
--rw-r--r--   0        0        0     2184 2024-04-09 13:39:59.762713 fastramqpi-7.1.0/fastramqpi/ra_utils/ensure_hashable.py
--rw-r--r--   0        0        0     3808 2024-04-09 13:39:59.762713 fastramqpi-7.1.0/fastramqpi/ra_utils/ensure_single_run.py
--rw-r--r--   0        0        0     1723 2024-04-09 13:39:59.762713 fastramqpi-7.1.0/fastramqpi/ra_utils/generate_uuid.py
--rw-r--r--   0        0        0     5633 2024-04-09 13:39:59.762713 fastramqpi-7.1.0/fastramqpi/ra_utils/headers.py
--rw-r--r--   0        0        0     3245 2024-04-09 13:39:59.763713 fastramqpi-7.1.0/fastramqpi/ra_utils/jinja_filter.py
--rw-r--r--   0        0        0     7347 2024-04-09 13:39:59.763713 fastramqpi-7.1.0/fastramqpi/ra_utils/job_settings.py
--rw-r--r--   0        0        0     6027 2024-04-09 13:39:59.763713 fastramqpi-7.1.0/fastramqpi/ra_utils/lazy_dict.py
--rw-r--r--   0        0        0     2929 2024-04-09 13:39:59.763713 fastramqpi-7.1.0/fastramqpi/ra_utils/load_settings.py
--rw-r--r--   0        0        0     2935 2024-04-09 13:39:59.763713 fastramqpi-7.1.0/fastramqpi/ra_utils/multiple_replace.py
--rw-r--r--   0        0        0     2891 2024-04-09 13:39:59.764713 fastramqpi-7.1.0/fastramqpi/ra_utils/semantic_version_type.py
--rw-r--r--   0        0        0     1280 2024-04-09 13:39:59.764713 fastramqpi-7.1.0/fastramqpi/ra_utils/sentry_init.py
--rw-r--r--   0        0        0     1003 2024-04-09 13:39:59.764713 fastramqpi-7.1.0/fastramqpi/ra_utils/strategies.py
--rw-r--r--   0        0        0     3782 2024-04-09 13:39:59.764713 fastramqpi-7.1.0/fastramqpi/ra_utils/structured_url.py
--rw-r--r--   0        0        0     4717 2024-04-09 13:39:59.764713 fastramqpi-7.1.0/fastramqpi/ra_utils/syncable.py
--rw-r--r--   0        0        0      548 2024-04-09 13:39:59.765713 fastramqpi-7.1.0/fastramqpi/ra_utils/tqdm_wrapper.py
--rw-r--r--   0        0        0     1834 2024-04-09 13:39:59.765713 fastramqpi-7.1.0/fastramqpi/ra_utils/transpose_dict.py
--rw-r--r--   0        0        0      300 2024-04-09 13:39:59.765713 fastramqpi-7.1.0/fastramqpi/raclients/__init__.py
--rw-r--r--   0        0        0     6858 2024-04-09 13:39:59.765713 fastramqpi-7.1.0/fastramqpi/raclients/auth.py
--rw-r--r--   0        0        0       99 2024-04-09 13:39:59.765713 fastramqpi-7.1.0/fastramqpi/raclients/graph/__init__.py
--rw-r--r--   0        0        0     7219 2024-04-09 13:39:59.766713 fastramqpi-7.1.0/fastramqpi/raclients/graph/client.py
--rw-r--r--   0        0        0     9303 2024-04-09 13:39:59.766713 fastramqpi-7.1.0/fastramqpi/raclients/graph/transport.py
--rw-r--r--   0        0        0     3482 2024-04-09 13:39:59.766713 fastramqpi-7.1.0/fastramqpi/raclients/graph/util.py
--rw-r--r--   0        0        0       99 2024-04-09 13:39:59.767713 fastramqpi-7.1.0/fastramqpi/raclients/modelclient/__init__.py
--rw-r--r--   0        0        0     4390 2024-04-09 13:39:59.767713 fastramqpi-7.1.0/fastramqpi/raclients/modelclient/base.py
--rw-r--r--   0        0        0     1919 2024-04-09 13:39:59.767713 fastramqpi-7.1.0/fastramqpi/raclients/modelclient/lora.py
--rw-r--r--   0        0        0     5296 2024-04-09 13:39:59.767713 fastramqpi-7.1.0/fastramqpi/raclients/modelclient/mo.py
--rw-r--r--   0        0        0     3459 2024-04-09 13:39:59.767713 fastramqpi-7.1.0/fastramqpi/raclients/upload.py
--rw-r--r--   0        0        0      321 2024-04-09 13:39:59.768713 fastramqpi-7.1.0/fastramqpi/ramqp/__init__.py
--rw-r--r--   0        0        0    18731 2024-04-09 13:39:59.768713 fastramqpi-7.1.0/fastramqpi/ramqp/abstract.py
--rw-r--r--   0        0        0      668 2024-04-09 13:39:59.768713 fastramqpi-7.1.0/fastramqpi/ramqp/amqp.py
--rw-r--r--   0        0        0     2858 2024-04-09 13:39:59.768713 fastramqpi-7.1.0/fastramqpi/ramqp/config.py
--rw-r--r--   0        0        0    11402 2024-04-09 13:39:59.769713 fastramqpi-7.1.0/fastramqpi/ramqp/depends.py
--rw-r--r--   0        0        0     7130 2024-04-09 13:39:59.769713 fastramqpi-7.1.0/fastramqpi/ramqp/metrics.py
--rw-r--r--   0        0        0     8642 2024-04-09 13:39:59.769713 fastramqpi-7.1.0/fastramqpi/ramqp/mo.py
--rw-r--r--   0        0        0     1941 2024-04-09 13:39:59.769713 fastramqpi-7.1.0/fastramqpi/ramqp/utils.py
--rw-r--r--   0        0        0     2173 2024-04-09 13:40:02.379889 fastramqpi-7.1.0/pyproject.toml
--rw-r--r--   0        0        0    15537 1970-01-01 00:00:00.000000 fastramqpi-7.1.0/PKG-INFO
+drwxr-xr-x   0        0        0        0 2024-04-17 17:21:04.415982 fastramqpi-7.2.0/LICENSES/
+-rw-r--r--   0        0        0    15177 2024-04-17 17:21:04.415982 fastramqpi-7.2.0/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0    14146 2024-04-17 17:21:04.415982 fastramqpi-7.2.0/README.md
+-rw-r--r--   0        0        0       85 2024-04-17 17:21:04.421983 fastramqpi-7.2.0/fastramqpi/__init__.py
+-rw-r--r--   0        0        0     7425 2024-04-17 17:21:04.421983 fastramqpi-7.2.0/fastramqpi/app.py
+-rw-r--r--   0        0        0     2207 2024-04-17 17:21:04.422983 fastramqpi-7.2.0/fastramqpi/config.py
+-rw-r--r--   0        0        0     1620 2024-04-17 17:21:04.422983 fastramqpi-7.2.0/fastramqpi/context.py
+-rw-r--r--   0        0        0     1498 2024-04-17 17:21:04.422983 fastramqpi-7.2.0/fastramqpi/depends.py
+-rw-r--r--   0        0        0     6738 2024-04-17 17:21:04.422983 fastramqpi-7.2.0/fastramqpi/main.py
+-rw-r--r--   0        0        0      477 2024-04-17 17:21:04.422983 fastramqpi-7.2.0/fastramqpi/metrics.py
+-rw-r--r--   0        0        0        0 2024-04-17 17:21:04.498988 fastramqpi-7.2.0/fastramqpi/py.typed
+-rw-r--r--   0        0        0     5174 2024-04-17 17:21:04.422983 fastramqpi-7.2.0/fastramqpi/pytest_plugin.py
+-rw-r--r--   0        0        0      884 2024-04-17 17:21:04.422983 fastramqpi-7.2.0/fastramqpi/pytest_util.py
+-rw-r--r--   0        0        0       99 2024-04-17 17:21:04.422983 fastramqpi-7.2.0/fastramqpi/ra_utils/__init__.py
+-rw-r--r--   0        0        0     2263 2024-04-17 17:21:04.423983 fastramqpi-7.2.0/fastramqpi/ra_utils/apply.py
+-rw-r--r--   0        0        0     1051 2024-04-17 17:21:04.423983 fastramqpi-7.2.0/fastramqpi/ra_utils/async_to_sync.py
+-rw-r--r--   0        0        0     2496 2024-04-17 17:21:04.423983 fastramqpi-7.2.0/fastramqpi/ra_utils/asyncio_utils.py
+-rw-r--r--   0        0        0      805 2024-04-17 17:21:04.423983 fastramqpi-7.2.0/fastramqpi/ra_utils/attrdict.py
+-rw-r--r--   0        0        0     1539 2024-04-17 17:21:04.423983 fastramqpi-7.2.0/fastramqpi/ra_utils/catchtime.py
+-rw-r--r--   0        0        0      979 2024-04-17 17:21:04.423983 fastramqpi-7.2.0/fastramqpi/ra_utils/deprecation.py
+-rw-r--r--   0        0        0     3961 2024-04-17 17:21:04.423983 fastramqpi-7.2.0/fastramqpi/ra_utils/dict_map.py
+-rw-r--r--   0        0        0     2184 2024-04-17 17:21:04.423983 fastramqpi-7.2.0/fastramqpi/ra_utils/ensure_hashable.py
+-rw-r--r--   0        0        0     3808 2024-04-17 17:21:04.423983 fastramqpi-7.2.0/fastramqpi/ra_utils/ensure_single_run.py
+-rw-r--r--   0        0        0     1723 2024-04-17 17:21:04.423983 fastramqpi-7.2.0/fastramqpi/ra_utils/generate_uuid.py
+-rw-r--r--   0        0        0     5633 2024-04-17 17:21:04.424983 fastramqpi-7.2.0/fastramqpi/ra_utils/headers.py
+-rw-r--r--   0        0        0     3245 2024-04-17 17:21:04.424983 fastramqpi-7.2.0/fastramqpi/ra_utils/jinja_filter.py
+-rw-r--r--   0        0        0     7347 2024-04-17 17:21:04.424983 fastramqpi-7.2.0/fastramqpi/ra_utils/job_settings.py
+-rw-r--r--   0        0        0     6027 2024-04-17 17:21:04.424983 fastramqpi-7.2.0/fastramqpi/ra_utils/lazy_dict.py
+-rw-r--r--   0        0        0     2929 2024-04-17 17:21:04.424983 fastramqpi-7.2.0/fastramqpi/ra_utils/load_settings.py
+-rw-r--r--   0        0        0     2935 2024-04-17 17:21:04.424983 fastramqpi-7.2.0/fastramqpi/ra_utils/multiple_replace.py
+-rw-r--r--   0        0        0     2891 2024-04-17 17:21:04.424983 fastramqpi-7.2.0/fastramqpi/ra_utils/semantic_version_type.py
+-rw-r--r--   0        0        0     1280 2024-04-17 17:21:04.424983 fastramqpi-7.2.0/fastramqpi/ra_utils/sentry_init.py
+-rw-r--r--   0        0        0     1003 2024-04-17 17:21:04.425983 fastramqpi-7.2.0/fastramqpi/ra_utils/strategies.py
+-rw-r--r--   0        0        0     3782 2024-04-17 17:21:04.425983 fastramqpi-7.2.0/fastramqpi/ra_utils/structured_url.py
+-rw-r--r--   0        0        0     4717 2024-04-17 17:21:04.425983 fastramqpi-7.2.0/fastramqpi/ra_utils/syncable.py
+-rw-r--r--   0        0        0      548 2024-04-17 17:21:04.425983 fastramqpi-7.2.0/fastramqpi/ra_utils/tqdm_wrapper.py
+-rw-r--r--   0        0        0     1834 2024-04-17 17:21:04.425983 fastramqpi-7.2.0/fastramqpi/ra_utils/transpose_dict.py
+-rw-r--r--   0        0        0      300 2024-04-17 17:21:04.425983 fastramqpi-7.2.0/fastramqpi/raclients/__init__.py
+-rw-r--r--   0        0        0     6858 2024-04-17 17:21:04.425983 fastramqpi-7.2.0/fastramqpi/raclients/auth.py
+-rw-r--r--   0        0        0       99 2024-04-17 17:21:04.425983 fastramqpi-7.2.0/fastramqpi/raclients/graph/__init__.py
+-rw-r--r--   0        0        0     7219 2024-04-17 17:21:04.426983 fastramqpi-7.2.0/fastramqpi/raclients/graph/client.py
+-rw-r--r--   0        0        0     9303 2024-04-17 17:21:04.426983 fastramqpi-7.2.0/fastramqpi/raclients/graph/transport.py
+-rw-r--r--   0        0        0     3482 2024-04-17 17:21:04.426983 fastramqpi-7.2.0/fastramqpi/raclients/graph/util.py
+-rw-r--r--   0        0        0       99 2024-04-17 17:21:04.426983 fastramqpi-7.2.0/fastramqpi/raclients/modelclient/__init__.py
+-rw-r--r--   0        0        0     4390 2024-04-17 17:21:04.426983 fastramqpi-7.2.0/fastramqpi/raclients/modelclient/base.py
+-rw-r--r--   0        0        0     1919 2024-04-17 17:21:04.426983 fastramqpi-7.2.0/fastramqpi/raclients/modelclient/lora.py
+-rw-r--r--   0        0        0     5296 2024-04-17 17:21:04.426983 fastramqpi-7.2.0/fastramqpi/raclients/modelclient/mo.py
+-rw-r--r--   0        0        0     3459 2024-04-17 17:21:04.427983 fastramqpi-7.2.0/fastramqpi/raclients/upload.py
+-rw-r--r--   0        0        0      321 2024-04-17 17:21:04.427983 fastramqpi-7.2.0/fastramqpi/ramqp/__init__.py
+-rw-r--r--   0        0        0    18731 2024-04-17 17:21:04.427983 fastramqpi-7.2.0/fastramqpi/ramqp/abstract.py
+-rw-r--r--   0        0        0      668 2024-04-17 17:21:04.427983 fastramqpi-7.2.0/fastramqpi/ramqp/amqp.py
+-rw-r--r--   0        0        0     2858 2024-04-17 17:21:04.427983 fastramqpi-7.2.0/fastramqpi/ramqp/config.py
+-rw-r--r--   0        0        0    11402 2024-04-17 17:21:04.427983 fastramqpi-7.2.0/fastramqpi/ramqp/depends.py
+-rw-r--r--   0        0        0     7130 2024-04-17 17:21:04.427983 fastramqpi-7.2.0/fastramqpi/ramqp/metrics.py
+-rw-r--r--   0        0        0     8642 2024-04-17 17:21:04.428983 fastramqpi-7.2.0/fastramqpi/ramqp/mo.py
+-rw-r--r--   0        0        0     1941 2024-04-17 17:21:04.428983 fastramqpi-7.2.0/fastramqpi/ramqp/utils.py
+-rw-r--r--   0        0        0     2173 2024-04-17 17:21:06.519128 fastramqpi-7.2.0/pyproject.toml
+-rw-r--r--   0        0        0    15537 1970-01-01 00:00:00.000000 fastramqpi-7.2.0/PKG-INFO
```

### Comparing `fastramqpi-7.1.0/LICENSES/MPL-2.0.txt` & `fastramqpi-7.2.0/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/README.md` & `fastramqpi-7.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/app.py` & `fastramqpi-7.2.0/fastramqpi/app.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/config.py` & `fastramqpi-7.2.0/fastramqpi/config.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/context.py` & `fastramqpi-7.2.0/fastramqpi/context.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/depends.py` & `fastramqpi-7.2.0/fastramqpi/depends.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/main.py` & `fastramqpi-7.2.0/fastramqpi/main.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/pytest_util.py` & `fastramqpi-7.2.0/fastramqpi/pytest_util.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ra_utils/apply.py` & `fastramqpi-7.2.0/fastramqpi/ra_utils/apply.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ra_utils/async_to_sync.py` & `fastramqpi-7.2.0/fastramqpi/ra_utils/async_to_sync.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ra_utils/asyncio_utils.py` & `fastramqpi-7.2.0/fastramqpi/ra_utils/asyncio_utils.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ra_utils/attrdict.py` & `fastramqpi-7.2.0/fastramqpi/ra_utils/attrdict.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ra_utils/catchtime.py` & `fastramqpi-7.2.0/fastramqpi/ra_utils/catchtime.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ra_utils/deprecation.py` & `fastramqpi-7.2.0/fastramqpi/ra_utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ra_utils/dict_map.py` & `fastramqpi-7.2.0/fastramqpi/ra_utils/dict_map.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ra_utils/ensure_hashable.py` & `fastramqpi-7.2.0/fastramqpi/ra_utils/ensure_hashable.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ra_utils/ensure_single_run.py` & `fastramqpi-7.2.0/fastramqpi/ra_utils/ensure_single_run.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ra_utils/generate_uuid.py` & `fastramqpi-7.2.0/fastramqpi/ra_utils/generate_uuid.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ra_utils/headers.py` & `fastramqpi-7.2.0/fastramqpi/ra_utils/headers.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ra_utils/jinja_filter.py` & `fastramqpi-7.2.0/fastramqpi/ra_utils/jinja_filter.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ra_utils/job_settings.py` & `fastramqpi-7.2.0/fastramqpi/ra_utils/job_settings.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ra_utils/lazy_dict.py` & `fastramqpi-7.2.0/fastramqpi/ra_utils/lazy_dict.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ra_utils/load_settings.py` & `fastramqpi-7.2.0/fastramqpi/ra_utils/load_settings.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ra_utils/multiple_replace.py` & `fastramqpi-7.2.0/fastramqpi/ra_utils/multiple_replace.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ra_utils/semantic_version_type.py` & `fastramqpi-7.2.0/fastramqpi/ra_utils/semantic_version_type.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ra_utils/sentry_init.py` & `fastramqpi-7.2.0/fastramqpi/ra_utils/sentry_init.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ra_utils/strategies.py` & `fastramqpi-7.2.0/fastramqpi/ra_utils/strategies.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ra_utils/structured_url.py` & `fastramqpi-7.2.0/fastramqpi/ra_utils/structured_url.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ra_utils/syncable.py` & `fastramqpi-7.2.0/fastramqpi/ra_utils/syncable.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ra_utils/tqdm_wrapper.py` & `fastramqpi-7.2.0/fastramqpi/ra_utils/tqdm_wrapper.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ra_utils/transpose_dict.py` & `fastramqpi-7.2.0/fastramqpi/ra_utils/transpose_dict.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/raclients/auth.py` & `fastramqpi-7.2.0/fastramqpi/raclients/auth.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/raclients/graph/client.py` & `fastramqpi-7.2.0/fastramqpi/raclients/graph/client.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/raclients/graph/transport.py` & `fastramqpi-7.2.0/fastramqpi/raclients/graph/transport.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/raclients/graph/util.py` & `fastramqpi-7.2.0/fastramqpi/raclients/graph/util.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/raclients/modelclient/base.py` & `fastramqpi-7.2.0/fastramqpi/raclients/modelclient/base.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/raclients/modelclient/lora.py` & `fastramqpi-7.2.0/fastramqpi/raclients/modelclient/lora.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/raclients/modelclient/mo.py` & `fastramqpi-7.2.0/fastramqpi/raclients/modelclient/mo.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/raclients/upload.py` & `fastramqpi-7.2.0/fastramqpi/raclients/upload.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ramqp/abstract.py` & `fastramqpi-7.2.0/fastramqpi/ramqp/abstract.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ramqp/amqp.py` & `fastramqpi-7.2.0/fastramqpi/ramqp/amqp.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ramqp/config.py` & `fastramqpi-7.2.0/fastramqpi/ramqp/config.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ramqp/depends.py` & `fastramqpi-7.2.0/fastramqpi/ramqp/depends.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ramqp/metrics.py` & `fastramqpi-7.2.0/fastramqpi/ramqp/metrics.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ramqp/mo.py` & `fastramqpi-7.2.0/fastramqpi/ramqp/mo.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/fastramqpi/ramqp/utils.py` & `fastramqpi-7.2.0/fastramqpi/ramqp/utils.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.1.0/pyproject.toml` & `fastramqpi-7.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-FileCopyrightText: 2019-2020 Magenta ApS
 # SPDX-License-Identifier: MPL-2.0
 [tool.poetry]
 name = "FastRAMQPI"
-version = "7.1.0"
+version = "7.2.0"
 description = "Rammearkitektur integrations framework"
 authors = ["Magenta ApS <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/FastRAMQPI"
 keywords = ["os2mo"]
```

### Comparing `fastramqpi-7.1.0/PKG-INFO` & `fastramqpi-7.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FastRAMQPI
-Version: 7.1.0
+Version: 7.2.0
 Summary: Rammearkitektur integrations framework
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: os2mo
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.11,<4.0
```

