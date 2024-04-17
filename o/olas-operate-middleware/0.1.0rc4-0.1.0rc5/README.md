# Comparing `tmp/olas_operate_middleware-0.1.0rc4.tar.gz` & `tmp/olas_operate_middleware-0.1.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olas_operate_middleware-0.1.0rc4.tar", max compression
+gzip compressed data, was "olas_operate_middleware-0.1.0rc5.tar", max compression
```

## Comparing `olas_operate_middleware-0.1.0rc4.tar` & `olas_operate_middleware-0.1.0rc5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11339 2024-02-06 05:22:56.471559 olas_operate_middleware-0.1.0rc4/LICENSE
--rw-r--r--   0        0        0     4282 2024-03-05 05:48:41.164427 olas_operate_middleware-0.1.0rc4/README.md
--rw-r--r--   0        0        0      803 2024-02-27 08:48:06.011840 olas_operate_middleware-0.1.0rc4/operate/__init__.py
--rw-r--r--   0        0        0      804 2024-04-05 14:54:43.348635 olas_operate_middleware-0.1.0rc4/operate/account/__init__.py
--rw-r--r--   0        0        0     2109 2024-04-05 14:54:43.349000 olas_operate_middleware-0.1.0rc4/operate/account/user.py
--rw-r--r--   0        0        0    17479 2024-04-16 04:07:53.585535 olas_operate_middleware-0.1.0rc4/operate/cli.py
--rw-r--r--   0        0        0     1091 2024-02-27 08:48:06.012404 olas_operate_middleware-0.1.0rc4/operate/constants.py
--rw-r--r--   0        0        0      864 2024-03-08 10:47:59.399920 olas_operate_middleware-0.1.0rc4/operate/data/__init__.py
--rw-r--r--   0        0        0      809 2024-02-27 08:48:06.013275 olas_operate_middleware-0.1.0rc4/operate/data/contracts/__init__.py
--rw-r--r--   0        0        0      866 2024-02-27 08:48:06.013458 olas_operate_middleware-0.1.0rc4/operate/data/contracts/service_staking_token/__init__.py
--rw-r--r--   0        0        0    82730 2024-02-27 08:48:06.014051 olas_operate_middleware-0.1.0rc4/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json
--rw-r--r--   0        0        0     5847 2024-02-27 08:48:06.014506 olas_operate_middleware-0.1.0rc4/operate/data/contracts/service_staking_token/contract.py
--rw-r--r--   0        0        0      724 2024-02-27 08:48:06.014716 olas_operate_middleware-0.1.0rc4/operate/data/contracts/service_staking_token/contract.yaml
--rw-r--r--   0        0        0      868 2024-02-28 14:31:11.754886 olas_operate_middleware-0.1.0rc4/operate/data/contracts/uniswap_v2_erc20/__init__.py
--rw-r--r--   0        0        0    14169 2024-02-28 14:31:11.755175 olas_operate_middleware-0.1.0rc4/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json
--rw-r--r--   0        0        0     6985 2024-03-08 10:47:59.400374 olas_operate_middleware-0.1.0rc4/operate/data/contracts/uniswap_v2_erc20/contract.py
--rw-r--r--   0        0        0      741 2024-02-28 14:31:11.755543 olas_operate_middleware-0.1.0rc4/operate/data/contracts/uniswap_v2_erc20/contract.yaml
--rw-r--r--   0        0        0     4646 2024-03-14 12:31:10.592254 olas_operate_middleware-0.1.0rc4/operate/http/__init__.py
--rw-r--r--   0        0        0     1232 2024-02-27 08:48:06.014903 olas_operate_middleware-0.1.0rc4/operate/http/exceptions.py
--rw-r--r--   0        0        0     2809 2024-03-27 11:16:42.979679 olas_operate_middleware-0.1.0rc4/operate/keys.py
--rw-r--r--   0        0        0     2883 2024-04-16 04:14:40.060498 olas_operate_middleware-0.1.0rc4/operate/ledger/__init__.py
--rw-r--r--   0        0        0     1154 2024-03-08 10:47:59.401479 olas_operate_middleware-0.1.0rc4/operate/ledger/base.py
--rw-r--r--   0        0        0     1510 2024-03-08 10:47:59.401635 olas_operate_middleware-0.1.0rc4/operate/ledger/ethereum.py
--rw-r--r--   0        0        0     1610 2024-03-08 10:47:59.401789 olas_operate_middleware-0.1.0rc4/operate/ledger/profiles.py
--rw-r--r--   0        0        0     1199 2024-03-08 10:47:59.401953 olas_operate_middleware-0.1.0rc4/operate/ledger/solana.py
--rw-r--r--   0        0        0     3880 2024-04-05 14:54:43.350296 olas_operate_middleware-0.1.0rc4/operate/resource.py
--rw-r--r--   0        0        0      855 2024-03-27 11:16:42.980219 olas_operate_middleware-0.1.0rc4/operate/services/__init__.py
--rw-r--r--   0        0        0    16425 2024-04-11 14:01:32.695097 olas_operate_middleware-0.1.0rc4/operate/services/manage.py
--rw-r--r--   0        0        0    21677 2024-04-05 14:54:43.352503 olas_operate_middleware-0.1.0rc4/operate/services/protocol.py
--rw-r--r--   0        0        0    13695 2024-04-16 04:14:40.061038 olas_operate_middleware-0.1.0rc4/operate/services/service.py
--rw-r--r--   0        0        0     5357 2024-04-05 14:54:43.352823 olas_operate_middleware-0.1.0rc4/operate/types.py
--rw-r--r--   0        0        0      808 2024-04-05 14:54:43.353285 olas_operate_middleware-0.1.0rc4/operate/utils/__init__.py
--rw-r--r--   0        0        0     6082 2024-04-05 14:54:43.353744 olas_operate_middleware-0.1.0rc4/operate/utils/gnosis.py
--rw-r--r--   0        0        0      813 2024-04-05 14:54:43.353950 olas_operate_middleware-0.1.0rc4/operate/wallet/__init__.py
--rw-r--r--   0        0        0     8662 2024-04-15 16:15:46.952707 olas_operate_middleware-0.1.0rc4/operate/wallet/master.py
--rw-r--r--   0        0        0      818 2024-04-16 04:17:39.321459 olas_operate_middleware-0.1.0rc4/pyproject.toml
--rw-r--r--   0        0        0     5122 1970-01-01 00:00:00.000000 olas_operate_middleware-0.1.0rc4/PKG-INFO
+-rw-r--r--   0        0        0    11339 2024-02-06 05:22:56.471559 olas_operate_middleware-0.1.0rc5/LICENSE
+-rw-r--r--   0        0        0     4282 2024-03-05 05:48:41.164427 olas_operate_middleware-0.1.0rc5/README.md
+-rw-r--r--   0        0        0      803 2024-02-27 08:48:06.011840 olas_operate_middleware-0.1.0rc5/operate/__init__.py
+-rw-r--r--   0        0        0      804 2024-04-05 14:54:43.348635 olas_operate_middleware-0.1.0rc5/operate/account/__init__.py
+-rw-r--r--   0        0        0     2109 2024-04-05 14:54:43.349000 olas_operate_middleware-0.1.0rc5/operate/account/user.py
+-rw-r--r--   0        0        0    18550 2024-04-17 09:26:07.366152 olas_operate_middleware-0.1.0rc5/operate/cli.py
+-rw-r--r--   0        0        0     1091 2024-02-27 08:48:06.012404 olas_operate_middleware-0.1.0rc5/operate/constants.py
+-rw-r--r--   0        0        0      864 2024-03-08 10:47:59.399920 olas_operate_middleware-0.1.0rc5/operate/data/__init__.py
+-rw-r--r--   0        0        0      809 2024-02-27 08:48:06.013275 olas_operate_middleware-0.1.0rc5/operate/data/contracts/__init__.py
+-rw-r--r--   0        0        0      866 2024-02-27 08:48:06.013458 olas_operate_middleware-0.1.0rc5/operate/data/contracts/service_staking_token/__init__.py
+-rw-r--r--   0        0        0    82730 2024-02-27 08:48:06.014051 olas_operate_middleware-0.1.0rc5/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json
+-rw-r--r--   0        0        0     5847 2024-02-27 08:48:06.014506 olas_operate_middleware-0.1.0rc5/operate/data/contracts/service_staking_token/contract.py
+-rw-r--r--   0        0        0      724 2024-02-27 08:48:06.014716 olas_operate_middleware-0.1.0rc5/operate/data/contracts/service_staking_token/contract.yaml
+-rw-r--r--   0        0        0      868 2024-02-28 14:31:11.754886 olas_operate_middleware-0.1.0rc5/operate/data/contracts/uniswap_v2_erc20/__init__.py
+-rw-r--r--   0        0        0    14169 2024-02-28 14:31:11.755175 olas_operate_middleware-0.1.0rc5/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json
+-rw-r--r--   0        0        0     6985 2024-03-08 10:47:59.400374 olas_operate_middleware-0.1.0rc5/operate/data/contracts/uniswap_v2_erc20/contract.py
+-rw-r--r--   0        0        0      741 2024-02-28 14:31:11.755543 olas_operate_middleware-0.1.0rc5/operate/data/contracts/uniswap_v2_erc20/contract.yaml
+-rw-r--r--   0        0        0     4646 2024-03-14 12:31:10.592254 olas_operate_middleware-0.1.0rc5/operate/http/__init__.py
+-rw-r--r--   0        0        0     1232 2024-02-27 08:48:06.014903 olas_operate_middleware-0.1.0rc5/operate/http/exceptions.py
+-rw-r--r--   0        0        0     2809 2024-03-27 11:16:42.979679 olas_operate_middleware-0.1.0rc5/operate/keys.py
+-rw-r--r--   0        0        0     3301 2024-04-17 09:26:07.366847 olas_operate_middleware-0.1.0rc5/operate/ledger/__init__.py
+-rw-r--r--   0        0        0     1154 2024-03-08 10:47:59.401479 olas_operate_middleware-0.1.0rc5/operate/ledger/base.py
+-rw-r--r--   0        0        0     1510 2024-03-08 10:47:59.401635 olas_operate_middleware-0.1.0rc5/operate/ledger/ethereum.py
+-rw-r--r--   0        0        0     1610 2024-03-08 10:47:59.401789 olas_operate_middleware-0.1.0rc5/operate/ledger/profiles.py
+-rw-r--r--   0        0        0     1199 2024-03-08 10:47:59.401953 olas_operate_middleware-0.1.0rc5/operate/ledger/solana.py
+-rw-r--r--   0        0        0     3880 2024-04-05 14:54:43.350296 olas_operate_middleware-0.1.0rc5/operate/resource.py
+-rw-r--r--   0        0        0      855 2024-03-27 11:16:42.980219 olas_operate_middleware-0.1.0rc5/operate/services/__init__.py
+-rw-r--r--   0        0        0    17523 2024-04-17 09:26:07.367524 olas_operate_middleware-0.1.0rc5/operate/services/manage.py
+-rw-r--r--   0        0        0    21677 2024-04-05 14:54:43.352503 olas_operate_middleware-0.1.0rc5/operate/services/protocol.py
+-rw-r--r--   0        0        0    13695 2024-04-16 04:14:40.061038 olas_operate_middleware-0.1.0rc5/operate/services/service.py
+-rw-r--r--   0        0        0     5357 2024-04-05 14:54:43.352823 olas_operate_middleware-0.1.0rc5/operate/types.py
+-rw-r--r--   0        0        0      808 2024-04-05 14:54:43.353285 olas_operate_middleware-0.1.0rc5/operate/utils/__init__.py
+-rw-r--r--   0        0        0     6082 2024-04-05 14:54:43.353744 olas_operate_middleware-0.1.0rc5/operate/utils/gnosis.py
+-rw-r--r--   0        0        0      813 2024-04-05 14:54:43.353950 olas_operate_middleware-0.1.0rc5/operate/wallet/__init__.py
+-rw-r--r--   0        0        0     8662 2024-04-16 14:21:46.519007 olas_operate_middleware-0.1.0rc5/operate/wallet/master.py
+-rw-r--r--   0        0        0     1171 2024-04-17 09:26:07.371553 olas_operate_middleware-0.1.0rc5/pyproject.toml
+-rw-r--r--   0        0        0     5668 1970-01-01 00:00:00.000000 olas_operate_middleware-0.1.0rc5/PKG-INFO
```

### Comparing `olas_operate_middleware-0.1.0rc4/LICENSE` & `olas_operate_middleware-0.1.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/README.md` & `olas_operate_middleware-0.1.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/__init__.py` & `olas_operate_middleware-0.1.0rc5/operate/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/account/__init__.py` & `olas_operate_middleware-0.1.0rc5/operate/account/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/account/user.py` & `olas_operate_middleware-0.1.0rc5/operate/account/user.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/cli.py` & `olas_operate_middleware-0.1.0rc5/operate/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 # ------------------------------------------------------------------------------
 
 """Operate app CLI module."""
 
