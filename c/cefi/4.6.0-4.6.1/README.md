# Comparing `tmp/cefi-4.6.0.tar.gz` & `tmp/cefi-4.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cefi-4.6.0.tar", max compression
+gzip compressed data, was "cefi-4.6.1.tar", max compression
```

## Comparing `cefi-4.6.0.tar` & `cefi-4.6.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1064 2024-04-16 17:12:56.757665 cefi-4.6.0/LICENSE
--rw-r--r--   0        0        0     2661 2024-04-16 17:12:56.757665 cefi-4.6.0/README.md
--rw-r--r--   0        0        0       87 2024-04-16 17:13:31.985818 cefi-4.6.0/cefi/__init__.py
--rw-r--r--   0        0        0      439 2024-04-16 17:12:56.757665 cefi-4.6.0/cefi/config.py
--rw-r--r--   0        0        0     3617 2024-04-16 17:12:56.757665 cefi-4.6.0/cefi/default_settings.toml
--rw-r--r--   0        0        0      158 2024-04-16 17:12:56.757665 cefi-4.6.0/cefi/handler/__init__.py
--rw-r--r--   0        0        0    10949 2024-04-16 17:12:56.757665 cefi-4.6.0/cefi/handler/capitalcom.py
--rw-r--r--   0        0        0     5517 2024-04-16 17:12:56.757665 cefi-4.6.0/cefi/handler/ccxt.py
--rw-r--r--   0        0        0     9015 2024-04-16 17:12:56.757665 cefi-4.6.0/cefi/handler/client.py
--rw-r--r--   0        0        0     1938 2024-04-16 17:12:56.761665 cefi-4.6.0/cefi/handler/ctrader.py
--rw-r--r--   0        0        0     7006 2024-04-16 17:12:56.761665 cefi-4.6.0/cefi/handler/ib_sync.py
--rw-r--r--   0        0        0     8160 2024-04-16 17:12:56.761665 cefi-4.6.0/cefi/main.py
--rw-r--r--   0        0        0     3760 2024-04-16 17:13:31.985818 cefi-4.6.0/pyproject.toml
--rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 cefi-4.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-16 19:55:41.286257 cefi-4.6.1/LICENSE
+-rw-r--r--   0        0        0     2661 2024-04-16 19:55:41.286257 cefi-4.6.1/README.md
+-rw-r--r--   0        0        0       87 2024-04-16 19:56:17.378278 cefi-4.6.1/cefi/__init__.py
+-rw-r--r--   0        0        0      439 2024-04-16 19:55:41.286257 cefi-4.6.1/cefi/config.py
+-rw-r--r--   0        0        0     3617 2024-04-16 19:55:41.286257 cefi-4.6.1/cefi/default_settings.toml
+-rw-r--r--   0        0        0      158 2024-04-16 19:55:41.286257 cefi-4.6.1/cefi/handler/__init__.py
+-rw-r--r--   0        0        0    11042 2024-04-16 19:55:41.286257 cefi-4.6.1/cefi/handler/capitalcom.py
+-rw-r--r--   0        0        0     5517 2024-04-16 19:55:41.286257 cefi-4.6.1/cefi/handler/ccxt.py
+-rw-r--r--   0        0        0     9015 2024-04-16 19:55:41.286257 cefi-4.6.1/cefi/handler/client.py
+-rw-r--r--   0        0        0     1938 2024-04-16 19:55:41.286257 cefi-4.6.1/cefi/handler/ctrader.py
+-rw-r--r--   0        0        0     7006 2024-04-16 19:55:41.286257 cefi-4.6.1/cefi/handler/ib_sync.py
+-rw-r--r--   0        0        0     8160 2024-04-16 19:55:41.286257 cefi-4.6.1/cefi/main.py
+-rw-r--r--   0        0        0     3762 2024-04-16 19:56:17.378278 cefi-4.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 cefi-4.6.1/PKG-INFO
```

### Comparing `cefi-4.6.0/LICENSE` & `cefi-4.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cefi-4.6.0/README.md` & `cefi-4.6.1/README.md`

 * *Files identical despite different names*

### Comparing `cefi-4.6.0/cefi/default_settings.toml` & `cefi-4.6.1/cefi/default_settings.toml`

 * *Files identical despite different names*

### Comparing `cefi-4.6.0/cefi/handler/capitalcom.py` & `cefi-4.6.1/cefi/handler/capitalcom.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,15 +244,17 @@
         decimals = instrument_info.get("snapshot", {}).get("decimalPlacesFactor", 0)
         logger.debug("Decimals {}", decimals)
         return int(decimals)
 
     async def get_instrument_min_amount(self, instrument):
         """ """
         instrument_info = self.client.single_market(instrument)
-        minimum_amount = instrument_info.get("minDealSize", {}).get("value", 0)
+        logger.debug("instrument_info {}", instrument_info)
+        minimum_amount = instrument_info.get("dealingRules", {}).get(
+        "minDealSize", {}).get("value", 0)
         logger.debug("Minimum {}", minimum_amount)
         return int(minimum_amount)
 
     async def execute_order(self, order_params):
         """
         Execute order
```

### Comparing `cefi-4.6.0/cefi/handler/ccxt.py` & `cefi-4.6.1/cefi/handler/ccxt.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.0/cefi/handler/client.py` & `cefi-4.6.1/cefi/handler/client.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.0/cefi/handler/ctrader.py` & `cefi-4.6.1/cefi/handler/ctrader.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.0/cefi/handler/ib_sync.py` & `cefi-4.6.1/cefi/handler/ib_sync.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.0/cefi/main.py` & `cefi-4.6.1/cefi/main.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.0/pyproject.toml` & `cefi-4.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "cefi"
-version = "4.6.0"
+version = "4.6.1"
 description = "A python library, to interact  with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)"
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["cex, cefi, crypto, exchange, broker"]
 packages = [
     {include = "cefi"}
@@ -159,27 +159,29 @@
 
 
 
 
 
 
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.23.0"
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.4.0"
 
 
 
 
 
 
 
+
```

### Comparing `cefi-4.6.0/PKG-INFO` & `cefi-4.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cefi
-Version: 4.6.0
+Version: 4.6.1
 Summary: A python library, to interact  with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)
 License: MIT
 Keywords: cex, cefi, crypto, exchange, broker
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cefi Version: 4.6.0 Summary: A python library, to
+Metadata-Version: 2.1 Name: cefi Version: 4.6.1 Summary: A python library, to
 interact with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)
 License: MIT Keywords: cex, cefi, crypto, exchange, broker Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: capitalcom-python
```

