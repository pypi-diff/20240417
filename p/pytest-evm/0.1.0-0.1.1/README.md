# Comparing `tmp/pytest_evm-0.1.0.tar.gz` & `tmp/pytest_evm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_evm-0.1.0.tar", max compression
+gzip compressed data, was "pytest_evm-0.1.1.tar", max compression
```

## Comparing `pytest_evm-0.1.0.tar` & `pytest_evm-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1063 2024-01-24 19:16:03.258573 pytest_evm-0.1.0/LICENSE
--rw-r--r--   0        0        0     4209 2024-01-24 19:16:03.261582 pytest_evm-0.1.0/README.md
--rw-r--r--   0        0        0     1423 2024-01-24 19:18:13.120083 pytest_evm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      192 2024-01-24 18:08:51.851477 pytest_evm-0.1.0/pytest_evm/__init__.py
--rw-r--r--   0        0        0      759 2024-01-24 18:35:25.074374 pytest_evm-0.1.0/pytest_evm/fixtures.py
--rw-r--r--   0        0        0     1919 2024-01-24 18:07:08.297737 pytest_evm-0.1.0/pytest_evm/hooks.py
--rw-r--r--   0        0        0       62 2023-12-04 17:21:05.182141 pytest_evm-0.1.0/pytest_evm/pytest.ini
--rw-r--r--   0        0        0     1345 2023-12-25 09:57:43.223064 pytest_evm-0.1.0/pytest_evm/utils.py
--rw-r--r--   0        0        0     5437 1970-01-01 00:00:00.000000 pytest_evm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-01-24 19:16:03.258573 pytest_evm-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4209 2024-01-24 19:16:03.261582 pytest_evm-0.1.1/README.md
+-rw-r--r--   0        0        0     1448 2024-04-17 17:37:09.523443 pytest_evm-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      192 2024-01-24 18:08:51.851477 pytest_evm-0.1.1/pytest_evm/__init__.py
+-rw-r--r--   0        0        0      759 2024-01-24 18:35:25.074374 pytest_evm-0.1.1/pytest_evm/fixtures.py
+-rw-r--r--   0        0        0     1956 2024-04-17 17:38:49.298623 pytest_evm-0.1.1/pytest_evm/hooks.py
+-rw-r--r--   0        0        0       62 2023-12-04 17:21:05.182141 pytest_evm-0.1.1/pytest_evm/pytest.ini
+-rw-r--r--   0        0        0     1859 2024-04-17 17:31:49.858690 pytest_evm-0.1.1/pytest_evm/utils.py
+-rw-r--r--   0        0        0     5437 1970-01-01 00:00:00.000000 pytest_evm-0.1.1/PKG-INFO
```

### Comparing `pytest_evm-0.1.0/LICENSE` & `pytest_evm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_evm-0.1.0/README.md` & `pytest_evm-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest_evm-0.1.0/pyproject.toml` & `pytest_evm-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'pytest_evm'
-version = '0.1.0'
+version = '0.1.1'
 description = 'The testing package containing tools to test Web3-based projects'
 authors = ['Alexey <abelenkov2006@gmail.com>']
 license = 'MIT'
 readme = 'README.md'
 repository = 'https://github.com/blnkoff/pytest-evm'
 homepage = 'https://github.com/blnkoff/pytest-evm'
 classifiers = [
@@ -20,25 +20,26 @@
     'Operating System :: MacOS'
 ]
 packages = [{ include = 'pytest_evm' }]
 
 [tool.poetry.dependencies]
 python = '^3.11'
 web3 = "^6.12.0"
-pytest = "^7.4.3"
-pytest-asyncio = "^0.23.2"
-evm-wallet = "^1.1.1"
+evm-wallet = "^1.2.0"
 python-dotenv = {version = "^1.0.1", optional = true}
+pytest = "^8.1.1"
+pytest-asyncio = "^0.23.6"
 
 [tool.poetry.extras]
 dotenv = ["python-dotenv"]
 
 [tool.poetry.group.dev.dependencies]
 build = "^1.0.3"
 twine = "^4.0.2"
+python-dotenv = "^1.0.1"
 
 [build-system]
 requires = ['poetry-core']
 build-backend = 'poetry.core.masonry.api'
 
 [tool.poetry.plugins."pytest11"]
 evm_fixtures = 'pytest_evm.fixtures'
