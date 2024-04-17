# Comparing `tmp/snet.contracts-0.0.9.tar.gz` & `tmp/snet_contracts-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snet.contracts-0.0.9.tar", last modified: Wed Apr  3 15:26:43 2024, max compression
+gzip compressed data, was "snet_contracts-0.1.0.tar", last modified: Wed Apr 17 09:46:39 2024, max compression
```

## Comparing `snet.contracts-0.0.9.tar` & `snet_contracts-0.1.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:26:43.683327 snet.contracts-0.0.9/
--rw-r--r--   0 root         (0) root         (0)     1071 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)      404 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2339 2024-04-03 15:26:43.683327 snet.contracts-0.0.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1975 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/README.md
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 15:26:43.683327 snet.contracts-0.0.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      911 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:26:43.679327 snet.contracts-0.0.9/snet/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:26:43.679327 snet.contracts-0.0.9/snet/contracts/
--rw-r--r--   0 root         (0) root         (0)       20 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:26:43.679327 snet.contracts-0.0.9/snet/contracts/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:26:43.683327 snet.contracts-0.0.9/snet/contracts/resources/abi/
--rw-r--r--   0 root         (0) root         (0)     8656 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/abi/MultiPartyEscrow.json
--rw-r--r--   0 root         (0) root         (0)     5433 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/abi/Registry.json
--rw-r--r--   0 root         (0) root         (0)     7461 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/abi/SingularityNetToken.json
--rw-r--r--   0 root         (0) root         (0)     4215 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/abi/TokenConversionManager.json
--rw-r--r--   0 root         (0) root         (0)     9861 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/abi/TokenStake.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:26:43.683327 snet.contracts-0.0.9/snet/contracts/resources/bytecode/
--rw-r--r--   0 root         (0) root         (0)    15025 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/bytecode/MultiPartyEscrow.json
--rw-r--r--   0 root         (0) root         (0)    14575 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/bytecode/Registry.json
--rw-r--r--   0 root         (0) root         (0)    15169 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/bytecode/SingularityNetToken.json
--rw-r--r--   0 root         (0) root         (0)     8967 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/bytecode/TokenConversionManager.json
--rw-r--r--   0 root         (0) root         (0)    22353 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/bytecode/TokenStake.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:26:43.683327 snet.contracts-0.0.9/snet/contracts/resources/networks/
--rw-r--r--   0 root         (0) root         (0)    26292 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/networks/MultiPartyEscrow.json
--rw-r--r--   0 root         (0) root         (0)    21210 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/networks/Registry.json
--rw-r--r--   0 root         (0) root         (0)    17268 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/networks/SingularityNetToken.json
--rw-r--r--   0 root         (0) root         (0)    30657 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/networks/TokenStake.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:26:43.679327 snet.contracts-0.0.9/snet/contracts/resources/networks/converter/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:26:43.683327 snet.contracts-0.0.9/snet/contracts/resources/networks/converter/AGIX/
--rw-r--r--   0 root         (0) root         (0)    14351 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/networks/converter/AGIX/TokenConversionManager.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:26:43.683327 snet.contracts-0.0.9/snet/contracts/resources/networks/converter/CGV/
--rw-r--r--   0 root         (0) root         (0)    15979 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/networks/converter/CGV/TokenConversionManager.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:26:43.683327 snet.contracts-0.0.9/snet/contracts/resources/networks/converter/NTX/
--rw-r--r--   0 root         (0) root         (0)    15979 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/networks/converter/NTX/TokenConversionManager.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:26:43.683327 snet.contracts-0.0.9/snet/contracts/resources/networks/converter/RJV/
--rw-r--r--   0 root         (0) root         (0)    15979 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/resources/networks/converter/RJV/TokenConversionManager.json
--rw-r--r--   0 root         (0) root         (0)     1525 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/snet/contracts/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 15:26:43.683327 snet.contracts-0.0.9/snet.contracts.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2339 2024-04-03 15:26:43.000000 snet.contracts-0.0.9/snet.contracts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1396 2024-04-03 15:26:43.000000 snet.contracts-0.0.9/snet.contracts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 15:26:43.000000 snet.contracts-0.0.9/snet.contracts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-03 15:26:43.000000 snet.contracts-0.0.9/snet.contracts.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-03 15:26:43.000000 snet.contracts-0.0.9/snet.contracts.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-03 15:26:43.000000 snet.contracts-0.0.9/snet.contracts.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-03 15:26:37.000000 snet.contracts-0.0.9/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:46:39.266853 snet_contracts-0.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-17 09:46:33.000000 snet_contracts-0.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      404 2024-04-17 09:46:33.000000 snet_contracts-0.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2339 2024-04-17 09:46:39.266853 snet_contracts-0.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1975 2024-04-17 09:46:33.000000 snet_contracts-0.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-17 09:46:33.000000 snet_contracts-0.1.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 09:46:39.266853 snet_contracts-0.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      942 2024-04-17 09:46:33.000000 snet_contracts-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:46:39.262853 snet_contracts-0.1.0/snet/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:46:39.262853 snet_contracts-0.1.0/snet/contracts/
+-rw-r--r--   0 root         (0) root         (0)      122 2024-04-17 09:46:33.000000 snet_contracts-0.1.0/snet/contracts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:46:39.262853 snet_contracts-0.1.0/snet/contracts/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:46:39.262853 snet_contracts-0.1.0/snet/contracts/resources/abi/
+-rw-r--r--   0 root         (0) root         (0)     8656 2024-04-17 09:46:33.000000 snet_contracts-0.1.0/snet/contracts/resources/abi/MultiPartyEscrow.json
+-rw-r--r--   0 root         (0) root         (0)     5433 2024-04-17 09:46:33.000000 snet_contracts-0.1.0/snet/contracts/resources/abi/Registry.json
+-rw-r--r--   0 root         (0) root         (0)     7461 2024-04-17 09:46:33.000000 snet_contracts-0.1.0/snet/contracts/resources/abi/SingularityNetToken.json
+-rw-r--r--   0 root         (0) root         (0)     4215 2024-04-17 09:46:33.000000 snet_contracts-0.1.0/snet/contracts/resources/abi/TokenConversionManager.json
+-rw-r--r--   0 root         (0) root         (0)     9861 2024-04-17 09:46:33.000000 snet_contracts-0.1.0/snet/contracts/resources/abi/TokenStake.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:46:39.262853 snet_contracts-0.1.0/snet/contracts/resources/bytecode/
+-rw-r--r--   0 root         (0) root         (0)    15025 2024-04-17 09:46:33.000000 snet_contracts-0.1.0/snet/contracts/resources/bytecode/MultiPartyEscrow.json
+-rw-r--r--   0 root         (0) root         (0)    14575 2024-04-17 09:46:33.000000 snet_contracts-0.1.0/snet/contracts/resources/bytecode/Registry.json
+-rw-r--r--   0 root         (0) root         (0)    15169 2024-04-17 09:46:33.000000 snet_contracts-0.1.0/snet/contracts/resources/bytecode/SingularityNetToken.json
+-rw-r--r--   0 root         (0) root         (0)     8967 2024-04-17 09:46:33.000000 snet_contracts-0.1.0/snet/contracts/resources/bytecode/TokenConversionManager.json
+-rw-r--r--   0 root         (0) root         (0)    22353 2024-04-17 09:46:33.000000 snet_contracts-0.1.0/snet/contracts/resources/bytecode/TokenStake.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:46:39.262853 snet_contracts-0.1.0/snet/contracts/resources/networks/
+-rw-r--r--   0 root         (0) root         (0)    26292 2024-04-17 09:46:33.000000 snet_contracts-0.1.0/snet/contracts/resources/networks/MultiPartyEscrow.json
+-rw-r--r--   0 root         (0) root         (0)    21210 2024-04-17 09:46:33.000000 snet_contracts-0.1.0/snet/contracts/resources/networks/Registry.json
+-rw-r--r--   0 root         (0) root         (0)    17268 2024-04-17 09:46:33.000000 snet_contracts-0.1.0/snet/contracts/resources/networks/SingularityNetToken.json
+-rw-r--r--   0 root         (0) root         (0)    30657 2024-04-17 09:46:33.000000 snet_contracts-0.1.0/snet/contracts/resources/networks/TokenStake.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:46:39.262853 snet_contracts-0.1.0/snet/contracts/resources/networks/converter/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:46:39.262853 snet_contracts-0.1.0/snet/contracts/resources/networks/converter/AGIX/
+-rw-r--r--   0 root         (0) root         (0)    14351 2024-04-17 09:46:33.000000 snet_contracts-0.1.0/snet/contracts/resources/networks/converter/AGIX/TokenConversionManager.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:46:39.262853 snet_contracts-0.1.0/snet/contracts/resources/networks/converter/CGV/
+-rw-r--r--   0 root         (0) root         (0)    15979 2024-04-17 09:46:33.000000 snet_contracts-0.1.0/snet/contracts/resources/networks/converter/CGV/TokenConversionManager.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:46:39.262853 snet_contracts-0.1.0/snet/contracts/resources/networks/converter/NTX/
+-rw-r--r--   0 root         (0) root         (0)    15979 2024-04-17 09:46:33.000000 snet_contracts-0.1.0/snet/contracts/resources/networks/converter/NTX/TokenConversionManager.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:46:39.262853 snet_contracts-0.1.0/snet/contracts/resources/networks/converter/RJV/
+-rw-r--r--   0 root         (0) root         (0)    15979 2024-04-17 09:46:33.000000 snet_contracts-0.1.0/snet/contracts/resources/networks/converter/RJV/TokenConversionManager.json
+-rw-r--r--   0 root         (0) root         (0)     2427 2024-04-17 09:46:33.000000 snet_contracts-0.1.0/snet/contracts/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:46:39.266853 snet_contracts-0.1.0/snet.contracts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2339 2024-04-17 09:46:39.000000 snet_contracts-0.1.0/snet.contracts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1396 2024-04-17 09:46:39.000000 snet_contracts-0.1.0/snet.contracts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 09:46:39.000000 snet_contracts-0.1.0/snet.contracts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-17 09:46:39.000000 snet_contracts-0.1.0/snet.contracts.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-17 09:46:39.000000 snet_contracts-0.1.0/snet.contracts.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-17 09:46:39.000000 snet_contracts-0.1.0/snet.contracts.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-17 09:46:33.000000 snet_contracts-0.1.0/version.py
```

### Comparing `snet.contracts-0.0.9/LICENSE` & `snet_contracts-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.9/PKG-INFO` & `snet_contracts-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snet.contracts
-Version: 0.0.9
+Version: 0.1.0
 Summary: SingularityNET Ecosystem Contracts
 Home-page: https://github.com/singnet/snet-ecosystem-contracts
 Author: SingularityNET Foundation
 Author-email: info@singularitynet.io
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `snet.contracts-0.0.9/README.md` & `snet_contracts-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.9/setup.py` & `snet_contracts-0.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,9 +22,10 @@
     description='SingularityNET Ecosystem Contracts',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     python_requires='>=3.10',
     install_requires=[
         'web3==6.11.1',
-    ]
+    ],
+    include_package_data=True
 )
```