+import asyncio
 import logging
 import os
 import traceback
 import typing as t
 from pathlib import Path
 
 from aea.helpers.logging import setup_logger
@@ -121,22 +122,24 @@
 def create_app(  # pylint: disable=too-many-locals, unused-argument, too-many-statements
     home: t.Optional[Path] = None,
 ) -> FastAPI:
     """Create FastAPI object."""
 
     logger = setup_logger(name="operate")
     operate = OperateApp(home=home, logger=logger)
-    app = FastAPI()
 
+    app = FastAPI()
     app.add_middleware(
         CORSMiddleware,
         allow_origins=["*"],
         allow_methods=["GET", "POST", "PUT", "DELETE"],
     )
 
+    funding_jobs: t.Dict[str, asyncio.Task] = {}
+
     def with_retries(f: t.Callable) -> t.Callable:
         """Retries decorator."""
 
         async def _call(request: Request) -> JSONResponse:
             """Call the endpoint."""
             logger.info(f"Calling `{f.__name__}` with retries enabled")
             retries = 0
@@ -329,14 +332,24 @@
         )
         if template.get("deploy", False):
             manager = operate.service_manager()
             manager.deploy_service_onchain(hash=service.hash)
             manager.stake_service_on_chain(hash=service.hash)
             manager.fund_service(hash=service.hash)
             manager.deploy_service_locally(hash=service.hash)