```

### Comparing `pytest_evm-0.1.0/pytest_evm/fixtures.py` & `pytest_evm-0.1.1/pytest_evm/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest_evm-0.1.0/pytest_evm/hooks.py` & `pytest_evm-0.1.1/pytest_evm/hooks.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,20 +29,21 @@
             pass
         else:
             if item.get_closest_marker("tx"):
                 try:
                     wallet = item.funcargs['wallet']
                     wallet = Wallet(wallet.private_key, wallet.network)
                     tx = get_last_transaction(wallet)
-                    last_tx_hash = tx['hash'].hex()
+                    last_tx_hash = tx['hash']
                     balance = get_balance(wallet)
                     costs = tx['value'] + tx['gas']*tx['gasPrice']
                     costs = Web3.from_wei(costs, 'ether')
                     print()
-                    print(f'From: https://goerli.etherscan.io/address/{wallet.public_key}')
+                    print(f'From: {wallet.public_key}')
                     print(f'Transaction: {wallet.get_explorer_url(last_tx_hash)}')
                     print(f'Costs: {costs} {wallet.network["token"]}')
                     print(f'Balance: {balance} {wallet.network["token"]}')
                     print(f'Network: {wallet.network["network"]}')
+                except TimeoutError as ex:
+                    print(ex)
                 except Exception as ex:
-                    print("There was an error while getting information about transaction")
-
+                    print(f"There was an error while getting information about transaction: {ex}")
```

### Comparing `pytest_evm-0.1.0/pytest_evm/utils.py` & `pytest_evm-0.1.1/pytest_evm/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,56 @@
+import time
 from functools import wraps
 from evm_wallet import Wallet
+from hexbytes import HexBytes
 from web3 import Web3
 from web3.middleware import geth_poa_middleware
 
 
 def validate_status(func):
     @wraps(func)
     async def wrapper(*args, **kwargs):
         wallet = kwargs['wallet']
         tx_hash = await func(*args, **kwargs)
-        status = bool(await wallet.provider.eth.wait_for_transaction_receipt(tx_hash))
+        status = (await wallet.provider.eth.wait_for_transaction_receipt(tx_hash)).get('status')
         assert status
 
     return wrapper
 
 
-def get_last_transaction(wallet: Wallet):
+def get_last_transaction(wallet: Wallet, timeout: float = 10):
     w3 = Web3(Web3.HTTPProvider(wallet.network['rpc']))
     w3.middleware_onion.inject(geth_poa_middleware, layer=0)
 
     block_number = w3.eth.block_number
     start_block = 0
     end_block = block_number
 
     last_transaction = None
     wallet_address = wallet.public_key
 
+    current_time = time.time()
+    deadline = current_time + timeout
     for block in range(end_block, start_block - 1, -1):
         block_info = w3.eth.get_block(block, True)
 
         for tx in reversed(block_info['transactions']):
-            if wallet_address.lower() in [tx['from'].lower(), tx['to'].lower()]:
-                last_transaction = tx
-                break
+            if time.time() > deadline:
+                raise TimeoutError(f'Timeout was exceeded for getting last transaction')
+            try:
+                from_address = tx['from'].lower()
+
+                if isinstance(from_address, HexBytes):
+                    from_address = from_address.hex()
+
+                if wallet_address.lower() == from_address.lower():
+                    last_transaction = tx
+                    break
+            except (AttributeError, KeyError):
+                continue
 
         if last_transaction:
             break
 
     return last_transaction
```

### Comparing `pytest_evm-0.1.0/PKG-INFO` & `pytest_evm-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_evm
-Version: 0.1.0
+Version: 0.1.1
 Summary: The testing package containing tools to test Web3-based projects
 Home-page: https://github.com/blnkoff/pytest-evm
 License: MIT
 Author: Alexey
 Author-email: abelenkov2006@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -16,17 +16,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 Provides-Extra: dotenv
-Requires-Dist: evm-wallet (>=1.1.1,<2.0.0)
-Requires-Dist: pytest (>=7.4.3,<8.0.0)
-Requires-Dist: pytest-asyncio (>=0.23.2,<0.24.0)
+Requires-Dist: evm-wallet (>=1.2.0,<2.0.0)
+Requires-Dist: pytest (>=8.1.1,<9.0.0)
+Requires-Dist: pytest-asyncio (>=0.23.6,<0.24.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0) ; extra == "dotenv"
 Requires-Dist: web3 (>=6.12.0,<7.0.0)
 Project-URL: Repository, https://github.com/blnkoff/pytest-evm
 Description-Content-Type: text/markdown
 
 # pytest-evm
```