### Comparing `snet.contracts-0.0.9/snet/contracts/resources/abi/MultiPartyEscrow.json` & `snet_contracts-0.1.0/snet/contracts/resources/abi/MultiPartyEscrow.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.9/snet/contracts/resources/abi/Registry.json` & `snet_contracts-0.1.0/snet/contracts/resources/abi/Registry.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.9/snet/contracts/resources/abi/SingularityNetToken.json` & `snet_contracts-0.1.0/snet/contracts/resources/abi/SingularityNetToken.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.9/snet/contracts/resources/abi/TokenConversionManager.json` & `snet_contracts-0.1.0/snet/contracts/resources/abi/TokenConversionManager.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.9/snet/contracts/resources/abi/TokenStake.json` & `snet_contracts-0.1.0/snet/contracts/resources/abi/TokenStake.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.9/snet/contracts/resources/bytecode/MultiPartyEscrow.json` & `snet_contracts-0.1.0/snet/contracts/resources/bytecode/MultiPartyEscrow.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.9/snet/contracts/resources/bytecode/Registry.json` & `snet_contracts-0.1.0/snet/contracts/resources/bytecode/Registry.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.9/snet/contracts/resources/bytecode/SingularityNetToken.json` & `snet_contracts-0.1.0/snet/contracts/resources/bytecode/SingularityNetToken.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.9/snet/contracts/resources/bytecode/TokenConversionManager.json` & `snet_contracts-0.1.0/snet/contracts/resources/bytecode/TokenConversionManager.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.9/snet/contracts/resources/bytecode/TokenStake.json` & `snet_contracts-0.1.0/snet/contracts/resources/bytecode/TokenStake.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.9/snet/contracts/resources/networks/MultiPartyEscrow.json` & `snet_contracts-0.1.0/snet/contracts/resources/networks/MultiPartyEscrow.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.9/snet/contracts/resources/networks/Registry.json` & `snet_contracts-0.1.0/snet/contracts/resources/networks/Registry.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.9/snet/contracts/resources/networks/SingularityNetToken.json` & `snet_contracts-0.1.0/snet/contracts/resources/networks/SingularityNetToken.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.9/snet/contracts/resources/networks/TokenStake.json` & `snet_contracts-0.1.0/snet/contracts/resources/networks/TokenStake.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.9/snet/contracts/resources/networks/converter/AGIX/TokenConversionManager.json` & `snet_contracts-0.1.0/snet/contracts/resources/networks/converter/AGIX/TokenConversionManager.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.9/snet/contracts/resources/networks/converter/CGV/TokenConversionManager.json` & `snet_contracts-0.1.0/snet/contracts/resources/networks/converter/CGV/TokenConversionManager.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.9/snet/contracts/resources/networks/converter/NTX/TokenConversionManager.json` & `snet_contracts-0.1.0/snet/contracts/resources/networks/converter/NTX/TokenConversionManager.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.9/snet/contracts/resources/networks/converter/RJV/TokenConversionManager.json` & `snet_contracts-0.1.0/snet/contracts/resources/networks/converter/RJV/TokenConversionManager.json`

 * *Files identical despite different names*

