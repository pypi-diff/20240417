# Comparing `tmp/giza_datasets-0.2.0.tar.gz` & `tmp/giza_datasets-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giza_datasets-0.2.0.tar", max compression
+gzip compressed data, was "giza_datasets-0.2.1.tar", max compression
```

## Comparing `giza_datasets-0.2.0.tar` & `giza_datasets-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2024-03-21 14:36:23.904180 giza_datasets-0.2.0/LICENSE
--rw-r--r--   0        0        0     3951 2024-03-21 14:36:23.904180 giza_datasets-0.2.0/README.md
--rw-r--r--   0        0        0      136 2024-03-21 14:36:23.904180 giza_datasets-0.2.0/giza_datasets/__init__.py
--rw-r--r--   0        0        0     2853 2024-03-21 14:36:23.904180 giza_datasets-0.2.0/giza_datasets/cache_manager.py
--rw-r--r--   0        0        0   148886 2024-03-21 14:36:23.904180 giza_datasets-0.2.0/giza_datasets/constants.py
--rw-r--r--   0        0        0      635 2024-03-21 14:36:23.904180 giza_datasets-0.2.0/giza_datasets/defillama_constants.py
--rw-r--r--   0        0        0     3240 2024-03-21 14:36:23.904180 giza_datasets-0.2.0/giza_datasets/hub.py
--rw-r--r--   0        0        0     5982 2024-03-21 14:36:23.904180 giza_datasets-0.2.0/giza_datasets/loaders.py
--rw-r--r--   0        0        0     1399 2024-03-21 14:36:23.904180 giza_datasets-0.2.0/giza_datasets/models.py
--rw-r--r--   0        0        0      554 2024-03-21 14:36:23.904180 giza_datasets-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4537 1970-01-01 00:00:00.000000 giza_datasets-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-17 13:07:02.194124 giza_datasets-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3951 2024-04-17 13:07:02.194124 giza_datasets-0.2.1/README.md
+-rw-r--r--   0        0        0      136 2024-04-17 13:07:02.194124 giza_datasets-0.2.1/giza_datasets/__init__.py
+-rw-r--r--   0        0        0     2853 2024-04-17 13:07:02.194124 giza_datasets-0.2.1/giza_datasets/cache_manager.py
+-rw-r--r--   0        0        0   150859 2024-04-17 13:07:02.198124 giza_datasets-0.2.1/giza_datasets/constants.py
+-rw-r--r--   0        0        0      635 2024-04-17 13:07:02.198124 giza_datasets-0.2.1/giza_datasets/defillama_constants.py
+-rw-r--r--   0        0        0     3240 2024-04-17 13:07:02.198124 giza_datasets-0.2.1/giza_datasets/hub.py
+-rw-r--r--   0        0        0     5982 2024-04-17 13:07:02.198124 giza_datasets-0.2.1/giza_datasets/loaders.py
+-rw-r--r--   0        0        0     1441 2024-04-17 13:07:02.198124 giza_datasets-0.2.1/giza_datasets/models.py
+-rw-r--r--   0        0        0      554 2024-04-17 13:07:02.198124 giza_datasets-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4537 1970-01-01 00:00:00.000000 giza_datasets-0.2.1/PKG-INFO
```

### Comparing `giza_datasets-0.2.0/LICENSE` & `giza_datasets-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `giza_datasets-0.2.0/README.md` & `giza_datasets-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `giza_datasets-0.2.0/giza_datasets/cache_manager.py` & `giza_datasets-0.2.1/giza_datasets/cache_manager.py`

 * *Files identical despite different names*

### Comparing `giza_datasets-0.2.0/giza_datasets/constants.py` & `giza_datasets-0.2.1/giza_datasets/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -2223,26 +2223,68 @@
         description="Snapshots of Uniswap V3 liquidity distribution in 1000 blocks intervals for UNI-WBTC pool with 0.3 % fee",
         tags=["Uniswap-v3", "Liquidity", "Ethereum", "DeFi", "DEX"],
         documentation="https://datasets.gizatech.xyz/hub-pending/uniswap-v3-liquidity-distribution",
     ),
     Dataset(
         name="farcaster-casts",
         path="gs://datasets-giza/Farcaster/Farcaster_Casts.parquet",
-        description="Individual farcaster casts, between 2023-01 to 2023-03",
+        description="Individual farcaster casts, between 2024-01 to 2024-03",
         tags=["Farcaster", "Social"],
         documentation="https://datasets.gizatech.xyz/hub/farcaster/individual-casts",
     ),
     Dataset(
         name="farcaster-links",
         path="gs://datasets-giza/Farcaster/Farcaster_Links.parquet",
-        description="Individual farcaster links, between 2023-01 to 2023-02",
+        description="Individual farcaster links, between 2024-01 to 2024-02",
         tags=["Farcaster", "Social"],
         documentation="https://datasets.gizatech.xyz/hub/farcaster/individual-links",
     ),
     Dataset(
         name="farcaster-reactions",
         path="gs://datasets-giza/Farcaster/Farcaster_Reactions.parquet",
-        description="Individual farcaster reactionss, between 2023-01-01 to 2023-01-04",
+        description="Individual farcaster reactionss, between 2024-01-01 to 2024-01-04",
         tags=["Farcaster", "Social"],
         documentation="https://datasets.gizatech.xyz/hub/farcaster/individual-reactions",
     ),