+
+            # Start funding job
+            logger.info(f"Starting funding job for {service}")
+            loop = asyncio.get_running_loop()
+            funding_jobs[service.hash] = loop.create_task(
+                operate.service_manager().funding_job(
+                    hash=service.hash,
+                    loop=loop,
+                )
+            )
         return JSONResponse(
             content=operate.service_manager().create_or_load(hash=service.hash).json
         )
 
     @app.put("/api/services")
     @with_retries
     async def _update_services(request: Request) -> JSONResponse:
@@ -350,14 +363,23 @@
         )
         if template.get("deploy", False):
             manager = operate.service_manager()
             manager.deploy_service_onchain(hash=service.hash)
             manager.stake_service_on_chain(hash=service.hash)
             manager.fund_service(hash=service.hash)
             manager.deploy_service_locally(hash=service.hash)
+
+            logger.info(f"Starting funding job for {service}")
+            loop = asyncio.get_running_loop()
+            funding_jobs[service.hash] = loop.create_task(
+                operate.service_manager().funding_job(
+                    hash=service.hash,
+                    loop=loop,
+                )
+            )
         return JSONResponse(content=service.json)
 
     @app.get("/api/services/{service}")
     @with_retries
     async def _get_service(request: Request) -> JSONResponse:
         """Create a service."""
         return JSONResponse(
@@ -439,38 +461,42 @@
         deployment.build(force=True)
         return JSONResponse(content=deployment.json)
 
     @app.post("/api/services/{service}/deployment/start")
     @with_retries
     async def _start_service_locally(request: Request) -> JSONResponse:
         """Create a service."""
-        deployment = (
-            operate.service_manager()
-            .create_or_load(
-                request.path_params["service"],
-            )
-            .deployment
-        )
+        service = request.path_params["service"]
+        deployment = operate.service_manager().create_or_load(service).deployment
+        operate.service_manager().fund_service(service)
         deployment.build(force=True)
-        operate.service_manager().fund_service(hash=request.path_params["service"])
         deployment.start()
+
+        # Start funding job
+        loop = asyncio.get_running_loop()
+        funding_jobs[service] = loop.create_task(
+            operate.service_manager().funding_job(
+                hash=service,
+                loop=loop,
+            )
+        )
         return JSONResponse(content=deployment.json)
 
     @app.post("/api/services/{service}/deployment/stop")
     @with_retries
     async def _stop_service_locally(request: Request) -> JSONResponse:
         """Create a service."""
-        deployment = (
-            operate.service_manager()
-            .create_or_load(
-                request.path_params["service"],
-            )
-            .deployment
-        )
+        service = request.path_params["service"]
+        deployment = operate.service_manager().create_or_load(service).deployment
         deployment.stop()
+
+        logger.info(f"Cancelling funding job for {service}")
+        status = funding_jobs[service].cancel()
+        if not status:
+            logger.info(f"Funding job cancellation for {service} failed")
         return JSONResponse(content=deployment.json)
 
     @app.post("/api/services/{service}/deployment/delete")
     @with_retries
     async def _delete_service_locally(request: Request) -> JSONResponse:
         """Create a service."""
         # TODO: Drain safe before deleting service
```

### Comparing `olas_operate_middleware-0.1.0rc4/operate/constants.py` & `olas_operate_middleware-0.1.0rc5/operate/constants.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/data/__init__.py` & `olas_operate_middleware-0.1.0rc5/operate/data/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/data/contracts/__init__.py` & `olas_operate_middleware-0.1.0rc5/operate/data/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/data/contracts/service_staking_token/__init__.py` & `olas_operate_middleware-0.1.0rc5/operate/data/contracts/service_staking_token/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json` & `olas_operate_middleware-0.1.0rc5/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/data/contracts/service_staking_token/contract.py` & `olas_operate_middleware-0.1.0rc5/operate/data/contracts/service_staking_token/contract.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/data/contracts/service_staking_token/contract.yaml` & `olas_operate_middleware-0.1.0rc5/operate/data/contracts/service_staking_token/contract.yaml`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/data/contracts/uniswap_v2_erc20/__init__.py` & `olas_operate_middleware-0.1.0rc5/operate/data/contracts/uniswap_v2_erc20/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json` & `olas_operate_middleware-0.1.0rc5/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/data/contracts/uniswap_v2_erc20/contract.py` & `olas_operate_middleware-0.1.0rc5/operate/data/contracts/uniswap_v2_erc20/contract.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/data/contracts/uniswap_v2_erc20/contract.yaml` & `olas_operate_middleware-0.1.0rc5/operate/data/contracts/uniswap_v2_erc20/contract.yaml`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/http/__init__.py` & `olas_operate_middleware-0.1.0rc5/operate/http/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/http/exceptions.py` & `olas_operate_middleware-0.1.0rc5/operate/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/keys.py` & `olas_operate_middleware-0.1.0rc5/operate/keys.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/ledger/__init__.py` & `olas_operate_middleware-0.1.0rc5/operate/ledger/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,21 +24,32 @@
 
 from operate.ledger.base import LedgerHelper
 from operate.ledger.ethereum import Ethereum
 from operate.ledger.solana import Solana
 from operate.types import ChainType, LedgerType
 
 
+ETHEREUM_PUBLIC_RPC = "https://ethereum.publicnode.com"
+GNOSIS_PUBLIC_RPC = "https://gnosis-rpc.publicnode.com"
+GOERLI_PUBLIC_RPC = "https://ethereum-goerli.publicnode.com"
+SOLANA_PUBLIC_RPC = "https://api.mainnet-beta.solana.com"
+
 ETHEREUM_RPC = os.environ.get("DEV_RPC", "https://ethereum.publicnode.com")
 GNOSIS_RPC = os.environ.get(
     "DEV_RPC", "https://go.getblock.io/2a1fa1ade5d547ca86eab099c35ce2a7"
 )
 GOERLI_RPC = os.environ.get("DEV_RPC", "https://ethereum-goerli.publicnode.com")
 SOLANA_RPC = os.environ.get("DEV_RPC", "https://api.mainnet-beta.solana.com")
 
+PUBLIC_RPCS = {
+    ChainType.ETHEREUM: ETHEREUM_PUBLIC_RPC,
+    ChainType.GNOSIS: GNOSIS_PUBLIC_RPC,
+    ChainType.GOERLI: GOERLI_PUBLIC_RPC,
+    ChainType.SOLANA: SOLANA_PUBLIC_RPC,
+}
 
 DEFAULT_RPCS = {
     ChainType.ETHEREUM: ETHEREUM_RPC,
     ChainType.GNOSIS: GNOSIS_RPC,
     ChainType.GOERLI: GOERLI_RPC,
     ChainType.SOLANA: SOLANA_RPC,
 }
```

### Comparing `olas_operate_middleware-0.1.0rc4/operate/ledger/base.py` & `olas_operate_middleware-0.1.0rc5/operate/ledger/base.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/ledger/ethereum.py` & `olas_operate_middleware-0.1.0rc5/operate/ledger/ethereum.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/ledger/profiles.py` & `olas_operate_middleware-0.1.0rc5/operate/ledger/profiles.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/ledger/solana.py` & `olas_operate_middleware-0.1.0rc5/operate/ledger/solana.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/resource.py` & `olas_operate_middleware-0.1.0rc5/operate/resource.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/services/__init__.py` & `olas_operate_middleware-0.1.0rc5/operate/services/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/services/manage.py` & `olas_operate_middleware-0.1.0rc5/operate/services/manage.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,23 +15,26 @@
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 # ------------------------------------------------------------------------------
 """Service manager."""
 
+import asyncio
 import logging
 import typing as t
+from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
 
 from aea.helpers.base import IPFSHash
 from aea.helpers.logging import setup_logger
 from autonomy.chain.base import registry_contracts
 
 from operate.keys import Key, KeysManager
+from operate.ledger import PUBLIC_RPCS
 from operate.ledger.profiles import CONTRACTS, OLAS, STAKING
 from operate.services.protocol import OnChainManager
 from operate.services.service import (
     Deployment,
     OnChainData,
     OnChainState,
     OnChainUserParams,
@@ -351,20 +354,29 @@
         ocm.unstake(
             service_id=service.chain_data.token,
             staking_contract=STAKING[service.ledger_config.chain],
         )
         service.chain_data.staked = False
         service.store()
 
-    def fund_service(self, hash: str) -> None:
+    def fund_service(
+        self,
+        hash: str,
+        rpc: t.Optional[str] = None,
+        agent_fund_requirement: t.Optional[float] = None,
+        safe_fund_requirement: t.Optional[float] = None,
+    ) -> None:
         """Fund service if required."""
         service = self.create_or_load(hash=hash)
         wallet = self.wallet_manager.load(ledger_type=service.ledger_config.type)
-        ledger_api = wallet.ledger_api(chain_type=service.ledger_config.chain)
-        agent_fund_requirement = service.chain_data.user_params.fund_requirements.agent
+        ledger_api = wallet.ledger_api(chain_type=service.ledger_config.chain, rpc=rpc)
+        agent_fund_requirement = (
+            agent_fund_requirement
+            or service.chain_data.user_params.fund_requirements.agent
+        )
 
         for key in service.keys:
             agent_balance = ledger_api.get_balance(address=key.address)
             self.logger.info(f"Agent {key.address} balance: {agent_balance}")
             self.logger.info(f"Required balance: {agent_fund_requirement}")
             if agent_balance < agent_fund_requirement:
                 self.logger.info("Funding agents")
@@ -373,29 +385,52 @@
                 wallet.transfer(
                     to=key.address,
                     amount=to_transfer,
                     chain_type=service.ledger_config.chain,
                 )
 
         safe_balanace = ledger_api.get_balance(service.chain_data.multisig)
-        safe_fund_requirement = service.chain_data.user_params.fund_requirements.safe
+        safe_fund_requirement = (
+            safe_fund_requirement
+            or service.chain_data.user_params.fund_requirements.safe
+        )
         self.logger.info(f"Safe {service.chain_data.multisig} balance: {safe_balanace}")
         self.logger.info(f"Required balance: {safe_fund_requirement}")
         if safe_balanace < safe_fund_requirement:
             self.logger.info("Funding safe")
             to_transfer = safe_fund_requirement - safe_balanace
             self.logger.info(
                 f"Transferring {to_transfer} units to {service.chain_data.multisig}"
             )
             wallet.transfer(
                 to=t.cast(str, service.chain_data.multisig),
                 amount=to_transfer,
                 chain_type=service.ledger_config.chain,
             )
 
+    async def funding_job(
+        self,
+        hash: str,
+        loop: t.Optional[asyncio.AbstractEventLoop] = None,
+    ) -> None:
+        """Start a background funding job."""
+        loop = loop or asyncio.get_event_loop()
+        service = self.create_or_load(hash=hash)
+        with ThreadPoolExecutor() as executor:
+            while True:
+                await loop.run_in_executor(
+                    executor,
+                    self.fund_service,
+                    hash,
+                    PUBLIC_RPCS[service.ledger_config.chain],
+                    10000000000000000,
+                    50000000000000000,
+                )
+                await asyncio.sleep(60)
+
     def deploy_service_locally(self, hash: str, force: bool = True) -> Deployment:
         """
         Deploy service locally
 
         :param hash: Service hash
         :param force: Remove previous deployment and start a new one.
         """
```

### Comparing `olas_operate_middleware-0.1.0rc4/operate/services/protocol.py` & `olas_operate_middleware-0.1.0rc5/operate/services/protocol.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/services/service.py` & `olas_operate_middleware-0.1.0rc5/operate/services/service.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/types.py` & `olas_operate_middleware-0.1.0rc5/operate/types.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/utils/__init__.py` & `olas_operate_middleware-0.1.0rc5/operate/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/utils/gnosis.py` & `olas_operate_middleware-0.1.0rc5/operate/utils/gnosis.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/wallet/__init__.py` & `olas_operate_middleware-0.1.0rc5/operate/wallet/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/operate/wallet/master.py` & `olas_operate_middleware-0.1.0rc5/operate/wallet/master.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc4/PKG-INFO` & `olas_operate_middleware-0.1.0rc5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,43 @@
 Metadata-Version: 2.1
 Name: olas-operate-middleware
-Version: 0.1.0rc4
+Version: 0.1.0rc5
 Summary: 
 Author: David Vilela
 Author-email: dvilelaf@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: clea (>=0.1.0rc4)
+Requires-Dist: clea (==0.1.0rc4)
+Requires-Dist: cytoolz (==0.12.3)
 Requires-Dist: docker (==6.1.2)
-Requires-Dist: fastapi (>=0.110.0)
-Requires-Dist: open-aea-ledger-ethereum (>=1.50.0)
-Requires-Dist: open-autonomy (>=0.14.10)
+Requires-Dist: eth-abi (==5.1.0)
+Requires-Dist: eth-account (==0.8.0)
+Requires-Dist: eth-hash (==0.7.0)
+Requires-Dist: eth-keyfile (==0.6.1)
+Requires-Dist: eth-keys (==0.4.0)
+Requires-Dist: eth-rlp (==0.3.0)
+Requires-Dist: eth-typing (==3.5.2)
+Requires-Dist: eth-utils (==2.3.1)
+Requires-Dist: fastapi (==0.110.0)
+Requires-Dist: frozenlist (==1.4.1)
+Requires-Dist: hexbytes (==0.3.1)
+Requires-Dist: ipfshttpclient (==0.8.0a2)
+Requires-Dist: jsonschema (==4.3.3)
+Requires-Dist: multidict (==6.0.5)
+Requires-Dist: open-aea-cli-ipfs (==1.51.0)
+Requires-Dist: open-aea-ledger-ethereum (==1.51.0)
+Requires-Dist: open-autonomy (==0.14.11.post1)
 Requires-Dist: requests-toolbelt (==1.0.0)
-Requires-Dist: starlette (>=0.36.3)
-Requires-Dist: uvicorn (>=0.27.0)
+Requires-Dist: starlette (==0.36.3)
+Requires-Dist: uvicorn (==0.27.0)
 Requires-Dist: web3 (==6.1.0)
 Description-Content-Type: text/markdown
 
 # Olas Operate
 Electron + NextJS + Python Backend application to one-click run Agents.
 
 ## Technologies Used
```