### Comparing `snet.contracts-0.0.9/snet/contracts/utils.py` & `snet_contracts-0.1.0/snet/contracts/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 import os
-from pathlib import PurePath
+from pathlib import Path, PurePath
 from typing import Any
 
 from eth_typing import BlockNumber
 import web3
 
 from web3.contract.contract import Contract
 
-import snet.contracts as contracts
+from snet import contracts
 
 RESOURCES_PATH = PurePath(os.path.dirname(contracts.__file__)).joinpath("resources")
 
 
 def get_contract_object(w3: web3.Web3, contract_file: str, address: Any=None) -> Contract:
     with open(RESOURCES_PATH.joinpath("abi", f"{contract_file}.json")) as f:
         abi = json.load(f)
@@ -31,7 +31,25 @@
             txn_hash = networks[w3.net.version]["transactionHash"]
         return w3.eth.get_transaction_receipt(txn_hash).blockNumber
     except Exception:
         # TODO Hack as currenlty dependecy is on snet-cli so for test purpose return 0,need to remove dependecies from snet-cli ,currently very tightly coupled with it
         if w3.net.version in [1, 5, 11155111]:
             raise Exception("Transaction hash not found for deployed mpe contract")
         return 0
+
+
+def get_contract_def(contract_name, contract_artifacts_root=RESOURCES_PATH):
+    contract_def = {}
+    with open(Path(__file__).absolute().parent.joinpath(contract_artifacts_root, "abi",
+                                                        f"{contract_name}.json")) as f:
+        contract_def["abi"] = json.load(f)
+    if os.path.isfile(Path(__file__).absolute().parent.joinpath(contract_artifacts_root, "networks",
+                                                                f"{contract_name}.json")):
+        with open(Path(__file__).absolute().parent.joinpath(contract_artifacts_root, "networks",
+                                                            f"{contract_name}.json")) as f:
+            contract_def["networks"] = json.load(f)
+    return contract_def
+
+
+def get_all_abi_contract_files():
+    contracts = Path(RESOURCES_PATH.joinpath("abi")).glob("*json")
+    return [*contracts]
```

### Comparing `snet.contracts-0.0.9/snet.contracts.egg-info/PKG-INFO` & `snet_contracts-0.1.0/snet.contracts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snet.contracts
-Version: 0.0.9
+Version: 0.1.0
 Summary: SingularityNET Ecosystem Contracts
 Home-page: https://github.com/singnet/snet-ecosystem-contracts
 Author: SingularityNET Foundation
 Author-email: info@singularitynet.io
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `snet.contracts-0.0.9/snet.contracts.egg-info/SOURCES.txt` & `snet_contracts-0.1.0/snet.contracts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