+    Dataset(
+        name="lens-posts",
+        path="gs://datasets-giza/Lens/Lens_Posts.parquet",
+        description="Individual lens posts, between 2024-01-01 to 2024-04-04",
+        tags=["Lens", "Social"],
+        documentation="https://datasets.gizatech.xyz/hub/lens/individual-posts",
+    ),
+    Dataset(
+        name="lens-mirrors",
+        path="gs://datasets-giza/Lens/Lens_Mirrors.parquet",
+        description="Individual lens mirrors, between 2024-01-01 to 2024-04-04",
+        tags=["Lens", "Social"],
+        documentation="https://datasets.gizatech.xyz/hub/lens/individual-mirrors",
+    ),
+    Dataset(
+        name="lens-comments",
+        path="gs://datasets-giza/Lens/Lens_Comments.parquet",
+        description="Individual lens comments, between 2024-01-01 to 2024-04-04",
+        tags=["Lens", "Social"],
+        documentation="https://datasets.gizatech.xyz/hub/lens/individual-comments",
+    ),
+    Dataset(
+        name="lens-quotes",
+        path="gs://datasets-giza/Lens/Lens_Quotes.parquet",
+        description="Individual lens quotes, between 2024-01-01 to 2024-04-04",
+        tags=["Lens", "Social"],
+        documentation="https://datasets.gizatech.xyz/hub/lens/individual-quotes",
+    ),
+    Dataset(
+        name="pancakeswap-daily-volume",
+        path="gs://datasets-giza/PancakeSwap/pancakeswap_daily_volume.parquet",
+        description="Daily PancakeSwap trade volume in USD, per pool ",
+        tags=["PancakeSwap", "Trade Volume", "daily", "DeFi", "DEX"],
+        documentation="https://datasets.gizatech.xyz/hub/pancakeswap/daily-trade-volume",
+    ),
+    Dataset(
+        name="curve-daily-volume-fees",
+        path="gs://datasets-giza/Curve/curve_daily_volume_fees.parquet",
+        description="Daily Curve trade volume and fees generated in USD, per pool",
+        tags=["Curve","Trade Volume","Fees" ,"daily", "DeFi", "DEX"],
+        documentation="https://datasets.gizatech.xyz/hub/curve/daily-trade-volume-and-fees",
+    ),
 ]
```

### Comparing `giza_datasets-0.2.0/giza_datasets/defillama_constants.py` & `giza_datasets-0.2.1/giza_datasets/defillama_constants.py`

 * *Files identical despite different names*

### Comparing `giza_datasets-0.2.0/giza_datasets/hub.py` & `giza_datasets-0.2.1/giza_datasets/hub.py`

 * *Files identical despite different names*

### Comparing `giza_datasets-0.2.0/giza_datasets/loaders.py` & `giza_datasets-0.2.1/giza_datasets/loaders.py`

 * *Files identical despite different names*

### Comparing `giza_datasets-0.2.0/giza_datasets/models.py` & `giza_datasets-0.2.1/giza_datasets/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from typing import List, Optional
 
 from pydantic import BaseModel
 
 from giza_datasets.defillama_constants import DEFILLAMA_SUPPORTED_PROJECTS
 
 sector_tags = ["DeFi","Social"]
-application_tags = ["Liquid Staking", "Dexes", "Yield", "Lending", "Yield Aggregator"]
+application_tags = ["Liquid Staking", "DEX", "Yield", "Lending", "Yield Aggregator"]
 protocol_tags = DEFILLAMA_SUPPORTED_PROJECTS + [
     "Aave-v2",
     "Aave-v3",
     "Compound-v2",
     "Balancer-v1",
     "Balancer-v2",
     "MorphoBlue",
     "Uniswap-v3",
     "Yearn-v2",
     "Farcaster",
+    "Lens",
+    "PancakeSwap",
+    "Curve",
 ]
 network_tags = [
     "Ethereum",
     "Arbitrum",
     "Optimism",
     "Avalanche",
     "Base",
```

### Comparing `giza_datasets-0.2.0/pyproject.toml` & `giza_datasets-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "giza-datasets"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["Fran Algaba <f.algaba@outlook.es>"]
 readme = "README.md"
 license = "MIT"
 include = ["datasets/*"]
```

### Comparing `giza_datasets-0.2.0/PKG-INFO` & `giza_datasets-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giza-datasets
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 License: MIT
 Author: Fran Algaba
 Author-email: f.algaba@outlook.es
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

